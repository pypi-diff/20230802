# Comparing `tmp/geomanager-0.0.4.tar.gz` & `tmp/geomanager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomanager-0.0.4.tar", last modified: Mon Jul 17 09:20:17 2023, max compression
+gzip compressed data, was "geomanager-0.0.5.tar", last modified: Wed Aug  2 11:09:13 2023, max compression
```

## Comparing `geomanager-0.0.4.tar` & `geomanager-0.0.5.tar`

### file list

```diff
@@ -1,135 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.344429 geomanager-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 09:19:56.000000 geomanager-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-17 09:20:17.344429 geomanager-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-17 09:19:56.000000 geomanager-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.328428 geomanager-0.0.4/geomanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    50516 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0004_alter_dataset_can_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0005_delete_countryboundary_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0006_stationsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0008_stationsettings_name_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0009_stationsettings_popup_props.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/0010_remove_stationsettings_popup_props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/models/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/models/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/samples/basemaps/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/samples/basemaps/basemaps.json
--rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/samples/basemaps/style.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/serializers/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/django_large_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/django_large_image/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/django_large_image/js/geojs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/static/django_large_image/js/geojs/1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/static/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/static/geomanager/css/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/css/preview-map.css
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/css/upload.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.332428 geomanager-0.0.4/geomanager/static/geomanager/css/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/css/vendor/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.336428 geomanager-0.0.4/geomanager/static/geomanager/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/images/geomapviewer-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.336428 geomanager-0.0.4/geomanager/static/geomanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/add-multiple.js
--rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/colorbrewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/mbt_source_extra.js
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/raster-preview.js
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/raster_style_extra.js
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vector-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.336428 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/d3-format.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   745424 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (123)   542509 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/vendor/ol.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/static/geomanager/js/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/widgets/icon_chooser.js
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/widgets/raster_style_widget.js
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/static/geomanager/js/wms-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.324428 geomanager-0.0.4/geomanager/templates/admin/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/admin/geomanager/layerrasterfile/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/django_nextjs/
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/django_nextjs/mapviewer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/geomanager/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/raster_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/raster_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/raster_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/stations_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/stations_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/vector_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/vector_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/vector_upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/geomanager/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/widgets/raster_style_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/geomanager/wms_preview.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templates/modeladmin/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templates/modeladmin/index_without_custom_create.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/templatetags/geomanager_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.340428 geomanager-0.0.4/geomanager/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/raster_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/utils/vector_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.344429 geomanager-0.0.4/geomanager/views/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/nextjs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/views/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.344429 geomanager-0.0.4/geomanager/viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/viewsets/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-17 09:19:56.000000 geomanager-0.0.4/geomanager/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:17.328428 geomanager-0.0.4/geomanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 09:20:17.000000 geomanager-0.0.4/geomanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 09:19:56.000000 geomanager-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-17 09:20:17.344429 geomanager-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.734232 geomanager-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-02 11:08:55.000000 geomanager-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-02 11:09:13.734232 geomanager-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-08-02 11:08:55.000000 geomanager-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.718231 geomanager-0.0.5/geomanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.722231 geomanager-0.0.5/geomanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    50516 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0004_alter_dataset_can_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0005_delete_countryboundary_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0006_stationsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0008_stationsettings_name_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0009_stationsettings_popup_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0010_remove_stationsettings_popup_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0011_vectorlayericon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0012_geomanagersettings_crop_raster_to_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0013_geomanagersettings_logo_external_link_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/0014_geomanagersettings_privacy_policy_page_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.722231 geomanager-0.0.5/geomanager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21239 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/models/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.722231 geomanager-0.0.5/geomanager/samples/basemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/samples/basemaps/basemaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/samples/basemaps/style.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.726231 geomanager-0.0.5/geomanager/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/serializers/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/serializers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/serializers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/serializers/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/serializers/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/serializers/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/static/django_large_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/static/django_large_image/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/static/django_large_image/js/geojs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.726231 geomanager-0.0.5/geomanager/static/django_large_image/js/geojs/1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/static/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.726231 geomanager-0.0.5/geomanager/static/geomanager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    35100 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/css/bulma-navbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/css/preview-map.css
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/css/stations_preview.css
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/css/upload.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.726231 geomanager-0.0.5/geomanager/static/geomanager/css/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/css/vendor/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.726231 geomanager-0.0.5/geomanager/static/geomanager/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/images/geomapviewer-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.726231 geomanager-0.0.5/geomanager/static/geomanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/add-multiple.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/colorbrewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/mbt_source_extra.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/raster-preview.js
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/raster_style_extra.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/vector-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/static/geomanager/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/vendor/d3-format.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   745424 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/vendor/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)   542509 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/vendor/ol.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/static/geomanager/js/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/widgets/icon_chooser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/widgets/raster_style_widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/static/geomanager/js/wms-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.714230 geomanager-0.0.5/geomanager/templates/admin/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/templates/admin/geomanager/layerrasterfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/templates/django_nextjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/django_nextjs/mapviewer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/templates/geomanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/raster_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/raster_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/raster_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/stations_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/stations_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/vector_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/vector_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/vector_upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/templates/geomanager/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/widgets/raster_style_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/geomanager/wms_preview.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/templates/modeladmin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templates/modeladmin/index_without_custom_create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/templatetags/geomanager_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.730232 geomanager-0.0.5/geomanager/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/utils/raster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/utils/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/utils/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/utils/vector_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.734232 geomanager-0.0.5/geomanager/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/nextjs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/views/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.734232 geomanager-0.0.5/geomanager/viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/viewsets/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/viewsets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/viewsets/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/viewsets/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 11:08:55.000000 geomanager-0.0.5/geomanager/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:09:13.718231 geomanager-0.0.5/geomanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-02 11:09:13.000000 geomanager-0.0.5/geomanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-02 11:09:13.000000 geomanager-0.0.5/geomanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:09:13.000000 geomanager-0.0.5/geomanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-02 11:09:13.000000 geomanager-0.0.5/geomanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 11:09:13.000000 geomanager-0.0.5/geomanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-02 11:08:55.000000 geomanager-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 11:09:13.734232 geomanager-0.0.5/setup.cfg
```

### Comparing `geomanager-0.0.4/PKG-INFO` & `geomanager-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wagtail based Geospatial Data Manager
 Home-page: https://github.com/wmo-raf/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `geomanager-0.0.4/README.md` & `geomanager-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/apps.py` & `geomanager-0.0.5/geomanager/apps.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/blocks.py` & `geomanager-0.0.5/geomanager/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from wagtail import blocks
 from wagtail_color_panel.blocks import NativeColorBlock
 from wagtailiconchooser.blocks import IconChooserBlock
 
 
 class NavigationItemsBlock(blocks.StructBlock):
     label = blocks.CharBlock(label=_("Label"))
-    page = blocks.PageChooserBlock(label=_("Page"))
+    page = blocks.PageChooserBlock(required=False, label=_("Page"), help_text=_("Internal page to navigate"))
+    external_link = blocks.URLBlock(required=False, label=_("External Link"),
+                                    help_text=_("External link to navigate to. Used if internal page not provided"))
 
 
 class WmsRequestParamSelectableBlock(blocks.StructBlock):
     SELECTOR_TYPE_CHOICES = (
         ("radio", "Radio"),
         ("dropdown", "Dropdown"),
     )
```

### Comparing `geomanager-0.0.4/geomanager/constants.py` & `geomanager-0.0.5/geomanager/constants.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/errors.py` & `geomanager-0.0.5/geomanager/errors.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/fields.py` & `geomanager-0.0.5/geomanager/fields.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/forms.py` & `geomanager-0.0.5/geomanager/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,7 +153,11 @@
 
         if column_choices:
             choices = [("", "--------")]
             choices.extend(column_choices)
             self.fields['name_column'].choices = choices
         else:
             self.fields['name_column'].widget = forms.HiddenInput()
+
+
+class VectorTableForm(forms.Form):
+    columns = forms.JSONField(required=False, widget=forms.HiddenInput)
```

### Comparing `geomanager-0.0.4/geomanager/helpers.py` & `geomanager-0.0.5/geomanager/helpers.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/migrations/0001_initial.py` & `geomanager-0.0.5/geomanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/migrations/0002_geomanagersettings_logo_and_more.py` & `geomanager-0.0.5/geomanager/migrations/0002_geomanagersettings_logo_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py` & `geomanager-0.0.5/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/migrations/0004_alter_dataset_can_clip.py` & `geomanager-0.0.5/geomanager/migrations/0004_alter_dataset_can_clip.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/migrations/0005_delete_countryboundary_and_more.py` & `geomanager-0.0.5/geomanager/migrations/0005_delete_countryboundary_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/migrations/0006_stationsettings.py` & `geomanager-0.0.5/geomanager/migrations/0006_stationsettings.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py` & `geomanager-0.0.5/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/models/__init__.py` & `geomanager-0.0.5/geomanager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/models/aoi.py` & `geomanager-0.0.5/geomanager/models/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/models/core.py` & `geomanager-0.0.5/geomanager/models/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     InlinePanel
 )
 from wagtail.contrib.modeladmin.helpers import AdminURLHelper
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 from wagtail.fields import StreamField, RichTextField
 from wagtail.images.blocks import ImageChooserBlock
