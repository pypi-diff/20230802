# Comparing `tmp/pyblue-3.0.2.tar.gz` & `tmp/pyblue-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyblue-3.0.2.tar", last modified: Tue Apr 12 18:56:16 2016, max compression
+gzip compressed data, was "dist/pyblue-3.0.3.tar", last modified: Wed Apr 13 15:56:20 2016, max compression
```

## Comparing `pyblue-3.0.2.tar` & `pyblue-3.0.3.tar`

### file list

```diff
@@ -1,108 +1,107 @@
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/
--rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-12-08 15:33:00.000000 pyblue-3.0.2/docs/.DS_Store
--rw-rw----   0 ialbert    (501) staff       (20)      104 2014-12-03 14:56:48.000000 pyblue-3.0.2/docs/__init__.py
--rw-rw----   0 ialbert    (501) staff       (20)      133 2014-12-03 15:21:08.000000 pyblue-3.0.2/docs/__init__.pyc
--rw-r--r--   0 ialbert    (501) staff       (20)      350 2015-04-27 18:06:57.000000 pyblue-3.0.2/docs/base.html
--rw-rw----   0 ialbert    (501) staff       (20)      251 2015-04-27 18:04:05.000000 pyblue-3.0.2/docs/context.py
--rw-rw----   0 ialbert    (501) staff       (20)      378 2015-04-27 18:04:10.000000 pyblue-3.0.2/docs/context.pyc
--rw-rw----   0 ialbert    (501) staff       (20)      430 2016-04-12 17:09:31.000000 pyblue-3.0.2/docs/demo.html
--rw-r--r--   0 ialbert    (501) staff       (20)      184 2015-04-27 18:06:03.000000 pyblue-3.0.2/docs/extend.html
--rw-rw----   0 ialbert    (501) staff       (20)     9465 2016-04-12 18:20:14.000000 pyblue-3.0.2/docs/index.html
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/info/
--rw-rw----   0 ialbert    (501) staff       (20)       79 2016-04-12 17:09:31.000000 pyblue-3.0.2/docs/info/context-loop.txt
--rw-rw----   0 ialbert    (501) staff       (20)     1780 2016-04-12 18:19:13.000000 pyblue-3.0.2/docs/info/context.html
--rw-rw----   0 ialbert    (501) staff       (20)       91 2016-04-11 19:27:56.000000 pyblue-3.0.2/docs/info/django-comments.txt
--rw-rw----   0 ialbert    (501) staff       (20)       51 2016-04-08 19:08:56.000000 pyblue-3.0.2/docs/info/example.md
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/
--rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-12-08 15:44:12.000000 pyblue-3.0.2/docs/slides/.DS_Store
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/lib/
--rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-12-08 15:43:28.000000 pyblue-3.0.2/docs/slides/lib/.DS_Store
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/lib/css/
--rw-rw----   0 ialbert    (501) staff       (20)     1748 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/css/zenburn.css
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/lib/font/
--rwxrwx---   0 ialbert    (501) staff       (20)    18485 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.eot
--rw-rw----   0 ialbert    (501) staff       (20)    47171 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.svg
--rw-rw----   0 ialbert    (501) staff       (20)    42324 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.ttf
--rw-rw----   0 ialbert    (501) staff       (20)    21288 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.woff
--rw-rw----   0 ialbert    (501) staff       (20)       92 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/font/league_gothic_license
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/lib/js/
--rw-rw----   0 ialbert    (501) staff       (20)     1582 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/js/classList.js
--rw-rw----   0 ialbert    (501) staff       (20)     3170 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/js/head.min.js
--rw-rw----   0 ialbert    (501) staff       (20)      235 2014-12-08 14:44:46.000000 pyblue-3.0.2/docs/slides/lib/js/html5shiv.js
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/reveal/
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/reveal/css/
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/reveal/css/print/
--rw-rw----   0 ialbert    (501) staff       (20)     4241 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/print/paper.css
--rw-rw----   0 ialbert    (501) staff       (20)     4012 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/print/pdf.css
--rw-rw----   0 ialbert    (501) staff       (20)    44719 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/reveal.min.css
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/
--rw-rw----   0 ialbert    (501) staff       (20)     4967 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/beige.css
--rw-rw----   0 ialbert    (501) staff       (20)     5193 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/blood.css
--rw-rw----   0 ialbert    (501) staff       (20)     4992 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/default.css
--rw-rw----   0 ialbert    (501) staff       (20)     4261 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/moon.css
--rw-rw----   0 ialbert    (501) staff       (20)     3796 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/night.css
--rw-rw----   0 ialbert    (501) staff       (20)     1734 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/README.md
--rw-rw----   0 ialbert    (501) staff       (20)     3869 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/serif.css
--rw-rw----   0 ialbert    (501) staff       (20)     4001 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/simple.css
--rw-rw----   0 ialbert    (501) staff       (20)     4410 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/sky.css
--rw-rw----   0 ialbert    (501) staff       (20)     4262 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/css/theme/solarized.css
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/slides/reveal/js/
--rw-rw----   0 ialbert    (501) staff       (20)    33368 2014-12-08 15:33:11.000000 pyblue-3.0.2/docs/slides/reveal/js/reveal.min.js
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/templates/
--rw-rw----   0 ialbert    (501) staff       (20)       16 2016-04-12 17:09:31.000000 pyblue-3.0.2/docs/templates/say_hello.html
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/docs/templatetags/
--rw-rw----   0 ialbert    (501) staff       (20)        5 2014-12-03 14:56:48.000000 pyblue-3.0.2/docs/templatetags/__init__.py
--rw-rw----   0 ialbert    (501) staff       (20)      146 2014-12-03 15:21:09.000000 pyblue-3.0.2/docs/templatetags/__init__.pyc
--rw-rw----   0 ialbert    (501) staff       (20)      466 2016-04-12 17:09:31.000000 pyblue-3.0.2/docs/templatetags/demotags.py
--rw-rw----   0 ialbert    (501) staff       (20)      962 2016-04-12 17:41:38.000000 pyblue-3.0.2/docs/templatetags/demotags.pyc
--rw-rw----   0 ialbert    (501) staff       (20)     1181 2014-05-12 17:20:40.000000 pyblue-3.0.2/LICENSE.txt
--rw-rw----   0 ialbert    (501) staff       (20)      123 2016-04-12 17:09:31.000000 pyblue-3.0.2/MANIFEST.in
--rw-rw----   0 ialbert    (501) staff       (20)     4119 2016-04-12 18:56:16.000000 pyblue-3.0.2/PKG-INFO
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue/
--rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-11-25 16:09:35.000000 pyblue-3.0.2/pyblue/.DS_Store
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue/.idea/
--rw-r--r--   0 ialbert    (501) staff       (20)        6 2014-05-12 17:29:07.000000 pyblue-3.0.2/pyblue/.idea/.name
--rw-r--r--   0 ialbert    (501) staff       (20)      166 2014-05-12 17:29:07.000000 pyblue-3.0.2/pyblue/.idea/encodings.xml
--rw-r--r--   0 ialbert    (501) staff       (20)     1352 2014-05-12 17:29:07.000000 pyblue-3.0.2/pyblue/.idea/misc.xml
--rw-r--r--   0 ialbert    (501) staff       (20)      266 2014-05-12 17:29:07.000000 pyblue-3.0.2/pyblue/.idea/modules.xml
--rw-r--r--   0 ialbert    (501) staff       (20)      286 2014-05-12 17:29:07.000000 pyblue-3.0.2/pyblue/.idea/pyblue.iml
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue/.idea/scopes/
--rw-r--r--   0 ialbert    (501) staff       (20)      139 2014-05-12 17:29:07.000000 pyblue-3.0.2/pyblue/.idea/scopes/scope_settings.xml
--rw-r--r--   0 ialbert    (501) staff       (20)      166 2014-05-12 17:29:07.000000 pyblue-3.0.2/pyblue/.idea/vcs.xml
--rw-r--r--   0 ialbert    (501) staff       (20)    16753 2014-05-12 17:32:34.000000 pyblue-3.0.2/pyblue/.idea/workspace.xml
--rw-rw----   0 ialbert    (501) staff       (20)       18 2016-04-12 18:55:50.000000 pyblue-3.0.2/pyblue/__init__.py
--rw-rw----   0 ialbert    (501) staff       (20)      167 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue/__init__.pyc
--rw-rw----   0 ialbert    (501) staff       (20)       68 2016-04-12 18:28:26.000000 pyblue-3.0.2/pyblue/__main__.py
--rw-rw----   0 ialbert    (501) staff       (20)    14223 2016-04-12 18:55:09.000000 pyblue-3.0.2/pyblue/engine.py
--rw-rw----   0 ialbert    (501) staff       (20)    14767 2016-04-12 18:55:15.000000 pyblue-3.0.2/pyblue/engine.pyc
--rwxrwx---   0 ialbert    (501) staff       (20)       80 2016-04-12 18:28:53.000000 pyblue-3.0.2/pyblue/pyblue
--rw-r-----   0 ialbert    (501) staff       (20)    14153 2016-04-11 19:26:44.000000 pyblue-3.0.2/pyblue/pyblue3.pyc
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue/templates/
--rw-rw----   0 ialbert    (501) staff       (20)      246 2016-04-12 17:09:31.000000 pyblue-3.0.2/pyblue/templates/pyblue_base.html
--rw-rw----   0 ialbert    (501) staff       (20)       14 2016-04-12 17:09:31.000000 pyblue-3.0.2/pyblue/templates/say_hello.html
--rw-rw----   0 ialbert    (501) staff       (20)      300 2016-04-12 17:09:31.000000 pyblue-3.0.2/pyblue/templates/site_assets.html
--rw-r--r--   0 ialbert    (501) staff       (20)      323 2016-04-08 19:55:24.000000 pyblue-3.0.2/pyblue/templates/thumbnail.html
--rw-rw----   0 ialbert    (501) staff       (20)       45 2016-04-12 17:09:31.000000 pyblue-3.0.2/pyblue/templates/toggle_box.html
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue/templatetags/
--rw-rw----   0 ialbert    (501) staff       (20)        0 2014-12-03 14:56:48.000000 pyblue-3.0.2/pyblue/templatetags/__init__.py
--rw-rw----   0 ialbert    (501) staff       (20)      152 2016-04-12 17:41:20.000000 pyblue-3.0.2/pyblue/templatetags/__init__.pyc
--rw-rw----   0 ialbert    (501) staff       (20)     4820 2016-04-12 18:42:58.000000 pyblue-3.0.2/pyblue/templatetags/pytags.py
--rw-rw----   0 ialbert    (501) staff       (20)     7058 2016-04-12 18:43:43.000000 pyblue-3.0.2/pyblue/templatetags/pytags.pyc
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue.egg-info/
--rw-rw----   0 ialbert    (501) staff       (20)        1 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue.egg-info/dependency_links.txt
--rw-rw----   0 ialbert    (501) staff       (20)       47 2015-11-06 20:04:43.000000 pyblue-3.0.2/pyblue.egg-info/pbr.json
--rw-rw----   0 ialbert    (501) staff       (20)     4119 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue.egg-info/PKG-INFO
--rw-rw----   0 ialbert    (501) staff       (20)       55 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue.egg-info/requires.txt
--rw-rw----   0 ialbert    (501) staff       (20)     2269 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue.egg-info/SOURCES.txt
--rw-rw----   0 ialbert    (501) staff       (20)        7 2016-04-12 18:56:16.000000 pyblue-3.0.2/pyblue.egg-info/top_level.txt
--rw-rw----   0 ialbert    (501) staff       (20)     2465 2016-04-12 17:09:31.000000 pyblue-3.0.2/README.md
--rw-rw----   0 ialbert    (501) staff       (20)     2346 2016-04-12 17:09:31.000000 pyblue-3.0.2/README.rst
--rw-rw----   0 ialbert    (501) staff       (20)       59 2016-04-12 18:56:16.000000 pyblue-3.0.2/setup.cfg
--rw-rw----   0 ialbert    (501) staff       (20)     1679 2016-04-12 17:09:31.000000 pyblue-3.0.2/setup.py
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/sites/
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/sites/demo/
--rw-rw----   0 ialbert    (501) staff       (20)      170 2014-11-21 20:35:13.000000 pyblue-3.0.2/sites/demo/data.pyc
-drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-12 18:56:16.000000 pyblue-3.0.2/tests/
--rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-11-21 15:22:57.000000 pyblue-3.0.2/tests/.DS_Store
--rw-rw----   0 ialbert    (501) staff       (20)       37 2014-12-03 14:56:48.000000 pyblue-3.0.2/tests/__init__.py
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/
+-rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-12-08 15:33:00.000000 pyblue-3.0.3/docs/.DS_Store
+-rw-rw----   0 ialbert    (501) staff       (20)      104 2014-12-03 14:56:48.000000 pyblue-3.0.3/docs/__init__.py
+-rw-rw----   0 ialbert    (501) staff       (20)      133 2014-12-03 15:21:08.000000 pyblue-3.0.3/docs/__init__.pyc
+-rw-r--r--   0 ialbert    (501) staff       (20)      350 2015-04-27 18:06:57.000000 pyblue-3.0.3/docs/base.html
+-rw-rw----   0 ialbert    (501) staff       (20)      251 2015-04-27 18:04:05.000000 pyblue-3.0.3/docs/context.py
+-rw-rw----   0 ialbert    (501) staff       (20)      378 2015-04-27 18:04:10.000000 pyblue-3.0.3/docs/context.pyc
+-rw-rw----   0 ialbert    (501) staff       (20)      430 2016-04-12 17:09:31.000000 pyblue-3.0.3/docs/demo.html
+-rw-r--r--   0 ialbert    (501) staff       (20)      184 2015-04-27 18:06:03.000000 pyblue-3.0.3/docs/extend.html
+-rw-rw----   0 ialbert    (501) staff       (20)     9465 2016-04-12 18:20:14.000000 pyblue-3.0.3/docs/index.html
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/info/
+-rw-rw----   0 ialbert    (501) staff       (20)       79 2016-04-12 17:09:31.000000 pyblue-3.0.3/docs/info/context-loop.txt
+-rw-rw----   0 ialbert    (501) staff       (20)     1780 2016-04-12 18:19:13.000000 pyblue-3.0.3/docs/info/context.html
+-rw-rw----   0 ialbert    (501) staff       (20)       91 2016-04-11 19:27:56.000000 pyblue-3.0.3/docs/info/django-comments.txt
+-rw-rw----   0 ialbert    (501) staff       (20)       51 2016-04-08 19:08:56.000000 pyblue-3.0.3/docs/info/example.md
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/
+-rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-12-08 15:44:12.000000 pyblue-3.0.3/docs/slides/.DS_Store
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/lib/
+-rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-12-08 15:43:28.000000 pyblue-3.0.3/docs/slides/lib/.DS_Store
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/lib/css/
+-rw-rw----   0 ialbert    (501) staff       (20)     1748 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/css/zenburn.css
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/lib/font/
+-rwxrwx---   0 ialbert    (501) staff       (20)    18485 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.eot
+-rw-rw----   0 ialbert    (501) staff       (20)    47171 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.svg
+-rw-rw----   0 ialbert    (501) staff       (20)    42324 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.ttf
+-rw-rw----   0 ialbert    (501) staff       (20)    21288 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.woff
+-rw-rw----   0 ialbert    (501) staff       (20)       92 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/font/league_gothic_license
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/lib/js/
+-rw-rw----   0 ialbert    (501) staff       (20)     1582 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/js/classList.js
+-rw-rw----   0 ialbert    (501) staff       (20)     3170 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/js/head.min.js
+-rw-rw----   0 ialbert    (501) staff       (20)      235 2014-12-08 14:44:46.000000 pyblue-3.0.3/docs/slides/lib/js/html5shiv.js
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/reveal/
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/reveal/css/
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/reveal/css/print/
+-rw-rw----   0 ialbert    (501) staff       (20)     4241 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/print/paper.css
+-rw-rw----   0 ialbert    (501) staff       (20)     4012 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/print/pdf.css
+-rw-rw----   0 ialbert    (501) staff       (20)    44719 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/reveal.min.css
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/
+-rw-rw----   0 ialbert    (501) staff       (20)     4967 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/beige.css
+-rw-rw----   0 ialbert    (501) staff       (20)     5193 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/blood.css
+-rw-rw----   0 ialbert    (501) staff       (20)     4992 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/default.css
+-rw-rw----   0 ialbert    (501) staff       (20)     4261 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/moon.css
+-rw-rw----   0 ialbert    (501) staff       (20)     3796 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/night.css
+-rw-rw----   0 ialbert    (501) staff       (20)     1734 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/README.md
+-rw-rw----   0 ialbert    (501) staff       (20)     3869 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/serif.css
+-rw-rw----   0 ialbert    (501) staff       (20)     4001 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/simple.css
+-rw-rw----   0 ialbert    (501) staff       (20)     4410 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/sky.css
+-rw-rw----   0 ialbert    (501) staff       (20)     4262 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/css/theme/solarized.css
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/slides/reveal/js/
+-rw-rw----   0 ialbert    (501) staff       (20)    33368 2014-12-08 15:33:11.000000 pyblue-3.0.3/docs/slides/reveal/js/reveal.min.js
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/templates/
+-rw-rw----   0 ialbert    (501) staff       (20)       16 2016-04-12 17:09:31.000000 pyblue-3.0.3/docs/templates/say_hello.html
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/docs/templatetags/
+-rw-rw----   0 ialbert    (501) staff       (20)        5 2014-12-03 14:56:48.000000 pyblue-3.0.3/docs/templatetags/__init__.py
+-rw-rw----   0 ialbert    (501) staff       (20)      146 2014-12-03 15:21:09.000000 pyblue-3.0.3/docs/templatetags/__init__.pyc
+-rw-rw----   0 ialbert    (501) staff       (20)      466 2016-04-12 17:09:31.000000 pyblue-3.0.3/docs/templatetags/demotags.py
+-rw-rw----   0 ialbert    (501) staff       (20)      962 2016-04-12 17:41:38.000000 pyblue-3.0.3/docs/templatetags/demotags.pyc
+-rw-rw----   0 ialbert    (501) staff       (20)     1181 2014-05-12 17:20:40.000000 pyblue-3.0.3/LICENSE.txt
+-rw-rw----   0 ialbert    (501) staff       (20)      123 2016-04-12 17:09:31.000000 pyblue-3.0.3/MANIFEST.in
+-rw-rw----   0 ialbert    (501) staff       (20)     4151 2016-04-13 15:56:20.000000 pyblue-3.0.3/PKG-INFO
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue/
+-rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-11-25 16:09:35.000000 pyblue-3.0.3/pyblue/.DS_Store
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue/.idea/
+-rw-r--r--   0 ialbert    (501) staff       (20)        6 2014-05-12 17:29:07.000000 pyblue-3.0.3/pyblue/.idea/.name
+-rw-r--r--   0 ialbert    (501) staff       (20)      220 2016-04-13 15:22:20.000000 pyblue-3.0.3/pyblue/.idea/encodings.xml
+-rw-r--r--   0 ialbert    (501) staff       (20)     1352 2014-05-12 17:29:07.000000 pyblue-3.0.3/pyblue/.idea/misc.xml
+-rw-r--r--   0 ialbert    (501) staff       (20)      266 2014-05-12 17:29:07.000000 pyblue-3.0.3/pyblue/.idea/modules.xml
+-rw-r--r--   0 ialbert    (501) staff       (20)      286 2014-05-12 17:29:07.000000 pyblue-3.0.3/pyblue/.idea/pyblue.iml
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue/.idea/scopes/
+-rw-r--r--   0 ialbert    (501) staff       (20)      139 2014-05-12 17:29:07.000000 pyblue-3.0.3/pyblue/.idea/scopes/scope_settings.xml
+-rw-r--r--   0 ialbert    (501) staff       (20)    16892 2016-04-13 15:25:59.000000 pyblue-3.0.3/pyblue/.idea/workspace.xml
+-rw-rw----   0 ialbert    (501) staff       (20)       18 2016-04-13 15:50:54.000000 pyblue-3.0.3/pyblue/__init__.py
+-rw-rw----   0 ialbert    (501) staff       (20)      167 2016-04-13 15:51:02.000000 pyblue-3.0.3/pyblue/__init__.pyc
+-rw-rw----   0 ialbert    (501) staff       (20)       68 2016-04-12 18:28:26.000000 pyblue-3.0.3/pyblue/__main__.py
+-rw-rw----   0 ialbert    (501) staff       (20)    14218 2016-04-13 15:32:57.000000 pyblue-3.0.3/pyblue/engine.py
+-rw-rw----   0 ialbert    (501) staff       (20)    14750 2016-04-13 15:46:57.000000 pyblue-3.0.3/pyblue/engine.pyc
+-rwxrwx---   0 ialbert    (501) staff       (20)       80 2016-04-12 18:28:53.000000 pyblue-3.0.3/pyblue/pyblue
+-rw-r-----   0 ialbert    (501) staff       (20)    14153 2016-04-11 19:26:44.000000 pyblue-3.0.3/pyblue/pyblue3.pyc
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue/templates/
+-rw-rw----   0 ialbert    (501) staff       (20)      246 2016-04-12 17:09:31.000000 pyblue-3.0.3/pyblue/templates/pyblue_base.html
+-rw-rw----   0 ialbert    (501) staff       (20)       14 2016-04-12 17:09:31.000000 pyblue-3.0.3/pyblue/templates/say_hello.html
+-rw-rw----   0 ialbert    (501) staff       (20)      300 2016-04-12 17:09:31.000000 pyblue-3.0.3/pyblue/templates/site_assets.html
+-rw-r--r--   0 ialbert    (501) staff       (20)      323 2016-04-08 19:55:24.000000 pyblue-3.0.3/pyblue/templates/thumbnail.html
+-rw-rw----   0 ialbert    (501) staff       (20)       45 2016-04-12 17:09:31.000000 pyblue-3.0.3/pyblue/templates/toggle_box.html
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue/templatetags/
+-rw-rw----   0 ialbert    (501) staff       (20)        0 2014-12-03 14:56:48.000000 pyblue-3.0.3/pyblue/templatetags/__init__.py
+-rw-rw----   0 ialbert    (501) staff       (20)      152 2016-04-12 17:41:20.000000 pyblue-3.0.3/pyblue/templatetags/__init__.pyc
+-rw-rw----   0 ialbert    (501) staff       (20)     4831 2016-04-13 15:21:42.000000 pyblue-3.0.3/pyblue/templatetags/pytags.py
+-rw-rw----   0 ialbert    (501) staff       (20)     7069 2016-04-13 15:22:49.000000 pyblue-3.0.3/pyblue/templatetags/pytags.pyc
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue.egg-info/
+-rw-rw----   0 ialbert    (501) staff       (20)        1 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue.egg-info/dependency_links.txt
+-rw-rw----   0 ialbert    (501) staff       (20)       47 2015-11-06 20:04:43.000000 pyblue-3.0.3/pyblue.egg-info/pbr.json
+-rw-rw----   0 ialbert    (501) staff       (20)     4151 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue.egg-info/PKG-INFO
+-rw-rw----   0 ialbert    (501) staff       (20)       55 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue.egg-info/requires.txt
+-rw-rw----   0 ialbert    (501) staff       (20)     2248 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue.egg-info/SOURCES.txt
+-rw-rw----   0 ialbert    (501) staff       (20)        7 2016-04-13 15:56:20.000000 pyblue-3.0.3/pyblue.egg-info/top_level.txt
+-rw-rw----   0 ialbert    (501) staff       (20)     2465 2016-04-13 15:50:54.000000 pyblue-3.0.3/README.md
+-rw-rw----   0 ialbert    (501) staff       (20)     2370 2016-04-13 15:55:39.000000 pyblue-3.0.3/README.rst
+-rw-rw----   0 ialbert    (501) staff       (20)       59 2016-04-13 15:56:20.000000 pyblue-3.0.3/setup.cfg
+-rw-rw----   0 ialbert    (501) staff       (20)     1679 2016-04-12 17:09:31.000000 pyblue-3.0.3/setup.py
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/sites/
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/sites/demo/
+-rw-rw----   0 ialbert    (501) staff       (20)      170 2014-11-21 20:35:13.000000 pyblue-3.0.3/sites/demo/data.pyc
+drwxrwx---   0 ialbert    (501) staff       (20)        0 2016-04-13 15:56:20.000000 pyblue-3.0.3/tests/
+-rw-r--r--   0 ialbert    (501) staff       (20)     6148 2014-11-21 15:22:57.000000 pyblue-3.0.3/tests/.DS_Store
+-rw-rw----   0 ialbert    (501) staff       (20)       37 2014-12-03 14:56:48.000000 pyblue-3.0.3/tests/__init__.py
```

### Comparing `pyblue-3.0.2/docs/.DS_Store` & `pyblue-3.0.3/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/index.html` & `pyblue-3.0.3/docs/index.html`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/info/context.html` & `pyblue-3.0.3/docs/info/context.html`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/.DS_Store` & `pyblue-3.0.3/docs/slides/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/.DS_Store` & `pyblue-3.0.3/docs/slides/lib/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/css/zenburn.css` & `pyblue-3.0.3/docs/slides/lib/css/zenburn.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.eot` & `pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.eot`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.svg` & `pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.svg`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.ttf` & `pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/font/league_gothic-webfont.woff` & `pyblue-3.0.3/docs/slides/lib/font/league_gothic-webfont.woff`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/js/classList.js` & `pyblue-3.0.3/docs/slides/lib/js/classList.js`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/lib/js/head.min.js` & `pyblue-3.0.3/docs/slides/lib/js/head.min.js`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/print/paper.css` & `pyblue-3.0.3/docs/slides/reveal/css/print/paper.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/print/pdf.css` & `pyblue-3.0.3/docs/slides/reveal/css/print/pdf.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/reveal.min.css` & `pyblue-3.0.3/docs/slides/reveal/css/reveal.min.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/beige.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/beige.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/blood.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/blood.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/default.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/default.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/moon.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/moon.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/night.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/night.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/README.md` & `pyblue-3.0.3/docs/slides/reveal/css/theme/README.md`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/serif.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/serif.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/simple.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/simple.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/sky.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/sky.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/css/theme/solarized.css` & `pyblue-3.0.3/docs/slides/reveal/css/theme/solarized.css`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/slides/reveal/js/reveal.min.js` & `pyblue-3.0.3/docs/slides/reveal/js/reveal.min.js`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/docs/templatetags/demotags.pyc` & `pyblue-3.0.3/docs/templatetags/demotags.pyc`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/LICENSE.txt` & `pyblue-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/PKG-INFO` & `pyblue-3.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,106 @@
 Metadata-Version: 1.1
 Name: pyblue
-Version: 3.0.2
+Version: 3.0.3
 Summary: PyBlue
 Home-page: https://github.com/ialbert/pyblue
 Author: Istvan Albert
 Author-email: istvan.albert@gmail.com
 License: MIT
-Description: Welcome to Pyblue
-        -----------------
-        
-        A simple static site generator.
-        
-        Why another one? There are `many static <https://www.staticgen.com/>`__
-        site generators already. I found to be way too complicated, they have
-        too many rules, put this here or there, call thing this or that.
-        
-        PyBlue is different. Everything is optional, only use what you need.
-        Stays out of the way.
-        
-        From the simplest tasks:
-        
-        -  No configuration required.
-        -  Works with any existing site.
-        -  Easy to include ``markdown``.
-        -  Easy linking to other pages.
-        -  Tiny codebase, pyblue is around 500 lines in a single file!
-        
-        To more complicated:
-        
-        -  PyBlue generates the correct links even if you move pages around.
-        -  Use `Django
-           Templates <https://docs.djangoproject.com/en/1.9/ref/templates/language/>`__
-           and all the features that it offers.
-        -  Easily add data into each page (title, link name, or any arbitrary
-           content).
-        
-        Or go all the way out:
-        
-        -  Load python modules into each page.
-        -  Exposed data: database queries, results of online requests etc.
-        -  Run python code, access and modify data from inside of each page.
-        -  Extend the Django templates. Add your own ``templatetags``.
-        
-        Install
-        ~~~~~~~
-        
-        ::
-        
-            pip install pyblue --upgrade
-        
-        Or download it from the `PyBlue at
-        PyPI <https://pypi.python.org/pypi/pyblue/>`__.
-        
-        Usage
-        ~~~~~
-        
-        Launch pyblue to serve a directory
-        
-        ::
-        
-            pyblue -r docs
-        
-        View your site by visiting http:://localhost:8080
-        
-        Edit your pages and make changes. Reload the page to see your edits
-        live. Generate static output with:
-        
-        ::
-        
-            pyblue -r docs -o html
-        
-        That's all. Told you it was simple. To see extra help on options run:
-        
-        ::
-        
-            pyblue -h
-        
-        Documentation
-        ~~~~~~~~~~~~~
-        
-        -  The `PyBlue Documentation <https://ialbert.github.io/pyblue/>`__ was
-           generated with PyBlue itself.
-        
-        You can also browse the `help in source
-        format <https://github.com/ialbert/pyblue/tree/master/docs>`__ for
-        examples.
-        
-        Licensing
-        ~~~~~~~~~
-        
-        -  PyBlue is being developed by Istvan Albert see
-           https://github.com/ialbert
-        -  PyBlue has been inspired by
-           `PyGreen <https://github.com/nicolas-van/pygreen>`__ created by
-           Nicolas Vanhoren see https://github.com/nicolas-van
-        -  PyBlue uses the `MIT
-           license <https://github.com/ialbert/pyblue/blob/master/LICENSE.txt>`__.
+Description: Welcome to PyBlue
+        -----------------
+        
+        A simple static site generator.
+        
+        Why another one? There are `many static <https://www.staticgen.com/>`__
+        site generators already. I found most to be way too complicated, too
+        many conventions and rules: put this here or there, call it this or
+        that. It was too tiring to keep up.
+        
+        PyBlue is different. Everything is optional, nothing is required, use
+        only what you need. It basically stays out of the way.
+        
+        Simple things are very easy:
+        
+        -  No configuration required.
+        -  Works with any existing site.
+        -  Easy to include ``markdown``.
+        -  Easy linking to other pages.
+        -  Tiny codebase, pyblue is around 500 lines in a single file!
+        
+        Complicated tasks are easy:
+        
+        -  PyBlue generates the correct links even if you move pages around.
+        -  Use `Django
+           Templates <https://docs.djangoproject.com/en/1.9/ref/templates/language/>`__
+           and all the features that it offers.
+        -  Easily add data into each page (title, link name, or any arbitrary
+           content).
+        
+        And you can go all the way out if you really want to:
+        
+        -  Load python modules into each page.
+        -  Exposed data: database queries, results of online requests etc.
+        -  Run python code, access and modify data from inside of each page.
+        -  Extend the Django templates. Add your own ``templatetags``.
+        
+        Install
+        ~~~~~~~
+        
+        ::
+        
+            pip install pyblue --upgrade
+        
+        Or download it from the `PyBlue at
+        PyPI <https://pypi.python.org/pypi/pyblue/>`__.
+        
+        Usage
+        ~~~~~
+        
+        Launch pyblue to serve a directory
+        
+        ::
+        
+            pyblue -r docs
+        
+        View your site by visiting http:://localhost:8080
+        
+        Edit your pages and make changes. Reload the page to see your edits
+        live. Generate static output with:
+        
+        ::
+        
+            pyblue -r docs -o html
+        
+        That's all. Told you it was simple. To see extra help on options run:
+        
+        ::
+        
+            pyblue -h
+        
+        Documentation
+        ~~~~~~~~~~~~~
+        
+        -  The `PyBlue Documentation <https://ialbert.github.io/pyblue/>`__ was
+           generated with PyBlue itself.
+        
+        You can also browse the `help in source
+        format <https://github.com/ialbert/pyblue/tree/master/docs>`__ for
+        examples.
+        
+        Licensing
+        ~~~~~~~~~
+        
+        -  PyBlue is being developed by Istvan Albert see
+           https://github.com/ialbert
+        -  PyBlue has been inspired by
+           `PyGreen <https://github.com/nicolas-van/pygreen>`__ created by
+           Nicolas Vanhoren see https://github.com/nicolas-van
+        -  PyBlue uses the `MIT
+           license <https://github.com/ialbert/pyblue/blob/master/LICENSE.txt>`__.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyblue-3.0.2/pyblue/.DS_Store` & `pyblue-3.0.3/pyblue/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/pyblue/.idea/misc.xml` & `pyblue-3.0.3/pyblue/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/pyblue/.idea/workspace.xml` & `pyblue-3.0.3/pyblue/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `pyblue-3.0.2/pyblue/.idea/workspace.xml` & `pyblue-3.0.3/pyblue/.idea/workspace.xml`

