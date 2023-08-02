# Comparing `tmp/shapelets-platform-2.0.95.tar.gz` & `tmp/shapelets-platform-2.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-platform-2.0.95.tar", last modified: Wed Aug  2 09:47:32 2023, max compression
+gzip compressed data, was "shapelets-platform-2.0.96.tar", last modified: Wed Aug  2 16:59:06 2023, max compression
```

## Comparing `shapelets-platform-2.0.95.tar` & `shapelets-platform-2.0.96.tar`

### file list

```diff
@@ -1,296 +1,276 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/COPYING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/noxfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     2813 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.559232 shapelets-platform-2.0.95/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.567232 shapelets-platform-2.0.95/src/shapelets/
--rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19253 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)    52015 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_relations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_uom.py
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_version.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.571232 shapelets-platform-2.0.95/src/shapelets/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    70253 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/data_app.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/data_app_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.575232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/
--rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/attribute_names.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.583232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/
--rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3364 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/altair_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/bar_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2584 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/folium_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/heatmap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19966 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/line_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/pie_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/plotly_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/polar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/radar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/scatter_plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.587232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/filtering_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_field.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/temporal_context.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.595232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/
--rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2014 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/button.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/collection_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8331 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8706 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/gauge.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8126 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5929 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/metric.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11032 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/number_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/progress.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9101 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/radio_group.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.599232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/resources/
--rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
--rw-r--r--   0 vsts      (1001) docker     (123)     4631 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/ring.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10545 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/sequence_list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14849 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/slider.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9017 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/timer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/datetime_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.599232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/
--rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/grid_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6038 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/horizontal_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/panel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5000 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/tabs_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5660 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/vertical_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26169 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/widget.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/iris.csv
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.607232 shapelets-platform-2.0.95/src/shapelets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/altair.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/capsule.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/collection.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/function_description.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/function_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/group.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/metadata_item.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/ndarray.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/replicated_param.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/sequence.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/sequence_axis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/user.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/view_match.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.611233 shapelets-platform-2.0.95/src/shapelets/svr/
--rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.619233 shapelets-platform-2.0.95/src/shapelets/svr/authn/
--rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/authhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/authrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/authservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/gc_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.619233 shapelets-platform-2.0.95/src/shapelets/svr/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.627233 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/access_token_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen2.py
--rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/dynamic_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/local.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/protocols.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/smb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/vfs_sample_config.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.635233 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3264 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataapps_ws.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9912 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2415 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.639233 shapelets-platform-2.0.95/src/shapelets/svr/db/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.639233 shapelets-platform-2.0.95/src/shapelets/svr/db/native/
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/native/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/native/database.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/native/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_builder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v4.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/setup.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/docs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.643233 shapelets-platform-2.0.95/src/shapelets/svr/execution/
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/executionhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/executionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/executionservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/iexecutionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/iexecutionservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.647233 shapelets-platform-2.0.95/src/shapelets/svr/groups/
--rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/groupservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4410 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/groupshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5028 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/groupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.651233 shapelets-platform-2.0.95/src/shapelets/svr/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/dataapps.py
--rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/function.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/groups.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/principals.py
--rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/users.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.659233 shapelets-platform-2.0.95/src/shapelets/svr/mustang/
--rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/asttranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/conversions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/core.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/decompiling.py
--rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/hashdict.py
--rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/identifier.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/ormtypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.659233 shapelets-platform-2.0.95/src/shapelets/svr/mustang/prototypes/
--rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/prototypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/python_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqlbuilding.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqltranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.667233 shapelets-platform-2.0.95/src/shapelets/svr/settings/
--rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/defaults.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/http.py
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/reload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/ssl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.667233 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/itelemetryservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/telemetryservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.671233 shapelets-platform-2.0.95/src/shapelets/svr/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/iusersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/iusersservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/usershttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/usersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/usersservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.671233 shapelets-platform-2.0.95/src/shapelets/svr/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/utils/crypto.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/utils/flexbytes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.675233 shapelets-platform-2.0.95/src/shapelets/svr/www/
--rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-08-02 09:47:25.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/altair.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/asset-manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/custom_sample.js
--rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/dataapp.json
--rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/robots.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.559232 shapelets-platform-2.0.95/src/shapelets/svr/www/static/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.675233 shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/
--rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
--rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.687233 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)  7622607 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   808300 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.695233 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/
--rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/audit.cb539a06.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/bin.7e762965.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/clear.27b15301.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/download-image.87310709.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/filter.cec803b8.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
--rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logout.57c593a5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/share.bc9a8370.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
--rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/systemd_template.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    11445 2023-08-02 09:47:32.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     1109 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.188452 shapelets-platform-2.0.96/
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/COPYING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-02 16:59:06.188452 shapelets-platform-2.0.96/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/noxfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     2856 2023-08-02 16:59:06.188452 shapelets-platform-2.0.96/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.076450 shapelets-platform-2.0.96/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.084451 shapelets-platform-2.0.96/src/shapelets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19253 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    52015 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/_relations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/_uom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-08-02 16:59:02.000000 shapelets-platform-2.0.96/src/shapelets/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/_version.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.084451 shapelets-platform-2.0.96/src/shapelets/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    70200 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/data_app.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/data_app_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.088451 shapelets-platform-2.0.96/src/shapelets/apps/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/attribute_names.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.092451 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      768 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3364 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/altair_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2129 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/bar_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2584 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/folium_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2627 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/heatmap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1783 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19323 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/line_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2129 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/pie_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/plotly_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2138 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/polar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/radar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4385 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/scatter_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.092451 shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      504 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/filtering_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1164 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/metadata_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1505 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/metadata_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/temporal_context.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.100451 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2014 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/button.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/checkbox.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2243 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/collection_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8331 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8706 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/datetime_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/gauge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8126 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5929 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/metric.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2108 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11032 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/number_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9101 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/radio_group.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.104451 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4631 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/ring.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10545 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1907 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/sequence_list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1929 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14849 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/slider.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/text.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9017 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/text_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/timer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/datetime_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.104451 shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/grid_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6038 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/horizontal_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/panel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5000 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/tabs_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5660 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/vertical_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26169 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/apps/widgets/widget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/iris.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.104451 shapelets-platform-2.0.96/src/shapelets/svr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.108451 shapelets-platform-2.0.96/src/shapelets/svr/authn/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/authn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/authn/authhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/authn/authrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/authn/authservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/authn/gc_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/authn/iauthrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/authn/iauthservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.108451 shapelets-platform-2.0.96/src/shapelets/svr/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.116451 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/access_token_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/azure_gen1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/azure_gen2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/dynamic_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_vfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/local.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/smb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/vfs_sample_config.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.120451 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3264 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataapps_ws.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9912 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataappshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2415 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataappsservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/idataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/dataapps/idataappsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.120451 shapelets-platform-2.0.96/src/shapelets/svr/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.124451 shapelets-platform-2.0.96/src/shapelets/svr/db/native/
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/native/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/native/database.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/native/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/schema_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v4.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/db/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/docs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.128451 shapelets-platform-2.0.96/src/shapelets/svr/execution/
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/execution/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/execution/executionhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/execution/executionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/execution/executionservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/execution/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/execution/iexecutionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/execution/iexecutionservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.132451 shapelets-platform-2.0.96/src/shapelets/svr/groups/
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/groups/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/groups/groupservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4410 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/groups/groupshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5028 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/groups/groupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/groups/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/groups/igroupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/groups/igroupsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.132451 shapelets-platform-2.0.96/src/shapelets/svr/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/model/dataapps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/model/function.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/model/groups.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/model/principals.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/model/users.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.140452 shapelets-platform-2.0.96/src/shapelets/svr/mustang/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/asttranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/core.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/decompiling.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/hashdict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/ormtypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.144452 shapelets-platform-2.0.96/src/shapelets/svr/mustang/prototypes/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/prototypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/python_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/sqlbuilding.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/mustang/sqltranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.148452 shapelets-platform-2.0.96/src/shapelets/svr/settings/
+-rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/http.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/reload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/settings.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/ssl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/settings/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.152452 shapelets-platform-2.0.96/src/shapelets/svr/telemetry/
+-rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/telemetry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/telemetry/itelemetryservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/telemetry/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/telemetry/telemetryservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.156452 shapelets-platform-2.0.96/src/shapelets/svr/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/users/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/users/iusersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/users/iusersservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/users/usershttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/users/usersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/users/usersservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.156452 shapelets-platform-2.0.96/src/shapelets/svr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/utils/crypto.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/svr/utils/flexbytes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.160452 shapelets-platform-2.0.96/src/shapelets/svr/www/
+-rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/altair.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/asset-manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/custom_sample.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/dataapp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-08-02 16:59:00.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-08-02 16:59:00.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/robots.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.076450 shapelets-platform-2.0.96/src/shapelets/svr/www/static/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.160452 shapelets-platform-2.0.96/src/shapelets/svr/www/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
+-rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.172452 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)  7622607 2023-08-02 16:59:02.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/2.379683b2.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   808300 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.184452 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/
+-rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/audit.cb539a06.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/bin.7e762965.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/clear.27b15301.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/download-image.87310709.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/filter.cec803b8.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logout.57c593a5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/share.bc9a8370.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-08-02 16:59:01.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-08-02 16:59:00.000000 shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-08-02 16:45:42.000000 shapelets-platform-2.0.96/src/shapelets/systemd_template.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 16:59:06.188452 shapelets-platform-2.0.96/src/shapelets_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-02 16:59:02.000000 shapelets-platform-2.0.96/src/shapelets_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    10804 2023-08-02 16:59:06.000000 shapelets-platform-2.0.96/src/shapelets_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-02 16:59:02.000000 shapelets-platform-2.0.96/src/shapelets_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-08-02 16:59:02.000000 shapelets-platform-2.0.96/src/shapelets_platform.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-08-02 16:59:02.000000 shapelets-platform-2.0.96/src/shapelets_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-08-02 16:59:02.000000 shapelets-platform-2.0.96/src/shapelets_platform.egg-info/top_level.txt
```

### Comparing `shapelets-platform-2.0.95/LICENSE.md` & `shapelets-platform-2.0.96/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/PKG-INFO` & `shapelets-platform-2.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.95
+Version: 2.0.96
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.95/README.md` & `shapelets-platform-2.0.96/README.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/noxfile.py` & `shapelets-platform-2.0.96/noxfile.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/pyproject.toml` & `shapelets-platform-2.0.96/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/setup.cfg` & `shapelets-platform-2.0.96/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,28 @@
 [options]
 packages = find:
 install_requires = 
 	adlfs ~= 2023.4
 	argparse ~= 1.4
 	blacksheep ~= 1.2
 	dill ~= 0.3