-from wagtail.models import Orderable
+from wagtail.models import Orderable, Page
 from wagtail_adminsortable.models import AdminSortable
 from wagtailiconchooser.widgets import IconChooserWidget
 
 from geomanager.helpers import (
     get_layer_action_url,
     get_preview_url,
     get_upload_url
@@ -352,14 +352,16 @@
     )
 
     max_upload_size_mb = models.IntegerField(default=DEFAULT_RASTER_MAX_UPLOAD_SIZE_MB,
                                              verbose_name=_("Maximum upload size in MegaBytes"),
                                              help_text=_(
                                                  "Maximum raster file size that can be uploaded in MegaBytes. "
                                                  "Default is 10Mbs."))
+    crop_raster_to_country = models.BooleanField(default=True, verbose_name=_("Crop raster to country"),
+                                                 help_text=_("Crop the uploaded raster file to the country boundaries"))
 
     cap_base_url = models.URLField(max_length=256, null=True, blank=True, verbose_name=_("cap base url"))
     cap_sub_category = models.ForeignKey(SubCategory, null=True, blank=True, verbose_name=_("cap layer sub category"),
                                          on_delete=models.SET_NULL)
     cap_auto_refresh_interval = models.IntegerField(blank=True, null=True,
                                                     verbose_name=_("Auto Refresh interval in minutes"),
                                                     help_text=_(
@@ -384,14 +386,45 @@
         'wagtailimages.Image',
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name='+',
         verbose_name=_("Logo")
     )
+    logo_page = models.ForeignKey(
+        Page,
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+        related_name='+',
+        verbose_name=_("Logo page"),
+        help_text=_("Internal page to navigate to on clicking the logo")
+    )
+    logo_external_link = models.URLField(max_length=255, null=True, blank=True,
+                                         verbose_name=_("Logo external link"),
+                                         help_text=_("Used if internal logo page not provided"))
+    terms_of_service_page = models.ForeignKey(
+        Page,
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+        related_name='+',
+        verbose_name=_("Terms of Service Page"),
+        help_text=_("MapViewer Terms of Service page")
+    )
+    privacy_policy_page = models.ForeignKey(
+        Page,
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+        related_name='+',
+        verbose_name=_("Privacy Policy Page"),
+        help_text=_("MapViewer Privacy Policy Page")
+    )
+
     navigation = StreamField([
         ('menu_items', blocks.ListBlock(NavigationItemsBlock(max_num=8))),
     ], block_counts={
         'menu_items': {'max_num': 1},
     }, use_json_field=True, null=True, blank=True)
 
     base_maps = StreamField([
@@ -405,14 +438,15 @@
             ('default', blocks.BooleanBlock(required=False, label=_("default"), help_text=_("Is default style ?"))),
         ]))
     ], use_json_field=True, null=True, blank=True)
 
     edit_handler = TabbedInterface([
         ObjectList([
             FieldPanel("max_upload_size_mb"),
+            FieldPanel("crop_raster_to_country"),
         ], heading=_("Upload Settings")),
         ObjectList([
             FieldPanel("tile_gl_fonts_url"),
             FieldPanel("tile_gl_source"),
             FieldPanel("base_maps"),
         ], heading=_("Basemap TileServer Settings")),
         ObjectList([
@@ -420,16 +454,20 @@
             FieldPanel("cap_sub_category"),
             FieldPanel("cap_auto_refresh_interval"),
             FieldPanel("cap_shown_by_default"),
             FieldPanel("cap_metadata"),
         ], heading=_("CAP Layer Settings")),
         ObjectList([
             FieldPanel("logo"),
+            FieldPanel("logo_page"),
+            FieldPanel("logo_external_link"),
+            FieldPanel("terms_of_service_page"),
+            FieldPanel("privacy_policy_page"),
             FieldPanel("navigation"),
-        ], heading=_("Branding Settings")),
+        ], heading=_("Navigation Settings")),
     ])
 
     @property
     def cap_auto_refresh_interval_milliseconds(self):
         if self.cap_auto_refresh_interval:
             return self.cap_auto_refresh_interval * 60000
         return None
```

### Comparing `geomanager-0.0.4/geomanager/models/profile.py` & `geomanager-0.0.5/geomanager/models/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/models/raster.py` & `geomanager-0.0.5/geomanager/models/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/models/stations.py` & `geomanager-0.0.5/geomanager/models/stations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.gis.db import models
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.html import format_html
-from django_tables2 import tables, LazyPaginator, Column, columns, TemplateColumn
+from django_tables2 import tables, LazyPaginator, TemplateColumn
 from wagtail.contrib.routable_page.models import RoutablePageMixin, path
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.models import Page
 
 from geomanager.fields import ListField
 from geomanager.utils.vector_utils import get_model_field
```

### Comparing `geomanager-0.0.4/geomanager/models/tile_gl.py` & `geomanager-0.0.5/geomanager/models/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/models/vector.py` & `geomanager-0.0.5/geomanager/models/vector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import uuid
 
 from django.contrib.admin.utils import quote
 from django.contrib.gis.db import models
+from django.core.files.base import ContentFile
 from django.db.models.signals import pre_delete
 from django.dispatch import receiver
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 from django_extensions.db.models import TimeStampedModel
+from modelcluster.fields import ParentalKey
+from modelcluster.models import ClusterableModel
 from wagtail.admin.panels import FieldPanel
 from wagtail.fields import StreamField
 from wagtail.images.blocks import ImageChooserBlock
 
 from geomanager.blocks import InlineLegendBlock, FillVectorLayerBlock, LineVectorLayerBlock, CircleVectorLayerBlock, \
     IconVectorLayerBlock, TextVectorLayerBlock, InlineIconLegendBlock
 from geomanager.constants import MAPBOX_GL_STYLE_SPEC
 from geomanager.fields import ListField
 from geomanager.helpers import get_vector_layer_files_url
 from geomanager.models import Dataset
 from geomanager.models.core import BaseLayer
 from geomanager.panels import ReadOnlyFieldPanel
+from geomanager.utils.svg import rasterize_svg_to_png
 from geomanager.utils.vector_utils import drop_vector_table
 
 
 class Geostore(TimeStampedModel):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     iso = models.CharField(max_length=100, blank=True, null=True)
     id1 = models.CharField(max_length=100, blank=True, null=True)
@@ -62,15 +66,15 @@
 
         if self.id3:
             info.update({"id3": self.id3, "name": self.id3})
 
         return info
 
 
