# Comparing `tmp/pyside-app-core-0.1.6.tar.gz` & `tmp/pyside-app-core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside-app-core-0.1.6.tar", last modified: Mon Jun  5 20:46:14 2023, max compression
+gzip compressed data, was "pyside-app-core-0.1.7.tar", last modified: Mon Jul 24 18:33:33 2023, max compression
```

## Comparing `pyside-app-core-0.1.6.tar` & `pyside-app-core-0.1.7.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42086 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.049160 pyside-app-core-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.053160 pyside-app-core-0.1.6/src/pyside_app_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/basic_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/encode_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/errors/serial_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/generate_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/down-arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/grab-corner.svg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/reload.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-down/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-up/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/standard_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/style_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/log/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/pixel_val.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/util/s_color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.061160 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/error_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/window_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/window_shade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/menu_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/multi_combo_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/object_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/settings_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/window_settings_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/application_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/debug_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/platform_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/serial_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.065160 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/float_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/src/pyside_app_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/types/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.069160 pyside-app-core-0.1.6/src/pyside_app_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-05 20:45:57.000000 pyside-app-core-0.1.6/src/pyside_app_core/utils/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:14.057160 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42086 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 20:46:14.000000 pyside-app-core-0.1.6/src/pyside_app_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    42292 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.637434 pyside-app-core-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.637434 pyside-app-core-0.1.7/src/pyside_app_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/basic_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/encode_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/errors/serial_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/generate_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/down-arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/grab-corner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/reload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-down/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-up/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/standard_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/style_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/pixel_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/s_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/util/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/base_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/error_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_shade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/menu_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/multi_combo_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/object_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/settings_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/window_settings_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/application_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/debug_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/platform_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/serial_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.645434 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/float_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/src/pyside_app_core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/types/numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.649434 pyside-app-core-0.1.7/src/pyside_app_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 18:33:15.000000 pyside-app-core-0.1.7/src/pyside_app_core/utils/compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:33.641434 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42292 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 18:33:33.000000 pyside-app-core-0.1.7/src/pyside_app_core.egg-info/top_level.txt
```

### Comparing `pyside-app-core-0.1.6/LICENSE` & `pyside-app-core-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/PKG-INFO` & `pyside-app-core-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.6
+Version: 0.1.7
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,24 +681,27 @@
 Project-URL: Homepage, https://github.com/leocov-dev/pyside-app-core
 Keywords: pyside,pyside6,frameless,app,style
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Desktop Environment
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyside-app-core
 
-Custom style, widgets, and utilities for PySide 6.5 applications.
+Custom style, widgets, and utilities for cross-platform PySide 6.5 applications with a focus on 'frameless' styling.
 
-> This project should be considered experimental and subject to breaking changes at any time.
+> This project should be considered experimental and subject to breaking changes until a 1.0.0 release.
 
 
 ### Install
 
 ```shell
 $ pip install pyside-app-core
 ```
```

### Comparing `pyside-app-core-0.1.6/README.md` & `pyside-app-core-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyside-app-core
 
-Custom style, widgets, and utilities for PySide 6.5 applications.
+Custom style, widgets, and utilities for cross-platform PySide 6.5 applications with a focus on 'frameless' styling.
 
-> This project should be considered experimental and subject to breaking changes at any time.
+> This project should be considered experimental and subject to breaking changes until a 1.0.0 release.
 
 
 ### Install
 
 ```shell
 $ pip install pyside-app-core
 ```
