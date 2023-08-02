# Comparing `tmp/sphinx-7.1.1.tar.gz` & `tmp/sphinx-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-7.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx-7.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx-7.1.1.tar` & `sphinx-7.1.2.tar`

### file list

```diff
@@ -1,1627 +1,1627 @@
--rw-r--r--   0        0        0     3818 2023-07-27 20:41:02.979620 sphinx-7.1.1/AUTHORS
--rw-r--r--   0        0        0   374191 2023-07-27 20:41:02.979620 sphinx-7.1.1/CHANGES
--rw-r--r--   0        0        0     3530 2023-07-27 20:41:02.979620 sphinx-7.1.1/CODE_OF_CONDUCT
--rw-r--r--   0        0        0    26147 2023-07-27 20:41:02.979620 sphinx-7.1.1/EXAMPLES
--rw-r--r--   0        0        0     3135 2023-07-27 20:41:02.979620 sphinx-7.1.1/LICENSE
--rw-r--r--   0        0        0     2323 2023-07-27 20:41:02.979620 sphinx-7.1.1/README.rst
--rw-r--r--   0        0        0      607 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/Makefile
--rw-r--r--   0        0        0      152 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/Makefile
--rw-r--r--   0        0        0    27523 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/bookcover.png
--rw-r--r--   0        0        0     9875 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/conf.py.txt
--rw-r--r--   0        0        0     3307 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/favicon.svg
--rw-r--r--   0        0        0     1351 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/more.png
--rw-r--r--   0        0        0    34213 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/sphinx.png
--rw-r--r--   0        0        0    25792 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/themes/agogo.png
--rw-r--r--   0        0        0    32356 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/themes/alabaster.png
--rw-r--r--   0        0        0    27139 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/themes/bizstyle.png
--rw-r--r--   0        0        0    39927 2023-07-27 20:41:02.979620 sphinx-7.1.1/doc/_static/themes/classic.png
--rw-r--r--   0        0        0    56954 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/agogo.png
--rw-r--r--   0        0        0    40248 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/alabaster.png
--rw-r--r--   0        0        0    75192 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/bizstyle.png
--rw-r--r--   0        0        0    72597 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/classic.png
--rw-r--r--   0        0        0    84200 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/haiku.png
--rw-r--r--   0        0        0    32266 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/nature.png
--rw-r--r--   0        0        0   102717 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/pyramid.png
--rw-r--r--   0        0        0    88111 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/scrolls.png
--rw-r--r--   0        0        0    39411 2023-07-27 20:41:02.983620 sphinx-7.1.1/doc/_static/themes/fullsize/sphinx_rtd_theme.png
--rw-r--r--   0        0        0    84439 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/fullsize/sphinxdoc.png
--rw-r--r--   0        0        0    91744 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/fullsize/traditional.png
--rw-r--r--   0        0        0    43184 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/haiku.png
--rw-r--r--   0        0        0    28536 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/nature.png
--rw-r--r--   0        0        0    38805 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/pyramid.png
--rw-r--r--   0        0        0    27800 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/scrolls.png
--rw-r--r--   0        0        0    29138 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/sphinx_rtd_theme.png
--rw-r--r--   0        0        0    30225 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/sphinxdoc.png
--rw-r--r--   0        0        0    32258 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/themes/traditional.png
--rw-r--r--   0        0        0    16371 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/translation.png
--rw-r--r--   0        0        0      342 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/translation.puml
--rw-r--r--   0        0        0     8232 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/translation.svg
--rw-r--r--   0        0        0    26500 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/tutorial/lumache-autosummary.png
--rw-r--r--   0        0        0    52126 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/tutorial/lumache-first-light.png
--rw-r--r--   0        0        0    51223 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/tutorial/lumache-furo.png
--rw-r--r--   0        0        0    71741 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/tutorial/lumache-py-function-full.png
--rw-r--r--   0        0        0    41828 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_static/tutorial/lumache-py-function.png
--rw-r--r--   0        0        0      225 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_templates/contents.html
--rw-r--r--   0        0        0     1860 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_themes/sphinx13/layout.html
--rw-r--r--   0        0        0     6552 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_themes/sphinx13/static/sphinx13.css
--rw-r--r--   0        0        0    11719 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_themes/sphinx13/static/sphinxheader.png
--rw-r--r--   0        0        0       60 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/_themes/sphinx13/theme.conf
--rw-r--r--   0        0        0       98 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/authors.rst
--rw-r--r--   0        0        0      400 2023-07-27 20:41:02.987620 sphinx-7.1.1/doc/changes.rst
--rw-r--r--   0        0        0     9027 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/conf.py
--rw-r--r--   0        0        0     1151 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/builders.rst
--rw-r--r--   0        0        0      649 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/index.rst
--rw-r--r--   0        0        0     1051 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/overview.rst
--rw-r--r--   0        0        0    15048 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/templating.rst
--rw-r--r--   0        0        0    12324 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/theming.rst
--rw-r--r--   0        0        0     4020 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/autodoc_ext.rst
--rw-r--r--   0        0        0      438 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/examples/README.rst
--rw-r--r--   0        0        0     1802 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/examples/autodoc_intenum.py
--rw-r--r--   0        0        0      400 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/examples/helloworld.py
--rw-r--r--   0        0        0     5030 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/examples/recipe.py
--rw-r--r--   0        0        0     3942 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/examples/todo.py
--rw-r--r--   0        0        0     5289 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/helloworld.rst
--rw-r--r--   0        0        0      262 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/index.rst
--rw-r--r--   0        0        0     8216 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/recipe.rst
--rw-r--r--   0        0        0    13435 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/development/tutorials/todo.rst
--rw-r--r--   0        0        0       54 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/examples.rst
--rw-r--r--   0        0        0    14235 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/appapi.rst
--rw-r--r--   0        0        0     1103 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/builderapi.rst
--rw-r--r--   0        0        0      165 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/collectorapi.rst
--rw-r--r--   0        0        0    40815 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/deprecated.rst
--rw-r--r--   0        0        0      518 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/domainapi.rst
--rw-r--r--   0        0        0     1043 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/envapi.rst
--rw-r--r--   0        0        0     2817 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/i18n.rst
--rw-r--r--   0        0        0     8597 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/index.rst
--rw-r--r--   0        0        0     2384 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/logging.rst
--rw-r--r--   0        0        0     4787 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/markupapi.rst
--rw-r--r--   0        0        0     1563 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/nodes.rst
--rw-r--r--   0        0        0     1243 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/parserapi.rst
--rw-r--r--   0        0        0      114 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/projectapi.rst
--rw-r--r--   0        0        0      943 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/extdev/utils.rst
--rw-r--r--   0        0        0    13425 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/faq.rst
--rw-r--r--   0        0        0     4173 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/glossary.rst
--rw-r--r--   0        0        0     3539 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/index.rst
--rw-r--r--   0        0        0       71 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/internals/code-of-conduct.rst
--rw-r--r--   0        0        0    11482 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/internals/contributing.rst
--rw-r--r--   0        0        0      353 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/internals/index.rst
--rw-r--r--   0        0        0     1964 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/internals/organization.rst
--rw-r--r--   0        0        0     4395 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/internals/release-process.rst
--rw-r--r--   0        0        0    69427 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/latex.rst
--rw-r--r--   0        0        0      784 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/make.bat
--rw-r--r--   0        0        0      314 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/man/index.rst
--rw-r--r--   0        0        0     4508 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/man/sphinx-apidoc.rst
--rw-r--r--   0        0        0     2122 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/man/sphinx-autogen.rst
--rw-r--r--   0        0        0    10673 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/man/sphinx-build.rst
--rw-r--r--   0        0        0     3692 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/man/sphinx-quickstart.rst
--rw-r--r--   0        0        0      806 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/support.rst
--rw-r--r--   0        0        0     4981 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/automatic-doc-generation.rst
--rw-r--r--   0        0        0    11036 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/deploying.rst
--rw-r--r--   0        0        0     9134 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/describing-code.rst
--rw-r--r--   0        0        0      240 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/end.rst
--rw-r--r--   0        0        0     3450 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/first-steps.rst
--rw-r--r--   0        0        0     3723 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/getting-started.rst
--rw-r--r--   0        0        0     1433 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/index.rst
--rw-r--r--   0        0        0     2528 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/more-sphinx-customization.rst
--rw-r--r--   0        0        0     4177 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/tutorial/narrative-documentation.rst
--rw-r--r--   0        0        0    11831 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/usage/advanced/intl.rst
--rw-r--r--   0        0        0     2670 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/usage/advanced/websupport/api.rst
--rw-r--r--   0        0        0      302 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/usage/advanced/websupport/index.rst
--rw-r--r--   0        0        0     9640 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/usage/advanced/websupport/quickstart.rst
--rw-r--r--   0        0        0     1368 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/usage/advanced/websupport/searchadapters.rst
--rw-r--r--   0        0        0     1231 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/usage/advanced/websupport/storagebackends.rst
--rw-r--r--   0        0        0    17742 2023-07-27 20:41:02.991620 sphinx-7.1.1/doc/usage/builders/index.rst
--rw-r--r--   0        0        0   103777 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/configuration.rst
--rw-r--r--   0        0        0    29861 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/autodoc.rst
--rw-r--r--   0        0        0     1899 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/autosectionlabel.rst
--rw-r--r--   0        0        0    11098 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/autosummary.rst
--rw-r--r--   0        0        0     1584 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/coverage.rst
--rw-r--r--   0        0        0    11838 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/doctest.rst
--rw-r--r--   0        0        0      404 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/duration.rst
--rw-r--r--   0        0        0     9665 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/example_google.py
--rw-r--r--   0        0        0      296 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/example_google.rst
--rw-r--r--   0        0        0     9714 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/example_numpy.py
--rw-r--r--   0        0        0      292 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/example_numpy.rst
--rw-r--r--   0        0        0     2781 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/extlinks.rst
--rw-r--r--   0        0        0      491 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/githubpages.rst
--rw-r--r--   0        0        0     6292 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/graphviz.rst
--rw-r--r--   0        0        0     1329 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/ifconfig.rst
--rw-r--r--   0        0        0     1705 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/imgconverter.rst
--rw-r--r--   0        0        0     2410 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/index.rst
--rw-r--r--   0        0        0     5594 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/inheritance.rst
--rw-r--r--   0        0        0     9934 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/intersphinx.rst
--rw-r--r--   0        0        0     1756 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/linkcode.rst
--rw-r--r--   0        0        0    11756 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/math.rst
--rw-r--r--   0        0        0    15980 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/napoleon.rst
--rw-r--r--   0        0        0     1644 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/todo.rst
--rw-r--r--   0        0        0     3748 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/extensions/viewcode.rst
--rw-r--r--   0        0        0      537 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/index.rst
--rw-r--r--   0        0        0     7146 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/installation.rst
--rw-r--r--   0        0        0     1584 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/markdown.rst
--rw-r--r--   0        0        0    13150 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/quickstart.rst
--rw-r--r--   0        0        0    20508 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/restructuredtext/basics.rst
--rw-r--r--   0        0        0    46040 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/restructuredtext/directives.rst
--rw-r--r--   0        0        0    68349 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/restructuredtext/domains.rst
--rw-r--r--   0        0        0     1967 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/restructuredtext/field-lists.rst
--rw-r--r--   0        0        0      574 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/restructuredtext/index.rst
--rw-r--r--   0        0        0    18409 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/restructuredtext/roles.rst
--rw-r--r--   0        0        0    14326 2023-07-27 20:41:02.995621 sphinx-7.1.1/doc/usage/theming.rst
--rw-r--r--   0        0        0    11978 2023-07-27 20:41:02.995621 sphinx-7.1.1/pyproject.toml
--rw-r--r--   0        0        0     1829 2023-07-27 20:41:02.995621 sphinx-7.1.1/sphinx/__init__.py
--rw-r--r--   0        0        0      103 2023-07-27 20:41:02.995621 sphinx-7.1.1/sphinx/__main__.py
--rw-r--r--   0        0        0    18542 2023-07-27 20:41:02.995621 sphinx-7.1.1/sphinx/addnodes.py
--rw-r--r--   0        0        0    56034 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/application.py
--rw-r--r--   0        0        0    26829 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/__init__.py
--rw-r--r--   0        0        0    28959 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/_epub_base.py
--rw-r--r--   0        0        0     6474 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/changes.py
--rw-r--r--   0        0        0     1504 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/dirhtml.py
--rw-r--r--   0        0        0      982 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/dummy.py
--rw-r--r--   0        0        0    11284 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/epub3.py
--rw-r--r--   0        0        0    11240 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/gettext.py
--rw-r--r--   0        0        0    59168 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/html/__init__.py
--rw-r--r--   0        0        0     2525 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/html/transforms.py
--rw-r--r--   0        0        0    24206 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/latex/__init__.py
--rw-r--r--   0        0        0     7365 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/latex/constants.py
--rw-r--r--   0        0        0      866 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/latex/nodes.py
--rw-r--r--   0        0        0     4445 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/latex/theming.py
--rw-r--r--   0        0        0    20998 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/latex/transforms.py
--rw-r--r--   0        0        0     1703 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/latex/util.py
--rw-r--r--   0        0        0    24525 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/linkcheck.py
--rw-r--r--   0        0        0     4511 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/manpage.py
--rw-r--r--   0        0        0     7425 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/singlehtml.py
--rw-r--r--   0        0        0     9666 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/texinfo.py
--rw-r--r--   0        0        0     2870 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/text.py
--rw-r--r--   0        0        0     3766 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/builders/xml.py
--rw-r--r--   0        0        0       44 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/cmd/__init__.py
--rw-r--r--   0        0        0    13671 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/cmd/build.py
--rw-r--r--   0        0        0     6552 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/cmd/make_mode.py
--rw-r--r--   0        0        0    23835 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/cmd/quickstart.py
--rw-r--r--   0        0        0    22727 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/config.py
--rw-r--r--   0        0        0     1816 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/deprecation.py
--rw-r--r--   0        0        0    13518 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/directives/__init__.py
--rw-r--r--   0        0        0    18354 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/directives/code.py
--rw-r--r--   0        0        0    14672 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/directives/other.py
--rw-r--r--   0        0        0     6781 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/directives/patches.py
--rw-r--r--   0        0        0    15270 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/domains/__init__.py
--rw-r--r--   0        0        0   151650 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/domains/c.py
--rw-r--r--   0        0        0     5524 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/domains/changeset.py
--rw-r--r--   0        0        0     5676 2023-07-27 20:41:02.999621 sphinx-7.1.1/sphinx/domains/citation.py
--rw-r--r--   0        0        0   330776 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/domains/cpp.py
--rw-r--r--   0        0        0     4140 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/domains/index.py
--rw-r--r--   0        0        0    18920 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/domains/javascript.py
--rw-r--r--   0        0        0     5459 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/domains/math.py
--rw-r--r--   0        0        0    70913 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/domains/python.py
--rw-r--r--   0        0        0    10366 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/domains/rst.py
--rw-r--r--   0        0        0    45842 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/domains/std.py
--rw-r--r--   0        0        0    30449 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/__init__.py
--rw-r--r--   0        0        0       34 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/adapters/__init__.py
--rw-r--r--   0        0        0      418 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/adapters/asset.py
--rw-r--r--   0        0        0     7503 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/adapters/indexentries.py
--rw-r--r--   0        0        0    16455 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/adapters/toctree.py
--rw-r--r--   0        0        0     2784 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/collectors/__init__.py
--rw-r--r--   0        0        0     6161 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/collectors/asset.py
--rw-r--r--   0        0        0     1887 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/collectors/dependencies.py
--rw-r--r--   0        0        0     2609 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/collectors/metadata.py
--rw-r--r--   0        0        0     2144 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/collectors/title.py
--rw-r--r--   0        0        0    15869 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/environment/collectors/toctree.py
--rw-r--r--   0        0        0     3388 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/errors.py
--rw-r--r--   0        0        0     4230 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/events.py
--rw-r--r--   0        0        0       57 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/__init__.py
--rw-r--r--   0        0        0    19197 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/apidoc.py
--rw-r--r--   0        0        0   114320 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autodoc/__init__.py
--rw-r--r--   0        0        0     5925 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autodoc/directive.py
--rw-r--r--   0        0        0    11371 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autodoc/importer.py
--rw-r--r--   0        0        0     5907 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autodoc/mock.py
--rw-r--r--   0        0        0     4664 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autodoc/preserve_defaults.py
--rw-r--r--   0        0        0     5406 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autodoc/type_comment.py
--rw-r--r--   0        0        0     7789 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autodoc/typehints.py
--rw-r--r--   0        0        0     2292 2023-07-27 20:41:03.003621 sphinx-7.1.1/sphinx/ext/autosectionlabel.py
--rw-r--r--   0        0        0    31056 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/autosummary/__init__.py
--rw-r--r--   0        0        0    26212 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/autosummary/generate.py
--rw-r--r--   0        0        0      106 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/autosummary/templates/autosummary/base.rst
--rw-r--r--   0        0        0      553 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/autosummary/templates/autosummary/class.rst
--rw-r--r--   0        0        0     1071 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/autosummary/templates/autosummary/module.rst
--rw-r--r--   0        0        0    14065 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/coverage.py
--rw-r--r--   0        0        0    22645 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/doctest.py
--rw-r--r--   0        0        0     2883 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/duration.py
--rw-r--r--   0        0        0     4523 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/extlinks.py
--rw-r--r--   0        0        0     1962 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/githubpages.py
--rw-r--r--   0        0        0    15843 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/graphviz.py
--rw-r--r--   0        0        0     2517 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/ifconfig.py
--rw-r--r--   0        0        0     3582 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/imgconverter.py
--rw-r--r--   0        0        0    15117 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/imgmath.py
--rw-r--r--   0        0        0    17031 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/inheritance_diagram.py
--rw-r--r--   0        0        0    28825 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/intersphinx.py
--rw-r--r--   0        0        0     2253 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/linkcode.py
--rw-r--r--   0        0        0     5182 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/mathjax.py
--rw-r--r--   0        0        0    17936 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/napoleon/__init__.py
--rw-r--r--   0        0        0    48417 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/napoleon/docstring.py
--rw-r--r--   0        0        0     8017 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/todo.py
--rw-r--r--   0        0        0    12900 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/ext/viewcode.py
--rw-r--r--   0        0        0     2995 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/extension.py
--rw-r--r--   0        0        0     6986 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/highlighting.py
--rw-r--r--   0        0        0     6148 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/io.py
--rw-r--r--   0        0        0     7107 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/jinja2glue.py
--rw-r--r--   0        0        0      165 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/locale/.tx/config
--rw-r--r--   0        0        0     7135 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/locale/__init__.py
--rw-r--r--   0        0        0     3494 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/locale/ar/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7688 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/locale/ar/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87237 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/locale/ar/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/locale/bg/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      492 2023-07-27 20:41:03.007621 sphinx-7.1.1/sphinx/locale/bg/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83916 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/bg/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     5977 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/bn/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7699 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/bn/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87859 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/bn/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4029 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/ca/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    84317 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/ca/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   123185 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/ca/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2385 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cak/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2391 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cak/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84630 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cak/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3976 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cs/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8071 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cs/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86669 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cs/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3411 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cy/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6018 2023-07-27 20:41:03.011621 sphinx-7.1.1/sphinx/locale/cy/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85933 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/cy/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3578 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/da/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    12705 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/da/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88403 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/da/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3533 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/de/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    11026 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/de/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88020 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/de/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      505 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/de_DE/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83929 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     8758 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/el/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    81252 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/el/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   131807 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/el/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      506 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_DE/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83930 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2302 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      462 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83929 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3630 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    76610 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   115479 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      508 2023-07-27 20:41:03.015621 sphinx-7.1.1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83932 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2457 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/eo/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     1864 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/eo/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84412 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/eo/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4155 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/es/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    81886 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/es/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   121969 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/es/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2342 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      546 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83970 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3615 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/et/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    33298 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/et/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    97534 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/et/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3102 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/eu/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6589 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/eu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86099 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/eu/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     7551 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/fa/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    98068 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/fa/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   139504 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/fa/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2787 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/fi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2912 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/fi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84716 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/fi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4162 2023-07-27 20:41:03.019621 sphinx-7.1.1/sphinx/locale/fr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    84318 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/fr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   124974 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/fr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2354 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      555 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83979 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4885 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/he/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     4905 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/he/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85734 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/he/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     7427 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    97733 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   146555 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      502 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83926 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3621 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    16774 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    90233 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3980 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hu/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    11338 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88363 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/hu/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3465 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/id/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    60908 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/id/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   109854 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/id/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2825 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/is/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     3082 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/is/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84836 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/is/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3579 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/it/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    10427 2023-07-27 20:41:03.023621 sphinx-7.1.1/sphinx/locale/it/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87816 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/it/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4957 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ja/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    86746 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ja/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   128634 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ja/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6108 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ka/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    74576 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ka/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   131640 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ka/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4807 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ko/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    83303 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ko/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   123022 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/ko/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3473 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/lt/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6907 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/lt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86276 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/lt/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3445 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/lv/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6585 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/lv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85991 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/lv/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2415 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/mk/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2011 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/mk/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84606 2023-07-27 20:41:03.027621 sphinx-7.1.1/sphinx/locale/mk/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3108 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6578 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85808 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6223 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ne/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8635 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ne/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88030 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ne/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3489 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/nl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    19033 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/nl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    91591 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/nl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3819 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    29289 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    96177 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2351 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      544 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83968 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4219 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    82142 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   121242 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3745 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7847 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86646 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3700 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ro/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8628 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ro/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86951 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ro/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     8165 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ru/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    15898 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ru/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    91959 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/ru/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3816 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/si/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     3560 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/si/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85398 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/si/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4117 2023-07-27 20:41:03.031621 sphinx-7.1.1/sphinx/locale/sk/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    67002 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sk/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   113035 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sk/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3185 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5228 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85484 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0    84079 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sphinx.pot
--rw-r--r--   0        0        0     4216 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sq/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    79775 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sq/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   120606 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sq/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4100 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     9193 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88044 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2380 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      584 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84008 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2382 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      579 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84003 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3281 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sv/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6568 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85829 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/sv/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/ta/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      647 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/ta/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84076 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/ta/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/te/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      489 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/te/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83913 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/te/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3937 2023-07-27 20:41:03.035621 sphinx-7.1.1/sphinx/locale/tr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    57535 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/tr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   109424 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/tr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6283 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6461 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86919 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/ur/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      487 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/ur/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83994 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/ur/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3520 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/vi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5771 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/vi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85912 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/vi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2294 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/yue/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      487 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/yue/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83911 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/yue/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4318 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    76477 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   115904 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2301 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      501 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83925 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2301 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      516 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    83940 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4451 2023-07-27 20:41:03.039621 sphinx-7.1.1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    74917 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   114627 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3098 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/parsers.py
--rw-r--r--   0        0        0     3432 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/project.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/py.typed
--rw-r--r--   0        0        0     5581 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/pycode/__init__.py
--rw-r--r--   0        0        0     6648 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/pycode/ast.py
--rw-r--r--   0        0        0    21346 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/pycode/parser.py
--rw-r--r--   0        0        0     2861 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/pygments_styles.py
--rw-r--r--   0        0        0    22138 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/registry.py
--rw-r--r--   0        0        0    15975 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/roles.py
--rw-r--r--   0        0        0    22183 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/__init__.py
--rw-r--r--   0        0        0     3561 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/da.py
--rw-r--r--   0        0        0     4637 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/de.py
--rw-r--r--   0        0        0     4899 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/en.py
--rw-r--r--   0        0        0     5723 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/es.py
--rw-r--r--   0        0        0     3207 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/fi.py
--rw-r--r--   0        0        0     3438 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/fr.py
--rw-r--r--   0        0        0     1949 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/hu.py
--rw-r--r--   0        0        0     5089 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/it.py
--rw-r--r--   0        0        0    30997 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/ja.py
--rw-r--r--   0        0        0     3594 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/base-stemmer.js
--rw-r--r--   0        0        0     3123 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/danish-stemmer.js
--rw-r--r--   0        0        0     5529 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/dutch-stemmer.js
--rw-r--r--   0        0        0     7529 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/finnish-stemmer.js
--rw-r--r--   0        0        0    11571 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/french-stemmer.js
--rw-r--r--   0        0        0     4669 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/german-stemmer.js
--rw-r--r--   0        0        0     6614 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/hungarian-stemmer.js
--rw-r--r--   0        0        0     9100 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/italian-stemmer.js
--rw-r--r--   0        0        0     2594 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/norwegian-stemmer.js
--rw-r--r--   0        0        0     6439 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/porter-stemmer.js
--rw-r--r--   0        0        0     8373 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/portuguese-stemmer.js
--rw-r--r--   0        0        0     8333 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/romanian-stemmer.js
--rw-r--r--   0        0        0     5735 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/russian-stemmer.js
--rw-r--r--   0        0        0     9121 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/spanish-stemmer.js
--rw-r--r--   0        0        0     2654 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/swedish-stemmer.js
--rw-r--r--   0        0        0    19972 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/minified-js/turkish-stemmer.js
--rw-r--r--   0        0        0     4571 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/nl.py
--rw-r--r--   0        0        0     4893 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/no.py
--rw-r--r--   0        0        0     8133 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/non-minified-js/base-stemmer.js
--rw-r--r--   0        0        0     8134 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/non-minified-js/danish-stemmer.js
--rw-r--r--   0        0        0    19495 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/non-minified-js/dutch-stemmer.js
--rw-r--r--   0        0        0    21286 2023-07-27 20:41:03.043621 sphinx-7.1.1/sphinx/search/non-minified-js/finnish-stemmer.js
--rw-r--r--   0        0        0    42080 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/french-stemmer.js
--rw-r--r--   0        0        0    17647 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/german-stemmer.js
--rw-r--r--   0        0        0    17564 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/hungarian-stemmer.js
--rw-r--r--   0        0        0    29065 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/italian-stemmer.js
--rw-r--r--   0        0        0     6870 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/norwegian-stemmer.js
--rw-r--r--   0        0        0    20391 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/porter-stemmer.js
--rw-r--r--   0        0        0    26718 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/portuguese-stemmer.js
--rw-r--r--   0        0        0    25006 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/romanian-stemmer.js
--rw-r--r--   0        0        0    17996 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/russian-stemmer.js
--rw-r--r--   0        0        0    28534 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/spanish-stemmer.js
--rw-r--r--   0        0        0     6851 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/swedish-stemmer.js
--rw-r--r--   0        0        0    77511 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/non-minified-js/turkish-stemmer.js
--rw-r--r--   0        0        0     4648 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/pt.py
--rw-r--r--   0        0        0      557 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/ro.py
--rw-r--r--   0        0        0     7905 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/ru.py
--rw-r--r--   0        0        0     3436 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/sv.py
--rw-r--r--   0        0        0      551 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/tr.py
--rw-r--r--   0        0        0     6146 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/search/zh.py
--rw-r--r--   0        0        0      196 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/apidoc/module.rst_t
--rw-r--r--   0        0        0     1173 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/apidoc/package.rst_t
--rw-r--r--   0        0        0      128 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/apidoc/toc.rst_t
--rw-r--r--   0        0        0      246 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/epub3/container.xml
--rw-r--r--   0        0        0     2127 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/epub3/content.opf_t
--rw-r--r--   0        0        0       20 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/epub3/mimetype
--rw-r--r--   0        0        0      629 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/epub3/nav.xhtml_t
--rw-r--r--   0        0        0      743 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/epub3/toc.ncx_t
--rw-r--r--   0        0        0      875 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/gettext/message.pot_t
--rw-r--r--   0        0        0      299 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/graphviz/graphviz.css
--rw-r--r--   0        0        0      864 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/htmlhelp/project.hhc
--rw-r--r--   0        0        0      570 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/htmlhelp/project.hhp
--rw-r--r--   0        0        0      165 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/htmlhelp/project.stp
--rw-r--r--   0        0        0      397 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/imgmath/preview.tex_t
--rw-r--r--   0        0        0      321 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/imgmath/template.tex_t
--rw-r--r--   0        0        0     2986 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/latex/latex.tex_t
--rw-r--r--   0        0        0     2156 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/latex/longtable.tex_t
--rw-r--r--   0        0        0      944 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/latex/sphinxmessages.sty_t
--rw-r--r--   0        0        0     1406 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/latex/tabular.tex_t
--rw-r--r--   0        0        0     1420 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/latex/tabulary.tex_t
--rw-r--r--   0        0        0      656 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/quickstart/Makefile.new_t
--rw-r--r--   0        0        0     4031 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/quickstart/Makefile_t
--rw-r--r--   0        0        0     2129 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/quickstart/conf.py_t
--rw-r--r--   0        0        0      787 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/quickstart/make.bat.new_t
--rw-r--r--   0        0        0     3293 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/quickstart/make.bat_t
--rw-r--r--   0        0        0      492 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/quickstart/root_doc.rst_t
--rw-r--r--   0        0        0     1423 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/templates/texinfo/Makefile
--rw-r--r--   0        0        0      171 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/testing/__init__.py
--rw-r--r--   0        0        0     2710 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/testing/comparer.py
--rw-r--r--   0        0        0     7508 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/testing/fixtures.py
--rw-r--r--   0        0        0     6317 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/testing/path.py
--rw-r--r--   0        0        0     1029 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/testing/restructuredtext.py
--rw-r--r--   0        0        0     7498 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/testing/util.py
--rw-r--r--   0        0        0     4366 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/LICRcyr2utf8.xdy
--rw-r--r--   0        0        0    10188 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/LICRlatin2utf8.xdy
--rw-r--r--   0        0        0    18890 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/LatinRules.xdy
--rw-r--r--   0        0        0     2401 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/Makefile_t
--rw-r--r--   0        0        0      695 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/latexmkjarc_t
--rw-r--r--   0        0        0     1104 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/latexmkrc_t
--rw-r--r--   0        0        0     1041 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/make.bat_t
--rw-r--r--   0        0        0      392 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/python.ist
--rw-r--r--   0        0        0    44560 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinx.sty
--rw-r--r--   0        0        0     9474 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinx.xdy
--rw-r--r--   0        0        0     3256 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxhowto.cls
--rw-r--r--   0        0        0    10989 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexadmonitions.sty
--rw-r--r--   0        0        0      901 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexcontainers.sty
--rw-r--r--   0        0        0     4840 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexgraphics.sty
--rw-r--r--   0        0        0     2066 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexindbibtoc.sty
--rw-r--r--   0        0        0     5139 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexlists.sty
--rw-r--r--   0        0        0    46048 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexliterals.sty
--rw-r--r--   0        0        0     4532 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexnumfig.sty
--rw-r--r--   0        0        0    14339 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexobjects.sty
--rw-r--r--   0        0        0     5066 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexshadowbox.sty
--rw-r--r--   0        0        0     3445 2023-07-27 20:41:03.047621 sphinx-7.1.1/sphinx/texinputs/sphinxlatexstyleheadings.sty
--rw-r--r--   0        0        0     3064 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxlatexstylepage.sty
--rw-r--r--   0        0        0     8589 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxlatexstyletext.sty
--rw-r--r--   0        0        0    57830 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxlatextables.sty
--rw-r--r--   0        0        0     4241 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxmanual.cls
--rw-r--r--   0        0        0     2061 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxoptionsgeometry.sty
--rw-r--r--   0        0        0     1094 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxoptionshyperref.sty
--rw-r--r--   0        0        0    36615 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxpackageboxes.sty
--rw-r--r--   0        0        0     2590 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxpackagecyrillic.sty
--rw-r--r--   0        0        0    15254 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs/sphinxpackagefootnote.sty
--rw-r--r--   0        0        0     2503 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/texinputs_win/Makefile_t
--rw-r--r--   0        0        0     3321 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/agogo/layout.html
--rw-r--r--   0        0        0     9144 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/agogo/static/agogo.css_t
--rw-r--r--   0        0        0      276 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/agogo/static/bgfooter.png
--rw-r--r--   0        0        0      266 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/agogo/static/bgtop.png
--rw-r--r--   0        0        0      477 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/agogo/theme.conf
--rw-r--r--   0        0        0      466 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/changes/frameset.html
--rw-r--r--   0        0        0      485 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/changes/rstsource.html
--rw-r--r--   0        0        0     1306 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/changes/versionchanges.html
--rw-r--r--   0        0        0     1636 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/defindex.html
--rw-r--r--   0        0        0     1892 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/domainindex.html
--rw-r--r--   0        0        0     1804 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/genindex-single.html
--rw-r--r--   0        0        0     1210 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/genindex-split.html
--rw-r--r--   0        0        0     2069 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/genindex.html
--rw-r--r--   0        0        0      432 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/globaltoc.html
--rw-r--r--   0        0        0     7634 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/layout.html
--rw-r--r--   0        0        0      370 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/localtoc.html
--rw-r--r--   0        0        0      679 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/opensearch.xml
--rw-r--r--   0        0        0      273 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/page.html
--rw-r--r--   0        0        0      652 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/relations.html
--rw-r--r--   0        0        0     2039 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/search.html
--rw-r--r--   0        0        0      809 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/searchbox.html
--rw-r--r--   0        0        0      947 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/searchfield.html
--rw-r--r--   0        0        0      544 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/sourcelink.html
--rw-r--r--   0        0        0    15139 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/basic.css_t
--rw-r--r--   0        0        0     4472 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/doctools.js
--rw-r--r--   0        0        0      673 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/documentation_options.js_t
--rw-r--r--   0        0        0      286 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/file.png
--rw-r--r--   0        0        0      676 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/language_data.js_t
--rw-r--r--   0        0        0       90 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/minus.png
--rw-r--r--   0        0        0       90 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/plus.png
--rw-r--r--   0        0        0    18215 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/static/sphinx_highlight.js
--rw-r--r--   0        0        0      371 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/basic/theme.conf
--rw-r--r--   0        0        0      664 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/bizstyle/layout.html
--rw-r--r--   0        0        0       78 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/bizstyle/static/background_b01.png
--rw-r--r--   0        0        0    10314 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/bizstyle/static/bizstyle.css_t
--rw-r--r--   0        0        0     1129 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/bizstyle/static/bizstyle.js_t
--rw-r--r--   0        0        0    14940 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/bizstyle/static/css3-mediaqueries.js
--rw-r--r--   0        0        0    28634 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js
--rw-r--r--   0        0        0      148 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/bizstyle/theme.conf
--rw-r--r--   0        0        0      661 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/classic/layout.html
--rw-r--r--   0        0        0     6635 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/classic/static/classic.css_t
--rw-r--r--   0        0        0     2659 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/classic/static/sidebar.js_t
--rw-r--r--   0        0        0      719 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/classic/theme.conf
--rw-r--r--   0        0        0       28 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/default/static/default.css
--rw-r--r--   0        0        0       26 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/default/theme.conf
--rw-r--r--   0        0        0      693 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/epub/epub-cover.html
--rw-r--r--   0        0        0      543 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/epub/layout.html
--rw-r--r--   0        0        0    12378 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/epub/static/epub.css_t
--rw-r--r--   0        0        0      108 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/epub/theme.conf
--rw-r--r--   0        0        0     2012 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/haiku/layout.html
--rw-r--r--   0        0        0     1128 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/haiku/static/alert_info_32.png
--rw-r--r--   0        0        0      944 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/haiku/static/alert_warning_32.png
--rw-r--r--   0        0        0       82 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/haiku/static/bg-page.png
--rw-r--r--   0        0        0      165 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/haiku/static/bullet_orange.png
--rw-r--r--   0        0        0     7059 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/haiku/static/haiku.css_t
--rw-r--r--   0        0        0      298 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/haiku/theme.conf
--rw-r--r--   0        0        0     4234 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/nature/static/nature.css_t
--rw-r--r--   0        0        0       71 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/nature/theme.conf
--rw-r--r--   0        0        0      642 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/nonav/layout.html
--rw-r--r--   0        0        0     9636 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/nonav/static/nonav.css_t
--rw-r--r--   0        0        0      109 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/nonav/theme.conf
--rw-r--r--   0        0        0      875 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/layout.html
--rw-r--r--   0        0        0     1394 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-note.png
--rw-r--r--   0        0        0     1351 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-seealso.png
--rw-r--r--   0        0        0     1186 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-todo.png
--rw-r--r--   0        0        0     1798 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-topic.png
--rw-r--r--   0        0        0     1280 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-warning.png
--rw-r--r--   0        0        0     5629 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/epub.css_t
--rw-r--r--   0        0        0      333 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/footerbg.png
--rw-r--r--   0        0        0      190 2023-07-27 20:41:03.051622 sphinx-7.1.1/sphinx/themes/pyramid/static/headerbg.png
--rw-r--r--   0        0        0      726 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/pyramid/static/ie6.css
--rw-r--r--   0        0        0      101 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/pyramid/static/middlebg.png
--rw-r--r--   0        0        0     6301 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/pyramid/static/pyramid.css_t
--rw-r--r--   0        0        0       49 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/pyramid/static/transparent.gif
--rw-r--r--   0        0        0      102 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/pyramid/theme.conf
--rw-r--r--   0        0        0     5775 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/artwork/logo.svg
--rw-r--r--   0        0        0     1661 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/layout.html
--rw-r--r--   0        0        0    25238 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/darkmetal.png
--rw-r--r--   0        0        0      172 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/headerbg.png
--rw-r--r--   0        0        0     8305 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/logo.png
--rw-r--r--   0        0        0     7547 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/metal.png
--rw-r--r--   0        0        0      124 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/navigation.png
--rw-r--r--   0        0        0      303 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/print.css
--rw-r--r--   0        0        0     7977 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/scrolls.css_t
--rw-r--r--   0        0        0      527 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/theme_extras.js
--rw-r--r--   0        0        0    44483 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/watermark.png
--rw-r--r--   0        0        0     8049 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/static/watermark_blur.png
--rw-r--r--   0        0        0      260 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/scrolls/theme.conf
--rw-r--r--   0        0        0      107 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/sphinxdoc/static/contents.png
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/sphinxdoc/static/navigation.png
--rw-r--r--   0        0        0     6314 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t
--rw-r--r--   0        0        0       77 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/sphinxdoc/theme.conf
--rw-r--r--   0        0        0    12162 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/traditional/static/traditional.css_t
--rw-r--r--   0        0        0      105 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/themes/traditional/theme.conf
--rw-r--r--   0        0        0     7937 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/theming.py
--rw-r--r--   0        0        0    15096 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/transforms/__init__.py
--rw-r--r--   0        0        0     2768 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/transforms/compact_bullet_list.py
--rw-r--r--   0        0        0    25668 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/transforms/i18n.py
--rw-r--r--   0        0        0    12028 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/transforms/post_transforms/__init__.py
--rw-r--r--   0        0        0     4486 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/transforms/post_transforms/code.py
--rw-r--r--   0        0        0    10268 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/transforms/post_transforms/images.py
--rw-r--r--   0        0        0     1361 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/transforms/references.py
--rw-r--r--   0        0        0    12524 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/__init__.py
--rw-r--r--   0        0        0      240 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/build_phase.py
--rw-r--r--   0        0        0    15386 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/cfamily.py
--rw-r--r--   0        0        0     3223 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/console.py
--rw-r--r--   0        0        0     2665 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/display.py
--rw-r--r--   0        0        0    16843 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/docfields.py
--rw-r--r--   0        0        0     2930 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/docstrings.py
--rw-r--r--   0        0        0    22767 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/docutils.py
--rw-r--r--   0        0        0     1960 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/exceptions.py
--rw-r--r--   0        0        0     3722 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/fileutil.py
--rw-r--r--   0        0        0      513 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/http_date.py
--rw-r--r--   0        0        0     9615 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/i18n.py
--rw-r--r--   0        0        0     3660 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/images.py
--rw-r--r--   0        0        0    28244 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/inspect.py
--rw-r--r--   0        0        0     6311 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/inventory.py
--rw-r--r--   0        0        0    18046 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/logging.py
--rw-r--r--   0        0        0     5279 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/matching.py
--rw-r--r--   0        0        0     1816 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/math.py
--rw-r--r--   0        0        0    23171 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/nodes.py
--rw-r--r--   0        0        0     6973 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/osutil.py
--rw-r--r--   0        0        0     5023 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/parallel.py
--rw-r--r--   0        0        0     1445 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/png.py
--rw-r--r--   0        0        0     2428 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/requests.py
--rw-r--r--   0        0        0     3302 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/rst.py
--rw-r--r--   0        0        0     2651 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/tags.py
--rw-r--r--   0        0        0     4691 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/template.py
--rw-r--r--   0        0        0     5442 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/texescape.py
--rw-r--r--   0        0        0    14994 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/util/typing.py
--rw-r--r--   0        0        0     5801 2023-07-27 20:41:03.055622 sphinx-7.1.1/sphinx/versioning.py
--rw-r--r--   0        0        0       31 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/__init__.py
--rw-r--r--   0        0        0     1605 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/html.py
--rw-r--r--   0        0        0    37087 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/html5.py
--rw-r--r--   0        0        0    90716 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/latex.py
--rw-r--r--   0        0        0    15917 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/manpage.py
--rw-r--r--   0        0        0    53161 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/texinfo.py
--rw-r--r--   0        0        0    43225 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/text.py
--rw-r--r--   0        0        0     1472 2023-07-27 20:41:03.059622 sphinx-7.1.1/sphinx/writers/xml.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3054 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/certs/cert.pem
--rw-r--r--   0        0        0     1574 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/conftest.py
--rw-r--r--   0        0        0      363 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/ext_napoleon_pep526_data_google.py
--rw-r--r--   0        0        0      385 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/ext_napoleon_pep526_data_numpy.py
--rw-r--r--   0        0        0       34 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/js/documentation_options.js
--rw-r--r--   0        0        0     1694 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/js/searchtools.js
--rw-r--r--   0        0        0     1985 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/js/sphinx_highlight.js
--rw-r--r--   0        0        0      111 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_enumerable_node/conf.py
--rw-r--r--   0        0        0     1464 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_enumerable_node/enumerable_node.py
--rw-r--r--   0        0        0      763 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_enumerable_node/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_enumerable_node/rimg.png
--rw-r--r--   0        0        0      277 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_source_parser-conflicts-with-users-setting/conf.py
--rw-r--r--   0        0        0      201 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_source_parser-conflicts-with-users-setting/source_parser.py
--rw-r--r--   0        0        0      121 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_source_parser/conf.py
--rw-r--r--   0        0        0      201 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-add_source_parser/source_parser.py
--rw-r--r--   0        0        0     1659 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-api-set-translator/conf.py
--rw-r--r--   0        0        0       72 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-api-set-translator/index.rst
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-api-set-translator/nonext/conf.py
--rw-r--r--   0        0        0      101 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-api-set-translator/translator.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-duplicates/fish_licence/halibut.cpython-38-x86_64-linux-gnu.so
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-duplicates/fish_licence/halibut.pyx
--rw-r--r--   0        0        0       12 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-pep420/a/b/c/__init__.py
--rw-r--r--   0        0        0       11 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-pep420/a/b/c/d.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-pep420/a/b/e/__init__.py
--rw-r--r--   0        0        0       11 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-pep420/a/b/e/f.py
--rw-r--r--   0        0        0       11 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-pep420/a/b/x/y.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-subpackage-in-toc/parent/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-subpackage-in-toc/parent/child/__init__.py
--rw-r--r--   0        0        0        6 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-subpackage-in-toc/parent/child/foo.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-toc/mypackage/__init__.py
--rwxr-xr-x   0        0        0      404 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-toc/mypackage/main.py
--rw-r--r--   0        0        0       79 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-toc/mypackage/no_init/foo.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-toc/mypackage/resource/__init__.py
--rw-r--r--   0        0        0       96 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-toc/mypackage/resource/resource.txt
--rw-r--r--   0        0        0       23 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-toc/mypackage/something/__init__.py
--rw-r--r--   0        0        0       44 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-trailing-underscore/package_/__init__.py
--rw-r--r--   0        0        0      215 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-apidoc-trailing-underscore/package_/module_.py
--rw-r--r--   0        0        0      221 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-autosummary/conf.py
--rw-r--r--   0        0        0     1335 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-autosummary/dummy_module.py
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-autosummary/index.rst
--rw-r--r--   0        0        0      507 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-autosummary/sphinx.rst
--rw-r--r--   0        0        0      198 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-autosummary/underscore_module_.py
--rw-r--r--   0        0        0      114 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-basic/conf.py
--rw-r--r--   0        0        0     1477 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-basic/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/extra.css
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/mytheme.css
--rw-r--r--   0        0        0       60 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/theme.conf
--rw-r--r--   0        0        0       53 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-html-theme-having-multiple-stylesheets/conf.py
--rw-r--r--   0        0        0      100 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-html-theme-having-multiple-stylesheets/index.rst
--rw-r--r--   0        0        0      372 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-html-translator/conf.py
--rw-r--r--   0        0        0      252 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-html-translator/index.rst
--rw-r--r--   0        0        0       53 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/conf.py
--rw-r--r--   0        0        0       20 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/doc1.txt
--rw-r--r--   0        0        0       51 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/doc2.txt
--rw-r--r--   0        0        0      135 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/index.txt
--rw-r--r--   0        0        0       62 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/lineblock.txt
--rw-r--r--   0        0        0       40 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/listitems.txt
--rw-r--r--   0        0        0      388 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/maxwidth.txt
--rw-r--r--   0        0        0      478 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/nonascii_maxwidth.txt
--rw-r--r--   0        0        0       75 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/nonascii_table.txt
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/nonascii_title.txt
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/table.txt
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/table_colspan.txt
--rw-r--r--   0        0        0      140 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/table_colspan_and_rowspan.txt
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/table_colspan_left.txt
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-build-text/table_rowspan.txt
--rw-r--r--   0        0        0       18 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-dirhtml/bar.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-dirhtml/conf.py
--rw-r--r--   0        0        0       32 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-dirhtml/foo/foo_1.rst
--rw-r--r--   0        0        0       32 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-dirhtml/foo/foo_2.rst
--rw-r--r--   0        0        0       63 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-dirhtml/foo/index.rst
--rw-r--r--   0        0        0       59 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-dirhtml/index.rst
--rw-r--r--   0        0        0       74 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-gettext-dont-rebuild-mo/bom.rst
--rw-r--r--   0        0        0       16 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-gettext-dont-rebuild-mo/conf.py
--rw-r--r--   0        0        0      108 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-gettext-dont-rebuild-mo/index.rst
--rw-r--r--   0        0        0      264 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-builder-gettext-dont-rebuild-mo/xx/LC_MESSAGES/bom.po
--rw-r--r--   0        0        0      330 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-changes/base.rst
--rw-r--r--   0        0        0      371 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-changes/c-api.rst
--rw-r--r--   0        0        0      134 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-changes/conf.py
--rw-r--r--   0        0        0      189 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-changes/contents.rst
--rw-r--r--   0        0        0      443 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-changes/library/utils.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-circular/conf.py
--rw-r--r--   0        0        0       22 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-circular/index.rst
--rw-r--r--   0        0        0       23 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-circular/sub.rst
--rw-r--r--   0        0        0       81 2023-07-27 20:41:03.059622 sphinx-7.1.1/tests/roots/test-config/conf.py
--rw-r--r--   0        0        0      155 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-copyright-multiline/conf.py
--rw-r--r--   0        0        0       75 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-copyright-multiline/index.rst
--rw-r--r--   0        0        0       32 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-correct-year/conf.py
--rw-r--r--   0        0        0       55 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-correct-year/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-default_role/conf.py
--rw-r--r--   0        0        0       29 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-default_role/foo.rst
--rw-r--r--   0        0        0       54 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-default_role/index.rst
--rw-r--r--   0        0        0      762 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/caption.rst
--rw-r--r--   0        0        0      263 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/classes.rst
--rw-r--r--   0        0        0       44 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/conf.py
--rw-r--r--   0        0        0     1434 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/dedent.rst
--rw-r--r--   0        0        0      170 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/emphasize.rst
--rw-r--r--   0        0        0        3 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/empty.inc
--rw-r--r--   0        0        0       21 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/error.inc
--rw-r--r--   0        0        0      203 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/force.rst
--rw-r--r--   0        0        0      345 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/highlight.rst
--rw-r--r--   0        0        0      267 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/index.rst
--rw-r--r--   0        0        0      349 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/linenos.rst
--rw-r--r--   0        0        0      396 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/linenothreshold.rst
--rw-r--r--   0        0        0      206 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/literal-diff.inc
--rw-r--r--   0        0        0       67 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/literal-short.inc
--rw-r--r--   0        0        0      213 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/literal.inc
--rw-r--r--   0        0        0      421 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/namedblocks.rst
--rw-r--r--   0        0        0      263 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/py-decorators.inc
--rw-r--r--   0        0        0      391 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/py-decorators.rst
--rw-r--r--   0        0        0      305 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/python.rst
--rw-r--r--   0        0        0      355 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-code/target.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-csv-table/conf.py
--rw-r--r--   0        0        0       12 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-csv-table/example.csv
--rw-r--r--   0        0        0       12 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-csv-table/subdir/example.csv
--rw-r--r--   0        0        0       62 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-only/conf.py
--rw-r--r--   0        0        0       63 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-only/index.rst
--rw-r--r--   0        0        0     3063 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directive-only/only.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directives-raw/conf.py
--rw-r--r--   0        0        0      404 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-directives-raw/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-docutilsconf/conf.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-docutilsconf/docutils.conf
--rw-r--r--   0        0        0       89 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-docutilsconf/index.rst
--rw-r--r--   0        0        0       65 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c-c_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      119 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c-c_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       74 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c-intersphinx/conf.py
--rw-r--r--   0        0        0     1146 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c-intersphinx/index.rst
--rw-r--r--   0        0        0      121 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c/anon-dup-decl.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c/conf.py
--rw-r--r--   0        0        0       70 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c/field-role.rst
--rw-r--r--   0        0        0      101 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c/function_param_target.rst
--rw-r--r--   0        0        0      785 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c/index.rst
--rw-r--r--   0        0        0      261 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c/namespace.rst
--rw-r--r--   0        0        0      163 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-c/ns_lookup.rst
--rw-r--r--   0        0        0       67 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      129 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       74 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp-intersphinx/conf.py
--rw-r--r--   0        0        0     2444 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp-intersphinx/index.rst
--rw-r--r--   0        0        0       92 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/anon-dup-decl.rst
--rw-r--r--   0        0        0      688 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/any-role.rst
--rw-r--r--   0        0        0       27 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/backslash.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/conf.py
--rw-r--r--   0        0        0       59 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/field-role.rst
--rw-r--r--   0        0        0     1136 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/index.rst
--rw-r--r--   0        0        0      133 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/lookup-key-overload.rst
--rw-r--r--   0        0        0      437 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/multi-decl-lookup.rst
--rw-r--r--   0        0        0     2136 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/roles-targets-ok.rst
--rw-r--r--   0        0        0     2406 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/roles-targets-warn.rst
--rw-r--r--   0        0        0      697 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/roles.rst
--rw-r--r--   0        0        0       90 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/roles2.rst
--rw-r--r--   0        0        0      383 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/semicolon.rst
--rw-r--r--   0        0        0      203 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/warn-template-param-qualified-name.rst
--rw-r--r--   0        0        0      249 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-cpp/xref_consistency.rst
--rw-r--r--   0        0        0       45 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-js-javascript_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      156 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-js-javascript_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-js/conf.py
--rw-r--r--   0        0        0       66 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-js/index.rst
--rw-r--r--   0        0        0      527 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-js/module.rst
--rw-r--r--   0        0        0      886 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-js/roles.rst
--rw-r--r--   0        0        0       41 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py-python_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      168 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py-python_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       41 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py-python_use_unqualified_type_names/conf.py
--rw-r--r--   0        0        0      240 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py-python_use_unqualified_type_names/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py-xref-warning/conf.py
--rw-r--r--   0        0        0      116 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py-xref-warning/index.rst
--rw-r--r--   0        0        0      359 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py/abbr.rst
--rw-r--r--   0        0        0      174 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py/canonical.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py/conf.py
--rw-r--r--   0        0        0      107 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py/index.rst
--rw-r--r--   0        0        0     1040 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py/module.rst
--rw-r--r--   0        0        0      383 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py/module_option.rst
--rw-r--r--   0        0        0      872 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-domain-py/roles.rst
--rw-r--r--   0        0        0       24 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme1/theme.conf
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme2/theme.conf
--rw-r--r--   0        0        0      127 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-double-inheriting-theme/conf.py
--rw-r--r--   0        0        0       87 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-double-inheriting-theme/index.rst
--rw-r--r--   0        0        0       40 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-environment-record-dependencies/api.rst
--rw-r--r--   0        0        0       99 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-environment-record-dependencies/conf.py
--rw-r--r--   0        0        0       38 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-environment-record-dependencies/example_module.py
--rw-r--r--   0        0        0       22 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-environment-record-dependencies/index.rst
--rw-r--r--   0        0        0       87 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-epub-anchor-id/conf.py
--rw-r--r--   0        0        0      191 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-epub-anchor-id/index.rst
--rw-r--r--   0        0        0      111 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/autodoc_dummy_bar.py
--rw-r--r--   0        0        0       94 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/autodoc_dummy_module.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/bug2437/__init__.py
--rw-r--r--   0        0        0       47 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/bug2437/autodoc_dummy_foo.py
--rw-r--r--   0        0        0      215 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/conf.py
--rw-r--r--   0        0        0      282 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/index.rst
--rw-r--r--   0        0        0      149 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/TYPE_CHECKING.py
--rw-r--r--   0        0        0     4363 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/__init__.py
--rw-r--r--   0        0        0      187 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/_functions_to_import.py
--rw-r--r--   0        0        0      428 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/abstractmethods.py
--rw-r--r--   0        0        0      150 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/annotated.py
--rw-r--r--   0        0        0      882 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/autoclass_content.py
--rw-r--r--   0        0        0      665 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py
--rw-r--r--   0        0        0      107 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/bound_method.py
--rw-r--r--   0        0        0      219 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/cached_property.py
--rw-r--r--   0        0        0      279 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/callable.py
--rw-r--r--   0        0        0       47 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/canonical/__init__.py
--rw-r--r--   0        0        0      158 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/canonical/original.py
--rw-r--r--   0        0        0      684 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/classes.py
--rw-r--r--   0        0        0      764 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/coroutine.py
--rw-r--r--   0        0        0      245 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/cython.pyx
--rw-r--r--   0        0        0      766 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/decorator.py
--rw-r--r--   0        0        0      683 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/descriptor.py
--rw-r--r--   0        0        0      643 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/docstring_signature.py
--rw-r--r--   0        0        0      150 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/empty_all.py
--rw-r--r--   0        0        0      384 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/enums.py
--rw-r--r--   0        0        0      227 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/final.py
--rw-r--r--   0        0        0      268 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/functions.py
--rw-r--r--   0        0        0      278 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/generic_class.py
--rw-r--r--   0        0        0      262 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/genericalias.py
--rw-r--r--   0        0        0      260 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/hide_value.py
--rw-r--r--   0        0        0       42 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/imported_members.py
--rw-r--r--   0        0        0      458 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/inheritance.py
--rw-r--r--   0        0        0      279 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/instance_variable.py
--rw-r--r--   0        0        0       52 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/metadata.py
--rw-r--r--   0        0        0      422 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/methods.py
--rw-r--r--   0        0        0      155 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/module.py
--rw-r--r--   0        0        0       93 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/name_conflict/__init__.py
--rw-r--r--   0        0        0       65 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/name_conflict/foo.py
--rw-r--r--   0        0        0      169 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/name_mangling.py
--rw-r--r--   0        0        0      894 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/need_mocks.py
--rw-r--r--   0        0        0     1345 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/overload.py
--rw-r--r--   0        0        0       59 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/overload2.py
--rw-r--r--   0        0        0      207 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/partialfunction.py
--rw-r--r--   0        0        0      420 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/partialmethod.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/pep570.py
--rw-r--r--   0        0        0      292 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/pep604.py
--rw-r--r--   0        0        0      831 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/preserve_defaults.py
--rw-r--r--   0        0        0      556 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/private.py
--rw-r--r--   0        0        0       90 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/process_docstring.py
--rw-r--r--   0        0        0      407 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/properties.py
--rw-r--r--   0        0        0      705 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/singledispatch.py
--rw-r--r--   0        0        0      628 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/singledispatchmethod.py
--rw-r--r--   0        0        0      396 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/slots.py
--rw-r--r--   0        0        0      168 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/sort_by_all.py
--rw-r--r--   0        0        0      551 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/typed_vars.py
--rw-r--r--   0        0        0     2107 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/typehints.py
--rw-r--r--   0        0        0      461 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/typevar.py
--rw-r--r--   0        0        0      123 2023-07-27 20:41:03.063622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/uninitialized_attributes.py
--rw-r--r--   0        0        0      372 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autodoc/target/wrappedfunction.py
--rw-r--r--   0        0        0       85 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosectionlabel-prefix-document/conf.py
--rw-r--r--   0        0        0      591 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst
--rw-r--r--   0        0        0       45 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosectionlabel/conf.py
--rw-r--r--   0        0        0      535 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosectionlabel/index.rst
--rw-r--r--   0        0        0      294 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-filename-map/autosummary_dummy_module.py
--rw-r--r--   0        0        0      255 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-filename-map/conf.py
--rw-r--r--   0        0        0      198 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-filename-map/index.rst
--rw-r--r--   0        0        0       47 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/__init__.py
--rw-r--r--   0        0        0       85 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/autosummary_dummy_module.py
--rw-r--r--   0        0        0      168 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-imported_members/conf.py
--rw-r--r--   0        0        0      147 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-imported_members/index.rst
--rw-r--r--   0        0        0      171 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-mock_imports/conf.py
--rw-r--r--   0        0        0       72 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-mock_imports/foo.py
--rw-r--r--   0        0        0      117 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-mock_imports/index.rst
--rw-r--r--   0        0        0      241 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/__init__.py
--rw-r--r--   0        0        0      201 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/autosummary_dummy_module.py
--rw-r--r--   0        0        0      201 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/extra_dummy_module.py
--rw-r--r--   0        0        0      170 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-module_all/conf.py
--rw-r--r--   0        0        0      154 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-module_all/index.rst
--rw-r--r--   0        0        0      132 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/conf.py
--rw-r--r--   0        0        0      174 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/package/__init__.py
--rw-r--r--   0        0        0      147 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/package/module.py
--rw-r--r--   0        0        0       63 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/package/module_importfail.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/package/package/__init__.py
--rw-r--r--   0        0        0      147 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/package/package/module.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/package2/__init__.py
--rw-r--r--   0        0        0      147 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-recursive/package2/module.py
--rw-r--r--   0        0        0      404 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-skip-member/conf.py
--rw-r--r--   0        0        0       54 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-skip-member/index.rst
--rw-r--r--   0        0        0      264 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-skip-member/target.py
--rw-r--r--   0        0        0        6 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-template/_templates/empty.rst
--rw-r--r--   0        0        0      209 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-template/conf.py
--rw-r--r--   0        0        0       78 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-template/index.rst
--rw-r--r--   0        0        0       39 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary-template/target.py
--rw-r--r--   0        0        0       22 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary/autosummary_class_module.py
--rw-r--r--   0        0        0      232 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary/autosummary_dummy_inherited_module.py
--rw-r--r--   0        0        0      932 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary/autosummary_dummy_module.py
--rw-r--r--   0        0        0       63 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary/autosummary_importfail.py
--rw-r--r--   0        0        0      190 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary/conf.py
--rw-r--r--   0        0        0      499 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-autosummary/index.rst
--rw-r--r--   0        0        0      242 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-coverage/conf.py
--rw-r--r--   0        0        0      254 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-coverage/coverage_ignored.py
--rw-r--r--   0        0        0      254 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-coverage/coverage_not_ignored.py
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-coverage/index.rst
--rw-r--r--   0        0        0      371 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-skipif/conf.py
--rw-r--r--   0        0        0     2052 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-skipif/skipif.txt
--rw-r--r--   0        0        0      205 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-with-autodoc/conf.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-with-autodoc/dir/__init__.py
--rw-r--r--   0        0        0       28 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-with-autodoc/dir/bar.py
--rw-r--r--   0        0        0       60 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-with-autodoc/dir/inner.rst
--rw-r--r--   0        0        0       25 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-with-autodoc/foo.py
--rw-r--r--   0        0        0       52 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest-with-autodoc/index.rst
--rw-r--r--   0        0        0      148 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest/conf.py
--rw-r--r--   0        0        0     2147 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-doctest/doctest.txt
--rw-r--r--   0        0        0      190 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/conf.py
--rw-r--r--   0        0        0      555 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst
--rw-r--r--   0        0        0      161 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-extlinks-hardcoded-urls/conf.py
--rw-r--r--   0        0        0      703 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst
--rw-r--r--   0        0        0       40 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-githubpages/conf.py
--rw-r--r--   0        0        0       25 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-githubpages/index.rst
--rw-r--r--   0        0        0       67 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-graphviz/conf.py
--rw-r--r--   0        0        0       25 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-graphviz/graph.dot
--rw-r--r--   0        0        0       25 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-graphviz/graph.xx.dot
--rw-r--r--   0        0        0      389 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-graphviz/index.rst
--rw-r--r--   0        0        0      256 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-ifconfig/conf.py
--rw-r--r--   0        0        0      274 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-ifconfig/index.rst
--rw-r--r--   0        0        0       41 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgconverter/conf.py
--rw-r--r--   0        0        0   141783 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgconverter/img.pdf
--rw-r--r--   0        0        0       86 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgconverter/index.rst
--rw-r--r--   0        0        0      243 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgconverter/svgimg.svg
--rw-r--r--   0        0        0      106 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgmockconverter/1/svgimg.svg
--rw-r--r--   0        0        0      243 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgmockconverter/2/svgimg.svg
--rw-r--r--   0        0        0       97 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgmockconverter/conf.py
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgmockconverter/index.rst
--rw-r--r--   0        0        0      881 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py
--rw-r--r--   0        0        0      112 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-inheritance_diagram/conf.py
--rw-r--r--   0        0        0       13 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-inheritance_diagram/example/__init__.py
--rw-r--r--   0        0        0       46 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-inheritance_diagram/example/sphinx.py
--rw-r--r--   0        0        0      215 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-inheritance_diagram/index.rst
--rw-r--r--   0        0        0      101 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-inheritance_diagram/test.py
--rw-r--r--   0        0        0       40 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-intersphinx-cppdomain/conf.py
--rw-r--r--   0        0        0      150 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-intersphinx-cppdomain/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-intersphinx-role/conf.py
--rw-r--r--   0        0        0     1211 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-intersphinx-role/index.rst
--rw-r--r--   0        0        0      488 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math-compat/conf.py
--rw-r--r--   0        0        0      199 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math-compat/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math-simple/conf.py
--rw-r--r--   0        0        0       43 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math-simple/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math/conf.py
--rw-r--r--   0        0        0      239 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math/index.rst
--rw-r--r--   0        0        0      396 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math/math.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math/nomath.rst
--rw-r--r--   0        0        0      128 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-math/page.rst
--rw-r--r--   0        0        0      100 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-napoleon/conf.py
--rw-r--r--   0        0        0       64 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-napoleon/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.067622 sphinx-7.1.1/tests/roots/test-ext-napoleon/mypackage/__init__.py
--rw-r--r--   0        0        0      194 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-napoleon/mypackage/typehints.py
--rw-r--r--   0        0        0       70 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-napoleon/typehints.rst
--rw-r--r--   0        0        0       31 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-todo/bar.rst
--rw-r--r--   0        0        0       33 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-todo/conf.py
--rw-r--r--   0        0        0      125 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-todo/foo.rst
--rw-r--r--   0        0        0      109 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-todo/index.rst
--rw-r--r--   0        0        0      108 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode-find/conf.py
--rw-r--r--   0        0        0      636 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode-find/index.rst
--rw-r--r--   0        0        0       37 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode-find/not_a_package/__init__.py
--rw-r--r--   0        0        0      371 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode-find/not_a_package/submodule.py
--rw-r--r--   0        0        0      745 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode/conf.py
--rw-r--r--   0        0        0      550 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode/index.rst
--rw-r--r--   0        0        0     3111 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode/objects.rst
--rw-r--r--   0        0        0       64 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode/spam/__init__.py
--rw-r--r--   0        0        0      308 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode/spam/mod1.py
--rw-r--r--   0        0        0      188 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode/spam/mod2.py
--rw-r--r--   0        0        0       52 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-ext-viewcode/spam/mod3.py
--rw-r--r--   0        0        0       63 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-extensions/conf.py
--rw-r--r--   0        0        0       70 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-extensions/read_parallel.py
--rw-r--r--   0        0        0       71 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-extensions/read_serial.py
--rw-r--r--   0        0        0       72 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-extensions/write_parallel.py
--rw-r--r--   0        0        0       72 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-extensions/write_serial.py
--rw-r--r--   0        0        0       70 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-footnotes/bar.rst
--rw-r--r--   0        0        0       70 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-footnotes/baz.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-footnotes/conf.py
--rw-r--r--   0        0        0     3385 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-footnotes/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-footnotes/rimg.png
--rw-r--r--   0        0        0      143 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-gettext-template/_templates/template1.html
--rw-r--r--   0        0        0      143 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-gettext-template/_templates/template2.html
--rw-r--r--   0        0        0       32 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-gettext-template/conf.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-gettext-template/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-glossary/conf.py
--rw-r--r--   0        0        0      260 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-glossary/index.rst
--rw-r--r--   0        0        0      103 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-highlight_options/conf.py
--rw-r--r--   0        0        0      166 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-highlight_options/index.rst
--rw-r--r--   0        0        0      468 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/conf.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/.htaccess
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/.htpasswd
--rw-r--r--   0        0        0       28 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/API.html_t
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/css/style.css
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/rimg.png
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/subdir/.htaccess
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/extra/subdir/.htpasswd
--rw-r--r--   0        0        0       65 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/.htaccess
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/.htpasswd
--rw-r--r--   0        0        0       28 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/API.html_t
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/css/style.css
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/js/custom.js
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/rimg.png
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/subdir/.htaccess
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/static/subdir/.htpasswd
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/subdir/_build/index.html
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_assets/subdir/background.png
--rw-r--r--   0        0        0       53 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_entity/conf.py
--rw-r--r--   0        0        0      561 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_entity/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_scaled_image_link/conf.py
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_scaled_image_link/img.png
--rw-r--r--   0        0        0      172 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_scaled_image_link/index.rst
--rw-r--r--   0        0        0       36 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_signaturereturn_icon/conf.py
--rw-r--r--   0        0        0      108 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_signaturereturn_icon/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_style/_static/default.css
--rw-r--r--   0        0        0       58 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_style/conf.py
--rw-r--r--   0        0        0       22 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-html_style/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-escape/conf.py
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-escape/img_#1.png
--rw-r--r--   0        0        0      145 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-escape/index.rst
--rw-r--r--   0        0        0      161 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-in-parsed-literal/conf.py
--rw-r--r--   0        0        0      113 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-in-parsed-literal/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-in-parsed-literal/pic.png
--rw-r--r--   0        0        0      143 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-in-section/conf.py
--rw-r--r--   0        0        0      287 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-in-section/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-image-in-section/pic.png
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/conf.py
--rw-r--r--   0        0        0    24976 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/img.gif
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/img.ja.png
--rw-r--r--   0        0        0   141783 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/img.pdf
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/img.png
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/img.zh.png
--rw-r--r--   0        0        0      466 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/rimg.png
--rw-r--r--   0        0        0      218 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/rimg.png.xx
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/rimg.xx.png
--rw-r--r--   0        0        0      128 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/subdir/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/subdir/rimg.png
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.071622 sphinx-7.1.1/tests/roots/test-images/subdir/rimg.xx.png
--rw-r--r--   0        0        0   141783 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-images/subdir/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-images/subdir/svgimg.svg
--rw-r--r--   0        0        0      243 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-images/subdir/svgimg.xx.svg
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-images/testimäge.png
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-index_on_title/conf.py
--rw-r--r--   0        0        0      117 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-index_on_title/contents.rst
--rw-r--r--   0        0        0       70 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/basic_diagram.rst
--rw-r--r--   0        0        0      135 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/conf.py
--rw-r--r--   0        0        0      166 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/diagram_module_w_2_top_classes.rst
--rw-r--r--   0        0        0      125 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/diagram_w_1_top_class.rst
--rw-r--r--   0        0        0      179 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/diagram_w_2_top_classes.rst
--rw-r--r--   0        0        0      104 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/diagram_w_nested_classes.rst
--rw-r--r--   0        0        0      118 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/diagram_w_parts.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/dummy/__init__.py
--rw-r--r--   0        0        0      267 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/dummy/test.py
--rw-r--r--   0        0        0       95 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/dummy/test_nested.py
--rw-r--r--   0        0        0       31 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-inheritance/index.rst
--rw-r--r--   0        0        0      216 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/_templates/contents.html
--rw-r--r--   0        0        0      599 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/admonitions.txt
--rw-r--r--   0        0        0       74 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/bom.txt
--rw-r--r--   0        0        0      262 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/conf.py
--rw-r--r--   0        0        0      342 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/definition_terms.txt
--rw-r--r--   0        0        0      704 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/docfields.txt
--rw-r--r--   0        0        0      858 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/external_links.txt
--rw-r--r--   0        0        0      747 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/figure.txt
--rw-r--r--   0        0        0      407 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/footnote.txt
--rw-r--r--   0        0        0      378 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/glossary_terms.txt
--rw-r--r--   0        0        0      151 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/glossary_terms_inconsistency.txt
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/i18n.png
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/img.png
--rw-r--r--   0        0        0      563 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/index.txt
--rw-r--r--   0        0        0      384 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/index_entries.txt
--rw-r--r--   0        0        0     1832 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/label_target.txt
--rw-r--r--   0        0        0      943 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/literalblock.txt
--rw-r--r--   0        0        0      278 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/noqa.txt
--rw-r--r--   0        0        0      128 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/only.txt
--rw-r--r--   0        0        0       78 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/raw.txt
--rw-r--r--   0        0        0     1094 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/refs.txt
--rw-r--r--   0        0        0      291 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/refs_inconsistency.txt
--rw-r--r--   0        0        0      252 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/refs_python_domain.txt
--rw-r--r--   0        0        0      738 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/role_xref.txt
--rw-r--r--   0        0        0      152 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/rubric.txt
--rw-r--r--   0        0        0       97 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/section.txt
--rw-r--r--   0        0        0      210 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/seealso.txt
--rw-r--r--   0        0        0       32 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/subdir/index.txt
--rw-r--r--   0        0        0      263 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/table.txt
--rw-r--r--   0        0        0      139 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/toctree.txt
--rw-r--r--   0        0        0      135 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/topic.txt
--rw-r--r--   0        0        0      800 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/translation_progress.txt
--rw-r--r--   0        0        0      337 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/versionchange.txt
--rw-r--r--   0        0        0       79 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/warnings.txt
--rw-r--r--   0        0        0     1513 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po
--rw-r--r--   0        0        0      264 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/bom.po
--rw-r--r--   0        0        0     1198 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po
--rw-r--r--   0        0        0     1086 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po
--rw-r--r--   0        0        0     1691 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po
--rw-r--r--   0        0        0     1307 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/figure.po
--rw-r--r--   0        0        0     1228 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po
--rw-r--r--   0        0        0     1327 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po
--rw-r--r--   0        0        0      754 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po
--rw-r--r--   0        0        0      773 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1318 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po
--rw-r--r--   0        0        0     2159 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po
--rw-r--r--   0        0        0     2211 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po
--rw-r--r--   0        0        0     1380 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po
--rw-r--r--   0        0        0      723 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/only.po
--rw-r--r--   0        0        0      644 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/raw.po
--rw-r--r--   0        0        0     2771 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/refs.po
--rw-r--r--   0        0        0     1045 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po
--rw-r--r--   0        0        0      675 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po
--rw-r--r--   0        0        0     1707 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po
--rw-r--r--   0        0        0      744 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po
--rw-r--r--   0        0        0      706 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/section.po
--rw-r--r--   0        0        0      792 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po
--rw-r--r--   0        0        0      621 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0      992 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/table.po
--rw-r--r--   0        0        0      767 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po
--rw-r--r--   0        0        0      750 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/topic.po
--rw-r--r--   0        0        0     1585 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po
--rw-r--r--   0        0        0     1070 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po
--rw-r--r--   0        0        0      710 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po
--rw-r--r--   0        0        0       21 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-keep_warnings/conf.py
--rw-r--r--   0        0        0       20 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-keep_warnings/index.rst
--rw-r--r--   0        0        0       13 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-babel/bar.rst
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-babel/conf.py
--rw-r--r--   0        0        0       13 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-babel/foo.rst
--rw-r--r--   0        0        0       87 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-babel/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-container/conf.py
--rw-r--r--   0        0        0       35 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-container/index.rst
--rw-r--r--   0        0        0       59 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-equations/conf.py
--rw-r--r--   0        0        0      256 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-equations/equations.rst
--rw-r--r--   0        0        0      452 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-equations/expects/latex-equations.tex
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-figure-in-admonition/conf.py
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-figure-in-admonition/img.png
--rw-r--r--   0        0        0      132 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-figure-in-admonition/index.rst
--rw-r--r--   0        0        0     1573 2023-07-27 20:41:03.075622 sphinx-7.1.1/tests/roots/test-latex-includegraphics/conf.py
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-includegraphics/img.png
--rw-r--r--   0        0        0      834 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-includegraphics/index.rst
--rw-r--r--   0        0        0    34213 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-includegraphics/sphinx.png
--rw-r--r--   0        0        0    38192 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-includegraphics/tall.png
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-index/conf.py
--rw-r--r--   0        0        0      215 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-index/index.rst
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels-before-module/automodule1.py
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels-before-module/automodule2a.py
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels-before-module/automodule2b.py
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels-before-module/automodule3.py
--rw-r--r--   0        0        0      117 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels-before-module/conf.py
--rw-r--r--   0        0        0      464 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels-before-module/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels/conf.py
--rw-r--r--   0        0        0      771 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels/index.rst
--rw-r--r--   0        0        0       18 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-labels/otherdoc.rst
--rw-r--r--   0        0        0      250 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-numfig/conf.py
--rw-r--r--   0        0        0      112 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-numfig/index.rst
--rw-r--r--   0        0        0      141 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-numfig/indexhowto.rst
--rw-r--r--   0        0        0      165 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-numfig/indexmanual.rst
--rw-r--r--   0        0        0       18 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/_mytemplates/latex/longtable.tex_t
--rw-r--r--   0        0        0     1661 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/complex.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/conf.py
--rw-r--r--   0        0        0     1933 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/complex_spanning_cell.tex
--rw-r--r--   0        0        0     1752 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/gridtable.tex
--rw-r--r--   0        0        0     1780 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex
--rw-r--r--   0        0        0     1323 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable.tex
--rw-r--r--   0        0        0     1300 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_align.tex
--rw-r--r--   0        0        0     1445 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_caption.tex
--rw-r--r--   0        0        0     1384 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex
--rw-r--r--   0        0        0     1637 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex
--rw-r--r--   0        0        0     1386 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex
--rw-r--r--   0        0        0     1656 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_widths.tex
--rw-r--r--   0        0        0     1409 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex
--rw-r--r--   0        0        0     1341 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex
--rw-r--r--   0        0        0      704 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/simple_table.tex
--rw-r--r--   0        0        0      851 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_caption.tex
--rw-r--r--   0        0        0      777 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex
--rw-r--r--   0        0        0      978 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex
--rw-r--r--   0        0        0      594 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex
--rw-r--r--   0        0        0      779 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_verbatim.tex
--rw-r--r--   0        0        0     1093 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_widths.tex
--rw-r--r--   0        0        0      802 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex
--rw-r--r--   0        0        0      733 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/tabular_having_widths.tex
--rw-r--r--   0        0        0      747 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/tabularcolumn.tex
--rw-r--r--   0        0        0      727 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/expects/tabulary_having_widths.tex
--rw-r--r--   0        0        0       84 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/index.rst
--rw-r--r--   0        0        0     2516 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/longtable.rst
--rw-r--r--   0        0        0     2770 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-table/tabular.rst
--rw-r--r--   0        0        0       52 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-theme/conf.py
--rw-r--r--   0        0        0       24 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-theme/index.rst
--rw-r--r--   0        0        0      117 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-theme/theme/custom/theme.conf
--rw-r--r--   0        0        0      160 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-title/conf.py
--rw-r--r--   0        0        0      165 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-title/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-unicode/conf.py
--rw-r--r--   0        0        0      142 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-latex-unicode/index.rst
--rw-r--r--   0        0        0       80 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-anchors-ignore-for-url/conf.py
--rw-r--r--   0        0        0      532 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst
--rw-r--r--   0        0        0       80 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-anchors-ignore/conf.py
--rw-r--r--   0        0        0      109 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-anchors-ignore/index.rst
--rw-r--r--   0        0        0      180 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-documents_exclude/br0ken_link.rst
--rw-r--r--   0        0        0      174 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-documents_exclude/broken_link.rst
--rw-r--r--   0        0        0      133 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-documents_exclude/conf.py
--rw-r--r--   0        0        0       40 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-documents_exclude/index.rst
--rw-r--r--   0        0        0       80 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver-anchor/conf.py
--rw-r--r--   0        0        0       48 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver-anchor/index.rst
--rw-r--r--   0        0        0       55 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver-https/conf.py
--rw-r--r--   0        0        0       42 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver-https/index.rst
--rw-r--r--   0        0        0       55 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver-warn-redirects/conf.py
--rw-r--r--   0        0        0       95 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver-warn-redirects/index.rst
--rw-r--r--   0        0        0       55 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver/conf.py
--rw-r--r--   0        0        0       41 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-localserver/index.rst
--rw-r--r--   0        0        0       55 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-raw-node/conf.py
--rw-r--r--   0        0        0       46 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-raw-node/index.rst
--rw-r--r--   0        0        0       80 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-too-many-retries/conf.py
--rw-r--r--   0        0        0       73 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck-too-many-retries/index.rst
--rw-r--r--   0        0        0       99 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck/conf.py
--rw-r--r--   0        0        0      648 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-linkcheck/links.rst
--rw-r--r--   0        0        0      143 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-local-logo/conf.py
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-local-logo/images/img.png
--rw-r--r--   0        0        0     1477 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-local-logo/index.rst
--rw-r--r--   0        0        0       80 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       41 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       80 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       41 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       82 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       43 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-manpage_url/conf.py
--rw-r--r--   0        0        0       61 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-manpage_url/index.rst
--rw-r--r--   0        0        0      114 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-markup-citation/conf.py
--rw-r--r--   0        0        0      166 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-markup-citation/index.rst
--rw-r--r--   0        0        0      114 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-markup-rubric/conf.py
--rw-r--r--   0        0        0      112 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-markup-rubric/index.rst
--rw-r--r--   0        0        0       78 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-maxlistdepth/conf.py
--rw-r--r--   0        0        0      687 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-maxlistdepth/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-metadata/conf.py
--rw-r--r--   0        0        0     1436 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-metadata/index.rst
--rw-r--r--   0        0        0        8 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-need-escaped/bar.rst
--rw-r--r--   0        0        0        8 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-need-escaped/baz.rst
--rw-r--r--   0        0        0       62 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-need-escaped/conf.py
--rw-r--r--   0        0        0       82 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-need-escaped/foo.rst
--rw-r--r--   0        0        0      574 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-need-escaped/index.rst
--rw-r--r--   0        0        0       10 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-need-escaped/quux.rst
--rw-r--r--   0        0        0       29 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-need-escaped/qux.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-nested-enumerated-list/conf.py
--rw-r--r--   0        0        0      300 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-nested-enumerated-list/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-nested-tables/conf.py
--rw-r--r--   0        0        0      248 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-nested-tables/index.rst
--rw-r--r--   0        0        0       16 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-nitpicky-warnings/conf.py
--rw-r--r--   0        0        0      176 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-nitpicky-warnings/index.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-numbered-circular/conf.py
--rw-r--r--   0        0        0       36 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-numbered-circular/index.rst
--rw-r--r--   0        0        0       23 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-numbered-circular/sub.rst
--rw-r--r--   0        0        0      710 2023-07-27 20:41:03.079622 sphinx-7.1.1/tests/roots/test-numfig/bar.rst
--rw-r--r--   0        0        0      259 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-numfig/baz.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-numfig/conf.py
--rw-r--r--   0        0        0      912 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-numfig/foo.rst
--rw-r--r--   0        0        0     1024 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-numfig/index.rst
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-numfig/rimg.png
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-object-description-sections/conf.py
--rw-r--r--   0        0        0       80 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-object-description-sections/index.rst
--rw-r--r--   0        0        0       73 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/Bare.rst
--rw-r--r--   0        0        0       58 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/Dup1.rst
--rw-r--r--   0        0        0       58 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/Dup2.rst
--rw-r--r--   0        0        0       94 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/LineContinuation.rst
--rw-r--r--   0        0        0       72 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/P1.rst
--rw-r--r--   0        0        0       72 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/P2.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/conf.py
--rw-r--r--   0        0        0       97 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/firstLineRule.rst
--rw-r--r--   0        0        0      663 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-productionlist/index.rst
--rw-r--r--   0        0        0      177 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-prolog/conf.py
--rw-r--r--   0        0        0       83 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-prolog/index.rst
--rw-r--r--   0        0        0       57 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-prolog/markdown.md
--rw-r--r--   0        0        0      299 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-prolog/prolog_markdown_parser.py
--rw-r--r--   0        0        0       67 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-prolog/restructuredtext.rst
--rw-r--r--   0        0        0       75 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-pycode/cp_1251_coded.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-reST-code-block/conf.py
--rw-r--r--   0        0        0       97 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-reST-code-block/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-reST-code-role/conf.py
--rw-r--r--   0        0        0      194 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-reST-code-role/index.rst
--rw-r--r--   0        0        0       27 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-refonly_bullet_list/conf.py
--rw-r--r--   0        0        0      147 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-refonly_bullet_list/index.rst
--rw-r--r--   0        0        0      237 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-remote-logo/conf.py
--rw-r--r--   0        0        0     1477 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-remote-logo/index.rst
--rw-r--r--   0        0        0       32 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-roles-download/another/dummy.dat
--rw-r--r--   0        0        0      114 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-roles-download/conf.py
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-roles-download/dummy.dat
--rw-r--r--   0        0        0      214 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-roles-download/index.rst
--rw-r--r--   0        0        0     2111 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/Makefile
--rw-r--r--   0        0        0       67 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/_templates/contentssb.html
--rw-r--r--   0        0        0       99 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/_templates/customsb.html
--rw-r--r--   0        0        0      428 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/_templates/layout.html
--rw-r--r--   0        0        0      578 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/autodoc.txt
--rw-r--r--   0        0        0     4587 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/autodoc_target.py
--rw-r--r--   0        0        0       74 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/bom.txt
--rw-r--r--   0        0        0     4257 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/conf.py
--rw-r--r--   0        0        0       87 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/extapi.txt
--rw-r--r--   0        0        0      365 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/extensions.txt
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/file_with_special_#_chars.xyz
--rw-r--r--   0        0        0      826 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/footnote.txt
--rw-r--r--   0        0        0      575 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/images.txt
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/img.foo.png
--rw-r--r--   0        0        0    24976 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/img.gif
--rw-r--r--   0        0        0   141783 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/img.pdf
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/img.png
--rw-r--r--   0        0        0     2108 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/includes.txt
--rw-r--r--   0        0        0     1118 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/index.txt
--rw-r--r--   0        0        0      750 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/lists.txt
--rw-r--r--   0        0        0      200 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/literal.inc
--rw-r--r--   0        0        0      208 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/literal_orig.inc
--rw-r--r--   0        0        0     6902 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/markup.txt
--rw-r--r--   0        0        0      373 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/math.txt
--rw-r--r--   0        0        0     4561 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/objects.txt
--rw-r--r--   0        0        0      110 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/otherext.foo
--rw-r--r--   0        0        0      346 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/parsermod.py
--rw-r--r--   0        0        0       45 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/quotes.inc
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/rimg.png
--rw-r--r--   0        0        0       40 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/special/api.h
--rw-r--r--   0        0        0       32 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/special/code.py
--rw-r--r--   0        0        0       96 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/subdir/excluded.txt
--rw-r--r--   0        0        0      106 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/subdir/images.txt
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/subdir/img.png
--rw-r--r--   0        0        0      143 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/subdir/include.inc
--rw-r--r--   0        0        0      328 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/subdir/includes.txt
--rw-r--r--   0        0        0    66247 2023-07-27 20:41:03.083622 sphinx-7.1.1/tests/roots/test-root/subdir/simg.png
--rw-r--r--   0        0        0   141783 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-root/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-root/svgimg.svg
--rw-r--r--   0        0        0       78 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-root/tabs.inc
--rw-r--r--   0        0        0       77 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-root/test.inc
--rw-r--r--   0        0        0      107 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-root/wrongenc.inc
--rw-r--r--   0        0        0       58 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-search/conf.py
--rw-r--r--   0        0        0      381 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-search/index.rst
--rw-r--r--   0        0        0       41 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-search/nosearch.rst
--rw-r--r--   0        0        0      184 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-search/tocitem.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-smartquotes/conf.py
--rw-r--r--   0        0        0      107 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-smartquotes/index.rst
--rw-r--r--   0        0        0      231 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-smartquotes/literals.rst
--rw-r--r--   0        0        0      453 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-stylesheets/_templates/layout.html
--rw-r--r--   0        0        0      318 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-stylesheets/conf.py
--rw-r--r--   0        0        0       53 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-stylesheets/index.rst
--rw-r--r--   0        0        0      182 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-templating/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      109 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-templating/_templates/layout.html
--rw-r--r--   0        0        0      135 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-templating/autosummary_templating.txt
--rw-r--r--   0        0        0      266 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-templating/conf.py
--rw-r--r--   0        0        0      124 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-templating/index.txt
--rw-r--r--   0        0        0      661 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/child.zip
--rw-r--r--   0        0        0       94 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/conf.py
--rw-r--r--   0        0        0       26 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/index.rst
--rw-r--r--   0        0        0     1039 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/parent.zip
--rw-r--r--   0        0        0       82 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/test_theme/__init__.py
--rw-r--r--   0        0        0      139 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/test_theme/staticfiles/layout.html
--rw-r--r--   0        0        0      120 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/test_theme/staticfiles/static/staticimg.png
--rw-r--r--   0        0        0       82 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/test_theme/staticfiles/static/statictmpl.html_t
--rw-r--r--   0        0        0      104 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/test_theme/staticfiles/theme.conf
--rw-r--r--   0        0        0       98 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/test_theme/test-theme/theme.conf
--rw-r--r--   0        0        0     1039 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-theming/ziptheme.zip
--rw-r--r--   0        0        0      150 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-tocdepth/bar.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-tocdepth/baz.rst
--rw-r--r--   0        0        0       53 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-tocdepth/conf.py
--rw-r--r--   0        0        0      146 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-tocdepth/foo.rst
--rw-r--r--   0        0        0       71 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-tocdepth/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-domain-objects/conf.py
--rw-r--r--   0        0        0      731 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-domain-objects/domains.rst
--rw-r--r--   0        0        0       90 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-domain-objects/index.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-duplicated/conf.py
--rw-r--r--   0        0        0        8 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-duplicated/foo.rst
--rw-r--r--   0        0        0       77 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-duplicated/index.rst
--rw-r--r--   0        0        0      101 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-empty/_templates/localtoc.html
--rw-r--r--   0        0        0       62 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-empty/conf.py
--rw-r--r--   0        0        0       52 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-empty/index.rst
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/bar/bar_1.rst
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/bar/bar_2.rst
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/bar/bar_3.rst
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/bar/bar_4/index.rst
--rw-r--r--   0        0        0       53 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/bar/index.rst
--rw-r--r--   0        0        0       13 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/baz.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/conf.py
--rw-r--r--   0        0        0       13 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/foo.rst
--rw-r--r--   0        0        0      303 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/index.rst
--rw-r--r--   0        0        0       16 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/quux.rst
--rw-r--r--   0        0        0       50 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/qux/index.rst
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/qux/qux_1.rst
--rw-r--r--   0        0        0       17 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-glob/qux/qux_2.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-index/conf.py
--rw-r--r--   0        0        0      105 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-index/foo.rst
--rw-r--r--   0        0        0      132 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-index/index.rst
--rw-r--r--   0        0        0      150 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-maxdepth/bar.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-maxdepth/baz.rst
--rw-r--r--   0        0        0       30 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-maxdepth/conf.py
--rw-r--r--   0        0        0      146 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-maxdepth/foo.rst
--rw-r--r--   0        0        0      105 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-maxdepth/index.rst
--rw-r--r--   0        0        0      105 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree-maxdepth/qux.rst
--rw-r--r--   0        0        0        8 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/bar.rst
--rw-r--r--   0        0        0        8 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/baz.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/conf.py
--rw-r--r--   0        0        0       74 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/foo.rst
--rw-r--r--   0        0        0      885 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/index.rst
--rw-r--r--   0        0        0       10 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/quux.rst
--rw-r--r--   0        0        0       29 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/qux.rst
--rw-r--r--   0        0        0       97 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-toctree/tocdepth.rst
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-transforms-post_transforms-keyboard/conf.py
--rw-r--r--   0        0        0       94 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-transforms-post_transforms-keyboard/index.rst
--rw-r--r--   0        0        0       16 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-transforms-post_transforms-missing-reference/conf.py
--rw-r--r--   0        0        0      113 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-transforms-post_transforms-missing-reference/index.rst
--rw-r--r--   0        0        0       36 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-trim_doctest_flags/conf.py
--rw-r--r--   0        0        0      784 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-trim_doctest_flags/index.rst
--rw-r--r--   0        0        0     1012 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/added.txt
--rw-r--r--   0        0        0       86 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/conf.py
--rw-r--r--   0        0        0      584 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/deleted.txt
--rw-r--r--   0        0        0      490 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/deleted_end.txt
--rw-r--r--   0        0        0      164 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/index.txt
--rw-r--r--   0        0        0      864 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/insert.txt
--rw-r--r--   0        0        0      850 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/insert_beginning.txt
--rw-r--r--   0        0        0      735 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/insert_similar.txt
--rw-r--r--   0        0        0      867 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/modified.txt
--rw-r--r--   0        0        0      715 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-versioning/original.txt
--rw-r--r--   0        0        0      151 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-warnings/autodoc_fodder.py
--rw-r--r--   0        0        0       97 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-warnings/conf.py
--rw-r--r--   0        0        0      697 2023-07-27 20:41:03.087622 sphinx-7.1.1/tests/roots/test-warnings/index.rst
--rw-r--r--   0        0        0   141783 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/roots/test-warnings/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/roots/test-warnings/svgimg.svg
--rw-r--r--   0        0        0       18 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/roots/test-warnings/undecodable.rst
--rw-r--r--   0        0        0      107 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/roots/test-warnings/wrongenc.inc
--rw-r--r--   0        0        0     3309 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_api_translator.py
--rw-r--r--   0        0        0     5605 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_application.py
--rw-r--r--   0        0        0     4771 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build.py
--rw-r--r--   0        0        0     1152 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_changes.py
--rw-r--r--   0        0        0     1407 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_dirhtml.py
--rw-r--r--   0        0        0    16623 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_epub.py
--rw-r--r--   0        0        0     6524 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_gettext.py
--rw-r--r--   0        0        0    80743 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_html.py
--rw-r--r--   0        0        0    76570 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_latex.py
--rw-r--r--   0        0        0    33264 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_linkcheck.py
--rw-r--r--   0        0        0     2751 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_manpage.py
--rw-r--r--   0        0        0     5910 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_texinfo.py
--rw-r--r--   0        0        0     8996 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_build_text.py
--rw-r--r--   0        0        0     1322 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_builder.py
--rw-r--r--   0        0        0     2646 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_catalogs.py
--rw-r--r--   0        0        0    17855 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_config.py
--rw-r--r--   0        0        0      811 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_correct_year.py
--rw-r--r--   0        0        0    23761 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_directive_code.py
--rw-r--r--   0        0        0     2088 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_directive_object_description.py
--rw-r--r--   0        0        0     1655 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_directive_only.py
--rw-r--r--   0        0        0     5207 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_directive_other.py
--rw-r--r--   0        0        0     4362 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_directive_patch.py
--rw-r--r--   0        0        0     1084 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_docutilsconf.py
--rw-r--r--   0        0        0    37525 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_domain_c.py
--rw-r--r--   0        0        0    76159 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_domain_cpp.py
--rw-r--r--   0        0        0    20319 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_domain_js.py
--rw-r--r--   0        0        0    98987 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_domain_py.py
--rw-r--r--   0        0        0     5896 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_domain_rst.py
--rw-r--r--   0        0        0    19424 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_domain_std.py
--rw-r--r--   0        0        0     5286 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_environment.py
--rw-r--r--   0        0        0     8068 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_environment_indexentries.py
--rw-r--r--   0        0        0      310 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_environment_record_dependencies.py
--rw-r--r--   0        0        0    20508 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_environment_toctree.py
--rw-r--r--   0        0        0      321 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_errors.py
--rw-r--r--   0        0        0     1826 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_events.py
--rw-r--r--   0        0        0    23255 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_apidoc.py
--rw-r--r--   0        0        0    76880 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_autodoc.py
--rw-r--r--   0        0        0     4801 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_autodoc_autoattribute.py
--rw-r--r--   0        0        0    14272 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_autodoc_autoclass.py
--rw-r--r--   0        0        0     2631 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_autodoc_autodata.py
--rw-r--r--   0        0        0     5647 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_autodoc_autofunction.py
--rw-r--r--   0        0        0     5355 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_autodoc_automodule.py
--rw-r--r--   0        0        0     2501 2023-07-27 20:41:03.091622 sphinx-7.1.1/tests/test_ext_autodoc_autoproperty.py
--rw-r--r--   0        0        0    55422 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_autodoc_configs.py
--rw-r--r--   0        0        0     3335 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_autodoc_events.py
--rw-r--r--   0        0        0     3963 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_autodoc_mock.py
--rw-r--r--   0        0        0     1666 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_autodoc_preserve_defaults.py
--rw-r--r--   0        0        0     4415 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_autodoc_private_members.py
--rw-r--r--   0        0        0     3145 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_autosectionlabel.py
--rw-r--r--   0        0        0    27705 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_autosummary.py
--rw-r--r--   0        0        0     3158 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_coverage.py
--rw-r--r--   0        0        0     5517 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_doctest.py
--rw-r--r--   0        0        0      378 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_duration.py
--rw-r--r--   0        0        0     2104 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_extlinks.py
--rw-r--r--   0        0        0      958 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_githubpages.py
--rw-r--r--   0        0        0     7667 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_graphviz.py
--rw-r--r--   0        0        0      850 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_ifconfig.py
--rw-r--r--   0        0        0     1038 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_imgconverter.py
--rw-r--r--   0        0        0      609 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_imgmockconverter.py
--rw-r--r--   0        0        0    10579 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_inheritance_diagram.py
--rw-r--r--   0        0        0    21393 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_intersphinx.py
--rw-r--r--   0        0        0    13142 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_math.py
--rw-r--r--   0        0        0     6912 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_napoleon.py
--rw-r--r--   0        0        0    70796 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_napoleon_docstring.py
--rw-r--r--   0        0        0     3878 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_todo.py
--rw-r--r--   0        0        0     5467 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_ext_viewcode.py
--rw-r--r--   0        0        0      857 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_extension.py
--rw-r--r--   0        0        0     3563 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_highlighting.py
--rw-r--r--   0        0        0    51540 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_intl.py
--rw-r--r--   0        0        0     2551 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_locale.py
--rw-r--r--   0        0        0    22328 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_markup.py
--rw-r--r--   0        0        0     1931 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_metadata.py
--rw-r--r--   0        0        0     2459 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_parser.py
--rw-r--r--   0        0        0     2573 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_project.py
--rw-r--r--   0        0        0     6918 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_pycode.py
--rw-r--r--   0        0        0     2835 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_pycode_ast.py
--rw-r--r--   0        0        0    18264 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_pycode_parser.py
--rw-r--r--   0        0        0     7347 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_quickstart.py
--rw-r--r--   0        0        0     2570 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_roles.py
--rw-r--r--   0        0        0    11627 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_search.py
--rw-r--r--   0        0        0     3747 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_smartquotes.py
--rw-r--r--   0        0        0     1435 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_templating.py
--rw-r--r--   0        0        0     4334 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_theming.py
--rw-r--r--   0        0        0     1843 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_toctree.py
--rw-r--r--   0        0        0     2231 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_transforms_post_transforms.py
--rw-r--r--   0        0        0     1324 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_transforms_post_transforms_code.py
--rw-r--r--   0        0        0     2799 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util.py
--rw-r--r--   0        0        0     3188 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_display.py
--rw-r--r--   0        0        0     3032 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_docstrings.py
--rw-r--r--   0        0        0     2647 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_docutils.py
--rw-r--r--   0        0        0     3800 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_fileutil.py
--rw-r--r--   0        0        0     8627 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_i18n.py
--rw-r--r--   0        0        0     2653 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_images.py
--rw-r--r--   0        0        0    26901 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_inspect.py
--rw-r--r--   0        0        0     4032 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_inventory.py
--rw-r--r--   0        0        0    13459 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_logging.py
--rw-r--r--   0        0        0     7180 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_matching.py
--rw-r--r--   0        0        0     7464 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_nodes.py
--rw-r--r--   0        0        0     7333 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_rst.py
--rw-r--r--   0        0        0      952 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_template.py
--rw-r--r--   0        0        0    22811 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_util_typing.py
--rw-r--r--   0        0        0     3561 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_versioning.py
--rw-r--r--   0        0        0     1065 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/test_writer_latex.py
--rw-r--r--   0        0        0     1859 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/typing_test_data.py
--rw-r--r--   0        0        0     1663 2023-07-27 20:41:03.095622 sphinx-7.1.1/tests/utils.py
--rw-r--r--   0        0        0      992 2023-07-27 20:41:03.095622 sphinx-7.1.1/tox.ini
--rw-r--r--   0        0        0      226 2023-07-27 20:41:03.095622 sphinx-7.1.1/utils/CHANGES_template
--rw-r--r--   0        0        0        0 2023-07-27 20:41:03.095622 sphinx-7.1.1/utils/__init__.py
--rw-r--r--   0        0        0     8358 2023-07-27 20:41:03.095622 sphinx-7.1.1/utils/babel_runner.py
--rwxr-xr-x   0        0        0      296 2023-07-27 20:41:03.095622 sphinx-7.1.1/utils/bump_docker.sh
--rwxr-xr-x   0        0        0     5808 2023-07-27 20:41:03.095622 sphinx-7.1.1/utils/bump_version.py
--rw-r--r--   0        0        0     1697 2023-07-27 20:41:03.095622 sphinx-7.1.1/utils/release-checklist
--rw-r--r--   0        0        0     5807 1970-01-01 00:00:00.000000 sphinx-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3818 2023-08-02 02:05:35.978913 sphinx-7.1.2/AUTHORS
+-rw-r--r--   0        0        0   374445 2023-08-02 02:05:35.982913 sphinx-7.1.2/CHANGES
+-rw-r--r--   0        0        0     3530 2023-08-02 02:05:35.982913 sphinx-7.1.2/CODE_OF_CONDUCT
+-rw-r--r--   0        0        0    26147 2023-08-02 02:05:35.982913 sphinx-7.1.2/EXAMPLES
+-rw-r--r--   0        0        0     3135 2023-08-02 02:05:35.982913 sphinx-7.1.2/LICENSE
+-rw-r--r--   0        0        0     2323 2023-08-02 02:05:35.982913 sphinx-7.1.2/README.rst
+-rw-r--r--   0        0        0      607 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/Makefile
+-rw-r--r--   0        0        0      152 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/Makefile
+-rw-r--r--   0        0        0    27523 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/bookcover.png
+-rw-r--r--   0        0        0     9875 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/conf.py.txt
+-rw-r--r--   0        0        0     3307 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/favicon.svg
+-rw-r--r--   0        0        0     1351 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/more.png
+-rw-r--r--   0        0        0    34213 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/sphinx.png
+-rw-r--r--   0        0        0    25792 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/themes/agogo.png
+-rw-r--r--   0        0        0    32356 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/themes/alabaster.png
+-rw-r--r--   0        0        0    27139 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/themes/bizstyle.png
+-rw-r--r--   0        0        0    39927 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/themes/classic.png
+-rw-r--r--   0        0        0    56954 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/themes/fullsize/agogo.png
+-rw-r--r--   0        0        0    40248 2023-08-02 02:05:35.982913 sphinx-7.1.2/doc/_static/themes/fullsize/alabaster.png
+-rw-r--r--   0        0        0    75192 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/bizstyle.png
+-rw-r--r--   0        0        0    72597 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/classic.png
+-rw-r--r--   0        0        0    84200 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/haiku.png
+-rw-r--r--   0        0        0    32266 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/nature.png
+-rw-r--r--   0        0        0   102717 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/pyramid.png
+-rw-r--r--   0        0        0    88111 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/scrolls.png
+-rw-r--r--   0        0        0    39411 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/sphinx_rtd_theme.png
+-rw-r--r--   0        0        0    84439 2023-08-02 02:05:35.986913 sphinx-7.1.2/doc/_static/themes/fullsize/sphinxdoc.png
+-rw-r--r--   0        0        0    91744 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/fullsize/traditional.png
+-rw-r--r--   0        0        0    43184 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/haiku.png
+-rw-r--r--   0        0        0    28536 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/nature.png
+-rw-r--r--   0        0        0    38805 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/pyramid.png
+-rw-r--r--   0        0        0    27800 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/scrolls.png
+-rw-r--r--   0        0        0    29138 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/sphinx_rtd_theme.png
+-rw-r--r--   0        0        0    30225 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/sphinxdoc.png
+-rw-r--r--   0        0        0    32258 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/themes/traditional.png
+-rw-r--r--   0        0        0    16371 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/translation.png
+-rw-r--r--   0        0        0      342 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/translation.puml
+-rw-r--r--   0        0        0     8232 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/translation.svg
+-rw-r--r--   0        0        0    26500 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/tutorial/lumache-autosummary.png
+-rw-r--r--   0        0        0    52126 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/tutorial/lumache-first-light.png
+-rw-r--r--   0        0        0    51223 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/tutorial/lumache-furo.png
+-rw-r--r--   0        0        0    71741 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/tutorial/lumache-py-function-full.png
+-rw-r--r--   0        0        0    41828 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_static/tutorial/lumache-py-function.png
+-rw-r--r--   0        0        0      225 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_templates/contents.html
+-rw-r--r--   0        0        0     1860 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_themes/sphinx13/layout.html
+-rw-r--r--   0        0        0     6552 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_themes/sphinx13/static/sphinx13.css
+-rw-r--r--   0        0        0    11719 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_themes/sphinx13/static/sphinxheader.png
+-rw-r--r--   0        0        0       60 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/_themes/sphinx13/theme.conf
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/authors.rst
+-rw-r--r--   0        0        0      400 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/changes.rst
+-rw-r--r--   0        0        0     9027 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/conf.py
+-rw-r--r--   0        0        0     1151 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/builders.rst
+-rw-r--r--   0        0        0      649 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/index.rst
+-rw-r--r--   0        0        0     1051 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/overview.rst
+-rw-r--r--   0        0        0    15048 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/templating.rst
+-rw-r--r--   0        0        0    12324 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/theming.rst
+-rw-r--r--   0        0        0     4020 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/tutorials/autodoc_ext.rst
+-rw-r--r--   0        0        0      438 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/tutorials/examples/README.rst
+-rw-r--r--   0        0        0     1802 2023-08-02 02:05:35.990913 sphinx-7.1.2/doc/development/tutorials/examples/autodoc_intenum.py
+-rw-r--r--   0        0        0      400 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/development/tutorials/examples/helloworld.py
+-rw-r--r--   0        0        0     5030 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/development/tutorials/examples/recipe.py
+-rw-r--r--   0        0        0     3942 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/development/tutorials/examples/todo.py
+-rw-r--r--   0        0        0     5289 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/development/tutorials/helloworld.rst
+-rw-r--r--   0        0        0      262 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/development/tutorials/index.rst
+-rw-r--r--   0        0        0     8216 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/development/tutorials/recipe.rst
+-rw-r--r--   0        0        0    13435 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/development/tutorials/todo.rst
+-rw-r--r--   0        0        0       54 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/examples.rst
+-rw-r--r--   0        0        0    14235 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/appapi.rst
+-rw-r--r--   0        0        0     1103 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/builderapi.rst
+-rw-r--r--   0        0        0      165 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/collectorapi.rst
+-rw-r--r--   0        0        0    40815 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/deprecated.rst
+-rw-r--r--   0        0        0      518 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/domainapi.rst
+-rw-r--r--   0        0        0     1043 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/envapi.rst
+-rw-r--r--   0        0        0     2817 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/i18n.rst
+-rw-r--r--   0        0        0     8597 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/index.rst
+-rw-r--r--   0        0        0     2384 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/logging.rst
+-rw-r--r--   0        0        0     4787 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/markupapi.rst
+-rw-r--r--   0        0        0     1563 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/nodes.rst
+-rw-r--r--   0        0        0     1243 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/parserapi.rst
+-rw-r--r--   0        0        0      114 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/projectapi.rst
+-rw-r--r--   0        0        0      943 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/extdev/utils.rst
+-rw-r--r--   0        0        0    13425 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/faq.rst
+-rw-r--r--   0        0        0     4173 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/glossary.rst
+-rw-r--r--   0        0        0     3539 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/index.rst
+-rw-r--r--   0        0        0       71 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/internals/code-of-conduct.rst
+-rw-r--r--   0        0        0    11482 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/internals/contributing.rst
+-rw-r--r--   0        0        0      353 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/internals/index.rst
+-rw-r--r--   0        0        0     1964 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/internals/organization.rst
+-rw-r--r--   0        0        0     4395 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/internals/release-process.rst
+-rw-r--r--   0        0        0    69427 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/latex.rst
+-rw-r--r--   0        0        0      784 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/make.bat
+-rw-r--r--   0        0        0      314 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/man/index.rst
+-rw-r--r--   0        0        0     4508 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/man/sphinx-apidoc.rst
+-rw-r--r--   0        0        0     2122 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/man/sphinx-autogen.rst
+-rw-r--r--   0        0        0    10673 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/man/sphinx-build.rst
+-rw-r--r--   0        0        0     3692 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/man/sphinx-quickstart.rst
+-rw-r--r--   0        0        0      806 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/support.rst
+-rw-r--r--   0        0        0     4981 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/automatic-doc-generation.rst
+-rw-r--r--   0        0        0    11036 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/deploying.rst
+-rw-r--r--   0        0        0     9134 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/describing-code.rst
+-rw-r--r--   0        0        0      240 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/end.rst
+-rw-r--r--   0        0        0     3450 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/first-steps.rst
+-rw-r--r--   0        0        0     3723 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/getting-started.rst
+-rw-r--r--   0        0        0     1433 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/index.rst
+-rw-r--r--   0        0        0     2528 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/more-sphinx-customization.rst
+-rw-r--r--   0        0        0     4177 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/tutorial/narrative-documentation.rst
+-rw-r--r--   0        0        0    11831 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/usage/advanced/intl.rst
+-rw-r--r--   0        0        0     2670 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/usage/advanced/websupport/api.rst
+-rw-r--r--   0        0        0      302 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/usage/advanced/websupport/index.rst
+-rw-r--r--   0        0        0     9640 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/usage/advanced/websupport/quickstart.rst
+-rw-r--r--   0        0        0     1368 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/usage/advanced/websupport/searchadapters.rst
+-rw-r--r--   0        0        0     1231 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/usage/advanced/websupport/storagebackends.rst
+-rw-r--r--   0        0        0    17742 2023-08-02 02:05:35.994913 sphinx-7.1.2/doc/usage/builders/index.rst
+-rw-r--r--   0        0        0   103777 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/configuration.rst
+-rw-r--r--   0        0        0    29861 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/autodoc.rst
+-rw-r--r--   0        0        0     1899 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/autosectionlabel.rst
+-rw-r--r--   0        0        0    11098 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/autosummary.rst
+-rw-r--r--   0        0        0     1584 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/coverage.rst
+-rw-r--r--   0        0        0    11838 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/doctest.rst
+-rw-r--r--   0        0        0      404 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/duration.rst
+-rw-r--r--   0        0        0     9665 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/example_google.py
+-rw-r--r--   0        0        0      296 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/example_google.rst
+-rw-r--r--   0        0        0     9714 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/example_numpy.py
+-rw-r--r--   0        0        0      292 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/example_numpy.rst
+-rw-r--r--   0        0        0     2781 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/extlinks.rst
+-rw-r--r--   0        0        0      491 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/githubpages.rst
+-rw-r--r--   0        0        0     6292 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/graphviz.rst
+-rw-r--r--   0        0        0     1329 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/ifconfig.rst
+-rw-r--r--   0        0        0     1705 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/imgconverter.rst
+-rw-r--r--   0        0        0     2410 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/index.rst
+-rw-r--r--   0        0        0     5594 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/inheritance.rst
+-rw-r--r--   0        0        0     9934 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/intersphinx.rst
+-rw-r--r--   0        0        0     1756 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/linkcode.rst
+-rw-r--r--   0        0        0    11756 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/math.rst
+-rw-r--r--   0        0        0    15980 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/napoleon.rst
+-rw-r--r--   0        0        0     1644 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/todo.rst
+-rw-r--r--   0        0        0     3748 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/extensions/viewcode.rst
+-rw-r--r--   0        0        0      537 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/index.rst
+-rw-r--r--   0        0        0     7146 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/installation.rst
+-rw-r--r--   0        0        0     1584 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/markdown.rst
+-rw-r--r--   0        0        0    13150 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/quickstart.rst
+-rw-r--r--   0        0        0    20508 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/restructuredtext/basics.rst
+-rw-r--r--   0        0        0    46040 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/restructuredtext/directives.rst
+-rw-r--r--   0        0        0    68349 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/restructuredtext/domains.rst
+-rw-r--r--   0        0        0     1967 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/restructuredtext/field-lists.rst
+-rw-r--r--   0        0        0      574 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/restructuredtext/index.rst
+-rw-r--r--   0        0        0    18409 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/restructuredtext/roles.rst
+-rw-r--r--   0        0        0    14326 2023-08-02 02:05:35.998913 sphinx-7.1.2/doc/usage/theming.rst
+-rw-r--r--   0        0        0    11978 2023-08-02 02:05:36.002913 sphinx-7.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1829 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/__init__.py
+-rw-r--r--   0        0        0      103 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/__main__.py
+-rw-r--r--   0        0        0    18542 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/addnodes.py
+-rw-r--r--   0        0        0    56034 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/application.py
+-rw-r--r--   0        0        0    26829 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/__init__.py
+-rw-r--r--   0        0        0    28959 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/_epub_base.py
+-rw-r--r--   0        0        0     6474 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/changes.py
+-rw-r--r--   0        0        0     1504 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/dirhtml.py
+-rw-r--r--   0        0        0      982 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/dummy.py
+-rw-r--r--   0        0        0    11284 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/epub3.py
+-rw-r--r--   0        0        0    11240 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/gettext.py
+-rw-r--r--   0        0        0    59168 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/html/__init__.py
+-rw-r--r--   0        0        0     2525 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/html/transforms.py
+-rw-r--r--   0        0        0    24206 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/latex/__init__.py
+-rw-r--r--   0        0        0     7365 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/latex/constants.py
+-rw-r--r--   0        0        0      866 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/latex/nodes.py
+-rw-r--r--   0        0        0     4445 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/latex/theming.py
+-rw-r--r--   0        0        0    20998 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/latex/transforms.py
+-rw-r--r--   0        0        0     1703 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/latex/util.py
+-rw-r--r--   0        0        0    24579 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/linkcheck.py
+-rw-r--r--   0        0        0     4511 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/manpage.py
+-rw-r--r--   0        0        0     7425 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/singlehtml.py
+-rw-r--r--   0        0        0     9666 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/texinfo.py
+-rw-r--r--   0        0        0     2870 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/text.py
+-rw-r--r--   0        0        0     3766 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/builders/xml.py
+-rw-r--r--   0        0        0       44 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/cmd/__init__.py
+-rw-r--r--   0        0        0    13671 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/cmd/build.py
+-rw-r--r--   0        0        0     6552 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/cmd/make_mode.py
+-rw-r--r--   0        0        0    23835 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/cmd/quickstart.py
+-rw-r--r--   0        0        0    22727 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/config.py
+-rw-r--r--   0        0        0     1816 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/deprecation.py
+-rw-r--r--   0        0        0    13518 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/directives/__init__.py
+-rw-r--r--   0        0        0    18354 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/directives/code.py
+-rw-r--r--   0        0        0    14672 2023-08-02 02:05:36.002913 sphinx-7.1.2/sphinx/directives/other.py
+-rw-r--r--   0        0        0     6781 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/directives/patches.py
+-rw-r--r--   0        0        0    15270 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/__init__.py
+-rw-r--r--   0        0        0   151650 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/c.py
+-rw-r--r--   0        0        0     5524 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/changeset.py
+-rw-r--r--   0        0        0     5676 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/citation.py
+-rw-r--r--   0        0        0   330776 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/cpp.py
+-rw-r--r--   0        0        0     4140 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/index.py
+-rw-r--r--   0        0        0    18920 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/javascript.py
+-rw-r--r--   0        0        0     5459 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/math.py
+-rw-r--r--   0        0        0    70913 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/python.py
+-rw-r--r--   0        0        0    10366 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/rst.py
+-rw-r--r--   0        0        0    45842 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/domains/std.py
+-rw-r--r--   0        0        0    30449 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/environment/__init__.py
+-rw-r--r--   0        0        0       34 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/environment/adapters/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/environment/adapters/asset.py
+-rw-r--r--   0        0        0     7503 2023-08-02 02:05:36.006913 sphinx-7.1.2/sphinx/environment/adapters/indexentries.py
+-rw-r--r--   0        0        0    16455 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/environment/adapters/toctree.py
+-rw-r--r--   0        0        0     2784 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/environment/collectors/__init__.py
+-rw-r--r--   0        0        0     6161 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/environment/collectors/asset.py
+-rw-r--r--   0        0        0     1887 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/environment/collectors/dependencies.py
+-rw-r--r--   0        0        0     2609 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/environment/collectors/metadata.py
+-rw-r--r--   0        0        0     2144 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/environment/collectors/title.py
+-rw-r--r--   0        0        0    15869 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/environment/collectors/toctree.py
+-rw-r--r--   0        0        0     3388 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/errors.py
+-rw-r--r--   0        0        0     4230 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/events.py
+-rw-r--r--   0        0        0       57 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/__init__.py
+-rw-r--r--   0        0        0    19197 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/apidoc.py
+-rw-r--r--   0        0        0   114320 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autodoc/__init__.py
+-rw-r--r--   0        0        0     5925 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autodoc/directive.py
+-rw-r--r--   0        0        0    11371 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autodoc/importer.py
+-rw-r--r--   0        0        0     5907 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autodoc/mock.py
+-rw-r--r--   0        0        0     4664 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autodoc/preserve_defaults.py
+-rw-r--r--   0        0        0     5406 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autodoc/type_comment.py
+-rw-r--r--   0        0        0     7789 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autodoc/typehints.py
+-rw-r--r--   0        0        0     2292 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autosectionlabel.py
+-rw-r--r--   0        0        0    31056 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autosummary/__init__.py
+-rw-r--r--   0        0        0    26212 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autosummary/generate.py
+-rw-r--r--   0        0        0      106 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autosummary/templates/autosummary/base.rst
+-rw-r--r--   0        0        0      553 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autosummary/templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1071 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/autosummary/templates/autosummary/module.rst
+-rw-r--r--   0        0        0    14065 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/coverage.py
+-rw-r--r--   0        0        0    22645 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/doctest.py
+-rw-r--r--   0        0        0     2883 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/duration.py
+-rw-r--r--   0        0        0     4523 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/extlinks.py
+-rw-r--r--   0        0        0     1962 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/githubpages.py
+-rw-r--r--   0        0        0    15843 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/graphviz.py
+-rw-r--r--   0        0        0     2517 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/ifconfig.py
+-rw-r--r--   0        0        0     3582 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/imgconverter.py
+-rw-r--r--   0        0        0    15117 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/imgmath.py
+-rw-r--r--   0        0        0    17031 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/inheritance_diagram.py
+-rw-r--r--   0        0        0    28825 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/intersphinx.py
+-rw-r--r--   0        0        0     2253 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/linkcode.py
+-rw-r--r--   0        0        0     5182 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/mathjax.py
+-rw-r--r--   0        0        0    17936 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/napoleon/__init__.py
+-rw-r--r--   0        0        0    48417 2023-08-02 02:05:36.010913 sphinx-7.1.2/sphinx/ext/napoleon/docstring.py
+-rw-r--r--   0        0        0     8017 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/ext/todo.py
+-rw-r--r--   0        0        0    12900 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/ext/viewcode.py
+-rw-r--r--   0        0        0     2995 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/extension.py
+-rw-r--r--   0        0        0     6986 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/highlighting.py
+-rw-r--r--   0        0        0     6148 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/io.py
+-rw-r--r--   0        0        0     7107 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/jinja2glue.py
+-rw-r--r--   0        0        0      165 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/.tx/config
+-rw-r--r--   0        0        0     7135 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/__init__.py
+-rw-r--r--   0        0        0     3494 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/ar/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7688 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/ar/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87237 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/ar/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/bg/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      492 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/bg/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83916 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/bg/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     5977 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/bn/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7699 2023-08-02 02:05:36.014913 sphinx-7.1.2/sphinx/locale/bn/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87859 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/bn/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4029 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/ca/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    84317 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/ca/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   123185 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/ca/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2385 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cak/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2391 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cak/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84630 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cak/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3976 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cs/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8071 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cs/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86669 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cs/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3411 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cy/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6018 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cy/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85933 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/cy/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3578 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/da/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    12705 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/da/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88403 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/da/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3533 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/de/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    11026 2023-08-02 02:05:36.018913 sphinx-7.1.2/sphinx/locale/de/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88020 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/de/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      505 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/de_DE/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83929 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     8758 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/el/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    81252 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/el/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   131807 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/el/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      506 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_DE/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83930 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2302 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      462 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_FR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83929 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3630 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    76610 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   115479 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      508 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_HK/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83932 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2457 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/eo/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     1864 2023-08-02 02:05:36.022913 sphinx-7.1.2/sphinx/locale/eo/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84412 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/eo/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4155 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/es/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    81886 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/es/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   121969 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/es/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2342 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      546 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83970 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3615 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/et/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    33298 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/et/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    97534 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/et/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3102 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/eu/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6589 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/eu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86099 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/eu/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     7551 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/fa/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    98068 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/fa/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   139504 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/fa/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2787 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/fi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2912 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/fi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84716 2023-08-02 02:05:36.026913 sphinx-7.1.2/sphinx/locale/fi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4162 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/fr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    84318 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/fr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   124974 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/fr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2354 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      555 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83979 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4885 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/he/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     4905 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/he/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85734 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/he/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     7427 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    97733 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   146555 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      502 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83926 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3621 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    16774 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    90233 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3980 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hu/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    11338 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88363 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/hu/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3465 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/id/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    60908 2023-08-02 02:05:36.030913 sphinx-7.1.2/sphinx/locale/id/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   109854 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/id/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2825 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/is/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     3082 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/is/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84836 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/is/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3579 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/it/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    10427 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/it/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87816 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/it/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4957 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ja/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    86746 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ja/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   128634 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ja/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6108 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ka/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    74576 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ka/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   131640 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ka/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4807 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ko/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    83303 2023-08-02 02:05:36.034913 sphinx-7.1.2/sphinx/locale/ko/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   123022 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/ko/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3473 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/lt/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6907 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/lt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86276 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/lt/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3445 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/lv/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6585 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/lv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85991 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/lv/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2415 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/mk/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2011 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/mk/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84606 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/mk/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3108 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6578 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85808 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6223 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/ne/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8635 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/ne/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88030 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/ne/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3489 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/nl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    19033 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/nl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    91591 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/nl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3819 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    29289 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    96177 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2351 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pt/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      544 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83968 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pt/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4219 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    82142 2023-08-02 02:05:36.038913 sphinx-7.1.2/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   121242 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3745 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7847 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86646 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3700 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/ro/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8628 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/ro/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86951 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/ro/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     8165 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/ru/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    15898 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/ru/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    91959 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/ru/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3816 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/si/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     3560 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/si/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85398 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/si/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4117 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sk/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    67002 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sk/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   113035 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sk/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3185 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5228 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85484 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0    84079 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sphinx.pot
+-rw-r--r--   0        0        0     4216 2023-08-02 02:05:36.042913 sphinx-7.1.2/sphinx/locale/sq/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    79775 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sq/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   120606 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sq/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4100 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     9193 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88044 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2380 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      584 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84008 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2382 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      579 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84003 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3281 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sv/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6568 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85829 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/sv/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/ta/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      647 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/ta/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84076 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/ta/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/te/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      489 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/te/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83913 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/te/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3937 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/tr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    57535 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/tr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   109424 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/tr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6283 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6461 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86919 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/ur/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      487 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/ur/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83994 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/ur/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3520 2023-08-02 02:05:36.046913 sphinx-7.1.2/sphinx/locale/vi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5771 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/vi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85912 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/vi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2294 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/yue/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      487 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/yue/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83911 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/yue/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4318 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    76477 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   115904 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2301 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      501 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83925 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2301 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      516 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    83940 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4451 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    74917 2023-08-02 02:05:36.050913 sphinx-7.1.2/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   114627 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3098 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/parsers.py
+-rw-r--r--   0        0        0     3432 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/project.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/py.typed
+-rw-r--r--   0        0        0     5581 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/pycode/__init__.py
+-rw-r--r--   0        0        0     6648 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/pycode/ast.py
+-rw-r--r--   0        0        0    21346 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/pycode/parser.py
+-rw-r--r--   0        0        0     2861 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/pygments_styles.py
+-rw-r--r--   0        0        0    22138 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/registry.py
+-rw-r--r--   0        0        0    15975 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/roles.py
+-rw-r--r--   0        0        0    22183 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/__init__.py
+-rw-r--r--   0        0        0     3561 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/da.py
+-rw-r--r--   0        0        0     4637 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/de.py
+-rw-r--r--   0        0        0     4899 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/en.py
+-rw-r--r--   0        0        0     5723 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/es.py
+-rw-r--r--   0        0        0     3207 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/fi.py
+-rw-r--r--   0        0        0     3438 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/fr.py
+-rw-r--r--   0        0        0     1949 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/hu.py
+-rw-r--r--   0        0        0     5089 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/it.py
+-rw-r--r--   0        0        0    30997 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/ja.py
+-rw-r--r--   0        0        0     3594 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/base-stemmer.js
+-rw-r--r--   0        0        0     3123 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/danish-stemmer.js
+-rw-r--r--   0        0        0     5529 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/dutch-stemmer.js
+-rw-r--r--   0        0        0     7529 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/finnish-stemmer.js
+-rw-r--r--   0        0        0    11571 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/french-stemmer.js
+-rw-r--r--   0        0        0     4669 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/german-stemmer.js
+-rw-r--r--   0        0        0     6614 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/hungarian-stemmer.js
+-rw-r--r--   0        0        0     9100 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/italian-stemmer.js
+-rw-r--r--   0        0        0     2594 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/norwegian-stemmer.js
+-rw-r--r--   0        0        0     6439 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/porter-stemmer.js
+-rw-r--r--   0        0        0     8373 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/portuguese-stemmer.js
+-rw-r--r--   0        0        0     8333 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/romanian-stemmer.js
+-rw-r--r--   0        0        0     5735 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/russian-stemmer.js
+-rw-r--r--   0        0        0     9121 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/spanish-stemmer.js
+-rw-r--r--   0        0        0     2654 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/swedish-stemmer.js
+-rw-r--r--   0        0        0    19972 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/minified-js/turkish-stemmer.js
+-rw-r--r--   0        0        0     4571 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/nl.py
+-rw-r--r--   0        0        0     4893 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/no.py
+-rw-r--r--   0        0        0     8133 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/non-minified-js/base-stemmer.js
+-rw-r--r--   0        0        0     8134 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/non-minified-js/danish-stemmer.js
+-rw-r--r--   0        0        0    19495 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/non-minified-js/dutch-stemmer.js
+-rw-r--r--   0        0        0    21286 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/non-minified-js/finnish-stemmer.js
+-rw-r--r--   0        0        0    42080 2023-08-02 02:05:36.054913 sphinx-7.1.2/sphinx/search/non-minified-js/french-stemmer.js
+-rw-r--r--   0        0        0    17647 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/german-stemmer.js
+-rw-r--r--   0        0        0    17564 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/hungarian-stemmer.js
+-rw-r--r--   0        0        0    29065 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/italian-stemmer.js
+-rw-r--r--   0        0        0     6870 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/norwegian-stemmer.js
+-rw-r--r--   0        0        0    20391 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/porter-stemmer.js
+-rw-r--r--   0        0        0    26718 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/portuguese-stemmer.js
+-rw-r--r--   0        0        0    25006 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/romanian-stemmer.js
+-rw-r--r--   0        0        0    17996 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/russian-stemmer.js
+-rw-r--r--   0        0        0    28534 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/spanish-stemmer.js
+-rw-r--r--   0        0        0     6851 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/swedish-stemmer.js
+-rw-r--r--   0        0        0    77511 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/non-minified-js/turkish-stemmer.js
+-rw-r--r--   0        0        0     4648 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/pt.py
+-rw-r--r--   0        0        0      557 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/ro.py
+-rw-r--r--   0        0        0     7905 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/ru.py
+-rw-r--r--   0        0        0     3436 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/sv.py
+-rw-r--r--   0        0        0      551 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/tr.py
+-rw-r--r--   0        0        0     6146 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/search/zh.py
+-rw-r--r--   0        0        0      196 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/apidoc/module.rst_t
+-rw-r--r--   0        0        0     1173 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/apidoc/package.rst_t
+-rw-r--r--   0        0        0      128 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/apidoc/toc.rst_t
+-rw-r--r--   0        0        0      246 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/epub3/container.xml
+-rw-r--r--   0        0        0     2127 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/epub3/content.opf_t
+-rw-r--r--   0        0        0       20 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/epub3/mimetype
+-rw-r--r--   0        0        0      629 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/epub3/nav.xhtml_t
+-rw-r--r--   0        0        0      743 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/epub3/toc.ncx_t
+-rw-r--r--   0        0        0      875 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/gettext/message.pot_t
+-rw-r--r--   0        0        0      299 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/graphviz/graphviz.css
+-rw-r--r--   0        0        0      864 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/htmlhelp/project.hhc
+-rw-r--r--   0        0        0      570 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/htmlhelp/project.hhp
+-rw-r--r--   0        0        0      165 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/htmlhelp/project.stp
+-rw-r--r--   0        0        0      397 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/imgmath/preview.tex_t
+-rw-r--r--   0        0        0      321 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/imgmath/template.tex_t
+-rw-r--r--   0        0        0     2986 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/latex/latex.tex_t
+-rw-r--r--   0        0        0     2156 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/latex/longtable.tex_t
+-rw-r--r--   0        0        0      944 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/latex/sphinxmessages.sty_t
+-rw-r--r--   0        0        0     1406 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/latex/tabular.tex_t
+-rw-r--r--   0        0        0     1420 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/latex/tabulary.tex_t
+-rw-r--r--   0        0        0      656 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/quickstart/Makefile.new_t
+-rw-r--r--   0        0        0     4031 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/quickstart/Makefile_t
+-rw-r--r--   0        0        0     2129 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/quickstart/conf.py_t
+-rw-r--r--   0        0        0      787 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/quickstart/make.bat.new_t
+-rw-r--r--   0        0        0     3293 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/quickstart/make.bat_t
+-rw-r--r--   0        0        0      492 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/quickstart/root_doc.rst_t
+-rw-r--r--   0        0        0     1423 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/templates/texinfo/Makefile
+-rw-r--r--   0        0        0      171 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/testing/__init__.py
+-rw-r--r--   0        0        0     2710 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/testing/comparer.py
+-rw-r--r--   0        0        0     7508 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/testing/fixtures.py
+-rw-r--r--   0        0        0     6317 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/testing/path.py
+-rw-r--r--   0        0        0     1029 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/testing/restructuredtext.py
+-rw-r--r--   0        0        0     7498 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/testing/util.py
+-rw-r--r--   0        0        0     4366 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/LICRcyr2utf8.xdy
+-rw-r--r--   0        0        0    10188 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/LICRlatin2utf8.xdy
+-rw-r--r--   0        0        0    18890 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/LatinRules.xdy
+-rw-r--r--   0        0        0     2401 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/Makefile_t
+-rw-r--r--   0        0        0      695 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/latexmkjarc_t
+-rw-r--r--   0        0        0     1104 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/latexmkrc_t
+-rw-r--r--   0        0        0     1041 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/make.bat_t
+-rw-r--r--   0        0        0      392 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/python.ist
+-rw-r--r--   0        0        0    44560 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinx.sty
+-rw-r--r--   0        0        0     9474 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinx.xdy
+-rw-r--r--   0        0        0     3256 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinxhowto.cls
+-rw-r--r--   0        0        0    10989 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexadmonitions.sty
+-rw-r--r--   0        0        0      901 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexcontainers.sty
+-rw-r--r--   0        0        0     4840 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexgraphics.sty
+-rw-r--r--   0        0        0     2066 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexindbibtoc.sty
+-rw-r--r--   0        0        0     5139 2023-08-02 02:05:36.058914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexlists.sty
+-rw-r--r--   0        0        0    46048 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexliterals.sty
+-rw-r--r--   0        0        0     4532 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexnumfig.sty
+-rw-r--r--   0        0        0    14339 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexobjects.sty
+-rw-r--r--   0        0        0     5066 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexshadowbox.sty
+-rw-r--r--   0        0        0     3445 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexstyleheadings.sty
+-rw-r--r--   0        0        0     3064 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexstylepage.sty
+-rw-r--r--   0        0        0     8589 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatexstyletext.sty
+-rw-r--r--   0        0        0    57830 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxlatextables.sty
+-rw-r--r--   0        0        0     4241 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxmanual.cls
+-rw-r--r--   0        0        0     2061 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxoptionsgeometry.sty
+-rw-r--r--   0        0        0     1094 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxoptionshyperref.sty
+-rw-r--r--   0        0        0    36615 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxpackageboxes.sty
+-rw-r--r--   0        0        0     2590 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxpackagecyrillic.sty
+-rw-r--r--   0        0        0    15254 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs/sphinxpackagefootnote.sty
+-rw-r--r--   0        0        0     2503 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/texinputs_win/Makefile_t
+-rw-r--r--   0        0        0     3321 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/agogo/layout.html
+-rw-r--r--   0        0        0     9144 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/agogo/static/agogo.css_t
+-rw-r--r--   0        0        0      276 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/agogo/static/bgfooter.png
+-rw-r--r--   0        0        0      266 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/agogo/static/bgtop.png
+-rw-r--r--   0        0        0      477 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/agogo/theme.conf
+-rw-r--r--   0        0        0      466 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/changes/frameset.html
+-rw-r--r--   0        0        0      485 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/changes/rstsource.html
+-rw-r--r--   0        0        0     1306 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/changes/versionchanges.html
+-rw-r--r--   0        0        0     1636 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/defindex.html
+-rw-r--r--   0        0        0     1892 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/domainindex.html
+-rw-r--r--   0        0        0     1804 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/genindex-single.html
+-rw-r--r--   0        0        0     1210 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/genindex-split.html
+-rw-r--r--   0        0        0     2069 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/genindex.html
+-rw-r--r--   0        0        0      432 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/globaltoc.html
+-rw-r--r--   0        0        0     7634 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/layout.html
+-rw-r--r--   0        0        0      370 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/localtoc.html
+-rw-r--r--   0        0        0      679 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/opensearch.xml
+-rw-r--r--   0        0        0      273 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/page.html
+-rw-r--r--   0        0        0      652 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/relations.html
+-rw-r--r--   0        0        0     2039 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/search.html
+-rw-r--r--   0        0        0      809 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/searchbox.html
+-rw-r--r--   0        0        0      947 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/searchfield.html
+-rw-r--r--   0        0        0      544 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/sourcelink.html
+-rw-r--r--   0        0        0    15139 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/basic.css_t
+-rw-r--r--   0        0        0     4472 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/doctools.js
+-rw-r--r--   0        0        0      673 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/documentation_options.js_t
+-rw-r--r--   0        0        0      286 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/file.png
+-rw-r--r--   0        0        0      676 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/language_data.js_t
+-rw-r--r--   0        0        0       90 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/minus.png
+-rw-r--r--   0        0        0       90 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/plus.png
+-rw-r--r--   0        0        0    18215 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/static/sphinx_highlight.js
+-rw-r--r--   0        0        0      371 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/basic/theme.conf
+-rw-r--r--   0        0        0      664 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/bizstyle/layout.html
+-rw-r--r--   0        0        0       78 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/bizstyle/static/background_b01.png
+-rw-r--r--   0        0        0    10314 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/bizstyle/static/bizstyle.css_t
+-rw-r--r--   0        0        0     1129 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/bizstyle/static/bizstyle.js_t
+-rw-r--r--   0        0        0    14940 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/bizstyle/static/css3-mediaqueries.js
+-rw-r--r--   0        0        0    28634 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js
+-rw-r--r--   0        0        0      148 2023-08-02 02:05:36.062914 sphinx-7.1.2/sphinx/themes/bizstyle/theme.conf
+-rw-r--r--   0        0        0      661 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/classic/layout.html
+-rw-r--r--   0        0        0     6635 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/classic/static/classic.css_t
+-rw-r--r--   0        0        0     2659 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/classic/static/sidebar.js_t
+-rw-r--r--   0        0        0      719 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/classic/theme.conf
+-rw-r--r--   0        0        0       28 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/default/static/default.css
+-rw-r--r--   0        0        0       26 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/default/theme.conf
+-rw-r--r--   0        0        0      693 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/epub/epub-cover.html
+-rw-r--r--   0        0        0      543 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/epub/layout.html
+-rw-r--r--   0        0        0    12378 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/epub/static/epub.css_t
+-rw-r--r--   0        0        0      108 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/epub/theme.conf
+-rw-r--r--   0        0        0     2012 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/haiku/layout.html
+-rw-r--r--   0        0        0     1128 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/haiku/static/alert_info_32.png
+-rw-r--r--   0        0        0      944 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/haiku/static/alert_warning_32.png
+-rw-r--r--   0        0        0       82 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/haiku/static/bg-page.png
+-rw-r--r--   0        0        0      165 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/haiku/static/bullet_orange.png
+-rw-r--r--   0        0        0     7059 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/haiku/static/haiku.css_t
+-rw-r--r--   0        0        0      298 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/haiku/theme.conf
+-rw-r--r--   0        0        0     4234 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/nature/static/nature.css_t
+-rw-r--r--   0        0        0       71 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/nature/theme.conf
+-rw-r--r--   0        0        0      642 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/nonav/layout.html
+-rw-r--r--   0        0        0     9636 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/nonav/static/nonav.css_t
+-rw-r--r--   0        0        0      109 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/nonav/theme.conf
+-rw-r--r--   0        0        0      875 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/layout.html
+-rw-r--r--   0        0        0     1394 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-note.png
+-rw-r--r--   0        0        0     1351 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-seealso.png
+-rw-r--r--   0        0        0     1186 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-todo.png
+-rw-r--r--   0        0        0     1798 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-topic.png
+-rw-r--r--   0        0        0     1280 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-warning.png
+-rw-r--r--   0        0        0     5629 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/epub.css_t
+-rw-r--r--   0        0        0      333 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/footerbg.png
+-rw-r--r--   0        0        0      190 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/headerbg.png
+-rw-r--r--   0        0        0      726 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/ie6.css
+-rw-r--r--   0        0        0      101 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/middlebg.png
+-rw-r--r--   0        0        0     6301 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/pyramid.css_t
+-rw-r--r--   0        0        0       49 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/static/transparent.gif
+-rw-r--r--   0        0        0      102 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/pyramid/theme.conf
+-rw-r--r--   0        0        0     5775 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/artwork/logo.svg
+-rw-r--r--   0        0        0     1661 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/layout.html
+-rw-r--r--   0        0        0    25238 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/darkmetal.png
+-rw-r--r--   0        0        0      172 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/headerbg.png
+-rw-r--r--   0        0        0     8305 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/logo.png
+-rw-r--r--   0        0        0     7547 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/metal.png
+-rw-r--r--   0        0        0      124 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/navigation.png
+-rw-r--r--   0        0        0      303 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/print.css
+-rw-r--r--   0        0        0     7977 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/scrolls.css_t
+-rw-r--r--   0        0        0      527 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/theme_extras.js
+-rw-r--r--   0        0        0    44483 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/watermark.png
+-rw-r--r--   0        0        0     8049 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/static/watermark_blur.png
+-rw-r--r--   0        0        0      260 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/scrolls/theme.conf
+-rw-r--r--   0        0        0      107 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/sphinxdoc/static/contents.png
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/sphinxdoc/static/navigation.png
+-rw-r--r--   0        0        0     6314 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t
+-rw-r--r--   0        0        0       77 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/sphinxdoc/theme.conf
+-rw-r--r--   0        0        0    12162 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/traditional/static/traditional.css_t
+-rw-r--r--   0        0        0      105 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/themes/traditional/theme.conf
+-rw-r--r--   0        0        0     7937 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/theming.py
+-rw-r--r--   0        0        0    15096 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/transforms/__init__.py
+-rw-r--r--   0        0        0     2768 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/transforms/compact_bullet_list.py
+-rw-r--r--   0        0        0    25668 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/transforms/i18n.py
+-rw-r--r--   0        0        0    12028 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/transforms/post_transforms/__init__.py
+-rw-r--r--   0        0        0     4486 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/transforms/post_transforms/code.py
+-rw-r--r--   0        0        0    10268 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/transforms/post_transforms/images.py
+-rw-r--r--   0        0        0     1361 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/transforms/references.py
+-rw-r--r--   0        0        0    12524 2023-08-02 02:05:36.066913 sphinx-7.1.2/sphinx/util/__init__.py
+-rw-r--r--   0        0        0      240 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/build_phase.py
+-rw-r--r--   0        0        0    15386 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/cfamily.py
+-rw-r--r--   0        0        0     3223 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/console.py
+-rw-r--r--   0        0        0     2665 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/display.py
+-rw-r--r--   0        0        0    16843 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/docfields.py
+-rw-r--r--   0        0        0     2930 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/docstrings.py
+-rw-r--r--   0        0        0    22767 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/docutils.py
+-rw-r--r--   0        0        0     1960 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/exceptions.py
+-rw-r--r--   0        0        0     3722 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/fileutil.py
+-rw-r--r--   0        0        0      513 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/http_date.py
+-rw-r--r--   0        0        0     9615 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/i18n.py
+-rw-r--r--   0        0        0     3660 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/images.py
+-rw-r--r--   0        0        0    28244 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/inspect.py
+-rw-r--r--   0        0        0     6311 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/inventory.py
+-rw-r--r--   0        0        0    18046 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/logging.py
+-rw-r--r--   0        0        0     5279 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/matching.py
+-rw-r--r--   0        0        0     1816 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/math.py
+-rw-r--r--   0        0        0    23171 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/nodes.py
+-rw-r--r--   0        0        0     6973 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/osutil.py
+-rw-r--r--   0        0        0     5023 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/parallel.py
+-rw-r--r--   0        0        0     1445 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/png.py
+-rw-r--r--   0        0        0     2428 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/requests.py
+-rw-r--r--   0        0        0     3302 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/rst.py
+-rw-r--r--   0        0        0     2651 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/tags.py
+-rw-r--r--   0        0        0     4691 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/template.py
+-rw-r--r--   0        0        0     5442 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/texescape.py
+-rw-r--r--   0        0        0    14994 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/util/typing.py
+-rw-r--r--   0        0        0     5801 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/versioning.py
+-rw-r--r--   0        0        0       31 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/__init__.py
+-rw-r--r--   0        0        0     1605 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/html.py
+-rw-r--r--   0        0        0    37087 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/html5.py
+-rw-r--r--   0        0        0    90716 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/latex.py
+-rw-r--r--   0        0        0    15917 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/manpage.py
+-rw-r--r--   0        0        0    53161 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/texinfo.py
+-rw-r--r--   0        0        0    43225 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/text.py
+-rw-r--r--   0        0        0     1472 2023-08-02 02:05:36.070914 sphinx-7.1.2/sphinx/writers/xml.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3054 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/certs/cert.pem
+-rw-r--r--   0        0        0     1574 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/conftest.py
+-rw-r--r--   0        0        0      363 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/ext_napoleon_pep526_data_google.py
+-rw-r--r--   0        0        0      385 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/ext_napoleon_pep526_data_numpy.py
+-rw-r--r--   0        0        0       34 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/js/documentation_options.js
+-rw-r--r--   0        0        0     1694 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/js/searchtools.js
+-rw-r--r--   0        0        0     1985 2023-08-02 02:05:36.070914 sphinx-7.1.2/tests/js/sphinx_highlight.js
+-rw-r--r--   0        0        0      111 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_enumerable_node/conf.py
+-rw-r--r--   0        0        0     1464 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_enumerable_node/enumerable_node.py
+-rw-r--r--   0        0        0      763 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_enumerable_node/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_enumerable_node/rimg.png
+-rw-r--r--   0        0        0      277 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_source_parser-conflicts-with-users-setting/conf.py
+-rw-r--r--   0        0        0      201 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_source_parser-conflicts-with-users-setting/source_parser.py
+-rw-r--r--   0        0        0      121 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_source_parser/conf.py
+-rw-r--r--   0        0        0      201 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-add_source_parser/source_parser.py
+-rw-r--r--   0        0        0     1659 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-api-set-translator/conf.py
+-rw-r--r--   0        0        0       72 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-api-set-translator/index.rst
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-api-set-translator/nonext/conf.py
+-rw-r--r--   0        0        0      101 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-api-set-translator/translator.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-duplicates/fish_licence/halibut.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-duplicates/fish_licence/halibut.pyx
+-rw-r--r--   0        0        0       12 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-pep420/a/b/c/__init__.py
+-rw-r--r--   0        0        0       11 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-pep420/a/b/c/d.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-pep420/a/b/e/__init__.py
+-rw-r--r--   0        0        0       11 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-pep420/a/b/e/f.py
+-rw-r--r--   0        0        0       11 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-pep420/a/b/x/y.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-subpackage-in-toc/parent/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-subpackage-in-toc/parent/child/__init__.py
+-rw-r--r--   0        0        0        6 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-subpackage-in-toc/parent/child/foo.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-toc/mypackage/__init__.py
+-rwxr-xr-x   0        0        0      404 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-toc/mypackage/main.py
+-rw-r--r--   0        0        0       79 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-toc/mypackage/no_init/foo.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-toc/mypackage/resource/__init__.py
+-rw-r--r--   0        0        0       96 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-toc/mypackage/resource/resource.txt
+-rw-r--r--   0        0        0       23 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-toc/mypackage/something/__init__.py
+-rw-r--r--   0        0        0       44 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-trailing-underscore/package_/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-apidoc-trailing-underscore/package_/module_.py
+-rw-r--r--   0        0        0      221 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-autosummary/conf.py
+-rw-r--r--   0        0        0     1335 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-autosummary/dummy_module.py
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-autosummary/index.rst
+-rw-r--r--   0        0        0      507 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-autosummary/sphinx.rst
+-rw-r--r--   0        0        0      198 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-autosummary/underscore_module_.py
+-rw-r--r--   0        0        0      114 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0     1477 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/extra.css
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/mytheme.css
+-rw-r--r--   0        0        0       60 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/theme.conf
+-rw-r--r--   0        0        0       53 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-html-theme-having-multiple-stylesheets/conf.py
+-rw-r--r--   0        0        0      100 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-html-theme-having-multiple-stylesheets/index.rst
+-rw-r--r--   0        0        0      372 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-html-translator/conf.py
+-rw-r--r--   0        0        0      252 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-html-translator/index.rst
+-rw-r--r--   0        0        0       53 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/conf.py
+-rw-r--r--   0        0        0       20 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/doc1.txt
+-rw-r--r--   0        0        0       51 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/doc2.txt
+-rw-r--r--   0        0        0      135 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/index.txt
+-rw-r--r--   0        0        0       62 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/lineblock.txt
+-rw-r--r--   0        0        0       40 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/listitems.txt
+-rw-r--r--   0        0        0      388 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/maxwidth.txt
+-rw-r--r--   0        0        0      478 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/nonascii_maxwidth.txt
+-rw-r--r--   0        0        0       75 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/nonascii_table.txt
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/nonascii_title.txt
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/table.txt
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/table_colspan.txt
+-rw-r--r--   0        0        0      140 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/table_colspan_and_rowspan.txt
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/table_colspan_left.txt
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-build-text/table_rowspan.txt
+-rw-r--r--   0        0        0       18 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-dirhtml/bar.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-dirhtml/conf.py
+-rw-r--r--   0        0        0       32 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-dirhtml/foo/foo_1.rst
+-rw-r--r--   0        0        0       32 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-dirhtml/foo/foo_2.rst
+-rw-r--r--   0        0        0       63 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-dirhtml/foo/index.rst
+-rw-r--r--   0        0        0       59 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-dirhtml/index.rst
+-rw-r--r--   0        0        0       74 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-gettext-dont-rebuild-mo/bom.rst
+-rw-r--r--   0        0        0       16 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-gettext-dont-rebuild-mo/conf.py
+-rw-r--r--   0        0        0      108 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-gettext-dont-rebuild-mo/index.rst
+-rw-r--r--   0        0        0      264 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-builder-gettext-dont-rebuild-mo/xx/LC_MESSAGES/bom.po
+-rw-r--r--   0        0        0      330 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-changes/base.rst
+-rw-r--r--   0        0        0      371 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-changes/c-api.rst
+-rw-r--r--   0        0        0      134 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-changes/conf.py
+-rw-r--r--   0        0        0      189 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-changes/contents.rst
+-rw-r--r--   0        0        0      443 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-changes/library/utils.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-circular/conf.py
+-rw-r--r--   0        0        0       22 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-circular/index.rst
+-rw-r--r--   0        0        0       23 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-circular/sub.rst
+-rw-r--r--   0        0        0       81 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-config/conf.py
+-rw-r--r--   0        0        0      155 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-copyright-multiline/conf.py
+-rw-r--r--   0        0        0       75 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-copyright-multiline/index.rst
+-rw-r--r--   0        0        0       32 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-correct-year/conf.py
+-rw-r--r--   0        0        0       55 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-correct-year/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-default_role/conf.py
+-rw-r--r--   0        0        0       29 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-default_role/foo.rst
+-rw-r--r--   0        0        0       54 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-default_role/index.rst
+-rw-r--r--   0        0        0      762 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/caption.rst
+-rw-r--r--   0        0        0      263 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/classes.rst
+-rw-r--r--   0        0        0       44 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/conf.py
+-rw-r--r--   0        0        0     1434 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/dedent.rst
+-rw-r--r--   0        0        0      170 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/emphasize.rst
+-rw-r--r--   0        0        0        3 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/empty.inc
+-rw-r--r--   0        0        0       21 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/error.inc
+-rw-r--r--   0        0        0      203 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/force.rst
+-rw-r--r--   0        0        0      345 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/highlight.rst
+-rw-r--r--   0        0        0      267 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/index.rst
+-rw-r--r--   0        0        0      349 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/linenos.rst
+-rw-r--r--   0        0        0      396 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/linenothreshold.rst
+-rw-r--r--   0        0        0      206 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/literal-diff.inc
+-rw-r--r--   0        0        0       67 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/literal-short.inc
+-rw-r--r--   0        0        0      213 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/literal.inc
+-rw-r--r--   0        0        0      421 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/namedblocks.rst
+-rw-r--r--   0        0        0      263 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/py-decorators.inc
+-rw-r--r--   0        0        0      391 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/py-decorators.rst
+-rw-r--r--   0        0        0      305 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/python.rst
+-rw-r--r--   0        0        0      355 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-code/target.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-csv-table/conf.py
+-rw-r--r--   0        0        0       12 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-csv-table/example.csv
+-rw-r--r--   0        0        0       12 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-csv-table/subdir/example.csv
+-rw-r--r--   0        0        0       62 2023-08-02 02:05:36.074914 sphinx-7.1.2/tests/roots/test-directive-only/conf.py
+-rw-r--r--   0        0        0       63 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-directive-only/index.rst
+-rw-r--r--   0        0        0     3063 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-directive-only/only.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-directives-raw/conf.py
+-rw-r--r--   0        0        0      404 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-directives-raw/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-docutilsconf/conf.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-docutilsconf/docutils.conf
+-rw-r--r--   0        0        0       89 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-docutilsconf/index.rst
+-rw-r--r--   0        0        0       65 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c-c_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      119 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c-c_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       74 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c-intersphinx/conf.py
+-rw-r--r--   0        0        0     1146 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c-intersphinx/index.rst
+-rw-r--r--   0        0        0      121 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c/anon-dup-decl.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c/conf.py
+-rw-r--r--   0        0        0       70 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c/field-role.rst
+-rw-r--r--   0        0        0      101 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c/function_param_target.rst
+-rw-r--r--   0        0        0      785 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c/index.rst
+-rw-r--r--   0        0        0      261 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c/namespace.rst
+-rw-r--r--   0        0        0      163 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-c/ns_lookup.rst
+-rw-r--r--   0        0        0       67 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      129 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       74 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp-intersphinx/conf.py
+-rw-r--r--   0        0        0     2444 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp-intersphinx/index.rst
+-rw-r--r--   0        0        0       92 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/anon-dup-decl.rst
+-rw-r--r--   0        0        0      688 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/any-role.rst
+-rw-r--r--   0        0        0       27 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/backslash.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/conf.py
+-rw-r--r--   0        0        0       59 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/field-role.rst
+-rw-r--r--   0        0        0     1136 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/index.rst
+-rw-r--r--   0        0        0      133 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/lookup-key-overload.rst
+-rw-r--r--   0        0        0      437 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/multi-decl-lookup.rst
+-rw-r--r--   0        0        0     2136 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/roles-targets-ok.rst
+-rw-r--r--   0        0        0     2406 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/roles-targets-warn.rst
+-rw-r--r--   0        0        0      697 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/roles.rst
+-rw-r--r--   0        0        0       90 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/roles2.rst
+-rw-r--r--   0        0        0      383 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/semicolon.rst
+-rw-r--r--   0        0        0      203 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/warn-template-param-qualified-name.rst
+-rw-r--r--   0        0        0      249 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-cpp/xref_consistency.rst
+-rw-r--r--   0        0        0       45 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-js-javascript_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      156 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-js-javascript_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-js/conf.py
+-rw-r--r--   0        0        0       66 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-js/index.rst
+-rw-r--r--   0        0        0      527 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-js/module.rst
+-rw-r--r--   0        0        0      886 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-js/roles.rst
+-rw-r--r--   0        0        0       41 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py-python_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      168 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py-python_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       41 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py-python_use_unqualified_type_names/conf.py
+-rw-r--r--   0        0        0      240 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py-python_use_unqualified_type_names/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py-xref-warning/conf.py
+-rw-r--r--   0        0        0      116 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py-xref-warning/index.rst
+-rw-r--r--   0        0        0      359 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py/abbr.rst
+-rw-r--r--   0        0        0      174 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py/canonical.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py/conf.py
+-rw-r--r--   0        0        0      107 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py/index.rst
+-rw-r--r--   0        0        0     1040 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py/module.rst
+-rw-r--r--   0        0        0      383 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py/module_option.rst
+-rw-r--r--   0        0        0      872 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-domain-py/roles.rst
+-rw-r--r--   0        0        0       24 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme1/theme.conf
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme2/theme.conf
+-rw-r--r--   0        0        0      127 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-double-inheriting-theme/conf.py
+-rw-r--r--   0        0        0       87 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-double-inheriting-theme/index.rst
+-rw-r--r--   0        0        0       40 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-environment-record-dependencies/api.rst
+-rw-r--r--   0        0        0       99 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-environment-record-dependencies/conf.py
+-rw-r--r--   0        0        0       38 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-environment-record-dependencies/example_module.py
+-rw-r--r--   0        0        0       22 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-environment-record-dependencies/index.rst
+-rw-r--r--   0        0        0       87 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-epub-anchor-id/conf.py
+-rw-r--r--   0        0        0      191 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-epub-anchor-id/index.rst
+-rw-r--r--   0        0        0      111 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/autodoc_dummy_bar.py
+-rw-r--r--   0        0        0       94 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/autodoc_dummy_module.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/bug2437/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/bug2437/autodoc_dummy_foo.py
+-rw-r--r--   0        0        0      215 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/conf.py
+-rw-r--r--   0        0        0      282 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/index.rst
+-rw-r--r--   0        0        0      149 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/TYPE_CHECKING.py
+-rw-r--r--   0        0        0     4363 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/__init__.py
+-rw-r--r--   0        0        0      187 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/_functions_to_import.py
+-rw-r--r--   0        0        0      428 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/abstractmethods.py
+-rw-r--r--   0        0        0      150 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/annotated.py
+-rw-r--r--   0        0        0      882 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/autoclass_content.py
+-rw-r--r--   0        0        0      665 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py
+-rw-r--r--   0        0        0      107 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/bound_method.py
+-rw-r--r--   0        0        0      219 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/cached_property.py
+-rw-r--r--   0        0        0      279 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/callable.py
+-rw-r--r--   0        0        0       47 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/canonical/__init__.py
+-rw-r--r--   0        0        0      158 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/canonical/original.py
+-rw-r--r--   0        0        0      684 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/classes.py
+-rw-r--r--   0        0        0      764 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/coroutine.py
+-rw-r--r--   0        0        0      245 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/cython.pyx
+-rw-r--r--   0        0        0      766 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/decorator.py
+-rw-r--r--   0        0        0      683 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/descriptor.py
+-rw-r--r--   0        0        0      643 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/docstring_signature.py
+-rw-r--r--   0        0        0      150 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/empty_all.py
+-rw-r--r--   0        0        0      384 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/enums.py
+-rw-r--r--   0        0        0      227 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/final.py
+-rw-r--r--   0        0        0      268 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/functions.py
+-rw-r--r--   0        0        0      278 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/generic_class.py
+-rw-r--r--   0        0        0      262 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/genericalias.py
+-rw-r--r--   0        0        0      260 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/hide_value.py
+-rw-r--r--   0        0        0       42 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/imported_members.py
+-rw-r--r--   0        0        0      458 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/inheritance.py
+-rw-r--r--   0        0        0      279 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/instance_variable.py
+-rw-r--r--   0        0        0       52 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/metadata.py
+-rw-r--r--   0        0        0      422 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/methods.py
+-rw-r--r--   0        0        0      155 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/module.py
+-rw-r--r--   0        0        0       93 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/name_conflict/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/name_conflict/foo.py
+-rw-r--r--   0        0        0      169 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/name_mangling.py
+-rw-r--r--   0        0        0      894 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/need_mocks.py
+-rw-r--r--   0        0        0     1345 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/overload.py
+-rw-r--r--   0        0        0       59 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/overload2.py
+-rw-r--r--   0        0        0      207 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/partialfunction.py
+-rw-r--r--   0        0        0      420 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/partialmethod.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/pep570.py
+-rw-r--r--   0        0        0      292 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/pep604.py
+-rw-r--r--   0        0        0      831 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/preserve_defaults.py
+-rw-r--r--   0        0        0      556 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/private.py
+-rw-r--r--   0        0        0       90 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/process_docstring.py
+-rw-r--r--   0        0        0      407 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/properties.py
+-rw-r--r--   0        0        0      705 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/singledispatch.py
+-rw-r--r--   0        0        0      628 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/singledispatchmethod.py
+-rw-r--r--   0        0        0      396 2023-08-02 02:05:36.078914 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/slots.py
+-rw-r--r--   0        0        0      168 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/sort_by_all.py
+-rw-r--r--   0        0        0      551 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/typed_vars.py
+-rw-r--r--   0        0        0     2107 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/typehints.py
+-rw-r--r--   0        0        0      461 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/typevar.py
+-rw-r--r--   0        0        0      123 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/uninitialized_attributes.py
+-rw-r--r--   0        0        0      372 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autodoc/target/wrappedfunction.py
+-rw-r--r--   0        0        0       85 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosectionlabel-prefix-document/conf.py
+-rw-r--r--   0        0        0      591 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst
+-rw-r--r--   0        0        0       45 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosectionlabel/conf.py
+-rw-r--r--   0        0        0      535 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosectionlabel/index.rst
+-rw-r--r--   0        0        0      294 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-filename-map/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      255 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-filename-map/conf.py
+-rw-r--r--   0        0        0      198 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-filename-map/index.rst
+-rw-r--r--   0        0        0       47 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/__init__.py
+-rw-r--r--   0        0        0       85 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      168 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-imported_members/conf.py
+-rw-r--r--   0        0        0      147 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-imported_members/index.rst
+-rw-r--r--   0        0        0      171 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-mock_imports/conf.py
+-rw-r--r--   0        0        0       72 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-mock_imports/foo.py
+-rw-r--r--   0        0        0      117 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-mock_imports/index.rst
+-rw-r--r--   0        0        0      241 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      201 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/extra_dummy_module.py
+-rw-r--r--   0        0        0      170 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-module_all/conf.py
+-rw-r--r--   0        0        0      154 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-module_all/index.rst
+-rw-r--r--   0        0        0      132 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/conf.py
+-rw-r--r--   0        0        0      174 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/package/__init__.py
+-rw-r--r--   0        0        0      147 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/package/module.py
+-rw-r--r--   0        0        0       63 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/package/module_importfail.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/package/package/__init__.py
+-rw-r--r--   0        0        0      147 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/package/package/module.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/package2/__init__.py
+-rw-r--r--   0        0        0      147 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-recursive/package2/module.py
+-rw-r--r--   0        0        0      404 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-skip-member/conf.py
+-rw-r--r--   0        0        0       54 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-skip-member/index.rst
+-rw-r--r--   0        0        0      264 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-skip-member/target.py
+-rw-r--r--   0        0        0        6 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-template/_templates/empty.rst
+-rw-r--r--   0        0        0      209 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-template/conf.py
+-rw-r--r--   0        0        0       78 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-template/index.rst
+-rw-r--r--   0        0        0       39 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary-template/target.py
+-rw-r--r--   0        0        0       22 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary/autosummary_class_module.py
+-rw-r--r--   0        0        0      232 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary/autosummary_dummy_inherited_module.py
+-rw-r--r--   0        0        0      932 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary/autosummary_dummy_module.py
+-rw-r--r--   0        0        0       63 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary/autosummary_importfail.py
+-rw-r--r--   0        0        0      190 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary/conf.py
+-rw-r--r--   0        0        0      499 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-autosummary/index.rst
+-rw-r--r--   0        0        0      242 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-coverage/conf.py
+-rw-r--r--   0        0        0      254 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-coverage/coverage_ignored.py
+-rw-r--r--   0        0        0      254 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-coverage/coverage_not_ignored.py
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-coverage/index.rst
+-rw-r--r--   0        0        0      371 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-skipif/conf.py
+-rw-r--r--   0        0        0     2052 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-skipif/skipif.txt
+-rw-r--r--   0        0        0      205 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-with-autodoc/conf.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-with-autodoc/dir/__init__.py
+-rw-r--r--   0        0        0       28 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-with-autodoc/dir/bar.py
+-rw-r--r--   0        0        0       60 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-with-autodoc/dir/inner.rst
+-rw-r--r--   0        0        0       25 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-with-autodoc/foo.py
+-rw-r--r--   0        0        0       52 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest-with-autodoc/index.rst
+-rw-r--r--   0        0        0      148 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest/conf.py
+-rw-r--r--   0        0        0     2147 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-doctest/doctest.txt
+-rw-r--r--   0        0        0      190 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/conf.py
+-rw-r--r--   0        0        0      555 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst
+-rw-r--r--   0        0        0      161 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-extlinks-hardcoded-urls/conf.py
+-rw-r--r--   0        0        0      703 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst
+-rw-r--r--   0        0        0       40 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-githubpages/conf.py
+-rw-r--r--   0        0        0       25 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-githubpages/index.rst
+-rw-r--r--   0        0        0       67 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-graphviz/conf.py
+-rw-r--r--   0        0        0       25 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-graphviz/graph.dot
+-rw-r--r--   0        0        0       25 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-graphviz/graph.xx.dot
+-rw-r--r--   0        0        0      389 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-graphviz/index.rst
+-rw-r--r--   0        0        0      256 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-ifconfig/conf.py
+-rw-r--r--   0        0        0      274 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-ifconfig/index.rst
+-rw-r--r--   0        0        0       41 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-imgconverter/conf.py
+-rw-r--r--   0        0        0   141783 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-imgconverter/img.pdf
+-rw-r--r--   0        0        0       86 2023-08-02 02:05:36.082913 sphinx-7.1.2/tests/roots/test-ext-imgconverter/index.rst
+-rw-r--r--   0        0        0      243 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-imgconverter/svgimg.svg
+-rw-r--r--   0        0        0      106 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-imgmockconverter/1/svgimg.svg
+-rw-r--r--   0        0        0      243 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-imgmockconverter/2/svgimg.svg
+-rw-r--r--   0        0        0       97 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-imgmockconverter/conf.py
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-imgmockconverter/index.rst
+-rw-r--r--   0        0        0      881 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py
+-rw-r--r--   0        0        0      112 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-inheritance_diagram/conf.py
+-rw-r--r--   0        0        0       13 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-inheritance_diagram/example/__init__.py
+-rw-r--r--   0        0        0       46 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-inheritance_diagram/example/sphinx.py
+-rw-r--r--   0        0        0      215 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-inheritance_diagram/index.rst
+-rw-r--r--   0        0        0      101 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-inheritance_diagram/test.py
+-rw-r--r--   0        0        0       40 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-intersphinx-cppdomain/conf.py
+-rw-r--r--   0        0        0      150 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-intersphinx-cppdomain/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-intersphinx-role/conf.py
+-rw-r--r--   0        0        0     1211 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-intersphinx-role/index.rst
+-rw-r--r--   0        0        0      488 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math-compat/conf.py
+-rw-r--r--   0        0        0      199 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math-compat/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math-simple/conf.py
+-rw-r--r--   0        0        0       43 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math-simple/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math/conf.py
+-rw-r--r--   0        0        0      239 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math/index.rst
+-rw-r--r--   0        0        0      396 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math/math.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math/nomath.rst
+-rw-r--r--   0        0        0      128 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-math/page.rst
+-rw-r--r--   0        0        0      100 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-napoleon/conf.py
+-rw-r--r--   0        0        0       64 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-napoleon/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-napoleon/mypackage/__init__.py
+-rw-r--r--   0        0        0      194 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-napoleon/mypackage/typehints.py
+-rw-r--r--   0        0        0       70 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-napoleon/typehints.rst
+-rw-r--r--   0        0        0       31 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-todo/bar.rst
+-rw-r--r--   0        0        0       33 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-todo/conf.py
+-rw-r--r--   0        0        0      125 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-todo/foo.rst
+-rw-r--r--   0        0        0      109 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-todo/index.rst
+-rw-r--r--   0        0        0      108 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode-find/conf.py
+-rw-r--r--   0        0        0      636 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode-find/index.rst
+-rw-r--r--   0        0        0       37 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode-find/not_a_package/__init__.py
+-rw-r--r--   0        0        0      371 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode-find/not_a_package/submodule.py
+-rw-r--r--   0        0        0      745 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode/conf.py
+-rw-r--r--   0        0        0      550 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode/index.rst
+-rw-r--r--   0        0        0     3111 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode/objects.rst
+-rw-r--r--   0        0        0       64 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode/spam/__init__.py
+-rw-r--r--   0        0        0      308 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode/spam/mod1.py
+-rw-r--r--   0        0        0      188 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode/spam/mod2.py
+-rw-r--r--   0        0        0       52 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-ext-viewcode/spam/mod3.py
+-rw-r--r--   0        0        0       63 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-extensions/conf.py
+-rw-r--r--   0        0        0       70 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-extensions/read_parallel.py
+-rw-r--r--   0        0        0       71 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-extensions/read_serial.py
+-rw-r--r--   0        0        0       72 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-extensions/write_parallel.py
+-rw-r--r--   0        0        0       72 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-extensions/write_serial.py
+-rw-r--r--   0        0        0       70 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-footnotes/bar.rst
+-rw-r--r--   0        0        0       70 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-footnotes/baz.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-footnotes/conf.py
+-rw-r--r--   0        0        0     3385 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-footnotes/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-footnotes/rimg.png
+-rw-r--r--   0        0        0      143 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-gettext-template/_templates/template1.html
+-rw-r--r--   0        0        0      143 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-gettext-template/_templates/template2.html
+-rw-r--r--   0        0        0       32 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-gettext-template/conf.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-gettext-template/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-glossary/conf.py
+-rw-r--r--   0        0        0      260 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-glossary/index.rst
+-rw-r--r--   0        0        0      103 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-highlight_options/conf.py
+-rw-r--r--   0        0        0      166 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-highlight_options/index.rst
+-rw-r--r--   0        0        0      468 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/conf.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/.htaccess
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/.htpasswd
+-rw-r--r--   0        0        0       28 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/API.html_t
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/css/style.css
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/rimg.png
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/subdir/.htaccess
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/extra/subdir/.htpasswd
+-rw-r--r--   0        0        0       65 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/.htaccess
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/.htpasswd
+-rw-r--r--   0        0        0       28 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/API.html_t
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/css/style.css
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/js/custom.js
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/rimg.png
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/subdir/.htaccess
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/static/subdir/.htpasswd
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/subdir/_build/index.html
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_assets/subdir/background.png
+-rw-r--r--   0        0        0       53 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_entity/conf.py
+-rw-r--r--   0        0        0      561 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_entity/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_scaled_image_link/conf.py
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_scaled_image_link/img.png
+-rw-r--r--   0        0        0      172 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_scaled_image_link/index.rst
+-rw-r--r--   0        0        0       36 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_signaturereturn_icon/conf.py
+-rw-r--r--   0        0        0      108 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_signaturereturn_icon/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_style/_static/default.css
+-rw-r--r--   0        0        0       58 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_style/conf.py
+-rw-r--r--   0        0        0       22 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-html_style/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-escape/conf.py
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-escape/img_#1.png
+-rw-r--r--   0        0        0      145 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-escape/index.rst
+-rw-r--r--   0        0        0      161 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-in-parsed-literal/conf.py
+-rw-r--r--   0        0        0      113 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-in-parsed-literal/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-in-parsed-literal/pic.png
+-rw-r--r--   0        0        0      143 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-in-section/conf.py
+-rw-r--r--   0        0        0      287 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-in-section/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-image-in-section/pic.png
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.086914 sphinx-7.1.2/tests/roots/test-images/conf.py
+-rw-r--r--   0        0        0    24976 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/img.gif
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/img.ja.png
+-rw-r--r--   0        0        0   141783 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/img.pdf
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/img.png
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/img.zh.png
+-rw-r--r--   0        0        0      466 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/rimg.png
+-rw-r--r--   0        0        0      218 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/rimg.png.xx
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/rimg.xx.png
+-rw-r--r--   0        0        0      128 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/subdir/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/subdir/rimg.png
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/subdir/rimg.xx.png
+-rw-r--r--   0        0        0   141783 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/subdir/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/subdir/svgimg.svg
+-rw-r--r--   0        0        0      243 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/subdir/svgimg.xx.svg
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-images/testimäge.png
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-index_on_title/conf.py
+-rw-r--r--   0        0        0      117 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-index_on_title/contents.rst
+-rw-r--r--   0        0        0       70 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/basic_diagram.rst
+-rw-r--r--   0        0        0      135 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/conf.py
+-rw-r--r--   0        0        0      166 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/diagram_module_w_2_top_classes.rst
+-rw-r--r--   0        0        0      125 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/diagram_w_1_top_class.rst
+-rw-r--r--   0        0        0      179 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/diagram_w_2_top_classes.rst
+-rw-r--r--   0        0        0      104 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/diagram_w_nested_classes.rst
+-rw-r--r--   0        0        0      118 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/diagram_w_parts.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/dummy/__init__.py
+-rw-r--r--   0        0        0      267 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/dummy/test.py
+-rw-r--r--   0        0        0       95 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/dummy/test_nested.py
+-rw-r--r--   0        0        0       31 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-inheritance/index.rst
+-rw-r--r--   0        0        0      216 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/_templates/contents.html
+-rw-r--r--   0        0        0      599 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/admonitions.txt
+-rw-r--r--   0        0        0       74 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/bom.txt
+-rw-r--r--   0        0        0      262 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/conf.py
+-rw-r--r--   0        0        0      342 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/definition_terms.txt
+-rw-r--r--   0        0        0      704 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/docfields.txt
+-rw-r--r--   0        0        0      858 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/external_links.txt
+-rw-r--r--   0        0        0      747 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/figure.txt
+-rw-r--r--   0        0        0      407 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/footnote.txt
+-rw-r--r--   0        0        0      378 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/glossary_terms.txt
+-rw-r--r--   0        0        0      151 2023-08-02 02:05:36.090914 sphinx-7.1.2/tests/roots/test-intl/glossary_terms_inconsistency.txt
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/i18n.png
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/img.png
+-rw-r--r--   0        0        0      563 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/index.txt
+-rw-r--r--   0        0        0      384 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/index_entries.txt
+-rw-r--r--   0        0        0     1832 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/label_target.txt
+-rw-r--r--   0        0        0      943 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/literalblock.txt
+-rw-r--r--   0        0        0      278 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/noqa.txt
+-rw-r--r--   0        0        0      128 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/only.txt
+-rw-r--r--   0        0        0       78 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/raw.txt
+-rw-r--r--   0        0        0     1094 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/refs.txt
+-rw-r--r--   0        0        0      291 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/refs_inconsistency.txt
+-rw-r--r--   0        0        0      252 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/refs_python_domain.txt
+-rw-r--r--   0        0        0      738 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/role_xref.txt
+-rw-r--r--   0        0        0      152 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/rubric.txt
+-rw-r--r--   0        0        0       97 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/section.txt
+-rw-r--r--   0        0        0      210 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/seealso.txt
+-rw-r--r--   0        0        0       32 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/subdir/index.txt
+-rw-r--r--   0        0        0      263 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/table.txt
+-rw-r--r--   0        0        0      139 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/toctree.txt
+-rw-r--r--   0        0        0      135 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/topic.txt
+-rw-r--r--   0        0        0      800 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/translation_progress.txt
+-rw-r--r--   0        0        0      337 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/versionchange.txt
+-rw-r--r--   0        0        0       79 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/warnings.txt
+-rw-r--r--   0        0        0     1513 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po
+-rw-r--r--   0        0        0      264 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/bom.po
+-rw-r--r--   0        0        0     1198 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po
+-rw-r--r--   0        0        0     1086 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po
+-rw-r--r--   0        0        0     1691 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po
+-rw-r--r--   0        0        0     1307 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/figure.po
+-rw-r--r--   0        0        0     1228 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po
+-rw-r--r--   0        0        0     1327 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po
+-rw-r--r--   0        0        0      754 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po
+-rw-r--r--   0        0        0      773 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     1318 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po
+-rw-r--r--   0        0        0     2159 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po
+-rw-r--r--   0        0        0     2211 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po
+-rw-r--r--   0        0        0     1380 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po
+-rw-r--r--   0        0        0      723 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/only.po
+-rw-r--r--   0        0        0      644 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/raw.po
+-rw-r--r--   0        0        0     2771 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/refs.po
+-rw-r--r--   0        0        0     1045 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po
+-rw-r--r--   0        0        0      675 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po
+-rw-r--r--   0        0        0     1707 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po
+-rw-r--r--   0        0        0      744 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po
+-rw-r--r--   0        0        0      706 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/section.po
+-rw-r--r--   0        0        0      792 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po
+-rw-r--r--   0        0        0      621 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0      992 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/table.po
+-rw-r--r--   0        0        0      767 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po
+-rw-r--r--   0        0        0      750 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/topic.po
+-rw-r--r--   0        0        0     1585 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po
+-rw-r--r--   0        0        0     1070 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po
+-rw-r--r--   0        0        0      710 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po
+-rw-r--r--   0        0        0       21 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-keep_warnings/conf.py
+-rw-r--r--   0        0        0       20 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-keep_warnings/index.rst
+-rw-r--r--   0        0        0       13 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-babel/bar.rst
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-babel/conf.py
+-rw-r--r--   0        0        0       13 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-babel/foo.rst
+-rw-r--r--   0        0        0       87 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-babel/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-container/conf.py
+-rw-r--r--   0        0        0       35 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-container/index.rst
+-rw-r--r--   0        0        0       59 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-equations/conf.py
+-rw-r--r--   0        0        0      256 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-equations/equations.rst
+-rw-r--r--   0        0        0      452 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-equations/expects/latex-equations.tex
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-figure-in-admonition/conf.py
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-figure-in-admonition/img.png
+-rw-r--r--   0        0        0      132 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-figure-in-admonition/index.rst
+-rw-r--r--   0        0        0     1573 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-includegraphics/conf.py
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-includegraphics/img.png
+-rw-r--r--   0        0        0      834 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-includegraphics/index.rst
+-rw-r--r--   0        0        0    34213 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-includegraphics/sphinx.png
+-rw-r--r--   0        0        0    38192 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-includegraphics/tall.png
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-index/conf.py
+-rw-r--r--   0        0        0      215 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-index/index.rst
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels-before-module/automodule1.py
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels-before-module/automodule2a.py
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels-before-module/automodule2b.py
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels-before-module/automodule3.py
+-rw-r--r--   0        0        0      117 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels-before-module/conf.py
+-rw-r--r--   0        0        0      464 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels-before-module/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels/conf.py
+-rw-r--r--   0        0        0      771 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels/index.rst
+-rw-r--r--   0        0        0       18 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-labels/otherdoc.rst
+-rw-r--r--   0        0        0      250 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-numfig/conf.py
+-rw-r--r--   0        0        0      112 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-numfig/index.rst
+-rw-r--r--   0        0        0      141 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-numfig/indexhowto.rst
+-rw-r--r--   0        0        0      165 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-numfig/indexmanual.rst
+-rw-r--r--   0        0        0       18 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-table/_mytemplates/latex/longtable.tex_t
+-rw-r--r--   0        0        0     1661 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-table/complex.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-table/conf.py
+-rw-r--r--   0        0        0     1933 2023-08-02 02:05:36.094914 sphinx-7.1.2/tests/roots/test-latex-table/expects/complex_spanning_cell.tex
+-rw-r--r--   0        0        0     1752 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/gridtable.tex
+-rw-r--r--   0        0        0     1780 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex
+-rw-r--r--   0        0        0     1323 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable.tex
+-rw-r--r--   0        0        0     1300 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_align.tex
+-rw-r--r--   0        0        0     1445 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_caption.tex
+-rw-r--r--   0        0        0     1384 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex
+-rw-r--r--   0        0        0     1637 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex
+-rw-r--r--   0        0        0     1386 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex
+-rw-r--r--   0        0        0     1656 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_widths.tex
+-rw-r--r--   0        0        0     1409 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex
+-rw-r--r--   0        0        0     1341 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex
+-rw-r--r--   0        0        0      704 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/simple_table.tex
+-rw-r--r--   0        0        0      851 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_caption.tex
+-rw-r--r--   0        0        0      777 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex
+-rw-r--r--   0        0        0      978 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex
+-rw-r--r--   0        0        0      594 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex
+-rw-r--r--   0        0        0      779 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_verbatim.tex
+-rw-r--r--   0        0        0     1093 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_widths.tex
+-rw-r--r--   0        0        0      802 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex
+-rw-r--r--   0        0        0      733 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/tabular_having_widths.tex
+-rw-r--r--   0        0        0      747 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/tabularcolumn.tex
+-rw-r--r--   0        0        0      727 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/expects/tabulary_having_widths.tex
+-rw-r--r--   0        0        0       84 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/index.rst
+-rw-r--r--   0        0        0     2516 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/longtable.rst
+-rw-r--r--   0        0        0     2770 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-table/tabular.rst
+-rw-r--r--   0        0        0       52 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-theme/conf.py
+-rw-r--r--   0        0        0       24 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-theme/index.rst
+-rw-r--r--   0        0        0      117 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-theme/theme/custom/theme.conf
+-rw-r--r--   0        0        0      160 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-title/conf.py
+-rw-r--r--   0        0        0      165 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-title/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-unicode/conf.py
+-rw-r--r--   0        0        0      142 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-latex-unicode/index.rst
+-rw-r--r--   0        0        0       80 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-anchors-ignore-for-url/conf.py
+-rw-r--r--   0        0        0      532 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst
+-rw-r--r--   0        0        0       80 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-anchors-ignore/conf.py
+-rw-r--r--   0        0        0      109 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-anchors-ignore/index.rst
+-rw-r--r--   0        0        0      180 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-documents_exclude/br0ken_link.rst
+-rw-r--r--   0        0        0      174 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-documents_exclude/broken_link.rst
+-rw-r--r--   0        0        0      133 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-documents_exclude/conf.py
+-rw-r--r--   0        0        0       40 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-documents_exclude/index.rst
+-rw-r--r--   0        0        0       80 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver-anchor/conf.py
+-rw-r--r--   0        0        0       48 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver-anchor/index.rst
+-rw-r--r--   0        0        0       55 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver-https/conf.py
+-rw-r--r--   0        0        0       42 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver-https/index.rst
+-rw-r--r--   0        0        0       55 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver-warn-redirects/conf.py
+-rw-r--r--   0        0        0       95 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver-warn-redirects/index.rst
+-rw-r--r--   0        0        0       55 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver/conf.py
+-rw-r--r--   0        0        0       41 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-localserver/index.rst
+-rw-r--r--   0        0        0       55 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-raw-node/conf.py
+-rw-r--r--   0        0        0       46 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-raw-node/index.rst
+-rw-r--r--   0        0        0       80 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-too-many-retries/conf.py
+-rw-r--r--   0        0        0       73 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck-too-many-retries/index.rst
+-rw-r--r--   0        0        0       99 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck/conf.py
+-rw-r--r--   0        0        0      648 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-linkcheck/links.rst
+-rw-r--r--   0        0        0      143 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-local-logo/conf.py
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-local-logo/images/img.png
+-rw-r--r--   0        0        0     1477 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-local-logo/index.rst
+-rw-r--r--   0        0        0       80 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       41 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       80 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       41 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       82 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       43 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-manpage_url/conf.py
+-rw-r--r--   0        0        0       61 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-manpage_url/index.rst
+-rw-r--r--   0        0        0      114 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-markup-citation/conf.py
+-rw-r--r--   0        0        0      166 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-markup-citation/index.rst
+-rw-r--r--   0        0        0      114 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-markup-rubric/conf.py
+-rw-r--r--   0        0        0      112 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-markup-rubric/index.rst
+-rw-r--r--   0        0        0       78 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-maxlistdepth/conf.py
+-rw-r--r--   0        0        0      687 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-maxlistdepth/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-metadata/conf.py
+-rw-r--r--   0        0        0     1436 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-metadata/index.rst
+-rw-r--r--   0        0        0        8 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-need-escaped/bar.rst
+-rw-r--r--   0        0        0        8 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-need-escaped/baz.rst
+-rw-r--r--   0        0        0       62 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-need-escaped/conf.py
+-rw-r--r--   0        0        0       82 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-need-escaped/foo.rst
+-rw-r--r--   0        0        0      574 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-need-escaped/index.rst
+-rw-r--r--   0        0        0       10 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-need-escaped/quux.rst
+-rw-r--r--   0        0        0       29 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-need-escaped/qux.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-nested-enumerated-list/conf.py
+-rw-r--r--   0        0        0      300 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-nested-enumerated-list/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-nested-tables/conf.py
+-rw-r--r--   0        0        0      248 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-nested-tables/index.rst
+-rw-r--r--   0        0        0       16 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-nitpicky-warnings/conf.py
+-rw-r--r--   0        0        0      176 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-nitpicky-warnings/index.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numbered-circular/conf.py
+-rw-r--r--   0        0        0       36 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numbered-circular/index.rst
+-rw-r--r--   0        0        0       23 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numbered-circular/sub.rst
+-rw-r--r--   0        0        0      710 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numfig/bar.rst
+-rw-r--r--   0        0        0      259 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numfig/baz.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numfig/conf.py
+-rw-r--r--   0        0        0      912 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numfig/foo.rst
+-rw-r--r--   0        0        0     1024 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numfig/index.rst
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-numfig/rimg.png
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-object-description-sections/conf.py
+-rw-r--r--   0        0        0       80 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-object-description-sections/index.rst
+-rw-r--r--   0        0        0       73 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/Bare.rst
+-rw-r--r--   0        0        0       58 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/Dup1.rst
+-rw-r--r--   0        0        0       58 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/Dup2.rst
+-rw-r--r--   0        0        0       94 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/LineContinuation.rst
+-rw-r--r--   0        0        0       72 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/P1.rst
+-rw-r--r--   0        0        0       72 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/P2.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/conf.py
+-rw-r--r--   0        0        0       97 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/firstLineRule.rst
+-rw-r--r--   0        0        0      663 2023-08-02 02:05:36.098914 sphinx-7.1.2/tests/roots/test-productionlist/index.rst
+-rw-r--r--   0        0        0      177 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-prolog/conf.py
+-rw-r--r--   0        0        0       83 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-prolog/index.rst
+-rw-r--r--   0        0        0       57 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-prolog/markdown.md
+-rw-r--r--   0        0        0      299 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-prolog/prolog_markdown_parser.py
+-rw-r--r--   0        0        0       67 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-prolog/restructuredtext.rst
+-rw-r--r--   0        0        0       75 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-pycode/cp_1251_coded.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-reST-code-block/conf.py
+-rw-r--r--   0        0        0       97 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-reST-code-block/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-reST-code-role/conf.py
+-rw-r--r--   0        0        0      194 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-reST-code-role/index.rst
+-rw-r--r--   0        0        0       27 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-refonly_bullet_list/conf.py
+-rw-r--r--   0        0        0      147 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-refonly_bullet_list/index.rst
+-rw-r--r--   0        0        0      237 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-remote-logo/conf.py
+-rw-r--r--   0        0        0     1477 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-remote-logo/index.rst
+-rw-r--r--   0        0        0       32 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-roles-download/another/dummy.dat
+-rw-r--r--   0        0        0      114 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-roles-download/conf.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-roles-download/dummy.dat
+-rw-r--r--   0        0        0      214 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-roles-download/index.rst
+-rw-r--r--   0        0        0     2111 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/Makefile
+-rw-r--r--   0        0        0       67 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/_templates/contentssb.html
+-rw-r--r--   0        0        0       99 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/_templates/customsb.html
+-rw-r--r--   0        0        0      428 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/_templates/layout.html
+-rw-r--r--   0        0        0      578 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/autodoc.txt
+-rw-r--r--   0        0        0     4587 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/autodoc_target.py
+-rw-r--r--   0        0        0       74 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/bom.txt
+-rw-r--r--   0        0        0     4257 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/conf.py
+-rw-r--r--   0        0        0       87 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/extapi.txt
+-rw-r--r--   0        0        0      365 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/extensions.txt
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/file_with_special_#_chars.xyz
+-rw-r--r--   0        0        0      826 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/footnote.txt
+-rw-r--r--   0        0        0      575 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/images.txt
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/img.foo.png
+-rw-r--r--   0        0        0    24976 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/img.gif
+-rw-r--r--   0        0        0   141783 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/img.pdf
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/img.png
+-rw-r--r--   0        0        0     2108 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/includes.txt
+-rw-r--r--   0        0        0     1118 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/index.txt
+-rw-r--r--   0        0        0      750 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/lists.txt
+-rw-r--r--   0        0        0      200 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/literal.inc
+-rw-r--r--   0        0        0      208 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/literal_orig.inc
+-rw-r--r--   0        0        0     6902 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/markup.txt
+-rw-r--r--   0        0        0      373 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/math.txt
+-rw-r--r--   0        0        0     4561 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/objects.txt
+-rw-r--r--   0        0        0      110 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/otherext.foo
+-rw-r--r--   0        0        0      346 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/parsermod.py
+-rw-r--r--   0        0        0       45 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/quotes.inc
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/rimg.png
+-rw-r--r--   0        0        0       40 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/special/api.h
+-rw-r--r--   0        0        0       32 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/special/code.py
+-rw-r--r--   0        0        0       96 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/subdir/excluded.txt
+-rw-r--r--   0        0        0      106 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/subdir/images.txt
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/subdir/img.png
+-rw-r--r--   0        0        0      143 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/subdir/include.inc
+-rw-r--r--   0        0        0      328 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/subdir/includes.txt
+-rw-r--r--   0        0        0    66247 2023-08-02 02:05:36.102914 sphinx-7.1.2/tests/roots/test-root/subdir/simg.png
+-rw-r--r--   0        0        0   141783 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-root/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-root/svgimg.svg
+-rw-r--r--   0        0        0       78 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-root/tabs.inc
+-rw-r--r--   0        0        0       77 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-root/test.inc
+-rw-r--r--   0        0        0      107 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-root/wrongenc.inc
+-rw-r--r--   0        0        0       58 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-search/conf.py
+-rw-r--r--   0        0        0      381 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-search/index.rst
+-rw-r--r--   0        0        0       41 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-search/nosearch.rst
+-rw-r--r--   0        0        0      184 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-search/tocitem.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-smartquotes/conf.py
+-rw-r--r--   0        0        0      107 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-smartquotes/index.rst
+-rw-r--r--   0        0        0      231 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-smartquotes/literals.rst
+-rw-r--r--   0        0        0      453 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-stylesheets/_templates/layout.html
+-rw-r--r--   0        0        0      318 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-stylesheets/conf.py
+-rw-r--r--   0        0        0       53 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-stylesheets/index.rst
+-rw-r--r--   0        0        0      182 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-templating/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      109 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-templating/_templates/layout.html
+-rw-r--r--   0        0        0      135 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-templating/autosummary_templating.txt
+-rw-r--r--   0        0        0      266 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-templating/conf.py
+-rw-r--r--   0        0        0      124 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-templating/index.txt
+-rw-r--r--   0        0        0      661 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/child.zip
+-rw-r--r--   0        0        0       94 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/conf.py
+-rw-r--r--   0        0        0       26 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/index.rst
+-rw-r--r--   0        0        0     1039 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/parent.zip
+-rw-r--r--   0        0        0       82 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/test_theme/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/test_theme/staticfiles/layout.html
+-rw-r--r--   0        0        0      120 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/test_theme/staticfiles/static/staticimg.png
+-rw-r--r--   0        0        0       82 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/test_theme/staticfiles/static/statictmpl.html_t
+-rw-r--r--   0        0        0      104 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/test_theme/staticfiles/theme.conf
+-rw-r--r--   0        0        0       98 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/test_theme/test-theme/theme.conf
+-rw-r--r--   0        0        0     1039 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-theming/ziptheme.zip
+-rw-r--r--   0        0        0      150 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-tocdepth/bar.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-tocdepth/baz.rst
+-rw-r--r--   0        0        0       53 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-tocdepth/conf.py
+-rw-r--r--   0        0        0      146 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-tocdepth/foo.rst
+-rw-r--r--   0        0        0       71 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-tocdepth/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-domain-objects/conf.py
+-rw-r--r--   0        0        0      731 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-domain-objects/domains.rst
+-rw-r--r--   0        0        0       90 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-domain-objects/index.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-duplicated/conf.py
+-rw-r--r--   0        0        0        8 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-duplicated/foo.rst
+-rw-r--r--   0        0        0       77 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-duplicated/index.rst
+-rw-r--r--   0        0        0      101 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-empty/_templates/localtoc.html
+-rw-r--r--   0        0        0       62 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-empty/conf.py
+-rw-r--r--   0        0        0       52 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-empty/index.rst
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/bar/bar_1.rst
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/bar/bar_2.rst
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/bar/bar_3.rst
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/bar/bar_4/index.rst
+-rw-r--r--   0        0        0       53 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/bar/index.rst
+-rw-r--r--   0        0        0       13 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/baz.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/conf.py
+-rw-r--r--   0        0        0       13 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/foo.rst
+-rw-r--r--   0        0        0      303 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/index.rst
+-rw-r--r--   0        0        0       16 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/quux.rst
+-rw-r--r--   0        0        0       50 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/qux/index.rst
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/qux/qux_1.rst
+-rw-r--r--   0        0        0       17 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-glob/qux/qux_2.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-index/conf.py
+-rw-r--r--   0        0        0      105 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-index/foo.rst
+-rw-r--r--   0        0        0      132 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-index/index.rst
+-rw-r--r--   0        0        0      150 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-maxdepth/bar.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-maxdepth/baz.rst
+-rw-r--r--   0        0        0       30 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-maxdepth/conf.py
+-rw-r--r--   0        0        0      146 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-maxdepth/foo.rst
+-rw-r--r--   0        0        0      105 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-maxdepth/index.rst
+-rw-r--r--   0        0        0      105 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree-maxdepth/qux.rst
+-rw-r--r--   0        0        0        8 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/bar.rst
+-rw-r--r--   0        0        0        8 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/baz.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/conf.py
+-rw-r--r--   0        0        0       74 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/foo.rst
+-rw-r--r--   0        0        0      885 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/index.rst
+-rw-r--r--   0        0        0       10 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/quux.rst
+-rw-r--r--   0        0        0       29 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/qux.rst
+-rw-r--r--   0        0        0       97 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-toctree/tocdepth.rst
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-transforms-post_transforms-keyboard/conf.py
+-rw-r--r--   0        0        0       94 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-transforms-post_transforms-keyboard/index.rst
+-rw-r--r--   0        0        0       16 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-transforms-post_transforms-missing-reference/conf.py
+-rw-r--r--   0        0        0      113 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-transforms-post_transforms-missing-reference/index.rst
+-rw-r--r--   0        0        0       36 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-trim_doctest_flags/conf.py
+-rw-r--r--   0        0        0      784 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-trim_doctest_flags/index.rst
+-rw-r--r--   0        0        0     1012 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/added.txt
+-rw-r--r--   0        0        0       86 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/conf.py
+-rw-r--r--   0        0        0      584 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/deleted.txt
+-rw-r--r--   0        0        0      490 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/deleted_end.txt
+-rw-r--r--   0        0        0      164 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/index.txt
+-rw-r--r--   0        0        0      864 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/insert.txt
+-rw-r--r--   0        0        0      850 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/insert_beginning.txt
+-rw-r--r--   0        0        0      735 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/insert_similar.txt
+-rw-r--r--   0        0        0      867 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/modified.txt
+-rw-r--r--   0        0        0      715 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-versioning/original.txt
+-rw-r--r--   0        0        0      151 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-warnings/autodoc_fodder.py
+-rw-r--r--   0        0        0       97 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-warnings/conf.py
+-rw-r--r--   0        0        0      697 2023-08-02 02:05:36.106914 sphinx-7.1.2/tests/roots/test-warnings/index.rst
+-rw-r--r--   0        0        0   141783 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/roots/test-warnings/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/roots/test-warnings/svgimg.svg
+-rw-r--r--   0        0        0       18 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/roots/test-warnings/undecodable.rst
+-rw-r--r--   0        0        0      107 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/roots/test-warnings/wrongenc.inc
+-rw-r--r--   0        0        0     3309 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_api_translator.py
+-rw-r--r--   0        0        0     5605 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_application.py
+-rw-r--r--   0        0        0     4771 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build.py
+-rw-r--r--   0        0        0     1152 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_changes.py
+-rw-r--r--   0        0        0     1407 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_dirhtml.py
+-rw-r--r--   0        0        0    16623 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_epub.py
+-rw-r--r--   0        0        0     6524 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_gettext.py
+-rw-r--r--   0        0        0    80743 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_html.py
+-rw-r--r--   0        0        0    76570 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_latex.py
+-rw-r--r--   0        0        0    33873 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_linkcheck.py
+-rw-r--r--   0        0        0     2751 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_manpage.py
+-rw-r--r--   0        0        0     5910 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_texinfo.py
+-rw-r--r--   0        0        0     8996 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_build_text.py
+-rw-r--r--   0        0        0     1322 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_builder.py
+-rw-r--r--   0        0        0     2646 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_catalogs.py
+-rw-r--r--   0        0        0    17855 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_config.py
+-rw-r--r--   0        0        0      811 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_correct_year.py
+-rw-r--r--   0        0        0    23761 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_directive_code.py
+-rw-r--r--   0        0        0     2088 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_directive_object_description.py
+-rw-r--r--   0        0        0     1655 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_directive_only.py
+-rw-r--r--   0        0        0     5207 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_directive_other.py
+-rw-r--r--   0        0        0     4362 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_directive_patch.py
+-rw-r--r--   0        0        0     1084 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_docutilsconf.py
+-rw-r--r--   0        0        0    37525 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_domain_c.py
+-rw-r--r--   0        0        0    76159 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_domain_cpp.py
+-rw-r--r--   0        0        0    20319 2023-08-02 02:05:36.110914 sphinx-7.1.2/tests/test_domain_js.py
+-rw-r--r--   0        0        0    98987 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_domain_py.py
+-rw-r--r--   0        0        0     5896 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_domain_rst.py
+-rw-r--r--   0        0        0    19424 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_domain_std.py
+-rw-r--r--   0        0        0     5286 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_environment.py
+-rw-r--r--   0        0        0     8068 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_environment_indexentries.py
+-rw-r--r--   0        0        0      310 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_environment_record_dependencies.py
+-rw-r--r--   0        0        0    20508 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_environment_toctree.py
+-rw-r--r--   0        0        0      321 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_errors.py
+-rw-r--r--   0        0        0     1826 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_events.py
+-rw-r--r--   0        0        0    23255 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_apidoc.py
+-rw-r--r--   0        0        0    76880 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc.py
+-rw-r--r--   0        0        0     4801 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_autoattribute.py
+-rw-r--r--   0        0        0    14272 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_autoclass.py
+-rw-r--r--   0        0        0     2631 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_autodata.py
+-rw-r--r--   0        0        0     5647 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_autofunction.py
+-rw-r--r--   0        0        0     5355 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_automodule.py
+-rw-r--r--   0        0        0     2501 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_autoproperty.py
+-rw-r--r--   0        0        0    55422 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_configs.py
+-rw-r--r--   0        0        0     3335 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_events.py
+-rw-r--r--   0        0        0     3963 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_mock.py
+-rw-r--r--   0        0        0     1666 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_preserve_defaults.py
+-rw-r--r--   0        0        0     4415 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autodoc_private_members.py
+-rw-r--r--   0        0        0     3145 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autosectionlabel.py
+-rw-r--r--   0        0        0    27705 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_autosummary.py
+-rw-r--r--   0        0        0     3158 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_coverage.py
+-rw-r--r--   0        0        0     5517 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_doctest.py
+-rw-r--r--   0        0        0      378 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_duration.py
+-rw-r--r--   0        0        0     2104 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_extlinks.py
+-rw-r--r--   0        0        0      958 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_githubpages.py
+-rw-r--r--   0        0        0     7667 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_graphviz.py
+-rw-r--r--   0        0        0      850 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_ifconfig.py
+-rw-r--r--   0        0        0     1038 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_imgconverter.py
+-rw-r--r--   0        0        0      609 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_imgmockconverter.py
+-rw-r--r--   0        0        0    10579 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_inheritance_diagram.py
+-rw-r--r--   0        0        0    21393 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_intersphinx.py
+-rw-r--r--   0        0        0    13142 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_math.py
+-rw-r--r--   0        0        0     6912 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_napoleon.py
+-rw-r--r--   0        0        0    70796 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_napoleon_docstring.py
+-rw-r--r--   0        0        0     3878 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_todo.py
+-rw-r--r--   0        0        0     5467 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_ext_viewcode.py
+-rw-r--r--   0        0        0      857 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_extension.py
+-rw-r--r--   0        0        0     3563 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_highlighting.py
+-rw-r--r--   0        0        0    51540 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_intl.py
+-rw-r--r--   0        0        0     2551 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_locale.py
+-rw-r--r--   0        0        0    22328 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_markup.py
+-rw-r--r--   0        0        0     1931 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_metadata.py
+-rw-r--r--   0        0        0     2459 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_parser.py
+-rw-r--r--   0        0        0     2573 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_project.py
+-rw-r--r--   0        0        0     6918 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_pycode.py
+-rw-r--r--   0        0        0     2835 2023-08-02 02:05:36.114914 sphinx-7.1.2/tests/test_pycode_ast.py
+-rw-r--r--   0        0        0    18264 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_pycode_parser.py
+-rw-r--r--   0        0        0     7347 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_quickstart.py
+-rw-r--r--   0        0        0     2570 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_roles.py
+-rw-r--r--   0        0        0    11627 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_search.py
+-rw-r--r--   0        0        0     3747 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_smartquotes.py
+-rw-r--r--   0        0        0     1435 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_templating.py
+-rw-r--r--   0        0        0     4334 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_theming.py
+-rw-r--r--   0        0        0     1843 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_toctree.py
+-rw-r--r--   0        0        0     2231 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_transforms_post_transforms.py
+-rw-r--r--   0        0        0     1324 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_transforms_post_transforms_code.py
+-rw-r--r--   0        0        0     2799 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util.py
+-rw-r--r--   0        0        0     3188 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_display.py
+-rw-r--r--   0        0        0     3032 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_docstrings.py
+-rw-r--r--   0        0        0     2647 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_docutils.py
+-rw-r--r--   0        0        0     3800 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_fileutil.py
+-rw-r--r--   0        0        0     8627 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_i18n.py
+-rw-r--r--   0        0        0     2653 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_images.py
+-rw-r--r--   0        0        0    26901 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_inspect.py
+-rw-r--r--   0        0        0     4032 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_inventory.py
+-rw-r--r--   0        0        0    13459 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_logging.py
+-rw-r--r--   0        0        0     7180 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_matching.py
+-rw-r--r--   0        0        0     7464 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_nodes.py
+-rw-r--r--   0        0        0     7333 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_rst.py
+-rw-r--r--   0        0        0      952 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_template.py
+-rw-r--r--   0        0        0    22811 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_util_typing.py
+-rw-r--r--   0        0        0     3561 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_versioning.py
+-rw-r--r--   0        0        0     1065 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/test_writer_latex.py
+-rw-r--r--   0        0        0     1859 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/typing_test_data.py
+-rw-r--r--   0        0        0     1663 2023-08-02 02:05:36.118914 sphinx-7.1.2/tests/utils.py
+-rw-r--r--   0        0        0      992 2023-08-02 02:05:36.118914 sphinx-7.1.2/tox.ini
+-rw-r--r--   0        0        0      226 2023-08-02 02:05:36.118914 sphinx-7.1.2/utils/CHANGES_template
+-rw-r--r--   0        0        0        0 2023-08-02 02:05:36.118914 sphinx-7.1.2/utils/__init__.py
+-rw-r--r--   0        0        0     8358 2023-08-02 02:05:36.118914 sphinx-7.1.2/utils/babel_runner.py
+-rwxr-xr-x   0        0        0      296 2023-08-02 02:05:36.118914 sphinx-7.1.2/utils/bump_docker.sh
+-rwxr-xr-x   0        0        0     5808 2023-08-02 02:05:36.118914 sphinx-7.1.2/utils/bump_version.py
+-rw-r--r--   0        0        0     1697 2023-08-02 02:05:36.118914 sphinx-7.1.2/utils/release-checklist
+-rw-r--r--   0        0        0     5807 1970-01-01 00:00:00.000000 sphinx-7.1.2/PKG-INFO
```