-class VectorLayer(TimeStampedModel, BaseLayer):
+class VectorLayer(TimeStampedModel, ClusterableModel, BaseLayer):
     dataset = models.ForeignKey(Dataset, on_delete=models.CASCADE, related_name="vector_layers", verbose_name="dataset")
     render_layers = StreamField([
         ("fill", FillVectorLayerBlock(label=_("Polygon Layer"))),
         ("line", LineVectorLayerBlock(label=_("Line Layer"))),
         ("circle", CircleVectorLayerBlock(label=_("Point Layer"))),
         ("icon", IconVectorLayerBlock(label=_("Icon Layer"))),
         ("text", TextVectorLayerBlock(label=_("Text Label Layer"))),
@@ -85,14 +89,18 @@
         return self.title
 
     def get_uploads_list_url(self):
         url = get_vector_layer_files_url(self.pk)
         return url
 
     @property
+    def has_data_table(self):
+        return self.vector_tables.all().exists()
+
+    @property
     def upload_url(self):
         upload_url = reverse(
             f"geomanager_dataset_layer_upload_vector",
             args=[quote(self.dataset.pk), quote(self.pk)],
         )
         return upload_url
 
@@ -244,14 +252,60 @@
                 config["items"].append({
                     "name": item.get("value"),
                     "color": item.get("color")
                 })
 
         return config
 
+    @property
+    def interaction_config(self):
+        config = {}
+
+        # TODO: What happens if we have multiple tables ?
+        vector_table = self.vector_tables.first()
+
+        if vector_table and vector_table.properties:
+            for column in vector_table.properties:
+                if column.get("popup"):
+                    if not config.get("output"):
+                        config["output"] = []
+                    name = column.get("name")
+                    label = column.get("label")
+                    config["output"].append({"column": name, "property": label or name}, )
+
+        return config
+
+    def save(self, *args, **kwargs):
+        # remove existing icons for this layer.
+        # TODO: Find efficient way to update exising icons, while deleting absolute ones
+        VectorLayerIcon.objects.filter(layer=self).delete()
+
+        for render_layer in self.render_layers:
+            if render_layer.block_type == "icon":
+                icon_image = render_layer.value.get("layout").get("icon_image")
+                icon_color = render_layer.value.get("paint").get("icon_color")
+                png_bytes = rasterize_svg_to_png(icon_image, fill_color=icon_color)
+
+                if png_bytes:
+                    layer_icon = VectorLayerIcon(name=icon_image, color=icon_color)
+                    layer_icon.file = ContentFile(png_bytes.getvalue(), f"{icon_image}.{icon_color}.png")
+                    self.icons.add(layer_icon)
+
+        super().save(*args, **kwargs)
+
+
+class VectorLayerIcon(models.Model):
+    layer = ParentalKey(VectorLayer, on_delete=models.CASCADE, related_name="icons")
+    name = models.CharField(max_length=255)
+    color = models.CharField(max_length=100, null=True)
+    file = models.FileField(upload_to="vector_icons/")
+
+    def __str__(self):
+        return f"{self.layer.title}-{self.name}-{self.color}"
+
 
 class VectorUpload(TimeStampedModel):
     dataset = models.ForeignKey(Dataset, blank=True, null=True, on_delete=models.SET_NULL)
     file = models.FileField(upload_to="vector_uploads")
     vector_metadata = models.JSONField(blank=True, null=True)
 
     panels = [
```

### Comparing `geomanager-0.0.4/geomanager/samples/basemaps/basemaps.json` & `geomanager-0.0.5/geomanager/samples/basemaps/basemaps.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/samples/basemaps/style.json` & `geomanager-0.0.5/geomanager/samples/basemaps/style.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/serializers/aoi.py` & `geomanager-0.0.5/geomanager/serializers/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/serializers/auth.py` & `geomanager-0.0.5/geomanager/serializers/auth.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/serializers/core.py` & `geomanager-0.0.5/geomanager/serializers/core.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/serializers/profile.py` & `geomanager-0.0.5/geomanager/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/serializers/raster.py` & `geomanager-0.0.5/geomanager/serializers/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/serializers/vector.py` & `geomanager-0.0.5/geomanager/serializers/vector.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class AdminBoundarySerializer(serializers.ModelSerializer):
     bbox = serializers.ListField()
 
     class Meta:
         model = AdminBoundary
-        fields = ("level", "name_0", "name_1", "name_2", "gid_0", "gid_1", "gid_2", "size", "bbox")
+        fields = ("level", "name_0", "name_1", "name_2", "gid_0", "gid_1", "gid_2", "bbox")
 
 
 class BoundsFieldSerializer(serializers.Field):
     def to_representation(self, value):
         # Convert the value of the custom field to a string for serialization
         return [float(value) for value in list(value)]
 
@@ -39,19 +39,21 @@
     paramsSelectorConfig = serializers.SerializerMethodField()
     legendConfig = serializers.SerializerMethodField()
     multiTemporal = serializers.SerializerMethodField()
     currentTimeMethod = serializers.SerializerMethodField()
     autoUpdateInterval = serializers.SerializerMethodField()
     isMultiLayer = serializers.SerializerMethodField()
     nestedLegend = serializers.SerializerMethodField()
+    interactionConfig = serializers.SerializerMethodField()
 
     class Meta:
         model = VectorLayer
         fields = ["id", "dataset", "name", "layerType", "multiTemporal", "isMultiLayer", "legendConfig", "nestedLegend",
-                  "layerConfig", "params", "paramsSelectorConfig", "currentTimeMethod", "autoUpdateInterval"]
+                  "layerConfig", "params", "paramsSelectorConfig", "currentTimeMethod", "autoUpdateInterval",
+                  "interactionConfig"]
 
     def get_isMultiLayer(self, obj):
         return obj.dataset.multi_layer
 
     def get_nestedLegend(self, obj):
         return obj.dataset.multi_layer
 
@@ -90,14 +92,17 @@
 
     def get_getCapabilitiesUrl(self, obj):
         return obj.get_capabilities_url
 
     def get_layerName(self, obj):
         return obj.layer_name
 
+    def get_interactionConfig(self, obj):
+        return obj.interaction_config
+
 
 class GeostoreSerializer(serializers.ModelSerializer):
     attributes = serializers.SerializerMethodField()
 
     class Meta:
         model = Geostore
         fields = ["id", "attributes"]
```

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/css/vendor/maplibre-gl.css` & `geomanager-0.0.5/geomanager/static/geomanager/css/vendor/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/images/geomapviewer-logo.png` & `geomanager-0.0.5/geomanager/static/geomanager/images/geomapviewer-logo.png`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/add-multiple.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/colorbrewer.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/colorbrewer.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/mbt_source_extra.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/mbt_source_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/raster-preview.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/raster-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/raster_style_extra.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/raster_style_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/vector-preview.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/vector-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/vendor/d3-format.min.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/vendor/d3-format.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/vendor/maplibre-gl.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/vendor/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/vendor/ol.min.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/vendor/ol.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/widgets/icon_chooser.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/widgets/icon_chooser.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/widgets/raster_style_widget.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/widgets/raster_style_widget.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/static/geomanager/js/wms-preview.js` & `geomanager-0.0.5/geomanager/static/geomanager/js/wms-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/raster_edit_form.html` & `geomanager-0.0.5/geomanager/templates/geomanager/raster_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/raster_preview.html` & `geomanager-0.0.5/geomanager/templates/geomanager/raster_preview.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/raster_upload.html` & `geomanager-0.0.5/geomanager/templates/geomanager/raster_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/stations_preview.html` & `geomanager-0.0.5/geomanager/templates/geomanager/stations_preview.html`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 {% load l10n %}
 {% load wagtailadmin_tags wagtailimages_tags static %}
 {% block titletag %}{% blocktrans with title=page.get_admin_display_title %}Stations Data{{ title }}
 {% endblocktrans %}{% endblock %}
 {% block extra_css %}
     {{ block.super }}
     <link href="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.css" rel="stylesheet"/>
+    <link href="{% static "geomanager/css/stations_preview.css" %}" rel="stylesheet"/>
 {% endblock %}
 
 {% block content %}
     {% trans "Stations Data" as header_str %}
 
     {% include "wagtailadmin/shared/header.html" with title=header_str icon="map" action_url=load_stations_url action_text="Load Stations" %}
 
     <div class="nice-padding">
-        <div style="margin-top: 40px;">
-            <div id="preview-map" style="height: 600px;width: 100%"></div>
-        </div>
-        <div style="margin-top: 20px;">
-            {% if station_columns %}
+        {% if station_columns %}
+            <div style="margin-top: 40px;">
+                <div id="preview-map" style="height: 600px;width: 100%"></div>
+            </div>
+            <div style="margin-top: 20px;">
                 <h2 class="title">Data Fields</h2>
                 <table class="listing">
                     <thead>
                     <tr>
                         <th style="font-weight: 700">Field</th>
                         <th style="font-weight: 700">Label</th>
                         <th style="font-weight: 700">Show in Table</th>
@@ -76,192 +77,205 @@
                             {% endif %}
                         {% endfor %}
                         <li>
                             <button type="submit" class="button"> {% trans 'Save' %}</button>
                         </li>
                     </ul>
                 </form>
-            {% endif %}
-        </div>
-    </div>
+            </div>
+            </div>
+        {% else %}
+
+            <div class="help-block help-info">
+                <svg class="icon icon-help icon" aria-hidden="true">
+                    <use href="#icon-help"></use>
+                </svg>
+                <p>
+                    No station data loaded. Please <a href="{{ load_stations_url }}">load station data</a> to preview
+                </p>
+
+            </div>
+        {% endif %}
 {% endblock %}
 
 {% block extra_js %}
     {{ block.super }}
-    <script src="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.js"></script>
-    <script>
-
-        const mapConfigObj = {{ mapConfig | safe }};
-        const {combinedBbox, stationsVectorTilesUrl} = mapConfigObj
-
-        const bounds = [[combinedBbox[0], combinedBbox[1]], [combinedBbox[2], combinedBbox[3]]]
-
-        const defaultStyle = {
-            'version': 8,
-            'sources': {
-                'carto-dark': {
-                    'type': 'raster',
-                    'tiles': [
-                        "https://a.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png",
-                        "https://b.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png",
-                        "https://c.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png",
-                        "https://d.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png"
-                    ]
-                },
-                'carto-light': {
-                    'type': 'raster',
-                    'tiles': [
-                        "https://a.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png",
-                        "https://b.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png",
-                        "https://c.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png",
-                        "https://d.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png"
-                    ]
+    {% if station_columns %}
+        <script src="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.js"></script>
+        <script>
+
+            const mapConfigObj = {{ mapConfig | safe }};
+            const {stationBounds, stationsVectorTilesUrl} = mapConfigObj
+
+            const bounds = [[stationBounds[0], stationBounds[1]], [stationBounds[2], stationBounds[3]]]
+
+            const defaultStyle = {
+                'version': 8,
+                'sources': {
+                    'carto-dark': {
+                        'type': 'raster',
+                        'tiles': [
+                            "https://a.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png",
+                            "https://b.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png",
+                            "https://c.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png",
+                            "https://d.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}@2x.png"
+                        ]
+                    },
+                    'carto-light': {
+                        'type': 'raster',
+                        'tiles': [
+                            "https://a.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png",
+                            "https://b.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png",
+                            "https://c.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png",
+                            "https://d.basemaps.cartocdn.com/light_all/{z}/{x}/{y}@2x.png"
+                        ]
+                    },
+                    'wikimedia': {
+                        'type': 'raster',
+                        'tiles': [
+                            "https://maps.wikimedia.org/osm-intl/{z}/{x}/{y}.png"
+                        ]
+                    }
                 },
-                'wikimedia': {
+                'layers': [{
+                    'id': 'carto-light-layer',
+                    'source': 'carto-light',
                     'type': 'raster',
-                    'tiles': [
-                        "https://maps.wikimedia.org/osm-intl/{z}/{x}/{y}.png"
-                    ]
-                }
-            },
-            'layers': [{
-                'id': 'carto-light-layer',
-                'source': 'carto-light',
-                'type': 'raster',
-                'minzoom': 0,
-                'maxzoom': 22
-            }]
-        }
-
-
-        $(document).ready(async function () {
-            const $columnsInput = $("#id_columns")
-
-            const map = new maplibregl.Map({
-                container: "preview-map",
-                style: defaultStyle,
-                doubleClickZoom: false,
-            });
-
-            await new Promise((resolve) => map.on("load", resolve));
-
-            if (bounds) {
-                map.fitBounds(bounds, {padding: 20})
+                    'minzoom': 0,
+                    'maxzoom': 22
+                }]
             }
 
 
-            // add source
-            map.addSource("stations-source", {
-                    type: "vector",
-                    tiles: [stationsVectorTilesUrl],
-                }
-            )
-
-            // add layer
-            map.addLayer({
-                'id': 'stations-circle',
-                'type': 'circle',
-                'source': 'stations-source',
-                "source-layer": "default",
-                'paint': {
-                    'circle-color': "red",
-                    'circle-radius': 10,
-                }
-            });
+            $(document).ready(async function () {
+                const $columnsInput = $("#id_columns")
 
+                const map = new maplibregl.Map({
+                    container: "preview-map",
+                    style: defaultStyle,
+                    doubleClickZoom: false,
+                });
 
-            const $stationLabelInput = $(".station_input")
+                await new Promise((resolve) => map.on("load", resolve));
 
-            $stationLabelInput.on("change", function () {
-                const $this = $(this)
-                const inputType = $this.attr('type')
+                if (bounds) {
+                    map.fitBounds(bounds, {padding: 20})
+                }
 
-                const columnName = $this.data("column")
-                const updateType = $this.data("updatetype")
 
-                if (columnName && updateType) {
-                    let inputValue = $this.val()
+                // add source
+                map.addSource("stations-source", {
+                        type: "vector",
+                        tiles: [stationsVectorTilesUrl],
+                    }
+                )
 
-                    if (inputType === "checkbox") {
-                        inputValue = $this.is(':checked')
+                // add layer
+                map.addLayer({
+                    'id': 'stations-circle',
+                    'type': 'circle',
+                    'source': 'stations-source',
+                    "source-layer": "default",
+                    'paint': {
+                        'circle-color': "red",
+                        'circle-radius': 10,
                     }
-                    updateColumnsData(columnName, updateType, inputValue)
-                }
-            })
+                });
 
-            const getColumnsData = () => {
-                let columnsData = $columnsInput.val()
 
-                if (columnsData) {
-                    columnsData = JSON.parse(columnsData)
+                const $stationLabelInput = $(".station_input")
 
-                    return columnsData
-                }
+                $stationLabelInput.on("change", function () {
+                    const $this = $(this)
+                    const inputType = $this.attr('type')
 
-                return []
-            }
+                    const columnName = $this.data("column")
+                    const updateType = $this.data("updatetype")
 
-            const getPopupFields = () => {
-                const allFields = getColumnsData()
-                return allFields.filter(c => c && c.popup)
-            }
+                    if (columnName && updateType) {
+                        let inputValue = $this.val()
 
-            const updateColumnsData = (columnName, updateType, value) => {
-                let columnsData = getColumnsData()
+                        if (inputType === "checkbox") {
+                            inputValue = $this.is(':checked')
+                        }
+                        updateColumnsData(columnName, updateType, inputValue)
+                    }
+                })
 
+                const getColumnsData = () => {
+                    let columnsData = $columnsInput.val()
 
-                columnsData = columnsData.reduce((all, item) => {
-                    if (item.name && item.name === columnName) {
-                        item[updateType] = value
-                    }
+                    if (columnsData) {
+                        columnsData = JSON.parse(columnsData)
 
-                    all.push(item)
+                        return columnsData
+                    }
 
-                    return all
-                }, [])
+                    return []
+                }
 
-                if (columnsData) {
-                    $columnsInput.val(JSON.stringify(columnsData))
+                const getPopupFields = () => {
+                    const allFields = getColumnsData()
+                    return allFields.filter(c => c && c.popup)
                 }
-            }
 
-            function featureHtml(f) {
-                const p = f.properties;
-                const popupFields = getPopupFields()
+                const updateColumnsData = (columnName, updateType, value) => {
+                    let columnsData = getColumnsData()
 
 
-                const popupProps = Object.keys(p).reduce((all, key) => {
-                    if (popupFields.find(f => f.name === key)) {
-                        all[key] = p[key]
-                    }
-                    return all
-                }, {})
+                    columnsData = columnsData.reduce((all, item) => {
+                        if (item.name && item.name === columnName) {
+                            item[updateType] = value
+                        }
+
+                        all.push(item)
 
+                        return all
+                    }, [])
 
-                if (popupProps && !!Object.keys(popupProps).length) {
-                    let h = "<p>";
-                    for (let k in popupProps) {
-                        const column = popupFields.find(f => f.name === k)
-                        h += "<b>" + `${column.label ? column.label : k}` + ":</b> " + popupProps[k] + "<br/>"
+                    if (columnsData) {
+                        $columnsInput.val(JSON.stringify(columnsData))
                     }
-                    h += "</p>";
-                    return h
                 }
-                return null
-            }
 
+                function featureHtml(f) {
+                    const p = f.properties;
+                    const popupFields = getPopupFields()
+
+
+                    const popupProps = Object.keys(p).reduce((all, key) => {
+                        if (popupFields.find(f => f.name === key)) {
+                            all[key] = p[key]
+                        }
+                        return all
+                    }, {})
+
+                    if (popupProps && !!Object.keys(popupProps).length) {
+                        let h = "<div class='station-popup-content'>";
+                        for (let k in popupProps) {
+                            const column = popupFields.find(f => f.name === k)
+                            h += "<p><b>" + `${column.label ? column.label : k}` + ":</b> " + popupProps[k] + "<br/></p>"
+                        }
+                        h += "</div>";
+                        return h
+                    }
 
-            map.on('click', "stations-circle", function (e) {
-                const popContent = featureHtml(e.features[0])
-                if (popContent) {
-                    new maplibregl.Popup()
-                        .setLngLat(e.lngLat)
-                        .setHTML(popContent)
-                        .addTo(map);
+                    return null
                 }
-            });
 
 
-        })
+                map.on('click', "stations-circle", function (e) {
+                    const popContent = featureHtml(e.features[0])
+                    if (popContent) {
+                        new maplibregl.Popup()
+                            .setLngLat(e.lngLat)
+                            .setHTML(popContent)
+                            .addTo(map);
+                    }
+                });
+
+
+            })
 
-    </script>
+        </script>
+    {% endif %}
 {% endblock %}
```

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/stations_upload.html` & `geomanager-0.0.5/geomanager/templates/geomanager/stations_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/vector_edit_form.html` & `geomanager-0.0.5/geomanager/templates/geomanager/vector_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/vector_preview.html` & `geomanager-0.0.5/geomanager/templates/geomanager/wms_preview.html`

 * *Files 14% similar despite different names*

```diff
@@ -3,72 +3,80 @@
 {% load l10n %}
 {% load wagtailadmin_tags wagtailimages_tags static %}
 {% block titletag %}{% blocktrans with title=page.get_admin_display_title %}Preview Layers{{ title }}
 {% endblocktrans %}{% endblock %}
 
 {% block extra_css %}
     {{ block.super }}
+
     {{ form_media.css }}
 
     <link rel="stylesheet" href="{% static 'geomanager/css/vendor/maplibre-gl.css' %}">
     <link rel="stylesheet" href="{% static 'geomanager/css/preview-map.css' %}">
 {% endblock %}
 
+
 {% block content %}
     {% trans "Preview" as preview_str %}
 
     {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:dataset.title subtitle=page.get_admin_display_title icon="view" %}
 
     <div class="nice-padding">
         <div class="go-to-datasets">
             <a href="
-                    {% if selected_layer %}{{ vector_layer_list_url }}{% else %}{{ datasets_index_url }}{% endif %}"
+                    {% if selected_layer %}{{ wms_layer_list_url }}{% else %}{{ datasets_index_url }}{% endif %}"
                class="button bicolor button--icon">
                 <span class="icon-wrapper">
                     <svg class="icon icon-plus icon" aria-hidden="true">
                         <use href="#icon-arrow-left"></use>
                     </svg>
                 </span>{% if selected_layer %}Back to Layers{% else %}Back to Datasets{% endif %}
             </a>
         </div>
+
         <div class="w-field__input" data-field-input="">
             <label class="w-field__label" for="layer_select" id="layer_select-label">
                 Select Layer
             </label>
             <select name="select" id="layer_select">
-                {% for layer in dataset.vector_layers.all %}
+                {% for layer in dataset.wms_layers.all %}
                     <option value="{{ layer.pk }}"
-                            {% if selected_layer and selected_layer == layer.pk %}selected{% endif %}>{{ layer.title }}</option>
+                            {% if selected_layer and selected_layer.pk == layer.pk %}selected{% endif %}>{{ layer.title }}</option>
                 {% endfor %}
             </select>
         </div>
-        <div id="preview-map">
+        <div id="preview-map" style="position: relative">
             <div class="layer-timestamps-wrapper">
                 <div class="w-field__input">
-                    <label class="w-field__label" for="vector_table_select" id="vector_table_select-label">
-                        Datasets
+                    <label class="w-field__label" for="timestamps_select" id="timestamps_select-label">
+                        Time
                     </label>
-                    <select name="select" id="vector_table_select">
+                    <select name="select" id="timestamps_select">
                     </select>
                 </div>
             </div>
         </div>
     </div>
 
 {% endblock %}
 
 {% block extra_js %}
     {{ block.super }}
 
     {{ form_media.js }}
     <script src="{% static 'geomanager/js/vendor/maplibre-gl.js' %}"></script>
+    <script src="{% static 'geomanager/js/vendor/ol.min.js' %}"></script>
 
     <script>
+        let dataLayers = '{{ dataset_layers|escapejs }}';
+        if (dataLayers) {
+            dataLayers = JSON.parse(dataLayers)
+        }
         window.geomanager_opts = {
-            vectorTilesUrl: "{{ vector_tiles_url }}",
-            dataVectorApiBaseUrl: "{{ data_vector_api_base_url }}",
+            dataLayers: dataLayers
         }
     </script>
 
     <!-- Main script -->
-    <script src="{% static 'geomanager/js/vector-preview.js' %}"></script>
+    <script src="{% static 'geomanager/js/wms-preview.js' %}"></script>
+
 {% endblock %}
```

#### html2text {}

```diff
@@ -4,14 +4,14 @@
 {% endblocktrans %}{% endblock %} {% block extra_css %} {{ block.super }} {
 { form_media.css }}
 
  {% endblock %} {% block content %} {% trans "Preview" as preview_str %} {%
 include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:
 dataset.title subtitle=page.get_admin_display_title icon="view" %}
 ____{%_if_selected_layer_%}Back_to_Layers{%_else_%}Back_to_Datasets{%_endif_%}
-{% for layer in dataset.vector_layers.all %}
-% if selected_layer and selected_layer == layer.pk %}selected{% endif %}>{
+{% for layer in dataset.wms_layers.all %}
+% if selected_layer and selected_layer.pk == layer.pk %}selected{% endif %}>{
 { layer.title }}
 {% endfor %}
 {% endblock %} {% block extra_js %} {{ block.super }} {{ form_media.js }}
 
  {% endblock %}
```

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/vector_upload.html` & `geomanager-0.0.5/geomanager/templates/geomanager/vector_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/geomanager/widgets/raster_style_widget.html` & `geomanager-0.0.5/geomanager/templates/geomanager/widgets/raster_style_widget.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/templates/modeladmin/index_without_custom_create.html` & `geomanager-0.0.5/geomanager/templates/modeladmin/index_without_custom_create.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/urls.py` & `geomanager-0.0.5/geomanager/urls.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/utils/raster_utils.py` & `geomanager-0.0.5/geomanager/utils/raster_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from large_image.exceptions import TileSourceError
 from rasterio import CRS
 from rasterio.mask import mask
 from rest_framework.exceptions import APIException
 from rio_cogeo.cogeo import cog_translate
 from rio_cogeo.profiles import cog_profiles
-from shapely import wkb
+from shapely import wkb, Polygon
 
 from geomanager.errors import UnsupportedRasterFormat
 from geomanager.models import LayerRasterFile, Geostore
 
 
 def get_tile_source(path, options=None):
     if options is None:
@@ -276,20 +276,52 @@
 
     with rio.open(out_file, "w", **out_meta) as dest:
         dest.write(out_img)
 
     return out_file
 
 
+def clip_netcdf(nc_path, geom, out_file):
+    rds = xr.open_dataset(nc_path, engine="rasterio")
+
+    # write crs
+    rds.rio.write_crs("epsg:4326", inplace=True)
+
+    # clip
+    rds = rds.rio.clip([geom], "epsg:4326", drop=True)
+
+    # write clipped data to file
+    rds.to_netcdf(out_file)
+
+    rds.close()
+
+    return out_file
+
+
 def field_file_to_local_path_for_geostore(path, geostore):
     field_file_basename = pathlib.PurePath(path.name).name
     directory = get_cache_dir() / f"{type(path.instance).__name__}-{path.instance.pk}" / "geostore"
     dest_path = directory / f"{geostore.pk.hex}-{field_file_basename}"
     lock = get_file_lock(dest_path)
     safe = get_file_safe_path(dest_path)
 
     with lock.acquire():
         if not safe.exists():
             dest_path.parent.mkdir(parents=True, exist_ok=True)
             clip_geotiff(path.file.name, geostore.geom, dest_path)
 
     return dest_path
+
+
+def bounds_to_polygon(bounds):
+    polygon_coords = ((bounds[0], bounds[1]), (bounds[2], bounds[1]), (bounds[2], bounds[3]), (bounds[0], bounds[3]))
+    return Polygon(polygon_coords)
+
+
+def check_raster_bounds_with_boundary(raster_bounds, boundary_bounds):
+    boundary_poly = bounds_to_polygon(boundary_bounds)
+    raster_poly = bounds_to_polygon(raster_bounds)
+
+    intersects = boundary_poly.intersects(raster_poly)
+    contains = boundary_poly.contains(raster_poly)
+
+    return intersects, contains
```

### Comparing `geomanager-0.0.4/geomanager/utils/tile_gl.py` & `geomanager-0.0.5/geomanager/utils/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/utils/vector_utils.py` & `geomanager-0.0.5/geomanager/utils/vector_utils.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/views/__init__.py` & `geomanager-0.0.5/geomanager/views/__init__.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/views/auth.py` & `geomanager-0.0.5/geomanager/views/auth.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from allauth.account.forms import ResetPasswordForm
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
+from django.utils.module_loading import import_string
 from rest_framework import generics
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
 from rest_framework_simplejwt.exceptions import TokenError, InvalidToken
 from rest_framework_simplejwt.settings import api_settings
 from rest_framework_simplejwt.tokens import AccessToken
-from django.utils.module_loading import import_string
 from rest_framework_simplejwt.views import TokenObtainPairView, TokenVerifyView
 
 from geomanager.serializers import RegisterSerializer, ResetPasswordSerializer
 from geomanager.serializers.auth import EmailTokenObtainSerializer
 
 
 class RegisterView(generics.CreateAPIView):
```

### Comparing `geomanager-0.0.4/geomanager/views/profile.py` & `geomanager-0.0.5/geomanager/views/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ObjectDoesNotExist
-from rest_framework.decorators import api_view
+from rest_framework.decorators import api_view, renderer_classes
+from rest_framework.renderers import JSONRenderer
 from rest_framework.response import Response
 
 from geomanager.forms import GeoManagerUserProfileForm
 from geomanager.models import GeoManagerUserProfile
 from geomanager.serializers.profile import GeoManagerUserProfileSerializer
 
 
 @api_view(['GET'])
+@renderer_classes([JSONRenderer])
 def get_geomanager_user_profile(request, user_id):
     try:
         profile = GeoManagerUserProfile.objects.get(user=user_id)
     except ObjectDoesNotExist:
         return Response({"detail": "Profile does not exist for user"}, status=404)
 
     serializer = GeoManagerUserProfileSerializer(profile)
 
     return Response(serializer.data)
 
 
 @api_view(['PATCH'])
+@renderer_classes([JSONRenderer])
 def create_or_update_geomanager_user_profile(request, user_id):
     try:
         profile = GeoManagerUserProfile.objects.get(user=user_id)
     except ObjectDoesNotExist:
         profile = None
 
     try:
```

### Comparing `geomanager-0.0.4/geomanager/views/raster.py` & `geomanager-0.0.5/geomanager/views/raster.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import datetime
 import json
+import tempfile
 from typing import Optional, Any
 
+from adminboundarymanager.models import AdminBoundarySettings, AdminBoundary
 from django.core.exceptions import ValidationError, ObjectDoesNotExist
+from django.core.files.base import File
 from django.http import JsonResponse, HttpResponse
 from django.shortcuts import get_object_or_404, render
 from django.template.defaultfilters import filesizeformat
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.decorators import method_decorator
 from django.utils.translation import gettext_lazy as _
 from django_large_image import tilesource
 from large_image.exceptions import TileSourceXYZRangeError
+from rest_framework.renderers import JSONRenderer
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.views import APIView
+from shapely import wkb
 from wagtail.admin.auth import (
     user_passes_test,
     user_has_any_page_permission,
     permission_denied
 )
 from wagtail.contrib.modeladmin.helpers import AdminURLHelper
 from wagtail.models import Site
@@ -38,15 +43,18 @@
 from geomanager.models.raster import WmsLayer
 from geomanager.serializers.raster import WmsLayerSerializer
 from geomanager.utils import UUIDEncoder
 from geomanager.utils.raster_utils import (
     get_tile_source,
     read_raster_info,
     create_layer_raster_file,
-    get_raster_pixel_data, get_geostore_data
+    get_raster_pixel_data, get_geostore_data,
+    check_raster_bounds_with_boundary,
+    clip_netcdf, clip_geotiff,
+    bounds_to_polygon
 )
 
 ALLOWED_RASTER_EXTENSIONS = ["tif", "tiff", "geotiff", "nc"]
 
 
 @user_passes_test(user_has_any_page_permission)
 def upload_raster_file(request, dataset_id=None, layer_id=None):
@@ -97,23 +105,80 @@
         "layer": layer,
         "datasets_index_url": dataset_list_url,
         "layers_index_url": layer_list_url,
         "dataset_preview_url": dataset.preview_url,
         "layer_preview_url": layer_preview_url
     })
 