```

### Comparing `pyside-app-core-0.1.6/pyproject.toml` & `pyside-app-core-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyside-app-core"
-version = "0.1.6"
+version = "0.1.7"
 description = "Framework for PySide Applications"
 readme = "README.md"
 authors = [{ name = "Leo Covarrubias", email = "leo@leocov.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Desktop Environment",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Typing :: Typed",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["pyside", "pyside6", "frameless", "app", "style"]
 dependencies = [
     "pyside6 ~= 6.5.0",
     "jinja2 ~= 3.1.2",
 ]
 requires-python = ">=3.11"
@@ -59,15 +62,15 @@
     "src.pyside_app_core",
 ]
 forbidden_modules = [
     "examples.simple_app",
 ]
 
 [tool.bumpver]
-current_version = "0.1.6"
+current_version = "0.1.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/constants.py` & `pyside-app-core-0.1.7/src/pyside_app_core/constants.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/errors/excepthook.py` & `pyside-app-core-0.1.7/src/pyside_app_core/errors/excepthook.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/errors/serial_errors.py` & `pyside-app-core-0.1.7/src/pyside_app_core/errors/serial_errors.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/__main__.py` & `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/generate_resources.py` & `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/generate_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/console.svg` & `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/console.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/reload.svg` & `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/reload.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/icons/save.svg` & `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/icons/save.svg`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/standard_resources.py` & `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/standard_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/generator_utils/templates/style.qss.jinja2` & `pyside-app-core-0.1.7/src/pyside_app_core/generator_utils/templates/style.qss.jinja2`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/log/__init__.py` & `pyside-app-core-0.1.7/src/pyside_app_core/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/log/logger.py` & `pyside-app-core-0.1.7/src/pyside_app_core/log/logger.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/style.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/style.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/util/s_color.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/util/s_color.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/about_dialog.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/about_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/error_dialog.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/error_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_dialog.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/base_window.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/base_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+from typing import Tuple
+
 from PySide6.QtCore import QPoint, QRect, QSize, Qt, Signal
 from PySide6.QtGui import (
-    QBitmap,
     QBrush,
-    QColor,
     QMouseEvent,
     QPainter,
     QPainterPath,
     QPaintEvent,
     QPen,
     QResizeEvent,
 )
-from PySide6.QtWidgets import QLabel, QSizePolicy, QVBoxLayout, QWidget
+from PySide6.QtWidgets import QLabel, QSizePolicy, QVBoxLayout
 
-from pyside_app_core.qt.style import QssTheme
-from pyside_app_core.qt.widgets.frameless.window_shade import FramelessWindowShade
 from pyside_app_core.qt.widgets.frameless.window_actions import WindowActions
-from pyside_app_core.services import application_service
+from pyside_app_core.qt.widgets.frameless.window_shade import FramelessWindowShade
+from pyside_app_core.services import application_service, platform_service
 
 
 class FramelessBaseMixin:
     close_window = Signal()
 
     def __init__(
         self,
@@ -147,14 +146,15 @@
 
         p.setPen(QPen(self._theme.background_color.lighter(130), 2))
         p.drawRoundedRect(
             draw_rect,
             self._theme.win_corner_radius - 2,
             self._theme.win_corner_radius - 2,
         )
+        p.setClipping(False)
 
     def _on_maximize(self):
         if self.isMaximized():
             self.setWindowState(Qt.WindowState.WindowNoState)
         else:
             self.setWindowState(Qt.WindowState.WindowMaximized)
 
@@ -171,15 +171,15 @@
             self.update()
 
         super().mouseMoveEvent(event)
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
         if (
             (event.buttons() & Qt.MouseButton.LeftButton) == Qt.MouseButton.LeftButton
-            and self.window_bar_rect.contains(event.pos())
+            and self.window_bar_geo.contains(event.pos())
             and not self._window_actions.geometry().contains(event.pos())
         ):
             self._moving = True
 
             win = self.window()
             rect = win.rect()
             pos: QPoint = win.mapToGlobal(event.pos())
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/main_window.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/main_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide6.QtCore import QRect, Qt
+from PySide6.QtCore import QPoint, QRect, Qt
 from PySide6.QtGui import QAction
 from PySide6.QtWidgets import QMainWindow, QWidget
 
 from pyside_app_core.qt.widgets.about_dialog import AboutDialog
 from pyside_app_core.qt.widgets.frameless.base_window import FramelessBaseMixin
 from pyside_app_core.qt.widgets.menu_ctx import MenuBarContext
 from pyside_app_core.qt.widgets.tool_bar_ctx import ToolBarContext
@@ -67,9 +67,9 @@
         return self._menu_bar
 
     @property
     def tool_bar(self):
         return self._tool_bar
 
     @property
-    def window_bar_rect(self) -> QRect:
-        return self.tool_bar.geometry()
+    def window_bar_geo(self) -> QRect:
+        return QRect(QPoint(0, 0), self.tool_bar.geometry().bottomRight())
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/window_actions.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from enum import IntEnum
 from typing import Callable, NamedTuple, Tuple
 
-from PySide6.QtCore import QEvent, QLine, QRect, Qt, Signal
+from PySide6.QtCore import QEvent, QLine, QPoint, QRect, Qt, Signal
 from PySide6.QtGui import (
     QBrush,
     QColor,
     QMouseEvent,
     QPainter,
+    QPainterPath,
     QPaintEvent,
     QPen,
     QResizeEvent,
 )
 from PySide6.QtWidgets import QWidget
 
 from pyside_app_core.services import application_service, platform_service
@@ -60,45 +61,45 @@
 
         _top_offset = self.contentsMargins().top() if platform_service.is_macos else 0
         self._side_offset = (
             self.contentsMargins().left()
             if platform_service.is_macos
             else self.contentsMargins().right()
         )
-        if platform_service.is_macos:
-            _width = 14
-        elif platform_service.is_windows:
-            _width = 45
-        else:
-            _width = 20
 
         if platform_service.is_macos:
+            _width = 14
             _height = 14
+            _spacing = 5
         elif platform_service.is_windows:
+            _width = 45
             _height = 35
+            _spacing = 3
         else:
+            _width = 20
             _height = 20
-
-        _spacing = (
-            3 if platform_service.is_windows else 5 if platform_service.is_macos else 10
-        )
+            _spacing = 10
 
         self._a_rect = QRect(self._side_offset, _top_offset, _width, _height)
         self._b_rect = self._a_rect.translated(_width + _spacing, 0)
         self._c_rect = self._b_rect.translated(_width + _spacing, 0)
 
-        self.container_height = (
-            self._a_rect.y() + self._a_rect.height()
-            if platform_service.is_windows
-            else self._a_rect.y() + self._a_rect.height() + self.contentsMargins().top()
-            if platform_service.is_macos
-            else self._a_rect.y()
-            + self._a_rect.height()
-            + self.contentsMargins().top() * 2
-        )
+        if platform_service.is_macos:
+            self.container_height = (
+                self._a_rect.y() + self._a_rect.height() + self.contentsMargins().top()
+            )
+        elif platform_service.is_windows:
+            self.container_height = self._a_rect.y() + self._a_rect.height()
+        else:
+            self.container_height = (
+                self._a_rect.y()
+                + self._a_rect.height()
+                + self.contentsMargins().top() * 2
+            )
+
         self.container_width = self._c_rect.x() + self._c_rect.width()
 
         self.setFixedHeight(self.container_height)
         self.setFixedWidth(self.container_width)
 
         _rect_list = [
             self._a_rect,
@@ -136,36 +137,30 @@
                     self.parent().windowFlags() & Qt.WindowType.WindowCloseButtonHint
                 )
                 > 0,
             ),
         ]
 
         _order = [2, 0, 1] if platform_service.is_macos else [0, 1, 2]
