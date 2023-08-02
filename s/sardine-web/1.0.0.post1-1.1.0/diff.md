# Comparing `tmp/sardine-web-1.0.0.post1.tar.gz` & `tmp/sardine-web-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sardine-web-1.0.0.post1.tar", last modified: Tue Jul 18 23:11:21 2023, max compression
+gzip compressed data, was "sardine-web-1.1.0.tar", last modified: Wed Aug  2 09:59:38 2023, max compression
```

## Comparing `sardine-web-1.0.0.post1.tar` & `sardine-web-1.1.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.568925 sardine-web-1.0.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.552925 sardine-web-1.0.0.post1/sardine_web/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web/client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.552925 sardine-web-1.0.0.post1/sardine_web/client/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web/client/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)   113421 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    80823 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/css/solid.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.552925 sardine-web-1.0.0.post1/sardine_web/client/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.560925 sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.560925 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/
--rw-r--r--   0 runner    (1001) docker     (123)   188876 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188468 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188244 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188252 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188604 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)  1605860 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   283288 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    86636 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   103524 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90904 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    45086 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/postcss.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/src/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/AppSettings.ts
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/Editor.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/EditorSetup.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/RunnerService.ts
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/counter.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/src/help/
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/help/generalHelp.ts
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/help/keybindingsHelp.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/highlightSelection.ts
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/main.ts
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/output.css
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/style copy.css
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/src/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/themes/sardineTheme.ts
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/tailwind.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)    58844 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/server/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/server/flask_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 23:11:21.568925 sardine-web-1.0.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.237943 sardine-web-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-08-02 09:59:25.000000 sardine-web-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-02 09:59:25.000000 sardine-web-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-02 09:59:38.237943 sardine-web-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 09:59:25.000000 sardine-web-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-02 09:59:25.000000 sardine-web-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.217943 sardine-web-1.1.0/sardine_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.221943 sardine-web-1.1.0/sardine_web/client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.213943 sardine-web-1.1.0/sardine_web/client/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.221943 sardine-web-1.1.0/sardine_web/client/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   113421 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    80823 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/css/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/css/solid.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.225943 sardine-web-1.1.0/sardine_web/client/assets/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.213943 sardine-web-1.1.0/sardine_web/client/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.225943 sardine-web-1.1.0/sardine_web/client/fonts/Droid/
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Droid/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.225943 sardine-web-1.1.0/sardine_web/client/fonts/Fira/
+-rw-r--r--   0 runner    (1001) docker     (123)   188876 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188468 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188244 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188252 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188604 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/Fira/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.229943 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1605860 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   283288 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.233943 sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    86636 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   103524 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90904 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    45086 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/postcss.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.233943 sardine-web-1.1.0/sardine_web/client/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/AppSettings.ts
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/Editor.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/EditorSetup.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/RunnerService.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/counter.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.237943 sardine-web-1.1.0/sardine_web/client/src/help/
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/help/generalHelp.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/help/keybindingsHelp.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/highlightSelection.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/main.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/output.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/style copy.css
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.237943 sardine-web-1.1.0/sardine_web/client/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/themes/sardineTheme.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/tailwind.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    58844 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/client/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.237943 sardine-web-1.1.0/sardine_web/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-08-02 09:59:25.000000 sardine-web-1.1.0/sardine_web/server/flask_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:59:38.217943 sardine-web-1.1.0/sardine_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-02 09:59:38.000000 sardine-web-1.1.0/sardine_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-02 09:59:38.000000 sardine-web-1.1.0/sardine_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:59:38.000000 sardine-web-1.1.0/sardine_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-02 09:59:38.000000 sardine-web-1.1.0/sardine_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-02 09:59:38.000000 sardine-web-1.1.0/sardine_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 09:59:38.000000 sardine-web-1.1.0/sardine_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:59:38.237943 sardine-web-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-02 09:59:25.000000 sardine-web-1.1.0/setup.py
```

### Comparing `sardine-web-1.0.0.post1/LICENSE.txt` & `sardine-web-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/PKG-INFO` & `sardine-web-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sardine-web
-Version: 1.0.0.post1
+Version: 1.1.0
 Summary: Official web editor plugin for sardine-system
 Author: Raphaël Forment, thegamecracks
 Author-email: raphael.forment@gmail.com
 License: GPL-3.0-only
 Project-URL: Homepage, https://sardine.raphaelforment.fr
 Project-URL: Documentation, https://sardine.raphaelforment.fr
 Project-URL: Source Code, https://github.com/sardine-system/sardine-web