+    gm_settings = GeomanagerSettings.for_request(request)
+
+    crop_raster = gm_settings.crop_raster_to_country
+
     # Check if user is submitting
     if request.method == 'POST':
         files = request.FILES.getlist('files[]', None)
-        file = files[0]
+        upload_file = files[0]
 
-        upload = RasterUpload.objects.create(file=file, dataset=dataset)
+        upload = RasterUpload.objects.create(file=upload_file, dataset=dataset)
 
         raster_metadata = read_raster_info(upload.file.path)
 
+        if crop_raster and raster_metadata.get("bounds"):
+            abm_settings = AdminBoundarySettings.for_request(request)
+            abm_extents = abm_settings.combined_countries_bounds
+            abm_countries = abm_settings.countries_list
+
+            intersects_with_boundary, within_boundary = check_raster_bounds_with_boundary(raster_metadata.get("bounds"),
+                                                                                          abm_extents)
+
+            # clipping raster to boundaries
+            if intersects_with_boundary and not within_boundary:
+                raster_driver = raster_metadata.get("driver")
+
+                country_geoms = []
+                for country in abm_countries:
+                    code = country.get("code")
+                    alpha3 = country.get("alpha3")
+
+                    # query using code (2-letter code)
+                    country_boundary = AdminBoundary.objects.filter(level=0, gid_0=code).first()
+
+                    # query using alpha 3 (3-letter code)
+                    if not country_boundary:
+                        country_boundary = AdminBoundary.objects.filter(level=0, gid_0=alpha3).first()
+
+                    if country_boundary:
+                        shapely_geom = wkb.loads(country_boundary.geom.hex)
+                        country_geoms.append(shapely_geom)
+                    else:
+                        # use bbox instead
+                        bbox = country.get("bbox")
+                        if bbox:
+                            bounds_geom = bounds_to_polygon(bbox)
+                            country_geoms.append(bounds_geom)
+
+                union_polygon = country_geoms[0]
+                for polygon in country_geoms[1:]:
+                    union_polygon = union_polygon.union(polygon)
+
+                if raster_driver == "netCDF":
+                    clip_fn = clip_netcdf
+                    suffix = ".nc"
+                else:
+                    clip_fn = clip_geotiff
+                    suffix = ".tif"
+
+                with tempfile.NamedTemporaryFile(suffix=suffix) as f:
+                    clipped_raster = clip_fn(upload.file.path, union_polygon, f.name)
+                    raster_metadata = read_raster_info(clipped_raster)
+
+                    with open(clipped_raster, 'rb') as clipped_file:
+                        file_obj = File(clipped_file, name=f.name)
+                        upload.file.save(upload.file.name, file_obj, save=True)
+
         upload.raster_metadata = raster_metadata
         upload.save()
 
         query_set = FileImageLayer.objects.filter(dataset=dataset)
 
         initial_data = {
             "layer": layer_id if layer_id else query_set.first()
@@ -490,27 +555,31 @@
         mime_type = source.getTileMimeType()
 
         return HttpResponse(tile_binary, content_type=mime_type)
 
 
 @method_decorator(cache_page, name='get')
 class RasterDataPixelView(RasterDataMixin, APIView):
+    renderer_classes = [JSONRenderer]
+
     def get(self, request):
         try:
             pixel_data = self.get_pixel_data(request)
         except QueryParamRequired as e:
             return JsonResponse(e.serialize, status=400)
         except RasterFileNotFound as e:
             return JsonResponse({"message": e}, status=404)
 
         return Response(pixel_data)
 
 
 @method_decorator(cache_page, name='get')
 class RasterDataPixelTimeseriesView(RasterDataMixin, APIView):
+    renderer_classes = [JSONRenderer]
+
     def get(self, request):
         try:
             raster_files = self.get_multiple_raster_files(request)
             x_coord, y_coord = self.get_coords(request)
         except QueryParamRequired as e:
             return JsonResponse(e.serialize, status=400)
         except RasterFileNotFound as e:
@@ -523,14 +592,16 @@
             timeseries_data.append({"date": raster_file.time, "value": pixel_data})
 
         return Response(timeseries_data)
 
 
 @method_decorator(cache_page, name='get')
 class RasterDataGeostoreView(RasterDataMixin, APIView):
+    renderer_classes = [JSONRenderer]
+
     def get(self, request):
         try:
             value_type = self.get_query_param(request, "value_type")
             geostore = self.get_geostore(request)
             raster_file = self.get_single_raster_file(request)
             data = get_geostore_data(raster_file.file, geostore, value_type)
         except QueryParamRequired as e:
@@ -538,14 +609,16 @@
         except (RasterFileNotFound, GeostoreNotFound) as e:
             return JsonResponse({"message": e}, status=404)
         return Response(data)
 
 
 @method_decorator(cache_page, name='get')
 class RasterDataGeostoreTimeseriesView(RasterDataMixin, APIView):
+    renderer_classes = [JSONRenderer]
+
     def get(self, request):
         try:
             value_type = self.get_query_param(request, "value_type")
             raster_files = self.get_multiple_raster_files(request)
             geostore = self.get_geostore(request)
         except QueryParamRequired as e:
             return JsonResponse(e.serialize, status=400)
```

### Comparing `geomanager-0.0.4/geomanager/views/stations.py` & `geomanager-0.0.5/geomanager/views/stations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import tempfile
 
-from adminboundarymanager.models import AdminBoundarySettings
 from django.conf import settings
 from django.db import connection, close_old_connections
 from django.http import Http404, HttpResponse
 from django.shortcuts import render, redirect
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.views import View
@@ -91,22 +90,21 @@
         return render(request, template_name=template, context=context)
 
 
 @user_passes_test(user_has_any_page_permission)
 def preview_stations(request):
     template = "geomanager/stations_preview.html"
 
-    abm_settings = AdminBoundarySettings.for_request(request)
     stations_settings = StationSettings.for_request(request)
     stations_vector_tiles_url = request.scheme + '://' + request.get_host() + \
                                 stations_settings.stations_vector_tiles_url
 
     context = {
         "mapConfig": {
-            "combinedBbox": abm_settings.combined_countries_bounds,
+            "stationBounds": stations_settings.bounds,
             "stationsVectorTilesUrl": stations_vector_tiles_url,
         },
         "load_stations_url": reverse("geomanager_load_stations"),
     }
 
     if stations_settings.columns:
         context.update({"station_columns": stations_settings.columns})
```

### Comparing `geomanager-0.0.4/geomanager/views/tile_gl.py` & `geomanager-0.0.5/geomanager/views/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/views/vector.py` & `geomanager-0.0.5/geomanager/views/vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
 
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import connection, close_old_connections
 from django.http import JsonResponse, Http404, HttpResponse
-from django.shortcuts import get_object_or_404, render
+from django.shortcuts import get_object_or_404, render, redirect
 from django.template.defaultfilters import filesizeformat
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.translation import gettext_lazy as _
 from django.views import View
+from wagtail.admin import messages
 from wagtail.admin.auth import user_passes_test, user_has_any_page_permission, permission_denied
 from wagtail.contrib.modeladmin.helpers import AdminURLHelper
 from wagtail.models import Site
 from wagtail.snippets.permissions import get_permission_name
-from wagtailcache.cache import cache_page
+from wagtailcache.cache import cache_page, clear_cache
 
-from geomanager.forms import VectorLayerFileForm
+from geomanager.forms import VectorLayerFileForm, VectorTableForm
 from geomanager.models import Dataset
 from geomanager.models.core import GeomanagerSettings
 from geomanager.models.vector import VectorLayer, VectorUpload, PgVectorTable
 from geomanager.settings import geomanager_settings
 from geomanager.utils.vector_utils import ogr_db_import
 
 ALLOWED_VECTOR_EXTENSIONS = ["zip", "geojson", "csv"]
@@ -226,34 +227,71 @@
         return JsonResponse({"success": True})
 
     return JsonResponse({"success": True, })
 
 
 @user_passes_test(user_has_any_page_permission)
 def preview_vector_layers(request, dataset_id, layer_id=None):
+    template_name = 'geomanager/vector_preview.html'
     dataset = get_object_or_404(Dataset, pk=dataset_id)
 
     base_absolute_url = request.scheme + '://' + request.get_host()
 
     dataset_admin_helper = AdminURLHelper(Dataset)
     dataset_list_url = dataset_admin_helper.get_action_url("index")
 
     vector_layer_admin_helper = AdminURLHelper(VectorLayer)
     vector_layer_list_url = vector_layer_admin_helper.get_action_url("index")
 
+    geojson_url = request.build_absolute_uri(
+        reverse("feature_serv", args=("table_name",)).replace("table_name.geojson", ""))
+
+    data_table = PgVectorTable.objects.filter(layer__id=layer_id)
+
+    if data_table.exists():
+        data_table = data_table.first()
+    else:
+        data_table = None
+
+    initial_data = {
+        "columns": data_table.properties if data_table else [],
+    }
+
     context = {
         "dataset": dataset,
         "selected_layer": layer_id,
         "datasets_index_url": dataset_list_url,
         "vector_layer_list_url": vector_layer_list_url,
         "data_vector_api_base_url": request.build_absolute_uri("/api/vector-data"),
         "vector_tiles_url": base_absolute_url + "/api/vector-tiles/{z}/{x}/{y}",
+        "geojson_url": geojson_url,
+        "data_table": data_table,
     }
 
-    return render(request, 'geomanager/vector_preview.html', context)
+    if request.POST:
+        form = VectorTableForm(request.POST, initial=initial_data)
+        if form.is_valid():
+            columns = form.cleaned_data.get("columns")
+
+            if columns and data_table:
+                data_table.properties = columns
+                data_table.save()
+                # clear wagtail cache
+                clear_cache()
+            messages.success(request, "Data fields updated successfully")
+            # redirect
+            return redirect(reverse("geomanager_preview_vector_layer", args=(dataset_id, layer_id)))
+        else:
+            context.update({"form": form})
+            return render(request, template_name=template_name, context=context)
+    else:
+        form = VectorTableForm(initial=initial_data)
+        context.update({"form": form})
+
+    return render(request, template_name=template_name, context=context)
 
 
 @method_decorator(cache_page, name='get')
 class VectorTileView(View):
     def get(self, request, z, x, y):
         table_name = request.GET.get("table_name")
 
@@ -288,17 +326,14 @@
             tile = cursor.fetchone()[0]
             if not len(tile):
                 raise Http404()
 
         return HttpResponse(tile, content_type="application/x-protobuf")
 
 
-
-
-
 @method_decorator(cache_page, name='get')
 class GeoJSONPgTableView(View):
     def get(self, request, table_name):
         try:
             vector_table = PgVectorTable.objects.get(table_name=table_name)
         except ObjectDoesNotExist:
             return JsonResponse({"message": f"Table with name: '{table_name}' does not exist"}, status=404)
```

### Comparing `geomanager-0.0.4/geomanager/viewsets/aoi.py` & `geomanager-0.0.5/geomanager/viewsets/aoi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from rest_framework import viewsets
 from rest_framework.permissions import IsAuthenticated
+from rest_framework.renderers import JSONRenderer
 
 from geomanager.models import AreaOfInterest
 from geomanager.serializers.aoi import AoiSerializer
 
 
 class AoiViewSet(viewsets.ModelViewSet):
     serializer_class = AoiSerializer
     queryset = AreaOfInterest.objects.all()
     permission_classes = [IsAuthenticated]
+    renderer_classes = [JSONRenderer]
 
     def get_queryset(self):
         queryset = self.queryset.filter(user=self.request.user.id)
         return queryset
 
     def create(self, request, *args, **kwargs):
         request.data.update({"user": request.user.id})
```

### Comparing `geomanager-0.0.4/geomanager/viewsets/core.py` & `geomanager-0.0.5/geomanager/viewsets/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,38 @@
 from adminboundarymanager.models import AdminBoundarySettings
 from django.utils.decorators import method_decorator
 from rest_framework import mixins, viewsets
+from rest_framework.renderers import JSONRenderer
 from rest_framework.response import Response
 from wagtailcache.cache import cache_page
 
 from geomanager import serializers
 from geomanager.models import Dataset
 from geomanager.models.core import GeomanagerSettings, Metadata
 
 
 class DatasetListViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     queryset = Dataset.objects.filter(published=True)
     serializer_class = serializers.DatasetSerializer
 
+    renderer_classes = [JSONRenderer]
+
     def get_serializer_context(self):
         context = super().get_serializer_context()
         context.update({'request': self.request})
         return context
 
     @method_decorator(cache_page)
     def list(self, request, *args, **kwargs):
         queryset = self.get_queryset()
         dataset_with_layers = []
 
-        icons = []
-
         # get only datasets with layers defined
         for dataset in queryset:
             if dataset.has_layers():
-                if dataset.layer_type == "vector":
-                    vector_layers = dataset.vector_layers.all()
-                    for layer in vector_layers:
-                        layer_config = layer.layer_config()
-                        render_layers = layer_config.get("render", {}).get("layers", [])
-                        for render_layer in render_layers:
-                            if render_layer.get("type", None) == "symbol":
-                                icon_image = render_layer.get("layout", {}).get("icon-image")
-                                icon_color = render_layer.get("paint", {}).get("icon-color")
-                                if icon_image:
-                                    icon = {"icon": icon_image, "type": "sprite"}
-                                    if icon_color:
-                                        icon.update({"icon-color": icon_color})
-                                    icons.append(icon)
-
                 dataset_with_layers.append(dataset)
 
         serializer = self.get_serializer(dataset_with_layers, many=True)
 
         lm_settings = GeomanagerSettings.for_request(request)
         abm_settings = AdminBoundarySettings.for_request(request)
         datasets = serializer.data
@@ -65,14 +51,14 @@
                     "baseUrl": lm_settings.cap_base_url,
                     "category": lm_settings.cap_sub_category.category.pk,
                     "subCategory": lm_settings.cap_sub_category.pk,
                     "refreshInterval": lm_settings.cap_auto_refresh_interval_milliseconds,
                     "metadata": lm_settings.cap_metadata.pk if lm_settings.cap_metadata else None
                 }})
 
