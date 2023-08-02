# Comparing `tmp/mkdocs-1.5.1.tar.gz` & `tmp/mkdocs-1.5.2.tar.gz`

## Comparing `mkdocs-1.5.1.tar` & `mkdocs-1.5.2.tar`

### file list

```diff
@@ -1,236 +1,236 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/__init__.py
--rw-r--r--   0        0        0    11907 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/__main__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/exceptions.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/localization.py
--rw-r--r--   0        0        0    22697 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/py.typed
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/theme.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/__init__.py
--rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/build.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/get_deps.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/gh_deploy.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/new.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/commands/serve.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/__init__.py
--rw-r--r--   0        0        0    13151 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/base.py
--rw-r--r--   0        0        0    43679 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/config_options.py
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/config/defaults.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/__init__.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/prebuild-index.js
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/search_index.py
--rw-r--r--   0        0        0    24525 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ar.js
--rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.da.js
--rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.de.js
--rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.du.js
--rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.es.js
--rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fi.js
--rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fr.js
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.hu.js
--rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.it.js
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ja.js
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.jp.js
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.multi.js
--rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.nl.js
--rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.no.js
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.pt.js
--rw-r--r--   0        0        0    23151 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ro.js
--rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ru.js
--rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.sv.js
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.th.js
--rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.tr.js
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.vi.js
--rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/tinyseg.js
--rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/templates/search/lunr.js
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/templates/search/main.js
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/contrib/search/templates/search/worker.js
--rw-r--r--   0        0        0    12954 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/livereload/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/__init__.py
--rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/files.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/nav.py
--rw-r--r--   0        0        0    17689 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/pages.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/structure/toc.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/templates/sitemap.xml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/__init__.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/base.py
--rw-r--r--   0        0        0    34742 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/build_tests.py
--rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/cli_tests.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/get_deps_tests.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/gh_deploy_tests.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration.py
--rw-r--r--   0        0        0    25502 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/livereload_tests.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/localization_tests.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/new_tests.py
--rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/plugin_tests.py
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/search_tests.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/theme_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/__init__.py
--rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/base_tests.py
--rw-r--r--   0        0        0    55357 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/config_options_legacy_tests.py
--rw-r--r--   0        0        0    82647 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/config_options_tests.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/config/config_tests.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/projects.yaml
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/mkdocs.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/custom.html
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/tweak.css
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/documentation/tweak.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/minimal/mkdocs.yml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/minimal/docs/testing.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/mkdocs.yml
--rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/image.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/index.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/metadata.md
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/non-index.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/page-title.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/pageTitle.md
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/image.png
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/index.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub2/index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/mkdocs.yml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/docs/index.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/docs/Übersicht.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/integration/unicode/docs/♪.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/__init__.py
--rw-r--r--   0        0        0    34219 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/file_tests.py
--rw-r--r--   0        0        0    19090 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/nav_tests.py
--rw-r--r--   0        0        0    52573 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/page_tests.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/structure/toc_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/__init__.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/babel_stub_tests.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/templates_tests.py
--rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/tests/utils/utils_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/babel.cfg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/__init__.py
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/base.html
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/content.html
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/keyboard-modal.html
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/main.html
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/messages.pot
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/mkdocs_theme.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/nav-sub.html
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/search-modal.html
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/toc.html
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/css/base.css
--rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/css/font-awesome.min.css
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/img/favicon.ico
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/img/grid.png
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/js/base.js
--rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/js/bootstrap.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/base.html
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/breadcrumbs.html
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/footer.html
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/main.html
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/messages.pot
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/mkdocs_theme.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/nav.html
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/search.html
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/searchbox.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/toc.html
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/versions.html
--rw-r--r--   0        0        0   135539 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme.css
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme_extra.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/img/favicon.ico
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/theme.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/js/theme_extra.js
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    13370 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/babel_stub.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/cache.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/filters.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/meta.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/templates.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 mkdocs-1.5.1/mkdocs/utils/yaml.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.5.1/.gitignore
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.5.1/LICENSE
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 mkdocs-1.5.1/README.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.5.1/hatch_build.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 mkdocs-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mkdocs-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/__init__.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/__main__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/exceptions.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/localization.py
+-rw-r--r--   0        0        0    22697 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/py.typed
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/theme.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/__init__.py
+-rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/build.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/get_deps.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/gh_deploy.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/new.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/serve.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/__init__.py
+-rw-r--r--   0        0        0    13151 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/base.py
+-rw-r--r--   0        0        0    43938 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/config_options.py
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/defaults.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/__init__.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/prebuild-index.js
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/search_index.py
+-rw-r--r--   0        0        0    24525 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ar.js
+-rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.da.js
+-rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.de.js
+-rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.du.js
+-rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.es.js
+-rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fi.js
+-rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fr.js
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.hu.js
+-rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.it.js
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ja.js
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.jp.js
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.multi.js
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.nl.js
+-rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.no.js
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.pt.js
+-rw-r--r--   0        0        0    23151 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ro.js
+-rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ru.js
+-rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.sv.js
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.th.js
+-rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.tr.js
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.vi.js
+-rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/tinyseg.js
+-rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/templates/search/lunr.js
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/templates/search/main.js
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/templates/search/worker.js
+-rw-r--r--   0        0        0    12998 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/livereload/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/__init__.py
+-rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/files.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/nav.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/pages.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/toc.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/templates/sitemap.xml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/__init__.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/base.py
+-rw-r--r--   0        0        0    34742 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/build_tests.py
+-rw-r--r--   0        0        0    25007 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/cli_tests.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/get_deps_tests.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/gh_deploy_tests.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration.py
+-rw-r--r--   0        0        0    25502 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/livereload_tests.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/localization_tests.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/new_tests.py
+-rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/plugin_tests.py
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/search_tests.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/theme_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/__init__.py
+-rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/base_tests.py
+-rw-r--r--   0        0        0    55357 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/config_options_legacy_tests.py
+-rw-r--r--   0        0        0    82667 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/config_options_tests.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/config_tests.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/projects.yaml
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/mkdocs.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/custom.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/tweak.css
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/tweak.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/minimal/mkdocs.yml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/minimal/docs/testing.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/mkdocs.yml
+-rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/image.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/index.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/metadata.md
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/non-index.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/page-title.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/pageTitle.md
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/image.png
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/index.md
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub2/index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/mkdocs.yml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/docs/index.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/docs/Übersicht.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/docs/♪.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/__init__.py
+-rw-r--r--   0        0        0    34219 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/file_tests.py
+-rw-r--r--   0        0        0    19090 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/nav_tests.py
+-rw-r--r--   0        0        0    52573 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/page_tests.py
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/toc_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/babel_stub_tests.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/templates_tests.py
+-rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/utils_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/babel.cfg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/__init__.py
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/base.html
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/content.html
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/keyboard-modal.html
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/main.html
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/messages.pot
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/nav-sub.html
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/search-modal.html
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/toc.html
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/css/base.css
+-rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/css/font-awesome.min.css
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/img/favicon.ico
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/img/grid.png
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/js/base.js
+-rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/js/bootstrap.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/base.html
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/breadcrumbs.html
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/footer.html
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/main.html
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/messages.pot
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/nav.html
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/search.html
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/searchbox.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/toc.html
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/versions.html
+-rw-r--r--   0        0        0   135539 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme.css
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme_extra.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/img/favicon.ico
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/html5shiv.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/theme.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/theme_extra.js
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    13370 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/babel_stub.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/cache.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/filters.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/meta.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/templates.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/yaml.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.5.2/LICENSE
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 mkdocs-1.5.2/README.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.5.2/hatch_build.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 mkdocs-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mkdocs-1.5.2/PKG-INFO
```