```

### Comparing `sardine-web-1.0.0.post1/README.md` & `sardine-web-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/pyproject.toml` & `sardine-web-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/__init__.py` & `sardine-web-1.1.0/sardine_web/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-__version__ = "1.0.0.post1"
+__version__ = "1.1.0"
 
 
 def install_web(main: click.Group):
     from sardine.console import ConsoleManager
 
     @main.command(
         short_help="Starts sardine as a web server",
```

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.css` & `sardine-web-1.1.0/sardine_web/client/assets/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.min.css` & `sardine-web-1.1.0/sardine_web/client/assets/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/css/solid.css` & `sardine-web-1.1.0/sardine_web/client/assets/css/solid.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.ttf` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.woff2` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.ttf` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.woff2` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.ttf` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.woff2` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2` & `sardine-web-1.1.0/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff` & `sardine-web-1.1.0/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Light.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Light.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/stylesheet.css` & `sardine-web-1.1.0/sardine_web/client/fonts/Fira/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs5.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff2` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs5.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs7.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff2` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs7.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs9.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff2` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/jgs9.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/stylesheet.css` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2` & `sardine-web-1.1.0/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/OFL.txt` & `sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf` & `sardine-web-1.1.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/index.html` & `sardine-web-1.1.0/sardine_web/client/index.html`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/package-lock.json` & `sardine-web-1.1.0/sardine_web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/package.json` & `sardine-web-1.1.0/sardine_web/client/package.json`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/AppSettings.ts` & `sardine-web-1.1.0/sardine_web/client/src/AppSettings.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/EditorSetup.ts` & `sardine-web-1.1.0/sardine_web/client/src/EditorSetup.ts`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     syntaxHighlighting, 
     indentOnInput, 
     bracketMatching,
     foldKeymap
 } from "@codemirror/language"
 import {
     defaultKeymap, 
-    historyKeymap
+    historyKeymap,
+    history,
 } from "@codemirror/commands"
 import {
     searchKeymap, 
     highlightSelectionMatches
 } from "@codemirror/search"
 import {
     autocompletion, 
@@ -81,15 +82,15 @@
 
 export const editorSetup: Extension = (() => [
     materialDark,
     lineNumbers(),
     python(),
     highlightActiveLineGutter(),
     highlightSpecialChars(),
-    // history(),
+    history(),
     // foldGutter(),
     drawSelection(),
     dropCursor(),
     EditorState.allowMultipleSelections.of(true),
     indentOnInput(),
     syntaxHighlighting(defaultHighlightStyle, {fallback: true}),
     bracketMatching(),
@@ -104,8 +105,8 @@
         ...defaultKeymap,
         ...searchKeymap,
         ...historyKeymap,
         ...foldKeymap,
         ...completionKeymap,
         ...lintKeymap
     ])
-])()
+])()
```

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/RunnerService.ts` & `sardine-web-1.1.0/sardine_web/client/src/RunnerService.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/help/generalHelp.ts` & `sardine-web-1.1.0/sardine_web/client/src/help/generalHelp.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/help/keybindingsHelp.ts` & `sardine-web-1.1.0/sardine_web/client/src/help/keybindingsHelp.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/highlightSelection.ts` & `sardine-web-1.1.0/sardine_web/client/src/highlightSelection.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/main.ts` & `sardine-web-1.1.0/sardine_web/client/src/main.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/output.css` & `sardine-web-1.1.0/sardine_web/client/src/output.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/src/style copy.css` & `sardine-web-1.1.0/sardine_web/client/src/style copy.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/tsconfig.json` & `sardine-web-1.1.0/sardine_web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/client/yarn.lock` & `sardine-web-1.1.0/sardine_web/client/yarn.lock`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/sardine_web/server/flask_server.py` & `sardine-web-1.1.0/sardine_web/server/flask_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+from __future__ import annotations
+
+import contextlib
+import json
 import logging
 import mimetypes
 import os
 import platform
 import subprocess
 import webbrowser
 from pathlib import Path
 from threading import Thread
-from typing import Optional
-import json
+from typing import TYPE_CHECKING, Any
 
-from appdirs import *
+from appdirs import user_data_dir
 from flask import (
     Flask,
     Response,
     jsonify,
     request,
     send_from_directory,
 )
 from flask_cors import CORS
 from pygtail import Pygtail
 from rich import print
 