-        return Response({"datasets": datasets, "config": config, "icons": icons})
+        return Response({"datasets": datasets, "config": config})
 
 
 @method_decorator(cache_page, name="retrieve")
 class MetadataViewSet(mixins.RetrieveModelMixin, viewsets.GenericViewSet):
     queryset = Metadata.objects.all()
     serializer_class = serializers.MetadataSerialiazer
```

### Comparing `geomanager-0.0.4/geomanager/viewsets/raster.py` & `geomanager-0.0.5/geomanager/viewsets/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.4/geomanager/viewsets/vector.py` & `geomanager-0.0.5/geomanager/viewsets/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from django.contrib.gis.geos import MultiPolygon
 from django.utils.decorators import method_decorator
 from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework import mixins
 from rest_framework import viewsets
 from rest_framework.decorators import action
 from rest_framework.exceptions import NotFound
+from rest_framework.renderers import JSONRenderer
 from rest_framework.response import Response
 from wagtailcache.cache import cache_page
 
 from geomanager import serializers
 from geomanager.models import Geostore
 from geomanager.models.vector import PgVectorTable
 from geomanager.serializers.vector import AdminBoundarySerializer, GeostoreSerializer
 
 
 class VectorTableFileDetailViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
+    renderer_classes = [JSONRenderer]
     queryset = PgVectorTable.objects.all()
     serializer_class = serializers.PgVectorTableSerializer
     filter_backends = [DjangoFilterBackend]
     filterset_fields = ["layer"]
 
 
 class AdminBoundaryViewSet(viewsets.ViewSet):