+	email-validator ~= 2.0
 	folium ~= 0.13
 	jmespath ~= 0.9
+	matplotlib ~= 3.7
 	mypy ~= 1.4
 	numpy ~= 1.24
 	pandas ~= 2.0
 	psutil ~= 5.9
 	pyarrow ~= 12.0
 	py-cpuinfo ~= 9.0
 	pydantic ~= 1.10
 	PyNaCl ~= 1.5
 	requests ~= 2.31
-	shapelets_native == 2.0.95
+	shapelets_native == 2.0.96
 	tabulate ~= 0.9
 	tomlkit ~= 0.12
 	typing_extensions ~= 4.7
 	uvicorn ~= 0.23
 	websocket-client ~= 1.5
 	websockets ~= 10.3
 	lockfile ~= 0.12; platform_system!="Windows"
```

### Comparing `shapelets-platform-2.0.95/setup.py` & `shapelets-platform-2.0.96/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/_api.py` & `shapelets-platform-2.0.96/src/shapelets/_api.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/_cli.py` & `shapelets-platform-2.0.96/src/shapelets/_cli.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/_relations.py` & `shapelets-platform-2.0.96/src/shapelets/_relations.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/_uom.py` & `shapelets-platform-2.0.96/src/shapelets/_uom.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/data_app.py` & `shapelets-platform-2.0.96/src/shapelets/apps/data_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from matplotlib.figure import Figure
 from pathlib import Path
 from typing import List, Optional, Union, NamedTuple
 from typing_extensions import Literal
 
 from .widgets.charts.altair_chart import AltairChartWidget
 from .widgets.charts.folium_chart import FoliumChartWidget
-from .widgets.charts.line_chart import LineChartWidget, LineChartValueType
+from .widgets.charts.line_chart import LineChartWidget, LineChartValueType,View
 # from .widgets.charts.plotly_chart import PlotlyChartWidget
-from .widgets.contexts.filtering_context import FilteringContext
-from .widgets.contexts.metadata_field import MetadataField
-from .widgets.contexts.temporal_context import TemporalContext
+# from .widgets.contexts.filtering_context import FilteringContext
+# from .widgets.contexts.metadata_field import MetadataField
+# from .widgets.contexts.temporal_context import TemporalContext
 from .widgets.controllers.button import Button
 from .widgets.controllers.checkbox import CheckboxWidget
 from .widgets.controllers.datetime_range_selector import DatetimeRangeSelectorWidget
 from .widgets.controllers.datetime_selector import DateSelectorWidget
 from .widgets.controllers import GaugeWidget, MetricWidget, RingWidget
 from .widgets.controllers.image import ImageWidget
 # from .widgets.controllers.list import ListWidget
@@ -39,15 +39,14 @@
 from .widgets.layouts.horizontal_layout import HorizontalLayoutWidget
 from .widgets.layouts.panel import PanelWidget
 from .widgets.layouts.tabs_layout import TabsLayoutWidget
 from .widgets.layouts.vertical_layout import VerticalLayoutWidget
 from .widgets.widget import Widget
 
 from .. import DataSet
-from ..model import View
 from ..svr import get_service, IDataAppsService
 
 
 class AttributeNames(Enum):
     CREATION_DATE = "creationDate"
     CUSTOM_GRAPH = "customGraphs"
     DESCRIPTION = "description"
@@ -193,97 +192,97 @@
 
         Examples
         --------
         >>> app.set_title('new title')             
         """
         self.title = title
 
-    def temporal_context(self,
-                         name: str = None,
-                         widgets: List[Widget] = None,
-                         context_id: str = None):
-        """
-        Defines a temporal context for your dataApp.
-
-        Parameters
-        ----------
-        name : str, optional
-            String with the temporal context name.
-
-        widgets : list[Widgets], optional
-            List of Widgets inside the temporal context.
-
-        context_id : str, optional
-            String with the temporal context ID.
-
-
-        Returns
-        -------
-        New Temporal Context.
-
-        Examples
-        --------
-        >>> lc1 = app.line_chart(data)
-        >>> lc2 = app.line_chart(data2)
-        >>> tc = app.temporal_context('Range A',[lc,lc2]) 
-        """
-        widget_ids = []
-        if widgets:
-            for widget in widgets:
-                if hasattr(widget, 'temporal_context'):
-                    widget_ids.append(widget.widget_id)
-                else:
-                    raise Exception(f"Component {widget.widget_type} does not allow temporal context")
-        temporal_context = TemporalContext(name, widget_ids, context_id)
-        self.temporal_contexts.append(temporal_context)
-        return temporal_context
-
-    def filtering_context(self,
-                          name: str = None,
-                          input_filter: List[MetadataField] = None,
-                          context_id: str = None):
-        """
-        Defines a filtering context for your dataApp.
-
-        Parameters
-        ----------
-        name : str, optional
-            String with the filtering context name.
-
-        input_filter : list, optional
-            List of Widgets inside the temporal context.
-
-        context_id : str, optional
-            String with the filtering context ID.
-
-        Returns
-        -------
-        New Filtering Context.
-
-        Examples
-        --------
-        TODO
-        """
-        input_filters_ids = []
-        collection_id = None
-        if input_filter:
-            collection_ids = [mfield.collection.collection_id for mfield in input_filter]
-            collection_ids_set = set(collection_ids)
-            if len(set(collection_ids)) == 1:
-                collection_id = collection_ids_set.pop()
-                for widget in input_filter:
-                    # if hasattr(widget, 'filtering_context'):
-                    input_filters_ids.append(widget.widget_id)
-                    # else:
-                    #     raise Exception(f"Component {widget.widget_type} does not allow filtering context")
-            else:
-                raise Exception("Collection missmatch: All MetadataFields need to come from the same Collection.")
-        filtering_context = FilteringContext(name, collection_id, input_filters_ids, context_id)
-        self.filtering_contexts.append(filtering_context)
-        return filtering_context
+    # def temporal_context(self,
+    #                      name: str = None,
+    #                      widgets: List[Widget] = None,
+    #                      context_id: str = None):
+    #     """
+    #     Defines a temporal context for your dataApp.
+    #
+    #     Parameters
+    #     ----------
+    #     name : str, optional
+    #         String with the temporal context name.
+    #
+    #     widgets : list[Widgets], optional
+    #         List of Widgets inside the temporal context.
+    #
+    #     context_id : str, optional
+    #         String with the temporal context ID.
+    #
+    #
+    #     Returns
+    #     -------
+    #     New Temporal Context.
+    #
+    #     Examples
+    #     --------
+    #     >>> lc1 = app.line_chart(data)
+    #     >>> lc2 = app.line_chart(data2)
+    #     >>> tc = app.temporal_context('Range A',[lc,lc2])
+    #     """
+    #     widget_ids = []
+    #     if widgets:
+    #         for widget in widgets:
+    #             if hasattr(widget, 'temporal_context'):
+    #                 widget_ids.append(widget.widget_id)
+    #             else:
+    #                 raise Exception(f"Component {widget.widget_type} does not allow temporal context")
+    #     temporal_context = TemporalContext(name, widget_ids, context_id)
+    #     self.temporal_contexts.append(temporal_context)
+    #     return temporal_context
+
+    # def filtering_context(self,
+    #                       name: str = None,
+    #                       input_filter: List[MetadataField] = None,
+    #                       context_id: str = None):
+    #     """
+    #     Defines a filtering context for your dataApp.
+    #
+    #     Parameters
+    #     ----------
+    #     name : str, optional
+    #         String with the filtering context name.
+    #
+    #     input_filter : list, optional
+    #         List of Widgets inside the temporal context.
+    #
+    #     context_id : str, optional
+    #         String with the filtering context ID.
+    #
+    #     Returns
+    #     -------
+    #     New Filtering Context.
+    #
+    #     Examples
+    #     --------
+    #     TODO
+    #     """
+    #     input_filters_ids = []
+    #     collection_id = None
+    #     if input_filter:
+    #         collection_ids = [mfield.collection.collection_id for mfield in input_filter]
+    #         collection_ids_set = set(collection_ids)
+    #         if len(set(collection_ids)) == 1:
+    #             collection_id = collection_ids_set.pop()
+    #             for widget in input_filter:
+    #                 # if hasattr(widget, 'filtering_context'):
+    #                 input_filters_ids.append(widget.widget_id)
+    #                 # else:
+    #                 #     raise Exception(f"Component {widget.widget_type} does not allow filtering context")
+    #         else:
+    #             raise Exception("Collection missmatch: All MetadataFields need to come from the same Collection.")
+    #     filtering_context = FilteringContext(name, collection_id, input_filters_ids, context_id)
+    #     self.filtering_contexts.append(filtering_context)
+    #     return filtering_context
 
     def image(self,
               img: Optional[Union[str, bytes, Path, Figure]] = None,
               caption: Optional[str] = None,
               placeholder: Optional[Union[str, bytes, Path]] = None,
               **additional):
         """
@@ -1094,16 +1093,16 @@
         """
         return TabsLayoutWidget(title, parent_data_app=self, **additional)
 
     def line_chart(self,
                    data: Optional[LineChartValueType] = None,
                    title: str = None,
                    views: List[View] = [],
-                   temporal_context: TemporalContext = None,
-                   filtering_context: FilteringContext = None,
+                   # temporal_context: TemporalContext = None,
+                   # filtering_context: FilteringContext = None,
                    multi_line_chart: bool = True,
                    multi_lane: Optional[bool] = True,
                    **additional) -> LineChartWidget:
         """
         Creates a Line Chart figure. It represents either a Sequence or X and Y axis.
 
         Parameters
@@ -1113,20 +1112,14 @@
 
         title : str, optional
             String with the Line Chart title. It will be placed on top of the Line Chart.
 
         views : List[Views], optional
             Views to be represented inside the Line Chart.
 
-        temporal_context : TemporalContext, optional
-            Temporal Context which the Line Chart is attached to.
-
-        filtering_context : FilteringContext, optional
-            Filtering Context which the Line Chart is attached to.
-
         multi_line_chart : bool, optional
             Try to plot multiple lines. (default True)
 
         multi_lane : bool, optional
             Plot one chart per lane. (default True)
 
         Returns
@@ -1184,16 +1177,16 @@
 
         *Currently this widget cannot be used as input in a binding function.*  
         """
         return LineChartWidget(
             data,
             title,
             views,
-            temporal_context,
-            filtering_context,
+            # temporal_context,
+            # filtering_context,
             multi_line_chart,
             multi_lane,
             parent_data_app=self,
             **additional)
 
     # def metadata_field(self,
     #                    field_name: str,
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/data_app_utils.py` & `shapelets-platform-2.0.96/src/shapelets/apps/data_app_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/attribute_names.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/attribute_names.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from .altair_chart import AltairChart, AltairChartWidget
-from .bar_chart import BarChart
+# from .bar_chart import BarChart
 from .folium_chart import FoliumChart, FoliumChartWidget
 # from .plotly_chart import PlotlyChart, PlotlyChartWidget