### Comparing `mkdocs-1.5.1/mkdocs/__main__.py` & `mkdocs-1.5.2/mkdocs/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,16 +247,16 @@
     """
     MkDocs - Project documentation with Markdown.
     """
 
 
 @cli.command(name="serve")
 @click.option('-a', '--dev-addr', help=dev_addr_help, metavar='<IP:PORT>')
-@click.option('--livereload', 'livereload', flag_value='livereload', default=True, hidden=True)
-@click.option('--no-livereload', 'livereload', flag_value='no-livereload', help=no_reload_help)
+@click.option('--no-livereload', 'livereload', flag_value=False, help=no_reload_help)
+@click.option('--livereload', 'livereload', flag_value=True, default=True, hidden=True)
 @click.option('--dirtyreload', 'build_type', flag_value='dirty', hidden=True)
 @click.option('--dirty', 'build_type', flag_value='dirty', help=serve_dirty_help)
 @click.option('-c', '--clean', 'build_type', flag_value='clean', help=serve_clean_help)
 @click.option('--watch-theme', help=watch_theme_help, is_flag=True)
 @click.option(
     '-w', '--watch', help=watch_help, type=click.Path(exists=True), multiple=True, default=[]
 )
```

### Comparing `mkdocs-1.5.1/mkdocs/exceptions.py` & `mkdocs-1.5.2/mkdocs/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/localization.py` & `mkdocs-1.5.2/mkdocs/localization.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/plugins.py` & `mkdocs-1.5.2/mkdocs/plugins.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/theme.py` & `mkdocs-1.5.2/mkdocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/commands/build.py` & `mkdocs-1.5.2/mkdocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/commands/get_deps.py` & `mkdocs-1.5.2/mkdocs/commands/get_deps.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/commands/gh_deploy.py` & `mkdocs-1.5.2/mkdocs/commands/gh_deploy.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/commands/new.py` & `mkdocs-1.5.2/mkdocs/commands/new.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/commands/serve.py` & `mkdocs-1.5.2/mkdocs/commands/serve.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import functools
 import logging
 import shutil
 import tempfile
 from os.path import isdir, isfile, join
 from typing import TYPE_CHECKING
 from urllib.parse import urlsplit
 