+    renderer_classes = [JSONRenderer]
+
     @action(detail=True, methods=['get'])
     @method_decorator(cache_page)
     def get(self, request):
         countries = AdminBoundary.objects.filter(level=0)
         data = AdminBoundarySerializer(countries, many=True).data
         return Response(data)
 
@@ -45,14 +49,16 @@
     def get_sub_regions(self, request, gid_0, gid_1):
         countries = AdminBoundary.objects.filter(level=2, gid_0=gid_0, gid_1=gid_1)
         data = AdminBoundarySerializer(countries, many=True).data
         return Response(data)
 
 
 class GeostoreViewSet(viewsets.ViewSet):
+    renderer_classes = [JSONRenderer]
+
     @action(detail=True, methods=['post'])
     def post(self, request):
         # parse the GeoJSON from the POST data
         payload = json.loads(request.body.decode('utf-8'))
 
         geojson = payload.get("geojson")
```

### Comparing `geomanager-0.0.4/geomanager/wagtail_hooks.py` & `geomanager-0.0.5/geomanager/wagtail_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,18 @@
             </a>
         """
         return mark_safe(button_html)
 
     def preview_dataset(self, obj):
         if not obj.preview_url:
             return None
+
+        if obj.layer_type == "vector":
+            return None
+
         disabled = "" if obj.can_preview() else "disabled"
         label = _("Preview Dataset")
         button_html = f"""
             <a href="{obj.preview_url}" class="button button-small button--icon button-secondary {disabled}">
                 <span class="icon-wrapper">
                     <svg class="icon icon-plus icon" aria-hidden="true">
                         <use href="#icon-view"></use>