-from .heatmap import HeatMap
-from .histogram import Histogram
-from .scatter_plot import ScatterPlot
-from .pie_chart import PieChart
-from .polar_area import PolarArea
+# from .heatmap import HeatMap
+# from .histogram import Histogram
+# from .scatter_plot import ScatterPlot
+# from .pie_chart import PieChart
+# from .polar_area import PolarArea
 from .radar_area import RadarArea, RadarAreaWidget
 from .line_chart import LineChart, LineChartValueType, LineChartWidget, View
 
 __all__ = [
     'AltairChart',
-    'BarChart',
+    # 'BarChart',
     'FoliumChart',
     # 'PlotlyChart',
-    'HeatMap',
-    'Histogram',
-    'ScatterPlot',
-    'PieChart',
-    'PolarArea',
+    # 'HeatMap',
+    # 'Histogram',
+    # 'ScatterPlot',
+    # 'PieChart',
+    # 'PolarArea',
     'RadarArea',
     'LineChart',
     'LineChartValueType',
     'View'
 ]
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/altair_chart.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/altair_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/bar_chart.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/polar_area.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-from typing import Union, List
-
-from ..widget import Widget, AttributeNames
-from ....model import NDArray
-
-
-class BarChart(Widget):
-    def __init__(self,
-                 data: Union[List[int], List[float], NDArray],
-                 categories: Union[List[str], List[int], List[float], NDArray] = None,
-                 name: str = None,
-                 title: str = None,
-                 **additional):
-        super().__init__(self.__class__.__name__, name, **additional)
-        if categories:
-            self.categories = categories
-        self.data = data
-        self.title = title
-
-    def to_dict_widget(self):
-        bar_chart_dict = super().to_dict_widget()
-        if hasattr(self, "categories"):
-            categories_value = None
-
-            if isinstance(self.categories, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
-                     self.categories]):
-                categories_value = self.categories
-
-            if isinstance(self.categories, NDArray):
-                categories_value = self.categories.nd_array_id
-
-            bar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.CATEGORIES.value: categories_value
-            })
-
-        if hasattr(self, "data"):
-            data_value = None
-
-            if isinstance(self.data, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) for item in self.data]):
-                data_value = self.data
-
-            if isinstance(self.data, NDArray):
-                data_value = self.data.nd_array_id
-
-            bar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.DATA.value: data_value
-            })
-
-        if self.title is not None:
-            if isinstance(self.title, str):
-                bar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.TITLE.value: self.title
-                })
-
-        return bar_chart_dict
+# from typing import Union, List
+#
+# from ..widget import Widget, AttributeNames
+# from ....model import NDArray
+#
+#
+# class PolarArea(Widget):
+#     def __init__(self,
+#                  categories: Union[List[int], List[float], List[str], NDArray],
+#                  data: Union[List[int], List[float], NDArray],
+#                  name: str = None,
+#                  title: str = None,
+#                  **additional):
+#         super().__init__(self.__class__.__name__,
+#                          name,
+#                          **additional)
+#         self.categories = categories
+#         self.data = data
+#         self.title = title
+#
+#     def to_dict_widget(self):
+#         polar_chart_dict = super().to_dict_widget()
+#         if self.categories is not None:
+#             categories_value = None
+#             if isinstance(self.categories, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
+#                      self.categories]):
+#                 categories_value = self.categories
+#
+#             if isinstance(self.categories, NDArray):
+#                 categories_value = self.categories.nd_array_id
+#
+#             polar_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.CATEGORIES.value: categories_value
+#             })
+#         if self.data:
+#             data_value = None
+#             if isinstance(self.data, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) for item in self.data]):
+#                 data_value = self.data
+#
+#             if isinstance(self.data, NDArray):
+#                 data_value = self.data.nd_array_id
+#
+#             polar_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.DATA.value: data_value
+#             })
+#         if self.title is not None:
+#             if isinstance(self.title, str):
+#                 polar_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                     AttributeNames.TITLE.value: self.title
+#                 })
+#
+#         return polar_chart_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/folium_chart.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/folium_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/heatmap.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/heatmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from typing import Union, List
-
-from ..widget import Widget, AttributeNames
-from ....model import NDArray
-
-
-class HeatMap(Widget):
-    def __init__(self,
-                 x_axis: Union[List[int], List[float], List[str], NDArray],
-                 y_axis: Union[List[int], List[float], List[str], NDArray],
-                 z_axis: Union[List[int], List[float], NDArray],
-                 name: str = None,
-                 title: str = None,
-                 **additional):
-        super().__init__(self.__class__.__name__, name, **additional)
-        self.title = title
-        self.x_axis = x_axis
-        self.y_axis = y_axis
-        self.z_axis = z_axis
-
-    def to_dict_widget(self):
-        heatmap_dict = super().to_dict_widget()
-
-        # title
-        if isinstance(self.title, str):
-            heatmap_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.TITLE.value: self.title
-            })
-
-        def _check_types(axis):
-            print(axis)
-            if all(isinstance(element, type(axis[0])) for element in axis):
-                return axis
-            else:
-                raise Exception("Mixed types not supported")
-
-        # x_axis
-        if isinstance(self.x_axis, List):
-            heatmap_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.X_AXIS.value: _check_types(self.x_axis)
-            })
-
-        if isinstance(self.x_axis, NDArray):
-            heatmap_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.X_AXIS.value: self.x_axis.nd_array_id
-            })
-
-        # y_axis
-        if isinstance(self.y_axis, List):
-            heatmap_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.Y_AXIS.value: _check_types(self.y_axis)
-            })
-
-        if isinstance(self.y_axis, NDArray):
-            heatmap_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.Y_AXIS.value: self.y_axis.nd_array_id
-            })
-
-        # z_axis
-        if isinstance(self.z_axis, List):
-            heatmap_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.Z_AXIS.value: _check_types(self.z_axis)
-            })
-
-        if isinstance(self.z_axis, NDArray):
-            heatmap_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.Z_AXIS.value: self.z_axis.nd_array_id
-            })
-
-        return heatmap_dict
+# from typing import Union, List
+#
+# from ..widget import Widget, AttributeNames
+# from ....model import NDArray
+#
+#
+# class HeatMap(Widget):
+#     def __init__(self,
+#                  x_axis: Union[List[int], List[float], List[str], NDArray],
+#                  y_axis: Union[List[int], List[float], List[str], NDArray],
+#                  z_axis: Union[List[int], List[float], NDArray],
+#                  name: str = None,
+#                  title: str = None,
+#                  **additional):
+#         super().__init__(self.__class__.__name__, name, **additional)
+#         self.title = title
+#         self.x_axis = x_axis
+#         self.y_axis = y_axis
+#         self.z_axis = z_axis
+#
+#     def to_dict_widget(self):
+#         heatmap_dict = super().to_dict_widget()
+#
+#         # title
+#         if isinstance(self.title, str):
+#             heatmap_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.TITLE.value: self.title
+#             })
+#
+#         def _check_types(axis):
+#             print(axis)
+#             if all(isinstance(element, type(axis[0])) for element in axis):
+#                 return axis
+#             else:
+#                 raise Exception("Mixed types not supported")
+#
+#         # x_axis
+#         if isinstance(self.x_axis, List):
+#             heatmap_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.X_AXIS.value: _check_types(self.x_axis)
+#             })
+#
+#         if isinstance(self.x_axis, NDArray):
+#             heatmap_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.X_AXIS.value: self.x_axis.nd_array_id
+#             })
+#
+#         # y_axis
+#         if isinstance(self.y_axis, List):
+#             heatmap_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.Y_AXIS.value: _check_types(self.y_axis)
+#             })
+#
+#         if isinstance(self.y_axis, NDArray):
+#             heatmap_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.Y_AXIS.value: self.y_axis.nd_array_id
+#             })
+#
+#         # z_axis
+#         if isinstance(self.z_axis, List):
+#             heatmap_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.Z_AXIS.value: _check_types(self.z_axis)
+#             })
+#
+#         if isinstance(self.z_axis, NDArray):
+#             heatmap_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.Z_AXIS.value: self.z_axis.nd_array_id
+#             })
+#
+#         return heatmap_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/histogram.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/histogram.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Union, List
-
-from ..widget import Widget, AttributeNames
-from ....model import NDArray
-
-
-class Histogram(Widget):
-    def __init__(self, x: Union[List[int], List[float], NDArray],
-                 bins: Union[int, float] = None,
-                 cumulative: bool = False, **additional):
-        super().__init__(self.__class__.__name__, "Histogram", **additional)
-        self._x = x
-        self._bins = bins
-        self._cumulative = cumulative
-
-    def to_dict_widget(self):
-        histogram_dict = super().to_dict_widget()
-
-        if isinstance(self._x, List) and all([isinstance(item, int) or isinstance(item, float) for item in self._x]):
-            histogram_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.X.value: self._x
-            })
-        if isinstance(self._x, NDArray):
-            histogram_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.X.value: self._x.nd_array_id
-            })
-
-        if self._bins is not None:
-            if isinstance(self._bins, int) or isinstance(self._bins, float):
-                histogram_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.BINS.value: self._bins
-                })
-            if isinstance(self._bins, float) or isinstance(self._bins, float):
-                histogram_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.BINS.value: self._bins
-                })
-
-        if isinstance(self._cumulative, bool):
-            histogram_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.CUMULATIVE.value: self._cumulative
-            })
-
-        return histogram_dict
+# from typing import Union, List
+#
+# from ..widget import Widget, AttributeNames
+# from ....model import NDArray
+#
+#
+# class Histogram(Widget):
+#     def __init__(self, x: Union[List[int], List[float], NDArray],
+#                  bins: Union[int, float] = None,
+#                  cumulative: bool = False, **additional):
+#         super().__init__(self.__class__.__name__, "Histogram", **additional)
+#         self._x = x
+#         self._bins = bins
+#         self._cumulative = cumulative
+#
+#     def to_dict_widget(self):
+#         histogram_dict = super().to_dict_widget()
+#
+#         if isinstance(self._x, List) and all([isinstance(item, int) or isinstance(item, float) for item in self._x]):
+#             histogram_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.X.value: self._x
+#             })
+#         if isinstance(self._x, NDArray):
+#             histogram_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.X.value: self._x.nd_array_id
+#             })
+#
+#         if self._bins is not None:
+#             if isinstance(self._bins, int) or isinstance(self._bins, float):
+#                 histogram_dict[AttributeNames.PROPERTIES.value].update({
+#                     AttributeNames.BINS.value: self._bins
+#                 })
+#             if isinstance(self._bins, float) or isinstance(self._bins, float):
+#                 histogram_dict[AttributeNames.PROPERTIES.value].update({
+#                     AttributeNames.BINS.value: self._bins
+#                 })
+#
+#         if isinstance(self._cumulative, bool):
+#             histogram_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.CUMULATIVE.value: self._cumulative
+#             })
+#
+#         return histogram_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/line_chart.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/line_chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 
 from dataclasses import dataclass, field
 from datetime import date, datetime
 
 from typing import List, Optional, Tuple, Union
 
 from ..widget import AttributeNames, StateControl, Widget