### Comparing `sphinx-7.1.1/AUTHORS` & `sphinx-7.1.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/CHANGES` & `sphinx-7.1.2/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Release 7.1.2 (released Aug 02, 2023)
+=====================================
+
+Bugs fixed
+----------
+
+* #11542: linkcheck: Properly respect :confval:`linkcheck_anchors`
+  and do not spuriously report failures to validate anchors.
+  Patch by James Addison.
+
 Release 7.1.1 (released Jul 27, 2023)
 =====================================
 
 Bugs fixed
 ----------
 
 * #11514: Fix ``SOURCE_DATE_EPOCH`` in multi-line copyright footer.
@@ -40,15 +50,15 @@
   directives, for example :rst:dir:`py:function:single-line-parameter-list`.
   Patch by Thomas Louf, Adam Turner, and Jean-François B.
 * #10983: Support for multiline copyright statements in the footer block.
   Patch by Stefanie Molin
 * ``sphinx.util.display.status_iterator`` now clears the current line
   with ANSI control codes, rather than overprinting with space characters.
 * #11431: linkcheck: Treat SSL failures as broken links.
-  Patch by Bénédikt Tran
+  Patch by James Addison.
 * #11157: Keep the ``translated`` attribute on translated nodes.
 * #11451: Improve the traceback displayed when using :option:`sphinx-build -T`
   in parallel builds. Patch by Bénédikt Tran
 * #11324: linkcheck: Use session-basd HTTP requests.
 * #11438: Add support for the :rst:dir:`py:class` and :rst:dir:`py:function`
   directives for PEP 695 (generic classes and functions declarations) and
   PEP 696 (default type parameters).  Multi-line support (#11011) is enabled
```

### Comparing `sphinx-7.1.1/CODE_OF_CONDUCT` & `sphinx-7.1.2/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/EXAMPLES` & `sphinx-7.1.2/EXAMPLES`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/LICENSE` & `sphinx-7.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/README.rst` & `sphinx-7.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/Makefile` & `sphinx-7.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/bookcover.png` & `sphinx-7.1.2/doc/_static/bookcover.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/conf.py.txt` & `sphinx-7.1.2/doc/_static/conf.py.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/favicon.svg` & `sphinx-7.1.2/doc/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/more.png` & `sphinx-7.1.2/doc/_static/more.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/sphinx.png` & `sphinx-7.1.2/doc/_static/sphinx.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/agogo.png` & `sphinx-7.1.2/doc/_static/themes/agogo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/alabaster.png` & `sphinx-7.1.2/doc/_static/themes/alabaster.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/bizstyle.png` & `sphinx-7.1.2/doc/_static/themes/bizstyle.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/classic.png` & `sphinx-7.1.2/doc/_static/themes/classic.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/agogo.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/agogo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/alabaster.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/alabaster.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/bizstyle.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/bizstyle.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/classic.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/classic.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/haiku.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/haiku.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/nature.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/nature.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/pyramid.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/pyramid.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/scrolls.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/scrolls.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/sphinx_rtd_theme.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/sphinx_rtd_theme.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/sphinxdoc.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/sphinxdoc.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/fullsize/traditional.png` & `sphinx-7.1.2/doc/_static/themes/fullsize/traditional.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/haiku.png` & `sphinx-7.1.2/doc/_static/themes/haiku.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/nature.png` & `sphinx-7.1.2/doc/_static/themes/nature.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/pyramid.png` & `sphinx-7.1.2/doc/_static/themes/pyramid.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/scrolls.png` & `sphinx-7.1.2/doc/_static/themes/scrolls.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/sphinx_rtd_theme.png` & `sphinx-7.1.2/doc/_static/themes/sphinx_rtd_theme.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/sphinxdoc.png` & `sphinx-7.1.2/doc/_static/themes/sphinxdoc.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/themes/traditional.png` & `sphinx-7.1.2/doc/_static/themes/traditional.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/translation.png` & `sphinx-7.1.2/doc/_static/translation.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/translation.svg` & `sphinx-7.1.2/doc/_static/translation.svg`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/tutorial/lumache-autosummary.png` & `sphinx-7.1.2/doc/_static/tutorial/lumache-autosummary.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/tutorial/lumache-first-light.png` & `sphinx-7.1.2/doc/_static/tutorial/lumache-first-light.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/tutorial/lumache-furo.png` & `sphinx-7.1.2/doc/_static/tutorial/lumache-furo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/tutorial/lumache-py-function-full.png` & `sphinx-7.1.2/doc/_static/tutorial/lumache-py-function-full.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_static/tutorial/lumache-py-function.png` & `sphinx-7.1.2/doc/_static/tutorial/lumache-py-function.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_themes/sphinx13/layout.html` & `sphinx-7.1.2/doc/_themes/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_themes/sphinx13/static/sphinx13.css` & `sphinx-7.1.2/doc/_themes/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/_themes/sphinx13/static/sphinxheader.png` & `sphinx-7.1.2/doc/_themes/sphinx13/static/sphinxheader.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/conf.py` & `sphinx-7.1.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/builders.rst` & `sphinx-7.1.2/doc/development/builders.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/index.rst` & `sphinx-7.1.2/doc/development/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/overview.rst` & `sphinx-7.1.2/doc/development/overview.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/templating.rst` & `sphinx-7.1.2/doc/development/templating.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/theming.rst` & `sphinx-7.1.2/doc/development/theming.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/tutorials/autodoc_ext.rst` & `sphinx-7.1.2/doc/development/tutorials/autodoc_ext.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/tutorials/examples/autodoc_intenum.py` & `sphinx-7.1.2/doc/development/tutorials/examples/autodoc_intenum.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/tutorials/examples/recipe.py` & `sphinx-7.1.2/doc/development/tutorials/examples/recipe.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/tutorials/examples/todo.py` & `sphinx-7.1.2/doc/development/tutorials/examples/todo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/tutorials/helloworld.rst` & `sphinx-7.1.2/doc/development/tutorials/helloworld.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/tutorials/recipe.rst` & `sphinx-7.1.2/doc/development/tutorials/recipe.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/development/tutorials/todo.rst` & `sphinx-7.1.2/doc/development/tutorials/todo.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/appapi.rst` & `sphinx-7.1.2/doc/extdev/appapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/builderapi.rst` & `sphinx-7.1.2/doc/extdev/builderapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/deprecated.rst` & `sphinx-7.1.2/doc/extdev/deprecated.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/domainapi.rst` & `sphinx-7.1.2/doc/extdev/domainapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/envapi.rst` & `sphinx-7.1.2/doc/extdev/envapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/i18n.rst` & `sphinx-7.1.2/doc/extdev/i18n.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/index.rst` & `sphinx-7.1.2/doc/extdev/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/logging.rst` & `sphinx-7.1.2/doc/extdev/logging.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/markupapi.rst` & `sphinx-7.1.2/doc/extdev/markupapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/nodes.rst` & `sphinx-7.1.2/doc/extdev/nodes.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/parserapi.rst` & `sphinx-7.1.2/doc/extdev/parserapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/extdev/utils.rst` & `sphinx-7.1.2/doc/extdev/utils.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/faq.rst` & `sphinx-7.1.2/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/glossary.rst` & `sphinx-7.1.2/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/index.rst` & `sphinx-7.1.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/internals/contributing.rst` & `sphinx-7.1.2/doc/internals/contributing.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/internals/organization.rst` & `sphinx-7.1.2/doc/internals/organization.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/internals/release-process.rst` & `sphinx-7.1.2/doc/internals/release-process.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/latex.rst` & `sphinx-7.1.2/doc/latex.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/make.bat` & `sphinx-7.1.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/man/sphinx-apidoc.rst` & `sphinx-7.1.2/doc/man/sphinx-apidoc.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/man/sphinx-autogen.rst` & `sphinx-7.1.2/doc/man/sphinx-autogen.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/man/sphinx-build.rst` & `sphinx-7.1.2/doc/man/sphinx-build.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/man/sphinx-quickstart.rst` & `sphinx-7.1.2/doc/man/sphinx-quickstart.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/support.rst` & `sphinx-7.1.2/doc/support.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/automatic-doc-generation.rst` & `sphinx-7.1.2/doc/tutorial/automatic-doc-generation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/deploying.rst` & `sphinx-7.1.2/doc/tutorial/deploying.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/describing-code.rst` & `sphinx-7.1.2/doc/tutorial/describing-code.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/first-steps.rst` & `sphinx-7.1.2/doc/tutorial/first-steps.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/getting-started.rst` & `sphinx-7.1.2/doc/tutorial/getting-started.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/index.rst` & `sphinx-7.1.2/doc/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/more-sphinx-customization.rst` & `sphinx-7.1.2/doc/tutorial/more-sphinx-customization.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/tutorial/narrative-documentation.rst` & `sphinx-7.1.2/doc/tutorial/narrative-documentation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/advanced/intl.rst` & `sphinx-7.1.2/doc/usage/advanced/intl.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/advanced/websupport/api.rst` & `sphinx-7.1.2/doc/usage/advanced/websupport/api.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/advanced/websupport/quickstart.rst` & `sphinx-7.1.2/doc/usage/advanced/websupport/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/advanced/websupport/searchadapters.rst` & `sphinx-7.1.2/doc/usage/advanced/websupport/searchadapters.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/advanced/websupport/storagebackends.rst` & `sphinx-7.1.2/doc/usage/advanced/websupport/storagebackends.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/builders/index.rst` & `sphinx-7.1.2/doc/usage/builders/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/configuration.rst` & `sphinx-7.1.2/doc/usage/configuration.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/autodoc.rst` & `sphinx-7.1.2/doc/usage/extensions/autodoc.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/autosectionlabel.rst` & `sphinx-7.1.2/doc/usage/extensions/autosectionlabel.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/autosummary.rst` & `sphinx-7.1.2/doc/usage/extensions/autosummary.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/coverage.rst` & `sphinx-7.1.2/doc/usage/extensions/coverage.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/doctest.rst` & `sphinx-7.1.2/doc/usage/extensions/doctest.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/example_google.py` & `sphinx-7.1.2/doc/usage/extensions/example_google.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/example_numpy.py` & `sphinx-7.1.2/doc/usage/extensions/example_numpy.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/extlinks.rst` & `sphinx-7.1.2/doc/usage/extensions/extlinks.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/graphviz.rst` & `sphinx-7.1.2/doc/usage/extensions/graphviz.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/ifconfig.rst` & `sphinx-7.1.2/doc/usage/extensions/ifconfig.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/imgconverter.rst` & `sphinx-7.1.2/doc/usage/extensions/imgconverter.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/index.rst` & `sphinx-7.1.2/doc/usage/extensions/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/inheritance.rst` & `sphinx-7.1.2/doc/usage/extensions/inheritance.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/intersphinx.rst` & `sphinx-7.1.2/doc/usage/extensions/intersphinx.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/linkcode.rst` & `sphinx-7.1.2/doc/usage/extensions/linkcode.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/math.rst` & `sphinx-7.1.2/doc/usage/extensions/math.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/napoleon.rst` & `sphinx-7.1.2/doc/usage/extensions/napoleon.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/todo.rst` & `sphinx-7.1.2/doc/usage/extensions/todo.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/extensions/viewcode.rst` & `sphinx-7.1.2/doc/usage/extensions/viewcode.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/index.rst` & `sphinx-7.1.2/doc/usage/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/installation.rst` & `sphinx-7.1.2/doc/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/markdown.rst` & `sphinx-7.1.2/doc/usage/markdown.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/quickstart.rst` & `sphinx-7.1.2/doc/usage/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/restructuredtext/basics.rst` & `sphinx-7.1.2/doc/usage/restructuredtext/basics.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/restructuredtext/directives.rst` & `sphinx-7.1.2/doc/usage/restructuredtext/directives.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/restructuredtext/domains.rst` & `sphinx-7.1.2/doc/usage/restructuredtext/domains.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/restructuredtext/field-lists.rst` & `sphinx-7.1.2/doc/usage/restructuredtext/field-lists.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/restructuredtext/index.rst` & `sphinx-7.1.2/doc/usage/restructuredtext/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/restructuredtext/roles.rst` & `sphinx-7.1.2/doc/usage/restructuredtext/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/doc/usage/theming.rst` & `sphinx-7.1.2/doc/usage/theming.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/pyproject.toml` & `sphinx-7.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/__init__.py` & `sphinx-7.1.2/sphinx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
     warnings.filterwarnings('default', category=RemovedInNextVersionWarning)
 # docutils.io using mode='rU' for open
 warnings.filterwarnings('ignore', "'U' mode is deprecated",
                         DeprecationWarning, module='docutils.io')
 warnings.filterwarnings('ignore', 'The frontend.Option class .*',
                         DeprecationWarning, module='docutils.frontend')
 
-__version__ = '7.1.1'
+__version__ = '7.1.2'
 __display_version__ = __version__  # used for command line version
 
 #: Version info for better programmatic use.
 #:
 #: A tuple of five elements; for Sphinx version 1.2.1 beta 3 this would be
 #: ``(1, 2, 1, 'beta', 3)``. The fourth element can be one of: ``alpha``,
 #: ``beta``, ``rc``, ``final``. ``final`` always has 0 as the last element.
 #:
 #: .. versionadded:: 1.2
 #:    Before version 1.2, check the string ``sphinx.__version__``.
-version_info = (7, 1, 1, 'final', 0)
+version_info = (7, 1, 2, 'final', 0)
 
 package_dir = path.abspath(path.dirname(__file__))
 
 _in_development = False
 if _in_development:
     # Only import subprocess if needed
     import subprocess
```

### Comparing `sphinx-7.1.1/sphinx/addnodes.py` & `sphinx-7.1.2/sphinx/addnodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/application.py` & `sphinx-7.1.2/sphinx/application.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/__init__.py` & `sphinx-7.1.2/sphinx/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/_epub_base.py` & `sphinx-7.1.2/sphinx/builders/_epub_base.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/changes.py` & `sphinx-7.1.2/sphinx/builders/changes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/dirhtml.py` & `sphinx-7.1.2/sphinx/builders/dirhtml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/dummy.py` & `sphinx-7.1.2/sphinx/builders/dummy.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/epub3.py` & `sphinx-7.1.2/sphinx/builders/epub3.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/gettext.py` & `sphinx-7.1.2/sphinx/builders/gettext.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/html/__init__.py` & `sphinx-7.1.2/sphinx/builders/html/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/html/transforms.py` & `sphinx-7.1.2/sphinx/builders/html/transforms.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/latex/__init__.py` & `sphinx-7.1.2/sphinx/builders/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/latex/constants.py` & `sphinx-7.1.2/sphinx/builders/latex/constants.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/latex/nodes.py` & `sphinx-7.1.2/sphinx/builders/latex/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/latex/theming.py` & `sphinx-7.1.2/sphinx/builders/latex/theming.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/latex/transforms.py` & `sphinx-7.1.2/sphinx/builders/latex/transforms.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/latex/util.py` & `sphinx-7.1.2/sphinx/builders/latex/util.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/linkcheck.py` & `sphinx-7.1.2/sphinx/builders/linkcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def finish(self) -> None:
         checker = HyperlinkAvailabilityChecker(self.config)
         logger.info('')
 
         output_text = path.join(self.outdir, 'output.txt')
         output_json = path.join(self.outdir, 'output.json')
-        with open(output_text, 'w', encoding='utf-8') as self.txt_outfile,\
+        with open(output_text, 'w', encoding='utf-8') as self.txt_outfile, \
              open(output_json, 'w', encoding='utf-8') as self.json_outfile:
             for result in checker.check(self.hyperlinks):
                 self.process_result(result)
 
         if self.broken_hyperlinks:
             self.app.statuscode = 1
 
@@ -402,15 +402,16 @@
                     url=req_url, auth=auth_info,
                     headers=headers,
                     timeout=self.timeout,
                     **kwargs,
                     _user_agent=self.user_agent,
                     _tls_info=(self.tls_verify, self.tls_cacerts),
                 ) as response:
-                    if response.ok and anchor and not contains_anchor(response, anchor):
+                    if (self.check_anchors and response.ok and anchor
+                            and not contains_anchor(response, anchor)):
                         raise Exception(__(f'Anchor {anchor!r} not found'))
 
                 # Copy data we need from the (closed) response
                 status_code = response.status_code
                 redirect_status_code = response.history[-1].status_code if response.history else None  # NoQA: E501
                 retry_after = response.headers.get('Retry-After')
                 response_url = f'{response.url}'
```

### Comparing `sphinx-7.1.1/sphinx/builders/manpage.py` & `sphinx-7.1.2/sphinx/builders/manpage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/singlehtml.py` & `sphinx-7.1.2/sphinx/builders/singlehtml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/texinfo.py` & `sphinx-7.1.2/sphinx/builders/texinfo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/text.py` & `sphinx-7.1.2/sphinx/builders/text.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/builders/xml.py` & `sphinx-7.1.2/sphinx/builders/xml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/cmd/build.py` & `sphinx-7.1.2/sphinx/cmd/build.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/cmd/make_mode.py` & `sphinx-7.1.2/sphinx/cmd/make_mode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/cmd/quickstart.py` & `sphinx-7.1.2/sphinx/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/config.py` & `sphinx-7.1.2/sphinx/config.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/deprecation.py` & `sphinx-7.1.2/sphinx/deprecation.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/directives/__init__.py` & `sphinx-7.1.2/sphinx/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/directives/code.py` & `sphinx-7.1.2/sphinx/directives/code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/directives/other.py` & `sphinx-7.1.2/sphinx/directives/other.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/directives/patches.py` & `sphinx-7.1.2/sphinx/directives/patches.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/__init__.py` & `sphinx-7.1.2/sphinx/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/c.py` & `sphinx-7.1.2/sphinx/domains/c.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/changeset.py` & `sphinx-7.1.2/sphinx/domains/changeset.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/citation.py` & `sphinx-7.1.2/sphinx/domains/citation.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/cpp.py` & `sphinx-7.1.2/sphinx/domains/cpp.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/index.py` & `sphinx-7.1.2/sphinx/domains/index.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/javascript.py` & `sphinx-7.1.2/sphinx/domains/javascript.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/math.py` & `sphinx-7.1.2/sphinx/domains/math.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/python.py` & `sphinx-7.1.2/sphinx/domains/python.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/rst.py` & `sphinx-7.1.2/sphinx/domains/rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/domains/std.py` & `sphinx-7.1.2/sphinx/domains/std.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/__init__.py` & `sphinx-7.1.2/sphinx/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/adapters/indexentries.py` & `sphinx-7.1.2/sphinx/environment/adapters/indexentries.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/adapters/toctree.py` & `sphinx-7.1.2/sphinx/environment/adapters/toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/collectors/__init__.py` & `sphinx-7.1.2/sphinx/environment/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/collectors/asset.py` & `sphinx-7.1.2/sphinx/environment/collectors/asset.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/collectors/dependencies.py` & `sphinx-7.1.2/sphinx/environment/collectors/dependencies.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/collectors/metadata.py` & `sphinx-7.1.2/sphinx/environment/collectors/metadata.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/collectors/title.py` & `sphinx-7.1.2/sphinx/environment/collectors/title.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/environment/collectors/toctree.py` & `sphinx-7.1.2/sphinx/environment/collectors/toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/errors.py` & `sphinx-7.1.2/sphinx/errors.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/events.py` & `sphinx-7.1.2/sphinx/events.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/apidoc.py` & `sphinx-7.1.2/sphinx/ext/apidoc.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autodoc/__init__.py` & `sphinx-7.1.2/sphinx/ext/autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autodoc/directive.py` & `sphinx-7.1.2/sphinx/ext/autodoc/directive.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autodoc/importer.py` & `sphinx-7.1.2/sphinx/ext/autodoc/importer.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autodoc/mock.py` & `sphinx-7.1.2/sphinx/ext/autodoc/mock.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autodoc/preserve_defaults.py` & `sphinx-7.1.2/sphinx/ext/autodoc/preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autodoc/type_comment.py` & `sphinx-7.1.2/sphinx/ext/autodoc/type_comment.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autodoc/typehints.py` & `sphinx-7.1.2/sphinx/ext/autodoc/typehints.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autosectionlabel.py` & `sphinx-7.1.2/sphinx/ext/autosectionlabel.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autosummary/__init__.py` & `sphinx-7.1.2/sphinx/ext/autosummary/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autosummary/generate.py` & `sphinx-7.1.2/sphinx/ext/autosummary/generate.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autosummary/templates/autosummary/class.rst` & `sphinx-7.1.2/sphinx/ext/autosummary/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/autosummary/templates/autosummary/module.rst` & `sphinx-7.1.2/sphinx/ext/autosummary/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/coverage.py` & `sphinx-7.1.2/sphinx/ext/coverage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/doctest.py` & `sphinx-7.1.2/sphinx/ext/doctest.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/duration.py` & `sphinx-7.1.2/sphinx/ext/duration.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/extlinks.py` & `sphinx-7.1.2/sphinx/ext/extlinks.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/githubpages.py` & `sphinx-7.1.2/sphinx/ext/githubpages.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/graphviz.py` & `sphinx-7.1.2/sphinx/ext/graphviz.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/ifconfig.py` & `sphinx-7.1.2/sphinx/ext/ifconfig.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/imgconverter.py` & `sphinx-7.1.2/sphinx/ext/imgconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/imgmath.py` & `sphinx-7.1.2/sphinx/ext/imgmath.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/inheritance_diagram.py` & `sphinx-7.1.2/sphinx/ext/inheritance_diagram.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/intersphinx.py` & `sphinx-7.1.2/sphinx/ext/intersphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/linkcode.py` & `sphinx-7.1.2/sphinx/ext/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/mathjax.py` & `sphinx-7.1.2/sphinx/ext/mathjax.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/napoleon/__init__.py` & `sphinx-7.1.2/sphinx/ext/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/napoleon/docstring.py` & `sphinx-7.1.2/sphinx/ext/napoleon/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/todo.py` & `sphinx-7.1.2/sphinx/ext/todo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/ext/viewcode.py` & `sphinx-7.1.2/sphinx/ext/viewcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/extension.py` & `sphinx-7.1.2/sphinx/extension.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/highlighting.py` & `sphinx-7.1.2/sphinx/highlighting.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/io.py` & `sphinx-7.1.2/sphinx/io.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/jinja2glue.py` & `sphinx-7.1.2/sphinx/jinja2glue.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/__init__.py` & `sphinx-7.1.2/sphinx/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ar/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ar/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ar/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ar/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ar/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ar/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/bg/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/bg/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/bg/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/bg/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/bn/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/bn/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/bn/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/bn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/bn/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/bn/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ca/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ca/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ca/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ca/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ca/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ca/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cak/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/cak/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cak/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/cak/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cak/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/cak/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cs/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/cs/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cs/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/cs/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cs/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/cs/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cy/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/cy/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cy/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/cy/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/cy/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/cy/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/da/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/da/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/da/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/da/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/da/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/da/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/de/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/de/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/de/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/de/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/de/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/el/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/el/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/el/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/el/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/el/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/el/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/eo/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/eo/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/eo/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/eo/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/eo/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/eo/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/es/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/es/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/es/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/es/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/es/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/et/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/et/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/et/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/et/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/et/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/et/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/eu/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/eu/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/eu/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/eu/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/eu/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/eu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fa/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/fa/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fa/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/fa/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fa/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/fa/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fi/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/fi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fi/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/fi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fi/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/fi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fr/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/fr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fr/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fr/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/fr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/he/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/he/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/he/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/he/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/he/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/he/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hi/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/hi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hi/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/hi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hi/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/hi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hr/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/hr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hr/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/hr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hr/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/hr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hu/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/hu/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hu/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/hu/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/hu/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/hu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/id/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/id/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/id/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/id/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/id/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/id/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/is/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/is/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/is/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/is/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/is/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/is/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/it/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/it/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/it/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/it/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/it/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/it/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ja/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ja/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ja/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ja/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ja/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ja/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ka/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ka/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ka/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ka/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ka/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ka/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ko/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ko/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ko/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ko/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ko/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ko/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/lt/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/lt/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/lt/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/lt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/lt/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/lt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/lv/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/lv/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/lv/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/lv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/lv/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/lv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/mk/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/mk/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/mk/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/mk/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/mk/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/mk/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ne/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ne/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ne/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ne/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ne/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ne/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/nl/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/nl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/nl/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/nl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/nl/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/nl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pl/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/pl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pl/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/pl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pl/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/pl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/pt/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/pt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ro/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ro/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ro/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ro/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ro/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ro/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ru/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ru/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ru/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ru/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ru/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ru/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/si/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/si/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/si/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/si/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/si/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/si/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sk/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/sk/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sk/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/sk/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sk/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/sk/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sl/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/sl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sl/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/sl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sl/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/sl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sphinx.pot` & `sphinx-7.1.2/sphinx/locale/sphinx.pot`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sq/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/sq/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sq/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/sq/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sq/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/sq/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/sr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/sr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sv/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/sv/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sv/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/sv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/sv/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/sv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ta/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ta/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ta/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/ta/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ta/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ta/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/te/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/te/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/te/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/te/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/tr/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/tr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/tr/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/tr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/tr/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/tr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ur/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/ur/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/ur/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/ur/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/vi/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/vi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/vi/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/vi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/vi/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/vi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/yue/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/yue/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/yue/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/yue/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js` & `sphinx-7.1.2/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo` & `sphinx-7.1.2/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/parsers.py` & `sphinx-7.1.2/sphinx/parsers.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/project.py` & `sphinx-7.1.2/sphinx/project.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/pycode/__init__.py` & `sphinx-7.1.2/sphinx/pycode/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/pycode/ast.py` & `sphinx-7.1.2/sphinx/pycode/ast.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/pycode/parser.py` & `sphinx-7.1.2/sphinx/pycode/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/pygments_styles.py` & `sphinx-7.1.2/sphinx/pygments_styles.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/registry.py` & `sphinx-7.1.2/sphinx/registry.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/roles.py` & `sphinx-7.1.2/sphinx/roles.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/__init__.py` & `sphinx-7.1.2/sphinx/search/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/da.py` & `sphinx-7.1.2/sphinx/search/da.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/de.py` & `sphinx-7.1.2/sphinx/search/de.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/en.py` & `sphinx-7.1.2/sphinx/search/en.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/es.py` & `sphinx-7.1.2/sphinx/search/es.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/fi.py` & `sphinx-7.1.2/sphinx/search/fi.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/fr.py` & `sphinx-7.1.2/sphinx/search/fr.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/hu.py` & `sphinx-7.1.2/sphinx/search/hu.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/it.py` & `sphinx-7.1.2/sphinx/search/it.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/ja.py` & `sphinx-7.1.2/sphinx/search/ja.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/base-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/danish-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/danish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/dutch-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/dutch-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/finnish-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/finnish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/french-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/french-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/german-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/german-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/hungarian-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/hungarian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/italian-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/italian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/norwegian-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/norwegian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/porter-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/porter-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/portuguese-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/portuguese-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/romanian-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/romanian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/russian-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/russian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/spanish-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/spanish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/swedish-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/swedish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/minified-js/turkish-stemmer.js` & `sphinx-7.1.2/sphinx/search/minified-js/turkish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/nl.py` & `sphinx-7.1.2/sphinx/search/nl.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/no.py` & `sphinx-7.1.2/sphinx/search/no.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/base-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/danish-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/danish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/dutch-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/dutch-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/finnish-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/finnish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/french-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/french-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/german-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/german-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/hungarian-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/hungarian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/italian-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/italian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/norwegian-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/norwegian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/porter-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/porter-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/portuguese-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/portuguese-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/romanian-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/romanian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/russian-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/russian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/spanish-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/spanish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/swedish-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/swedish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/non-minified-js/turkish-stemmer.js` & `sphinx-7.1.2/sphinx/search/non-minified-js/turkish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/pt.py` & `sphinx-7.1.2/sphinx/search/pt.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/ro.py` & `sphinx-7.1.2/sphinx/search/ro.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/ru.py` & `sphinx-7.1.2/sphinx/search/ru.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/sv.py` & `sphinx-7.1.2/sphinx/search/sv.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/tr.py` & `sphinx-7.1.2/sphinx/search/tr.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/search/zh.py` & `sphinx-7.1.2/sphinx/search/zh.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/apidoc/package.rst_t` & `sphinx-7.1.2/sphinx/templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/epub3/content.opf_t` & `sphinx-7.1.2/sphinx/templates/epub3/content.opf_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/epub3/nav.xhtml_t` & `sphinx-7.1.2/sphinx/templates/epub3/nav.xhtml_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/epub3/toc.ncx_t` & `sphinx-7.1.2/sphinx/templates/epub3/toc.ncx_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/gettext/message.pot_t` & `sphinx-7.1.2/sphinx/templates/gettext/message.pot_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/htmlhelp/project.hhc` & `sphinx-7.1.2/sphinx/templates/htmlhelp/project.hhc`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/htmlhelp/project.hhp` & `sphinx-7.1.2/sphinx/templates/htmlhelp/project.hhp`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/latex/latex.tex_t` & `sphinx-7.1.2/sphinx/templates/latex/latex.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/latex/longtable.tex_t` & `sphinx-7.1.2/sphinx/templates/latex/longtable.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/latex/sphinxmessages.sty_t` & `sphinx-7.1.2/sphinx/templates/latex/sphinxmessages.sty_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/latex/tabular.tex_t` & `sphinx-7.1.2/sphinx/templates/latex/tabular.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/latex/tabulary.tex_t` & `sphinx-7.1.2/sphinx/templates/latex/tabulary.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/quickstart/Makefile.new_t` & `sphinx-7.1.2/sphinx/templates/quickstart/Makefile.new_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/quickstart/Makefile_t` & `sphinx-7.1.2/sphinx/templates/quickstart/Makefile_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/quickstart/conf.py_t` & `sphinx-7.1.2/sphinx/templates/quickstart/conf.py_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/quickstart/make.bat.new_t` & `sphinx-7.1.2/sphinx/templates/quickstart/make.bat.new_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/quickstart/make.bat_t` & `sphinx-7.1.2/sphinx/templates/quickstart/make.bat_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/templates/texinfo/Makefile` & `sphinx-7.1.2/sphinx/templates/texinfo/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/testing/comparer.py` & `sphinx-7.1.2/sphinx/testing/comparer.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/testing/fixtures.py` & `sphinx-7.1.2/sphinx/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/testing/path.py` & `sphinx-7.1.2/sphinx/testing/path.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/testing/restructuredtext.py` & `sphinx-7.1.2/sphinx/testing/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/testing/util.py` & `sphinx-7.1.2/sphinx/testing/util.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/LICRcyr2utf8.xdy` & `sphinx-7.1.2/sphinx/texinputs/LICRcyr2utf8.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/LICRlatin2utf8.xdy` & `sphinx-7.1.2/sphinx/texinputs/LICRlatin2utf8.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/LatinRules.xdy` & `sphinx-7.1.2/sphinx/texinputs/LatinRules.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/Makefile_t` & `sphinx-7.1.2/sphinx/texinputs/Makefile_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/latexmkjarc_t` & `sphinx-7.1.2/sphinx/texinputs/latexmkjarc_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/latexmkrc_t` & `sphinx-7.1.2/sphinx/texinputs/latexmkrc_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/make.bat_t` & `sphinx-7.1.2/sphinx/texinputs/make.bat_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinx.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinx.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinx.xdy` & `sphinx-7.1.2/sphinx/texinputs/sphinx.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxhowto.cls` & `sphinx-7.1.2/sphinx/texinputs/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexadmonitions.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexadmonitions.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexcontainers.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexcontainers.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexgraphics.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexgraphics.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexindbibtoc.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexindbibtoc.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexlists.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexlists.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexliterals.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexliterals.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexnumfig.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexnumfig.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexobjects.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexobjects.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexshadowbox.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexshadowbox.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexstyleheadings.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexstyleheadings.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexstylepage.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexstylepage.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatexstyletext.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatexstyletext.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxlatextables.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxlatextables.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxmanual.cls` & `sphinx-7.1.2/sphinx/texinputs/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxoptionsgeometry.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxoptionsgeometry.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxoptionshyperref.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxoptionshyperref.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxpackageboxes.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxpackageboxes.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxpackagecyrillic.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxpackagecyrillic.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs/sphinxpackagefootnote.sty` & `sphinx-7.1.2/sphinx/texinputs/sphinxpackagefootnote.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/texinputs_win/Makefile_t` & `sphinx-7.1.2/sphinx/texinputs_win/Makefile_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/agogo/layout.html` & `sphinx-7.1.2/sphinx/themes/agogo/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/agogo/static/agogo.css_t` & `sphinx-7.1.2/sphinx/themes/agogo/static/agogo.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/changes/versionchanges.html` & `sphinx-7.1.2/sphinx/themes/basic/changes/versionchanges.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/defindex.html` & `sphinx-7.1.2/sphinx/themes/basic/defindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/domainindex.html` & `sphinx-7.1.2/sphinx/themes/basic/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/genindex-single.html` & `sphinx-7.1.2/sphinx/themes/basic/genindex-single.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/genindex-split.html` & `sphinx-7.1.2/sphinx/themes/basic/genindex-split.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/genindex.html` & `sphinx-7.1.2/sphinx/themes/basic/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/layout.html` & `sphinx-7.1.2/sphinx/themes/basic/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/opensearch.xml` & `sphinx-7.1.2/sphinx/themes/basic/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/relations.html` & `sphinx-7.1.2/sphinx/themes/basic/relations.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/search.html` & `sphinx-7.1.2/sphinx/themes/basic/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/searchbox.html` & `sphinx-7.1.2/sphinx/themes/basic/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/searchfield.html` & `sphinx-7.1.2/sphinx/themes/basic/searchfield.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/sourcelink.html` & `sphinx-7.1.2/sphinx/themes/basic/sourcelink.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/static/basic.css_t` & `sphinx-7.1.2/sphinx/themes/basic/static/basic.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/static/doctools.js` & `sphinx-7.1.2/sphinx/themes/basic/static/doctools.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/static/documentation_options.js_t` & `sphinx-7.1.2/sphinx/themes/basic/static/documentation_options.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/static/language_data.js_t` & `sphinx-7.1.2/sphinx/themes/basic/static/language_data.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/static/searchtools.js` & `sphinx-7.1.2/sphinx/themes/basic/static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/basic/static/sphinx_highlight.js` & `sphinx-7.1.2/sphinx/themes/basic/static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/bizstyle/layout.html` & `sphinx-7.1.2/sphinx/themes/bizstyle/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/bizstyle/static/bizstyle.css_t` & `sphinx-7.1.2/sphinx/themes/bizstyle/static/bizstyle.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/bizstyle/static/bizstyle.js_t` & `sphinx-7.1.2/sphinx/themes/bizstyle/static/bizstyle.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/bizstyle/static/css3-mediaqueries.js` & `sphinx-7.1.2/sphinx/themes/bizstyle/static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js` & `sphinx-7.1.2/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/classic/layout.html` & `sphinx-7.1.2/sphinx/themes/classic/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/classic/static/classic.css_t` & `sphinx-7.1.2/sphinx/themes/classic/static/classic.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/classic/static/sidebar.js_t` & `sphinx-7.1.2/sphinx/themes/classic/static/sidebar.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/classic/theme.conf` & `sphinx-7.1.2/sphinx/themes/classic/theme.conf`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/epub/epub-cover.html` & `sphinx-7.1.2/sphinx/themes/epub/epub-cover.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/epub/layout.html` & `sphinx-7.1.2/sphinx/themes/epub/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/epub/static/epub.css_t` & `sphinx-7.1.2/sphinx/themes/epub/static/epub.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/haiku/layout.html` & `sphinx-7.1.2/sphinx/themes/haiku/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/haiku/static/alert_info_32.png` & `sphinx-7.1.2/sphinx/themes/haiku/static/alert_info_32.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/haiku/static/alert_warning_32.png` & `sphinx-7.1.2/sphinx/themes/haiku/static/alert_warning_32.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/haiku/static/haiku.css_t` & `sphinx-7.1.2/sphinx/themes/haiku/static/haiku.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/nature/static/nature.css_t` & `sphinx-7.1.2/sphinx/themes/nature/static/nature.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/nonav/layout.html` & `sphinx-7.1.2/sphinx/themes/nonav/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/nonav/static/nonav.css_t` & `sphinx-7.1.2/sphinx/themes/nonav/static/nonav.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/layout.html` & `sphinx-7.1.2/sphinx/themes/pyramid/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-note.png` & `sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-note.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-seealso.png` & `sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-seealso.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-todo.png` & `sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-todo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-topic.png` & `sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-topic.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/dialog-warning.png` & `sphinx-7.1.2/sphinx/themes/pyramid/static/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/epub.css_t` & `sphinx-7.1.2/sphinx/themes/pyramid/static/epub.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/ie6.css` & `sphinx-7.1.2/sphinx/themes/pyramid/static/ie6.css`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/pyramid/static/pyramid.css_t` & `sphinx-7.1.2/sphinx/themes/pyramid/static/pyramid.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/artwork/logo.svg` & `sphinx-7.1.2/sphinx/themes/scrolls/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/layout.html` & `sphinx-7.1.2/sphinx/themes/scrolls/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/static/darkmetal.png` & `sphinx-7.1.2/sphinx/themes/scrolls/static/darkmetal.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/static/logo.png` & `sphinx-7.1.2/sphinx/themes/scrolls/static/logo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/static/metal.png` & `sphinx-7.1.2/sphinx/themes/scrolls/static/metal.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/static/scrolls.css_t` & `sphinx-7.1.2/sphinx/themes/scrolls/static/scrolls.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/static/theme_extras.js` & `sphinx-7.1.2/sphinx/themes/scrolls/static/theme_extras.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/static/watermark.png` & `sphinx-7.1.2/sphinx/themes/scrolls/static/watermark.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/scrolls/static/watermark_blur.png` & `sphinx-7.1.2/sphinx/themes/scrolls/static/watermark_blur.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t` & `sphinx-7.1.2/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/themes/traditional/static/traditional.css_t` & `sphinx-7.1.2/sphinx/themes/traditional/static/traditional.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/theming.py` & `sphinx-7.1.2/sphinx/theming.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/transforms/__init__.py` & `sphinx-7.1.2/sphinx/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/transforms/compact_bullet_list.py` & `sphinx-7.1.2/sphinx/transforms/compact_bullet_list.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/transforms/i18n.py` & `sphinx-7.1.2/sphinx/transforms/i18n.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/transforms/post_transforms/__init__.py` & `sphinx-7.1.2/sphinx/transforms/post_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/transforms/post_transforms/code.py` & `sphinx-7.1.2/sphinx/transforms/post_transforms/code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/transforms/post_transforms/images.py` & `sphinx-7.1.2/sphinx/transforms/post_transforms/images.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/transforms/references.py` & `sphinx-7.1.2/sphinx/transforms/references.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/__init__.py` & `sphinx-7.1.2/sphinx/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/cfamily.py` & `sphinx-7.1.2/sphinx/util/cfamily.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/console.py` & `sphinx-7.1.2/sphinx/util/console.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/display.py` & `sphinx-7.1.2/sphinx/util/display.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/docfields.py` & `sphinx-7.1.2/sphinx/util/docfields.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/docstrings.py` & `sphinx-7.1.2/sphinx/util/docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/docutils.py` & `sphinx-7.1.2/sphinx/util/docutils.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/exceptions.py` & `sphinx-7.1.2/sphinx/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/fileutil.py` & `sphinx-7.1.2/sphinx/util/fileutil.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/http_date.py` & `sphinx-7.1.2/sphinx/util/http_date.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/i18n.py` & `sphinx-7.1.2/sphinx/util/i18n.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/images.py` & `sphinx-7.1.2/sphinx/util/images.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/inspect.py` & `sphinx-7.1.2/sphinx/util/inspect.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/inventory.py` & `sphinx-7.1.2/sphinx/util/inventory.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/logging.py` & `sphinx-7.1.2/sphinx/util/logging.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/matching.py` & `sphinx-7.1.2/sphinx/util/matching.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/math.py` & `sphinx-7.1.2/sphinx/util/math.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/nodes.py` & `sphinx-7.1.2/sphinx/util/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/osutil.py` & `sphinx-7.1.2/sphinx/util/osutil.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/parallel.py` & `sphinx-7.1.2/sphinx/util/parallel.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/png.py` & `sphinx-7.1.2/sphinx/util/png.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/requests.py` & `sphinx-7.1.2/sphinx/util/requests.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/rst.py` & `sphinx-7.1.2/sphinx/util/rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/tags.py` & `sphinx-7.1.2/sphinx/util/tags.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/template.py` & `sphinx-7.1.2/sphinx/util/template.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/texescape.py` & `sphinx-7.1.2/sphinx/util/texescape.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/util/typing.py` & `sphinx-7.1.2/sphinx/util/typing.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/versioning.py` & `sphinx-7.1.2/sphinx/versioning.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/writers/html.py` & `sphinx-7.1.2/sphinx/writers/html.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/writers/html5.py` & `sphinx-7.1.2/sphinx/writers/html5.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/writers/latex.py` & `sphinx-7.1.2/sphinx/writers/latex.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/writers/manpage.py` & `sphinx-7.1.2/sphinx/writers/manpage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/writers/texinfo.py` & `sphinx-7.1.2/sphinx/writers/texinfo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/writers/text.py` & `sphinx-7.1.2/sphinx/writers/text.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/sphinx/writers/xml.py` & `sphinx-7.1.2/sphinx/writers/xml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/certs/cert.pem` & `sphinx-7.1.2/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/conftest.py` & `sphinx-7.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/js/searchtools.js` & `sphinx-7.1.2/tests/js/searchtools.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/js/sphinx_highlight.js` & `sphinx-7.1.2/tests/js/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-add_enumerable_node/enumerable_node.py` & `sphinx-7.1.2/tests/roots/test-add_enumerable_node/enumerable_node.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-add_enumerable_node/index.rst` & `sphinx-7.1.2/tests/roots/test-add_enumerable_node/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-api-set-translator/conf.py` & `sphinx-7.1.2/tests/roots/test-api-set-translator/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-autosummary/dummy_module.py` & `sphinx-7.1.2/tests/roots/test-autosummary/dummy_module.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-basic/index.rst` & `sphinx-7.1.2/tests/roots/test-basic/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-directive-code/caption.rst` & `sphinx-7.1.2/tests/roots/test-directive-code/caption.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-directive-code/dedent.rst` & `sphinx-7.1.2/tests/roots/test-directive-code/dedent.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-directive-only/only.rst` & `sphinx-7.1.2/tests/roots/test-directive-only/only.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-c-intersphinx/index.rst` & `sphinx-7.1.2/tests/roots/test-domain-c-intersphinx/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-c/index.rst` & `sphinx-7.1.2/tests/roots/test-domain-c/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-cpp-intersphinx/index.rst` & `sphinx-7.1.2/tests/roots/test-domain-cpp-intersphinx/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-cpp/any-role.rst` & `sphinx-7.1.2/tests/roots/test-domain-cpp/any-role.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-cpp/index.rst` & `sphinx-7.1.2/tests/roots/test-domain-cpp/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-cpp/roles-targets-ok.rst` & `sphinx-7.1.2/tests/roots/test-domain-cpp/roles-targets-ok.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-cpp/roles-targets-warn.rst` & `sphinx-7.1.2/tests/roots/test-domain-cpp/roles-targets-warn.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-cpp/roles.rst` & `sphinx-7.1.2/tests/roots/test-domain-cpp/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-js/module.rst` & `sphinx-7.1.2/tests/roots/test-domain-js/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-js/roles.rst` & `sphinx-7.1.2/tests/roots/test-domain-js/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-py/module.rst` & `sphinx-7.1.2/tests/roots/test-domain-py/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-domain-py/roles.rst` & `sphinx-7.1.2/tests/roots/test-domain-py/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/__init__.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/autoclass_content.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/autoclass_content.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/classes.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/classes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/coroutine.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/coroutine.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/decorator.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/decorator.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/descriptor.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/descriptor.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/docstring_signature.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/docstring_signature.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/need_mocks.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/need_mocks.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/overload.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/overload.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/preserve_defaults.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/private.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/private.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/singledispatch.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/singledispatch.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/singledispatchmethod.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/singledispatchmethod.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/typed_vars.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/typed_vars.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autodoc/target/typehints.py` & `sphinx-7.1.2/tests/roots/test-ext-autodoc/target/typehints.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst` & `sphinx-7.1.2/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autosectionlabel/index.rst` & `sphinx-7.1.2/tests/roots/test-ext-autosectionlabel/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-autosummary/autosummary_dummy_module.py` & `sphinx-7.1.2/tests/roots/test-ext-autosummary/autosummary_dummy_module.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-doctest-skipif/skipif.txt` & `sphinx-7.1.2/tests/roots/test-ext-doctest-skipif/skipif.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-doctest/doctest.txt` & `sphinx-7.1.2/tests/roots/test-ext-doctest/doctest.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst` & `sphinx-7.1.2/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst` & `sphinx-7.1.2/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-imgconverter/img.pdf` & `sphinx-7.1.2/tests/roots/test-ext-imgconverter/img.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py` & `sphinx-7.1.2/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-intersphinx-role/index.rst` & `sphinx-7.1.2/tests/roots/test-ext-intersphinx-role/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-viewcode-find/index.rst` & `sphinx-7.1.2/tests/roots/test-ext-viewcode-find/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-viewcode/conf.py` & `sphinx-7.1.2/tests/roots/test-ext-viewcode/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-viewcode/index.rst` & `sphinx-7.1.2/tests/roots/test-ext-viewcode/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-ext-viewcode/objects.rst` & `sphinx-7.1.2/tests/roots/test-ext-viewcode/objects.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-footnotes/index.rst` & `sphinx-7.1.2/tests/roots/test-footnotes/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-html_entity/index.rst` & `sphinx-7.1.2/tests/roots/test-html_entity/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-html_scaled_image_link/img.png` & `sphinx-7.1.2/tests/roots/test-html_scaled_image_link/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-image-escape/img_#1.png` & `sphinx-7.1.2/tests/roots/test-image-escape/img_#1.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-images/img.gif` & `sphinx-7.1.2/tests/roots/test-images/img.gif`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-images/img.ja.png` & `sphinx-7.1.2/tests/roots/test-images/img.ja.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-images/img.pdf` & `sphinx-7.1.2/tests/roots/test-images/img.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-images/img.png` & `sphinx-7.1.2/tests/roots/test-images/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-images/img.zh.png` & `sphinx-7.1.2/tests/roots/test-images/img.zh.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-images/subdir/svgimg.pdf` & `sphinx-7.1.2/tests/roots/test-images/subdir/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-images/testimäge.png` & `sphinx-7.1.2/tests/roots/test-images/testimäge.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/admonitions.txt` & `sphinx-7.1.2/tests/roots/test-intl/admonitions.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/docfields.txt` & `sphinx-7.1.2/tests/roots/test-intl/docfields.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/external_links.txt` & `sphinx-7.1.2/tests/roots/test-intl/external_links.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/figure.txt` & `sphinx-7.1.2/tests/roots/test-intl/figure.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/i18n.png` & `sphinx-7.1.2/tests/roots/test-intl/i18n.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/img.png` & `sphinx-7.1.2/tests/roots/test-intl/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/index.txt` & `sphinx-7.1.2/tests/roots/test-intl/index.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/label_target.txt` & `sphinx-7.1.2/tests/roots/test-intl/label_target.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/literalblock.txt` & `sphinx-7.1.2/tests/roots/test-intl/literalblock.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/refs.txt` & `sphinx-7.1.2/tests/roots/test-intl/refs.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/role_xref.txt` & `sphinx-7.1.2/tests/roots/test-intl/role_xref.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/translation_progress.txt` & `sphinx-7.1.2/tests/roots/test-intl/translation_progress.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/figure.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/figure.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/index.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/only.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/only.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/raw.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/raw.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/refs.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/refs.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/section.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/section.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/table.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/table.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/topic.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/topic.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po` & `sphinx-7.1.2/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-figure-in-admonition/img.png` & `sphinx-7.1.2/tests/roots/test-latex-figure-in-admonition/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-includegraphics/conf.py` & `sphinx-7.1.2/tests/roots/test-latex-includegraphics/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-includegraphics/img.png` & `sphinx-7.1.2/tests/roots/test-latex-includegraphics/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-includegraphics/index.rst` & `sphinx-7.1.2/tests/roots/test-latex-includegraphics/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-includegraphics/sphinx.png` & `sphinx-7.1.2/tests/roots/test-latex-includegraphics/sphinx.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-includegraphics/tall.png` & `sphinx-7.1.2/tests/roots/test-latex-includegraphics/tall.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-labels/index.rst` & `sphinx-7.1.2/tests/roots/test-latex-labels/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/complex.rst` & `sphinx-7.1.2/tests/roots/test-latex-table/complex.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/complex_spanning_cell.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/complex_spanning_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/gridtable.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/gridtable.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_align.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_align.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_caption.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_caption.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_widths.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/simple_table.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/simple_table.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_caption.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_caption.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_verbatim.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_verbatim.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_widths.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/tabular_having_widths.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/tabular_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/tabularcolumn.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/expects/tabulary_having_widths.tex` & `sphinx-7.1.2/tests/roots/test-latex-table/expects/tabulary_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/longtable.rst` & `sphinx-7.1.2/tests/roots/test-latex-table/longtable.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-latex-table/tabular.rst` & `sphinx-7.1.2/tests/roots/test-latex-table/tabular.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst` & `sphinx-7.1.2/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-linkcheck/links.rst` & `sphinx-7.1.2/tests/roots/test-linkcheck/links.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-local-logo/images/img.png` & `sphinx-7.1.2/tests/roots/test-local-logo/images/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-local-logo/index.rst` & `sphinx-7.1.2/tests/roots/test-local-logo/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-maxlistdepth/index.rst` & `sphinx-7.1.2/tests/roots/test-maxlistdepth/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-metadata/index.rst` & `sphinx-7.1.2/tests/roots/test-metadata/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-need-escaped/index.rst` & `sphinx-7.1.2/tests/roots/test-need-escaped/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-numfig/bar.rst` & `sphinx-7.1.2/tests/roots/test-numfig/bar.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-numfig/foo.rst` & `sphinx-7.1.2/tests/roots/test-numfig/foo.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-numfig/index.rst` & `sphinx-7.1.2/tests/roots/test-numfig/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-productionlist/index.rst` & `sphinx-7.1.2/tests/roots/test-productionlist/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-remote-logo/index.rst` & `sphinx-7.1.2/tests/roots/test-remote-logo/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/Makefile` & `sphinx-7.1.2/tests/roots/test-root/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/autodoc.txt` & `sphinx-7.1.2/tests/roots/test-root/autodoc.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/autodoc_target.py` & `sphinx-7.1.2/tests/roots/test-root/autodoc_target.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/conf.py` & `sphinx-7.1.2/tests/roots/test-root/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/footnote.txt` & `sphinx-7.1.2/tests/roots/test-root/footnote.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/images.txt` & `sphinx-7.1.2/tests/roots/test-root/images.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/img.foo.png` & `sphinx-7.1.2/tests/roots/test-root/img.foo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/img.gif` & `sphinx-7.1.2/tests/roots/test-root/img.gif`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/img.pdf` & `sphinx-7.1.2/tests/roots/test-root/img.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/img.png` & `sphinx-7.1.2/tests/roots/test-root/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/includes.txt` & `sphinx-7.1.2/tests/roots/test-root/includes.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/index.txt` & `sphinx-7.1.2/tests/roots/test-root/index.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/lists.txt` & `sphinx-7.1.2/tests/roots/test-root/lists.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/markup.txt` & `sphinx-7.1.2/tests/roots/test-root/markup.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/objects.txt` & `sphinx-7.1.2/tests/roots/test-root/objects.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/subdir/img.png` & `sphinx-7.1.2/tests/roots/test-root/subdir/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/subdir/simg.png` & `sphinx-7.1.2/tests/roots/test-root/subdir/simg.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-root/svgimg.pdf` & `sphinx-7.1.2/tests/roots/test-root/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-theming/child.zip` & `sphinx-7.1.2/tests/roots/test-theming/child.zip`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-theming/parent.zip` & `sphinx-7.1.2/tests/roots/test-theming/parent.zip`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-theming/ziptheme.zip` & `sphinx-7.1.2/tests/roots/test-theming/ziptheme.zip`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-toctree-domain-objects/domains.rst` & `sphinx-7.1.2/tests/roots/test-toctree-domain-objects/domains.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-toctree/index.rst` & `sphinx-7.1.2/tests/roots/test-toctree/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-trim_doctest_flags/index.rst` & `sphinx-7.1.2/tests/roots/test-trim_doctest_flags/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-versioning/added.txt` & `sphinx-7.1.2/tests/roots/test-versioning/added.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-versioning/deleted.txt` & `sphinx-7.1.2/tests/roots/test-versioning/deleted.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-versioning/insert.txt` & `sphinx-7.1.2/tests/roots/test-versioning/insert.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-versioning/insert_beginning.txt` & `sphinx-7.1.2/tests/roots/test-versioning/insert_beginning.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-versioning/insert_similar.txt` & `sphinx-7.1.2/tests/roots/test-versioning/insert_similar.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-versioning/modified.txt` & `sphinx-7.1.2/tests/roots/test-versioning/modified.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-versioning/original.txt` & `sphinx-7.1.2/tests/roots/test-versioning/original.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-warnings/index.rst` & `sphinx-7.1.2/tests/roots/test-warnings/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/roots/test-warnings/svgimg.pdf` & `sphinx-7.1.2/tests/roots/test-warnings/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_api_translator.py` & `sphinx-7.1.2/tests/test_api_translator.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_application.py` & `sphinx-7.1.2/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build.py` & `sphinx-7.1.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_changes.py` & `sphinx-7.1.2/tests/test_build_changes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_dirhtml.py` & `sphinx-7.1.2/tests/test_build_dirhtml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_epub.py` & `sphinx-7.1.2/tests/test_build_epub.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_gettext.py` & `sphinx-7.1.2/tests/test_build_gettext.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_html.py` & `sphinx-7.1.2/tests/test_build_html.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_latex.py` & `sphinx-7.1.2/tests/test_build_latex.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_linkcheck.py` & `sphinx-7.1.2/tests/test_build_linkcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,28 +148,45 @@
         'status': 'broken',
         'code': 0,
         'uri': 'http://localhost:7777/image2.png',
         'info': '404 Client Error: Not Found for url: http://localhost:7777/image2.png',
     }
     # looking for '#top' and '#does-not-exist' not found should fail
     assert rowsby["http://localhost:7777/#top"]["info"] == "Anchor 'top' not found"