+
         self._rect_map = []
         for i, o in enumerate(_order):
             self._rect_map.append((_rect_list[i], _button_data[o]))
 
-    @property
-    def min_bounds(self) -> QRect:
-        return QRect(
-            self._rect_map[0][0].topLeft(), self._rect_map[-1][0].bottomRight()
-        )
-
     def paintEvent(self, event: QPaintEvent) -> None:
         p = QPainter(self)
         p.setRenderHint(QPainter.RenderHint.Antialiasing)
 
         p.setPen(Qt.GlobalColor.transparent)
         p.setBrush(Qt.GlobalColor.transparent)
 
         for rect, data in self._rect_map:
             enabled = self.isActiveWindow() and data.enabled_fn()
 
-            c_background = data.color if enabled else self._theme.win_action_inactive
-            self._draw_shape(p, rect, c_background, data.action, enabled)
+            self._draw_button(p, rect, data.color, data.action, enabled)
 
             if platform_service.is_macos and not enabled:
                 pass
             else:
                 c_shape = data.color if enabled else data.color.darker(300)
                 c_shape = c_shape.darker(200) if platform_service.is_macos else c_shape
                 data.shape_fn(p, rect, c_shape, data.action)
@@ -241,59 +236,62 @@
                 self.contentsMargins().top(),
                 self.width(),
                 self.height(),
             )
 
         super().resizeEvent(event)
 