```diff
@@ -1,48 +1,41 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="68e76c6a-edd0-4129-9a2c-94269793f7f2" name="Default" comment=""/>
     <ignored path="pyblue.iws"/>
     <ignored path=".idea/workspace.xml"/>
+    <option name="EXCLUDED_CONVERTED_TO_IGNORED" value="true"/>
     <option name="TRACKING_ENABLED" value="true"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="ChangesViewManager" flattened_view="true" show_ignored="false"/>
   <component name="CreatePatchCommitExecutor">
     <option name="PATCH_PATH" value=""/>
   </component>
-  <component name="DaemonCodeAnalyzer">
-    <disable_hints/>
-  </component>
   <component name="ExecutionTargetManager" SELECTED_TARGET="default_target"/>
   <component name="FavoritesManager">
     <favorites_list name="pyblue"/>
   </component>
   <component name="FileEditorManager">
-    <leaf>
-      <file leaf-file-name="base.mako" pinned="false" current="true" current-in-tab="true">
-        <entry file="file://$PROJECT_DIR$/templates/base.mako">
-          <provider selected="true" editor-type-id="text-editor">
-            <state line="4" column="35" selection-start="77" selection-end="77" vertical-scroll-proportion="0.08791209" vertical-offset="0" max-vertical-offset="1176">
-              <folding/>
-            </state>
-          </provider>
-        </entry>
-      </file>
-    </leaf>
+    <leaf SIDE_TABS_SIZE_LIMIT_KEY="300"/>
   </component>
   <component name="FindManager">
     <FindUsagesManager>
       <setting name="OPEN_NEW_TAB" value="false"/>
     </FindUsagesManager>
   </component>
+  <component name="JsBuildToolGruntFileManager" detection-done="true"/>
+  <component name="JsBuildToolPackageJson" detection-done="true"/>
+  <component name="JsGulpfileManager">
+    <detection-done>true</detection-done>
+  </component>
   <component name="ProjectFrameBounds">
     <option name="x" value="757"/>
     <option name="y" value="154"/>
     <option name="width" value="1739"/>
     <option name="height" value="1254"/>
   </component>
   <component name="ProjectLevelVcsManager" settingsEditedManually="false">
@@ -55,26 +48,29 @@
     <ConfirmationsSetting value="0" id="Add"/>
     <ConfirmationsSetting value="0" id="Remove"/>
   </component>
   <component name="ProjectReloadState">
     <option name="STATE" value="0"/>
   </component>
   <component name="ProjectView">
-    <navigator currentView="ProjectPane" proportions="" version="1" splitterProportion="0.5">
+    <navigator currentView="ProjectPane" proportions="" version="1">
       <flattenPackages/>
       <showMembers/>
       <showModules/>
       <showLibraryContents/>
       <hideEmptyPackages/>
       <abbreviatePackageNames/>
       <autoscrollToSource/>
       <autoscrollFromSource/>
       <sortByType/>
+      <manualOrder/>
+      <foldersAlwaysOnTop value="true"/>
     </navigator>
     <panes>
+      <pane id="Scratches"/>
       <pane id="ProjectPane">
         <subPane>
           <PATH>
             <PATH_ELEMENT>
               <option name="myItemId" value="pyblue"/>
               <option name="myItemType" value="com.intellij.ide.projectView.impl.nodes.ProjectViewProjectNode"/>
             </PATH_ELEMENT>
@@ -97,14 +93,15 @@
   <component name="PropertiesComponent">
     <property name="options.splitter.main.proportions" value="0.3"/>
     <property name="options.lastSelected" value="preferences.keymap"/>
     <property name="options.searchVisible" value="true"/>
     <property name="options.splitter.details.proportions" value="0.2"/>
     <property name="WebServerToolWindowFactoryState" value="false"/>
     <property name="FullScreen" value="false"/>
+    <property name="last_opened_file_path" value="$PROJECT_DIR$"/>
   </component>
   <component name="RunManager">
     <configuration default="true" type="DjangoTestsConfigurationType" factoryName="Django tests">
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
@@ -119,40 +116,36 @@
       <option name="TARGET" value=""/>
       <option name="SETTINGS_FILE" value=""/>
       <option name="CUSTOM_SETTINGS" value="false"/>
       <option name="USE_OPTIONS" value="false"/>
       <option name="OPTIONS" value=""/>
       <method/>
     </configuration>
-    <configuration default="true" type="tests" factoryName="py.test">
+    <configuration default="true" type="JavascriptDebugType" factoryName="JavaScript Debug">
+      <method/>
+    </configuration>
+    <configuration default="true" type="PythonConfigurationType" factoryName="Python">
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
-      <envs/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value=""/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <module name="pyblue"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" enabled="false" sample_coverage="true" runner="coverage.py"/>
       <option name="SCRIPT_NAME" value=""/>
-      <option name="CLASS_NAME" value=""/>
-      <option name="METHOD_NAME" value=""/>
-      <option name="FOLDER_NAME" value=""/>
-      <option name="TEST_TYPE" value="TEST_SCRIPT"/>
-      <option name="PATTERN" value=""/>
-      <option name="USE_PATTERN" value="false"/>
-      <option name="testToRun" value=""/>
-      <option name="keywords" value=""/>
-      <option name="params" value=""/>
-      <option name="USE_PARAM" value="false"/>
-      <option name="USE_KEYWORD" value="false"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
       <method/>
     </configuration>
-    <configuration default="true" type="tests" factoryName="Nosetests">
+    <configuration default="true" type="tests" factoryName="Attests">
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value=""/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
@@ -162,39 +155,37 @@
       <option name="SCRIPT_NAME" value=""/>
       <option name="CLASS_NAME" value=""/>
       <option name="METHOD_NAME" value=""/>
       <option name="FOLDER_NAME" value=""/>
       <option name="TEST_TYPE" value="TEST_SCRIPT"/>
       <option name="PATTERN" value=""/>
       <option name="USE_PATTERN" value="false"/>
-      <option name="PARAMS" value=""/>
-      <option name="USE_PARAM" value="false"/>
       <method/>
     </configuration>
-    <configuration default="true" type="PythonConfigurationType" factoryName="Python">
+    <configuration default="true" type="tests" factoryName="Doctests">
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
-      <envs>
-        <env name="PYTHONUNBUFFERED" value="1"/>
-      </envs>
+      <envs/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value=""/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <module name="pyblue"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" enabled="false" sample_coverage="true" runner="coverage.py"/>
       <option name="SCRIPT_NAME" value=""/>
-      <option name="PARAMETERS" value=""/>
-      <method/>
-    </configuration>
-    <configuration default="true" type="JavascriptDebugType" factoryName="JavaScript Debug" singleton="true">
+      <option name="CLASS_NAME" value=""/>
+      <option name="METHOD_NAME" value=""/>
+      <option name="FOLDER_NAME" value=""/>
+      <option name="TEST_TYPE" value="TEST_SCRIPT"/>
+      <option name="PATTERN" value=""/>
+      <option name="USE_PATTERN" value="false"/>
       <method/>
     </configuration>
-    <configuration default="true" type="tests" factoryName="Unittests">
+    <configuration default="true" type="tests" factoryName="Nosetests">
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value=""/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
@@ -204,20 +195,19 @@
       <option name="SCRIPT_NAME" value=""/>
       <option name="CLASS_NAME" value=""/>
       <option name="METHOD_NAME" value=""/>
       <option name="FOLDER_NAME" value=""/>
       <option name="TEST_TYPE" value="TEST_SCRIPT"/>
       <option name="PATTERN" value=""/>
       <option name="USE_PATTERN" value="false"/>
-      <option name="PUREUNITTEST" value="true"/>
       <option name="PARAMS" value=""/>
       <option name="USE_PARAM" value="false"/>
       <method/>
     </configuration>
-    <configuration default="true" type="tests" factoryName="Doctests">
+    <configuration default="true" type="tests" factoryName="Unittests">
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value=""/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
@@ -227,17 +217,20 @@
       <option name="SCRIPT_NAME" value=""/>
       <option name="CLASS_NAME" value=""/>
       <option name="METHOD_NAME" value=""/>
       <option name="FOLDER_NAME" value=""/>
       <option name="TEST_TYPE" value="TEST_SCRIPT"/>
       <option name="PATTERN" value=""/>
       <option name="USE_PATTERN" value="false"/>
+      <option name="PUREUNITTEST" value="true"/>
+      <option name="PARAMS" value=""/>
+      <option name="USE_PARAM" value="false"/>
       <method/>
     </configuration>
-    <configuration default="true" type="tests" factoryName="Attests">
+    <configuration default="true" type="tests" factoryName="py.test">
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value=""/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
@@ -247,70 +240,63 @@
       <option name="SCRIPT_NAME" value=""/>
       <option name="CLASS_NAME" value=""/>
       <option name="METHOD_NAME" value=""/>
       <option name="FOLDER_NAME" value=""/>
       <option name="TEST_TYPE" value="TEST_SCRIPT"/>
       <option name="PATTERN" value=""/>
       <option name="USE_PATTERN" value="false"/>
+      <option name="testToRun" value=""/>
+      <option name="keywords" value=""/>
+      <option name="params" value=""/>
+      <option name="USE_PARAM" value="false"/>
+      <option name="USE_KEYWORD" value="false"/>
       <method/>
     </configuration>
-    <list size="0"/>
   </component>
   <component name="ShelveChangesManager" show_recycled="false"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="68e76c6a-edd0-4129-9a2c-94269793f7f2" name="Default" comment=""/>
       <created>1399915745892</created>
+      <option name="number" value="Default"/>
       <updated>1399915745892</updated>
     </task>
     <servers/>
   </component>
   <component name="ToolWindowManager">
     <frame x="757" y="154" width="1739" height="1254" extended-state="0"/>
-    <editor active="false"/>
+    <editor active="true"/>
     <layout>
-      <window_info id="Changes" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
-      <window_info id="Terminal" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
-      <window_info id="TODO" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="6" side_tool="false" content_ui="tabs"/>
-      <window_info id="Database" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="3" side_tool="false" content_ui="tabs"/>
-      <window_info id="Structure" active="false" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.25" sideWeight="0.5" order="1" side_tool="false" content_ui="tabs"/>
-      <window_info id="Project" active="true" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="true" weight="0.25279906" sideWeight="0.5" order="0" side_tool="false" content_ui="combo"/>
-      <window_info id="Debug" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.4" sideWeight="0.5" order="3" side_tool="false" content_ui="tabs"/>
-      <window_info id="Favorites" active="false" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="2" side_tool="true" content_ui="tabs"/>
-      <window_info id="Event Log" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="7" side_tool="true" content_ui="tabs"/>
-      <window_info id="Run" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="2" side_tool="false" content_ui="tabs"/>
-      <window_info id="Version Control" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
-      <window_info id="Cvs" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.25" sideWeight="0.5" order="4" side_tool="false" content_ui="tabs"/>
-      <window_info id="Message" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="0" side_tool="false" content_ui="tabs"/>
-      <window_info id="Ant Build" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.25" sideWeight="0.5" order="1" side_tool="false" content_ui="tabs"/>
-      <window_info id="Find" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.33" sideWeight="0.5" order="1" side_tool="false" content_ui="tabs"/>
-      <window_info id="Commander" active="false" anchor="right" auto_hide="false" internal_type="SLIDING" type="SLIDING" visible="false" weight="0.4" sideWeight="0.5" order="0" side_tool="false" content_ui="tabs"/>
-      <window_info id="Hierarchy" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.25" sideWeight="0.5" order="2" side_tool="false" content_ui="combo"/>
-      <window_info id="Inspection" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" weight="0.4" sideWeight="0.5" order="5" side_tool="false" content_ui="tabs"/>
+      <window_info id="Project" active="true" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="true" show_stripe_button="true" weight="0.25574544" sideWeight="0.5" order="0" side_tool="false" content_ui="combo"/>
+      <window_info id="TODO" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="6" side_tool="false" content_ui="tabs"/>
+      <window_info id="Event Log" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="7" side_tool="true" content_ui="tabs"/>
+      <window_info id="Database" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="3" side_tool="false" content_ui="tabs"/>
+      <window_info id="Python Console" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="-1" side_tool="false" content_ui="tabs"/>
+      <window_info id="Version Control" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
+      <window_info id="Structure" active="false" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.25" sideWeight="0.5" order="1" side_tool="false" content_ui="tabs"/>
+      <window_info id="Terminal" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
+      <window_info id="Favorites" active="false" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="2" side_tool="true" content_ui="tabs"/>
+      <window_info id="Changes" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
+      <window_info id="Cvs" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.25" sideWeight="0.5" order="4" side_tool="false" content_ui="tabs"/>
+      <window_info id="Message" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="0" side_tool="false" content_ui="tabs"/>
+      <window_info id="Commander" active="false" anchor="right" auto_hide="false" internal_type="SLIDING" type="SLIDING" visible="false" show_stripe_button="true" weight="0.4" sideWeight="0.5" order="0" side_tool="false" content_ui="tabs"/>
+      <window_info id="Inspection" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.4" sideWeight="0.5" order="5" side_tool="false" content_ui="tabs"/>
+      <window_info id="Run" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="2" side_tool="false" content_ui="tabs"/>
+      <window_info id="Hierarchy" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.25" sideWeight="0.5" order="2" side_tool="false" content_ui="combo"/>
+      <window_info id="Find" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="1" side_tool="false" content_ui="tabs"/>
+      <window_info id="Ant Build" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.25" sideWeight="0.5" order="1" side_tool="false" content_ui="tabs"/>
+      <window_info id="Debug" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.4" sideWeight="0.5" order="3" side_tool="false" content_ui="tabs"/>
     </layout>
   </component>
   <component name="Vcs.Log.UiProperties">
     <option name="RECENTLY_FILTERED_USER_GROUPS">
       <collection/>
     </option>
   </component>
   <component name="VcsContentAnnotationSettings">
     <option name="myLimit" value="2678400000"/>
   </component>
-  <component name="VcsManagerConfiguration">
-    <option name="myTodoPanelSettings">
-      <TodoPanelSettings/>
-    </option>
-  </component>
   <component name="XDebuggerManager">
     <breakpoint-manager/>
-  </component>
-  <component name="editorHistoryManager">
-    <entry file="file://$PROJECT_DIR$/templates/base.mako">
-      <provider selected="true" editor-type-id="text-editor">
-        <state line="4" column="35" selection-start="77" selection-end="77" vertical-scroll-proportion="0.08791209" vertical-offset="0" max-vertical-offset="1176">
-          <folding/>
-        </state>
-      </provider>
-    </entry>
+    <watches-manager/>
   </component>
 </project>
```

### Comparing `pyblue-3.0.2/pyblue/engine.py` & `pyblue-3.0.3/pyblue/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,18 +276,20 @@
     def nicer_name(self, fname):
         """
         Attempts to generate a nicer name from the filename.
         Removes underscores, dashes and extensions.
         """
         head, tail = os.path.split(fname)
         base, ext = os.path.splitext(tail)