@@ -209,16 +213,14 @@
                 </span>
                 {label}
             </a>
         """
         return mark_safe(button_html)
 
     def upload_files(self, obj):
-        if not obj.upload_url:
-            return None
         disabled = "" if obj.has_layers() else "disabled"
         label = _("Upload Files")
         button_html = f"""
             <a href="{obj.upload_url}" class="button button-small bicolor button--icon {disabled}">
                 <span class="icon-wrapper">
                     <svg class="icon icon-plus icon" aria-hidden="true">
                         <use href="#icon-upload"></use>
@@ -514,17 +516,19 @@
             <a href="{obj.dataset.dataset_url()}">
             {obj.dataset.title}
             </a>
         """
         return mark_safe(button_html)
 
     def upload_files(self, obj):
+        disabled = "" if not obj.has_data_table else "disabled"
+
         label = _("Upload Files")
         button_html = f"""
-            <a href="{obj.upload_url}" class="button button-small bicolor button--icon">
+            <a href="{obj.upload_url}" class="button button-small bicolor button--icon" {disabled}>
                 <span class="icon-wrapper">
                     <svg class="icon icon-plus icon" aria-hidden="true">
                         <use href="#icon-upload"></use>
                     </svg>
                 </span>
                 {label}
             </a>
```

### Comparing `geomanager-0.0.4/geomanager.egg-info/PKG-INFO` & `geomanager-0.0.5/geomanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wagtail based Geospatial Data Manager
 Home-page: https://github.com/wmo-raf/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `geomanager-0.0.4/geomanager.egg-info/SOURCES.txt` & `geomanager-0.0.5/geomanager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 geomanager/migrations/0004_alter_dataset_can_clip.py
 geomanager/migrations/0005_delete_countryboundary_and_more.py
 geomanager/migrations/0006_stationsettings.py
 geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py
 geomanager/migrations/0008_stationsettings_name_column.py
 geomanager/migrations/0009_stationsettings_popup_props.py
 geomanager/migrations/0010_remove_stationsettings_popup_props.py
