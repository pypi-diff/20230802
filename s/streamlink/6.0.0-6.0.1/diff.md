# Comparing `tmp/streamlink-6.0.0.tar.gz` & `tmp/streamlink-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-6.0.0.tar", last modified: Thu Jul 20 12:43:24 2023, max compression
+gzip compressed data, was "streamlink-6.0.1.tar", last modified: Wed Aug  2 13:55:50 2023, max compression
```

## Comparing `streamlink-6.0.0.tar` & `streamlink-6.0.1.tar`

### file list

```diff
@@ -1,627 +1,627 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.782695 streamlink-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 12:42:25.000000 streamlink-6.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-07-20 12:42:25.000000 streamlink-6.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-20 12:42:25.000000 streamlink-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 12:42:25.000000 streamlink-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-20 12:43:24.778695 streamlink-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-20 12:42:25.000000 streamlink-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.666692 streamlink-6.0.0/completions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.674692 streamlink-6.0.0/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-20 12:43:08.000000 streamlink-6.0.0/completions/bash/streamlink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.674692 streamlink-6.0.0/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)    34901 2023-07-20 12:43:09.000000 streamlink-6.0.0/completions/zsh/_streamlink
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 12:42:25.000000 streamlink-6.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_applications.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.666692 streamlink-6.0.0/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (123)    39501 2023-07-20 12:43:15.000000 streamlink-6.0.0/docs/_build/man/streamlink.1
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_man.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/icon-ffmpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/icon-python.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/opengraph-image.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/sidebar/github-buttons.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/options.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/session.rst
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/streamlink.rst
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/webbrowser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/applications.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugin-sideloading.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/docs/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugins/crunchyroll.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugins/twitch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/donate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_html_template_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_releaseref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/migrations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/players.rst
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/thirdparty.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-20 12:42:25.000000 streamlink-6.0.0/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-20 12:42:25.000000 streamlink-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:43:24.782695 streamlink-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-20 12:42:25.000000 streamlink-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.670692 streamlink-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.782695 streamlink-6.0.0/src/streamlink/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 12:43:24.782695 streamlink-6.0.0/src/streamlink/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/packages/requests_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink/plugin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/useragents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.686693 streamlink-6.0.0/src/streamlink/plugin/api/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.718693 streamlink-6.0.0/src/streamlink/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/app17.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/btv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/htv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/qq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/streann.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/stv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    33839 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/welt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zhanqi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.722693 streamlink-6.0.0/src/streamlink/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    34111 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/dash_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20613 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/segmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.726693 streamlink-6.0.0/src/streamlink/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.726693 streamlink-6.0.0/src/streamlink/webbrowser/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.726693 streamlink-6.0.0/src/streamlink/webbrowser/cdp/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19550 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.730693 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    49431 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/dom.py
--rw-r--r--   0 runner    (1001) docker     (123)    26108 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    27656 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/input_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/io.py
--rw-r--r--   0 runner    (1001) docker     (123)   130730 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/network.py
--rw-r--r--   0 runner    (1001) docker     (123)   107545 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    62134 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/chromium.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/webbrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.730693 streamlink-6.0.0/src/streamlink_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47629 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31600 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.730693 streamlink-6.0.0/src/streamlink_cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.734694 streamlink-6.0.0/src/streamlink_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/player.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.734694 streamlink-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/output/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/output/test_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_cmdline_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_main_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_main_setup_config_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_plugin_args_and_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_player.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_versioncheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/mixins/stream_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.742694 streamlink-6.0.0/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.742694 streamlink-6.0.0/tests/plugin/override/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/override/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/testplugin_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/testplugin_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_app17.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_btv.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_htv.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_huya.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nos.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_qq.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_streann.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_stv.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    34427 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_welt.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zhanqi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.670692 streamlink-6.0.0/tests/resources/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/resources/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/custom
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/primary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/primary.testplugin
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/secondary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/secondary.testplugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/resources/dash/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_10.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_11_static.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_3.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_8.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_9.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_nested_baseurls.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_no_segment_list_or_template.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_segment_list.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_segments_byterange.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_segments_dynamic_number.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_static_no_publish_time.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_timeline_ids.mpd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.774695 streamlink-6.0.0/tests/resources/hls/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_1.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_2.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_date.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_master.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_master_twitch_vod.m3u8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.774695 streamlink-6.0.0/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_dash_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    39039 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_hls_filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_stream_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_stream_to_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_api_http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    48165 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_api_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16043 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_plugin_userinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23565 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_streamlink_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.774695 streamlink-6.0.0/tests/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/testutils/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/testutils/test_handshake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.778695 streamlink-6.0.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.778695 streamlink-6.0.0/tests/webbrowser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.778695 streamlink-6.0.0/tests/webbrowser/cdp/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    39456 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/test_chromium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/test_webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.783730 streamlink-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-02 13:54:43.000000 streamlink-6.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    82098 2023-08-02 13:54:43.000000 streamlink-6.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-02 13:54:43.000000 streamlink-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-02 13:54:43.000000 streamlink-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-02 13:55:50.783730 streamlink-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-02 13:54:43.000000 streamlink-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.667729 streamlink-6.0.1/completions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.675729 streamlink-6.0.1/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-08-02 13:55:32.000000 streamlink-6.0.1/completions/bash/streamlink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.675729 streamlink-6.0.1/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)    34866 2023-08-02 13:55:33.000000 streamlink-6.0.1/completions/zsh/_streamlink
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-02 13:54:43.000000 streamlink-6.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.679729 streamlink-6.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_applications.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.667729 streamlink-6.0.1/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.679729 streamlink-6.0.1/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    39501 2023-08-02 13:55:40.000000 streamlink-6.0.1/docs/_build/man/streamlink.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_man.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.679729 streamlink-6.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/icon-ffmpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/icon-python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/opengraph-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.679729 streamlink-6.0.1/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.679729 streamlink-6.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.679729 streamlink-6.0.1/docs/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_templates/sidebar/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/_templates/sidebar/github-buttons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.679729 streamlink-6.0.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api/options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api/plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api/session.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api/streamlink.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api/webbrowser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/api_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/applications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    82098 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.683729 streamlink-6.0.1/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/plugin-sideloading.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.683729 streamlink-6.0.1/docs/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/plugins/crunchyroll.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/plugins/twitch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/donate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/ext_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/ext_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/ext_html_template_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/ext_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/ext_releaseref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/players.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs/thirdparty.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 13:54:43.000000 streamlink-6.0.1/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-08-02 13:54:43.000000 streamlink-6.0.1/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-08-02 13:54:43.000000 streamlink-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:55:50.783730 streamlink-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-02 13:54:43.000000 streamlink-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.671729 streamlink-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.787730 streamlink-6.0.1/src/streamlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-02 13:55:50.787730 streamlink-6.0.1/src/streamlink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.683729 streamlink-6.0.1/src/streamlink/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/packages/requests_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.687729 streamlink-6.0.1/src/streamlink/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.687729 streamlink-6.0.1/src/streamlink/plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/useragents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.687729 streamlink-6.0.1/src/streamlink/plugin/api/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/validate/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/validate/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/validate/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/validate/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/api/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.715729 streamlink-6.0.1/src/streamlink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33839 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/plugins/zhanqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.723729 streamlink-6.0.1/src/streamlink/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34165 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/dash_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20613 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/stream/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.727729 streamlink-6.0.1/src/streamlink/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.727729 streamlink-6.0.1/src/streamlink/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.727729 streamlink-6.0.1/src/streamlink/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19550 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.731730 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49431 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/dom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26108 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27656 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/input_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130730 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107545 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62134 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/cdp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/chromium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink/webbrowser/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.683729 streamlink-6.0.1/src/streamlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-02 13:55:50.000000 streamlink-6.0.1/src/streamlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-08-02 13:55:50.000000 streamlink-6.0.1/src/streamlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:55:50.000000 streamlink-6.0.1/src/streamlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 13:55:50.000000 streamlink-6.0.1/src/streamlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-02 13:55:50.000000 streamlink-6.0.1/src/streamlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 13:55:50.000000 streamlink-6.0.1/src/streamlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.731730 streamlink-6.0.1/src/streamlink_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47629 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31600 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.731730 streamlink-6.0.1/src/streamlink_cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/output/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/output/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/output/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/output/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.735730 streamlink-6.0.1/src/streamlink_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/utils/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-02 13:54:43.000000 streamlink-6.0.1/src/streamlink_cli/utils/versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.735730 streamlink-6.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.739730 streamlink-6.0.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.739730 streamlink-6.0.1/tests/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/output/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/output/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_cmdline_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_main_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_main_setup_config_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_plugin_args_and_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/test_streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.739730 streamlink-6.0.1/tests/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/utils/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/cli/utils/test_versioncheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.739730 streamlink-6.0.1/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/mixins/stream_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.739730 streamlink-6.0.1/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.739730 streamlink-6.0.1/tests/plugin/override/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugin/override/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugin/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugin/testplugin_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugin/testplugin_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.767730 streamlink-6.0.1/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34427 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/plugins/test_zhanqi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.767730 streamlink-6.0.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.671729 streamlink-6.0.1/tests/resources/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.771730 streamlink-6.0.1/tests/resources/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/cli/config/custom
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/cli/config/primary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/cli/config/primary.testplugin
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/cli/config/secondary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/cli/config/secondary.testplugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.775730 streamlink-6.0.1/tests/resources/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_10.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_11_static.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_3.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_8.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_9.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_nested_baseurls.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_no_segment_list_or_template.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_segment_list.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_segments_byterange.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_segments_dynamic_number.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_static_no_publish_time.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/dash/test_timeline_ids.mpd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.775730 streamlink-6.0.1/tests/resources/hls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/hls/test_1.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/hls/test_2.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/hls/test_date.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/hls/test_master.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/resources/hls/test_master_twitch_vod.m3u8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.779730 streamlink-6.0.1/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_dash_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39039 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_hls_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_stream_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_stream_to_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/stream/test_stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_api_http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48166 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_api_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16043 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_plugin_userinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23961 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/test_streamlink_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.779730 streamlink-6.0.1/tests/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/testutils/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/testutils/test_handshake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.783730 streamlink-6.0.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.783730 streamlink-6.0.1/tests/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:55:50.783730 streamlink-6.0.1/tests/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/cdp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39456 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/cdp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/cdp/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/test_chromium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-08-02 13:54:43.000000 streamlink-6.0.1/tests/webbrowser/test_webbrowser.py
```

### Comparing `streamlink-6.0.0/CHANGELOG.md` & `streamlink-6.0.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Changelog
 