+if TYPE_CHECKING:
+    from sardine.console import AsyncIOInteractiveConsole
+
 # Monkey-patching to prevent some initial printing
 # More info can be found here: https://gist.github.com/daryltucker/e40c59a267ea75db12b1
 import flask.cli
 
 flask.cli.show_server_banner = lambda *args: None
 logging.getLogger("werkzeug").disabled = True
 mimetypes.add_type("text/css", ".css")
@@ -45,54 +51,52 @@
     """
     This is a small Flask WebServer serving the Sardine Code Editor. This web server is
     also charged of loading / dispatching locally stored buffer files that act as a
     temporary memory for the editor. Files are stored in plain-text in the Sardine conf-
     iguration folder under the buffers/folder.
     """
 
-    def __init__(self, host="localhost", port=8000):
+    def __init__(self, host: str = "localhost", port: int = 8000):
         self.host, self.port = host, port
         self.reset_log_file()
         self.local_files = self.load_buffer_files()
 
-    def reset_log_file(self):
+    def reset_log_file(self) -> None:
         """Reset the log file on application start. Writing to the file
         and immediately closing is effectively erasing the content."""
-        open(LOG_FILE, "w", encoding="utf-8").close()
+        with contextlib.suppress(FileNotFoundError):
+            os.truncate(LOG_FILE, 0)
 
     def check_buffer_files(self) -> None:
         """This function will check the integrity of the buffer folder."""
-        buffer_folder: Path = Path(USER_DIR / "buffers")
+        buffer_folder = USER_DIR / "buffers"
         for filename in FILENAMES:
-            check_file: Path = buffer_folder / filename
-            if not check_file.exists():
-                with open(check_file, "w", encoding="utf-8") as f:
-                    f.write("")
-            else:
-                pass
+            buffer_file = buffer_folder / filename
+            buffer_file.touch()
 
-    def load_buffer_files(self) -> Optional[dict]:
+    def load_buffer_files(self) -> dict[str, str] | None:
         """
         Loading buffer files from a local folder. If the folder doesn't exist, this
         function will automatically create it and load empty files for the first round.
         If the folder exists, read files in their current state
         """
-        buffer_files: dict = {}
+        buffer_files: dict[str, str] = {}
 
         # Creating the folder to store text files if it doesn't exist
-        if not (USER_DIR / "buffers").is_dir():
+        buffer_folder = USER_DIR / "buffers"
+        if not buffer_folder.is_dir():
             try:
-                (USER_DIR / "buffers").mkdir()
+                buffer_folder.mkdir()
                 for filename in FILENAMES:
-                    print(f"Creating file {filename}.py.")
-                    with open(filename, "w", encoding="utf-8") as f:
-                        f.write("")
-                    buffer_files[filename] = f"{filename}"
-                    return buffer_files
-            except FileExistsError or OSError:
+                    print(f"Creating {filename}")
+                    buffer_file = buffer_folder / filename
+                    buffer_file.touch()
+                    buffer_files[filename] = filename
+                return buffer_files
+            except OSError:
                 print("[red]Fishery was not able to create web editor files![/red]")
                 exit()
         # If it already exists, read files from the folder
         else:
             self.check_buffer_files()
             buffer_folder = Path(USER_DIR / "buffers")
             for file in os.listdir(buffer_folder):
@@ -100,35 +104,39 @@
                 if str(file).startswith("."):
                     continue
                 path = (buffer_folder / file).as_posix()
                 with open(path, "r", encoding="utf-8") as buffer:
                     buffer_files[file] = buffer.read()
             return buffer_files
 
-    def start(self, console):
+    def start(self, console: AsyncIOInteractiveConsole) -> None:
         app = server_factory(console)
 
         # Start the application
         app.run(
             host=self.host,
             port=self.port,
             use_reloader=False,
             debug=False,
         )
 
-    def start_in_thread(self, console):
-        Thread(target=self.start, args=(console,)).start()
+    def start_in_thread(self, console: AsyncIOInteractiveConsole) -> None:
+        # FIXME: daemon=True is not a good idea because we can't perform
+        #        any cleanup, however the alternative is users having to
+        #        SIGKILL the hanging process which is no better.
+        #        This webserver should be re-written to run as a subprocess.
+        Thread(target=self.start, args=(console,), daemon=True).start()
 
     def open_in_browser(self):
         address = f"http://{self.host}:{self.port}"
         print(f"[red]Opening embedded editor at: [yellow]{address}[/yellow][/red]")
         webbrowser.open(address)
 
 