+geomanager/migrations/0011_vectorlayericon.py
+geomanager/migrations/0012_geomanagersettings_crop_raster_to_country.py
+geomanager/migrations/0013_geomanagersettings_logo_external_link_and_more.py
+geomanager/migrations/0014_geomanagersettings_privacy_policy_page_and_more.py
 geomanager/migrations/__init__.py
 geomanager/models/__init__.py
 geomanager/models/aoi.py
 geomanager/models/core.py
 geomanager/models/profile.py
 geomanager/models/raster.py
 geomanager/models/stations.py
@@ -47,15 +51,17 @@
 geomanager/serializers/aoi.py
 geomanager/serializers/auth.py
 geomanager/serializers/core.py
 geomanager/serializers/profile.py
 geomanager/serializers/raster.py
 geomanager/serializers/vector.py
 geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
+geomanager/static/geomanager/css/bulma-navbar.css
 geomanager/static/geomanager/css/preview-map.css
+geomanager/static/geomanager/css/stations_preview.css
 geomanager/static/geomanager/css/upload.css
 geomanager/static/geomanager/css/vendor/maplibre-gl.css
 geomanager/static/geomanager/images/geomapviewer-logo.png
 geomanager/static/geomanager/js/add-multiple.js
 geomanager/static/geomanager/js/colorbrewer.js
 geomanager/static/geomanager/js/mbt_source_extra.js
 geomanager/static/geomanager/js/raster-preview.js
@@ -80,14 +86,15 @@
 geomanager/templates/geomanager/wms_preview.html
 geomanager/templates/geomanager/widgets/raster_style_widget.html
 geomanager/templates/modeladmin/index_without_custom_create.html
 geomanager/templatetags/__init__.py
 geomanager/templatetags/geomanager_tags.py
 geomanager/utils/__init__.py
 geomanager/utils/raster_utils.py
+geomanager/utils/svg.py
 geomanager/utils/tile_gl.py
 geomanager/utils/vector_utils.py
 geomanager/views/__init__.py
 geomanager/views/auth.py
 geomanager/views/core.py
 geomanager/views/nextjs.py
 geomanager/views/profile.py
```

### Comparing `geomanager-0.0.4/geomanager.egg-info/requires.txt` & `geomanager-0.0.5/geomanager.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 wagtail>=4.2.2
-adm-boundary-manager>=0.0.1
+adm-boundary-manager>=0.0.5
 django_extensions>=3.2.1
 wagtail_color_panel>=1.4.1
 wagtail-font-awesome-svg>=0.0.3
 django_json_widget>=1.1.1
 django_nextjs>=2.2.2
 django-allauth>=0.54.0
 django-large-image>=0.10.0
@@ -15,10 +15,13 @@
 rasterio>=1.3.6
 rio-cogeo>=3.5.1
 xarray>=2023.3.0
 rioxarray>=0.14.0
 shapely>=2.0.1
 djangorestframework-simplejwt>=5.2.2
 wagtail-humanitarian-icons>=2.0.0
-wagtail-icon-chooser>=0.0.1
+wagtail-icon-chooser>=0.0.5
 matplotlib>=3.7.1
-wagtail-cache>=2.2.0
+django-tables2>=2.6.0
+django-tables2-bulma-template>=0.2.0
+CairoSVG>=2.7.0
+wagtail-cache>=2.3.0
```

### Comparing `geomanager-0.0.4/setup.cfg` & `geomanager-0.0.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geomanager
-version = 0.0.4
+version = 0.0.5
 description = Wagtail based Geospatial Data Manager
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/geomanager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
@@ -22,15 +22,15 @@
 
 [options]
 packages = find:
 include_package_data = true
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
-	adm-boundary-manager>=0.0.1
+	adm-boundary-manager>=0.0.5
 	django_extensions>=3.2.1
 	wagtail_color_panel>=1.4.1
 	wagtail-font-awesome-svg>=0.0.3
 	django_json_widget>=1.1.1
 	django_nextjs>=2.2.2
 	django-allauth>=0.54.0
 	django-large-image>=0.10.0
@@ -42,15 +42,18 @@
 	rasterio>=1.3.6
 	rio-cogeo>=3.5.1
 	xarray>=2023.3.0
 	rioxarray>=0.14.0
 	shapely>=2.0.1
 	djangorestframework-simplejwt>=5.2.2
 	wagtail-humanitarian-icons>=2.0.0
-	wagtail-icon-chooser>=0.0.1
+	wagtail-icon-chooser>=0.0.5
 	matplotlib>=3.7.1
-	wagtail-cache>=2.2.0
+	django-tables2>=2.6.0
+	django-tables2-bulma-template>=0.2.0
+	CairoSVG>=2.7.0
+	wagtail-cache>=2.3.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