@@ -18,25 +17,21 @@
 if TYPE_CHECKING:
     from mkdocs.config.defaults import MkDocsConfig
 
 log = logging.getLogger(__name__)
 
 
 def serve(
-    config_file=None,
-    dev_addr=None,
-    strict=None,
-    theme=None,
-    theme_dir=None,
-    livereload='livereload',
-    build_type=None,
-    watch_theme=False,
-    watch=[],
+    config_file: str | None = None,
+    livereload: bool = True,
+    build_type: str | None = None,
+    watch_theme: bool = False,
+    watch: list[str] = [],
     **kwargs,
-):
+) -> None:
     """
     Start the MkDocs development server
 
     By default it will serve the documentation on http://localhost:8000/ and
     it will rebuild the documentation and refresh the page automatically
     whenever a file is edited.
     """
@@ -44,42 +39,35 @@
     # PY2 returns a byte string by default. The Unicode prefix ensures a Unicode
     # string is returned. And it makes MkDocs temp dirs easier to identify.
     site_dir = tempfile.mkdtemp(prefix='mkdocs_')
 
     def mount_path(config: MkDocsConfig):
         return urlsplit(config.site_url or '/').path
 
-    get_config = functools.partial(
-        load_config,
-        config_file=config_file,
-        dev_addr=dev_addr,
-        strict=strict,
-        theme=theme,
-        theme_dir=theme_dir,
-        site_dir=site_dir,
-        **kwargs,
-    )
+    def get_config():
+        config = load_config(
+            config_file=config_file,
+            site_dir=site_dir,
+            **kwargs,
+        )
+        config.watch.extend(watch)
+        config.site_url = f'http://{config.dev_addr}{mount_path(config)}'
+        return config
 
     is_clean = build_type == 'clean'
     is_dirty = build_type == 'dirty'
 
     config = get_config()
     config.plugins.on_startup(command=('build' if is_clean else 'serve'), dirty=is_dirty)
 
     def builder(config: MkDocsConfig | None = None):
         log.info("Building documentation...")
         if config is None:
             config = get_config()
 