+    assert rowsby["http://localhost:7777/#top"]["status"] == "broken"
     assert rowsby["http://localhost:7777#does-not-exist"]["info"] == "Anchor 'does-not-exist' not found"
     # images should fail
     assert "Not Found for url: http://localhost:7777/image.png" in rowsby["http://localhost:7777/image.png"]["info"]
     # anchor should be found
     assert rowsby['http://localhost:7777/anchor.html#found'] == {
         'filename': 'links.rst',
         'lineno': 14,
         'status': 'working',
         'code': 0,
         'uri': 'http://localhost:7777/anchor.html#found',
         'info': '',
     }
 
 
+@pytest.mark.sphinx(
+    'linkcheck', testroot='linkcheck', freshenv=True,
+    confoverrides={'linkcheck_anchors': False})
+def test_check_link_response_only(app):
+    with http_server(DefaultsHandler):
+        app.build()
+
+    # JSON output
+    assert (app.outdir / 'output.json').exists()
+    content = (app.outdir / 'output.json').read_text(encoding='utf8')
+
+    rows = [json.loads(x) for x in content.splitlines()]
+    rowsby = {row["uri"]: row for row in rows}
+    assert rowsby["http://localhost:7777/#top"]["status"] == "working"
+
+
 @pytest.mark.sphinx('linkcheck', testroot='linkcheck-too-many-retries', freshenv=True)
 def test_too_many_retries(app):
     with http_server(DefaultsHandler):
         app.build()
 
     # Text output
     assert (app.outdir / 'output.txt').exists()