-    def _get_shape_color(self, color: QColor) -> QColor:
+    def _get_button_color(self, color: QColor, is_enabled: bool) -> QColor:
         if platform_service.is_windows:
             return QColor(Qt.GlobalColor.transparent)
         else:
-            return color
+            return color if is_enabled else self._theme.win_action_inactive
 
-    def _draw_shape(
+    def _draw_button(
         self, p: QPainter, rect: QRect, color: QColor, action: Action, enabled: bool
     ):
         p.setPen(Qt.GlobalColor.transparent)
 
-        f_col = self._get_shape_color(color)
+        f_col = self._get_button_color(color, enabled)
 
         if enabled:
             if self._hover == action:
                 f_col = color
             if self._press == action:
                 f_col = color.lighter(135)
 
         p.setBrush(f_col)
 
         if platform_service.is_windows:
-            p.drawRect(rect)
+            if action == Action.CLOSE:
+                offset = QPoint(0, 1)
+                path = QPainterPath(rect.topLeft() + offset)
+                path.lineTo(rect.bottomLeft() + offset)
+                path.lineTo(rect.bottomRight() + offset)
+
+                a = rect.topRight() + offset + QPoint(0, self._theme.win_corner_radius)
+                b = rect.topRight() + offset - QPoint(self._theme.win_corner_radius, 0)
+
+                path.lineTo(a)
+                path.cubicTo(rect.topRight(), b, b)
+
+                path.lineTo(rect.topLeft() + offset)
+                p.drawPath(path)
+            else:
+                p.drawRect(rect)
         else:
             p.drawEllipse(rect)
 
     def _get_shape_tools(self, color: QColor, action: Action) -> Tuple[QPen, QBrush]:
         if self._press == action:
             color = color if platform_service.is_macos else color.lighter(200)
         elif self._hover == action:
-            color = (
-                color
-                if platform_service.is_macos
-                else color.lighter()
-                if platform_service.is_windows
-                else color.lighter(175)
-            )
+            color = color if platform_service.is_macos else color.lighter()
         else:
-            color = (
-                Qt.GlobalColor.transparent
-                if platform_service.is_macos
-                else color
-                if platform_service.is_windows
-                else color.lighter()
-            )
+            color = Qt.GlobalColor.transparent if platform_service.is_macos else color
 
         pen = QPen(color)
         pen.setWidth(3 if platform_service.is_windows else 2)
         pen.setCapStyle(Qt.PenCapStyle.RoundCap)
 
         brush = QBrush(color)
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/frameless/window_shade.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/frameless/window_shade.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/menu_ctx.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/menu_ctx.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/multi_combo_box.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/multi_combo_box.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/object_name_mixin.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/object_name_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/settings_mixin.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_bar_ctx.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_bar_ctx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
-from typing import ContextManager, Literal
+from typing import ContextManager, List, Literal
 
 from PySide6 import QtGui
 from PySide6.QtCore import QSize, Qt
-from PySide6.QtGui import QIcon
-from PySide6.QtWidgets import QMainWindow, QToolBar
+from PySide6.QtGui import QAction, QIcon
+from PySide6.QtWidgets import QMainWindow, QToolBar, QToolButton
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.services import application_service
 
 ToolBarArea = Literal["top", "bottom", "left", "right"]
 
 _TOOL_BAR_AREA_MAP = {
@@ -19,16 +19,17 @@
 }
 
 
 class ToolBarContext(ObjectNameMixin, QToolBar):
     def __init__(self, area: ToolBarArea, parent: QMainWindow, movable=False):
         self._area = area
         self._theme = application_service.get_app_theme()
+        self._actions: List[QAction] = []
 
-        _margins = [1, 1, 1, 1]
+        _margins = [0, 0, 0, 0]
 
         if area == "left":
             self._border_side = "right"
         elif area == "right":
             self._border_side = "left"
         elif area == "top":
             self._border_side = "bottom"
@@ -37,30 +38,34 @@
             self._border_side = "top"
             _margins[3] = 5
 
         self.OBJECT_NAME = f"ToolBar_{area}"
         super(ToolBarContext, self).__init__(self.OBJECT_NAME, parent=parent)
 
         self.setContentsMargins(*_margins)
+        self.setGeometry(10, 10, self.width(), self.height())
         self.setMovable(movable)
         self.setIconSize(QSize(28, 28))
 
         parent.addToolBar(_TOOL_BAR_AREA_MAP[self._area], self)
 
         self._setup_style()
 
     @contextlib.contextmanager
     def add_action(
         self, name: str, icon: QIcon | None = None
-    ) -> ContextManager[QtGui.QAction]:
-        action = QtGui.QAction(text=name, parent=self)
+    ) -> ContextManager[QAction]:
+        action = QAction(text=name, parent=self)
         action.setObjectName(f"ToolBarAction_{name}")
         if icon:
             action.setIcon(icon)
 