-        # combine CLI watch arguments with config file values
-        config.watch.extend(watch)
-
-        # Override a few config settings after validation
-        config.site_url = f'http://{config.dev_addr}{mount_path(config)}'
-
         build(config, live_server=None if is_clean else server, dirty=is_dirty)
 
     host, port = config.dev_addr
     server = LiveReloadServer(
         builder=builder, host=host, port=port, root=site_dir, mount_path=mount_path(config)
     )
```

### Comparing `mkdocs-1.5.1/mkdocs/config/base.py` & `mkdocs-1.5.2/mkdocs/config/base.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/config/config_options.py` & `mkdocs-1.5.2/mkdocs/config/config_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -941,19 +941,26 @@
     def __str__(self):
         return self.path
 
     def __fspath__(self):
         return self.path
 
 
-class ExtraScript(SubConfig[ExtraScriptValue]):
-    def run_validation(self, value: object) -> ExtraScriptValue:
+class ExtraScript(BaseConfigOption[Union[ExtraScriptValue, str]]):
+    def __init__(self):
+        super().__init__()
+        self.option_type = SubConfig[ExtraScriptValue]()
+
+    def run_validation(self, value: object) -> ExtraScriptValue | str:
+        self.option_type.warnings = self.warnings
         if isinstance(value, str):