@@ -778,15 +795,15 @@
         127.0.0.1 - - [] "HEAD / HTTP/1.1" 200 -
         """,
     )
 
 
 @pytest.mark.sphinx('linkcheck', testroot='linkcheck-localserver', freshenv=True)
 def test_too_many_requests_retry_after_without_header(app, capsys):
-    with http_server(make_retry_after_handler([(429, None), (200, None)])),\
+    with http_server(make_retry_after_handler([(429, None), (200, None)])), \
          mock.patch("sphinx.builders.linkcheck.DEFAULT_DELAY", 0):
         app.build()
     content = (app.outdir / 'output.json').read_text(encoding='utf8')
     assert json.loads(content) == {
         "filename": "index.rst",
         "lineno": 1,
         "status": "working",
```

### Comparing `sphinx-7.1.1/tests/test_build_manpage.py` & `sphinx-7.1.2/tests/test_build_manpage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_texinfo.py` & `sphinx-7.1.2/tests/test_build_texinfo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_build_text.py` & `sphinx-7.1.2/tests/test_build_text.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_builder.py` & `sphinx-7.1.2/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_catalogs.py` & `sphinx-7.1.2/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_config.py` & `sphinx-7.1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_correct_year.py` & `sphinx-7.1.2/tests/test_correct_year.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_directive_code.py` & `sphinx-7.1.2/tests/test_directive_code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_directive_object_description.py` & `sphinx-7.1.2/tests/test_directive_object_description.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_directive_only.py` & `sphinx-7.1.2/tests/test_directive_only.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_directive_other.py` & `sphinx-7.1.2/tests/test_directive_other.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_directive_patch.py` & `sphinx-7.1.2/tests/test_directive_patch.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_docutilsconf.py` & `sphinx-7.1.2/tests/test_docutilsconf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_domain_c.py` & `sphinx-7.1.2/tests/test_domain_c.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_domain_cpp.py` & `sphinx-7.1.2/tests/test_domain_cpp.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_domain_js.py` & `sphinx-7.1.2/tests/test_domain_js.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_domain_py.py` & `sphinx-7.1.2/tests/test_domain_py.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_domain_rst.py` & `sphinx-7.1.2/tests/test_domain_rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_domain_std.py` & `sphinx-7.1.2/tests/test_domain_std.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_environment.py` & `sphinx-7.1.2/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_environment_indexentries.py` & `sphinx-7.1.2/tests/test_environment_indexentries.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_environment_toctree.py` & `sphinx-7.1.2/tests/test_environment_toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_events.py` & `sphinx-7.1.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_apidoc.py` & `sphinx-7.1.2/tests/test_ext_apidoc.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc.py` & `sphinx-7.1.2/tests/test_ext_autodoc.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_autoattribute.py` & `sphinx-7.1.2/tests/test_ext_autodoc_autoattribute.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_autoclass.py` & `sphinx-7.1.2/tests/test_ext_autodoc_autoclass.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_autodata.py` & `sphinx-7.1.2/tests/test_ext_autodoc_autodata.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_autofunction.py` & `sphinx-7.1.2/tests/test_ext_autodoc_autofunction.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_automodule.py` & `sphinx-7.1.2/tests/test_ext_autodoc_automodule.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_autoproperty.py` & `sphinx-7.1.2/tests/test_ext_autodoc_autoproperty.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_configs.py` & `sphinx-7.1.2/tests/test_ext_autodoc_configs.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_events.py` & `sphinx-7.1.2/tests/test_ext_autodoc_events.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_mock.py` & `sphinx-7.1.2/tests/test_ext_autodoc_mock.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_preserve_defaults.py` & `sphinx-7.1.2/tests/test_ext_autodoc_preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autodoc_private_members.py` & `sphinx-7.1.2/tests/test_ext_autodoc_private_members.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autosectionlabel.py` & `sphinx-7.1.2/tests/test_ext_autosectionlabel.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_autosummary.py` & `sphinx-7.1.2/tests/test_ext_autosummary.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_coverage.py` & `sphinx-7.1.2/tests/test_ext_coverage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_doctest.py` & `sphinx-7.1.2/tests/test_ext_doctest.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_extlinks.py` & `sphinx-7.1.2/tests/test_ext_extlinks.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_githubpages.py` & `sphinx-7.1.2/tests/test_ext_githubpages.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_graphviz.py` & `sphinx-7.1.2/tests/test_ext_graphviz.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_ifconfig.py` & `sphinx-7.1.2/tests/test_ext_ifconfig.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_imgconverter.py` & `sphinx-7.1.2/tests/test_ext_imgconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_imgmockconverter.py` & `sphinx-7.1.2/tests/test_ext_imgmockconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_inheritance_diagram.py` & `sphinx-7.1.2/tests/test_ext_inheritance_diagram.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_intersphinx.py` & `sphinx-7.1.2/tests/test_ext_intersphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_math.py` & `sphinx-7.1.2/tests/test_ext_math.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_napoleon.py` & `sphinx-7.1.2/tests/test_ext_napoleon.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_napoleon_docstring.py` & `sphinx-7.1.2/tests/test_ext_napoleon_docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_todo.py` & `sphinx-7.1.2/tests/test_ext_todo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_ext_viewcode.py` & `sphinx-7.1.2/tests/test_ext_viewcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_extension.py` & `sphinx-7.1.2/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_highlighting.py` & `sphinx-7.1.2/tests/test_highlighting.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_intl.py` & `sphinx-7.1.2/tests/test_intl.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_locale.py` & `sphinx-7.1.2/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_markup.py` & `sphinx-7.1.2/tests/test_markup.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_metadata.py` & `sphinx-7.1.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_parser.py` & `sphinx-7.1.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_project.py` & `sphinx-7.1.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_pycode.py` & `sphinx-7.1.2/tests/test_pycode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_pycode_ast.py` & `sphinx-7.1.2/tests/test_pycode_ast.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_pycode_parser.py` & `sphinx-7.1.2/tests/test_pycode_parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_quickstart.py` & `sphinx-7.1.2/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_roles.py` & `sphinx-7.1.2/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_search.py` & `sphinx-7.1.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_smartquotes.py` & `sphinx-7.1.2/tests/test_smartquotes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_templating.py` & `sphinx-7.1.2/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_theming.py` & `sphinx-7.1.2/tests/test_theming.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_toctree.py` & `sphinx-7.1.2/tests/test_toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_transforms_post_transforms.py` & `sphinx-7.1.2/tests/test_transforms_post_transforms.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_transforms_post_transforms_code.py` & `sphinx-7.1.2/tests/test_transforms_post_transforms_code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util.py` & `sphinx-7.1.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_display.py` & `sphinx-7.1.2/tests/test_util_display.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_docstrings.py` & `sphinx-7.1.2/tests/test_util_docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_docutils.py` & `sphinx-7.1.2/tests/test_util_docutils.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_fileutil.py` & `sphinx-7.1.2/tests/test_util_fileutil.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_i18n.py` & `sphinx-7.1.2/tests/test_util_i18n.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_images.py` & `sphinx-7.1.2/tests/test_util_images.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_inspect.py` & `sphinx-7.1.2/tests/test_util_inspect.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_inventory.py` & `sphinx-7.1.2/tests/test_util_inventory.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_logging.py` & `sphinx-7.1.2/tests/test_util_logging.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_matching.py` & `sphinx-7.1.2/tests/test_util_matching.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_nodes.py` & `sphinx-7.1.2/tests/test_util_nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_rst.py` & `sphinx-7.1.2/tests/test_util_rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_template.py` & `sphinx-7.1.2/tests/test_util_template.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_util_typing.py` & `sphinx-7.1.2/tests/test_util_typing.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_versioning.py` & `sphinx-7.1.2/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/test_writer_latex.py` & `sphinx-7.1.2/tests/test_writer_latex.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/typing_test_data.py` & `sphinx-7.1.2/tests/typing_test_data.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tests/utils.py` & `sphinx-7.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/tox.ini` & `sphinx-7.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/utils/babel_runner.py` & `sphinx-7.1.2/utils/babel_runner.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/utils/bump_version.py` & `sphinx-7.1.2/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/utils/release-checklist` & `sphinx-7.1.2/utils/release-checklist`

 * *Files identical despite different names*

### Comparing `sphinx-7.1.1/PKG-INFO` & `sphinx-7.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sphinx
-Version: 7.1.1
+Version: 7.1.2
 Summary: Python documentation generator
 Author-email: Georg Brandl <georg@python.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