-        name = base.title().replace("-", " ").replace("_", " ")
+
+        # Non templates keep their original name.
         if not self.is_template:
-            # Add back extension for non templates.
-            name += self.ext
+            return tail
+
+        name = base.title().replace("-", " ").replace("_", " ")
         return name
 
     def write(self, output, content='', check=True):
         """
         Writes the text into an output folder
         """
         dest = os.path.join(output, self.fname)
```

### Comparing `pyblue-3.0.2/pyblue/engine.pyc` & `pyblue-3.0.3/pyblue/engine.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 8d44 0d57 6300 0000 0000 0000  .....D.Wc.......
+00000000: 03f3 0d0a a966 0e57 6300 0000 0000 0000  .....f.Wc.......
 00000010: 0003 0000 0040 6003 0073 cb01 0000 6400  .....@`..s....d.
 00000020: 005a 0000 6401 0064 0200 6c01 006d 0200  .Z..d..d..l..m..
 00000030: 5a02 006d 0300 5a03 006d 0400 5a04 006d  Z..m..Z..m..Z..m
 00000040: 0500 5a05 0001 6401 0064 0300 6c06 005a  ..Z...d..d..l..Z
 00000050: 0600 6401 0064 0300 6c07 005a 0700 6401  ..d..d..l..Z..d.
 00000060: 0064 0300 6c08 005a 0800 6401 0064 0300  .d..l..Z..d..d..
 00000070: 6c09 005a 0900 6401 0064 0300 6c0a 005a  l..Z..d..d..l..Z
@@ -557,367 +557,366 @@
 000022c0: 0700 0000 4d41 5853 495a 4528 0000 0000  ....MAXSIZE(....
 000022d0: 2800 0000 0073 3200 0000 2f55 7365 7273  (....s2.../Users
 000022e0: 2f69 616c 6265 7274 2f61 7070 2f70 7962  /ialbert/app/pyb
 000022f0: 6c75 652d 6365 6e74 7261 6c2f 7079 626c  lue-central/pybl
 00002300: 7565 2f65 6e67 696e 652e 7079 523e 0000  ue/engine.pyR>..
 00002310: 000a 0100 0073 0a00 0000 0002 0602 0f01  .....s..........
 00002320: 1401 0402 6302 0000 0007 0000 0003 0000  ....c...........
-00002330: 0043 6003 0073 7100 0000 7400 006a 0100  .C`..sq...t..j..
+00002330: 0043 6003 0073 6500 0000 7400 006a 0100  .C`..se...t..j..
 00002340: 6a02 007c 0100 8301 005c 0200 7d02 007d  j..|.....\..}..}
 00002350: 0300 7400 006a 0100 6a03 007c 0300 8301  ..t..j..j..|....
-00002360: 005c 0200 7d04 007d 0500 7c04 006a 0400  .\..}..}..|..j..
-00002370: 8300 006a 0500 6401 0064 0200 8302 006a  ...j..d..d.....j
-00002380: 0500 6403 0064 0200 8302 007d 0600 7c00  ..d..d.....}..|.
-00002390: 006a 0600 736d 007c 0600 7c00 006a 0700  .j..sm.|..|..j..
-000023a0: 377d 0600 6e00 007c 0600 5328 0400 0000  7}..n..|..S(....
-000023b0: 757a 0000 000a 2020 2020 2020 2020 4174  uz....        At
-000023c0: 7465 6d70 7473 2074 6f20 6765 6e65 7261  tempts to genera
-000023d0: 7465 2061 206e 6963 6572 206e 616d 6520  te a nicer name 
-000023e0: 6672 6f6d 2074 6865 2066 696c 656e 616d  from the filenam
-000023f0: 652e 0a20 2020 2020 2020 2052 656d 6f76  e..        Remov
-00002400: 6573 2075 6e64 6572 7363 6f72 6573 2c20  es underscores, 
-00002410: 6461 7368 6573 2061 6e64 2065 7874 656e  dashes and exten
-00002420: 7369 6f6e 732e 0a20 2020 2020 2020 2075  sions..        u
-00002430: 0100 0000 2d75 0100 0000 2075 0100 0000  ....-u.... u....
-00002440: 5f28 0800 0000 520a 0000 0052 0b00 0000  _(....R....R....
-00002450: 525e 0000 0052 4b00 0000 5273 0000 0074  R^...RK...Rs...t
-00002460: 0700 0000 7265 706c 6163 6552 1a00 0000  ....replaceR....
-00002470: 5254 0000 0028 0700 0000 5223 0000 0052  RT...(....R#...R
-00002480: 1000 0000 7404 0000 0068 6561 6474 0400  ....t....headt..
-00002490: 0000 7461 696c 526a 0000 0052 5400 0000  ..tailRj...RT...
-000024a0: 5252 0000 0028 0000 0000 2800 0000 0073  RR...(....(....s
-000024b0: 3200 0000 2f55 7365 7273 2f69 616c 6265  2.../Users/ialbe
-000024c0: 7274 2f61 7070 2f70 7962 6c75 652d 6365  rt/app/pyblue-ce
-000024d0: 6e74 7261 6c2f 7079 626c 7565 2f65 6e67  ntral/pyblue/eng
-000024e0: 696e 652e 7079 5283 0000 0014 0100 0073  ine.pyR........s
-000024f0: 0c00 0000 0005 1801 1801 2401 0902 1001  ..........$.....
-00002500: 7500 0000 0063 0400 0000 0700 0000 0600  u....c..........
-00002510: 0000 4360 0300 7335 0100 0074 0000 6a01  ..C`..s5...t..j.
-00002520: 006a 0200 7c01 007c 0000 6a03 0083 0200  .j..|..|..j.....
-00002530: 7d04 0074 0000 6a01 006a 0400 7c04 0083  }..t..j..j..|...
-00002540: 0100 7400 006a 0100 6a04 007c 0000 6a01  ..t..j..j..|..j.
-00002550: 0083 0100 6b02 0072 5200 7405 0064 0100  ....k..rR.t..d..
-00002560: 7c04 0016 8301 0082 0100 6e00 007c 0300  |.........n..|..
-00002570: 7288 0074 0600 7c04 0083 0100 7406 007c  r..t..|.....t..|
-00002580: 0000 6a01 0083 0100 6b04 0072 8800 7407  ..j.....k..r..t.
-00002590: 006a 0800 6402 007c 0400 1683 0100 0164  .j..d..|.......d
-000025a0: 0300 5374 0000 6a01 006a 0900 7c04 0083  ..St..j..j..|...
-000025b0: 0100 7d05 0074 0000 6a01 006a 0a00 7c05  ..}..t..j..j..|.
-000025c0: 0083 0100 73bc 0074 0000 6a0b 007c 0500  ....s..t..j..|..
-000025d0: 8301 0001 6e00 007c 0000 6a0c 0072 0d01  ....n..|..j..r..
-000025e0: 7c02 0072 0d01 7407 006a 0d00 6404 007c  |..r..t..j..d..|
-000025f0: 0400 1683 0100 0174 0e00 6a0f 007c 0400  .......t..j..|..
-00002600: 6405 0064 0600 6407 0083 0201 8f14 007d  d..d..d........}
-00002610: 0600 7c06 006a 1000 7c02 0083 0100 0157  ..|..j..|......W
-00002620: 6403 0051 586e 2400 7407 006a 0d00 6408  d..QXn$.t..j..d.
-00002630: 007c 0400 1683 0100 0174 1100 6a12 007c  .|.......t..j..|
-00002640: 0000 6a01 007c 0400 8302 0001 6403 0053  ..j..|......d..S
-00002650: 2809 0000 0075 3700 0000 0a20 2020 2020  (....u7....     
-00002660: 2020 2057 7269 7465 7320 7468 6520 7465     Writes the te
-00002670: 7874 2069 6e74 6f20 616e 206f 7574 7075  xt into an outpu
-00002680: 7420 666f 6c64 6572 0a20 2020 2020 2020  t folder.       
-00002690: 2075 2a00 0000 6361 6e6e 6f74 206e 6f74   u*...cannot not
-000026a0: 206f 7665 7277 7269 7465 2074 6865 206f   overwrite the o
-000026b0: 7269 6769 6e61 6c20 6669 6c65 3a20 2573  riginal file: %s
-000026c0: 7508 0000 0073 6b69 703a 2025 734e 750a  u....skip: %sNu.
-000026d0: 0000 0073 6176 696e 673a 2025 7375 0200  ...saving: %su..
-000026e0: 0000 7774 5288 0000 0075 0500 0000 7574  ..wtR....u....ut
-000026f0: 662d 3875 0b00 0000 636f 7079 696e 673a  f-8u....copying:
-00002700: 2025 7328 1300 0000 520a 0000 0052 0b00   %s(....R....R..
-00002710: 0000 520d 0000 0052 1000 0000 520c 0000  ..R....R....R...
-00002720: 0052 3000 0000 5272 0000 0052 1700 0000  .R0...Rr...R....
-00002730: 5218 0000 0052 6200 0000 7406 0000 0065  R....Rb...t....e
-00002740: 7869 7374 7374 0800 0000 6d61 6b65 6469  xistst....makedi
-00002750: 7273 521a 0000 0052 3b00 0000 5289 0000  rsR....R;...R...
-00002760: 0052 8a00 0000 5244 0000 0074 0600 0000  .R....RD...t....
-00002770: 7368 7574 696c 7408 0000 0063 6f70 7966  shutilt....copyf
-00002780: 696c 6528 0700 0000 5223 0000 0052 4600  ile(....R#...RF.
-00002790: 0000 523e 0000 0052 3f00 0000 7404 0000  ..R>...R?...t...
-000027a0: 0064 6573 7474 0500 0000 6470 6174 6874  .destt....dpatht
-000027b0: 0200 0000 6670 2800 0000 0028 0000 0000  ....fp(....(....
-000027c0: 7332 0000 002f 5573 6572 732f 6961 6c62  s2.../Users/ialb
-000027d0: 6572 742f 6170 702f 7079 626c 7565 2d63  ert/app/pyblue-c
-000027e0: 656e 7472 616c 2f70 7962 6c75 652f 656e  entral/pyblue/en
-000027f0: 6769 6e65 2e70 7952 4400 0000 2101 0000  gine.pyRD...!...
-00002800: 731e 0000 0000 0418 0327 0113 0321 0111  s........'...!..
-00002810: 0104 0312 0112 0110 030f 0111 011b 0116  ................
-00002820: 0211 0163 0200 0000 0300 0000 0300 0000  ...c............
-00002830: 4360 0300 7343 0000 007c 0100 7009 007c  C`..sC...|..p..|
-00002840: 0000 7d01 0074 0000 6a01 006a 0200 7c00  ..}..t..j..j..|.
-00002850: 006a 0300 7c01 006a 0400 8302 007d 0200  .j..|..j.....}..
-00002860: 7400 006a 0100 6a05 007c 0200 7c00 006a  t..j..j..|..|..j
-00002870: 0600 8302 007d 0200 7c02 0053 2801 0000  .....}..|..S(...
-00002880: 0075 4200 0000 0a20 2020 2020 2020 2052  .uB....        R
-00002890: 656c 6174 6976 6520 7061 7468 206f 6620  elative path of 
-000028a0: 7468 6973 2066 696c 6520 6672 6f6d 2061  this file from a
-000028b0: 2073 7461 7274 206c 6f63 6174 696f 6e0a   start location.
-000028c0: 2020 2020 2020 2020 2807 0000 0052 0a00          (....R..
-000028d0: 0000 520b 0000 0052 4d00 0000 5211 0000  ..R....RM...R...
-000028e0: 0052 7d00 0000 520d 0000 0052 1000 0000  .R}...R....R....
-000028f0: 2803 0000 0052 2300 0000 5253 0000 0074  (....R#...RS...t
-00002900: 0500 0000 7270 6174 6828 0000 0000 2800  ....rpath(....(.
-00002910: 0000 0073 3200 0000 2f55 7365 7273 2f69  ...s2.../Users/i
-00002920: 616c 6265 7274 2f61 7070 2f70 7962 6c75  albert/app/pyblu
-00002930: 652d 6365 6e74 7261 6c2f 7079 626c 7565  e-central/pyblue
-00002940: 2f65 6e67 696e 652e 7079 524d 0000 003e  /engine.pyRM...>
-00002950: 0100 0073 0800 0000 0004 0c01 1b01 1801  ...s............
-00002960: 6302 0000 0003 0000 0003 0000 0043 6003  c............C`.
-00002970: 0073 1900 0000 7c00 006a 0000 6a01 007c  .s....|..j..j..|
-00002980: 0100 6401 0083 0200 7d02 007c 0200 5328  ..d.....}..|..S(
-00002990: 0200 0000 7591 0000 000a 2020 2020 2020  ....u.....      
-000029a0: 2020 4d65 7461 6461 7461 206d 6179 2062    Metadata may b
-000029b0: 6520 6163 6365 7373 6564 2061 7320 616e  e accessed as an
-000029c0: 2061 7474 7269 6275 7465 7320 6f6e 2074   attributes on t
-000029d0: 6865 2063 6c61 7373 2e0a 2020 2020 2020  he class..      
-000029e0: 2020 5468 6973 2067 6574 7320 7472 6967    This gets trig
-000029f0: 6765 7265 6420 6173 2061 2066 616c 6c62  gered as a fallb
-00002a00: 6163 6b20 6966 2061 6e20 6174 7472 6962  ack if an attrib
-00002a10: 7574 6520 6973 206e 6f74 2066 6f75 6e64  ute is not found
-00002a20: 2e0a 2020 2020 2020 2020 4e28 0300 0000  ..        N(....
-00002a30: 5275 0000 0074 0300 0000 6765 7452 2900  Ru...t....getR).
-00002a40: 0000 2803 0000 0052 2300 0000 5252 0000  ..(....R#...RR..
-00002a50: 0074 0500 0000 7661 6c75 6528 0000 0000  .t....value(....
-00002a60: 2800 0000 0073 3200 0000 2f55 7365 7273  (....s2.../Users
-00002a70: 2f69 616c 6265 7274 2f61 7070 2f70 7962  /ialbert/app/pyb
-00002a80: 6c75 652d 6365 6e74 7261 6c2f 7079 626c  lue-central/pybl
-00002a90: 7565 2f65 6e67 696e 652e 7079 740b 0000  ue/engine.pyt...
-00002aa0: 005f 5f67 6574 6174 7472 5f5f 4701 0000  .__getattr__G...
-00002ab0: 7304 0000 0000 0515 0163 0100 0000 0100  s........c......
-00002ac0: 0000 0400 0000 4360 0300 731d 0000 0064  ......C`..s....d
-00002ad0: 0100 7c00 006a 0000 6a01 007c 0000 6a02  ..|..j..j..|..j.
-00002ae0: 007c 0000 6a03 0066 0300 1653 2802 0000  .|..j..f...S(...
-00002af0: 0075 2e00 0000 0a20 2020 2020 2020 2055  .u.....        U
-00002b00: 7365 7220 6672 6965 6e64 6c79 2072 6570  ser friendly rep
-00002b10: 7265 7365 6e74 6174 696f 6e0a 2020 2020  resentation.    
-00002b20: 2020 2020 750b 0000 0025 733a 2025 7320      u....%s: %s 
-00002b30: 2825 7329 2804 0000 0074 0900 0000 5f5f  (%s)(....t....__
-00002b40: 636c 6173 735f 5f52 6d00 0000 5252 0000  class__Rm...RR..
-00002b50: 0052 1000 0000 2801 0000 0052 2300 0000  .R....(....R#...
-00002b60: 2800 0000 0028 0000 0000 7332 0000 002f  (....(....s2.../
-00002b70: 5573 6572 732f 6961 6c62 6572 742f 6170  Users/ialbert/ap
-00002b80: 702f 7079 626c 7565 2d63 656e 7472 616c  p/pyblue-central
-00002b90: 2f70 7962 6c75 652f 656e 6769 6e65 2e70  /pyblue/engine.p
-00002ba0: 7974 0800 0000 5f5f 7265 7072 5f5f 4f01  yt....__repr__O.
-00002bb0: 0000 7302 0000 0000 044e 2810 0000 0052  ..s......N(....R
-00002bc0: 6d00 0000 526e 0000 0074 0700 0000 5f5f  m...Rn...t....__
-00002bd0: 646f 635f 5f52 7e00 0000 527f 0000 0052  doc__R~...R....R
-00002be0: 8100 0000 5236 0000 0074 0800 0000 7072  ....R6...t....pr
-00002bf0: 6f70 6572 7479 523e 0000 0052 8300 0000  opertyR>...R....
-00002c00: 523d 0000 0052 4400 0000 5229 0000 0052  R=...RD...R)...R
-00002c10: 4d00 0000 529a 0000 0052 9c00 0000 2800  M...R....R....(.
-00002c20: 0000 0028 0000 0000 2800 0000 0073 3200  ...(....(....s2.
-00002c30: 0000 2f55 7365 7273 2f69 616c 6265 7274  ../Users/ialbert
-00002c40: 2f61 7070 2f70 7962 6c75 652d 6365 6e74  /app/pyblue-cent
-00002c50: 7261 6c2f 7079 626c 7565 2f65 6e67 696e  ral/pyblue/engin
-00002c60: 652e 7079 5219 0000 00d0 0000 0073 1600  e.pyR........s..
-00002c70: 0000 0603 0602 0c01 1501 0902 0931 0f0a  .............1..
-00002c80: 090d 0f1d 0c09 0908 6301 0000 000a 0000  ........c.......
-00002c90: 0006 0000 0043 6003 0073 d700 0000 7400  .....C`..s....t.
-00002ca0: 006a 0100 6401 0083 0100 7d01 0074 0200  .j..d.....}..t..
-00002cb0: 6a03 007c 0000 6402 0064 0300 8301 016a  j..|..d..d.....j
-00002cc0: 0400 8300 006a 0500 8300 0064 0400 207d  .....j.....d.. }
-00002cd0: 0200 7406 0074 0700 7c02 0083 0200 7d02  ..t..t..|.....}.
-00002ce0: 0074 0800 8300 007d 0300 7884 007c 0200  .t.....}..x..|..
-00002cf0: 445d 7c00 7d04 007c 0100 6a09 007c 0400  D]|.}..|..j..|..
-00002d00: 8301 007d 0500 7c05 0072 5300 7c05 006a  ...}..|..rS.|..j
-00002d10: 0a00 6405 0083 0100 7c05 006a 0a00 6406  ..d.....|..j..d.
-00002d20: 0083 0100 027d 0600 7d07 0079 1300 740b  .....}..}..y..t.
-00002d30: 006a 0c00 7c07 0083 0100 7d08 0057 6e1f  .j..|.....}..Wn.
-00002d40: 0004 740d 006b 0a00 72c1 0001 7d09 0001  ..t..k..r...}...
-00002d50: 740e 007c 0700 8301 007d 0800 6e01 0058  t..|.....}..n..X
-00002d60: 7c08 007c 0300 7c06 003c 7153 0071 5300  |..|..|..<qS.qS.
-00002d70: 577c 0300 5328 0700 0000 758e 0000 000a  W|..S(....u.....
-00002d80: 2020 2020 4174 7465 6d70 7473 2074 6f20      Attempts to 
-00002d90: 7061 7273 6520 6f75 7420 6d65 7461 6461  parse out metada
-00002da0: 7461 2066 726f 6d20 646a 616e 676f 2063  ta from django c
-00002db0: 6f6d 6d65 6e74 732e 0a20 2020 2045 6163  omments..    Eac
-00002dc0: 6820 636f 6d6d 656e 7420 6973 2061 7373  h comment is ass
-00002dd0: 756d 6564 2074 6f20 6265 206b 6579 203d  umed to be key =
-00002de0: 2076 616c 7565 2077 6865 7265 2074 6865   value where the
-00002df0: 2076 616c 7565 2069 7320 6120 4a53 4f4e   value is a JSON
-00002e00: 206f 626a 6563 742e 0a20 2020 2075 3100   object..    u1.
-00002e10: 0000 5e7b 235c 733f 283f 503c 6e61 6d65  ..^{#\s?(?P<name
-00002e20: 3e5c 772b 295c 733f 3d5c 733f 283f 503c  >\w+)\s?=\s?(?P<
-00002e30: 7661 6c75 653e 5b5c 535c 735d 2b29 5c73  value>[\S\s]+)\s
-00002e40: 3f23 7d52 8800 0000 7505 0000 0075 7466  ?#}R....u....utf
-00002e50: 2d38 6964 0000 0075 0400 0000 6e61 6d65  -8id...u....name
-00002e60: 7505 0000 0076 616c 7565 280f 0000 0074  u....value(....t
-00002e70: 0200 0000 7265 7407 0000 0063 6f6d 7069  ....ret....compi
-00002e80: 6c65 5289 0000 0052 8a00 0000 528b 0000  leR....R....R...
-00002e90: 0074 0a00 0000 7370 6c69 746c 696e 6573  .t....splitlines
-00002ea0: 7403 0000 006d 6170 5204 0000 0052 1b00  t....mapR....R..
-00002eb0: 0000 7406 0000 0073 6561 7263 6874 0500  ..t....searcht..
-00002ec0: 0000 6772 6f75 7074 0400 0000 6a73 6f6e  ..groupt....json
-00002ed0: 7405 0000 006c 6f61 6473 740a 0000 0056  t....loadst....V
-00002ee0: 616c 7565 4572 726f 7274 0300 0000 7374  alueErrort....st
-00002ef0: 7228 0a00 0000 520b 0000 0074 0700 0000  r(....R....t....
-00002f00: 5041 5454 4552 4e74 0500 0000 6c69 6e65  PATTERNt....line
-00002f10: 7352 7500 0000 7404 0000 006c 696e 6574  sRu...t....linet
-00002f20: 0100 0000 6d52 5200 0000 5299 0000 0074  ....mRR...R....t
-00002f30: 0300 0000 6f62 6a52 3500 0000 2800 0000  ....objR5...(...
-00002f40: 0028 0000 0000 7332 0000 002f 5573 6572  .(....s2.../User
-00002f50: 732f 6961 6c62 6572 742f 6170 702f 7079  s/ialbert/app/py
-00002f60: 626c 7565 2d63 656e 7472 616c 2f70 7962  blue-central/pyb
-00002f70: 6c75 652f 656e 6769 6e65 2e70 7952 8400  lue/engine.pyR..
-00002f80: 0000 5601 0000 731c 0000 0000 060f 0325  ..V...s........%
-00002f90: 010f 0109 010d 010f 0106 011f 0103 0113  ................
-00002fa0: 010f 0110 0111 0263 0100 0000 0100 0000  .......c........
-00002fb0: 0100 0000 4360 0300 7304 0000 0064 0100  ....C`..s....d..
-00002fc0: 5328 0200 0000 7537 0000 000a 2020 2020  S(....u7....    
-00002fd0: 4164 6473 2074 6865 2063 6f6d 6d6f 6e20  Adds the common 
-00002fe0: 7061 7261 6d65 7465 7273 2074 6f20 6561  parameters to ea
-00002ff0: 6368 2073 7562 7061 7273 6572 2e0a 2020  ch subparser..  
-00003000: 2020 4e28 0000 0000 2801 0000 0074 0600    N(....(....t..
-00003010: 0000 7061 7273 6572 2800 0000 0028 0000  ..parser(....(..
-00003020: 0000 7332 0000 002f 5573 6572 732f 6961  ..s2.../Users/ia
-00003030: 6c62 6572 742f 6170 702f 7079 626c 7565  lbert/app/pyblue
-00003040: 2d63 656e 7472 616c 2f70 7962 6c75 652f  -central/pyblue/
-00003050: 656e 6769 6e65 2e70 7974 1400 0000 6164  engine.pyt....ad
-00003060: 645f 636f 6d6d 6f6e 5f61 7267 756d 656e  d_common_argumen
-00003070: 7473 6f01 0000 7300 0000 0063 0000 0000  tso...s....c....
-00003080: 0100 0000 0e00 0000 4360 0300 7346 0100  ........C`..sF..
-00003090: 0074 0000 6a01 0064 0100 7402 0083 0001  .t..j..d..t.....
-000030a0: 7d00 007c 0000 6a03 0064 0200 6403 0064  }..|..j..d..d..d
-000030b0: 0400 6405 0064 0600 6407 0064 0800 6409  ..d..d..d..d..d.
-000030c0: 0074 0400 640a 0064 0b00 8301 0501 7c00  .t..d..d......|.
-000030d0: 006a 0300 640c 0064 0300 640d 0064 0500  .j..d..d..d..d..
-000030e0: 6406 0064 0e00 7405 0064 0900 7406 0064  d..d..t..d..t..d
-000030f0: 0700 640f 0064 0a00 6410 0083 0106 017c  ..d..d..d......|
-00003100: 0000 6a03 0064 1100 6403 0064 1200 6405  ..j..d..d..d..d.
-00003110: 0064 1300 640e 0074 0500 6409 0074 0600  .d..d..t..d..t..
-00003120: 6407 0064 1400 640a 0064 1500 8301 0601  d..d..d..d......
-00003130: 7c00 006a 0300 6416 0064 0500 6417 0064  |..j..d..d..d..d
-00003140: 0e00 7407 0064 0300 6418 0064 0700 6419  ..t..d..d..d..d.
-00003150: 0064 0a00 641a 0083 0105 017c 0000 6a03  .d..d......|..j.
-00003160: 0064 1b00 641c 0064 0300 641d 0064 0700  .d..d..d..d..d..
-00003170: 7406 0064 1e00 641f 0064 0a00 6420 0083  t..d..d..d..d ..
-00003180: 0204 017c 0000 6a03 0064 2100 6422 0064  ...|..j..d!.d".d
-00003190: 0300 6423 0064 0700 7406 0064 1e00 641f  ..d#.d..t..d..d.
-000031a0: 0064 0a00 6424 0083 0204 017c 0000 6a03  .d..d$.....|..j.
-000031b0: 0064 2500 6426 0064 0300 6427 0064 0700  .d%.d&.d..d'.d..
-000031c0: 7406 0064 1e00 641f 0064 0a00 6428 0083  t..d..d..d..d(..
-000031d0: 0204 017c 0000 5328 2900 0000 752a 0000  ...|..S()...u*..
-000031e0: 000a 2020 2020 5265 7475 726e 7320 7468  ..    Returns th
-000031f0: 6520 636f 6d6d 616e 6420 6c69 6e65 2070  e command line p
-00003200: 6172 7365 722e 0a20 2020 2074 0b00 0000  arser..    t....
-00003210: 6465 7363 7269 7074 696f 6e75 0200 0000  descriptionu....
-00003220: 2d72 5294 0000 0075 0400 0000 726f 6f74  -rR....u....root
-00003230: 7407 0000 006d 6574 6176 6172 7503 0000  t....metavaru...
-00003240: 0044 4952 7407 0000 0064 6566 6175 6c74  .DIRt....default
-00003250: 7501 0000 002e 7408 0000 0072 6571 7569  u.....t....requi
-00003260: 7265 6474 0400 0000 6865 6c70 7529 0000  redt....helpu)..
-00003270: 0072 6f6f 7420 6469 7265 6374 6f72 7920  .root directory 
-00003280: 666f 7220 7468 6520 7369 7465 2028 2528  for the site (%(
-00003290: 6465 6661 756c 7429 7329 7502 0000 002d  default)s)u....-
-000032a0: 6f75 0600 0000 6f75 7470 7574 7404 0000  ou....outputt...
-000032b0: 0074 7970 6575 0000 0000 752b 0000 0074  .typeu....u+...t
-000032c0: 6865 206f 7574 7075 7420 6469 7265 6374  he output direct
-000032d0: 6f72 7920 666f 7220 7468 6520 6765 6e65  ory for the gene
-000032e0: 7261 7465 6420 7369 7465 7502 0000 002d  rated siteu....-
-000032f0: 6375 0700 0000 636f 6e74 6578 7475 0400  cu....contextu..
-00003300: 0000 4649 4c45 750a 0000 0063 6f6e 7465  ..FILEu....conte
-00003310: 7874 2e70 7975 2700 0000 7468 6520 7079  xt.pyu'...the py
-00003320: 7468 6f6e 206d 6f64 756c 6520 746f 206c  thon module to l
-00003330: 6f61 6420 2825 2864 6566 6175 6c74 2973  oad (%(default)s
-00003340: 2975 0200 0000 2d70 7506 0000 004e 554d  )u....-pu....NUM
-00003350: 4245 5275 0400 0000 706f 7274 6990 1f00  BERu....porti...
-00003360: 0075 2400 0000 7365 7276 6572 2070 6f72  .u$...server por
-00003370: 7420 746f 2062 696e 6420 746f 2028 2528  t to bind to (%(
-00003380: 6465 6661 756c 7429 7329 7502 0000 002d  default)s)u....-
-00003390: 7375 0900 0000 2d2d 6e6f 2d73 6361 6e75  su....--no-scanu
-000033a0: 0700 0000 6e6f 5f73 6361 6e74 0600 0000  ....no_scant....
-000033b0: 6163 7469 6f6e 750a 0000 0073 746f 7265  actionu....store
-000033c0: 5f74 7275 6575 3000 0000 7475 726e 206f  _trueu0...turn o
-000033d0: 6666 2066 696c 6520 7363 616e 206f 6e20  ff file scan on 
-000033e0: 6561 6368 2072 6571 7565 7374 2028 2528  each request (%(
-000033f0: 6465 6661 756c 7429 7329 7502 0000 002d  default)s)u....-
-00003400: 6e75 0900 0000 2d2d 6e6f 2d74 696d 6575  nu....--no-timeu
-00003410: 0700 0000 6e6f 5f74 696d 6575 2400 0000  ....no_timeu$...
-00003420: 6279 7061 7373 2074 696d 6573 7461 6d70  bypass timestamp
-00003430: 2063 6865 636b 2028 2528 6465 6661 756c   check (%(defaul
-00003440: 7429 7329 7502 0000 002d 7675 0900 0000  t)s)u....-vu....
-00003450: 2d2d 7665 7262 6f73 6575 0700 0000 7665  --verboseu....ve
-00003460: 7262 6f73 6575 2700 0000 696e 6372 6561  rboseu'...increa
-00003470: 7365 206c 6f67 6765 7220 7665 7262 6f73  se logger verbos
-00003480: 6974 7920 2825 2864 6566 6175 6c74 2973  ity (%(default)s
-00003490: 2928 0800 0000 7408 0000 0061 7267 7061  )(....t....argpa
-000034a0: 7273 6574 0e00 0000 4172 6775 6d65 6e74  rset....Argument
-000034b0: 5061 7273 6572 740b 0000 0044 4553 4352  Parsert....DESCR
-000034c0: 4950 5449 4f4e 740c 0000 0061 6464 5f61  IPTIONt....add_a
-000034d0: 7267 756d 656e 7452 3d00 0000 52a8 0000  rgumentR=...R...
-000034e0: 0052 4300 0000 7403 0000 0069 6e74 2801  .RC...t....int(.
-000034f0: 0000 0052 ae00 0000 2800 0000 0028 0000  ...R....(....(..
-00003500: 0000 7332 0000 002f 5573 6572 732f 6961  ..s2.../Users/ia
-00003510: 6c62 6572 742f 6170 702f 7079 626c 7565  lbert/app/pyblue
-00003520: 2d63 656e 7472 616c 2f70 7962 6c75 652f  -central/pyblue/
-00003530: 656e 6769 6e65 2e70 7974 0a00 0000 6765  engine.pyt....ge
-00003540: 745f 7061 7273 6572 7501 0000 7322 0000  t_parseru...s"..
-00003550: 0000 0412 0224 0107 022a 0107 0224 0106  .....$...*...$..
-00003560: 0107 0224 0107 0221 0107 0221 0107 0221  ...$...!...!...!
-00003570: 0107 0263 0000 0000 0500 0000 0500 0000  ...c............
-00003580: 4360 0300 73bf 0000 0074 0000 8300 007d  C`..s....t.....}
-00003590: 0000 7401 0074 0200 6a03 0083 0100 6401  ..t..t..j.....d.
-000035a0: 006b 0000 7231 0074 0200 6a03 006a 0400  .k..r1.t..j..j..
-000035b0: 6402 0083 0100 016e 0000 7c00 006a 0500  d......n..|..j..
-000035c0: 8300 007d 0100 7c01 006a 0600 724f 0074  ...}..|..j..rO.t
-000035d0: 0700 6a08 006e 0600 7407 006a 0900 7d02  ..j..n..t..j..}.
-000035e0: 0064 0300 7d03 0074 0700 6a0a 0064 0400  .d..}..t..j..d..
-000035f0: 7c03 0064 0500 7c02 0083 0002 0174 0b00  |..d..|......t..
-00003600: 6406 007c 0100 6a0c 0064 0700 7c01 0083  d..|..j..d..|...
-00003610: 0002 7d04 007c 0100 6a0d 0072 a800 7c04  ..}..|..j..r..|.
-00003620: 006a 0e00 7c01 006a 0d00 8301 0001 6e13  .j..|..j......n.
-00003630: 007c 0400 6a0f 0064 0800 7c01 006a 1000  .|..j..d..|..j..
-00003640: 8300 0101 6400 0053 2809 0000 004e 6903  ....d..S(....Ni.
-00003650: 0000 0075 0600 0000 2d2d 6865 6c70 7526  ...u....--helpu&
-00003660: 0000 0025 286c 6576 656c 6e61 6d65 2973  ...%(levelname)s
-00003670: 0925 2866 756e 634e 616d 6529 7309 2528  .%(funcName)s.%(
-00003680: 6d65 7373 6167 6529 7352 2f00 0000 7405  message)sR/...t.
-00003690: 0000 006c 6576 656c 5211 0000 0052 0e00  ...levelR....R..
-000036a0: 0000 5238 0000 0028 1100 0000 52bc 0000  ..R8...(....R...
-000036b0: 0052 4500 0000 5256 0000 0074 0400 0000  .RE...RV...t....
-000036c0: 6172 6776 524e 0000 0074 0a00 0000 7061  argvRN...t....pa
-000036d0: 7273 655f 6172 6773 7407 0000 0076 6572  rse_argst....ver
-000036e0: 626f 7365 7407 0000 006c 6f67 6769 6e67  boset....logging
-000036f0: 5259 0000 0074 0400 0000 494e 464f 740b  RY...t....INFOt.
-00003700: 0000 0062 6173 6963 436f 6e66 6967 520f  ...basicConfigR.
-00003710: 0000 0052 1100 0000 5246 0000 0052 4800  ...R....RF...RH.
-00003720: 0000 523c 0000 0052 3800 0000 2805 0000  ..R<...R8...(...
-00003730: 0052 ae00 0000 520e 0000 0052 bd00 0000  .R....R....R....
-00003740: 522f 0000 0074 0200 0000 7062 2800 0000  R/...t....pb(...
-00003750: 0028 0000 0000 7332 0000 002f 5573 6572  .(....s2.../User
-00003760: 732f 6961 6c62 6572 742f 6170 702f 7079  s/ialbert/app/py
-00003770: 626c 7565 2d63 656e 7472 616c 2f70 7962  blue-central/pyb
-00003780: 6c75 652f 656e 6769 6e65 2e70 7974 0300  lue/engine.pyt..
-00003790: 0000 7275 6e94 0100 0073 1600 0000 0002  ..run....s......
-000037a0: 0903 1501 1303 0c03 1b01 0601 1602 1802  ................
-000037b0: 0901 1302 7508 0000 005f 5f6d 6169 6e5f  ....u....__main_
-000037c0: 5f28 2d00 0000 529d 0000 0074 0a00 0000  _(-...R....t....
-000037d0: 5f5f 6675 7475 7265 5f5f 5200 0000 0052  __future__R....R
-000037e0: 0100 0000 5202 0000 0052 0300 0000 52b7  ....R....R....R.
-000037f0: 0000 0052 5600 0000 5289 0000 0052 a500  ...RV...R....R..
-00003800: 0000 529f 0000 0052 9200 0000 520a 0000  ..R....R....R...
-00003810: 0052 c100 0000 5279 0000 0052 2c00 0000  .R....Ry...R,...
-00003820: 525f 0000 0052 1d00 0000 7406 0000 0073  R_...R....t....s
-00003830: 7472 696e 6752 0400 0000 5265 0000 0074  tringR....Re...t
-00003840: 0b00 0000 646a 616e 676f 2e63 6f6e 6652  ....django.confR
-00003850: 0500 0000 740f 0000 0064 6a61 6e67 6f2e  ....t....django.
-00003860: 7465 6d70 6c61 7465 5206 0000 0074 1f00  templateR....t..
-00003870: 0000 646a 616e 676f 2e74 656d 706c 6174  ..django.templat
-00003880: 652e 6261 636b 656e 6473 2e64 6a61 6e67  e.backends.djang
-00003890: 6f52 0700 0000 7416 0000 0064 6a61 6e67  oR....t....djang
-000038a0: 6f2e 7465 6d70 6c61 7465 2e6c 6f61 6465  o.template.loade
-000038b0: 7252 0800 0000 740a 0000 005f 5f61 7574  rR....t....__aut
-000038c0: 686f 725f 5f74 0600 0000 7079 626c 7565  hor__t....pyblue
-000038d0: 5209 0000 0052 b900 0000 7409 0000 0067  R....R....t....g
-000038e0: 6574 4c6f 6767 6572 5217 0000 0052 0d00  etLoggerR....R..
-000038f0: 0000 7406 0000 006f 626a 6563 7452 0f00  ..t....objectR..
-00003900: 0000 5272 0000 0052 1900 0000 5284 0000  ..Rr...R....R...
-00003910: 0052 af00 0000 52bc 0000 0052 c500 0000  .R....R....R....
-00003920: 526d 0000 0028 0000 0000 2800 0000 0028  Rm...(....(....(
-00003930: 0000 0000 7332 0000 002f 5573 6572 732f  ....s2.../Users/
-00003940: 6961 6c62 6572 742f 6170 702f 7079 626c  ialbert/app/pybl
-00003950: 7565 2d63 656e 7472 616c 2f70 7962 6c75  ue-central/pyblu
-00003960: 652f 656e 6769 6e65 2e70 7974 0800 0000  e/engine.pyt....
-00003970: 3c6d 6f64 756c 653e 0300 0000 732e 0000  <module>....s...
-00003980: 0006 0222 0184 0118 0110 010c 0110 0110  ..."............
-00003990: 0110 0110 0206 0210 020a 020f 0309 0516  ................
-000039a0: ab09 0816 8609 1909 0609 1f09 180c 01    ...............
+00002360: 005c 0200 7d04 007d 0500 7c00 006a 0400  .\..}..}..|..j..
+00002370: 733d 007c 0300 537c 0400 6a05 0083 0000  s=.|..S|..j.....
+00002380: 6a06 0064 0100 6402 0083 0200 6a06 0064  j..d..d.....j..d
+00002390: 0300 6402 0083 0200 7d06 007c 0600 5328  ..d.....}..|..S(
+000023a0: 0400 0000 757a 0000 000a 2020 2020 2020  ....uz....      
+000023b0: 2020 4174 7465 6d70 7473 2074 6f20 6765    Attempts to ge
+000023c0: 6e65 7261 7465 2061 206e 6963 6572 206e  nerate a nicer n
+000023d0: 616d 6520 6672 6f6d 2074 6865 2066 696c  ame from the fil
+000023e0: 656e 616d 652e 0a20 2020 2020 2020 2052  ename..        R
+000023f0: 656d 6f76 6573 2075 6e64 6572 7363 6f72  emoves underscor
+00002400: 6573 2c20 6461 7368 6573 2061 6e64 2065  es, dashes and e
+00002410: 7874 656e 7369 6f6e 732e 0a20 2020 2020  xtensions..     
+00002420: 2020 2075 0100 0000 2d75 0100 0000 2075     u....-u.... u
+00002430: 0100 0000 5f28 0700 0000 520a 0000 0052  ...._(....R....R
+00002440: 0b00 0000 525e 0000 0052 4b00 0000 521a  ....R^...RK...R.
+00002450: 0000 0052 7300 0000 7407 0000 0072 6570  ...Rs...t....rep
+00002460: 6c61 6365 2807 0000 0052 2300 0000 5210  lace(....R#...R.
+00002470: 0000 0074 0400 0000 6865 6164 7404 0000  ...t....headt...
+00002480: 0074 6169 6c52 6a00 0000 5254 0000 0052  .tailRj...RT...R
+00002490: 5200 0000 2800 0000 0028 0000 0000 7332  R...(....(....s2
+000024a0: 0000 002f 5573 6572 732f 6961 6c62 6572  .../Users/ialber
+000024b0: 742f 6170 702f 7079 626c 7565 2d63 656e  t/app/pyblue-cen
+000024c0: 7472 616c 2f70 7962 6c75 652f 656e 6769  tral/pyblue/engi
+000024d0: 6e65 2e70 7952 8300 0000 1401 0000 730c  ne.pyR........s.
+000024e0: 0000 0000 0518 0118 0309 0104 0224 0175  .............$.u
+000024f0: 0000 0000 6304 0000 0007 0000 0006 0000  ....c...........
+00002500: 0043 6003 0073 3501 0000 7400 006a 0100  .C`..s5...t..j..
+00002510: 6a02 007c 0100 7c00 006a 0300 8302 007d  j..|..|..j.....}
+00002520: 0400 7400 006a 0100 6a04 007c 0400 8301  ..t..j..j..|....
+00002530: 0074 0000 6a01 006a 0400 7c00 006a 0100  .t..j..j..|..j..
+00002540: 8301 006b 0200 7252 0074 0500 6401 007c  ...k..rR.t..d..|
+00002550: 0400 1683 0100 8201 006e 0000 7c03 0072  .........n..|..r
+00002560: 8800 7406 007c 0400 8301 0074 0600 7c00  ..t..|.....t..|.
+00002570: 006a 0100 8301 006b 0400 7288 0074 0700  .j.....k..r..t..
+00002580: 6a08 0064 0200 7c04 0016 8301 0001 6403  j..d..|.......d.
+00002590: 0053 7400 006a 0100 6a09 007c 0400 8301  .St..j..j..|....
+000025a0: 007d 0500 7400 006a 0100 6a0a 007c 0500  .}..t..j..j..|..
+000025b0: 8301 0073 bc00 7400 006a 0b00 7c05 0083  ...s..t..j..|...
+000025c0: 0100 016e 0000 7c00 006a 0c00 720d 017c  ...n..|..j..r..|
+000025d0: 0200 720d 0174 0700 6a0d 0064 0400 7c04  ..r..t..j..d..|.
+000025e0: 0016 8301 0001 740e 006a 0f00 7c04 0064  ......t..j..|..d
+000025f0: 0500 6406 0064 0700 8302 018f 1400 7d06  ..d..d........}.
+00002600: 007c 0600 6a10 007c 0200 8301 0001 5764  .|..j..|......Wd
+00002610: 0300 5158 6e24 0074 0700 6a0d 0064 0800  ..QXn$.t..j..d..
+00002620: 7c04 0016 8301 0001 7411 006a 1200 7c00  |.......t..j..|.
+00002630: 006a 0100 7c04 0083 0200 0164 0300 5328  .j..|......d..S(
+00002640: 0900 0000 7537 0000 000a 2020 2020 2020  ....u7....      
+00002650: 2020 5772 6974 6573 2074 6865 2074 6578    Writes the tex
+00002660: 7420 696e 746f 2061 6e20 6f75 7470 7574  t into an output
+00002670: 2066 6f6c 6465 720a 2020 2020 2020 2020   folder.        
+00002680: 752a 0000 0063 616e 6e6f 7420 6e6f 7420  u*...cannot not 
+00002690: 6f76 6572 7772 6974 6520 7468 6520 6f72  overwrite the or
+000026a0: 6967 696e 616c 2066 696c 653a 2025 7375  iginal file: %su
+000026b0: 0800 0000 736b 6970 3a20 2573 4e75 0a00  ....skip: %sNu..
+000026c0: 0000 7361 7669 6e67 3a20 2573 7502 0000  ..saving: %su...
+000026d0: 0077 7452 8800 0000 7505 0000 0075 7466  .wtR....u....utf
+000026e0: 2d38 750b 0000 0063 6f70 7969 6e67 3a20  -8u....copying: 
+000026f0: 2573 2813 0000 0052 0a00 0000 520b 0000  %s(....R....R...
+00002700: 0052 0d00 0000 5210 0000 0052 0c00 0000  .R....R....R....
+00002710: 5230 0000 0052 7200 0000 5217 0000 0052  R0...Rr...R....R
+00002720: 1800 0000 5262 0000 0074 0600 0000 6578  ....Rb...t....ex
+00002730: 6973 7473 7408 0000 006d 616b 6564 6972  istst....makedir
+00002740: 7352 1a00 0000 523b 0000 0052 8900 0000  sR....R;...R....
+00002750: 528a 0000 0052 4400 0000 7406 0000 0073  R....RD...t....s
+00002760: 6875 7469 6c74 0800 0000 636f 7079 6669  hutilt....copyfi
+00002770: 6c65 2807 0000 0052 2300 0000 5246 0000  le(....R#...RF..
+00002780: 0052 3e00 0000 523f 0000 0074 0400 0000  .R>...R?...t....
+00002790: 6465 7374 7405 0000 0064 7061 7468 7402  destt....dpatht.
+000027a0: 0000 0066 7028 0000 0000 2800 0000 0073  ...fp(....(....s
+000027b0: 3200 0000 2f55 7365 7273 2f69 616c 6265  2.../Users/ialbe
+000027c0: 7274 2f61 7070 2f70 7962 6c75 652d 6365  rt/app/pyblue-ce
+000027d0: 6e74 7261 6c2f 7079 626c 7565 2f65 6e67  ntral/pyblue/eng
+000027e0: 696e 652e 7079 5244 0000 0023 0100 0073  ine.pyRD...#...s
+000027f0: 1e00 0000 0004 1803 2701 1303 2101 1101  ........'...!...
+00002800: 0403 1201 1201 1003 0f01 1101 1b01 1602  ................
+00002810: 1101 6302 0000 0003 0000 0003 0000 0043  ..c............C
+00002820: 6003 0073 4300 0000 7c01 0070 0900 7c00  `..sC...|..p..|.
+00002830: 007d 0100 7400 006a 0100 6a02 007c 0000  .}..t..j..j..|..
+00002840: 6a03 007c 0100 6a04 0083 0200 7d02 0074  j..|..j.....}..t
+00002850: 0000 6a01 006a 0500 7c02 007c 0000 6a06  ..j..j..|..|..j.
+00002860: 0083 0200 7d02 007c 0200 5328 0100 0000  ....}..|..S(....
+00002870: 7542 0000 000a 2020 2020 2020 2020 5265  uB....        Re
+00002880: 6c61 7469 7665 2070 6174 6820 6f66 2074  lative path of t
+00002890: 6869 7320 6669 6c65 2066 726f 6d20 6120  his file from a 
+000028a0: 7374 6172 7420 6c6f 6361 7469 6f6e 0a20  start location. 
+000028b0: 2020 2020 2020 2028 0700 0000 520a 0000         (....R...
+000028c0: 0052 0b00 0000 524d 0000 0052 1100 0000  .R....RM...R....
+000028d0: 527d 0000 0052 0d00 0000 5210 0000 0028  R}...R....R....(
+000028e0: 0300 0000 5223 0000 0052 5300 0000 7405  ....R#...RS...t.
+000028f0: 0000 0072 7061 7468 2800 0000 0028 0000  ...rpath(....(..
+00002900: 0000 7332 0000 002f 5573 6572 732f 6961  ..s2.../Users/ia
+00002910: 6c62 6572 742f 6170 702f 7079 626c 7565  lbert/app/pyblue
+00002920: 2d63 656e 7472 616c 2f70 7962 6c75 652f  -central/pyblue/
+00002930: 656e 6769 6e65 2e70 7952 4d00 0000 4001  engine.pyRM...@.
+00002940: 0000 7308 0000 0000 040c 011b 0118 0163  ..s............c
+00002950: 0200 0000 0300 0000 0300 0000 4360 0300  ............C`..
+00002960: 7319 0000 007c 0000 6a00 006a 0100 7c01  s....|..j..j..|.
+00002970: 0064 0100 8302 007d 0200 7c02 0053 2802  .d.....}..|..S(.
+00002980: 0000 0075 9100 0000 0a20 2020 2020 2020  ...u.....       
+00002990: 204d 6574 6164 6174 6120 6d61 7920 6265   Metadata may be
+000029a0: 2061 6363 6573 7365 6420 6173 2061 6e20   accessed as an 
+000029b0: 6174 7472 6962 7574 6573 206f 6e20 7468  attributes on th
+000029c0: 6520 636c 6173 732e 0a20 2020 2020 2020  e class..       
+000029d0: 2054 6869 7320 6765 7473 2074 7269 6767   This gets trigg
+000029e0: 6572 6564 2061 7320 6120 6661 6c6c 6261  ered as a fallba
+000029f0: 636b 2069 6620 616e 2061 7474 7269 6275  ck if an attribu
+00002a00: 7465 2069 7320 6e6f 7420 666f 756e 642e  te is not found.
+00002a10: 0a20 2020 2020 2020 204e 2803 0000 0052  .        N(....R
+00002a20: 7500 0000 7403 0000 0067 6574 5229 0000  u...t....getR)..
+00002a30: 0028 0300 0000 5223 0000 0052 5200 0000  .(....R#...RR...
+00002a40: 7405 0000 0076 616c 7565 2800 0000 0028  t....value(....(
+00002a50: 0000 0000 7332 0000 002f 5573 6572 732f  ....s2.../Users/
+00002a60: 6961 6c62 6572 742f 6170 702f 7079 626c  ialbert/app/pybl
+00002a70: 7565 2d63 656e 7472 616c 2f70 7962 6c75  ue-central/pyblu
+00002a80: 652f 656e 6769 6e65 2e70 7974 0b00 0000  e/engine.pyt....
+00002a90: 5f5f 6765 7461 7474 725f 5f49 0100 0073  __getattr__I...s
+00002aa0: 0400 0000 0005 1501 6301 0000 0001 0000  ........c.......
+00002ab0: 0004 0000 0043 6003 0073 1d00 0000 6401  .....C`..s....d.
+00002ac0: 007c 0000 6a00 006a 0100 7c00 006a 0200  .|..j..j..|..j..
+00002ad0: 7c00 006a 0300 6603 0016 5328 0200 0000  |..j..f...S(....
+00002ae0: 752e 0000 000a 2020 2020 2020 2020 5573  u.....        Us
+00002af0: 6572 2066 7269 656e 646c 7920 7265 7072  er friendly repr
+00002b00: 6573 656e 7461 7469 6f6e 0a20 2020 2020  esentation.     
+00002b10: 2020 2075 0b00 0000 2573 3a20 2573 2028     u....%s: %s (
+00002b20: 2573 2928 0400 0000 7409 0000 005f 5f63  %s)(....t....__c
+00002b30: 6c61 7373 5f5f 526d 0000 0052 5200 0000  lass__Rm...RR...
+00002b40: 5210 0000 0028 0100 0000 5223 0000 0028  R....(....R#...(
+00002b50: 0000 0000 2800 0000 0073 3200 0000 2f55  ....(....s2.../U
+00002b60: 7365 7273 2f69 616c 6265 7274 2f61 7070  sers/ialbert/app
+00002b70: 2f70 7962 6c75 652d 6365 6e74 7261 6c2f  /pyblue-central/
+00002b80: 7079 626c 7565 2f65 6e67 696e 652e 7079  pyblue/engine.py
+00002b90: 7408 0000 005f 5f72 6570 725f 5f51 0100  t....__repr__Q..
+00002ba0: 0073 0200 0000 0004 4e28 1000 0000 526d  .s......N(....Rm
+00002bb0: 0000 0052 6e00 0000 7407 0000 005f 5f64  ...Rn...t....__d
+00002bc0: 6f63 5f5f 527e 0000 0052 7f00 0000 5281  oc__R~...R....R.
+00002bd0: 0000 0052 3600 0000 7408 0000 0070 726f  ...R6...t....pro
+00002be0: 7065 7274 7952 3e00 0000 5283 0000 0052  pertyR>...R....R
+00002bf0: 3d00 0000 5244 0000 0052 2900 0000 524d  =...RD...R)...RM
+00002c00: 0000 0052 9a00 0000 529c 0000 0028 0000  ...R....R....(..
+00002c10: 0000 2800 0000 0028 0000 0000 7332 0000  ..(....(....s2..
+00002c20: 002f 5573 6572 732f 6961 6c62 6572 742f  ./Users/ialbert/
+00002c30: 6170 702f 7079 626c 7565 2d63 656e 7472  app/pyblue-centr
+00002c40: 616c 2f70 7962 6c75 652f 656e 6769 6e65  al/pyblue/engine
+00002c50: 2e70 7952 1900 0000 d000 0000 7316 0000  .pyR........s...
+00002c60: 0006 0306 020c 0115 0109 0209 310f 0a09  ............1...
+00002c70: 0f0f 1d0c 0909 0863 0100 0000 0a00 0000  .......c........
+00002c80: 0600 0000 4360 0300 73d7 0000 0074 0000  ....C`..s....t..
+00002c90: 6a01 0064 0100 8301 007d 0100 7402 006a  j..d.....}..t..j
+00002ca0: 0300 7c00 0064 0200 6403 0083 0101 6a04  ..|..d..d.....j.
+00002cb0: 0083 0000 6a05 0083 0000 6404 0020 7d02  ....j.....d.. }.
+00002cc0: 0074 0600 7407 007c 0200 8302 007d 0200  .t..t..|.....}..
+00002cd0: 7408 0083 0000 7d03 0078 8400 7c02 0044  t.....}..x..|..D
+00002ce0: 5d7c 007d 0400 7c01 006a 0900 7c04 0083  ]|.}..|..j..|...
+00002cf0: 0100 7d05 007c 0500 7253 007c 0500 6a0a  ..}..|..rS.|..j.
+00002d00: 0064 0500 8301 007c 0500 6a0a 0064 0600  .d.....|..j..d..
+00002d10: 8301 0002 7d06 007d 0700 7913 0074 0b00  ....}..}..y..t..
+00002d20: 6a0c 007c 0700 8301 007d 0800 576e 1f00  j..|.....}..Wn..
+00002d30: 0474 0d00 6b0a 0072 c100 017d 0900 0174  .t..k..r...}...t
+00002d40: 0e00 7c07 0083 0100 7d08 006e 0100 587c  ..|.....}..n..X|
+00002d50: 0800 7c03 007c 0600 3c71 5300 7153 0057  ..|..|..<qS.qS.W
+00002d60: 7c03 0053 2807 0000 0075 8e00 0000 0a20  |..S(....u..... 
+00002d70: 2020 2041 7474 656d 7074 7320 746f 2070     Attempts to p
+00002d80: 6172 7365 206f 7574 206d 6574 6164 6174  arse out metadat
+00002d90: 6120 6672 6f6d 2064 6a61 6e67 6f20 636f  a from django co
+00002da0: 6d6d 656e 7473 2e0a 2020 2020 4561 6368  mments..    Each
+00002db0: 2063 6f6d 6d65 6e74 2069 7320 6173 7375   comment is assu
+00002dc0: 6d65 6420 746f 2062 6520 6b65 7920 3d20  med to be key = 
+00002dd0: 7661 6c75 6520 7768 6572 6520 7468 6520  value where the 
+00002de0: 7661 6c75 6520 6973 2061 204a 534f 4e20  value is a JSON 
+00002df0: 6f62 6a65 6374 2e0a 2020 2020 7531 0000  object..    u1..
+00002e00: 005e 7b23 5c73 3f28 3f50 3c6e 616d 653e  .^{#\s?(?P<name>
+00002e10: 5c77 2b29 5c73 3f3d 5c73 3f28 3f50 3c76  \w+)\s?=\s?(?P<v
+00002e20: 616c 7565 3e5b 5c53 5c73 5d2b 295c 733f  alue>[\S\s]+)\s?
+00002e30: 237d 5288 0000 0075 0500 0000 7574 662d  #}R....u....utf-
+00002e40: 3869 6400 0000 7504 0000 006e 616d 6575  8id...u....nameu
+00002e50: 0500 0000 7661 6c75 6528 0f00 0000 7402  ....value(....t.
+00002e60: 0000 0072 6574 0700 0000 636f 6d70 696c  ...ret....compil
+00002e70: 6552 8900 0000 528a 0000 0052 8b00 0000  eR....R....R....
+00002e80: 740a 0000 0073 706c 6974 6c69 6e65 7374  t....splitlinest
+00002e90: 0300 0000 6d61 7052 0400 0000 521b 0000  ....mapR....R...
+00002ea0: 0074 0600 0000 7365 6172 6368 7405 0000  .t....searcht...
+00002eb0: 0067 726f 7570 7404 0000 006a 736f 6e74  .groupt....jsont
+00002ec0: 0500 0000 6c6f 6164 7374 0a00 0000 5661  ....loadst....Va
+00002ed0: 6c75 6545 7272 6f72 7403 0000 0073 7472  lueErrort....str
+00002ee0: 280a 0000 0052 0b00 0000 7407 0000 0050  (....R....t....P
+00002ef0: 4154 5445 524e 7405 0000 006c 696e 6573  ATTERNt....lines
+00002f00: 5275 0000 0074 0400 0000 6c69 6e65 7401  Ru...t....linet.
+00002f10: 0000 006d 5252 0000 0052 9900 0000 7403  ...mRR...R....t.
+00002f20: 0000 006f 626a 5235 0000 0028 0000 0000  ...objR5...(....
+00002f30: 2800 0000 0073 3200 0000 2f55 7365 7273  (....s2.../Users
+00002f40: 2f69 616c 6265 7274 2f61 7070 2f70 7962  /ialbert/app/pyb
+00002f50: 6c75 652d 6365 6e74 7261 6c2f 7079 626c  lue-central/pybl
+00002f60: 7565 2f65 6e67 696e 652e 7079 5284 0000  ue/engine.pyR...
+00002f70: 0058 0100 0073 1c00 0000 0006 0f03 2501  .X...s........%.
+00002f80: 0f01 0901 0d01 0f01 0601 1f01 0301 1301  ................
+00002f90: 0f01 1001 1102 6301 0000 0001 0000 0001  ......c.........
+00002fa0: 0000 0043 6003 0073 0400 0000 6401 0053  ...C`..s....d..S
+00002fb0: 2802 0000 0075 3700 0000 0a20 2020 2041  (....u7....    A
+00002fc0: 6464 7320 7468 6520 636f 6d6d 6f6e 2070  dds the common p
+00002fd0: 6172 616d 6574 6572 7320 746f 2065 6163  arameters to eac
+00002fe0: 6820 7375 6270 6172 7365 722e 0a20 2020  h subparser..   
+00002ff0: 204e 2800 0000 0028 0100 0000 7406 0000   N(....(....t...
+00003000: 0070 6172 7365 7228 0000 0000 2800 0000  .parser(....(...
+00003010: 0073 3200 0000 2f55 7365 7273 2f69 616c  .s2.../Users/ial
+00003020: 6265 7274 2f61 7070 2f70 7962 6c75 652d  bert/app/pyblue-
+00003030: 6365 6e74 7261 6c2f 7079 626c 7565 2f65  central/pyblue/e
+00003040: 6e67 696e 652e 7079 7414 0000 0061 6464  ngine.pyt....add
+00003050: 5f63 6f6d 6d6f 6e5f 6172 6775 6d65 6e74  _common_argument
+00003060: 7371 0100 0073 0000 0000 6300 0000 0001  sq...s....c.....
+00003070: 0000 000e 0000 0043 6003 0073 4601 0000  .......C`..sF...
+00003080: 7400 006a 0100 6401 0074 0200 8300 017d  t..j..d..t.....}
+00003090: 0000 7c00 006a 0300 6402 0064 0300 6404  ..|..j..d..d..d.
+000030a0: 0064 0500 6406 0064 0700 6408 0064 0900  .d..d..d..d..d..
+000030b0: 7404 0064 0a00 640b 0083 0105 017c 0000  t..d..d......|..
+000030c0: 6a03 0064 0c00 6403 0064 0d00 6405 0064  j..d..d..d..d..d
+000030d0: 0600 640e 0074 0500 6409 0074 0600 6407  ..d..t..d..t..d.
+000030e0: 0064 0f00 640a 0064 1000 8301 0601 7c00  .d..d..d......|.
+000030f0: 006a 0300 6411 0064 0300 6412 0064 0500  .j..d..d..d..d..
+00003100: 6413 0064 0e00 7405 0064 0900 7406 0064  d..d..t..d..t..d
+00003110: 0700 6414 0064 0a00 6415 0083 0106 017c  ..d..d..d......|
+00003120: 0000 6a03 0064 1600 6405 0064 1700 640e  ..j..d..d..d..d.
+00003130: 0074 0700 6403 0064 1800 6407 0064 1900  .t..d..d..d..d..
+00003140: 640a 0064 1a00 8301 0501 7c00 006a 0300  d..d......|..j..
+00003150: 641b 0064 1c00 6403 0064 1d00 6407 0074  d..d..d..d..d..t
+00003160: 0600 641e 0064 1f00 640a 0064 2000 8302  ..d..d..d..d ...
+00003170: 0401 7c00 006a 0300 6421 0064 2200 6403  ..|..j..d!.d".d.
+00003180: 0064 2300 6407 0074 0600 641e 0064 1f00  .d#.d..t..d..d..
+00003190: 640a 0064 2400 8302 0401 7c00 006a 0300  d..d$.....|..j..
+000031a0: 6425 0064 2600 6403 0064 2700 6407 0074  d%.d&.d..d'.d..t
+000031b0: 0600 641e 0064 1f00 640a 0064 2800 8302  ..d..d..d..d(...
+000031c0: 0401 7c00 0053 2829 0000 0075 2a00 0000  ..|..S()...u*...
+000031d0: 0a20 2020 2052 6574 7572 6e73 2074 6865  .    Returns the
+000031e0: 2063 6f6d 6d61 6e64 206c 696e 6520 7061   command line pa
+000031f0: 7273 6572 2e0a 2020 2020 740b 0000 0064  rser..    t....d
+00003200: 6573 6372 6970 7469 6f6e 7502 0000 002d  escriptionu....-
+00003210: 7252 9400 0000 7504 0000 0072 6f6f 7474  rR....u....roott
+00003220: 0700 0000 6d65 7461 7661 7275 0300 0000  ....metavaru....
+00003230: 4449 5274 0700 0000 6465 6661 756c 7475  DIRt....defaultu
+00003240: 0100 0000 2e74 0800 0000 7265 7175 6972  .....t....requir
+00003250: 6564 7404 0000 0068 656c 7075 2900 0000  edt....helpu)...
+00003260: 726f 6f74 2064 6972 6563 746f 7279 2066  root directory f
+00003270: 6f72 2074 6865 2073 6974 6520 2825 2864  or the site (%(d
+00003280: 6566 6175 6c74 2973 2975 0200 0000 2d6f  efault)s)u....-o
+00003290: 7506 0000 006f 7574 7075 7474 0400 0000  u....outputt....
+000032a0: 7479 7065 7500 0000 0075 2b00 0000 7468  typeu....u+...th
+000032b0: 6520 6f75 7470 7574 2064 6972 6563 746f  e output directo
+000032c0: 7279 2066 6f72 2074 6865 2067 656e 6572  ry for the gener
+000032d0: 6174 6564 2073 6974 6575 0200 0000 2d63  ated siteu....-c
+000032e0: 7507 0000 0063 6f6e 7465 7874 7504 0000  u....contextu...
+000032f0: 0046 494c 4575 0a00 0000 636f 6e74 6578  .FILEu....contex
+00003300: 742e 7079 7527 0000 0074 6865 2070 7974  t.pyu'...the pyt
+00003310: 686f 6e20 6d6f 6475 6c65 2074 6f20 6c6f  hon module to lo
+00003320: 6164 2028 2528 6465 6661 756c 7429 7329  ad (%(default)s)
+00003330: 7502 0000 002d 7075 0600 0000 4e55 4d42  u....-pu....NUMB
+00003340: 4552 7504 0000 0070 6f72 7469 901f 0000  ERu....porti....
+00003350: 7524 0000 0073 6572 7665 7220 706f 7274  u$...server port
+00003360: 2074 6f20 6269 6e64 2074 6f20 2825 2864   to bind to (%(d
+00003370: 6566 6175 6c74 2973 2975 0200 0000 2d73  efault)s)u....-s
+00003380: 7509 0000 002d 2d6e 6f2d 7363 616e 7507  u....--no-scanu.
+00003390: 0000 006e 6f5f 7363 616e 7406 0000 0061  ...no_scant....a
+000033a0: 6374 696f 6e75 0a00 0000 7374 6f72 655f  ctionu....store_
+000033b0: 7472 7565 7530 0000 0074 7572 6e20 6f66  trueu0...turn of
+000033c0: 6620 6669 6c65 2073 6361 6e20 6f6e 2065  f file scan on e
+000033d0: 6163 6820 7265 7175 6573 7420 2825 2864  ach request (%(d
+000033e0: 6566 6175 6c74 2973 2975 0200 0000 2d6e  efault)s)u....-n
+000033f0: 7509 0000 002d 2d6e 6f2d 7469 6d65 7507  u....--no-timeu.
+00003400: 0000 006e 6f5f 7469 6d65 7524 0000 0062  ...no_timeu$...b
+00003410: 7970 6173 7320 7469 6d65 7374 616d 7020  ypass timestamp 
+00003420: 6368 6563 6b20 2825 2864 6566 6175 6c74  check (%(default
+00003430: 2973 2975 0200 0000 2d76 7509 0000 002d  )s)u....-vu....-
+00003440: 2d76 6572 626f 7365 7507 0000 0076 6572  -verboseu....ver
+00003450: 626f 7365 7527 0000 0069 6e63 7265 6173  boseu'...increas
+00003460: 6520 6c6f 6767 6572 2076 6572 626f 7369  e logger verbosi
+00003470: 7479 2028 2528 6465 6661 756c 7429 7329  ty (%(default)s)
+00003480: 2808 0000 0074 0800 0000 6172 6770 6172  (....t....argpar
+00003490: 7365 740e 0000 0041 7267 756d 656e 7450  set....ArgumentP
+000034a0: 6172 7365 7274 0b00 0000 4445 5343 5249  arsert....DESCRI
+000034b0: 5054 494f 4e74 0c00 0000 6164 645f 6172  PTIONt....add_ar
+000034c0: 6775 6d65 6e74 523d 0000 0052 a800 0000  gumentR=...R....
+000034d0: 5243 0000 0074 0300 0000 696e 7428 0100  RC...t....int(..
+000034e0: 0000 52ae 0000 0028 0000 0000 2800 0000  ..R....(....(...
+000034f0: 0073 3200 0000 2f55 7365 7273 2f69 616c  .s2.../Users/ial
+00003500: 6265 7274 2f61 7070 2f70 7962 6c75 652d  bert/app/pyblue-
+00003510: 6365 6e74 7261 6c2f 7079 626c 7565 2f65  central/pyblue/e
+00003520: 6e67 696e 652e 7079 740a 0000 0067 6574  ngine.pyt....get
+00003530: 5f70 6172 7365 7277 0100 0073 2200 0000  _parserw...s"...
+00003540: 0004 1202 2401 0702 2a01 0702 2401 0601  ....$...*...$...
+00003550: 0702 2401 0702 2101 0702 2101 0702 2101  ..$...!...!...!.
+00003560: 0702 6300 0000 0005 0000 0005 0000 0043  ..c............C
+00003570: 6003 0073 bf00 0000 7400 0083 0000 7d00  `..s....t.....}.
+00003580: 0074 0100 7402 006a 0300 8301 0064 0100  .t..t..j.....d..
+00003590: 6b00 0072 3100 7402 006a 0300 6a04 0064  k..r1.t..j..j..d
+000035a0: 0200 8301 0001 6e00 007c 0000 6a05 0083  ......n..|..j...
+000035b0: 0000 7d01 007c 0100 6a06 0072 4f00 7407  ..}..|..j..rO.t.
+000035c0: 006a 0800 6e06 0074 0700 6a09 007d 0200  .j..n..t..j..}..
+000035d0: 6403 007d 0300 7407 006a 0a00 6404 007c  d..}..t..j..d..|
+000035e0: 0300 6405 007c 0200 8300 0201 740b 0064  ..d..|......t..d
+000035f0: 0600 7c01 006a 0c00 6407 007c 0100 8300  ..|..j..d..|....
+00003600: 027d 0400 7c01 006a 0d00 72a8 007c 0400  .}..|..j..r..|..
+00003610: 6a0e 007c 0100 6a0d 0083 0100 016e 1300  j..|..j......n..
+00003620: 7c04 006a 0f00 6408 007c 0100 6a10 0083  |..j..d..|..j...
+00003630: 0001 0164 0000 5328 0900 0000 4e69 0300  ...d..S(....Ni..
+00003640: 0000 7506 0000 002d 2d68 656c 7075 2600  ..u....--helpu&.
+00003650: 0000 2528 6c65 7665 6c6e 616d 6529 7309  ..%(levelname)s.
+00003660: 2528 6675 6e63 4e61 6d65 2973 0925 286d  %(funcName)s.%(m
+00003670: 6573 7361 6765 2973 522f 0000 0074 0500  essage)sR/...t..
+00003680: 0000 6c65 7665 6c52 1100 0000 520e 0000  ..levelR....R...
+00003690: 0052 3800 0000 2811 0000 0052 bc00 0000  .R8...(....R....
+000036a0: 5245 0000 0052 5600 0000 7404 0000 0061  RE...RV...t....a
+000036b0: 7267 7652 4e00 0000 740a 0000 0070 6172  rgvRN...t....par
+000036c0: 7365 5f61 7267 7374 0700 0000 7665 7262  se_argst....verb
+000036d0: 6f73 6574 0700 0000 6c6f 6767 696e 6752  oset....loggingR
+000036e0: 5900 0000 7404 0000 0049 4e46 4f74 0b00  Y...t....INFOt..
+000036f0: 0000 6261 7369 6343 6f6e 6669 6752 0f00  ..basicConfigR..
+00003700: 0000 5211 0000 0052 4600 0000 5248 0000  ..R....RF...RH..
+00003710: 0052 3c00 0000 5238 0000 0028 0500 0000  .R<...R8...(....
+00003720: 52ae 0000 0052 0e00 0000 52bd 0000 0052  R....R....R....R
+00003730: 2f00 0000 7402 0000 0070 6228 0000 0000  /...t....pb(....
+00003740: 2800 0000 0073 3200 0000 2f55 7365 7273  (....s2.../Users
+00003750: 2f69 616c 6265 7274 2f61 7070 2f70 7962  /ialbert/app/pyb
+00003760: 6c75 652d 6365 6e74 7261 6c2f 7079 626c  lue-central/pybl
+00003770: 7565 2f65 6e67 696e 652e 7079 7403 0000  ue/engine.pyt...
+00003780: 0072 756e 9601 0000 7316 0000 0000 0209  .run....s.......
+00003790: 0315 0113 030c 031b 0106 0116 0218 0209  ................
+000037a0: 0113 0275 0800 0000 5f5f 6d61 696e 5f5f  ...u....__main__
+000037b0: 282d 0000 0052 9d00 0000 740a 0000 005f  (-...R....t...._
+000037c0: 5f66 7574 7572 655f 5f52 0000 0000 5201  _future__R....R.
+000037d0: 0000 0052 0200 0000 5203 0000 0052 b700  ...R....R....R..
+000037e0: 0000 5256 0000 0052 8900 0000 52a5 0000  ..RV...R....R...
+000037f0: 0052 9f00 0000 5292 0000 0052 0a00 0000  .R....R....R....
+00003800: 52c1 0000 0052 7900 0000 522c 0000 0052  R....Ry...R,...R
+00003810: 5f00 0000 521d 0000 0074 0600 0000 7374  _...R....t....st
+00003820: 7269 6e67 5204 0000 0052 6500 0000 740b  ringR....Re...t.
+00003830: 0000 0064 6a61 6e67 6f2e 636f 6e66 5205  ...django.confR.
+00003840: 0000 0074 0f00 0000 646a 616e 676f 2e74  ...t....django.t
+00003850: 656d 706c 6174 6552 0600 0000 741f 0000  emplateR....t...
+00003860: 0064 6a61 6e67 6f2e 7465 6d70 6c61 7465  .django.template
+00003870: 2e62 6163 6b65 6e64 732e 646a 616e 676f  .backends.django
+00003880: 5207 0000 0074 1600 0000 646a 616e 676f  R....t....django
+00003890: 2e74 656d 706c 6174 652e 6c6f 6164 6572  .template.loader
+000038a0: 5208 0000 0074 0a00 0000 5f5f 6175 7468  R....t....__auth
+000038b0: 6f72 5f5f 7406 0000 0070 7962 6c75 6552  or__t....pyblueR
+000038c0: 0900 0000 52b9 0000 0074 0900 0000 6765  ....R....t....ge
+000038d0: 744c 6f67 6765 7252 1700 0000 520d 0000  tLoggerR....R...
+000038e0: 0074 0600 0000 6f62 6a65 6374 520f 0000  .t....objectR...
+000038f0: 0052 7200 0000 5219 0000 0052 8400 0000  .Rr...R....R....
+00003900: 52af 0000 0052 bc00 0000 52c5 0000 0052  R....R....R....R
+00003910: 6d00 0000 2800 0000 0028 0000 0000 2800  m...(....(....(.
+00003920: 0000 0073 3200 0000 2f55 7365 7273 2f69  ...s2.../Users/i
+00003930: 616c 6265 7274 2f61 7070 2f70 7962 6c75  albert/app/pyblu
+00003940: 652d 6365 6e74 7261 6c2f 7079 626c 7565  e-central/pyblue
+00003950: 2f65 6e67 696e 652e 7079 7408 0000 003c  /engine.pyt....<
+00003960: 6d6f 6475 6c65 3e03 0000 0073 2e00 0000  module>....s....
+00003970: 0602 2201 8401 1801 1001 0c01 1001 1001  ..".............
+00003980: 1001 1002 0602 1002 0a02 0f03 0905 16ab  ................
+00003990: 0908 1688 0919 0906 091f 0918 0c01       ..............
```

### Comparing `pyblue-3.0.2/pyblue/pyblue3.pyc` & `pyblue-3.0.3/pyblue/pyblue3.pyc`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/pyblue/templatetags/pytags.py` & `pyblue-3.0.3/pyblue/templatetags/pytags.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 @register.simple_tag(takes_context=True)
 def img(context, pattern, css='', attrs={}):
     obj, relpath, name = match_file(context=context, pattern=pattern)
     extras = render_attrs(attrs)
     html = '<img src="{}" class="{}" alt="{}" {}>'.format(relpath, css, name, extras)
-    return html
+    return mark_safe(html)
 
 @register.inclusion_tag('say_hello.html')
 def say_hello():
     return dict()
 
 
 @register.inclusion_tag('thumbnail.html', takes_context=True)
```

### Comparing `pyblue-3.0.2/pyblue/templatetags/pytags.pyc` & `pyblue-3.0.3/pyblue/templatetags/pytags.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a b241 0d57 6300 0000 0000 0000  .....A.Wc.......
+00000000: 03f3 0d0a 0664 0e57 6300 0000 0000 0000  .....d.Wc.......
 00000010: 0006 0000 0040 6003 0073 0402 0000 6400  .....@`..s....d.
 00000020: 0064 0100 6c00 006d 0100 5a01 006d 0200  .d..l..m..Z..m..
 00000030: 5a02 006d 0300 5a03 006d 0400 5a04 0001  Z..m..Z..m..Z...
 00000040: 6400 0064 0200 6c05 006d 0600 5a06 0001  d..d..l..m..Z...
 00000050: 6400 0064 0300 6c07 005a 0700 6400 0064  d..d..l..Z..d..d
 00000060: 0300 6c08 005a 0800 6400 0064 0300 6c09  ..l..Z..d..d..l.
 00000070: 005a 0900 6400 0064 0300 6c0a 005a 0a00  .Z..d..d..l..Z..
@@ -170,273 +170,273 @@
 00000a90: 0000 2800 0000 0073 3f00 0000 2f55 7365  ..(....s?.../Use
 00000aa0: 7273 2f69 616c 6265 7274 2f61 7070 2f70  rs/ialbert/app/p
 00000ab0: 7962 6c75 652d 6365 6e74 7261 6c2f 7079  yblue-central/py
 00000ac0: 626c 7565 2f74 656d 706c 6174 6574 6167  blue/templatetag
 00000ad0: 732f 7079 7461 6773 2e70 7974 0400 0000  s/pytags.pyt....
 00000ae0: 6669 6e64 3900 0000 730a 0000 0000 031e  find9...s.......
 00000af0: 0106 0118 0206 0175 0000 0000 6304 0000  .......u....c...
-00000b00: 0009 0000 0005 0000 0043 6003 0073 4600  .........C`..sF.
+00000b00: 0009 0000 0005 0000 0043 6003 0073 4c00  .........C`..sL.
 00000b10: 0000 7400 0064 0100 7c00 0064 0200 7c01  ..t..d..|..d..|.
 00000b20: 0083 0002 5c03 007d 0400 7d05 007d 0600  ....\..}..}..}..
 00000b30: 7401 007c 0300 8301 007d 0700 6403 006a  t..|.....}..d..j
 00000b40: 0200 7c05 007c 0200 7c06 007c 0700 8304  ..|..|..|..|....
-00000b50: 007d 0800 7c08 0053 2804 0000 004e 5223  .}..|..S(....NR#
-00000b60: 0000 0052 1800 0000 7525 0000 003c 696d  ...R....u%...<im
-00000b70: 6720 7372 633d 227b 7d22 2063 6c61 7373  g src="{}" class
-00000b80: 3d22 7b7d 2220 616c 743d 227b 7d22 207b  ="{}" alt="{}" {
-00000b90: 7d3e 2803 0000 0052 2800 0000 5212 0000  }>(....R(...R...
-00000ba0: 0052 1c00 0000 2809 0000 0052 2300 0000  .R....(....R#...
-00000bb0: 5218 0000 0074 0300 0000 6373 7352 1000  R....t....cssR..
-00000bc0: 0000 522d 0000 0052 2200 0000 5221 0000  ..R-...R"...R!..
-00000bd0: 0074 0600 0000 6578 7472 6173 7404 0000  .t....extrast...
-00000be0: 0068 746d 6c28 0000 0000 2800 0000 0073  .html(....(....s
-00000bf0: 3f00 0000 2f55 7365 7273 2f69 616c 6265  ?.../Users/ialbe
-00000c00: 7274 2f61 7070 2f70 7962 6c75 652d 6365  rt/app/pyblue-ce
-00000c10: 6e74 7261 6c2f 7079 626c 7565 2f74 656d  ntral/pyblue/tem
-00000c20: 706c 6174 6574 6167 732f 7079 7461 6773  platetags/pytags
-00000c30: 2e70 7974 0300 0000 696d 6744 0000 0073  .pyt....imgD...s
-00000c40: 0800 0000 0002 1e01 0c01 1801 750e 0000  ............u...
-00000c50: 0073 6179 5f68 656c 6c6f 2e68 746d 6c63  .say_hello.htmlc
-00000c60: 0000 0000 0000 0000 0100 0000 4360 0300  ............C`..
-00000c70: 7307 0000 0074 0000 8300 0053 2801 0000  s....t.....S(...
-00000c80: 004e 2801 0000 0074 0400 0000 6469 6374  .N(....t....dict
-00000c90: 2800 0000 0028 0000 0000 2800 0000 0073  (....(....(....s
-00000ca0: 3f00 0000 2f55 7365 7273 2f69 616c 6265  ?.../Users/ialbe
-00000cb0: 7274 2f61 7070 2f70 7962 6c75 652d 6365  rt/app/pyblue-ce
-00000cc0: 6e74 7261 6c2f 7079 626c 7565 2f74 656d  ntral/pyblue/tem
-00000cd0: 706c 6174 6574 6167 732f 7079 7461 6773  platetags/pytags
-00000ce0: 2e70 7974 0900 0000 7361 795f 6865 6c6c  .pyt....say_hell
-00000cf0: 6f4b 0000 0073 0200 0000 0002 750e 0000  oK...s......u...
-00000d00: 0074 6875 6d62 6e61 696c 2e68 746d 6c75  .thumbnail.htmlu
-00000d10: 0100 0000 2369 0400 0000 6306 0000 000c  ....#i....c.....
-00000d20: 0000 000d 0000 0043 6003 0073 7900 0000  .......C`..sy...
-00000d30: 7400 0064 0100 7c00 0064 0200 7c01 0083  t..d..|..d..|...
-00000d40: 0002 5c03 007d 0600 7d07 007d 0800 7400  ..\..}..}..}..t.
-00000d50: 0064 0100 7c00 0064 0200 7c02 0083 0002  .d..|..d..|.....
-00000d60: 5c03 007d 0600 7d09 007d 0a00 7c03 0070  \..}..}..}..|..p
-00000d70: 4500 7c0a 007d 0300 7401 0064 0300 7c07  E.|..}..t..d..|.
-00000d80: 0064 0400 7c08 0064 0500 7c09 0064 0600  .d..|..d..|..d..
-00000d90: 7c03 0064 0700 7c04 0064 0800 7c05 0083  |..d..|..d..|...
-00000da0: 0006 7d0b 007c 0b00 5328 0900 0000 4e52  ..}..|..S(....NR
-00000db0: 2300 0000 5218 0000 0074 0300 0000 7372  #...R....t....sr
-00000dc0: 6352 2100 0000 7404 0000 006c 696e 6b74  cR!...t....linkt
-00000dd0: 0500 0000 7469 746c 6574 0400 0000 7369  ....titlet....si
-00000de0: 7a65 7408 0000 0063 6c65 6172 6669 7828  zet....clearfix(
-00000df0: 0200 0000 5228 0000 0052 3300 0000 280c  ....R(...R3...(.
-00000e00: 0000 0052 2300 0000 5218 0000 0052 3600  ...R#...R....R6.
-00000e10: 0000 5237 0000 0052 3800 0000 5239 0000  ..R7...R8...R9..
-00000e20: 0052 2d00 0000 5222 0000 0052 2100 0000  .R-...R"...R!...
-00000e30: 7407 0000 0072 656c 6c69 6e6b 7408 0000  t....rellinkt...
-00000e40: 006c 696e 6b6e 616d 6574 0600 0000 7061  .linknamet....pa
-00000e50: 7261 6d73 2800 0000 0028 0000 0000 733f  rams(....(....s?
-00000e60: 0000 002f 5573 6572 732f 6961 6c62 6572  .../Users/ialber
-00000e70: 742f 6170 702f 7079 626c 7565 2d63 656e  t/app/pyblue-cen
-00000e80: 7472 616c 2f70 7962 6c75 652f 7465 6d70  tral/pyblue/temp
-00000e90: 6c61 7465 7461 6773 2f70 7974 6167 732e  latetags/pytags.
-00000ea0: 7079 7405 0000 0074 6875 6d62 5000 0000  pyt....thumbP...
-00000eb0: 730a 0000 0000 021e 011e 010c 012d 0163  s............-.c
-00000ec0: 0500 0000 0a00 0000 0500 0000 4360 0300  ............C`..
-00000ed0: 7356 0000 0074 0000 6401 007c 0000 6402  sV...t..d..|..d.
-00000ee0: 007c 0100 8300 025c 0300 7d05 007d 0600  .|.....\..}..}..
-00000ef0: 7d07 007c 0200 7027 007c 0700 7d02 0074  }..|..p'.|..}..t
-00000f00: 0100 7c04 0083 0100 7d08 0064 0300 7c03  ..|.....}..d..|.
-00000f10: 007c 0600 7c08 007c 0200 6604 0016 7d09  .|..|..|..f...}.
-00000f20: 0074 0200 7c09 0083 0100 5328 0400 0000  .t..|.....S(....
-00000f30: 4e52 2300 0000 5218 0000 0075 2100 0000  NR#...R....u!...
-00000f40: 3c61 2063 6c61 7373 3d22 2573 2220 6872  <a class="%s" hr
-00000f50: 6566 3d22 2573 2220 2573 3e25 733c 2f61  ef="%s" %s>%s</a
-00000f60: 3e28 0300 0000 5228 0000 0052 1200 0000  >(....R(...R....
-00000f70: 5206 0000 0028 0a00 0000 5223 0000 0052  R....(....R#...R
-00000f80: 1800 0000 5211 0000 0052 2f00 0000 5210  ....R....R/...R.
-00000f90: 0000 0052 2d00 0000 5222 0000 0052 2100  ...R-...R"...R!.
-00000fa0: 0000 5230 0000 0052 3100 0000 2800 0000  ..R0...R1...(...
-00000fb0: 0028 0000 0000 733f 0000 002f 5573 6572  .(....s?.../User
-00000fc0: 732f 6961 6c62 6572 742f 6170 702f 7079  s/ialbert/app/py
-00000fd0: 626c 7565 2d63 656e 7472 616c 2f70 7962  blue-central/pyb
-00000fe0: 6c75 652f 7465 6d70 6c61 7465 7461 6773  lue/templatetags
-00000ff0: 2f70 7974 6167 732e 7079 5236 0000 0058  /pytags.pyR6...X
-00001000: 0000 0073 0a00 0000 0002 1e02 0c01 0c01  ...s............
-00001010: 1601 7504 0000 0062 6173 6863 0400 0000  ..u....bashc....
-00001020: 0600 0000 0500 0000 4360 0300 7340 0000  ........C`..s@..
-00001030: 0074 0000 6401 007c 0000 6402 007c 0100  .t..d..|..d..|..
-00001040: 8300 027d 0400 6403 006a 0100 7c02 007c  ...}..d..j..|..|
-00001050: 0400 8302 007d 0500 7c03 0072 3c00 7402  .....}..|..r<.t.
-00001060: 007c 0500 8301 007d 0500 6e00 007c 0500  .|.....}..n..|..
-00001070: 5328 0400 0000 4e52 2300 0000 5218 0000  S(....NR#...R...
-00001080: 0075 2e00 0000 3c70 7265 3e3c 636f 6465  .u....<pre><code
-00001090: 2063 6c61 7373 3d22 6c61 6e67 7561 6765   class="language
-000010a0: 2d7b 7d22 3e7b 7d3c 2f63 6f64 653e 3c2f  -{}">{}</code></
-000010b0: 7072 653e 2803 0000 0052 2e00 0000 521c  pre>(....R....R.
-000010c0: 0000 0052 0600 0000 2806 0000 0052 2300  ...R....(....R#.
-000010d0: 0000 5218 0000 0074 0400 0000 6c61 6e67  ..R....t....lang
-000010e0: 7404 0000 0073 6166 6552 1100 0000 5231  t....safeR....R1
-000010f0: 0000 0028 0000 0000 2800 0000 0073 3f00  ...(....(....s?.
-00001100: 0000 2f55 7365 7273 2f69 616c 6265 7274  ../Users/ialbert
-00001110: 2f61 7070 2f70 7962 6c75 652d 6365 6e74  /app/pyblue-cent
-00001120: 7261 6c2f 7079 626c 7565 2f74 656d 706c  ral/pyblue/templ
-00001130: 6174 6574 6167 732f 7079 7461 6773 2e70  atetags/pytags.p
-00001140: 7974 0400 0000 636f 6465 6200 0000 730a  yt....codeb...s.
-00001150: 0000 0000 0215 0112 0106 010f 0163 0300  .............c..
-00001160: 0000 0500 0000 0500 0000 4360 0300 7331  ..........C`..s1
-00001170: 0000 0074 0000 6401 007c 0000 6402 007c  ...t..d..|..d..|
-00001180: 0100 8300 027d 0300 7401 007c 0300 8301  .....}..t..|....
-00001190: 007d 0400 7402 007c 0400 8301 007d 0400  .}..t..|.....}..
-000011a0: 7c04 0053 2803 0000 004e 5223 0000 0052  |..S(....NR#...R
-000011b0: 1800 0000 2803 0000 0052 2e00 0000 7408  ....(....R....t.
-000011c0: 0000 006d 6172 6b64 6f77 6e52 0600 0000  ...markdownR....
-000011d0: 2805 0000 0052 2300 0000 5218 0000 0052  (....R#...R....R
-000011e0: 3f00 0000 5211 0000 0052 3100 0000 2800  ?...R....R1...(.
-000011f0: 0000 0028 0000 0000 733f 0000 002f 5573  ...(....s?.../Us
-00001200: 6572 732f 6961 6c62 6572 742f 6170 702f  ers/ialbert/app/
-00001210: 7079 626c 7565 2d63 656e 7472 616c 2f70  pyblue-central/p
-00001220: 7962 6c75 652f 7465 6d70 6c61 7465 7461  yblue/templateta
-00001230: 6773 2f70 7974 6167 732e 7079 7410 0000  gs/pytags.pyt...
-00001240: 0069 6e63 6c75 6465 5f6d 6172 6b64 6f77  .include_markdow
-00001250: 6e6b 0000 0073 0800 0000 0002 1501 0c01  nk...s..........
-00001260: 0c01 7510 0000 0073 6974 655f 6173 7365  ..u....site_asse
-00001270: 7473 2e68 746d 6c63 0100 0000 0100 0000  ts.htmlc........
-00001280: 0300 0000 4360 0300 730d 0000 0074 0000  ....C`..s....t..
-00001290: 6401 007c 0000 8300 0153 2802 0000 004e  d..|.....S(....N
-000012a0: 5223 0000 0028 0100 0000 5233 0000 0028  R#...(....R3...(
-000012b0: 0100 0000 5223 0000 0028 0000 0000 2800  ....R#...(....(.
-000012c0: 0000 0073 3f00 0000 2f55 7365 7273 2f69  ...s?.../Users/i
-000012d0: 616c 6265 7274 2f61 7070 2f70 7962 6c75  albert/app/pyblu
-000012e0: 652d 6365 6e74 7261 6c2f 7079 626c 7565  e-central/pyblue
-000012f0: 2f74 656d 706c 6174 6574 6167 732f 7079  /templatetags/py
-00001300: 7461 6773 2e70 7974 0b00 0000 7369 7465  tags.pyt....site
-00001310: 5f61 7373 6574 7373 0000 0073 0200 0000  _assetss...s....
-00001320: 0002 6302 0000 0003 0000 0003 0000 0043  ..c............C
-00001330: 6003 0073 2b00 0000 7c01 0073 0a00 7c00  `..s+...|..s..|.
-00001340: 0053 7c00 0064 0100 197d 0200 7c02 006a  .S|..d...}..|..j
-00001350: 0000 6404 0083 0100 7327 0064 0000 537c  ..d.....s'.d..S|
-00001360: 0000 5328 0500 0000 4e75 0500 0000 5f74  ..S(....Nu...._t
-00001370: 6578 7475 0500 0000 6874 7470 3a75 0600  extu....http:u..
-00001380: 0000 6874 7470 733a 2802 0000 0075 0500  ..https:(....u..
-00001390: 0000 6874 7470 3a75 0600 0000 6874 7470  ..http:u....http
-000013a0: 733a 2802 0000 0074 0a00 0000 7374 6172  s:(....t....star
-000013b0: 7473 7769 7468 521f 0000 0028 0300 0000  tswithR....(....
-000013c0: 5210 0000 0074 0300 0000 6e65 7752 1100  R....t....newR..
-000013d0: 0000 2800 0000 0028 0000 0000 733f 0000  ..(....(....s?..
-000013e0: 002f 5573 6572 732f 6961 6c62 6572 742f  ./Users/ialbert/
-000013f0: 6170 702f 7079 626c 7565 2d63 656e 7472  app/pyblue-centr
-00001400: 616c 2f70 7962 6c75 652f 7465 6d70 6c61  al/pyblue/templa
-00001410: 7465 7461 6773 2f70 7974 6167 732e 7079  tetags/pytags.py
-00001420: 740e 0000 0074 6f70 5f6c 6576 656c 5f6f  t....top_level_o
-00001430: 6e6c 797c 0000 0073 0c00 0000 0001 0601  nly|...s........
-00001440: 0401 0a01 0f01 0401 740c 0000 004d 6172  ........t....Mar
-00001450: 6b44 6f77 6e4e 6f64 6563 0000 0000 0000  kDownNodec......
-00001460: 0000 0100 0000 4260 0300 7323 0000 0065  ......B`..s#...e
-00001470: 0000 5a01 0065 0200 6701 005a 0300 6400  ..Z..e..g..Z..d.
-00001480: 0084 0000 5a04 0064 0100 8400 005a 0500  ....Z..d.....Z..
-00001490: 5253 2802 0000 0063 0200 0000 0200 0000  RS(....c........
-000014a0: 0200 0000 4360 0300 730d 0000 007c 0100  ....C`..s....|..
-000014b0: 7c00 005f 0000 6400 0053 2801 0000 004e  |.._..d..S(....N
-000014c0: 2801 0000 0074 0800 0000 6e6f 6465 6c69  (....t....nodeli
-000014d0: 7374 2802 0000 0074 0400 0000 7365 6c66  st(....t....self
-000014e0: 5248 0000 0028 0000 0000 2800 0000 0073  RH...(....(....s
-000014f0: 3f00 0000 2f55 7365 7273 2f69 616c 6265  ?.../Users/ialbe
-00001500: 7274 2f61 7070 2f70 7962 6c75 652d 6365  rt/app/pyblue-ce
-00001510: 6e74 7261 6c2f 7079 626c 7565 2f74 656d  ntral/pyblue/tem
-00001520: 706c 6174 6574 6167 732f 7079 7461 6773  platetags/pytags
-00001530: 2e70 7974 0800 0000 5f5f 696e 6974 5f5f  .pyt....__init__
-00001540: 8600 0000 7302 0000 0000 0163 0200 0000  ....s......c....
-00001550: 0300 0000 0600 0000 4360 0300 7340 0000  ........C`..s@..
-00001560: 007c 0000 6a00 006a 0100 7c01 0083 0100  .|..j..j..|.....
-00001570: 7d02 0074 0200 7c02 0083 0100 7d02 0074  }..t..|.....}..t
-00001580: 0300 6a04 007c 0200 6401 007c 0000 6a05  ..j..|..d..|..j.
-00001590: 0064 0200 7406 0083 0102 7d02 007c 0200  .d..t.....}..|..
-000015a0: 5328 0300 0000 4e74 0900 0000 6361 6c6c  S(....Nt....call
-000015b0: 6261 636b 7374 0800 0000 736b 6970 5f70  backst....skip_p
-000015c0: 7265 2807 0000 0052 4800 0000 7406 0000  re(....RH...t...
-000015d0: 0072 656e 6465 7252 4100 0000 7406 0000  .renderRA...t...
-000015e0: 0062 6c65 6163 6874 0700 0000 6c69 6e6b  .bleacht....link
-000015f0: 6966 7974 0900 0000 4341 4c4c 4241 434b  ifyt....CALLBACK
-00001600: 5374 0400 0000 5472 7565 2803 0000 0052  St....True(....R
-00001610: 4900 0000 5223 0000 0052 1100 0000 2800  I...R#...R....(.
-00001620: 0000 0028 0000 0000 733f 0000 002f 5573  ...(....s?.../Us
-00001630: 6572 732f 6961 6c62 6572 742f 6170 702f  ers/ialbert/app/
-00001640: 7079 626c 7565 2d63 656e 7472 616c 2f70  pyblue-central/p
-00001650: 7962 6c75 652f 7465 6d70 6c61 7465 7461  yblue/templateta
-00001660: 6773 2f70 7974 6167 732e 7079 524d 0000  gs/pytags.pyRM..
-00001670: 0089 0000 0073 0800 0000 0001 1201 0c01  .....s..........
-00001680: 1e01 2806 0000 0074 0800 0000 5f5f 6e61  ..(....t....__na
-00001690: 6d65 5f5f 740a 0000 005f 5f6d 6f64 756c  me__t....__modul
-000016a0: 655f 5f52 4600 0000 5250 0000 0052 4a00  e__RF...RP...RJ.
-000016b0: 0000 524d 0000 0028 0000 0000 2800 0000  ..RM...(....(...
-000016c0: 0028 0000 0000 733f 0000 002f 5573 6572  .(....s?.../User
-000016d0: 732f 6961 6c62 6572 742f 6170 702f 7079  s/ialbert/app/py
-000016e0: 626c 7565 2d63 656e 7472 616c 2f70 7962  blue-central/pyb
-000016f0: 6c75 652f 7465 6d70 6c61 7465 7461 6773  lue/templatetags
-00001700: 2f70 7974 6167 732e 7079 5247 0000 0084  /pytags.pyRG....
-00001710: 0000 0073 0600 0000 0601 0901 0903 7508  ...s..........u.
-00001720: 0000 006d 6172 6b64 6f77 6e63 0200 0000  ...markdownc....
-00001730: 0300 0000 0200 0000 4360 0300 7323 0000  ........C`..s#..
-00001740: 007c 0000 6a00 0064 0200 8301 007d 0200  .|..j..d.....}..
-00001750: 7c00 006a 0100 8300 0001 7402 007c 0200  |..j......t..|..
-00001760: 8301 0053 2803 0000 0075 5a01 0000 0a20  ...S(....uZ.... 
-00001770: 2020 2045 6e61 626c 6573 2061 2062 6c6f     Enables a blo
-00001780: 636b 206f 6620 6d61 726b 646f 776e 2074  ck of markdown t
-00001790: 6578 7420 746f 2062 6520 7573 6564 2069  ext to be used i
-000017a0: 6e20 6120 7465 6d70 6c61 7465 2e0a 0a20  n a template... 
-000017b0: 2020 2053 796e 7461 783a 3a0a 0a20 2020     Syntax::..   
-000017c0: 2020 2020 2020 2020 207b 2520 6d61 726b           {% mark
-000017d0: 646f 776e 2025 7d0a 2020 2020 2020 2020  down %}.        
-000017e0: 2020 2020 2323 204d 6172 6b64 6f77 6e0a      ## Markdown.
-000017f0: 0a20 2020 2020 2020 2020 2020 204e 6f77  .            Now
-00001800: 2079 6f75 2063 616e 2077 7269 7465 206d   you can write m
-00001810: 6172 6b64 6f77 6e20 696e 2079 6f75 7220  arkdown in your 
-00001820: 7465 6d70 6c61 7465 732e 2054 6869 7320  templates. This 
-00001830: 6973 2067 6f6f 6420 6265 6361 7573 653a  is good because:
-00001840: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-00001850: 6d61 726b 646f 776e 2069 7320 6177 6573  markdown is awes
-00001860: 6f6d 650a 2020 2020 2020 2020 2020 2020  ome.            
-00001870: 2a20 6d61 726b 646f 776e 2069 7320 6c65  * markdown is le
-00001880: 7373 2076 6572 626f 7365 2074 6861 6e20  ss verbose than 
-00001890: 7772 6974 696e 6720 6874 6d6c 2062 7920  writing html by 
-000018a0: 6861 6e64 0a0a 2020 2020 2020 2020 2020  hand..          
-000018b0: 2020 7b25 2065 6e64 6d61 726b 646f 776e    {% endmarkdown
-000018c0: 2025 7d0a 2020 2020 750b 0000 0065 6e64   %}.    u....end
-000018d0: 6d61 726b 646f 776e 2801 0000 0075 0b00  markdown(....u..
-000018e0: 0000 656e 646d 6172 6b64 6f77 6e28 0300  ..endmarkdown(..
-000018f0: 0000 7405 0000 0070 6172 7365 7412 0000  ..t....parset...
-00001900: 0064 656c 6574 655f 6669 7273 745f 746f  .delete_first_to
-00001910: 6b65 6e52 4700 0000 2803 0000 0074 0600  kenRG...(....t..
-00001920: 0000 7061 7273 6572 7405 0000 0074 6f6b  ..parsert....tok
-00001930: 656e 5248 0000 0028 0000 0000 2800 0000  enRH...(....(...
-00001940: 0073 3f00 0000 2f55 7365 7273 2f69 616c  .s?.../Users/ial
-00001950: 6265 7274 2f61 7070 2f70 7962 6c75 652d  bert/app/pyblue-
-00001960: 6365 6e74 7261 6c2f 7079 626c 7565 2f74  central/pyblue/t
-00001970: 656d 706c 6174 6574 6167 732f 7079 7461  emplatetags/pyta
-00001980: 6773 2e70 7974 0c00 0000 6d61 726b 646f  gs.pyt....markdo
-00001990: 776e 5f74 6167 8f00 0000 7306 0000 0000  wn_tag....s.....
-000019a0: 110f 020a 0128 2900 0000 740a 0000 005f  .....()...t...._
-000019b0: 5f66 7574 7572 655f 5f52 0000 0000 5201  _future__R....R.
-000019c0: 0000 0052 0200 0000 5203 0000 0074 0600  ...R....R....t..
-000019d0: 0000 646a 616e 676f 5204 0000 0074 0700  ..djangoR....t..
-000019e0: 0000 6c6f 6767 696e 6752 1300 0000 524e  ..loggingR....RN
-000019f0: 0000 0052 0700 0000 7411 0000 0064 6a61  ...R....t....dja
-00001a00: 6e67 6f2e 7574 696c 732e 6874 6d6c 5205  ngo.utils.htmlR.
-00001a10: 0000 0074 1700 0000 646a 616e 676f 2e75  ...t....django.u
-00001a20: 7469 6c73 2e73 6166 6573 7472 696e 6752  tils.safestringR
-00001a30: 0600 0000 7409 0000 0067 6574 4c6f 6767  ....t....getLogg
-00001a40: 6572 521d 0000 0074 0700 0000 4c69 6272  erR....t....Libr
-00001a50: 6172 7974 0800 0000 7265 6769 7374 6572  aryt....register
-00001a60: 520a 0000 0052 4100 0000 5212 0000 0052  R....RA...R....R
-00001a70: 2800 0000 740a 0000 0073 696d 706c 655f  (...t....simple_
-00001a80: 7461 6752 5100 0000 522e 0000 0052 3200  tagRQ...R....R2.
-00001a90: 0000 740d 0000 0069 6e63 6c75 7369 6f6e  ..t....inclusion
-00001aa0: 5f74 6167 5234 0000 0074 0500 0000 4661  _tagR4...t....Fa
-00001ab0: 6c73 6552 3d00 0000 521f 0000 0052 3600  lseR=...R....R6.
-00001ac0: 0000 5240 0000 0052 4200 0000 5243 0000  ..R@...RB...RC..
-00001ad0: 0052 4600 0000 7404 0000 004e 6f64 6552  .RF...t....NodeR
-00001ae0: 4700 0000 7403 0000 0074 6167 5258 0000  G...t....tagRX..
-00001af0: 0028 0000 0000 2800 0000 0028 0000 0000  .(....(....(....
-00001b00: 733f 0000 002f 5573 6572 732f 6961 6c62  s?.../Users/ialb
-00001b10: 6572 742f 6170 702f 7079 626c 7565 2d63  ert/app/pyblue-c
-00001b20: 656e 7472 616c 2f70 7962 6c75 652f 7465  entral/pyblue/te
-00001b30: 6d70 6c61 7465 7461 6773 2f70 7974 6167  mplatetags/pytag
-00001b40: 732e 7079 7408 0000 003c 6d6f 6475 6c65  s.pyt....<module
-00001b50: 3e01 0000 0073 3800 0000 2201 1001 1801  >....s8...".....
-00001b60: 0c01 0c01 1001 1002 0f02 0c02 0905 0903  ................
-00001b70: 0c07 091d 1b0b 0f01 1206 1805 1201 1807  ................
-00001b80: 0f01 1509 0f01 1208 0f01 0f07 1e09 0c08  ................
-00001b90: 190b                                     ..
+00000b50: 007d 0800 7403 007c 0800 8301 0053 2804  .}..t..|.....S(.
+00000b60: 0000 004e 5223 0000 0052 1800 0000 7525  ...NR#...R....u%
+00000b70: 0000 003c 696d 6720 7372 633d 227b 7d22  ...<img src="{}"
+00000b80: 2063 6c61 7373 3d22 7b7d 2220 616c 743d   class="{}" alt=
+00000b90: 227b 7d22 207b 7d3e 2804 0000 0052 2800  "{}" {}>(....R(.
+00000ba0: 0000 5212 0000 0052 1c00 0000 5206 0000  ..R....R....R...
+00000bb0: 0028 0900 0000 5223 0000 0052 1800 0000  .(....R#...R....
+00000bc0: 7403 0000 0063 7373 5210 0000 0052 2d00  t....cssR....R-.
+00000bd0: 0000 5222 0000 0052 2100 0000 7406 0000  ..R"...R!...t...
+00000be0: 0065 7874 7261 7374 0400 0000 6874 6d6c  .extrast....html
+00000bf0: 2800 0000 0028 0000 0000 733f 0000 002f  (....(....s?.../
+00000c00: 5573 6572 732f 6961 6c62 6572 742f 6170  Users/ialbert/ap
+00000c10: 702f 7079 626c 7565 2d63 656e 7472 616c  p/pyblue-central
+00000c20: 2f70 7962 6c75 652f 7465 6d70 6c61 7465  /pyblue/template
+00000c30: 7461 6773 2f70 7974 6167 732e 7079 7403  tags/pytags.pyt.
+00000c40: 0000 0069 6d67 4400 0000 7308 0000 0000  ...imgD...s.....
+00000c50: 021e 010c 0118 0175 0e00 0000 7361 795f  .......u....say_
+00000c60: 6865 6c6c 6f2e 6874 6d6c 6300 0000 0000  hello.htmlc.....
+00000c70: 0000 0001 0000 0043 6003 0073 0700 0000  .......C`..s....
+00000c80: 7400 0083 0000 5328 0100 0000 4e28 0100  t.....S(....N(..
+00000c90: 0000 7404 0000 0064 6963 7428 0000 0000  ..t....dict(....
+00000ca0: 2800 0000 0028 0000 0000 733f 0000 002f  (....(....s?.../
+00000cb0: 5573 6572 732f 6961 6c62 6572 742f 6170  Users/ialbert/ap
+00000cc0: 702f 7079 626c 7565 2d63 656e 7472 616c  p/pyblue-central
+00000cd0: 2f70 7962 6c75 652f 7465 6d70 6c61 7465  /pyblue/template
+00000ce0: 7461 6773 2f70 7974 6167 732e 7079 7409  tags/pytags.pyt.
+00000cf0: 0000 0073 6179 5f68 656c 6c6f 4b00 0000  ...say_helloK...
+00000d00: 7302 0000 0000 0275 0e00 0000 7468 756d  s......u....thum
+00000d10: 626e 6169 6c2e 6874 6d6c 7501 0000 0023  bnail.htmlu....#
+00000d20: 6904 0000 0063 0600 0000 0c00 0000 0d00  i....c..........
+00000d30: 0000 4360 0300 7379 0000 0074 0000 6401  ..C`..sy...t..d.
+00000d40: 007c 0000 6402 007c 0100 8300 025c 0300  .|..d..|.....\..
+00000d50: 7d06 007d 0700 7d08 0074 0000 6401 007c  }..}..}..t..d..|
+00000d60: 0000 6402 007c 0200 8300 025c 0300 7d06  ..d..|.....\..}.
+00000d70: 007d 0900 7d0a 007c 0300 7045 007c 0a00  .}..}..|..pE.|..
+00000d80: 7d03 0074 0100 6403 007c 0700 6404 007c  }..t..d..|..d..|
+00000d90: 0800 6405 007c 0900 6406 007c 0300 6407  ..d..|..d..|..d.
+00000da0: 007c 0400 6408 007c 0500 8300 067d 0b00  .|..d..|.....}..
+00000db0: 7c0b 0053 2809 0000 004e 5223 0000 0052  |..S(....NR#...R
+00000dc0: 1800 0000 7403 0000 0073 7263 5221 0000  ....t....srcR!..
+00000dd0: 0074 0400 0000 6c69 6e6b 7405 0000 0074  .t....linkt....t
+00000de0: 6974 6c65 7404 0000 0073 697a 6574 0800  itlet....sizet..
+00000df0: 0000 636c 6561 7266 6978 2802 0000 0052  ..clearfix(....R
+00000e00: 2800 0000 5233 0000 0028 0c00 0000 5223  (...R3...(....R#
+00000e10: 0000 0052 1800 0000 5236 0000 0052 3700  ...R....R6...R7.
+00000e20: 0000 5238 0000 0052 3900 0000 522d 0000  ..R8...R9...R-..
+00000e30: 0052 2200 0000 5221 0000 0074 0700 0000  .R"...R!...t....
+00000e40: 7265 6c6c 696e 6b74 0800 0000 6c69 6e6b  rellinkt....link
+00000e50: 6e61 6d65 7406 0000 0070 6172 616d 7328  namet....params(
+00000e60: 0000 0000 2800 0000 0073 3f00 0000 2f55  ....(....s?.../U
+00000e70: 7365 7273 2f69 616c 6265 7274 2f61 7070  sers/ialbert/app
+00000e80: 2f70 7962 6c75 652d 6365 6e74 7261 6c2f  /pyblue-central/
+00000e90: 7079 626c 7565 2f74 656d 706c 6174 6574  pyblue/templatet
+00000ea0: 6167 732f 7079 7461 6773 2e70 7974 0500  ags/pytags.pyt..
+00000eb0: 0000 7468 756d 6250 0000 0073 0a00 0000  ..thumbP...s....
+00000ec0: 0002 1e01 1e01 0c01 2d01 6305 0000 000a  ........-.c.....
+00000ed0: 0000 0005 0000 0043 6003 0073 5600 0000  .......C`..sV...
+00000ee0: 7400 0064 0100 7c00 0064 0200 7c01 0083  t..d..|..d..|...
+00000ef0: 0002 5c03 007d 0500 7d06 007d 0700 7c02  ..\..}..}..}..|.
+00000f00: 0070 2700 7c07 007d 0200 7401 007c 0400  .p'.|..}..t..|..
+00000f10: 8301 007d 0800 6403 007c 0300 7c06 007c  ...}..d..|..|..|
+00000f20: 0800 7c02 0066 0400 167d 0900 7402 007c  ..|..f...}..t..|
+00000f30: 0900 8301 0053 2804 0000 004e 5223 0000  .....S(....NR#..
+00000f40: 0052 1800 0000 7521 0000 003c 6120 636c  .R....u!...<a cl
+00000f50: 6173 733d 2225 7322 2068 7265 663d 2225  ass="%s" href="%
+00000f60: 7322 2025 733e 2573 3c2f 613e 2803 0000  s" %s>%s</a>(...
+00000f70: 0052 2800 0000 5212 0000 0052 0600 0000  .R(...R....R....
+00000f80: 280a 0000 0052 2300 0000 5218 0000 0052  (....R#...R....R
+00000f90: 1100 0000 522f 0000 0052 1000 0000 522d  ....R/...R....R-
+00000fa0: 0000 0052 2200 0000 5221 0000 0052 3000  ...R"...R!...R0.
+00000fb0: 0000 5231 0000 0028 0000 0000 2800 0000  ..R1...(....(...
+00000fc0: 0073 3f00 0000 2f55 7365 7273 2f69 616c  .s?.../Users/ial
+00000fd0: 6265 7274 2f61 7070 2f70 7962 6c75 652d  bert/app/pyblue-
+00000fe0: 6365 6e74 7261 6c2f 7079 626c 7565 2f74  central/pyblue/t
+00000ff0: 656d 706c 6174 6574 6167 732f 7079 7461  emplatetags/pyta
+00001000: 6773 2e70 7952 3600 0000 5800 0000 730a  gs.pyR6...X...s.
+00001010: 0000 0000 021e 020c 010c 0116 0175 0400  .............u..
+00001020: 0000 6261 7368 6304 0000 0006 0000 0005  ..bashc.........
+00001030: 0000 0043 6003 0073 4000 0000 7400 0064  ...C`..s@...t..d
+00001040: 0100 7c00 0064 0200 7c01 0083 0002 7d04  ..|..d..|.....}.
+00001050: 0064 0300 6a01 007c 0200 7c04 0083 0200  .d..j..|..|.....
+00001060: 7d05 007c 0300 723c 0074 0200 7c05 0083  }..|..r<.t..|...
+00001070: 0100 7d05 006e 0000 7c05 0053 2804 0000  ..}..n..|..S(...
+00001080: 004e 5223 0000 0052 1800 0000 752e 0000  .NR#...R....u...
+00001090: 003c 7072 653e 3c63 6f64 6520 636c 6173  .<pre><code clas
+000010a0: 733d 226c 616e 6775 6167 652d 7b7d 223e  s="language-{}">
+000010b0: 7b7d 3c2f 636f 6465 3e3c 2f70 7265 3e28  {}</code></pre>(
+000010c0: 0300 0000 522e 0000 0052 1c00 0000 5206  ....R....R....R.
+000010d0: 0000 0028 0600 0000 5223 0000 0052 1800  ...(....R#...R..
+000010e0: 0000 7404 0000 006c 616e 6774 0400 0000  ..t....langt....
+000010f0: 7361 6665 5211 0000 0052 3100 0000 2800  safeR....R1...(.
+00001100: 0000 0028 0000 0000 733f 0000 002f 5573  ...(....s?.../Us
+00001110: 6572 732f 6961 6c62 6572 742f 6170 702f  ers/ialbert/app/
+00001120: 7079 626c 7565 2d63 656e 7472 616c 2f70  pyblue-central/p
+00001130: 7962 6c75 652f 7465 6d70 6c61 7465 7461  yblue/templateta
+00001140: 6773 2f70 7974 6167 732e 7079 7404 0000  gs/pytags.pyt...
+00001150: 0063 6f64 6562 0000 0073 0a00 0000 0002  .codeb...s......
+00001160: 1501 1201 0601 0f01 6303 0000 0005 0000  ........c.......
+00001170: 0005 0000 0043 6003 0073 3100 0000 7400  .....C`..s1...t.
+00001180: 0064 0100 7c00 0064 0200 7c01 0083 0002  .d..|..d..|.....
+00001190: 7d03 0074 0100 7c03 0083 0100 7d04 0074  }..t..|.....}..t
+000011a0: 0200 7c04 0083 0100 7d04 007c 0400 5328  ..|.....}..|..S(
+000011b0: 0300 0000 4e52 2300 0000 5218 0000 0028  ....NR#...R....(
+000011c0: 0300 0000 522e 0000 0074 0800 0000 6d61  ....R....t....ma
+000011d0: 726b 646f 776e 5206 0000 0028 0500 0000  rkdownR....(....
+000011e0: 5223 0000 0052 1800 0000 523f 0000 0052  R#...R....R?...R
+000011f0: 1100 0000 5231 0000 0028 0000 0000 2800  ....R1...(....(.
+00001200: 0000 0073 3f00 0000 2f55 7365 7273 2f69  ...s?.../Users/i
+00001210: 616c 6265 7274 2f61 7070 2f70 7962 6c75  albert/app/pyblu
+00001220: 652d 6365 6e74 7261 6c2f 7079 626c 7565  e-central/pyblue
+00001230: 2f74 656d 706c 6174 6574 6167 732f 7079  /templatetags/py
+00001240: 7461 6773 2e70 7974 1000 0000 696e 636c  tags.pyt....incl
+00001250: 7564 655f 6d61 726b 646f 776e 6b00 0000  ude_markdownk...
+00001260: 7308 0000 0000 0215 010c 010c 0175 1000  s............u..
+00001270: 0000 7369 7465 5f61 7373 6574 732e 6874  ..site_assets.ht
+00001280: 6d6c 6301 0000 0001 0000 0003 0000 0043  mlc............C
+00001290: 6003 0073 0d00 0000 7400 0064 0100 7c00  `..s....t..d..|.
+000012a0: 0083 0001 5328 0200 0000 4e52 2300 0000  ....S(....NR#...
+000012b0: 2801 0000 0052 3300 0000 2801 0000 0052  (....R3...(....R
+000012c0: 2300 0000 2800 0000 0028 0000 0000 733f  #...(....(....s?
+000012d0: 0000 002f 5573 6572 732f 6961 6c62 6572  .../Users/ialber
+000012e0: 742f 6170 702f 7079 626c 7565 2d63 656e  t/app/pyblue-cen
+000012f0: 7472 616c 2f70 7962 6c75 652f 7465 6d70  tral/pyblue/temp
+00001300: 6c61 7465 7461 6773 2f70 7974 6167 732e  latetags/pytags.
+00001310: 7079 740b 0000 0073 6974 655f 6173 7365  pyt....site_asse
+00001320: 7473 7300 0000 7302 0000 0000 0263 0200  tss...s......c..
+00001330: 0000 0300 0000 0300 0000 4360 0300 732b  ..........C`..s+
+00001340: 0000 007c 0100 730a 007c 0000 537c 0000  ...|..s..|..S|..
+00001350: 6401 0019 7d02 007c 0200 6a00 0064 0400  d...}..|..j..d..
+00001360: 8301 0073 2700 6400 0053 7c00 0053 2805  ...s'.d..S|..S(.
+00001370: 0000 004e 7505 0000 005f 7465 7874 7505  ...Nu...._textu.
+00001380: 0000 0068 7474 703a 7506 0000 0068 7474  ...http:u....htt
+00001390: 7073 3a28 0200 0000 7505 0000 0068 7474  ps:(....u....htt
+000013a0: 703a 7506 0000 0068 7474 7073 3a28 0200  p:u....https:(..
+000013b0: 0000 740a 0000 0073 7461 7274 7377 6974  ..t....startswit
+000013c0: 6852 1f00 0000 2803 0000 0052 1000 0000  hR....(....R....
+000013d0: 7403 0000 006e 6577 5211 0000 0028 0000  t....newR....(..
+000013e0: 0000 2800 0000 0073 3f00 0000 2f55 7365  ..(....s?.../Use
+000013f0: 7273 2f69 616c 6265 7274 2f61 7070 2f70  rs/ialbert/app/p
+00001400: 7962 6c75 652d 6365 6e74 7261 6c2f 7079  yblue-central/py
+00001410: 626c 7565 2f74 656d 706c 6174 6574 6167  blue/templatetag
+00001420: 732f 7079 7461 6773 2e70 7974 0e00 0000  s/pytags.pyt....
+00001430: 746f 705f 6c65 7665 6c5f 6f6e 6c79 7c00  top_level_only|.
+00001440: 0000 730c 0000 0000 0106 0104 010a 010f  ..s.............
+00001450: 0104 0174 0c00 0000 4d61 726b 446f 776e  ...t....MarkDown
+00001460: 4e6f 6465 6300 0000 0000 0000 0001 0000  Nodec...........
+00001470: 0042 6003 0073 2300 0000 6500 005a 0100  .B`..s#...e..Z..
+00001480: 6502 0067 0100 5a03 0064 0000 8400 005a  e..g..Z..d.....Z
+00001490: 0400 6401 0084 0000 5a05 0052 5328 0200  ..d.....Z..RS(..
+000014a0: 0000 6302 0000 0002 0000 0002 0000 0043  ..c............C
+000014b0: 6003 0073 0d00 0000 7c01 007c 0000 5f00  `..s....|..|.._.
+000014c0: 0064 0000 5328 0100 0000 4e28 0100 0000  .d..S(....N(....
+000014d0: 7408 0000 006e 6f64 656c 6973 7428 0200  t....nodelist(..
+000014e0: 0000 7404 0000 0073 656c 6652 4800 0000  ..t....selfRH...
+000014f0: 2800 0000 0028 0000 0000 733f 0000 002f  (....(....s?.../
+00001500: 5573 6572 732f 6961 6c62 6572 742f 6170  Users/ialbert/ap
+00001510: 702f 7079 626c 7565 2d63 656e 7472 616c  p/pyblue-central
+00001520: 2f70 7962 6c75 652f 7465 6d70 6c61 7465  /pyblue/template
+00001530: 7461 6773 2f70 7974 6167 732e 7079 7408  tags/pytags.pyt.
+00001540: 0000 005f 5f69 6e69 745f 5f86 0000 0073  ...__init__....s
+00001550: 0200 0000 0001 6302 0000 0003 0000 0006  ......c.........
+00001560: 0000 0043 6003 0073 4000 0000 7c00 006a  ...C`..s@...|..j
+00001570: 0000 6a01 007c 0100 8301 007d 0200 7402  ..j..|.....}..t.
+00001580: 007c 0200 8301 007d 0200 7403 006a 0400  .|.....}..t..j..
+00001590: 7c02 0064 0100 7c00 006a 0500 6402 0074  |..d..|..j..d..t
+000015a0: 0600 8301 027d 0200 7c02 0053 2803 0000  .....}..|..S(...
+000015b0: 004e 7409 0000 0063 616c 6c62 6163 6b73  .Nt....callbacks
+000015c0: 7408 0000 0073 6b69 705f 7072 6528 0700  t....skip_pre(..
+000015d0: 0000 5248 0000 0074 0600 0000 7265 6e64  ..RH...t....rend
+000015e0: 6572 5241 0000 0074 0600 0000 626c 6561  erRA...t....blea
+000015f0: 6368 7407 0000 006c 696e 6b69 6679 7409  cht....linkifyt.
+00001600: 0000 0043 414c 4c42 4143 4b53 7404 0000  ...CALLBACKSt...
+00001610: 0054 7275 6528 0300 0000 5249 0000 0052  .True(....RI...R
+00001620: 2300 0000 5211 0000 0028 0000 0000 2800  #...R....(....(.
+00001630: 0000 0073 3f00 0000 2f55 7365 7273 2f69  ...s?.../Users/i
+00001640: 616c 6265 7274 2f61 7070 2f70 7962 6c75  albert/app/pyblu
+00001650: 652d 6365 6e74 7261 6c2f 7079 626c 7565  e-central/pyblue
+00001660: 2f74 656d 706c 6174 6574 6167 732f 7079  /templatetags/py
+00001670: 7461 6773 2e70 7952 4d00 0000 8900 0000  tags.pyRM.......
+00001680: 7308 0000 0000 0112 010c 011e 0128 0600  s............(..
+00001690: 0000 7408 0000 005f 5f6e 616d 655f 5f74  ..t....__name__t
+000016a0: 0a00 0000 5f5f 6d6f 6475 6c65 5f5f 5246  ....__module__RF
+000016b0: 0000 0052 5000 0000 524a 0000 0052 4d00  ...RP...RJ...RM.
+000016c0: 0000 2800 0000 0028 0000 0000 2800 0000  ..(....(....(...
+000016d0: 0073 3f00 0000 2f55 7365 7273 2f69 616c  .s?.../Users/ial
+000016e0: 6265 7274 2f61 7070 2f70 7962 6c75 652d  bert/app/pyblue-
+000016f0: 6365 6e74 7261 6c2f 7079 626c 7565 2f74  central/pyblue/t
+00001700: 656d 706c 6174 6574 6167 732f 7079 7461  emplatetags/pyta
+00001710: 6773 2e70 7952 4700 0000 8400 0000 7306  gs.pyRG.......s.
+00001720: 0000 0006 0109 0109 0375 0800 0000 6d61  .........u....ma
+00001730: 726b 646f 776e 6302 0000 0003 0000 0002  rkdownc.........
+00001740: 0000 0043 6003 0073 2300 0000 7c00 006a  ...C`..s#...|..j
+00001750: 0000 6402 0083 0100 7d02 007c 0000 6a01  ..d.....}..|..j.
+00001760: 0083 0000 0174 0200 7c02 0083 0100 5328  .....t..|.....S(
+00001770: 0300 0000 755a 0100 000a 2020 2020 456e  ....uZ....    En
+00001780: 6162 6c65 7320 6120 626c 6f63 6b20 6f66  ables a block of
+00001790: 206d 6172 6b64 6f77 6e20 7465 7874 2074   markdown text t
+000017a0: 6f20 6265 2075 7365 6420 696e 2061 2074  o be used in a t
+000017b0: 656d 706c 6174 652e 0a0a 2020 2020 5379  emplate...    Sy
+000017c0: 6e74 6178 3a3a 0a0a 2020 2020 2020 2020  ntax::..        
+000017d0: 2020 2020 7b25 206d 6172 6b64 6f77 6e20      {% markdown 
+000017e0: 257d 0a20 2020 2020 2020 2020 2020 2023  %}.            #
+000017f0: 2320 4d61 726b 646f 776e 0a0a 2020 2020  # Markdown..    
+00001800: 2020 2020 2020 2020 4e6f 7720 796f 7520          Now you 
+00001810: 6361 6e20 7772 6974 6520 6d61 726b 646f  can write markdo
+00001820: 776e 2069 6e20 796f 7572 2074 656d 706c  wn in your templ
+00001830: 6174 6573 2e20 5468 6973 2069 7320 676f  ates. This is go
+00001840: 6f64 2062 6563 6175 7365 3a0a 0a20 2020  od because:..   
+00001850: 2020 2020 2020 2020 202a 206d 6172 6b64           * markd
+00001860: 6f77 6e20 6973 2061 7765 736f 6d65 0a20  own is awesome. 
+00001870: 2020 2020 2020 2020 2020 202a 206d 6172             * mar
+00001880: 6b64 6f77 6e20 6973 206c 6573 7320 7665  kdown is less ve
+00001890: 7262 6f73 6520 7468 616e 2077 7269 7469  rbose than writi
+000018a0: 6e67 2068 746d 6c20 6279 2068 616e 640a  ng html by hand.
+000018b0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+000018c0: 656e 646d 6172 6b64 6f77 6e20 257d 0a20  endmarkdown %}. 
+000018d0: 2020 2075 0b00 0000 656e 646d 6172 6b64     u....endmarkd
+000018e0: 6f77 6e28 0100 0000 750b 0000 0065 6e64  own(....u....end
+000018f0: 6d61 726b 646f 776e 2803 0000 0074 0500  markdown(....t..
+00001900: 0000 7061 7273 6574 1200 0000 6465 6c65  ..parset....dele
+00001910: 7465 5f66 6972 7374 5f74 6f6b 656e 5247  te_first_tokenRG
+00001920: 0000 0028 0300 0000 7406 0000 0070 6172  ...(....t....par
+00001930: 7365 7274 0500 0000 746f 6b65 6e52 4800  sert....tokenRH.
+00001940: 0000 2800 0000 0028 0000 0000 733f 0000  ..(....(....s?..
+00001950: 002f 5573 6572 732f 6961 6c62 6572 742f  ./Users/ialbert/
+00001960: 6170 702f 7079 626c 7565 2d63 656e 7472  app/pyblue-centr
+00001970: 616c 2f70 7962 6c75 652f 7465 6d70 6c61  al/pyblue/templa
+00001980: 7465 7461 6773 2f70 7974 6167 732e 7079  tetags/pytags.py
+00001990: 740c 0000 006d 6172 6b64 6f77 6e5f 7461  t....markdown_ta
+000019a0: 678f 0000 0073 0600 0000 0011 0f02 0a01  g....s..........
+000019b0: 2829 0000 0074 0a00 0000 5f5f 6675 7475  ()...t....__futu
+000019c0: 7265 5f5f 5200 0000 0052 0100 0000 5202  re__R....R....R.
+000019d0: 0000 0052 0300 0000 7406 0000 0064 6a61  ...R....t....dja
+000019e0: 6e67 6f52 0400 0000 7407 0000 006c 6f67  ngoR....t....log
+000019f0: 6769 6e67 5213 0000 0052 4e00 0000 5207  gingR....RN...R.
+00001a00: 0000 0074 1100 0000 646a 616e 676f 2e75  ...t....django.u
+00001a10: 7469 6c73 2e68 746d 6c52 0500 0000 7417  tils.htmlR....t.
+00001a20: 0000 0064 6a61 6e67 6f2e 7574 696c 732e  ...django.utils.
+00001a30: 7361 6665 7374 7269 6e67 5206 0000 0074  safestringR....t
+00001a40: 0900 0000 6765 744c 6f67 6765 7252 1d00  ....getLoggerR..
+00001a50: 0000 7407 0000 004c 6962 7261 7279 7408  ..t....Libraryt.
+00001a60: 0000 0072 6567 6973 7465 7252 0a00 0000  ...registerR....
+00001a70: 5241 0000 0052 1200 0000 5228 0000 0074  RA...R....R(...t
+00001a80: 0a00 0000 7369 6d70 6c65 5f74 6167 5251  ....simple_tagRQ
+00001a90: 0000 0052 2e00 0000 5232 0000 0074 0d00  ...R....R2...t..
+00001aa0: 0000 696e 636c 7573 696f 6e5f 7461 6752  ..inclusion_tagR
+00001ab0: 3400 0000 7405 0000 0046 616c 7365 523d  4...t....FalseR=
+00001ac0: 0000 0052 1f00 0000 5236 0000 0052 4000  ...R....R6...R@.
+00001ad0: 0000 5242 0000 0052 4300 0000 5246 0000  ..RB...RC...RF..
+00001ae0: 0074 0400 0000 4e6f 6465 5247 0000 0074  .t....NodeRG...t
+00001af0: 0300 0000 7461 6752 5800 0000 2800 0000  ....tagRX...(...
+00001b00: 0028 0000 0000 2800 0000 0073 3f00 0000  .(....(....s?...
+00001b10: 2f55 7365 7273 2f69 616c 6265 7274 2f61  /Users/ialbert/a
+00001b20: 7070 2f70 7962 6c75 652d 6365 6e74 7261  pp/pyblue-centra
+00001b30: 6c2f 7079 626c 7565 2f74 656d 706c 6174  l/pyblue/templat
+00001b40: 6574 6167 732f 7079 7461 6773 2e70 7974  etags/pytags.pyt
+00001b50: 0800 0000 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001b60: 7338 0000 0022 0110 0118 010c 010c 0110  s8..."..........
+00001b70: 0110 020f 020c 0209 0509 030c 0709 1d1b  ................
+00001b80: 0b0f 0112 0618 0512 0118 070f 0115 090f  ................
+00001b90: 0112 080f 010f 071e 090c 0819 0b         .............
```

### Comparing `pyblue-3.0.2/pyblue.egg-info/PKG-INFO` & `pyblue-3.0.3/pyblue.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,106 @@
 Metadata-Version: 1.1
 Name: pyblue
-Version: 3.0.2
+Version: 3.0.3
 Summary: PyBlue
 Home-page: https://github.com/ialbert/pyblue
 Author: Istvan Albert
 Author-email: istvan.albert@gmail.com
 License: MIT
-Description: Welcome to Pyblue
-        -----------------
-        
-        A simple static site generator.
-        
-        Why another one? There are `many static <https://www.staticgen.com/>`__
-        site generators already. I found to be way too complicated, they have
-        too many rules, put this here or there, call thing this or that.
-        
-        PyBlue is different. Everything is optional, only use what you need.
-        Stays out of the way.
-        
-        From the simplest tasks:
-        
-        -  No configuration required.
-        -  Works with any existing site.
-        -  Easy to include ``markdown``.
-        -  Easy linking to other pages.
-        -  Tiny codebase, pyblue is around 500 lines in a single file!
-        
-        To more complicated:
-        
-        -  PyBlue generates the correct links even if you move pages around.
-        -  Use `Django
-           Templates <https://docs.djangoproject.com/en/1.9/ref/templates/language/>`__
-           and all the features that it offers.
-        -  Easily add data into each page (title, link name, or any arbitrary
-           content).
-        
-        Or go all the way out:
-        
-        -  Load python modules into each page.
-        -  Exposed data: database queries, results of online requests etc.
-        -  Run python code, access and modify data from inside of each page.
-        -  Extend the Django templates. Add your own ``templatetags``.
-        
-        Install
-        ~~~~~~~
-        
-        ::
-        
-            pip install pyblue --upgrade
-        
-        Or download it from the `PyBlue at
-        PyPI <https://pypi.python.org/pypi/pyblue/>`__.
-        
-        Usage
-        ~~~~~
-        
-        Launch pyblue to serve a directory
-        
-        ::
-        
-            pyblue -r docs
-        
-        View your site by visiting http:://localhost:8080
-        
-        Edit your pages and make changes. Reload the page to see your edits
-        live. Generate static output with:
-        
-        ::
-        
-            pyblue -r docs -o html
-        
-        That's all. Told you it was simple. To see extra help on options run:
-        
-        ::
-        
-            pyblue -h
-        
-        Documentation
-        ~~~~~~~~~~~~~
-        
-        -  The `PyBlue Documentation <https://ialbert.github.io/pyblue/>`__ was
-           generated with PyBlue itself.
-        
-        You can also browse the `help in source
-        format <https://github.com/ialbert/pyblue/tree/master/docs>`__ for
-        examples.
-        
-        Licensing
-        ~~~~~~~~~
-        
-        -  PyBlue is being developed by Istvan Albert see
-           https://github.com/ialbert
-        -  PyBlue has been inspired by
-           `PyGreen <https://github.com/nicolas-van/pygreen>`__ created by
-           Nicolas Vanhoren see https://github.com/nicolas-van
-        -  PyBlue uses the `MIT
-           license <https://github.com/ialbert/pyblue/blob/master/LICENSE.txt>`__.
+Description: Welcome to PyBlue
+        -----------------
+        
+        A simple static site generator.
+        
+        Why another one? There are `many static <https://www.staticgen.com/>`__
+        site generators already. I found most to be way too complicated, too
+        many conventions and rules: put this here or there, call it this or
+        that. It was too tiring to keep up.
+        
+        PyBlue is different. Everything is optional, nothing is required, use
+        only what you need. It basically stays out of the way.
+        
+        Simple things are very easy:
+        
+        -  No configuration required.
+        -  Works with any existing site.
+        -  Easy to include ``markdown``.
+        -  Easy linking to other pages.
+        -  Tiny codebase, pyblue is around 500 lines in a single file!
+        
+        Complicated tasks are easy:
+        
+        -  PyBlue generates the correct links even if you move pages around.
+        -  Use `Django
+           Templates <https://docs.djangoproject.com/en/1.9/ref/templates/language/>`__
+           and all the features that it offers.
+        -  Easily add data into each page (title, link name, or any arbitrary
+           content).
+        
+        And you can go all the way out if you really want to:
+        
+        -  Load python modules into each page.
+        -  Exposed data: database queries, results of online requests etc.
+        -  Run python code, access and modify data from inside of each page.
+        -  Extend the Django templates. Add your own ``templatetags``.
+        
+        Install
+        ~~~~~~~
+        
+        ::
+        
+            pip install pyblue --upgrade
+        
+        Or download it from the `PyBlue at
+        PyPI <https://pypi.python.org/pypi/pyblue/>`__.
+        
+        Usage
+        ~~~~~
+        
+        Launch pyblue to serve a directory
+        
+        ::
+        
+            pyblue -r docs
+        
+        View your site by visiting http:://localhost:8080
+        
+        Edit your pages and make changes. Reload the page to see your edits
+        live. Generate static output with:
+        
+        ::
+        
+            pyblue -r docs -o html
+        
+        That's all. Told you it was simple. To see extra help on options run:
+        
+        ::
+        
+            pyblue -h
+        
+        Documentation
+        ~~~~~~~~~~~~~
+        
+        -  The `PyBlue Documentation <https://ialbert.github.io/pyblue/>`__ was
+           generated with PyBlue itself.
+        
+        You can also browse the `help in source
+        format <https://github.com/ialbert/pyblue/tree/master/docs>`__ for
+        examples.
+        
+        Licensing
+        ~~~~~~~~~
+        
+        -  PyBlue is being developed by Istvan Albert see
+           https://github.com/ialbert
+        -  PyBlue has been inspired by
+           `PyGreen <https://github.com/nicolas-van/pygreen>`__ created by
+           Nicolas Vanhoren see https://github.com/nicolas-van
+        -  PyBlue uses the `MIT
+           license <https://github.com/ialbert/pyblue/blob/master/LICENSE.txt>`__.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyblue-3.0.2/pyblue.egg-info/SOURCES.txt` & `pyblue-3.0.3/pyblue.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 pyblue.egg-info/requires.txt
 pyblue.egg-info/top_level.txt
 pyblue/.idea/.name
 pyblue/.idea/encodings.xml
 pyblue/.idea/misc.xml
 pyblue/.idea/modules.xml
 pyblue/.idea/pyblue.iml
-pyblue/.idea/vcs.xml
 pyblue/.idea/workspace.xml
 pyblue/.idea/scopes/scope_settings.xml
 pyblue/templates/pyblue_base.html
 pyblue/templates/say_hello.html
 pyblue/templates/site_assets.html
 pyblue/templates/thumbnail.html
 pyblue/templates/toggle_box.html
```

### Comparing `pyblue-3.0.2/README.md` & `pyblue-3.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Welcome to Pyblue
+## Welcome to PyBlue
 
 A simple static site generator.
 
 Why another one? There are [many static](https://www.staticgen.com/) site
 generators already. I found most to be way too complicated,
 too many conventions and rules: put this here or there, call it this or that.
 It was too tiring to keep up.
```

### Comparing `pyblue-3.0.2/README.rst` & `pyblue-3.0.3/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,91 @@
-Welcome to Pyblue
------------------
-
-A simple static site generator.
-
-Why another one? There are `many static <https://www.staticgen.com/>`__
-site generators already. I found to be way too complicated, they have
-too many rules, put this here or there, call thing this or that.
-
-PyBlue is different. Everything is optional, only use what you need.
-Stays out of the way.
-
-From the simplest tasks:
-
--  No configuration required.
--  Works with any existing site.
--  Easy to include ``markdown``.
--  Easy linking to other pages.
--  Tiny codebase, pyblue is around 500 lines in a single file!
-
-To more complicated:
-
--  PyBlue generates the correct links even if you move pages around.
--  Use `Django
-   Templates <https://docs.djangoproject.com/en/1.9/ref/templates/language/>`__
-   and all the features that it offers.
--  Easily add data into each page (title, link name, or any arbitrary
-   content).
-
-Or go all the way out:
-
--  Load python modules into each page.
--  Exposed data: database queries, results of online requests etc.
--  Run python code, access and modify data from inside of each page.
--  Extend the Django templates. Add your own ``templatetags``.
-
-Install
-~~~~~~~
-
-::
-
-    pip install pyblue --upgrade
-
-Or download it from the `PyBlue at
-PyPI <https://pypi.python.org/pypi/pyblue/>`__.
-
-Usage
-~~~~~
-
-Launch pyblue to serve a directory
-
-::
-
-    pyblue -r docs
-
-View your site by visiting http:://localhost:8080
-
-Edit your pages and make changes. Reload the page to see your edits
-live. Generate static output with:
-
-::
-
-    pyblue -r docs -o html
-
-That's all. Told you it was simple. To see extra help on options run:
-
-::
-
-    pyblue -h
-
-Documentation
-~~~~~~~~~~~~~
-
--  The `PyBlue Documentation <https://ialbert.github.io/pyblue/>`__ was
-   generated with PyBlue itself.
-
-You can also browse the `help in source
-format <https://github.com/ialbert/pyblue/tree/master/docs>`__ for
-examples.
-
-Licensing
-~~~~~~~~~
-
--  PyBlue is being developed by Istvan Albert see
-   https://github.com/ialbert
--  PyBlue has been inspired by
-   `PyGreen <https://github.com/nicolas-van/pygreen>`__ created by
-   Nicolas Vanhoren see https://github.com/nicolas-van
--  PyBlue uses the `MIT
-   license <https://github.com/ialbert/pyblue/blob/master/LICENSE.txt>`__.
+Welcome to PyBlue
+-----------------
+
+A simple static site generator.
+
+Why another one? There are `many static <https://www.staticgen.com/>`__
+site generators already. I found most to be way too complicated, too
+many conventions and rules: put this here or there, call it this or
+that. It was too tiring to keep up.
+
+PyBlue is different. Everything is optional, nothing is required, use
+only what you need. It basically stays out of the way.
+
+Simple things are very easy:
+
+-  No configuration required.
+-  Works with any existing site.
+-  Easy to include ``markdown``.
+-  Easy linking to other pages.
+-  Tiny codebase, pyblue is around 500 lines in a single file!
+
+Complicated tasks are easy:
+
+-  PyBlue generates the correct links even if you move pages around.
+-  Use `Django
+   Templates <https://docs.djangoproject.com/en/1.9/ref/templates/language/>`__
+   and all the features that it offers.
+-  Easily add data into each page (title, link name, or any arbitrary
+   content).
+
+And you can go all the way out if you really want to:
+
+-  Load python modules into each page.
+-  Exposed data: database queries, results of online requests etc.
+-  Run python code, access and modify data from inside of each page.
+-  Extend the Django templates. Add your own ``templatetags``.
+
+Install
+~~~~~~~
+
+::
+
+    pip install pyblue --upgrade
+
+Or download it from the `PyBlue at
+PyPI <https://pypi.python.org/pypi/pyblue/>`__.
+
+Usage
+~~~~~
+
+Launch pyblue to serve a directory
+
+::
+
+    pyblue -r docs
+
+View your site by visiting http:://localhost:8080
+
+Edit your pages and make changes. Reload the page to see your edits
+live. Generate static output with:
+
+::
+
+    pyblue -r docs -o html
+
+That's all. Told you it was simple. To see extra help on options run:
+
+::
+
+    pyblue -h
+
+Documentation
+~~~~~~~~~~~~~
+
+-  The `PyBlue Documentation <https://ialbert.github.io/pyblue/>`__ was
+   generated with PyBlue itself.
+
+You can also browse the `help in source
+format <https://github.com/ialbert/pyblue/tree/master/docs>`__ for
+examples.
+
+Licensing
+~~~~~~~~~
+
+-  PyBlue is being developed by Istvan Albert see
+   https://github.com/ialbert
+-  PyBlue has been inspired by
+   `PyGreen <https://github.com/nicolas-van/pygreen>`__ created by
+   Nicolas Vanhoren see https://github.com/nicolas-van
+-  PyBlue uses the `MIT
+   license <https://github.com/ialbert/pyblue/blob/master/LICENSE.txt>`__.
```

### Comparing `pyblue-3.0.2/setup.py` & `pyblue-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyblue-3.0.2/tests/.DS_Store` & `pyblue-3.0.3/tests/.DS_Store`

 * *Files identical despite different names*