-def server_factory(console):
+def server_factory(console: AsyncIOInteractiveConsole) -> Flask:
     app = Flask(__name__, static_folder="../client/dist")
     app.logger.disabled = True  # Disable some of the logging
     CORS(app, resources={r"/*": {"origins": "*"}})
 
     @app.route("/save", methods=["POST"])
     def save_files_to_disk() -> str:
         try:
@@ -141,36 +149,37 @@
                         # formatting.
                         new_file.write(
                             "\n".join(content) if isinstance(content, list) else content
                         )
                 return "OK"
         except Exception as e:
             print(e)
+        finally:
             return "FAILED"
 
     @app.post("/open_folder")
-    def open_folder():
+    def open_folder() -> str:
         """Open Sardine Default Folder using the default file Explorer"""
 
-        def showFileExplorer(file):  # Path to file (string)
+        def showFileExplorer(path: str) -> None:
             if platform.system() == "Windows":
-                os.startfile(file)
+                os.startfile(path)
             elif platform.system() == "Darwin":
-                subprocess.call(["open", "-R", file])
+                subprocess.call(["open", "-R", path])
             else:
-                subprocess.Popen(["xdg-open", file])
+                subprocess.Popen(["xdg-open", path])
 
         # Open the file explorer
         showFileExplorer(str(USER_DIR))
 
         return "OK"
 
     @app.post("/execute")
-    def execute():
-        code = request.json["code"]
+    def execute() -> dict[str, Any]:
+        code: str = request.json["code"]  # type: ignore
         try:
             # If `code` contains multiple statements, an exception occurs but
             # code.InteractiveInterpreter.runsource swallows it.
             # This means `console`s buffer will fill up with garbage and break
             # any subsequent correctly-formed statements.
             # So, reset the buffer first.
             console.resetbuffer()
@@ -179,22 +188,23 @@
         except Exception as e:
             # Due to the above, there's no way to send a SyntaxError back to the client.
             return {"error": str(e)}
 
     # Serve App
     @app.route("/", defaults={"path": ""})
     @app.route("/<path:path>")
-    def serve(path):
+    def serve(path: str) -> Response:
+        assert app.static_folder is not None
         if path != "" and os.path.exists(app.static_folder + "/" + path):
             return send_from_directory(app.static_folder, path)
         else:
             return send_from_directory(app.static_folder, "index.html")
 
     @app.route("/log")
-    def progress_log():
+    def progress_log() -> Response:
         def generate():
             try:
                 unread_lines = Pygtail(
                     str(LOG_FILE),
                     every_n=1,
                     full_lines=True,
                     encoding="utf-8",
@@ -205,15 +215,15 @@
                     yield "data:" + str("") + "\n\n"
             except Exception as e:
                 yield "data: An error occured while reading the logfile\n\n"
 
         return Response(generate(), mimetype="text/plain")
 
     @app.route("/config")
-    def get_config():
+    def get_config() -> Response:
         try:
             with open(USER_DIR / "config.json", "r") as f:
                 config_data = json.load(f)["config"]
             response = jsonify(config_data)
         except Exception as e:
             print("Error while reading config.json:", e)
             response = jsonify({"error": "Internal server error"})
@@ -227,15 +237,15 @@
 
         with open(USER_DIR / "config.json", "w") as f:
             json.dump(wrapped_data, f)
 
         return "OK"
 
     @app.route("/text_files", methods=["GET"])
-    def get_text_files():
+    def get_text_files() -> Response:
         files = {}
         for file_name in os.listdir(USER_DIR / "buffers"):
             if file_name.endswith(".py"):
                 buffer_directory = USER_DIR / "buffers"
                 with open((buffer_directory / file_name).as_posix(), "r") as f:
                     files[file_name] = f.read()
         files = jsonify(files)
```

### Comparing `sardine-web-1.0.0.post1/sardine_web.egg-info/PKG-INFO` & `sardine-web-1.1.0/sardine_web.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sardine-web
-Version: 1.0.0.post1
+Version: 1.1.0
 Summary: Official web editor plugin for sardine-system
 Author: Raphaël Forment, thegamecracks
 Author-email: raphael.forment@gmail.com
 License: GPL-3.0-only
 Project-URL: Homepage, https://sardine.raphaelforment.fr
 Project-URL: Documentation, https://sardine.raphaelforment.fr
 Project-URL: Source Code, https://github.com/sardine-system/sardine-web
```

### Comparing `sardine-web-1.0.0.post1/sardine_web.egg-info/SOURCES.txt` & `sardine-web-1.1.0/sardine_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0.post1/setup.py` & `sardine-web-1.1.0/setup.py`

 * *Files identical despite different names*