-from ..contexts import FilteringContext, TemporalContext
+# from ..contexts import FilteringContext, TemporalContext
 from ..util import _to_utf64_arrow_buffer
-from ....model import Sequence
 from .... import DataSet
 
 
 @dataclass
 class View:
     """
     Highlight a section of a Linechart.
@@ -153,33 +152,30 @@
 
     *Currently this widget cannot be used as input in a binding function.*                
     """
 
     data: Optional[LineChartValueType] = None
     title: Optional[str] = None
     views: Optional[List[View]] = field(default_factory=lambda: [])
-    temporal_context: Optional[TemporalContext] = None
-    filtering_context: Optional[FilteringContext] = None
+    # temporal_context: Optional[TemporalContext] = None
+    # filtering_context: Optional[FilteringContext] = None
     multi_line_chart: Optional[bool] = True
     multi_lane: Optional[bool] = True
     _plots: List = field(default_factory=lambda: [])
     _is_type = None
 
     def __post_init__(self):
         if not hasattr(self, "widget_id"):
             self.widget_id = str(uuid.uuid1())
         # A subtype to differentiate between sequences or y_axis/x_axis. Requested by UI.
         self.linechart_sub_type = None
         self.sequence = None
         self.y_axis = None
         self.x_axis = None
-        if isinstance(self.data, Sequence):
-            self.linechart_sub_type = f"{AttributeNames.SEQUENCE.value.capitalize()}"
-            self.sequence = self.data
-        elif isinstance(self.data, List):
+        if isinstance(self.data, List):
             self.linechart_sub_type = f"{AttributeNames.NUMPY_ARRAY.value.capitalize()}"
             self.y_axis = self.data
         elif isinstance(self.data, np.ndarray):
             self.linechart_sub_type = f"{AttributeNames.NUMPY_ARRAY.value.capitalize()}"
             self.y_axis = self.data
         elif isinstance(self.data, pd.Series):
             self.linechart_sub_type = f"Arrow"
@@ -254,28 +250,14 @@
         """
         Return the current value of the widget. Return None is the widget value is not set.
         """
         if self.data is not None:
             return self.data
         return None
 
-    # TODO Adjust LineChart Type
-    def from_sequences(self, sequences: List[Sequence]) -> LineChart:
-        self.linechart_sub_type = f"{AttributeNames.SEQUENCE.value.capitalize()}"
-        self.data = sequences
-        return self
-
-    def from_sequence(self, sequence: Sequence) -> LineChart:
-        self.linechart_sub_type = f"{AttributeNames.SEQUENCE.value.capitalize()}"
-        self.data = sequence
-        return self
-
-    def to_sequence(self) -> Sequence:
-        return self.sequence
-
     def from_views(self, views: List[View]) -> LineChart:
         self.views = views
         return self
 
     def from_view(self, view: View) -> LineChart:
         self.views.append(view)
         return self
@@ -317,56 +299,56 @@
 
     def to_list(self) -> pd.DataFrame:
         return self.y_axis
 
     def plot(self,
              y_axis: Union[List[int], List[float], np.ndarray, pd.Series] = None,
              x_axis: Union[List[int], List[float], List[str], np.ndarray] = None,
-             sequence: Union[List[Sequence], Sequence] = None,
+             # sequence: Union[List[Sequence], Sequence] = None,
              label: str = None,
              lane_index: int = 0):
         # TODO: I want to complety modify or remove this function. Doesn't make sense to have a function with some many
         # isInstances once we are already checking that in previous functions.
         plot_dict = {}
 
         plot_dict.update({AttributeNames.LANE_INDEX.value: lane_index})
 
-        if sequence is not None:
-            # Adjust subtype for UI
-            self.linechart_sub_type = f"{AttributeNames.SEQUENCE.value.capitalize()}"
+        # if sequence is not None:
+        #     # Adjust subtype for UI
+        #     self.linechart_sub_type = f"{AttributeNames.SEQUENCE.value.capitalize()}"
             # list of sequences
-            if isinstance(sequence, List) and all([isinstance(seq, Sequence) for seq in sequence]):
-                for seq in sequence:
-                    if isinstance(seq, Sequence):
-                        plot_dict_array = dict()
-                        plot_dict_array.update({
-                            AttributeNames.LANE_INDEX.value: lane_index,
-                            AttributeNames.SEQUENCE_ID.value: seq.sequence_id
-                        })
-                        self._plots.append(plot_dict_array)
-                    else:
-                        raise ValueError(f"Unexpected type {type(seq)}")
+            # if isinstance(sequence, List) and all([isinstance(seq, Sequence) for seq in sequence]):
+            #     for seq in sequence:
+            #         if isinstance(seq, Sequence):
+            #             plot_dict_array = dict()
+            #             plot_dict_array.update({
+            #                 AttributeNames.LANE_INDEX.value: lane_index,
+            #                 AttributeNames.SEQUENCE_ID.value: seq.sequence_id
+            #             })
+            #             self._plots.append(plot_dict_array)
+            #         else:
+            #             raise ValueError(f"Unexpected type {type(seq)}")
                     # elif isinstance(seq, SequenceSelector):
                     #     seq_node = dict()
                     #     seq_node.update({
                     #         AttributeNames.LANE_INDEX.value: lane_index,
                     #         AttributeNames.WIDGET_REF.value: seq.widget_id
                     #     })
                     #     self._plots.append(seq_node)
 
             # if isinstance(sequence, SequenceSelector) or isinstance(sequence, CollectionSelector):
             #     if self.sequence:
             #         self._plots.append({AttributeNames.WIDGET_REF.value: sequence.widget_id})
 
             # a single sequence
-            if isinstance(sequence, Sequence):
-                plot_dict.update({
-                    AttributeNames.SEQUENCE_ID.value: sequence.sequence_id
-                })
-                self._plots.append(plot_dict)
+            # if isinstance(sequence, Sequence):
+            #     plot_dict.update({
+            #         AttributeNames.SEQUENCE_ID.value: sequence.sequence_id
+            #     })
+            #     self._plots.append(plot_dict)
 
         # Handle arrays: y-axis
         # TODO: save array and send ID
         if y_axis is not None:
             self.linechart_sub_type = f"{AttributeNames.NUMPY_ARRAY.value.capitalize()}"
             if isinstance(y_axis, np.ndarray):
                 plot_dict.update({AttributeNames.Y_AXIS.value: y_axis.tolist()})
@@ -382,22 +364,22 @@
                 plot_dict.update({AttributeNames.X_AXIS.value: x_axis.tolist()})
             elif isinstance(x_axis, List):
                 plot_dict.update({AttributeNames.X_AXIS.value: x_axis})
             elif isinstance(x_axis, pd.Series):
                 plot_dict.update({AttributeNames.X_AXIS.value: x_axis.values.tolist()})
 
         if label is not None:
-            if sequence:
-                plot_dict.update({AttributeNames.LABEL.value: sequence})
+            # if sequence:
+            #     plot_dict.update({AttributeNames.LABEL.value: sequence})
             if isinstance(label, str):
                 plot_dict.update({
                     AttributeNames.LABEL.value: label
                 })