+        self._actions.append(action)
+        if len(self._actions) == 1:
+            tool_button = [c for c in self.children() if isinstance(c, QToolButton)][0]
         yield action
         self.addAction(action)
 
     def _setup_style(self):
         self.setStyleSheet(
             f"""
 #{self.obj_name} {{
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_button.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_button.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/tool_stack.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/tool_stack.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/qt/widgets/window_settings_mixin.py` & `pyside-app-core-0.1.7/src/pyside_app_core/qt/widgets/window_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/services/application_service.py` & `pyside-app-core-0.1.7/src/pyside_app_core/services/application_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Type
+
 from pyside_app_core.errors.basic_errors import ApplicationError
 from pyside_app_core.qt.style import QssTheme
 
 __app_name = ""
 __app_id = ""
 __app_version = ""
 __app_theme = None
@@ -27,15 +29,15 @@
     global __app_version
     if __app_version:
         raise ApplicationError("Can't update app_version after its been set once.")
 
     __app_version = app_version
 
 
-def set_app_theme(app_theme: QssTheme) -> None:
+def set_app_theme(app_theme: QssTheme | Type[QssTheme]) -> None:
     global __app_theme
     if __app_theme:
         raise ApplicationError("Can't update app_theme after its been set once.")
 
     __app_theme = app_theme
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/serial_service.py` & `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/serial_service.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py` & `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/conversion_utils.py` & `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core/services/serial_service/utils/float_map.py` & `pyside-app-core-0.1.7/src/pyside_app_core/services/serial_service/utils/float_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 from pyside_app_core.utils import compare
 from pyside_app_core.constants import (
     DATA_STRUCT_ENDIAN,
     FLOAT_PRECISION,
     STRUCT_FLOAT_FMT,
 )
-from pyside_app_core.services.serial_service.utils.conversion_utils import (
-    int_from_bytes,
-)
+from pyside_app_core.services.serial_service.utils import conversion_utils
 
 K = TypeVar("K", bound=int)
 
 
 class FloatMap(Mapping[K, float]):
     _count_fmt = "H"  # unsigned short, 2 bytes
     _key_fmt = "H"  # unsigned short, 2 bytes
@@ -104,15 +102,15 @@
 
     @classmethod
     def unpack(cls, raw_data: bytes) -> Self:
         count_bytes = 2
         raw_pair_count = raw_data[:count_bytes]
         raw_key_val = raw_data[count_bytes:]
 
-        pair_count = int_from_bytes(raw_pair_count, signed=False)
+        pair_count = conversion_utils.int_from_bytes(raw_pair_count, signed=False)
         fmt_chars = [cls._key_fmt, STRUCT_FLOAT_FMT] * pair_count
 
         flat_pairs = struct.unpack(
             f"{DATA_STRUCT_ENDIAN}{''.join(fmt_chars)}", raw_key_val
         )
 
         data = {}
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core.egg-info/PKG-INFO` & `pyside-app-core-0.1.7/src/pyside_app_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.6
+Version: 0.1.7
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,24 +681,27 @@
 Project-URL: Homepage, https://github.com/leocov-dev/pyside-app-core
 Keywords: pyside,pyside6,frameless,app,style
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Desktop Environment
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyside-app-core
 
-Custom style, widgets, and utilities for PySide 6.5 applications.
+Custom style, widgets, and utilities for cross-platform PySide 6.5 applications with a focus on 'frameless' styling.
 
-> This project should be considered experimental and subject to breaking changes at any time.
+> This project should be considered experimental and subject to breaking changes until a 1.0.0 release.
 
 
 ### Install
 
 ```shell
 $ pip install pyside-app-core
 ```
```

### Comparing `pyside-app-core-0.1.6/src/pyside_app_core.egg-info/SOURCES.txt` & `pyside-app-core-0.1.7/src/pyside_app_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,29 @@
 src/pyside_app_core/log/__init__.py
 src/pyside_app_core/log/logger.py
 src/pyside_app_core/qt/__init__.py
 src/pyside_app_core/qt/style.py
 src/pyside_app_core/qt/util/__init__.py
 src/pyside_app_core/qt/util/pixel_val.py
 src/pyside_app_core/qt/util/s_color.py
+src/pyside_app_core/qt/util/style_sheet.py
 src/pyside_app_core/qt/widgets/__init__.py
 src/pyside_app_core/qt/widgets/about_dialog.py
+src/pyside_app_core/qt/widgets/base_app.py
 src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
 src/pyside_app_core/qt/widgets/error_dialog.py
 src/pyside_app_core/qt/widgets/menu_ctx.py
 src/pyside_app_core/qt/widgets/multi_combo_box.py
 src/pyside_app_core/qt/widgets/object_name_mixin.py
 src/pyside_app_core/qt/widgets/settings_mixin.py
 src/pyside_app_core/qt/widgets/tool_bar_ctx.py
 src/pyside_app_core/qt/widgets/tool_button.py
 src/pyside_app_core/qt/widgets/tool_stack.py
 src/pyside_app_core/qt/widgets/window_settings_mixin.py
 src/pyside_app_core/qt/widgets/frameless/__init__.py
-src/pyside_app_core/qt/widgets/frameless/application.py
 src/pyside_app_core/qt/widgets/frameless/base_dialog.py
 src/pyside_app_core/qt/widgets/frameless/base_window.py
 src/pyside_app_core/qt/widgets/frameless/main_window.py
 src/pyside_app_core/qt/widgets/frameless/window_actions.py
 src/pyside_app_core/qt/widgets/frameless/window_shade.py
 src/pyside_app_core/services/__init__.py
 src/pyside_app_core/services/application_service.py
```