-            value = {'path': value, 'type': 'module' if value.endswith('.mjs') else ''}
-        return super().run_validation(value)
+            if value.endswith('.mjs'):
+                return self.option_type.run_validation({'path': value, 'type': 'module'})
+            return value
+        return self.option_type.run_validation(value)
 
 
 class MarkdownExtensions(OptionallyRequired[List[str]]):
     """
     Markdown Extensions Config Option
 
     A list or dict of extensions. Each list item may contain either a string or a one item dict.
```

### Comparing `mkdocs-1.5.1/mkdocs/config/defaults.py` & `mkdocs-1.5.2/mkdocs/config/defaults.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/__init__.py` & `mkdocs-1.5.2/mkdocs/contrib/search/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/prebuild-index.js` & `mkdocs-1.5.2/mkdocs/contrib/search/prebuild-index.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/search_index.py` & `mkdocs-1.5.2/mkdocs/contrib/search/search_index.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ar.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ar.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.da.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.da.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.de.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.de.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.du.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.du.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.es.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.es.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fi.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.fr.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.hu.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.it.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.it.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ja.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.multi.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.nl.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.no.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.no.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.pt.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ro.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ro.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.ru.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ru.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.sv.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.th.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.th.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.tr.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/lunr.vi.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.vi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/lunr-language/tinyseg.js` & `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/tinyseg.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/templates/search/lunr.js` & `mkdocs-1.5.2/mkdocs/contrib/search/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/templates/search/main.js` & `mkdocs-1.5.2/mkdocs/contrib/search/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/contrib/search/templates/search/worker.js` & `mkdocs-1.5.2/mkdocs/contrib/search/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/livereload/__init__.py` & `mkdocs-1.5.2/mkdocs/livereload/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,18 +151,19 @@
             self._watched_paths.pop(path)
             self.observer.unschedule(self._watch_refs.pop(path))
 
     def serve(self):
         self.server_bind()
         self.server_activate()
 
-        self.observer.start()
+        if self._watched_paths:
+            self.observer.start()
 
-        paths_str = ", ".join(f"'{_try_relativize_path(path)}'" for path in self._watched_paths)
-        log.info(f"Watching paths for changes: {paths_str}")
+            paths_str = ", ".join(f"'{_try_relativize_path(path)}'" for path in self._watched_paths)
+            log.info(f"Watching paths for changes: {paths_str}")
 
         log.info(f"Serving on {self.url}")
         self.serve_thread.start()
 
         self._build_loop()
 
     def _build_loop(self):
```

### Comparing `mkdocs-1.5.1/mkdocs/structure/__init__.py` & `mkdocs-1.5.2/mkdocs/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/structure/files.py` & `mkdocs-1.5.2/mkdocs/structure/files.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/structure/nav.py` & `mkdocs-1.5.2/mkdocs/structure/nav.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/structure/pages.py` & `mkdocs-1.5.2/mkdocs/structure/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
     title: str | None = None
     postprocessors: Sequence[markdown.postprocessors.Postprocessor] = ()
 
     def run(self, root: etree.Element) -> etree.Element:
         for el in root:
             if el.tag == 'h1':
                 # Drop anchorlink from the element, if present.
-                if len(el) > 0 and el[-1].tag == 'a' and not (el.tail or '').strip():
+                if len(el) > 0 and el[-1].tag == 'a' and not (el[-1].tail or '').strip():
                     el = copy.copy(el)
                     del el[-1]
                 # Extract the text only, recursively.
                 title = ''.join(el.itertext())
                 # Unescape per Markdown implementation details.
                 for pp in self.postprocessors:
                     title = pp.run(title)
```

### Comparing `mkdocs-1.5.1/mkdocs/structure/toc.py` & `mkdocs-1.5.2/mkdocs/structure/toc.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/templates/sitemap.xml` & `mkdocs-1.5.2/mkdocs/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/base.py` & `mkdocs-1.5.2/mkdocs/tests/base.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/build_tests.py` & `mkdocs-1.5.2/mkdocs/tests/build_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/cli_tests.py` & `mkdocs-1.5.2/mkdocs/tests/cli_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     @mock.patch('mkdocs.commands.serve.serve', autospec=True)
     def test_serve_default(self, mock_serve):
         result = self.runner.invoke(cli.cli, ["serve"], catch_exceptions=False)
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=None,
             watch_theme=False,
             watch=(),
@@ -49,15 +49,15 @@
         result = self.runner.invoke(
             cli.cli, ["serve", '--dev-addr', '0.0.0.0:80'], catch_exceptions=False
         )
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr='0.0.0.0:80',
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=None,
             watch_theme=False,
             watch=(),
@@ -66,15 +66,15 @@
     @mock.patch('mkdocs.commands.serve.serve', autospec=True)
     def test_serve_strict(self, mock_serve):
         result = self.runner.invoke(cli.cli, ["serve", '--strict'], catch_exceptions=False)
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=True,
             theme=None,
             use_directory_urls=None,
             watch_theme=False,
             watch=(),
@@ -85,15 +85,15 @@
         result = self.runner.invoke(
             cli.cli, ["serve", '--theme', 'readthedocs'], catch_exceptions=False
         )
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=None,
             theme='readthedocs',
             use_directory_urls=None,
             watch_theme=False,
             watch=(),
@@ -104,15 +104,15 @@
         result = self.runner.invoke(
             cli.cli, ["serve", '--use-directory-urls'], catch_exceptions=False
         )
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=True,
             watch_theme=False,
             watch=(),
@@ -123,15 +123,15 @@
         result = self.runner.invoke(
             cli.cli, ["serve", '--no-directory-urls'], catch_exceptions=False
         )
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=False,
             watch_theme=False,
             watch=(),
@@ -140,15 +140,15 @@
     @mock.patch('mkdocs.commands.serve.serve', autospec=True)
     def test_serve_livereload(self, mock_serve):
         result = self.runner.invoke(cli.cli, ["serve", '--livereload'], catch_exceptions=False)
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=None,
             watch_theme=False,
             watch=(),
@@ -157,15 +157,15 @@
     @mock.patch('mkdocs.commands.serve.serve', autospec=True)
     def test_serve_no_livereload(self, mock_serve):
         result = self.runner.invoke(cli.cli, ["serve", '--no-livereload'], catch_exceptions=False)
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='no-livereload',
+            livereload=False,
             build_type=None,
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=None,
             watch_theme=False,
             watch=(),
@@ -174,15 +174,15 @@
     @mock.patch('mkdocs.commands.serve.serve', autospec=True)
     def test_serve_dirtyreload(self, mock_serve):
         result = self.runner.invoke(cli.cli, ["serve", '--dirty'], catch_exceptions=False)
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type='dirty',
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=None,
             watch_theme=False,
             watch=(),
@@ -191,15 +191,15 @@
     @mock.patch('mkdocs.commands.serve.serve', autospec=True)
     def test_serve_watch_theme(self, mock_serve):
         result = self.runner.invoke(cli.cli, ["serve", '--watch-theme'], catch_exceptions=False)
 
         self.assertEqual(result.exit_code, 0)
         mock_serve.assert_called_once_with(
             dev_addr=None,
-            livereload='livereload',
+            livereload=True,
             build_type=None,
             config_file=None,
             strict=None,
             theme=None,
             use_directory_urls=None,
             watch_theme=True,
             watch=(),
```

### Comparing `mkdocs-1.5.1/mkdocs/tests/get_deps_tests.py` & `mkdocs-1.5.2/mkdocs/tests/get_deps_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/gh_deploy_tests.py` & `mkdocs-1.5.2/mkdocs/tests/gh_deploy_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/integration.py` & `mkdocs-1.5.2/mkdocs/tests/integration.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/livereload_tests.py` & `mkdocs-1.5.2/mkdocs/tests/livereload_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/localization_tests.py` & `mkdocs-1.5.2/mkdocs/tests/localization_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/new_tests.py` & `mkdocs-1.5.2/mkdocs/tests/new_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/plugin_tests.py` & `mkdocs-1.5.2/mkdocs/tests/plugin_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/search_tests.py` & `mkdocs-1.5.2/mkdocs/tests/search_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/theme_tests.py` & `mkdocs-1.5.2/mkdocs/tests/theme_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/config/base_tests.py` & `mkdocs-1.5.2/mkdocs/tests/config/base_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/config/config_options_legacy_tests.py` & `mkdocs-1.5.2/mkdocs/tests/config/config_options_legacy_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/config/config_options_tests.py` & `mkdocs-1.5.2/mkdocs/tests/config/config_options_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import logging
 import os
 import re
 import sys
 import textwrap
 import unittest
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, TypeVar, Union
 from unittest.mock import patch
 
 if TYPE_CHECKING:
     from typing_extensions import assert_type
 else:
 
     def assert_type(val, typ):
@@ -696,40 +696,40 @@
 
 class ExtraScriptsTest(TestCase):
     def test_js_async(self) -> None:
         class Schema(Config):
             option = c.ListOfItems(c.ExtraScript(), default=[])
 
         conf = self.get_config(Schema, {'option': ['foo.js', {'path': 'bar.js', 'async': True}]})
-        assert_type(conf.option, List[c.ExtraScriptValue])
+        assert_type(conf.option, List[Union[c.ExtraScriptValue, str]])
         self.assertEqual(len(conf.option), 2)
-        self.assertIsInstance(conf.option[0], c.ExtraScriptValue)
+        self.assertIsInstance(conf.option[1], c.ExtraScriptValue)
         self.assertEqual(
-            [(x.path, x.type, x.defer, x.async_) for x in conf.option],
+            conf.option,
             [
-                ('foo.js', '', False, False),
-                ('bar.js', '', False, True),
+                'foo.js',
+                {'path': 'bar.js', 'type': '', 'defer': False, 'async': True},
             ],
         )
 
     def test_mjs(self) -> None:
         class Schema(Config):
             option = c.ListOfItems(c.ExtraScript(), default=[])
 
         conf = self.get_config(
             Schema, {'option': ['foo.mjs', {'path': 'bar.js', 'type': 'module'}]}
         )
-        assert_type(conf.option, List[c.ExtraScriptValue])
+        assert_type(conf.option, List[Union[c.ExtraScriptValue, str]])
         self.assertEqual(len(conf.option), 2)
         self.assertIsInstance(conf.option[0], c.ExtraScriptValue)
         self.assertEqual(
-            [(x.path, x.type, x.defer, x.async_) for x in conf.option],
+            conf.option,
             [
-                ('foo.mjs', 'module', False, False),
-                ('bar.js', 'module', False, False),
+                {'path': 'foo.mjs', 'type': 'module', 'defer': False, 'async': False},
+                {'path': 'bar.js', 'type': 'module', 'defer': False, 'async': False},
             ],
         )
 
     def test_wrong_type(self) -> None:
         class Schema(Config):
             option = c.ListOfItems(c.ExtraScript(), default=[])
 
@@ -744,16 +744,16 @@
 
         conf = self.get_config(
             Schema,
             {'option': [{'path': 'foo.js', 'foo': 'bar'}]},
             warnings=dict(option="Sub-option 'foo': Unrecognised configuration name: foo"),
         )
         self.assertEqual(
-            [(x.path, x.type, x.defer, x.async_) for x in conf.option],
-            [('foo.js', '', False, False)],
+            conf.option,
+            [{'path': 'foo.js', 'type': '', 'defer': False, 'async': False, 'foo': 'bar'}],
         )
 
 
 class DictOfItemsTest(TestCase):
     def test_int_type(self) -> None:
         class Schema(Config):
             option = c.DictOfItems(c.Type(int))
```

### Comparing `mkdocs-1.5.1/mkdocs/tests/config/config_tests.py` & `mkdocs-1.5.2/mkdocs/tests/config/config_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/integration/projects.yaml` & `mkdocs-1.5.2/mkdocs/tests/integration/projects.yaml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/integration/complicated_config/mkdocs.yml` & `mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/image.png` & `mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/integration/subpages/docs/sub1/image.png` & `mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/structure/file_tests.py` & `mkdocs-1.5.2/mkdocs/tests/structure/file_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/structure/nav_tests.py` & `mkdocs-1.5.2/mkdocs/tests/structure/nav_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/structure/page_tests.py` & `mkdocs-1.5.2/mkdocs/tests/structure/page_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/structure/toc_tests.py` & `mkdocs-1.5.2/mkdocs/tests/structure/toc_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/utils/babel_stub_tests.py` & `mkdocs-1.5.2/mkdocs/tests/utils/babel_stub_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/utils/templates_tests.py` & `mkdocs-1.5.2/mkdocs/tests/utils/templates_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/tests/utils/utils_tests.py` & `mkdocs-1.5.2/mkdocs/tests/utils/utils_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/base.html` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/keyboard-modal.html` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/keyboard-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/messages.pot` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/search-modal.html` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/search-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/toc.html` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/toc.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/css/base.css` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/css/base.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/css/bootstrap.min.css` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/css/font-awesome.min.css` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/img/favicon.ico` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/img/grid.png` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/img/grid.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/js/base.js` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/js/base.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/js/bootstrap.min.js` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/base.html` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/breadcrumbs.html` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/footer.html` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/messages.pot` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/nav.html` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/search.html` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/versions.html` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/versions.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme.css` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/theme_extra.css` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/img/favicon.ico` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/js/html5shiv.min.js` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/js/theme.js` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/utils/__init__.py` & `mkdocs-1.5.2/mkdocs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/utils/babel_stub.py` & `mkdocs-1.5.2/mkdocs/utils/babel_stub.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/utils/cache.py` & `mkdocs-1.5.2/mkdocs/utils/cache.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/utils/meta.py` & `mkdocs-1.5.2/mkdocs/utils/meta.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/utils/templates.py` & `mkdocs-1.5.2/mkdocs/utils/templates.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/mkdocs/utils/yaml.py` & `mkdocs-1.5.2/mkdocs/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/.gitignore` & `mkdocs-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/LICENSE` & `mkdocs-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/README.md` & `mkdocs-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/pyproject.toml` & `mkdocs-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.1/PKG-INFO` & `mkdocs-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs
-Version: 1.5.1
+Version: 1.5.2
 Summary: Project documentation with Markdown.
 Project-URL: Documentation, https://www.mkdocs.org/
 Project-URL: Source, https://github.com/mkdocs/mkdocs
 Project-URL: Issues, https://github.com/mkdocs/mkdocs/issues
 Project-URL: History, https://www.mkdocs.org/about/release-notes/
 Author-email: Tom Christie <tom@tomchristie.com>
 License-Expression: BSD-2-Clause
```