-        if self.sequence is None:
-            self._plots.append(plot_dict)
+        # if self.sequence is None:
+        self._plots.append(plot_dict)
 
     def to_dict_widget(self, line_chart_dict: dict = None):
         if line_chart_dict is None:
             line_chart_dict = {
                 AttributeNames.ID.value: self.widget_id,
                 AttributeNames.TYPE.value: LineChart.__name__,
                 AttributeNames.DRAGGABLE.value: self.draggable,
@@ -463,48 +445,48 @@
 
 
 class LineChartWidget(Widget, LineChart):
     def __init__(self,
                  data: Optional[LineChartValueType] = None,
                  title: Optional[str] = None,
                  views: Optional[List[View]] = [],
-                 temporal_context: Optional[TemporalContext] = None,
-                 filtering_context: Optional[FilteringContext] = None,
+                 # temporal_context: Optional[TemporalContext] = None,
+                 # filtering_context: Optional[FilteringContext] = None,
                  multi_line_chart: Optional[bool] = True,
                  multi_lane: Optional[bool] = True,
                  **additional):
 
         # define TYPE
         widget_type = LineChart.__name__
         Widget.__init__(self, widget_type,
                         compatibility=tuple(
-                            [str.__name__, int.__name__, float.__name__, LineChart.__name__, Sequence.__name__,
+                            [str.__name__, int.__name__, float.__name__, LineChart.__name__,
                              View.__name__, "List[View]", "List[Sequence]", pd.DataFrame.__name__,
                              list.__name__, np.ndarray.__name__, pd.Series.__name__]),
                         **additional)
         LineChart.__init__(
             self,
             data=data,
             title=title,
             views=views,
-            temporal_context=temporal_context,
-            filtering_context=filtering_context,
+            # temporal_context=temporal_context,
+            # filtering_context=filtering_context,
             multi_line_chart=multi_line_chart,
             multi_lane=multi_lane
         )
         self._parent_class = LineChart.__name__
 
-        temporal_context_id = None
-        if self.temporal_context:
-            temporal_context_id = self.temporal_context.context_id
-            self.temporal_context.widgets.append(self.widget_id)
-        filtering_context_id = None
-        if self.filtering_context:
-            filtering_context_id = filtering_context.context_id
-            filtering_context.output_widgets.append(self.widget_id)
-        self.temporal_context = temporal_context_id
-        self.filtering_context = filtering_context_id
+        # temporal_context_id = None
+        # if self.temporal_context:
+        #     temporal_context_id = self.temporal_context.context_id
+        #     self.temporal_context.widgets.append(self.widget_id)
+        # filtering_context_id = None
+        # if self.filtering_context:
+        #     filtering_context_id = filtering_context.context_id
+        #     filtering_context.output_widgets.append(self.widget_id)
+        # self.temporal_context = temporal_context_id
+        # self.filtering_context = filtering_context_id
 
     def to_dict_widget(self):
         line_chart_dict = Widget.to_dict_widget(self)
         line_chart_dict = LineChart.to_dict_widget(self, line_chart_dict)
         return line_chart_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/pie_chart.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/radar_area.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,75 @@
 from typing import Union, List
+from dataclasses import dataclass
 
-from ..widget import Widget, AttributeNames
-from ....model import NDArray
+from ..widget import Widget, AttributeNames, StateControl
 
 
-class PieChart(Widget):
+@dataclass
+class RadarArea(StateControl):
+    categories: Union[List[int], List[float], List[str]] = None
+    data: Union[List[int], List[float]] = None
+    groups: Union[List[int], List[float], List[str]] = None
+    name: str = None
+    title: str = None
+
+
+class RadarAreaWidget(Widget, RadarArea):
     def __init__(self,
-                 data: Union[List[int], List[float], NDArray],
-                 categories: Union[List[int], List[float], List[str], NDArray] = None,
+                 categories: Union[List[int], List[float], List[str]],
+                 data: Union[List[int], List[float]],
+                 groups: Union[List[int], List[float], List[str]],
                  name: str = None,
                  title: str = None,
                  **additional):
-        super().__init__(self.__class__.__name__, name, **additional)
-        if categories:
-            self.categories = categories
+
+        Widget.__init__(self, 'RadarArea', **additional)
+        RadarArea.__init__(self, categories, data, groups, name, title)
+
+        self.categories = categories
         self.data = data
+        self.groups = groups
         self.title = title
 
     def to_dict_widget(self):
-        pie_chart_dict = super().to_dict_widget()
-        if hasattr(self, "categories"):
+        radar_chart_dict = super().to_dict_widget()
+        if self.categories is not None:
             categories_value = None
-
             if isinstance(self.categories, List) and all(
                     [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
                      self.categories]):
                 categories_value = self.categories
+            # if isinstance(self.categories, NDArray):
+            #     categories_value = self.categories.nd_array_id
 
-            if isinstance(self.categories, NDArray):
-                categories_value = self.categories.nd_array_id
-
-            pie_chart_dict[AttributeNames.PROPERTIES.value].update({
+            radar_chart_dict[AttributeNames.PROPERTIES.value].update({
                 AttributeNames.CATEGORIES.value: categories_value
             })
-
-        if hasattr(self, "data"):
+        if self.data:
             data_value = None
-
-            if isinstance(self.data, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) for item in self.data]):
+            if isinstance(self.data, List) and all([isinstance(item, (int, float)) for item in self.data]):
                 data_value = self.data
+            # if isinstance(self.data, NDArray):
+            #     data_value = self.data.nd_array_id
 
-            if isinstance(self.data, NDArray):
-                data_value = self.data.nd_array_id
-
-            pie_chart_dict[AttributeNames.PROPERTIES.value].update({
+            radar_chart_dict[AttributeNames.PROPERTIES.value].update({
                 AttributeNames.DATA.value: data_value
             })
+        if self.groups:
+            groups_value = None
+            if isinstance(self.groups, List) and all(
+                    [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
+                     self.groups]):
+                groups_value = self.groups
+            # if isinstance(self.groups, NDArray):
+            #     groups_value = self.groups.nd_array_id
 
+            radar_chart_dict[AttributeNames.PROPERTIES.value].update({
+                AttributeNames.GROUPS.value: groups_value
+            })
         if self.title is not None:
             if isinstance(self.title, str):
-                pie_chart_dict[AttributeNames.PROPERTIES.value].update({
+                radar_chart_dict[AttributeNames.PROPERTIES.value].update({
                     AttributeNames.TITLE.value: self.title
                 })
 
-        return pie_chart_dict
+        return radar_chart_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/plotly_chart.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/polar_area.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/bar_chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-from typing import Union, List
-
-from ..widget import Widget, AttributeNames
-from ....model import NDArray
-
-
-class PolarArea(Widget):
-    def __init__(self,
-                 categories: Union[List[int], List[float], List[str], NDArray],
-                 data: Union[List[int], List[float], NDArray],
-                 name: str = None,
-                 title: str = None,
-                 **additional):
-        super().__init__(self.__class__.__name__,
-                         name,
-                         **additional)
-        self.categories = categories
-        self.data = data
-        self.title = title
-
-    def to_dict_widget(self):
-        polar_chart_dict = super().to_dict_widget()
-        if self.categories is not None:
-            categories_value = None
-            if isinstance(self.categories, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
-                     self.categories]):
-                categories_value = self.categories
-
-            if isinstance(self.categories, NDArray):
-                categories_value = self.categories.nd_array_id
-
-            polar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.CATEGORIES.value: categories_value
-            })
-        if self.data:
-            data_value = None
-            if isinstance(self.data, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) for item in self.data]):
-                data_value = self.data
-
-            if isinstance(self.data, NDArray):
-                data_value = self.data.nd_array_id
-
-            polar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.DATA.value: data_value
-            })
-        if self.title is not None:
-            if isinstance(self.title, str):
-                polar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.TITLE.value: self.title
-                })
-
-        return polar_chart_dict
+# from typing import Union, List
+#
+# from ..widget import Widget, AttributeNames
+# from ....model import NDArray
+#
+#
+# class BarChart(Widget):
+#     def __init__(self,
+#                  data: Union[List[int], List[float], NDArray],
+#                  categories: Union[List[str], List[int], List[float], NDArray] = None,
+#                  name: str = None,
+#                  title: str = None,
+#                  **additional):
+#         super().__init__(self.__class__.__name__, name, **additional)
+#         if categories:
+#             self.categories = categories
+#         self.data = data
+#         self.title = title
+#
+#     def to_dict_widget(self):
+#         bar_chart_dict = super().to_dict_widget()
+#         if hasattr(self, "categories"):
+#             categories_value = None
+#
+#             if isinstance(self.categories, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
+#                      self.categories]):
+#                 categories_value = self.categories
+#
+#             if isinstance(self.categories, NDArray):
+#                 categories_value = self.categories.nd_array_id
+#
+#             bar_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.CATEGORIES.value: categories_value
+#             })
+#
+#         if hasattr(self, "data"):
+#             data_value = None
+#
+#             if isinstance(self.data, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) for item in self.data]):
+#                 data_value = self.data
+#
+#             if isinstance(self.data, NDArray):
+#                 data_value = self.data.nd_array_id
+#
+#             bar_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.DATA.value: data_value
+#             })
+#
+#         if self.title is not None:
+#             if isinstance(self.title, str):
+#                 bar_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                     AttributeNames.TITLE.value: self.title
+#                 })
+#
+#         return bar_chart_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/radar_area.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/pie_chart.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,57 @@
-from typing import Union, List
-from dataclasses import dataclass
-
-from ..widget import Widget, AttributeNames, StateControl
-
-
-@dataclass
-class RadarArea(StateControl):
-    categories: Union[List[int], List[float], List[str]] = None
-    data: Union[List[int], List[float]] = None
-    groups: Union[List[int], List[float], List[str]] = None
-    name: str = None
-    title: str = None
-
-
-class RadarAreaWidget(Widget, RadarArea):
-    def __init__(self,
-                 categories: Union[List[int], List[float], List[str]],
-                 data: Union[List[int], List[float]],
-                 groups: Union[List[int], List[float], List[str]],
-                 name: str = None,
-                 title: str = None,
-                 **additional):
-
-        Widget.__init__(self, 'RadarArea', **additional)
-        RadarArea.__init__(self, categories, data, groups, name, title)
-
-        self.categories = categories
-        self.data = data
-        self.groups = groups
-        self.title = title
-
-    def to_dict_widget(self):
-        radar_chart_dict = super().to_dict_widget()
-        if self.categories is not None:
-            categories_value = None
-            if isinstance(self.categories, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
-                     self.categories]):
-                categories_value = self.categories
-            # if isinstance(self.categories, NDArray):
-            #     categories_value = self.categories.nd_array_id
-
-            radar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.CATEGORIES.value: categories_value
-            })
-        if self.data:
-            data_value = None
-            if isinstance(self.data, List) and all([isinstance(item, (int, float)) for item in self.data]):
-                data_value = self.data
-            # if isinstance(self.data, NDArray):
-            #     data_value = self.data.nd_array_id
-
-            radar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.DATA.value: data_value
-            })
-        if self.groups:
-            groups_value = None
-            if isinstance(self.groups, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
-                     self.groups]):
-                groups_value = self.groups
-            # if isinstance(self.groups, NDArray):
-            #     groups_value = self.groups.nd_array_id
-
-            radar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.GROUPS.value: groups_value
-            })
-        if self.title is not None:
-            if isinstance(self.title, str):
-                radar_chart_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.TITLE.value: self.title
-                })
-
-        return radar_chart_dict
+# from typing import Union, List
+#
+# from ..widget import Widget, AttributeNames
+# from ....model import NDArray
+#
+#
+# class PieChart(Widget):
+#     def __init__(self,
+#                  data: Union[List[int], List[float], NDArray],
+#                  categories: Union[List[int], List[float], List[str], NDArray] = None,
+#                  name: str = None,
+#                  title: str = None,
+#                  **additional):
+#         super().__init__(self.__class__.__name__, name, **additional)
+#         if categories:
+#             self.categories = categories
+#         self.data = data
+#         self.title = title
+#
+#     def to_dict_widget(self):
+#         pie_chart_dict = super().to_dict_widget()
+#         if hasattr(self, "categories"):
+#             categories_value = None
+#
+#             if isinstance(self.categories, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
+#                      self.categories]):
+#                 categories_value = self.categories
+#
+#             if isinstance(self.categories, NDArray):
+#                 categories_value = self.categories.nd_array_id
+#
+#             pie_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.CATEGORIES.value: categories_value
+#             })
+#
+#         if hasattr(self, "data"):
+#             data_value = None
+#
+#             if isinstance(self.data, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) for item in self.data]):
+#                 data_value = self.data
+#
+#             if isinstance(self.data, NDArray):
+#                 data_value = self.data.nd_array_id
+#
+#             pie_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.DATA.value: data_value
+#             })
+#
+#         if self.title is not None:
+#             if isinstance(self.title, str):
+#                 pie_chart_dict[AttributeNames.PROPERTIES.value].update({
+#                     AttributeNames.TITLE.value: self.title
+#                 })
+#
+#         return pie_chart_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/scatter_plot.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/charts/scatter_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-from typing import Union, List
-from ..widget import Widget, AttributeNames
-from ....model import NDArray
-
-
-class ScatterPlot(Widget):
-    def __init__(self,
-                 x_axis: Union[List[int], List[float], NDArray],
-                 y_axis: Union[List[int], List[float], NDArray],
-                 size: Union[List[int], List[float], NDArray] = None,
-                 color: Union[List[int], List[float], NDArray] = None,
-                 categories: Union[List[int], List[float], List[str], NDArray] = None,
-                 name: str = None,
-                 title: str = None,
-                 trend_line: bool = False,
-                 **additional):
-        super().__init__(self.__class__.__name__, name, **additional)
-        if size:
-            self.size = size
-        if color:
-            self.color = color
-        if categories:
-            self.categories = categories
-        self.x_axis = x_axis
-        self.y_axis = y_axis
-        self.title = title
-        self.trend_line = trend_line
-
-    def to_dict_widget(self):
-        scatter_plot_dict = super().to_dict_widget()
-        if hasattr(self, "size"):
-            size_value = None
-
-            if isinstance(self.size, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) for item in self.size]):
-                size_value = self.size
-
-            if isinstance(self.size, NDArray):
-                size_value = self.size.nd_array_id
-
-            scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.SIZE.value: size_value
-            })
-        if hasattr(self, "color"):
-            color_value = None
-
-            if isinstance(self.color, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) for item in self.color]):
-                color_value = self.color
-
-            if isinstance(self.color, NDArray):
-                color_value = self.color.nd_array_id
-
-            scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.COLOR.value: color_value
-            })
-
-        if hasattr(self, "categories"):
-            categories_value = None
-
-            if isinstance(self.categories, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
-                     self.categories]):
-                categories_value = self.categories
-
-            if isinstance(self.categories, NDArray):
-                categories_value = self.categories.nd_array_id
-
-            scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.CATEGORIES.value: categories_value
-            })
-
-        if self.title is not None:
-            if isinstance(self.title, str):
-                scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.TITLE.value: self.title
-                })
-
-        if hasattr(self, "x_axis"):
-            x_axis_value = None
-
-            if isinstance(self.x_axis, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) for item in self.x_axis]):
-                x_axis_value = self.x_axis
-
-            if isinstance(self.x_axis, NDArray):
-                x_axis_value = self.x_axis.nd_array_id
-
-            scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.X_AXIS.value: x_axis_value
-            })
-
-        if hasattr(self, "y_axis"):
-            y_axis_value = None
-
-            if isinstance(self.y_axis, List) and all(
-                    [isinstance(item, int) or isinstance(item, float) for item in self.y_axis]):
-                y_axis_value = self.y_axis
-
-            if isinstance(self.y_axis, NDArray):
-                y_axis_value = self.y_axis.nd_array_id
-
-            scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.Y_AXIS.value: y_axis_value
-            })
-
-        if hasattr(self, "trend_line"):
-            scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.TREND_LINE.value: self.trend_line
-            })
-        return scatter_plot_dict
+# from typing import Union, List
+# from ..widget import Widget, AttributeNames
+# from ....model import NDArray
+#
+#
+# class ScatterPlot(Widget):
+#     def __init__(self,
+#                  x_axis: Union[List[int], List[float], NDArray],
+#                  y_axis: Union[List[int], List[float], NDArray],
+#                  size: Union[List[int], List[float], NDArray] = None,
+#                  color: Union[List[int], List[float], NDArray] = None,
+#                  categories: Union[List[int], List[float], List[str], NDArray] = None,
+#                  name: str = None,
+#                  title: str = None,
+#                  trend_line: bool = False,
+#                  **additional):
+#         super().__init__(self.__class__.__name__, name, **additional)
+#         if size:
+#             self.size = size
+#         if color:
+#             self.color = color
+#         if categories:
+#             self.categories = categories
+#         self.x_axis = x_axis
+#         self.y_axis = y_axis
+#         self.title = title
+#         self.trend_line = trend_line
+#
+#     def to_dict_widget(self):
+#         scatter_plot_dict = super().to_dict_widget()
+#         if hasattr(self, "size"):
+#             size_value = None
+#
+#             if isinstance(self.size, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) for item in self.size]):
+#                 size_value = self.size
+#
+#             if isinstance(self.size, NDArray):
+#                 size_value = self.size.nd_array_id
+#
+#             scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.SIZE.value: size_value
+#             })
+#         if hasattr(self, "color"):
+#             color_value = None
+#
+#             if isinstance(self.color, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) for item in self.color]):
+#                 color_value = self.color
+#
+#             if isinstance(self.color, NDArray):
+#                 color_value = self.color.nd_array_id
+#
+#             scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.COLOR.value: color_value
+#             })
+#
+#         if hasattr(self, "categories"):
+#             categories_value = None
+#
+#             if isinstance(self.categories, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) or isinstance(item, str) for item in
+#                      self.categories]):
+#                 categories_value = self.categories
+#
+#             if isinstance(self.categories, NDArray):
+#                 categories_value = self.categories.nd_array_id
+#
+#             scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.CATEGORIES.value: categories_value
+#             })
+#
+#         if self.title is not None:
+#             if isinstance(self.title, str):
+#                 scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
+#                     AttributeNames.TITLE.value: self.title
+#                 })
+#
+#         if hasattr(self, "x_axis"):
+#             x_axis_value = None
+#
+#             if isinstance(self.x_axis, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) for item in self.x_axis]):
+#                 x_axis_value = self.x_axis
+#
+#             if isinstance(self.x_axis, NDArray):
+#                 x_axis_value = self.x_axis.nd_array_id
+#
+#             scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.X_AXIS.value: x_axis_value
+#             })
+#
+#         if hasattr(self, "y_axis"):
+#             y_axis_value = None
+#
+#             if isinstance(self.y_axis, List) and all(
+#                     [isinstance(item, int) or isinstance(item, float) for item in self.y_axis]):
+#                 y_axis_value = self.y_axis
+#
+#             if isinstance(self.y_axis, NDArray):
+#                 y_axis_value = self.y_axis.nd_array_id
+#
+#             scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.Y_AXIS.value: y_axis_value
+#             })
+#
+#         if hasattr(self, "trend_line"):
+#             scatter_plot_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.TREND_LINE.value: self.trend_line
+#             })
+#         return scatter_plot_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/filtering_context.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/filtering_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_field.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/metadata_field.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from ....model import MetadataType, Collection
-from ..widget import Widget, AttributeNames
-
-
-class MetadataField(Widget):
-    def __init__(self,
-                 field_name: str,
-                 field_type: MetadataType,
-                 collection: Collection,
-                 name: str = None,
-                 **additional):
-        super().__init__(widget_type=self.__class__.__name__,
-                         widget_name=name,
-                         **additional)
-        self.field_type = field_type
-        self.collection = collection
-        self.field_name = field_name
-
-    def to_dict_widget(self):
-        metadata_field_dict = super().to_dict_widget()
-        metadata_field_dict[AttributeNames.PROPERTIES.value].update({
-            AttributeNames.COLLECTION_ID.value: self.collection.collection_id,
-            AttributeNames.NAME.value: self.field_name,
-            AttributeNames.TYPE.value: self.frontend_type
-        })
-        return metadata_field_dict
-
-    @property
-    def frontend_type(self):
-        value = self.field_type.value
-        return value[0] + value[1:].lower()
+# from ....model import MetadataType, Collection
+# from ..widget import Widget, AttributeNames
+#
+#
+# class MetadataField(Widget):
+#     def __init__(self,
+#                  field_name: str,
+#                  field_type: MetadataType,
+#                  collection: Collection,
+#                  name: str = None,
+#                  **additional):
+#         super().__init__(widget_type=self.__class__.__name__,
+#                          widget_name=name,
+#                          **additional)
+#         self.field_type = field_type
+#         self.collection = collection
+#         self.field_name = field_name
+#
+#     def to_dict_widget(self):
+#         metadata_field_dict = super().to_dict_widget()
+#         metadata_field_dict[AttributeNames.PROPERTIES.value].update({
+#             AttributeNames.COLLECTION_ID.value: self.collection.collection_id,
+#             AttributeNames.NAME.value: self.field_name,
+#             AttributeNames.TYPE.value: self.frontend_type
+#         })
+#         return metadata_field_dict
+#
+#     @property
+#     def frontend_type(self):
+#         value = self.field_type.value
+#         return value[0] + value[1:].lower()
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_filter.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/metadata_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from typing import List
-
-from ..widget import Widget, AttributeNames
-from .filtering_context import FilteringContext
-from .metadata_field import MetadataField
-
-
-class MetadataFilter(Widget):
-    def __init__(self,
-                 metadata_elements: List[MetadataField],
-                 name: str = None,
-                 title: str = None,
-                 filtering_context: List[FilteringContext] = None,
-                 **additional):
-        super().__init__(widget_type=self.__class__.__name__,
-                         widget_name=name,
-                         **additional)
-        metadata_fields = []
-        for metadata in metadata_elements:
-            metadata_fields.append([metadata.field_name, metadata.frontend_type])
-        self.metadata_fields = metadata_fields
-        self.title = title
-        filtering_context_id = []
-        if filtering_context:
-            for filtering in filtering_context:
-                filtering_context_id.append(filtering.context_id)
-                filtering.input_filters.append(self.widget_id)
-        self.filtering_context = filtering_context_id
-
-    def to_dict_widget(self):
-        metadata_filter_dict = super().to_dict_widget()
-        metadata_filter_dict[AttributeNames.PROPERTIES.value].update({
-            AttributeNames.METADATA_FIELDS.value: self.metadata_fields,
-            AttributeNames.TITLE.value: self.title,
-        })
-        return metadata_filter_dict
+# from typing import List
+#
+# from ..widget import Widget, AttributeNames
+# from .filtering_context import FilteringContext
+# from .metadata_field import MetadataField
+#
+#
+# class MetadataFilter(Widget):
+#     def __init__(self,
+#                  metadata_elements: List[MetadataField],
+#                  name: str = None,
+#                  title: str = None,
+#                  filtering_context: List[FilteringContext] = None,
+#                  **additional):
+#         super().__init__(widget_type=self.__class__.__name__,
+#                          widget_name=name,
+#                          **additional)
+#         metadata_fields = []
+#         for metadata in metadata_elements:
+#             metadata_fields.append([metadata.field_name, metadata.frontend_type])
+#         self.metadata_fields = metadata_fields
+#         self.title = title
+#         filtering_context_id = []
+#         if filtering_context:
+#             for filtering in filtering_context:
+#                 filtering_context_id.append(filtering.context_id)
+#                 filtering.input_filters.append(self.widget_id)
+#         self.filtering_context = filtering_context_id
+#
+#     def to_dict_widget(self):
+#         metadata_filter_dict = super().to_dict_widget()
+#         metadata_filter_dict[AttributeNames.PROPERTIES.value].update({
+#             AttributeNames.METADATA_FIELDS.value: self.metadata_fields,
+#             AttributeNames.TITLE.value: self.title,
+#         })
+#         return metadata_filter_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/temporal_context.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/contexts/temporal_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/button.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/button.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/checkbox.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/checkbox.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/collection_selector.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/collection_selector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-
-from ...widgets import AttributeNames, Widget
-from ....model import Collection, Sequence
-
-
-class CollectionSelector(Widget):
-    def __init__(self,
-                 default_collection: Collection = None,
-                 default_sequence: Sequence = None,
-                 name: str = None,
-                 title: str = None,
-                 collection_label: str = None,
-                 sequence_label: str = None,
-                 **additional):
-        super().__init__(self.__class__.__name__,
-                         name,
-                         ArgumentType(ArgumentTypeEnum.SEQUENCE),
-                         default_sequence,
-                         **additional)
-        self.title = title
-        self.default_collection = default_collection
-        self.default_sequence = default_sequence
-        self.collection_label = collection_label
-        self.sequence_label = sequence_label
-
-    def to_dict_widget(self):
-        collection_selector_dict = super().to_dict_widget()
-        if self.title is not None:
-            collection_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.TITLE.value: self.title}
-            )
-        if self.default_collection is not None:
-            collection_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.COLLECTION_ID.value: self.default_collection.collection_id}
-            )
-        if self.default_sequence is not None:
-            collection_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.SEQUENCE_ID.value: self.default_sequence.sequence_id}
-            )
-        if self.collection_label is not None:
-            collection_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.COLLECTION_LABEL.value: self.collection_label}
-            )
-        if self.sequence_label is not None:
-            collection_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.SEQUENCE_LABEL.value: self.sequence_label}
-            )
-        return collection_selector_dict
+#
+# from ...widgets import AttributeNames, Widget
+# from ....model import Collection, Sequence
+#
+#
+# class CollectionSelector(Widget):
+#     def __init__(self,
+#                  default_collection: Collection = None,
+#                  default_sequence: Sequence = None,
+#                  name: str = None,
+#                  title: str = None,
+#                  collection_label: str = None,
+#                  sequence_label: str = None,
+#                  **additional):
+#         super().__init__(self.__class__.__name__,
+#                          name,
+#                          ArgumentType(ArgumentTypeEnum.SEQUENCE),
+#                          default_sequence,
+#                          **additional)
+#         self.title = title
+#         self.default_collection = default_collection
+#         self.default_sequence = default_sequence
+#         self.collection_label = collection_label
+#         self.sequence_label = sequence_label
+#
+#     def to_dict_widget(self):
+#         collection_selector_dict = super().to_dict_widget()
+#         if self.title is not None:
+#             collection_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.TITLE.value: self.title}
+#             )
+#         if self.default_collection is not None:
+#             collection_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.COLLECTION_ID.value: self.default_collection.collection_id}
+#             )
+#         if self.default_sequence is not None:
+#             collection_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.SEQUENCE_ID.value: self.default_sequence.sequence_id}
+#             )
+#         if self.collection_label is not None:
+#             collection_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.COLLECTION_LABEL.value: self.collection_label}
+#             )
+#         if self.sequence_label is not None:
+#             collection_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.SEQUENCE_LABEL.value: self.sequence_label}
+#             )
+#         return collection_selector_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_range_selector.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/datetime_range_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_selector.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/datetime_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/gauge.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/gauge.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/image.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/list.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/metric.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/metric.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import List
-
-from ... import ArgumentType, ArgumentTypeEnum
-from ...widgets import Widget, AttributeNames
-from ....model import Collection, Sequence
-
-
-class MultiSequenceSelector(Widget):
-    def __init__(self,
-                 collection: Collection = None,
-                 sequences: List[Sequence] = None,
-                 default_sequence: List[Sequence] = None,
-                 name: str = None,
-                 title: str = None,
-                 **additional):
-        super().__init__(self.__class__.__name__,
-                         name,
-                         ArgumentType(ArgumentTypeEnum.LIST, ArgumentTypeEnum.SEQUENCE),
-                         default_sequence if default_sequence else list(),
-                         **additional)
-        self.collection = collection
-        self.sequences = sequences
-        self.title = title
-        self.default_sequence = default_sequence if default_sequence is not None else []
-
-    def to_dict_widget(self):
-        multi_sequence_selector_dict = super().to_dict_widget()
-        if self.collection is not None:
-            multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.COLLECTION_ID.value: f"{self.collection.collection_id}"}
-            )
-        if self.sequences is not None:
-            sequences = [seq.sequence_id for seq in self.sequences]
-            multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
-                f"{AttributeNames.SEQUENCE_ID.value}s": sequences
-            })
-        if self.title is not None:
-            multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.TITLE.value: f"{self.title}"}
-            )
-        if self.default_sequence:
-            multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.DEFAULT.value: [sequence.sequence_id for sequence in self.default_sequence]
-            })
-        return multi_sequence_selector_dict
+# from typing import List
+#
+# from ... import ArgumentType, ArgumentTypeEnum
+# from ...widgets import Widget, AttributeNames
+# from ....model import Collection, Sequence
+#
+#
+# class MultiSequenceSelector(Widget):
+#     def __init__(self,
+#                  collection: Collection = None,
+#                  sequences: List[Sequence] = None,
+#                  default_sequence: List[Sequence] = None,
+#                  name: str = None,
+#                  title: str = None,
+#                  **additional):
+#         super().__init__(self.__class__.__name__,
+#                          name,
+#                          ArgumentType(ArgumentTypeEnum.LIST, ArgumentTypeEnum.SEQUENCE),
+#                          default_sequence if default_sequence else list(),
+#                          **additional)
+#         self.collection = collection
+#         self.sequences = sequences
+#         self.title = title
+#         self.default_sequence = default_sequence if default_sequence is not None else []
+#
+#     def to_dict_widget(self):
+#         multi_sequence_selector_dict = super().to_dict_widget()
+#         if self.collection is not None:
+#             multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.COLLECTION_ID.value: f"{self.collection.collection_id}"}
+#             )
+#         if self.sequences is not None:
+#             sequences = [seq.sequence_id for seq in self.sequences]
+#             multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
+#                 f"{AttributeNames.SEQUENCE_ID.value}s": sequences
+#             })
+#         if self.title is not None:
+#             multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.TITLE.value: f"{self.title}"}
+#             )
+#         if self.default_sequence:
+#             multi_sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.DEFAULT.value: [sequence.sequence_id for sequence in self.default_sequence]
+#             })
+#         return multi_sequence_selector_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/number_input.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/number_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/progress.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/progress.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/radio_group.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/radio_group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/ring.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/ring.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/selector.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/sequence_selector.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/sequence_selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import List
-
-from ... import ArgumentType, ArgumentTypeEnum
-from ...widgets import Widget, AttributeNames
-from ....model import Collection, Sequence
-
-
-class SequenceSelector(Widget):
-    def __init__(self,
-                 collection: Collection = None,
-                 sequences: List[Sequence] = None,
-                 default_sequence: Sequence = None,
-                 name: str = None,
-                 title: str = None,
-                 **additional):
-        super().__init__(self.__class__.__name__,
-                         name,
-                         ArgumentType(ArgumentTypeEnum.SEQUENCE),
-                         default_sequence,
-                         **additional)
-        self.collection = collection
-        self.sequences = sequences
-        self.title = title
-        self.default_sequence = default_sequence
-
-    def to_dict_widget(self):
-        sequence_selector_dict = super().to_dict_widget()
-        if self.collection is not None:
-            sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.COLLECTION_ID.value: self.collection.collection_id}
-            )
-        if self.sequences is not None:
-            sequences = [seq.sequence_id for seq in self.sequences]
-            sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
-                f"{AttributeNames.SEQUENCE_ID.value}s": sequences
-            })
-        if self.title is not None:
-            sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
-                {AttributeNames.TITLE.value: self.title}
-            )
-        if self.default_sequence:
-            sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.DEFAULT.value: self.default_sequence.sequence_id
-            })
-        return sequence_selector_dict
+# from typing import List
+#
+# from ... import ArgumentType, ArgumentTypeEnum
+# from ...widgets import Widget, AttributeNames
+# from ....model import Collection, Sequence
+#
+#
+# class SequenceSelector(Widget):
+#     def __init__(self,
+#                  collection: Collection = None,
+#                  sequences: List[Sequence] = None,
+#                  default_sequence: Sequence = None,
+#                  name: str = None,
+#                  title: str = None,
+#                  **additional):
+#         super().__init__(self.__class__.__name__,
+#                          name,
+#                          ArgumentType(ArgumentTypeEnum.SEQUENCE),
+#                          default_sequence,
+#                          **additional)
+#         self.collection = collection
+#         self.sequences = sequences
+#         self.title = title
+#         self.default_sequence = default_sequence
+#
+#     def to_dict_widget(self):
+#         sequence_selector_dict = super().to_dict_widget()
+#         if self.collection is not None:
+#             sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.COLLECTION_ID.value: self.collection.collection_id}
+#             )
+#         if self.sequences is not None:
+#             sequences = [seq.sequence_id for seq in self.sequences]
+#             sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
+#                 f"{AttributeNames.SEQUENCE_ID.value}s": sequences
+#             })
+#         if self.title is not None:
+#             sequence_selector_dict[AttributeNames.PROPERTIES.value].update(
+#                 {AttributeNames.TITLE.value: self.title}
+#             )
+#         if self.default_sequence:
+#             sequence_selector_dict[AttributeNames.PROPERTIES.value].update({
+#                 AttributeNames.DEFAULT.value: self.default_sequence.sequence_id
+#             })
+#         return sequence_selector_dict
```

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/slider.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/slider.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/table.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/table.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/text.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text_input.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/text_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/timer.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/controllers/timer.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/datetime_utils.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/grid_layout.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/horizontal_layout.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/horizontal_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/panel.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/panel.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/tabs_layout.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/tabs_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/vertical_layout.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/layouts/vertical_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/util.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/util.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/apps/widgets/widget.py` & `shapelets-platform-2.0.96/src/shapelets/apps/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/functions.py` & `shapelets-platform-2.0.96/src/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/iris.csv` & `shapelets-platform-2.0.96/src/shapelets/iris.csv`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/app.py` & `shapelets-platform-2.0.96/src/shapelets/svr/app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/authn/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/authn/authhttp.py` & `shapelets-platform-2.0.96/src/shapelets/svr/authn/authhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/authn/authrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/authn/authrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/authn/authservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/authn/authservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/authn/gc_client.py` & `shapelets-platform-2.0.96/src/shapelets/svr/authn/gc_client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/authn/iauthrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/authn/iauthservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/access_token_credentials.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/access_token_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen1.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/azure_gen1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen2.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/azure_gen2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/driver.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/driver.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/dynamic_credentials.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_config.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_config.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_vfs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_file.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/fsspec_vfs_file.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/ftp.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/ftp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/local.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/local.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/protocols.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/protocols.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/smb.py` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/smb.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/vfs_sample_config.toml` & `shapelets-platform-2.0.96/src/shapelets/svr/data/vfs/vfs_sample_config.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataapps_ws.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataapps_ws.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappshttp.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataappshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/dataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/http_docs.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/idataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/dataapps/idataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/native/database.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/native/database.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/native/settings.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/native/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_builder.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/schema_builder.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v1.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v2.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v3.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v3.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v4.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/schema_v4.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/db/setup.py` & `shapelets-platform-2.0.96/src/shapelets/svr/db/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/execution/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/execution/executionhttp.py` & `shapelets-platform-2.0.96/src/shapelets/svr/execution/executionhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/execution/executionservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/execution/executionservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/execution/http_docs.py` & `shapelets-platform-2.0.96/src/shapelets/svr/execution/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/groups/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/groups/groupservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/groups/groupservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/groups/groupshttp.py` & `shapelets-platform-2.0.96/src/shapelets/svr/groups/groupshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/groups/groupsrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/groups/groupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/groups/igroupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/groups/igroupsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/model/dataapps.py` & `shapelets-platform-2.0.96/src/shapelets/svr/model/dataapps.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/model/principals.py` & `shapelets-platform-2.0.96/src/shapelets/svr/model/principals.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/model/users.py` & `shapelets-platform-2.0.96/src/shapelets/svr/model/users.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/asttranslation.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/asttranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/conversions.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/conversions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/core.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/core.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/decompiling.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/decompiling.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/exceptions.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/hashdict.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/hashdict.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/ormtypes.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/ormtypes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/prototypes/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/serialization.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/serialization.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqlbuilding.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/sqlbuilding.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqltranslation.py` & `shapelets-platform-2.0.96/src/shapelets/svr/mustang/sqltranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/server.py` & `shapelets-platform-2.0.96/src/shapelets/svr/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/client.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/defaults.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/functions.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/http.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/http.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/reload.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/reload.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/server.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.toml` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/ssl.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/ssl.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/telemetry.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/telemetry.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/settings/websocket.py` & `shapelets-platform-2.0.96/src/shapelets/svr/settings/websocket.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/telemetry/sysinfo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/telemetry/sysinfo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/telemetry/telemetryservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/telemetry/telemetryservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/users/__init__.py` & `shapelets-platform-2.0.96/src/shapelets/svr/users/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/users/http_docs.py` & `shapelets-platform-2.0.96/src/shapelets/svr/users/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/users/iusersrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/users/iusersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/users/iusersservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/users/iusersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/users/usershttp.py` & `shapelets-platform-2.0.96/src/shapelets/svr/users/usershttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/users/usersrepo.py` & `shapelets-platform-2.0.96/src/shapelets/svr/users/usersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/users/usersservice.py` & `shapelets-platform-2.0.96/src/shapelets/svr/users/usersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/utils/crypto.py` & `shapelets-platform-2.0.96/src/shapelets/svr/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/utils/flexbytes.py` & `shapelets-platform-2.0.96/src/shapelets/svr/utils/flexbytes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/altair.json` & `shapelets-platform-2.0.96/src/shapelets/svr/www/altair.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/asset-manifest.json` & `shapelets-platform-2.0.96/src/shapelets/svr/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/dataapp.json` & `shapelets-platform-2.0.96/src/shapelets/svr/www/dataapp.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/favicon.ico` & `shapelets-platform-2.0.96/src/shapelets/svr/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/index.html` & `shapelets-platform-2.0.96/src/shapelets/svr/www/index.html`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/2.379683b2.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/audit.cb539a06.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/audit.cb539a06.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/bin.7e762965.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/bin.7e762965.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/clear.27b15301.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/clear.27b15301.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/collections.06fdf54a.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/collections.06fdf54a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-time.a1e86419.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/date-time.a1e86419.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/download-image.87310709.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/download-image.87310709.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/filter.cec803b8.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/filter.cec803b8.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logout.57c593a5.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/logout.57c593a5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf.5d189efa.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/pdf.5d189efa.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/share.bc9a8370.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/share.bc9a8370.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/single-plot.864a583b.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/single-plot.864a583b.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-top.6d51781b.png` & `shapelets-platform-2.0.96/src/shapelets/svr/www/static/media/wave-top.6d51781b.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.95/src/shapelets_platform.egg-info/PKG-INFO` & `shapelets-platform-2.0.96/src/shapelets_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.95
+Version: 2.0.96
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.95/src/shapelets_platform.egg-info/SOURCES.txt` & `shapelets-platform-2.0.96/src/shapelets_platform.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -69,33 +69,14 @@
 src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
 src/shapelets/apps/widgets/layouts/__init__.py
 src/shapelets/apps/widgets/layouts/grid_layout.py
 src/shapelets/apps/widgets/layouts/horizontal_layout.py
 src/shapelets/apps/widgets/layouts/panel.py
 src/shapelets/apps/widgets/layouts/tabs_layout.py
 src/shapelets/apps/widgets/layouts/vertical_layout.py
-src/shapelets/model/__init__.py
-src/shapelets/model/altair.py
-src/shapelets/model/capsule.py
-src/shapelets/model/collection.py
-src/shapelets/model/dataframe.py
-src/shapelets/model/exceptions.py
-src/shapelets/model/function_description.py
-src/shapelets/model/function_parameter.py
-src/shapelets/model/group.py
-src/shapelets/model/image.py
-src/shapelets/model/metadata_item.py
-src/shapelets/model/model.py
-src/shapelets/model/ndarray.py
-src/shapelets/model/permissions.py
-src/shapelets/model/replicated_param.py
-src/shapelets/model/sequence.py
-src/shapelets/model/sequence_axis.py
-src/shapelets/model/user.py
-src/shapelets/model/view_match.py
 src/shapelets/svr/__init__.py
 src/shapelets/svr/app.py
 src/shapelets/svr/docs.py
 src/shapelets/svr/server.py
 src/shapelets/svr/authn/__init__.py
 src/shapelets/svr/authn/authhttp.py
 src/shapelets/svr/authn/authrepo.py
```

### Comparing `shapelets-platform-2.0.95/src/shapelets_platform.egg-info/requires.txt` & `shapelets-platform-2.0.96/src/shapelets_platform.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 adlfs~=2023.4
 argparse~=1.4
 blacksheep~=1.2
 dill~=0.3
+email-validator~=2.0
 folium~=0.13
 jmespath~=0.9
+matplotlib~=3.7
 mypy~=1.4
 numpy~=1.24
 pandas~=2.0
 psutil~=5.9
 pyarrow~=12.0
 py-cpuinfo~=9.0
 pydantic~=1.10
 PyNaCl~=1.5
 requests~=2.31
-shapelets_native==2.0.95
+shapelets_native==2.0.96
 tabulate~=0.9
 tomlkit~=0.12
 typing_extensions~=4.7
 uvicorn~=0.23
 websocket-client~=1.5
 websockets~=10.3
```

