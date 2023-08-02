# Comparing `tmp/djangocms_leaflet-0.0.3b1.tar.gz` & `tmp/djangocms_leaflet-0.0.3b2.tar.gz`

## Comparing `djangocms_leaflet-0.0.3b1.tar` & `djangocms_leaflet-0.0.3b2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    58673 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/package-lock.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/package.json
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/webpack.config.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/assets/src/leaflet.js
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/apps.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/cms_plugins.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/models.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0001_initial.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0003_map_location_search_term_marker_location_search_term_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-black.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-blue.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-gold.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-green.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-grey.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-orange.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-red.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-violet.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-yellow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-black.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-blue.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-gold.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-green.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-grey.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-orange.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-red.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-violet.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-yellow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-shadow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-shadow.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   174912 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/tests/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/LICENSE.txt
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/README.md
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/pyproject.toml
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/PKG-INFO
+-rw-r--r--   0        0        0    58673 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/package-lock.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/package.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/webpack.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/assets/src/leaflet.js
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/apps.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/cms_plugins.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/models.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/migrations/0001_initial.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/migrations/0003_rename_name_map__name_remove_marker_name_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/migrations/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-shadow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-shadow.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   174912 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/LICENSE.txt
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/README.md
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/pyproject.toml
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b2/PKG-INFO
```

### Comparing `djangocms_leaflet-0.0.3b1/package-lock.json` & `djangocms_leaflet-0.0.3b2/package-lock.json`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/cms_plugins.py` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/models.py` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,50 +2,41 @@
 from cms.models import CMSPlugin
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext as _
 from requests import Response
 
 
-class Map(CMSPlugin):
-    """Map with name and location, optionally with a marker set in the centre"""
-    name = models.CharField(verbose_name=_('name'), blank=True, max_length=100)
+class Geocode(CMSPlugin):
+    _name = models.CharField(verbose_name=_('name'), blank=True, max_length=100)
     location_search_term = models.CharField(
         verbose_name=_('location search term'),
         blank=True,
         max_length=100,
         help_text=_(
             'Instead of coordinates you can enter the address or a search term, and Nominatim will try to look up the '
             'location. The first hit of the list will be used.'
         )
     )
     latitude = models.FloatField(
-        blank=True, verbose_name=_('latitude'), help_text=_('in °')
+        blank=True, verbose_name=_('latitude in °')
     )
     longitude = models.FloatField(
-        blank=True, verbose_name=_('longitude'), help_text=_('in °')
-    )
-
-    zoom_level = models.PositiveSmallIntegerField(
-        verbose_name=_('zoom level'), help_text=_('0…18'), default=10
-    )
-    height = models.PositiveSmallIntegerField(
-        verbose_name=_('height of map'), help_text=_('in px'), default=400
-    )
-    set_marker = models.BooleanField(
-        verbose_name=_('set marker'),
-        help_text=_('Set marker with name at the centre'),
-        default=400
+        blank=True,
+        verbose_name=_('longitude in °'),
+        help_text=_(
+            'If you enter both latitude and longitude, these data won’t be overridden by a geocoding lookup.'
+        )
     )
+    @property
+    def name(self):
+        return self._name if self._name else self.location_search_term
 
-    def __str__(self) -> str:
-        return (
-            self.name if self.name else
-            f'{self.latitude}° {self.longitude}°, zoom {self.zoom_level}'
-        )
+    class Meta:
+        abstract = True
 
     def clean(self):
         if (
             self.latitude is None or self.longitude is None
         ) and self.location_search_term == '':
             raise ValidationError(
                 _(
@@ -62,60 +53,38 @@
             geo_json = response.json()
             try:
                 self.latitude = geo_json[0]['lat']
                 self.longitude = geo_json[0]['lon']
             except IndexError:
                 raise ValidationError(_('Location not found.'))
 
-    def save(self, *args, **kwargs) -> None:
-        super().save(*args, **kwargs)
 
+class Map(Geocode):
+    """Map with name and location, optionally with a marker set in the centre"""
 
-class Marker(CMSPlugin):
-    """Marker that can be added to a map"""
-    name = models.CharField(verbose_name=_('name'), max_length=100)
-    location_search_term = models.CharField(
-        verbose_name=_('location search term'),
-        blank=True,
-        max_length=100,
-        help_text=_(
-            'Instead of coordinates you can enter the address or a search term, and Nominatim will try to look up the '
-            'location. The first hit of the list will be used.'
-        )
+    zoom_level = models.PositiveSmallIntegerField(
+        verbose_name=_('zoom level'), help_text=_('0…18'), default=10
     )
-    latitude = models.FloatField(blank=True, verbose_name=_('latitude'))
-    longitude = models.FloatField(
-        blank=True,
-        verbose_name=_('longitude'),
-        help_text=_(
-            'If you enter both latitude and longitude, these data won’t be overridden by a geocoding lookup.'
-        )
+    height = models.PositiveSmallIntegerField(
+        verbose_name=_('height of map'), help_text=_('in px'), default=400
+    )
+    set_marker = models.BooleanField(
+        verbose_name=_('set marker'),
+        help_text=_('Set marker with name at the centre'),
+        default=400
     )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
             self.name if self.name else
+            self.location_search_term if self.location_search_term else
             f'{self.latitude}° {self.longitude}°, zoom {self.zoom_level}'
         )
 
-    def clean(self):
-        if (
-            self.latitude is None or self.longitude is None
-        ) and self.location_search_term == '':
-            raise ValidationError(
-                _(
-                    'If you don’t specify latitude and longitude, you need to enter a search term for the location.'
-                )
-            )
-        if self.location_search_term and (
-            self.latitude is None or self.longitude is None
-        ):
-            payload = {'q': self.location_search_term, 'format': 'jsonv2'}
-            response: Response = requests.get(
-                'https://nominatim.openstreetmap.org/search', params=payload
-            )
-            geo_json = response.json()
-            try:
-                self.latitude = geo_json[0]['lat']
-                self.longitude = geo_json[0]['lon']
-            except IndexError:
-                raise ValidationError(_('Location not found.'))
+
+class Marker(Geocode):
+    """Marker that can be added to a map"""
+    def __str__(self):
+        return (
+            self.name if self.name else self.location_search_term if
+            self.location_search_term else f'{self.latitude}° {self.longitude}°'
+        )
```

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0001_initial.py` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/templates/djangocms_leaflet/map.html` & `djangocms_leaflet-0.0.3b2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         iconSize: [24, 36],
         iconAnchor: [12, 36]
     });
     L.Marker.prototype.options.icon = DefaultIcon;
 
     {% if instance.set_marker %}
         L.marker([{{ instance.latitude }}, {{ instance.longitude }}]).addTo(map)
-            .bindPopup('{{ instance.name }}')
+            .bindPopup('{{ instance }}')
             .openPopup();
     {% endif %}
 })
 </script>
 {% endaddtoblock %}
 
 {% for plugin in instance.child_plugin_instances %}
```

### Comparing `djangocms_leaflet-0.0.3b1/LICENSE.txt` & `djangocms_leaflet-0.0.3b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/README.md` & `djangocms_leaflet-0.0.3b2/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/pyproject.toml` & `djangocms_leaflet-0.0.3b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.3b1/PKG-INFO` & `djangocms_leaflet-0.0.3b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-leaflet
-Version: 0.0.3b1
+Version: 0.0.3b2
 Summary: django CMS plug-ins for the JavaScript map library Leaflet
 Project-URL: Documentation, https://github.com/MacLake/djangocms-leaflet#readme
 Project-URL: Issues, https://github.com/MacLake/djangocms-leaflet/issues
 Project-URL: Source, https://github.com/MacLake/djangocms-leaflet
 Author-email: Jens-Erik Weber <Jens-Erik.Weber@passiv.de>
 License-Expression: MIT
 License-File: LICENSE.txt
```