+## streamlink 6.0.1 (2023-08-02)
+
+Patch release:
+
+- Added: missing `options` argument to `Streamlink.streams()` ([#5469](https://github.com/streamlink/streamlink/pull/5469))
+- Fixed: migration docs and the [`6.0.0` changelog](https://streamlink.github.io/changelog.html#streamlink-6-0-0-2023-07-20) of the [`Streamlink.{g,s}et_plugin_option()` removal](https://streamlink.github.io/migrations.html#streamlink-g-s-et-plugin-option) ([#5471](https://github.com/streamlink/streamlink/pull/5471))
+- Fixed plugins: huya ([#5467](https://github.com/streamlink/streamlink/pull/5467))
+- Docs: updated build-dependencies and the furo theme ([#5464](https://github.com/streamlink/streamlink/pull/5464), [#5465](https://github.com/streamlink/streamlink/pull/5465))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/6.0.0...6.0.1)
+
+
 ## streamlink 6.0.0 (2023-07-20)
 
 Breaking changes:
 
 - BREAKING: dropped support for Python 3.7 ([#5302](https://github.com/streamlink/streamlink/pull/5302))
 - BREAKING: [turned `--player` CLI argument into a player-path-only argument](https://streamlink.github.io/migrations.html#player-path-only-player-cli-argument) ([#5305](https://github.com/streamlink/streamlink/issues/5305), [#5310](https://github.com/streamlink/streamlink/pull/5310))  
   Its value won't be interpreted as a command line string anymore, so paths with whitespace don't require additional quotation. Custom player arguments now always need to be set via `--player-args`.
 - BREAKING: [removed deprecated `{filename}` variable from `--player-args`](https://streamlink.github.io/migrations.html#filename-variable-in-player-args) ([#5310](https://github.com/streamlink/streamlink/pull/5310))
 - BREAKING/API: [removed support for the deprecated `Plugin.can_handle_url()` / `Plugin.priority()` classmethods](https://streamlink.github.io/migrations.html#plugin-can-handle-url-and-plugin-priority) ([#5403](https://github.com/streamlink/streamlink/pull/5403))
 - BREAKING/API: [removed deprecated compatibility wrapper for the `Plugin` constructor](https://streamlink.github.io/migrations.html#plugin-init-self-url-compatibility-wrapper) ([#5402](https://github.com/streamlink/streamlink/pull/5402))
+- BREAKING/API: [removed `Streamlink.{g,s}et_plugin_option()`](https://streamlink.github.io/migrations.html#streamlink-g-s-et-plugin-option) ([#5033](https://github.com/streamlink/streamlink/pull/5033))
 - BREAKING/API: [removed deprecated global plugin arguments](https://streamlink.github.io/migrations.html#global-plugin-arguments) ([#5033](https://github.com/streamlink/streamlink/pull/5033))
 - BREAKING/API: [removed deprecated `streamlink.plugin.api.validate.text`](https://streamlink.github.io/migrations.html#plugin-api-validate-text) ([#5404](https://github.com/streamlink/streamlink/pull/5404))
 - BREAKING/API: [fixed/changed signatures of `HTTPStream`, `HLSStream` and `HLSStream.parse_variant_playlist()`](https://streamlink.github.io/migrations.html#httpstream-and-hlsstream-signature-changes) ([#5429](https://github.com/streamlink/streamlink/pull/5429))
 - BREAKING/packaging: new signing key [`44448A298D5C3618`](https://keyserver.ubuntu.com/pks/lookup?search=44448A298D5C3618&fingerprint=on&op=index) ([#5449](https://github.com/streamlink/streamlink/pull/5449))
 
 Release highlights:
```

### Comparing `streamlink-6.0.0/LICENSE` & `streamlink-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/PKG-INFO` & `streamlink-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 6.0.0
+Version: 6.0.1
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 6.0.0 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.0.1 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Author: Streamlink Author-email:
 streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
 //github.com/streamlink/streamlink Project-URL: Documentation, https://
 streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
 streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
```

### Comparing `streamlink-6.0.0/README.md` & `streamlink-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/completions/bash/streamlink` & `streamlink-6.0.1/completions/bash/streamlink`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 _shtab_replace_nonword() {
   echo "${1//[^[:word:]]/_}"
 }
 
 # set default values (called for the initial parser & any subparsers)
 _set_parser_defaults() {
   local subparsers_var="${prefix}_subparsers[@]"
-  sub_parsers=${!subparsers_var}
+  sub_parsers=${!subparsers_var-}
 
   local current_option_strings_var="${prefix}_option_strings[@]"
   current_option_strings=${!current_option_strings_var}
 
   completed_positional_actions=0
 
   _set_new_action "pos_${completed_positional_actions}" true
@@ -98,21 +98,21 @@
 # $1=action identifier
 # $2=positional action (bool)
 # set all identifiers for an action's parameters
 _set_new_action() {
   current_action="${prefix}_$(_shtab_replace_nonword $1)"
 
   local current_action_compgen_var=${current_action}_COMPGEN
-  current_action_compgen="${!current_action_compgen_var}"
+  current_action_compgen="${!current_action_compgen_var-}"
 
   local current_action_choices_var="${current_action}_choices[@]"
-  current_action_choices="${!current_action_choices_var}"
+  current_action_choices="${!current_action_choices_var-}"
 
   local current_action_nargs_var="${current_action}_nargs"
-  if [ -n "${!current_action_nargs_var}" ]; then
+  if [ -n "${!current_action_nargs_var-}" ]; then
     current_action_nargs="${!current_action_nargs_var}"
   else
     current_action_nargs=1
   fi
 
   current_action_args_start_index=$(( $word_index + 1 ))
 
@@ -126,31 +126,31 @@
 #     hello="world"
 #     x="hello"
 #     ${!x} -> ${hello} -> "world"
 _shtab_streamlink_cli() {
   local completing_word="${COMP_WORDS[COMP_CWORD]}"
   COMPREPLY=()
 
-  prefix=_shtab_streamlink_cli
-  word_index=0
+  local prefix=_shtab_streamlink_cli
+  local word_index=0
   _set_parser_defaults
   word_index=1
 
   # determine what arguments are appropriate for the current state
   # of the arg parser
   while [ $word_index -ne $COMP_CWORD ]; do
     local this_word="${COMP_WORDS[$word_index]}"
 
-    if [[ -n $sub_parsers && " ${sub_parsers[@]} " =~ " ${this_word} " ]]; then
+    if [[ -n $sub_parsers && " ${sub_parsers[@]} " == *" ${this_word} "* ]]; then
       # valid subcommand: add it to the prefix & reset the current action
       prefix="${prefix}_$(_shtab_replace_nonword $this_word)"
       _set_parser_defaults
     fi
 
-    if [[ " ${current_option_strings[@]} " =~ " ${this_word} " ]]; then
+    if [[ " ${current_option_strings[@]} " == *" ${this_word} "* ]]; then
       # a new action should be acquired (due to recognised option string or
       # no more input expected from current action);
       # the next positional action can fill in here
       _set_new_action $this_word false
     fi
 
     if [[ "$current_action_nargs" != "*" ]] && \
```

### Comparing `streamlink-6.0.0/completions/zsh/_streamlink` & `streamlink-6.0.1/completions/zsh/_streamlink`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         User prompts and download progress won\'t be written to \`FILE\`.
 
         A value of \`-\` (dash) will set the file name to an ISO8601-like string
         and will choose the following default log directories.
 
         Windows\:
 
-          \%\%TEMP\%\%\\streamlink\\logs
+          \%TEMP\%\\streamlink\\logs
 
         macOS\:
 
           \$\{HOME\}\/Library\/Logs\/streamlink
 
         Linux\/BSD\:
 
@@ -138,15 +138,15 @@
 
         \`\{playertitleargs\}\`
             The automatically generated player title arguments, if a supported player was found. See --title for more.
             If unset, automatically generated player title arguments will be prepended to the parsed player arguments list.
 
         Example\:
 
-          \%(prog)s -p vlc -a \"--play-and-exit --no-one-instance\" \<url\> \[stream\]
+          streamlink -p vlc -a \"--play-and-exit --no-one-instance\" \<url\> \[stream\]
 
         Default is \"\".
         ]:player_args:"
   {-v,--verbose-player}"[
         Allow the player to display its console output.
         ]"
   {-n,--player-fifo,--fifo}"[
@@ -236,15 +236,15 @@
             in front of the dollar sign which VLC uses as its formatting character.
 
             For example, to put the current date in your VLC window title,
             the string \`\\\$A\` could be inserted inside the --title string.
 
         Example\:
 
-            \%(prog)s -p mpv --title \"\{author\} - \{category\} - \{title\}\" \<URL\> \[STREAM\]
+            streamlink -p mpv --title \"\{author\} - \{category\} - \{title\}\" \<URL\> \[STREAM\]
         ]:title:"
   {-o,--output}"[
         Write stream data to \`FILENAME\` instead of playing it. If \`FILENAME\` is set to \`-\` (dash), then the stream data will be
         written to stdout, similar to the --stdout argument.
 
         Non-existent directories and subdirectories will be created if they do not exist, if filesystem permissions allow.
 
@@ -252,15 +252,15 @@
 
         Please see the \"Metadata variables\" section of Streamlink\'s CLI documentation for all available metadata variables.
 
         Unsupported characters in substituted variables will be replaced with an underscore.
 
         Example\:
 
-            \%(prog)s --output \"\~\/recordings\/\{author\}\/\{category\}\/\{id\}-\{time\:\%\%Y\%\%m\%\%d\%\%H\%\%M\%\%S\}.ts\" \<URL\> \[STREAM\]
+            streamlink --output \"\~\/recordings\/\{author\}\/\{category\}\/\{id\}-\{time\:\%Y\%m\%d\%H\%M\%S\}.ts\" \<URL\> \[STREAM\]
         ]:output:"
   {-O,--stdout}"[
         Write stream data to stdout instead of playing it.
         ]"
   {-r,--record}"[
         Open the stream in the player, while at the same time writing it to \`FILENAME\`. If \`FILENAME\` is set to \`-\` (dash),
         then the stream data will be written to stdout, similar to the --stdout argument, while still opening the player.
@@ -271,30 +271,30 @@
 
         Please see the \"Metadata variables\" section of Streamlink\'s CLI documentation for all available metadata variables.
 
         Unsupported characters in substituted variables will be replaced with an underscore.
 
         Example\:
 
-            \%(prog)s --record \"\~\/recordings\/\{author\}\/\{category\}\/\{id\}-\{time\:\%\%Y\%\%m\%\%d\%\%H\%\%M\%\%S\}.ts\" \<URL\> \[STREAM\]
+            streamlink --record \"\~\/recordings\/\{author\}\/\{category\}\/\{id\}-\{time\:\%Y\%m\%d\%H\%M\%S\}.ts\" \<URL\> \[STREAM\]
         ]:record:"
   {-R,--record-and-pipe}"[
         Write stream data to stdout, while at the same time writing it to \`FILENAME\`.
 
         Non-existent directories and subdirectories will be created if they do not exist, if filesystem permissions allow.
 
         You will be prompted if the file already exists.
 
         Please see the \"Metadata variables\" section of Streamlink\'s CLI documentation for all available metadata variables.
 
         Unsupported characters in substituted variables will be replaced with an underscore.
 
         Example\:
 
-            \%(prog)s --record-and-pipe \"\~\/recordings\/\{author\}\/\{category\}\/\{id\}-\{time\:\%\%Y\%\%m\%\%d\%\%H\%\%M\%\%S\}.ts\" \<URL\> \[STREAM\]
+            streamlink --record-and-pipe \"\~\/recordings\/\{author\}\/\{category\}\/\{id\}-\{time\:\%Y\%m\%d\%H\%M\%S\}.ts\" \<URL\> \[STREAM\]
         ]:record_and_pipe:"
   "--fs-safe-rules[
         The rules used to make formatting variables filesystem-safe are chosen
         automatically according to the type of system in use. This overrides
         the automatic detection.
 
         Intended for use when Streamlink is running on a UNIX-like OS but writing
```

### Comparing `streamlink-6.0.0/docs/Makefile` & `streamlink-6.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_build/man/streamlink.1` & `streamlink-6.0.1/docs/_build/man/streamlink.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "STREAMLINK" "1" "Jul 20, 2023" "6.0.0" "Streamlink"
+.TH "STREAMLINK" "1" "Aug 02, 2023" "6.0.1" "Streamlink"
 .SH NAME
 streamlink \- extracts streams from various services and pipes them into a video player of choice
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
```

### Comparing `streamlink-6.0.0/docs/_man.rst` & `streamlink-6.0.1/docs/_man.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/apple-touch-icon.png` & `streamlink-6.0.1/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/favicon-16x16.png` & `streamlink-6.0.1/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/favicon-32x32.png` & `streamlink-6.0.1/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/favicon.ico` & `streamlink-6.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/icon-ffmpeg.svg` & `streamlink-6.0.1/docs/_static/icon-ffmpeg.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/icon-python.svg` & `streamlink-6.0.1/docs/_static/icon-python.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/icon.svg` & `streamlink-6.0.1/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/opengraph-image.png` & `streamlink-6.0.1/docs/_static/opengraph-image.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_static/styles/custom.css` & `streamlink-6.0.1/docs/_static/styles/custom.css`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_templates/base.html` & `streamlink-6.0.1/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_templates/sidebar/brand.html` & `streamlink-6.0.1/docs/_templates/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/_templates/sidebar/github-buttons.html` & `streamlink-6.0.1/docs/_templates/sidebar/github-buttons.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/api/webbrowser.rst` & `streamlink-6.0.1/docs/api/webbrowser.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/api_guide.rst` & `streamlink-6.0.1/docs/api_guide.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/applications.rst` & `streamlink-6.0.1/docs/applications.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/changelog.md` & `streamlink-6.0.1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Changelog
 
+## streamlink 6.0.1 (2023-08-02)
+
+Patch release:
+
+- Added: missing `options` argument to `Streamlink.streams()` ([#5469](https://github.com/streamlink/streamlink/pull/5469))
+- Fixed: migration docs and the [`6.0.0` changelog](https://streamlink.github.io/changelog.html#streamlink-6-0-0-2023-07-20) of the [`Streamlink.{g,s}et_plugin_option()` removal](https://streamlink.github.io/migrations.html#streamlink-g-s-et-plugin-option) ([#5471](https://github.com/streamlink/streamlink/pull/5471))
+- Fixed plugins: huya ([#5467](https://github.com/streamlink/streamlink/pull/5467))
+- Docs: updated build-dependencies and the furo theme ([#5464](https://github.com/streamlink/streamlink/pull/5464), [#5465](https://github.com/streamlink/streamlink/pull/5465))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/6.0.0...6.0.1)
+
+
 ## streamlink 6.0.0 (2023-07-20)
 
 Breaking changes:
 
 - BREAKING: dropped support for Python 3.7 ([#5302](https://github.com/streamlink/streamlink/pull/5302))
 - BREAKING: [turned `--player` CLI argument into a player-path-only argument](https://streamlink.github.io/migrations.html#player-path-only-player-cli-argument) ([#5305](https://github.com/streamlink/streamlink/issues/5305), [#5310](https://github.com/streamlink/streamlink/pull/5310))  
   Its value won't be interpreted as a command line string anymore, so paths with whitespace don't require additional quotation. Custom player arguments now always need to be set via `--player-args`.
 - BREAKING: [removed deprecated `{filename}` variable from `--player-args`](https://streamlink.github.io/migrations.html#filename-variable-in-player-args) ([#5310](https://github.com/streamlink/streamlink/pull/5310))
 - BREAKING/API: [removed support for the deprecated `Plugin.can_handle_url()` / `Plugin.priority()` classmethods](https://streamlink.github.io/migrations.html#plugin-can-handle-url-and-plugin-priority) ([#5403](https://github.com/streamlink/streamlink/pull/5403))
 - BREAKING/API: [removed deprecated compatibility wrapper for the `Plugin` constructor](https://streamlink.github.io/migrations.html#plugin-init-self-url-compatibility-wrapper) ([#5402](https://github.com/streamlink/streamlink/pull/5402))
+- BREAKING/API: [removed `Streamlink.{g,s}et_plugin_option()`](https://streamlink.github.io/migrations.html#streamlink-g-s-et-plugin-option) ([#5033](https://github.com/streamlink/streamlink/pull/5033))
 - BREAKING/API: [removed deprecated global plugin arguments](https://streamlink.github.io/migrations.html#global-plugin-arguments) ([#5033](https://github.com/streamlink/streamlink/pull/5033))
 - BREAKING/API: [removed deprecated `streamlink.plugin.api.validate.text`](https://streamlink.github.io/migrations.html#plugin-api-validate-text) ([#5404](https://github.com/streamlink/streamlink/pull/5404))
 - BREAKING/API: [fixed/changed signatures of `HTTPStream`, `HLSStream` and `HLSStream.parse_variant_playlist()`](https://streamlink.github.io/migrations.html#httpstream-and-hlsstream-signature-changes) ([#5429](https://github.com/streamlink/streamlink/pull/5429))
 - BREAKING/packaging: new signing key [`44448A298D5C3618`](https://keyserver.ubuntu.com/pks/lookup?search=44448A298D5C3618&fingerprint=on&op=index) ([#5449](https://github.com/streamlink/streamlink/pull/5449))
 
 Release highlights:
```

### Comparing `streamlink-6.0.0/docs/cli/config.rst` & `streamlink-6.0.1/docs/cli/config.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli/metadata.rst` & `streamlink-6.0.1/docs/cli/metadata.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli/plugin-sideloading.rst` & `streamlink-6.0.1/docs/cli/plugin-sideloading.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli/plugins/crunchyroll.rst` & `streamlink-6.0.1/docs/cli/plugins/crunchyroll.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli/plugins/twitch.rst` & `streamlink-6.0.1/docs/cli/plugins/twitch.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli/protocols.rst` & `streamlink-6.0.1/docs/cli/protocols.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli/proxy.rst` & `streamlink-6.0.1/docs/cli/proxy.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli/tutorial.rst` & `streamlink-6.0.1/docs/cli/tutorial.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/cli.rst` & `streamlink-6.0.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/conf.py` & `streamlink-6.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/deprecations.rst` & `streamlink-6.0.1/docs/deprecations.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/developing.rst` & `streamlink-6.0.1/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/donate.rst` & `streamlink-6.0.1/docs/donate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/ext_argparse.py` & `streamlink-6.0.1/docs/ext_argparse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/ext_github.py` & `streamlink-6.0.1/docs/ext_github.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/ext_plugins.py` & `streamlink-6.0.1/docs/ext_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/ext_releaseref.py` & `streamlink-6.0.1/docs/ext_releaseref.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/index.rst` & `streamlink-6.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/install.rst` & `streamlink-6.0.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/issues.rst` & `streamlink-6.0.1/docs/issues.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/migrations.rst` & `streamlink-6.0.1/docs/migrations.rst`

 * *Files 12% similar despite different names*

```diff
@@ -81,14 +81,43 @@
 .. admonition:: Migration
    :class: hint
 
    1. Replace the arguments of custom constructors of each :py:class:`Plugin <streamlink.plugin.Plugin>` subclass with
       ``*args, **kwargs`` and call ``super().__init__(*args, **kwargs)``
    2. If needed, access the ``url`` using ``self.url``
 
+Streamlink.{g,s}et_plugin_option()
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+The ``Streamlink.get_plugin_option()`` and ``Streamlink.set_plugin_option()`` methods were removed as a result of moving
+plugin options from the :py:class:`Plugin <streamlink.plugin.Plugin>` classes to individual ``Plugin`` instances.
+
+Plugin options now must be set referencing the :py:attr:`Plugin.options <streamlink.plugin.Plugin.options>` instance and its
+respective :py:meth:`get <streamlink.options.Options.get>` and :py:meth:`set <streamlink.options.Options.set>` methods.
+
+Alternatively, when initializing a :py:class:`Plugin <streamlink.plugin.Plugin>` class, e.g. after calling
+:py:meth:`Streamlink.resolve_url() <streamlink.session.Streamlink.resolve_url>`, an optional pre-initialized instance of
+:py:class:`Options <streamlink.options.Options>` can be passed to the ``Plugin`` constructor.
+The :py:meth:`Streamlink.streams() <streamlink.session.Streamlink.streams>` method also supports passing an optional ``Options``
+instance to the ``Plugin`` constructor, if a plugin can be resolved from the input URL.
+
+| :octicon:`git-pull-request` #5033
+
+.. admonition:: Migration
+   :class: hint
+
+   1. Initialize an :py:class:`Options <streamlink.options.Options>` object with the desired key-value pairs and pass it to the
+      :py:class:`Plugin <streamlink.plugin.Plugin>` constructor or the
+      :py:meth:`Streamlink.streams() <streamlink.session.Streamlink.streams>` method.
+   2. After instantiating a ``Plugin`` class, get or set its options using the ``get``/``set`` methods on the
+      :py:attr:`Plugin.options <streamlink.plugin.Plugin.options>` instance.
+   3. If plugin options need to be accessed in custom :py:class:`Stream <streamlink.streams.Stream>` implementations related to
+      custom ``Plugin`` implementations, then those options need to be passed from the ``Plugin`` to the ``Stream`` constructor
+      beforehand, since the :py:class:`Streamlink <streamlink.session.Streamlink>` session can't be used for that anymore.
+
 Global plugin arguments
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 Streamlink 5.3.0 :ref:`deprecated <deprecations:Global plugin arguments>` the ``is_global=True`` argument
 of the :py:meth:`pluginargument <streamlink.plugin.pluginargument>` decorator (as well as the
 :py:class:`Argument <streamlink.options.Argument>` class), as global plugin arguments were deemed unnecessary.
 The ``is_global`` argument has thus been removed now.
```

### Comparing `streamlink-6.0.0/docs/players.rst` & `streamlink-6.0.1/docs/players.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/plugins.rst` & `streamlink-6.0.1/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/docs/thirdparty.rst` & `streamlink-6.0.1/docs/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/icon.svg` & `streamlink-6.0.1/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/pyproject.toml` & `streamlink-6.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/setup.py` & `streamlink-6.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/__init__.py` & `streamlink-6.0.1/src/streamlink/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/_version.py` & `streamlink-6.0.1/src/streamlink/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
     return get_version(
         project_dir=Path(streamlink.__file__).parents[2],
     )
 
 
 # The following _get_version() call will get replaced by versioningit with a static version string when building streamlink
 # `pip install .` / `pip wheel .` / `python setup.py build` / `python setup.py bdist_wheel` / etc.
-__version__ = "6.0.0"
+__version__ = "6.0.1"
```

### Comparing `streamlink-6.0.0/src/streamlink/api.py` & `streamlink-6.0.1/src/streamlink/api.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/buffers.py` & `streamlink-6.0.1/src/streamlink/buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/cache.py` & `streamlink-6.0.1/src/streamlink/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/exceptions.py` & `streamlink-6.0.1/src/streamlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/logger.py` & `streamlink-6.0.1/src/streamlink/logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/options.py` & `streamlink-6.0.1/src/streamlink/options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/packages/requests_file.py` & `streamlink-6.0.1/src/streamlink/packages/requests_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugin/__init__.py` & `streamlink-6.0.1/src/streamlink/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/http_session.py` & `streamlink-6.0.1/src/streamlink/plugin/api/http_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
                 break
             except KeyboardInterrupt:
                 raise
             except Exception as rerr:
                 if retries >= total_retries:
                     err = exception(f"Unable to open URL: {url} ({rerr})")
                     err.err = rerr
-                    raise err
+                    raise err from None  # TODO: fix this
                 retries += 1
                 # back off retrying, but only to a maximum sleep time
                 delay = min(retry_max_backoff,
                             retry_backoff * (2 ** (retries - 1)))
                 time.sleep(delay)
 
         if schema:
```

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/useragents.py` & `streamlink-6.0.1/src/streamlink/plugin/api/useragents.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-ANDROID = "Mozilla/5.0 (Linux; Android 13) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.5735.196 Mobile Safari/537.36"
-CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
+ANDROID = "Mozilla/5.0 (Linux; Android 13) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.5790.136 Mobile Safari/537.36"
+CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36"
 CHROME_OS = "Mozilla/5.0 (X11; CrOS x86_64 15359.58.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.5615.134 Safari/537.36"
-FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0"
+FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0"
 IE_11 = "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko"
-IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 16_5_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.5 Mobile/15E148 Safari/604.1"
-OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 OPR/100.0.0.0"
-SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4_1) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.5 Safari/605.1.15"
+IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 16_6 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.5 Mobile/15E148 Safari/604.1"
+OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36 OPR/102.0.0.0"
+SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_5) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.5 Safari/605.1.15"
 
 # Backwards compatibility
 EDGE = CHROME
 FIREFOX_MAC = FIREFOX
 IE_6 = IE_7 = IE_8 = IE_9 = IE_11
 IPHONE_6 = IPAD = IPHONE
 SAFARI_7 = SAFARI_8 = SAFARI
```

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/validate/__init__.py` & `streamlink-6.0.1/src/streamlink/plugin/api/validate/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+# ruff: noqa: A001
+
 # noinspection PyPep8Naming,PyShadowingBuiltins
-from streamlink.plugin.api.validate._schemas import (  # noqa: A001
+from streamlink.plugin.api.validate._schemas import (
     AllSchema as all,
     AnySchema as any,
     AttrSchema as attr,
     GetItemSchema as get,
     ListSchema as list,
     NoneOrAllSchema as none_or_all,
     OptionalSchema as optional,
@@ -16,15 +18,15 @@
 )
 from streamlink.plugin.api.validate._validate import (
     Schema,
     validate,
 )
 
 # noinspection PyShadowingBuiltins
-from streamlink.plugin.api.validate._validators import (  # noqa: A001
+from streamlink.plugin.api.validate._validators import (
     validator_contains as contains,
     validator_endswith as endswith,
     validator_filter as filter,
     validator_getattr as getattr,
     validator_hasattr as hasattr,
     validator_length as length,
     validator_map as map,
```

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/validate/_exception.py` & `streamlink-6.0.1/src/streamlink/plugin/api/validate/_exception.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/validate/_schemas.py` & `streamlink-6.0.1/src/streamlink/plugin/api/validate/_schemas.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/validate/_validate.py` & `streamlink-6.0.1/src/streamlink/plugin/api/validate/_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/validate/_validators.py` & `streamlink-6.0.1/src/streamlink/plugin/api/validate/_validators.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugin/api/websocket.py` & `streamlink-6.0.1/src/streamlink/plugin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugin/plugin.py` & `streamlink-6.0.1/src/streamlink/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/abematv.py` & `streamlink-6.0.1/src/streamlink/plugins/abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/adultswim.py` & `streamlink-6.0.1/src/streamlink/plugins/adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/afreeca.py` & `streamlink-6.0.1/src/streamlink/plugins/afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/albavision.py` & `streamlink-6.0.1/src/streamlink/plugins/albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/aloula.py` & `streamlink-6.0.1/src/streamlink/plugins/aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/app17.py` & `streamlink-6.0.1/src/streamlink/plugins/app17.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ard_live.py` & `streamlink-6.0.1/src/streamlink/plugins/ard_live.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ard_mediathek.py` & `streamlink-6.0.1/src/streamlink/plugins/ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/artetv.py` & `streamlink-6.0.1/src/streamlink/plugins/artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/atpchallenger.py` & `streamlink-6.0.1/src/streamlink/plugins/atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/atresplayer.py` & `streamlink-6.0.1/src/streamlink/plugins/atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/bbciplayer.py` & `streamlink-6.0.1/src/streamlink/plugins/bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/bfmtv.py` & `streamlink-6.0.1/src/streamlink/plugins/bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/bigo.py` & `streamlink-6.0.1/src/streamlink/plugins/bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/bilibili.py` & `streamlink-6.0.1/src/streamlink/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/blazetv.py` & `streamlink-6.0.1/src/streamlink/plugins/blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/bloomberg.py` & `streamlink-6.0.1/src/streamlink/plugins/bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/booyah.py` & `streamlink-6.0.1/src/streamlink/plugins/booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/brightcove.py` & `streamlink-6.0.1/src/streamlink/plugins/brightcove.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/btv.py` & `streamlink-6.0.1/src/streamlink/plugins/btv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/cbsnews.py` & `streamlink-6.0.1/src/streamlink/plugins/cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/cdnbg.py` & `streamlink-6.0.1/src/streamlink/plugins/cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ceskatelevize.py` & `streamlink-6.0.1/src/streamlink/plugins/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/cinergroup.py` & `streamlink-6.0.1/src/streamlink/plugins/cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/clubbingtv.py` & `streamlink-6.0.1/src/streamlink/plugins/clubbingtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/cmmedia.py` & `streamlink-6.0.1/src/streamlink/plugins/cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/cnews.py` & `streamlink-6.0.1/src/streamlink/plugins/cnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/crunchyroll.py` & `streamlink-6.0.1/src/streamlink/plugins/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/dailymotion.py` & `streamlink-6.0.1/src/streamlink/plugins/dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/dash.py` & `streamlink-6.0.1/src/streamlink/plugins/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/delfi.py` & `streamlink-6.0.1/src/streamlink/plugins/delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/deutschewelle.py` & `streamlink-6.0.1/src/streamlink/plugins/deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/dlive.py` & `streamlink-6.0.1/src/streamlink/plugins/dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/dogan.py` & `streamlink-6.0.1/src/streamlink/plugins/dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/dogus.py` & `streamlink-6.0.1/src/streamlink/plugins/dogus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/drdk.py` & `streamlink-6.0.1/src/streamlink/plugins/drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/earthcam.py` & `streamlink-6.0.1/src/streamlink/plugins/earthcam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/euronews.py` & `streamlink-6.0.1/src/streamlink/plugins/euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/facebook.py` & `streamlink-6.0.1/src/streamlink/plugins/facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/filmon.py` & `streamlink-6.0.1/src/streamlink/plugins/filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/foxtr.py` & `streamlink-6.0.1/src/streamlink/plugins/foxtr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/galatasaraytv.py` & `streamlink-6.0.1/src/streamlink/plugins/galatasaraytv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/goltelevision.py` & `streamlink-6.0.1/src/streamlink/plugins/goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/goodgame.py` & `streamlink-6.0.1/src/streamlink/plugins/goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/googledrive.py` & `streamlink-6.0.1/src/streamlink/plugins/googledrive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/gulli.py` & `streamlink-6.0.1/src/streamlink/plugins/gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/hiplayer.py` & `streamlink-6.0.1/src/streamlink/plugins/hiplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/hls.py` & `streamlink-6.0.1/src/streamlink/plugins/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/http.py` & `streamlink-6.0.1/src/streamlink/plugins/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/htv.py` & `streamlink-6.0.1/src/streamlink/plugins/htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/huajiao.py` & `streamlink-6.0.1/src/streamlink/plugins/huajiao.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/huya.py` & `streamlink-6.0.1/src/streamlink/plugins/huya.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import re
 from html import unescape as html_unescape
 from typing import Dict
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.http import HTTPStream
+from streamlink.utils.url import update_scheme
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
     r"https?://(?:www\.)?huya\.com/(?P<channel>[^/]+)",
@@ -92,13 +93,13 @@
             return
 
         self.id, self.author, self.title, streamdata = data
 
         for cdntype, priority, streamname, flvurl, suffix, anticode in streamdata:
             name = f"source_{cdntype.lower()}"
             self.QUALITY_WEIGHTS[name] = priority
-            yield name, HTTPStream(self.session, f"{flvurl}/{streamname}.{suffix}?{anticode}")
+            yield name, HTTPStream(self.session, update_scheme("https://", f"{flvurl}/{streamname}.{suffix}?{anticode}"))
 
         log.debug(f"QUALITY_WEIGHTS: {self.QUALITY_WEIGHTS!r}")
 
 
 __plugin__ = Huya
```

### Comparing `streamlink-6.0.0/src/streamlink/plugins/idf1.py` & `streamlink-6.0.1/src/streamlink/plugins/idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/indihometv.py` & `streamlink-6.0.1/src/streamlink/plugins/indihometv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/invintus.py` & `streamlink-6.0.1/src/streamlink/plugins/invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/kugou.py` & `streamlink-6.0.1/src/streamlink/plugins/kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/linelive.py` & `streamlink-6.0.1/src/streamlink/plugins/linelive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/livestream.py` & `streamlink-6.0.1/src/streamlink/plugins/livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/lnk.py` & `streamlink-6.0.1/src/streamlink/plugins/lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/lrt.py` & `streamlink-6.0.1/src/streamlink/plugins/lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ltv_lsm_lv.py` & `streamlink-6.0.1/src/streamlink/plugins/ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mdstrm.py` & `streamlink-6.0.1/src/streamlink/plugins/mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mediaklikk.py` & `streamlink-6.0.1/src/streamlink/plugins/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mediavitrina.py` & `streamlink-6.0.1/src/streamlink/plugins/mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mildom.py` & `streamlink-6.0.1/src/streamlink/plugins/mildom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mitele.py` & `streamlink-6.0.1/src/streamlink/plugins/mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mixcloud.py` & `streamlink-6.0.1/src/streamlink/plugins/mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mjunoon.py` & `streamlink-6.0.1/src/streamlink/plugins/mjunoon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/mrtmk.py` & `streamlink-6.0.1/src/streamlink/plugins/mrtmk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/n13tv.py` & `streamlink-6.0.1/src/streamlink/plugins/n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/nhkworld.py` & `streamlink-6.0.1/src/streamlink/plugins/nhkworld.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/nicolive.py` & `streamlink-6.0.1/src/streamlink/plugins/nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/nimotv.py` & `streamlink-6.0.1/src/streamlink/plugins/nimotv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/nos.py` & `streamlink-6.0.1/src/streamlink/plugins/nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/nownews.py` & `streamlink-6.0.1/src/streamlink/plugins/nownews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/nrk.py` & `streamlink-6.0.1/src/streamlink/plugins/nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ntv.py` & `streamlink-6.0.1/src/streamlink/plugins/ntv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/okru.py` & `streamlink-6.0.1/src/streamlink/plugins/okru.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/olympicchannel.py` & `streamlink-6.0.1/src/streamlink/plugins/olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/oneplusone.py` & `streamlink-6.0.1/src/streamlink/plugins/oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/onetv.py` & `streamlink-6.0.1/src/streamlink/plugins/onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/openrectv.py` & `streamlink-6.0.1/src/streamlink/plugins/openrectv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/pandalive.py` & `streamlink-6.0.1/src/streamlink/plugins/pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/picarto.py` & `streamlink-6.0.1/src/streamlink/plugins/picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/piczel.py` & `streamlink-6.0.1/src/streamlink/plugins/piczel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/pixiv.py` & `streamlink-6.0.1/src/streamlink/plugins/pixiv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/pluto.py` & `streamlink-6.0.1/src/streamlink/plugins/pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/pluzz.py` & `streamlink-6.0.1/src/streamlink/plugins/pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/qq.py` & `streamlink-6.0.1/src/streamlink/plugins/qq.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/radiko.py` & `streamlink-6.0.1/src/streamlink/plugins/radiko.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/radionet.py` & `streamlink-6.0.1/src/streamlink/plugins/radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/raiplay.py` & `streamlink-6.0.1/src/streamlink/plugins/raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/reuters.py` & `streamlink-6.0.1/src/streamlink/plugins/reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/rtbf.py` & `streamlink-6.0.1/src/streamlink/plugins/rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/rtpa.py` & `streamlink-6.0.1/src/streamlink/plugins/rtpa.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/rtpplay.py` & `streamlink-6.0.1/src/streamlink/plugins/rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/rtve.py` & `streamlink-6.0.1/src/streamlink/plugins/rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/rtvs.py` & `streamlink-6.0.1/src/streamlink/plugins/rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ruv.py` & `streamlink-6.0.1/src/streamlink/plugins/ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/sbscokr.py` & `streamlink-6.0.1/src/streamlink/plugins/sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/showroom.py` & `streamlink-6.0.1/src/streamlink/plugins/showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/sportal.py` & `streamlink-6.0.1/src/streamlink/plugins/sportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/sportschau.py` & `streamlink-6.0.1/src/streamlink/plugins/sportschau.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ssh101.py` & `streamlink-6.0.1/src/streamlink/plugins/ssh101.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/stadium.py` & `streamlink-6.0.1/src/streamlink/plugins/stadium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/steam.py` & `streamlink-6.0.1/src/streamlink/plugins/steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/streamable.py` & `streamlink-6.0.1/src/streamlink/plugins/streamable.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/streann.py` & `streamlink-6.0.1/src/streamlink/plugins/streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/stv.py` & `streamlink-6.0.1/src/streamlink/plugins/stv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/svtplay.py` & `streamlink-6.0.1/src/streamlink/plugins/svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/swisstxt.py` & `streamlink-6.0.1/src/streamlink/plugins/swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/telefe.py` & `streamlink-6.0.1/src/streamlink/plugins/telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/telemadrid.py` & `streamlink-6.0.1/src/streamlink/plugins/telemadrid.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tf1.py` & `streamlink-6.0.1/src/streamlink/plugins/tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/trovo.py` & `streamlink-6.0.1/src/streamlink/plugins/trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/turkuvaz.py` & `streamlink-6.0.1/src/streamlink/plugins/turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tv360.py` & `streamlink-6.0.1/src/streamlink/plugins/tv360.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tv3cat.py` & `streamlink-6.0.1/src/streamlink/plugins/tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tv4play.py` & `streamlink-6.0.1/src/streamlink/plugins/tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tv5monde.py` & `streamlink-6.0.1/src/streamlink/plugins/tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tv8.py` & `streamlink-6.0.1/src/streamlink/plugins/tv8.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tv999.py` & `streamlink-6.0.1/src/streamlink/plugins/tv999.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tvibo.py` & `streamlink-6.0.1/src/streamlink/plugins/tvibo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tviplayer.py` & `streamlink-6.0.1/src/streamlink/plugins/tviplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tvp.py` & `streamlink-6.0.1/src/streamlink/plugins/tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tvrby.py` & `streamlink-6.0.1/src/streamlink/plugins/tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tvrplus.py` & `streamlink-6.0.1/src/streamlink/plugins/tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/tvtoya.py` & `streamlink-6.0.1/src/streamlink/plugins/tvtoya.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/twitcasting.py` & `streamlink-6.0.1/src/streamlink/plugins/twitcasting.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/twitch.py` & `streamlink-6.0.1/src/streamlink/plugins/twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ustreamtv.py` & `streamlink-6.0.1/src/streamlink/plugins/ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/ustvnow.py` & `streamlink-6.0.1/src/streamlink/plugins/ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/vidio.py` & `streamlink-6.0.1/src/streamlink/plugins/vidio.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/vimeo.py` & `streamlink-6.0.1/src/streamlink/plugins/vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/vinhlongtv.py` & `streamlink-6.0.1/src/streamlink/plugins/vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/vk.py` & `streamlink-6.0.1/src/streamlink/plugins/vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/vkplay.py` & `streamlink-6.0.1/src/streamlink/plugins/vkplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/vlive.py` & `streamlink-6.0.1/src/streamlink/plugins/vlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/vtvgo.py` & `streamlink-6.0.1/src/streamlink/plugins/vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/wasd.py` & `streamlink-6.0.1/src/streamlink/plugins/wasd.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/webtv.py` & `streamlink-6.0.1/src/streamlink/plugins/webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/welt.py` & `streamlink-6.0.1/src/streamlink/plugins/welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/wwenetwork.py` & `streamlink-6.0.1/src/streamlink/plugins/wwenetwork.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/youtube.py` & `streamlink-6.0.1/src/streamlink/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/yupptv.py` & `streamlink-6.0.1/src/streamlink/plugins/yupptv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/zattoo.py` & `streamlink-6.0.1/src/streamlink/plugins/zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/zdf_mediathek.py` & `streamlink-6.0.1/src/streamlink/plugins/zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/zeenews.py` & `streamlink-6.0.1/src/streamlink/plugins/zeenews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/zengatv.py` & `streamlink-6.0.1/src/streamlink/plugins/zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/plugins/zhanqi.py` & `streamlink-6.0.1/src/streamlink/plugins/zhanqi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/session.py` & `streamlink-6.0.1/src/streamlink/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,26 +599,27 @@
 
         :param url: a URL to match against loaded plugins
         :raises NoPluginError: on plugin resolve failure
         """
 
         return self.resolve_url(url, follow_redirect=False)
 
-    def streams(self, url: str, **params):
+    def streams(self, url: str, options: Optional[Options] = None, **params):
         """
         Attempts to find a plugin and extracts streams from the *url* if a plugin was found.
 
         :param url: a URL to match against loaded plugins
+        :param options: Optional options instance passed to the resolved plugin
         :param params: Additional keyword arguments passed to :meth:`Plugin.streams() <streamlink.plugin.Plugin.streams>`
         :raises NoPluginError: on plugin resolve failure
         :return: A :class:`dict` of stream names and :class:`Stream <streamlink.stream.Stream>` instances
         """
 
         pluginname, pluginclass, resolved_url = self.resolve_url(url)
-        plugin = pluginclass(self, resolved_url)
+        plugin = pluginclass(self, resolved_url, options)
 
         return plugin.streams(**params)
 
     def get_plugins(self):
         """Returns the loaded plugins for the session."""
 
         return self.plugins
```

### Comparing `streamlink-6.0.0/src/streamlink/stream/dash.py` & `streamlink-6.0.1/src/streamlink/stream/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/dash_manifest.py` & `streamlink-6.0.1/src/streamlink/stream/dash_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         return start, end and ((end - start) + 1)
 
 
 class MPDParsingError(Exception):
     pass
 
 
-TMPDNode = TypeVar("TMPDNode", bound="MPDNode", covariant=True)
+TMPDNode_co = TypeVar("TMPDNode_co", bound="MPDNode", covariant=True)
 TAttrDefault = TypeVar("TAttrDefault", Any, None)
 TAttrParseResult = TypeVar("TAttrParseResult")
 
 TTimelineIdent = Tuple[Optional[str], Optional[str], str]
 
 
 class MPDNode:
@@ -194,48 +194,48 @@
     @overload
     def attr(  # type: ignore[misc]  # "Overloaded function signatures 1 and 2 overlap with incompatible return types"
         self,
         key: str,
         parser: None = None,
         default: None = None,
         required: bool = False,
-        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        inherited: Optional[Union[Type[TMPDNode_co], Sequence[Type[TMPDNode_co]]]] = None,
     ) -> Optional[str]:  # pragma: no cover
         pass
 
     @overload
     def attr(
         self,
         key: str,
         parser: None,
         default: TAttrDefault,
         required: bool = False,
-        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        inherited: Optional[Union[Type[TMPDNode_co], Sequence[Type[TMPDNode_co]]]] = None,
     ) -> TAttrDefault:  # pragma: no cover
         pass
 
     @overload
     def attr(
         self,
         key: str,
         parser: Callable[[Any], TAttrParseResult],
         default: None = None,
         required: bool = False,
-        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        inherited: Optional[Union[Type[TMPDNode_co], Sequence[Type[TMPDNode_co]]]] = None,
     ) -> Optional[TAttrParseResult]:  # pragma: no cover
         pass
 
     @overload
     def attr(
         self,
         key: str,
         parser: Callable[[Any], TAttrParseResult],
         default: TAttrDefault,
         required: bool = False,
-        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        inherited: Optional[Union[Type[TMPDNode_co], Sequence[Type[TMPDNode_co]]]] = None,
     ) -> Union[TAttrParseResult, TAttrDefault]:  # pragma: no cover
         pass
 
     def attr(self, key, parser=None, default=None, required=False, inherited=None):
         self.attributes.add(key)
         if key in self.attrib:
             value = self.attrib.get(key)
@@ -251,54 +251,54 @@
         if required:  # pragma: no cover
             raise MPDParsingError(f"Could not find required attribute {self.__tag__}@{key} ")
 
         return default
 
     def children(
         self,
-        cls: Type[TMPDNode],
+        cls: Type[TMPDNode_co],
         minimum: int = 0,
         maximum: Optional[int] = None,
         **kwargs,
-    ) -> List[TMPDNode]:
+    ) -> List[TMPDNode_co]:
         children = self.node.findall(cls.__tag__)
         if len(children) < minimum or (maximum and len(children) > maximum):
             raise MPDParsingError(f"Expected to find {self.__tag__}/{cls.__tag__} required [{minimum}..{maximum or 'unbound'})")
 
         return [
             cls(child, root=self.root, parent=self, i=i, base_url=self.base_url, **kwargs)
             for i, child in enumerate(children)
         ]
 
     def only_child(
         self,
-        cls: Type[TMPDNode],
+        cls: Type[TMPDNode_co],
         minimum: int = 0,
         **kwargs,
-    ) -> Optional[TMPDNode]:
+    ) -> Optional[TMPDNode_co]:
         children = self.children(cls, minimum=minimum, maximum=1, **kwargs)
         return children[0] if len(children) else None
 
     def walk_back(
         self,
-        cls: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        cls: Optional[Union[Type[TMPDNode_co], Sequence[Type[TMPDNode_co]]]] = None,
         mapper: Callable[["MPDNode"], Optional["MPDNode"]] = _identity,
     ) -> Iterator["MPDNode"]:
         node = self.parent
         while node:
             if cls is None or isinstance(node, cls):  # type: ignore[arg-type]
                 n = mapper(node)  # type: ignore[arg-type]
                 if n is not None:
                     yield n
             node = node.parent
 
     def walk_back_get_attr(
         self,
         attr: str,
-        cls: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        cls: Optional[Union[Type[TMPDNode_co], Sequence[Type[TMPDNode_co]]]] = None,
         mapper: Callable[["MPDNode"], Optional["MPDNode"]] = _identity,
     ) -> Optional[Any]:
         for ancestor in self.walk_back(cls, mapper):
             value = getattr(ancestor, attr, None)
             if value is not None:
                 return value
```

### Comparing `streamlink-6.0.0/src/streamlink/stream/ffmpegmux.py` & `streamlink-6.0.1/src/streamlink/stream/ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/file.py` & `streamlink-6.0.1/src/streamlink/stream/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/filtered.py` & `streamlink-6.0.1/src/streamlink/stream/filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/hls.py` & `streamlink-6.0.1/src/streamlink/stream/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/hls_playlist.py` & `streamlink-6.0.1/src/streamlink/stream/hls_playlist.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/http.py` & `streamlink-6.0.1/src/streamlink/stream/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/segmented.py` & `streamlink-6.0.1/src/streamlink/stream/segmented.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/stream.py` & `streamlink-6.0.1/src/streamlink/stream/stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/stream/wrappers.py` & `streamlink-6.0.1/src/streamlink/stream/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/user_input.py` & `streamlink-6.0.1/src/streamlink/user_input.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/__init__.py` & `streamlink-6.0.1/src/streamlink/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/args.py` & `streamlink-6.0.1/src/streamlink/utils/args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/cache.py` & `streamlink-6.0.1/src/streamlink/utils/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/crypto.py` & `streamlink-6.0.1/src/streamlink/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/data.py` & `streamlink-6.0.1/src/streamlink/utils/data.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/formatter.py` & `streamlink-6.0.1/src/streamlink/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/l10n.py` & `streamlink-6.0.1/src/streamlink/utils/l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/named_pipe.py` & `streamlink-6.0.1/src/streamlink/utils/named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/parse.py` & `streamlink-6.0.1/src/streamlink/utils/parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/processoutput.py` & `streamlink-6.0.1/src/streamlink/utils/processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/random.py` & `streamlink-6.0.1/src/streamlink/utils/random.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/socket.py` & `streamlink-6.0.1/src/streamlink/utils/socket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/times.py` & `streamlink-6.0.1/src/streamlink/utils/times.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/utils/url.py` & `streamlink-6.0.1/src/streamlink/utils/url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/client.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/client.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/connection.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/connection.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/__init__.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/browser.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/browser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/debugger.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/debugger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/dom.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/dom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/emulation.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/emulation.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/fetch.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/fetch.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/input_.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/input_.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/inspector.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/inspector.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/io.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/io.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/network.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/network.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/page.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/page.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/runtime.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/security.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/security.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/target.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/target.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/util.py` & `streamlink-6.0.1/src/streamlink/webbrowser/cdp/devtools/util.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/chromium.py` & `streamlink-6.0.1/src/streamlink/webbrowser/chromium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink/webbrowser/webbrowser.py` & `streamlink-6.0.1/src/streamlink/webbrowser/webbrowser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink.egg-info/PKG-INFO` & `streamlink-6.0.1/src/streamlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 6.0.0
+Version: 6.0.1
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 6.0.0 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.0.1 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Author: Streamlink Author-email:
 streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
 //github.com/streamlink/streamlink Project-URL: Documentation, https://
 streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
 streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
```

### Comparing `streamlink-6.0.0/src/streamlink.egg-info/SOURCES.txt` & `streamlink-6.0.1/src/streamlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/argparser.py` & `streamlink-6.0.1/src/streamlink_cli/argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/console.py` & `streamlink-6.0.1/src/streamlink_cli/console.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/constants.py` & `streamlink-6.0.1/src/streamlink_cli/constants.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/main.py` & `streamlink-6.0.1/src/streamlink_cli/main.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/output/abc.py` & `streamlink-6.0.1/src/streamlink_cli/output/abc.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/output/file.py` & `streamlink-6.0.1/src/streamlink_cli/output/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/output/http.py` & `streamlink-6.0.1/src/streamlink_cli/output/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/output/player.py` & `streamlink-6.0.1/src/streamlink_cli/output/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/streamrunner.py` & `streamlink-6.0.1/src/streamlink_cli/streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/utils/__init__.py` & `streamlink-6.0.1/src/streamlink_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/utils/formatter.py` & `streamlink-6.0.1/src/streamlink_cli/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/utils/path.py` & `streamlink-6.0.1/src/streamlink_cli/utils/path.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/utils/player.py` & `streamlink-6.0.1/src/streamlink_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/utils/progress.py` & `streamlink-6.0.1/src/streamlink_cli/utils/progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/src/streamlink_cli/utils/versioncheck.py` & `streamlink-6.0.1/src/streamlink_cli/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/__init__.py` & `streamlink-6.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/output/test_file.py` & `streamlink-6.0.1/tests/cli/output/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/output/test_player.py` & `streamlink-6.0.1/tests/cli/output/test_player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_argparser.py` & `streamlink-6.0.1/tests/cli/test_argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_cmdline.py` & `streamlink-6.0.1/tests/cli/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_cmdline_title.py` & `streamlink-6.0.1/tests/cli/test_cmdline_title.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_console.py` & `streamlink-6.0.1/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_main.py` & `streamlink-6.0.1/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_main_formatter.py` & `streamlink-6.0.1/tests/cli/test_main_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_main_setup_config_args.py` & `streamlink-6.0.1/tests/cli/test_main_setup_config_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_plugin_args_and_options.py` & `streamlink-6.0.1/tests/cli/test_plugin_args_and_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/test_streamrunner.py` & `streamlink-6.0.1/tests/cli/test_streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/utils/test_formatter.py` & `streamlink-6.0.1/tests/cli/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/utils/test_path.py` & `streamlink-6.0.1/tests/cli/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/utils/test_player.py` & `streamlink-6.0.1/tests/cli/utils/test_player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/utils/test_progress.py` & `streamlink-6.0.1/tests/cli/utils/test_progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/cli/utils/test_versioncheck.py` & `streamlink-6.0.1/tests/cli/utils/test_versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/conftest.py` & `streamlink-6.0.1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,13 +73,13 @@
             session.set_option(key, value)
         yield session
 
     Streamlink.resolve_url.cache_clear()
 
 
 @pytest.fixture()
-def requests_mock(requests_mock: rm.Mocker) -> rm.Mocker:  # noqa: PT004
+def requests_mock(requests_mock: rm.Mocker) -> rm.Mocker:
     """
     Override of the default `requests_mock` fixture, with `InvalidRequest` raised on unknown requests
     """
     requests_mock.register_uri(rm.ANY, rm.ANY, exc=rm.exceptions.InvalidRequest)
     return requests_mock
```

### Comparing `streamlink-6.0.0/tests/mixins/stream_hls.py` & `streamlink-6.0.1/tests/mixins/stream_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugin/testplugin.py` & `streamlink-6.0.1/tests/plugin/testplugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from io import BytesIO
 
 from streamlink import NoStreamsError
-from streamlink.options import Options
 from streamlink.plugin import pluginargument, pluginmatcher
 from streamlink.plugins import Plugin
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 from streamlink.stream.stream import Stream
 
 
@@ -26,18 +25,14 @@
 )
 @pluginargument(
     "password",
     sensitive=True,
     metavar="PASSWORD",
 )
 class TestPlugin(Plugin):
-    options = Options({
-        "a_option": "default",
-    })
-
     id = "test-id-1234-5678"
     author = "Tѥst Āuƭhǿr"
     category = None
     title = "Test Title"
 
     def _get_streams(self):
         if "empty" in self.url:
@@ -49,14 +44,17 @@
                     yield "vod", HTTPStream(self.session, "http://test.se/stream")
 
             return gen()
 
         if "NoStreamsError" in self.url:
             raise NoStreamsError
 
+        if "fromoptions" in self.url:
+            return {"fromoptions": HTTPStream(self.session, self.options.get("streamurl"))}
+
         streams = {}
         streams["test"] = TestStream(self.session)
         streams["hls"] = HLSStream(self.session, "http://test.se/playlist.m3u8")
         streams["http"] = HTTPStream(self.session, "http://test.se/stream")
 
         streams["240p"] = HTTPStream(self.session, "http://test.se/stream")
         streams["360p"] = HTTPStream(self.session, "http://test.se/stream")
```

### Comparing `streamlink-6.0.0/tests/plugins/__init__.py` & `streamlink-6.0.1/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/conftest.py` & `streamlink-6.0.1/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_abematv.py` & `streamlink-6.0.1/tests/plugins/test_abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_adultswim.py` & `streamlink-6.0.1/tests/plugins/test_adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_afreeca.py` & `streamlink-6.0.1/tests/plugins/test_afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_albavision.py` & `streamlink-6.0.1/tests/plugins/test_albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_aloula.py` & `streamlink-6.0.1/tests/plugins/test_aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_ard_mediathek.py` & `streamlink-6.0.1/tests/plugins/test_ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_artetv.py` & `streamlink-6.0.1/tests/plugins/test_artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_atpchallenger.py` & `streamlink-6.0.1/tests/plugins/test_atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_atresplayer.py` & `streamlink-6.0.1/tests/plugins/test_atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_bbciplayer.py` & `streamlink-6.0.1/tests/plugins/test_bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_bfmtv.py` & `streamlink-6.0.1/tests/plugins/test_bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_bigo.py` & `streamlink-6.0.1/tests/plugins/test_bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_blazetv.py` & `streamlink-6.0.1/tests/plugins/test_blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_bloomberg.py` & `streamlink-6.0.1/tests/plugins/test_bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_booyah.py` & `streamlink-6.0.1/tests/plugins/test_booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_cbsnews.py` & `streamlink-6.0.1/tests/plugins/test_cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_cdnbg.py` & `streamlink-6.0.1/tests/plugins/test_cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_ceskatelevize.py` & `streamlink-6.0.1/tests/plugins/test_ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_cinergroup.py` & `streamlink-6.0.1/tests/plugins/test_cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_cmmedia.py` & `streamlink-6.0.1/tests/plugins/test_cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_crunchyroll.py` & `streamlink-6.0.1/tests/plugins/test_crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_dailymotion.py` & `streamlink-6.0.1/tests/plugins/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_dash.py` & `streamlink-6.0.1/tests/plugins/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_delfi.py` & `streamlink-6.0.1/tests/plugins/test_delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_deutschewelle.py` & `streamlink-6.0.1/tests/plugins/test_deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_dogan.py` & `streamlink-6.0.1/tests/plugins/test_dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_drdk.py` & `streamlink-6.0.1/tests/plugins/test_drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_euronews.py` & `streamlink-6.0.1/tests/plugins/test_euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_facebook.py` & `streamlink-6.0.1/tests/plugins/test_facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_filmon.py` & `streamlink-6.0.1/tests/plugins/test_filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_goltelevision.py` & `streamlink-6.0.1/tests/plugins/test_goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_gulli.py` & `streamlink-6.0.1/tests/plugins/test_gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_hls.py` & `streamlink-6.0.1/tests/plugins/test_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_http.py` & `streamlink-6.0.1/tests/plugins/test_http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_htv.py` & `streamlink-6.0.1/tests/plugins/test_htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_idf1.py` & `streamlink-6.0.1/tests/plugins/test_idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_invintus.py` & `streamlink-6.0.1/tests/plugins/test_invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_kugou.py` & `streamlink-6.0.1/tests/plugins/test_kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_livestream.py` & `streamlink-6.0.1/tests/plugins/test_livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_lnk.py` & `streamlink-6.0.1/tests/plugins/test_lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_lrt.py` & `streamlink-6.0.1/tests/plugins/test_lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_ltv_lsm_lv.py` & `streamlink-6.0.1/tests/plugins/test_ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_mdstrm.py` & `streamlink-6.0.1/tests/plugins/test_mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_mediaklikk.py` & `streamlink-6.0.1/tests/plugins/test_mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_mediavitrina.py` & `streamlink-6.0.1/tests/plugins/test_mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_mitele.py` & `streamlink-6.0.1/tests/plugins/test_mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_mixcloud.py` & `streamlink-6.0.1/tests/plugins/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_n13tv.py` & `streamlink-6.0.1/tests/plugins/test_n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_nicolive.py` & `streamlink-6.0.1/tests/plugins/test_nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_nos.py` & `streamlink-6.0.1/tests/plugins/test_nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_nrk.py` & `streamlink-6.0.1/tests/plugins/test_nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_olympicchannel.py` & `streamlink-6.0.1/tests/plugins/test_olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_oneplusone.py` & `streamlink-6.0.1/tests/plugins/test_oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_onetv.py` & `streamlink-6.0.1/tests/plugins/test_onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_pandalive.py` & `streamlink-6.0.1/tests/plugins/test_pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_picarto.py` & `streamlink-6.0.1/tests/plugins/test_picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_pluto.py` & `streamlink-6.0.1/tests/plugins/test_pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_pluzz.py` & `streamlink-6.0.1/tests/plugins/test_pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_radionet.py` & `streamlink-6.0.1/tests/plugins/test_radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_raiplay.py` & `streamlink-6.0.1/tests/plugins/test_raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_reuters.py` & `streamlink-6.0.1/tests/plugins/test_reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_rtbf.py` & `streamlink-6.0.1/tests/plugins/test_rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_rtpplay.py` & `streamlink-6.0.1/tests/plugins/test_rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_rtve.py` & `streamlink-6.0.1/tests/plugins/test_rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_rtvs.py` & `streamlink-6.0.1/tests/plugins/test_rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_ruv.py` & `streamlink-6.0.1/tests/plugins/test_ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_sbscokr.py` & `streamlink-6.0.1/tests/plugins/test_sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_showroom.py` & `streamlink-6.0.1/tests/plugins/test_showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_steam.py` & `streamlink-6.0.1/tests/plugins/test_steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_streann.py` & `streamlink-6.0.1/tests/plugins/test_streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_svtplay.py` & `streamlink-6.0.1/tests/plugins/test_svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_swisstxt.py` & `streamlink-6.0.1/tests/plugins/test_swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_telefe.py` & `streamlink-6.0.1/tests/plugins/test_telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_tf1.py` & `streamlink-6.0.1/tests/plugins/test_tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_trovo.py` & `streamlink-6.0.1/tests/plugins/test_trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_turkuvaz.py` & `streamlink-6.0.1/tests/plugins/test_turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_tv4play.py` & `streamlink-6.0.1/tests/plugins/test_tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_tv5monde.py` & `streamlink-6.0.1/tests/plugins/test_tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_tvp.py` & `streamlink-6.0.1/tests/plugins/test_tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_tvrby.py` & `streamlink-6.0.1/tests/plugins/test_tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_tvrplus.py` & `streamlink-6.0.1/tests/plugins/test_tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_twitch.py` & `streamlink-6.0.1/tests/plugins/test_twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_ustreamtv.py` & `streamlink-6.0.1/tests/plugins/test_ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_ustvnow.py` & `streamlink-6.0.1/tests/plugins/test_ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_vimeo.py` & `streamlink-6.0.1/tests/plugins/test_vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_vinhlongtv.py` & `streamlink-6.0.1/tests/plugins/test_vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_vk.py` & `streamlink-6.0.1/tests/plugins/test_vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_vtvgo.py` & `streamlink-6.0.1/tests/plugins/test_vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_webtv.py` & `streamlink-6.0.1/tests/plugins/test_webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_welt.py` & `streamlink-6.0.1/tests/plugins/test_welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_youtube.py` & `streamlink-6.0.1/tests/plugins/test_youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_zattoo.py` & `streamlink-6.0.1/tests/plugins/test_zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_zdf_mediathek.py` & `streamlink-6.0.1/tests/plugins/test_zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/plugins/test_zengatv.py` & `streamlink-6.0.1/tests/plugins/test_zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/__init__.py` & `streamlink-6.0.1/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_1.mpd` & `streamlink-6.0.1/tests/resources/dash/test_1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_10.mpd` & `streamlink-6.0.1/tests/resources/dash/test_10.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_11_static.mpd` & `streamlink-6.0.1/tests/resources/dash/test_11_static.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_2.mpd` & `streamlink-6.0.1/tests/resources/dash/test_2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_3.mpd` & `streamlink-6.0.1/tests/resources/dash/test_3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_8.mpd` & `streamlink-6.0.1/tests/resources/dash/test_8.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_9.mpd` & `streamlink-6.0.1/tests/resources/dash/test_9.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd` & `streamlink-6.0.1/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd` & `streamlink-6.0.1/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-6.0.1/tests/resources/dash/test_nested_baseurls.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_no_segment_list_or_template.mpd` & `streamlink-6.0.1/tests/resources/dash/test_no_segment_list_or_template.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_segment_list.mpd` & `streamlink-6.0.1/tests/resources/dash/test_segment_list.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_segments_byterange.mpd` & `streamlink-6.0.1/tests/resources/dash/test_segments_byterange.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_segments_dynamic_number.mpd` & `streamlink-6.0.1/tests/resources/dash/test_segments_dynamic_number.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_static_no_publish_time.mpd` & `streamlink-6.0.1/tests/resources/dash/test_static_no_publish_time.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/dash/test_timeline_ids.mpd` & `streamlink-6.0.1/tests/resources/dash/test_timeline_ids.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/hls/test_1.m3u8` & `streamlink-6.0.1/tests/resources/hls/test_1.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/hls/test_2.m3u8` & `streamlink-6.0.1/tests/resources/hls/test_2.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/hls/test_date.m3u8` & `streamlink-6.0.1/tests/resources/hls/test_date.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/hls/test_master.m3u8` & `streamlink-6.0.1/tests/resources/hls/test_master.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/resources/hls/test_master_twitch_vod.m3u8` & `streamlink-6.0.1/tests/resources/hls/test_master_twitch_vod.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_dash.py` & `streamlink-6.0.1/tests/stream/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_dash_parser.py` & `streamlink-6.0.1/tests/stream/test_dash_parser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_ffmpegmux.py` & `streamlink-6.0.1/tests/stream/test_ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_file.py` & `streamlink-6.0.1/tests/stream/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_hls.py` & `streamlink-6.0.1/tests/stream/test_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_hls_filtered.py` & `streamlink-6.0.1/tests/stream/test_hls_filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_hls_playlist.py` & `streamlink-6.0.1/tests/stream/test_hls_playlist.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_stream_json.py` & `streamlink-6.0.1/tests/stream/test_stream_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_stream_to_url.py` & `streamlink-6.0.1/tests/stream/test_stream_to_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/stream/test_stream_wrappers.py` & `streamlink-6.0.1/tests/stream/test_stream_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_api_http_session.py` & `streamlink-6.0.1/tests/test_api_http_session.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_api_validate.py` & `streamlink-6.0.1/tests/test_api_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1448,8 +1448,8 @@
             "foo {foo} bar {bar} baz",
             foo="Some really long error message that exceeds the maximum error message length",
             bar=repr("Some really long error message that exceeds the maximum error message length"),
         )
         assert_validationerror(err, """
             ValidationError:
               foo <Some really long error message that exceeds the maximum...> bar <'Some really long error message that exceeds the maximu...> baz
-        """)  # noqa: 501
+        """)  # noqa: E501
```

### Comparing `streamlink-6.0.0/tests/test_api_websocket.py` & `streamlink-6.0.1/tests/test_api_websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_buffers.py` & `streamlink-6.0.1/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_cache.py` & `streamlink-6.0.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_logger.py` & `streamlink-6.0.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_options.py` & `streamlink-6.0.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_plugin.py` & `streamlink-6.0.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_plugin_userinput.py` & `streamlink-6.0.1/tests/test_plugin_userinput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_plugins.py` & `streamlink-6.0.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/test_session.py` & `streamlink-6.0.1/tests/test_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pytest
 import requests_mock as rm
 import urllib3
 from requests.adapters import HTTPAdapter
 
 import tests.plugin
 from streamlink.exceptions import NoPluginError, StreamlinkDeprecationWarning
+from streamlink.options import Options
 from streamlink.plugin import HIGH_PRIORITY, LOW_PRIORITY, NO_PRIORITY, NORMAL_PRIORITY, Plugin, pluginmatcher
 from streamlink.plugin.api.http_session import TLSNoDHAdapter
 from streamlink.session import Streamlink
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 
 
@@ -250,14 +251,21 @@
         assert "best" in streams
         assert "worst" in streams
         assert streams["best"] is streams["1080p"]
         assert streams["worst"] is streams["350k"]
         assert isinstance(streams["http"], HTTPStream)
         assert isinstance(streams["hls"], HLSStream)
 
+    def test_streams_options(self, session: Streamlink):
+        streams = session.streams("http://test.se/fromoptions", Options({"streamurl": "http://foo/"}))
+
+        assert sorted(streams.keys()) == ["best", "fromoptions", "worst"]
+        assert isinstance(streams["fromoptions"], HTTPStream)
+        assert streams["fromoptions"].url == "http://foo/"
+
     def test_stream_types(self, session: Streamlink):
         streams = session.streams("http://test.se/channel", stream_types=["http", "hls"])
         assert isinstance(streams["480p"], HTTPStream)
         assert isinstance(streams["480p_hls"], HLSStream)
 
         streams = session.streams("http://test.se/channel", stream_types=["hls", "http"])
         assert isinstance(streams["480p"], HLSStream)
```

### Comparing `streamlink-6.0.0/tests/test_streamlink_api.py` & `streamlink-6.0.1/tests/test_streamlink_api.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/testutils/handshake.py` & `streamlink-6.0.1/tests/testutils/handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/testutils/test_handshake.py` & `streamlink-6.0.1/tests/testutils/test_handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_args.py` & `streamlink-6.0.1/tests/utils/test_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_cache.py` & `streamlink-6.0.1/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_crypto.py` & `streamlink-6.0.1/tests/utils/test_crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_data.py` & `streamlink-6.0.1/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_formatter.py` & `streamlink-6.0.1/tests/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_l10n.py` & `streamlink-6.0.1/tests/utils/test_l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_module.py` & `streamlink-6.0.1/tests/utils/test_module.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_named_pipe.py` & `streamlink-6.0.1/tests/utils/test_named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_parse.py` & `streamlink-6.0.1/tests/utils/test_parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_path.py` & `streamlink-6.0.1/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_processoutput.py` & `streamlink-6.0.1/tests/utils/test_processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_random.py` & `streamlink-6.0.1/tests/utils/test_random.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_times.py` & `streamlink-6.0.1/tests/utils/test_times.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/utils/test_url.py` & `streamlink-6.0.1/tests/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/webbrowser/cdp/__init__.py` & `streamlink-6.0.1/tests/webbrowser/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/webbrowser/cdp/conftest.py` & `streamlink-6.0.1/tests/webbrowser/cdp/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/webbrowser/cdp/test_client.py` & `streamlink-6.0.1/tests/webbrowser/cdp/test_client.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/webbrowser/cdp/test_connection.py` & `streamlink-6.0.1/tests/webbrowser/cdp/test_connection.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/webbrowser/conftest.py` & `streamlink-6.0.1/tests/webbrowser/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/webbrowser/test_chromium.py` & `streamlink-6.0.1/tests/webbrowser/test_chromium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.0.0/tests/webbrowser/test_webbrowser.py` & `streamlink-6.0.1/tests/webbrowser/test_webbrowser.py`

 * *Files identical despite different names*

