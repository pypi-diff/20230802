# Comparing `tmp/shapelets-platform-2.0.94.tar.gz` & `tmp/shapelets-platform-2.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-platform-2.0.94.tar", last modified: Tue Jul 18 13:03:51 2023, max compression
+gzip compressed data, was "shapelets-platform-2.0.95.tar", last modified: Wed Aug  2 09:47:32 2023, max compression
```

## Comparing `shapelets-platform-2.0.94.tar` & `shapelets-platform-2.0.95.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.157002 shapelets-platform-2.0.94/
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/COPYING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-18 13:03:51.157002 shapelets-platform-2.0.94/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/noxfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     3008 2023-07-18 13:03:51.161002 shapelets-platform-2.0.94/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.061003 shapelets-platform-2.0.94/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.069003 shapelets-platform-2.0.94/src/shapelets/
--rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/_cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)    51403 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/_relations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/_uom.py
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-07-18 13:03:47.000000 shapelets-platform-2.0.94/src/shapelets/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/_version.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.073003 shapelets-platform-2.0.94/src/shapelets/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    68871 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/data_app.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/data_app_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.073003 shapelets-platform-2.0.94/src/shapelets/apps/widgets/
--rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/attribute_names.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.077003 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/
--rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/altair_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/bar_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/folium_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/heatmap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19053 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/line_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/pie_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/plotly_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/polar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/radar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/scatter_plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.081003 shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/filtering_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/metadata_field.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/metadata_filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/temporal_context.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.093003 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/
--rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1996 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/button.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4503 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/collection_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7578 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8196 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/datetime_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/gauge.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5978 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/metric.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/number_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/progress.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9880 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/radio_group.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.093003 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/resources/
--rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
--rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/ring.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/sequence_list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14789 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/slider.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/text.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/text_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/timer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/datetime_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.097003 shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/
--rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/grid_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6057 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/horizontal_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/panel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/tabs_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5683 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/vertical_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26169 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/apps/widgets/widget.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/iris.csv
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.105003 shapelets-platform-2.0.94/src/shapelets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/altair.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/capsule.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/collection.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/function_description.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/function_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/group.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/metadata_item.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/ndarray.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/replicated_param.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/sequence.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/sequence_axis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/user.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/model/view_match.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.105003 shapelets-platform-2.0.94/src/shapelets/svr/
--rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.109003 shapelets-platform-2.0.94/src/shapelets/svr/authn/
--rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/authn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/authn/authhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/authn/authrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/authn/authservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/authn/gc_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/authn/iauthrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/authn/iauthservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.109003 shapelets-platform-2.0.94/src/shapelets/svr/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.113003 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/access_token_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/azure_gen1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/azure_gen2.py
--rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/dynamic_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_vfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/local.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/protocols.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/smb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/vfs_sample_config.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.117003 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataapps_ws.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9536 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataappshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2407 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataappsservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/idataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1507 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/dataapps/idataappsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.121003 shapelets-platform-2.0.94/src/shapelets/svr/db/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.121003 shapelets-platform-2.0.94/src/shapelets/svr/db/native/
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/native/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/native/database.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/native/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/schema_builder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v4.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/db/setup.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/docs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.125003 shapelets-platform-2.0.94/src/shapelets/svr/execution/
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/execution/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/execution/executionhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/execution/executionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/execution/executionservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/execution/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/execution/iexecutionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/execution/iexecutionservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.129003 shapelets-platform-2.0.94/src/shapelets/svr/groups/
--rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/groups/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/groups/groupservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4410 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/groups/groupshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5028 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/groups/groupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/groups/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/groups/igroupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/groups/igroupsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.129003 shapelets-platform-2.0.94/src/shapelets/svr/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/model/dataapps.py
--rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/model/function.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/model/groups.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/model/principals.py
--rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/model/users.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.133003 shapelets-platform-2.0.94/src/shapelets/svr/mustang/
--rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/asttranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/conversions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/core.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/decompiling.py
--rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/hashdict.py
--rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/identifier.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/ormtypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.137003 shapelets-platform-2.0.94/src/shapelets/svr/mustang/prototypes/
--rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/prototypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/python_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/sqlbuilding.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/mustang/sqltranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.141003 shapelets-platform-2.0.94/src/shapelets/svr/settings/
--rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/defaults.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/http.py
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/reload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/settings.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/ssl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/settings/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.141003 shapelets-platform-2.0.94/src/shapelets/svr/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/telemetry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/telemetry/itelemetryservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/telemetry/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/telemetry/telemetryservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.141003 shapelets-platform-2.0.94/src/shapelets/svr/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/users/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/users/iusersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/users/iusersservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/users/usershttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/users/usersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/users/usersservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.145002 shapelets-platform-2.0.94/src/shapelets/svr/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/utils/crypto.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/svr/utils/flexbytes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.145002 shapelets-platform-2.0.94/src/shapelets/svr/www/
--rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-07-18 13:03:45.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/altair.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/asset-manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/custom_sample.js
--rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/dataapp.json
--rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/robots.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.061003 shapelets-platform-2.0.94/src/shapelets/svr/www/static/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.145002 shapelets-platform-2.0.94/src/shapelets/svr/www/static/css/
--rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
--rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.153002 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)  7622607 2023-07-18 13:03:45.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/2.379683b2.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-07-18 13:03:45.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   808300 2023-07-18 13:03:45.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.157002 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/
--rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/audit.cb539a06.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/bin.7e762965.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/clear.27b15301.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/download-image.87310709.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/filter.cec803b8.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
--rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logout.57c593a5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/share.bc9a8370.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
--rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-07-18 13:03:44.000000 shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-07-18 12:46:50.000000 shapelets-platform-2.0.94/src/shapelets/systemd_template.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 13:03:51.157002 shapelets-platform-2.0.94/src/shapelets_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-18 13:03:47.000000 shapelets-platform-2.0.94/src/shapelets_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    11445 2023-07-18 13:03:51.000000 shapelets-platform-2.0.94/src/shapelets_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-18 13:03:47.000000 shapelets-platform-2.0.94/src/shapelets_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-07-18 13:03:47.000000 shapelets-platform-2.0.94/src/shapelets_platform.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     1241 2023-07-18 13:03:47.000000 shapelets-platform-2.0.94/src/shapelets_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-07-18 13:03:47.000000 shapelets-platform-2.0.94/src/shapelets_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/COPYING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/noxfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     2813 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.559232 shapelets-platform-2.0.95/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.567232 shapelets-platform-2.0.95/src/shapelets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19253 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    52015 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_relations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_uom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/_version.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.571232 shapelets-platform-2.0.95/src/shapelets/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    70253 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/data_app.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/data_app_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.575232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/attribute_names.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.583232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3364 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/altair_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/bar_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2584 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/folium_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/heatmap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19966 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/line_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/pie_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/plotly_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/polar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/radar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/scatter_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.587232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/filtering_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/temporal_context.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.595232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2014 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/button.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/checkbox.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/collection_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8331 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8706 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/gauge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8126 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5929 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/metric.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11032 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/number_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9101 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/radio_group.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.599232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4631 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/ring.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10545 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/sequence_list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14849 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/slider.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9017 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/timer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/datetime_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.599232 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/grid_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6038 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/horizontal_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/panel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5000 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/tabs_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5660 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/vertical_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26169 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/apps/widgets/widget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/iris.csv
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.607232 shapelets-platform-2.0.95/src/shapelets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/altair.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/capsule.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/function_description.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/function_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/group.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/metadata_item.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/ndarray.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/replicated_param.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/sequence.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/sequence_axis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/user.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/model/view_match.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.611233 shapelets-platform-2.0.95/src/shapelets/svr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.619233 shapelets-platform-2.0.95/src/shapelets/svr/authn/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/authhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/authrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/authservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/gc_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.619233 shapelets-platform-2.0.95/src/shapelets/svr/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.627233 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/access_token_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/dynamic_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/local.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/smb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/vfs_sample_config.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.635233 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3264 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataapps_ws.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9912 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2415 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.639233 shapelets-platform-2.0.95/src/shapelets/svr/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.639233 shapelets-platform-2.0.95/src/shapelets/svr/db/native/
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/native/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/native/database.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/native/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v4.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/db/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/docs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.643233 shapelets-platform-2.0.95/src/shapelets/svr/execution/
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/executionhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/executionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/executionservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/iexecutionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/execution/iexecutionservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.647233 shapelets-platform-2.0.95/src/shapelets/svr/groups/
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/groupservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4410 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/groupshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5028 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/groupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.651233 shapelets-platform-2.0.95/src/shapelets/svr/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/dataapps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/function.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/groups.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/principals.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/model/users.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.659233 shapelets-platform-2.0.95/src/shapelets/svr/mustang/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/asttranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/core.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/decompiling.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/hashdict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/ormtypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.659233 shapelets-platform-2.0.95/src/shapelets/svr/mustang/prototypes/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/prototypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/python_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqlbuilding.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqltranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.667233 shapelets-platform-2.0.95/src/shapelets/svr/settings/
+-rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/http.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/reload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/ssl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/settings/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.667233 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/
+-rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/itelemetryservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/telemetry/telemetryservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.671233 shapelets-platform-2.0.95/src/shapelets/svr/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/iusersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/iusersservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/usershttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/usersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/users/usersservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.671233 shapelets-platform-2.0.95/src/shapelets/svr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/utils/crypto.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/svr/utils/flexbytes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.675233 shapelets-platform-2.0.95/src/shapelets/svr/www/
+-rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-08-02 09:47:25.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/altair.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/asset-manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/custom_sample.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/dataapp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/robots.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.559232 shapelets-platform-2.0.95/src/shapelets/svr/www/static/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.675233 shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
+-rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.687233 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)  7622607 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   808300 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.695233 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/
+-rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/audit.cb539a06.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/bin.7e762965.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/clear.27b15301.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-08-02 09:47:28.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/download-image.87310709.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/filter.cec803b8.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logout.57c593a5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/share.bc9a8370.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-08-02 09:47:24.000000 shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-08-02 09:33:26.000000 shapelets-platform-2.0.95/src/shapelets/systemd_template.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 09:47:32.699233 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    11445 2023-08-02 09:47:32.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1109 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-08-02 09:47:29.000000 shapelets-platform-2.0.95/src/shapelets_platform.egg-info/top_level.txt
```

### Comparing `shapelets-platform-2.0.94/LICENSE.md` & `shapelets-platform-2.0.95/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/PKG-INFO` & `shapelets-platform-2.0.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.94
+Version: 2.0.95
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
@@ -15,24 +15,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Classifier: License :: Other/Proprietary License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: vfs-all
 Provides-Extra: vfs-azure
 Provides-Extra: vfs-dropbox
 Provides-Extra: vfs-google
```

### Comparing `shapelets-platform-2.0.94/README.md` & `shapelets-platform-2.0.95/README.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/noxfile.py` & `shapelets-platform-2.0.95/noxfile.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/pyproject.toml` & `shapelets-platform-2.0.95/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["error"]
 testpaths = ["tests"]
 
 [tool.mypy]
 files = "src"
-python_version = "3.7"
+python_version = "3.8"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 
 
@@ -38,15 +38,15 @@
   "noxfile.py"
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.master]
-py-version = "3.7"
+py-version = "3.8"
 ignore-paths= ["src/package/_version.py"]
 
 [tool.pylint.reports]
 output-format = "colorized"
 
 [tool.pylint.similarities]
 ignore-imports = "yes"
```

### Comparing `shapelets-platform-2.0.94/setup.cfg` & `shapelets-platform-2.0.95/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 	Intended Audience :: Science/Research
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: Unix
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering
 	Topic :: Software Development
 	Typing :: Typed
@@ -34,48 +33,40 @@
 project_urls = 
 	Homepage = https://shapelets.io/
 	Documentation = https://shapelets.io/doc/contents.html
 
 [options]
 packages = find:
 install_requires = 
-	altair ~= 4.2
+	adlfs ~= 2023.4
 	argparse ~= 1.4
 	blacksheep ~= 1.2
-	cloudpickle ~= 2.2
 	dill ~= 0.3
-	email-validator ~= 1.3
 	folium ~= 0.13
-	h11 ~= 0.12
 	jmespath ~= 0.9
-	matplotlib ~= 3.5
-	mypy ~= 0.990
-	numpy ~= 1.25
+	mypy ~= 1.4
+	numpy ~= 1.24
 	pandas ~= 2.0
 	psutil ~= 5.9
 	pyarrow ~= 12.0
 	py-cpuinfo ~= 9.0
-	pydantic == 1.10.11
-	pygeohash ~= 1.2
+	pydantic ~= 1.10
 	PyNaCl ~= 1.5
-	requests ~= 2.28
-	setuptools-scm ~= 7.1
-	shapelets_native == 2.0.94
-	tabulate ~= 0.8
-	tomlkit ~= 0.11
-	tqdm ~= 4.64
+	requests ~= 2.31
+	shapelets_native == 2.0.95
+	tabulate ~= 0.9
+	tomlkit ~= 0.12
 	typing_extensions ~= 4.7
-	uvicorn ~= 0.18
-	vega-datasets ~= 0.9
+	uvicorn ~= 0.23
 	websocket-client ~= 1.5
 	websockets ~= 10.3
 	lockfile ~= 0.12; platform_system!="Windows"
 	python_daemon >= 2.3.2; platform_system!="Windows"
 	uvloop ~= 0.17; platform_system!="Windows"
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.entry_points]
 console_scripts = 
 	shapelets = shapelets:cli
```

### Comparing `shapelets-platform-2.0.94/setup.py` & `shapelets-platform-2.0.95/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/_api.py` & `shapelets-platform-2.0.95/src/shapelets/_api.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/_cli.py` & `shapelets-platform-2.0.95/src/shapelets/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,16 +198,16 @@
     which_server.add_argument("--local", action="store_true", help='Use Local server')
     which_server.add_argument("--url", type=str, help='URL of the server to connect to')
 
     client_parser.add_argument("-u", "--usr", type=str, help='User Name')
     client_parser.add_argument("-p", "--pwd", type=str, help='User Password')
     client_parser.add_argument("--create", action="store_true", help='Create user if not exists')
     client_parser.add_argument("--remember-me", action="store_true", help='Logon and remember credentials')
-    client_parser.add_argument("--enable-telemetry", action="store_true", help='Enable telemetry')
-    client_parser.add_argument("--disable-telemetry", action="store_true", help='Disable telemetry')
+    # client_parser.add_argument("--enable-telemetry", action="store_true", help='Enable telemetry')
+    # client_parser.add_argument("--disable-telemetry", action="store_true", help='Disable telemetry')
     return parser
 
 
 def resolve_host(expression: str) -> Optional[str]:
     try:
         return str(IPv4Address(expression))
     except:
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/_relations.py` & `shapelets-platform-2.0.95/src/shapelets/_relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 from threading import get_ident
 
 import numpy as np
 import pandas as pd
 import pyarrow
 import pyarrow.dataset
+import pyarrow.feather as feather
 import tabulate
 import pandas
 
 from .svr import mustang
 
 
 def _resolveFile(file: str, expanded: bool = False) -> str:
@@ -968,14 +969,34 @@
                 pyarrow.Table, pyarrow.RecordBatchReader, pyarrow.dataset.FileSystemDataset,
                 pyarrow.dataset.InMemoryDataset,
                 pyarrow.dataset.Scanner)):
             raise ValueError(
                 "Expected an arrow object of type Table, RecordBatchReader, FileSystemDataset, InMemoryDataset or Scanner")
         return DataSet(self.__factory.arrow(arrowObj), self.__map_fn)
 
+    def from_feather(self, path: Union[str, Path]) -> DataSet:
+        r"""
+        Imports a feather file as a Relation.
+
+        Examples
+        --------
+
+        >>> dataset = session.from_feather("myPath")
+
+        """
+        if isinstance(path, str):
+            file_expression = _resolveFile(path)
+        elif isinstance(path, Path):
+            file_expression = str(path.resolve())
+        else:
+            raise ValueError(f"[{path}] didn't resolve any files")
+
+        arrow_obj = feather.read_table(file_expression)
+        return self.from_arrow(arrow_obj)
+
     def from_pandas(self, df: pandas.DataFrame) -> DataSet:
         r"""
         Load a pandas dataset as a relation.
 
         Examples
         --------
 
@@ -1264,15 +1285,15 @@
 
         """
         query = mustang.make_query(genExpr, frame_depth=1, left_join=False)
         sql = mustang.construct_sql_from_query(query)
 
         return DataSet(self.__factory.relation_from_query(sql), self.__map_fn)
 
-    def from_sql(self, sql: str) -> DataSet:
+    def execute_sql(self, sql: str) -> DataSet:
         r"""
         Returns a Dataset from raw SQL query
 
         Parameters
         ----------
         sql: str with SQL query in raw format
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/_uom.py` & `shapelets-platform-2.0.95/src/shapelets/_uom.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/data_app.py` & `shapelets-platform-2.0.95/src/shapelets/apps/data_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -321,22 +321,15 @@
             * :func:`~shapelets.apps.DataApp.figure`
             * :func:`~shapelets.apps.DataApp.image`   
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
-
-            * str
-            * bytes
-            * :func:`~shapelets.apps.DataApp.path`
-            * :func:`~shapelets.apps.DataApp.figure`
-            * :func:`~shapelets.apps.DataApp.image`
+        *Currently this widget cannot be used as input in a binding function.*
 
         """
         return ImageWidget(img, caption, placeholder, parent_data_app=self, **additional)
 
     # def list(self,
     #          list_title: Optional[str] = None,
     #          items: Optional[List[Widget]] = [],
@@ -419,15 +412,14 @@
         You can bind this widget as: 
 
         .. hlist::
             :columns: 1
 
             * int
             * float
-            * :func:`~shapelets.apps.DataApp.number_input`
 
         """
 
         return NumberInputWidget(title, value, default_value, placeholder, min, max, step, text_style, units,
                                  parent_data_app=self, **additional)
 
     # def sequence_list(self,
@@ -509,15 +501,14 @@
         You can bind this widget as: 
 
         .. hlist::
             :columns: 1
 
             * str
             * int
-            * :func:`~shapelets.apps.DataApp.text_input`
         """
         return TextInputWidget(title=title, value=value, placeholder=placeholder, multiline=multiline,
                                text_style=text_style, toolbar=toolbar, markdown=markdown, width=width,
                                parent_data_app=self, **additional)
 
     def datetime_selector(self,
                           title: str = None,
@@ -547,18 +538,32 @@
         -------
         DateSelectorWidget
 
         Examples
         --------
         >>> date_selector = app.datetime_selector()
 
-        >>> date = datetime.date(2022, 10, 17)
-        >>> date1 = datetime.date(2009, 10, 8)
-        >>> date2 = datetime.date(2029, 10, 27)
-        >>> date_selector = app.datetime_selector("Date only", date, date1, date2)
+        >>> # Datetime selector with int
+        >>> dt = app.datetime_selector(date_time=1667468964,
+        >>>                             min_date=1667460964,
+        >>>                             max_date=1676913679)
+
+        >>> # Datetime selector with datetime
+        >>> dt = app.datetime_selector(date_time=datetime(year=2022, month=1, day=1, hour=18, minute=20))
+
+        >>> # Datetime selector with date
+        >>> dt = app.datetime_selector(date_time=date(year=2022, month=1, day=1),
+        >>>                             min_date=date(year=1950, month=1, day=1),
+        >>>                             max_date=date(year=2050, month=1, day=1))
+
+        >>> # Datetime selector with strings
+        >>> dt = app.datetime_selector(date_time='1970-01-01',
+        >>>                             min_date='1955-01-01',
+        >>>                             max_date='2100-01-01')
+
 
 
         .. rubric:: Bind compatibility
 
         You can bind this widget with this:
 
         .. hlist::
@@ -574,18 +579,14 @@
 
         You can bind this widget as: 
 
         .. hlist::
             :columns: 1
 
             * str
-            * int
-            * :func:`~shapelets.apps.DataApp.datetime_selector`
-            * datetime.datetime
-            * datetime.date
         """
         return DateSelectorWidget(title, date_time, min_date, max_date, parent_data_app=self, **additional)
 
     def datetime_range_selector(self,
                                 title: str = None,
                                 start_datetime: Union[
                                     float, int, str, datetime.datetime, datetime.date, datetime.time] = None,
@@ -620,52 +621,57 @@
         -------
         DatetimeRangeSelectorWidget
 
         Examples
         --------
         >>> date_selector = app.datetime_range_selector()
 
-        >>> # Create sample dates using datetime
-        >>> start_date = datetime.date(2021, 1, 17)
-        >>> end_date = datetime.date(2022, 1, 28)
-        >>> min_date = datetime.date(2018, 1, 17)
-        >>> max_date = datetime.date(2023, 1, 28)
-        >>> # Create selector based on datetime objects
-        >>> dateSelector1 = app.datetime_range_selector("selector from datetime", 
-        >>>     start_datetime=start_date, 
-        >>>     end_datetime=end_date, 
-        >>>     min_datetime=min_date, 
-        >>>     max_datetime=max_date)
+        >>> # Datetime range selector with int
+        >>> dt = app.datetime_range_selector(start_datetime=1667468964,
+        >>>                                 end_datetime=1667468964,
+        >>>                                 min_datetime=1667468964,
+        >>>                                 max_datetime=1667468964)
+
+        >>> # Datetime range selector with date
+        >>> dt = app.datetime_range_selector(start_datetime=date(year=2022, month=11, day=1),
+        >>>                                 end_datetime=date(year=2022, month=11, day=10),
+        >>>                                 min_datetime=date(year=1950, month=1, day=1),
+        >>>                                 max_datetime=date(year=2050, month=1, day=1))
+
+        >>> # Datetime range selector with datetime
+        >>> dt = app.datetime_range_selector(start_datetime=datetime(year=2022, month=11, day=1, hour=21),
+        >>>                                 end_datetime=datetime(year=2022, month=11, day=10, hour=19, second=5),
+        >>>                                 min_datetime=date(year=1950, month=1, day=1),
+        >>>                                 max_datetime=date(year=2050, month=1, day=1))
+
+        >>> # Datetime range selector with string
+        >>> dt = app.datetime_range_selector(start_datetime='2022-01-01 00:05:00',
+        >>>                                 end_datetime='2022-12-31 23:59:59',
+        >>>                                 min_datetime='1955-01-01',
+        >>>                                 max_datetime='2100-01-01')
+
 
 
         .. rubric:: Bind compatibility
 
         You can bind this widget with this:
 
         .. hlist::
             :columns: 1
 
-            * str
-            * int
             * :func:`~shapelets.apps.DataApp.datetime_range_selector`
-            * datetime.datetime
-            * datetime.date
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
         .. hlist::
             :columns: 1
 
-            * str
-            * int
-            * :func:`~shapelets.apps.DataApp.datetime_range_selector`
-            * datetime.datetime
-            * datetime.date
+            * tuple
         """
         return DatetimeRangeSelectorWidget(title, start_datetime, end_datetime, min_datetime, max_datetime,
                                            parent_data_app=self,
                                            **additional)
 
     def slider(self,
                title: str = None,
@@ -717,30 +723,38 @@
         .. rubric:: Bind compatibility
 
         You can bind this widget with this:
 
         .. hlist::
             :columns: 1
 
-            * :func:`~shapelets.apps.DataApp.slider`
             * int
             * float
             * list
+            * :func:`~shapelets.apps.DataApp.slider`
+
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
+        If you are using `range=False`
+
         .. hlist::
             :columns: 1
 
-            * :func:`~shapelets.apps.DataApp.slider`
             * int
             * float
-            * list
+
+        If you are using `range=True`
+
+        .. hlist::
+            :columns: 1
+
+            * tuple 
         """
 
         return SliderWidget(title, value, min_value, max_value, step, range, options, parent_data_app=self,
                             **additional)
 
     def button(self, text: str = "", **additional) -> Button:
         """
@@ -760,14 +774,15 @@
         >>> button = app.button("Press me") 
 
         You can bind this widget with this:
 
         .. hlist::
             :columns: 1
 
+            * str
             * :func:`~shapelets.apps.DataApp.button`
 
         Note: bind function will change button text.
 
         """
         return Button(text, parent_data_app=self, **additional)
 
@@ -849,18 +864,15 @@
 
             * :func:`~shapelets.apps.DataApp.altair_chart`
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
-
-            * :func:`~shapelets.apps.DataApp.altair_chart`           
+        *Currently this widget cannot be used as input in a binding function.*             
         """
         return AltairChartWidget(title, chart, parent_data_app=self, **additional)
 
     def folium_chart(self, title: Optional[str] = None, folium: Optional[any] = None,
                      **additional) -> FoliumChartWidget:
         """
         Creates a Folium map: a declarative statistical visualization library for Python
@@ -893,18 +905,16 @@
 
             * :func:`~shapelets.apps.DataApp.folium_chart`
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
+        *Currently this widget cannot be used as input in a binding function.* 
 
-            * :func:`~shapelets.apps.DataApp.folium_chart`                
         """
         return FoliumChartWidget(title, folium, parent_data_app=self, **additional)
 
     # def plotly_chart(self, title: Optional[str] = None, fig: Optional[any] = None, **additional) -> PlotlyChartWidget:
     #     """
     #     Creates a Plotly graph. Plotly's Python graphing library makes interactive, publication-quality graphs
     #     (https://plotly.com/graphing-libraries).
@@ -961,18 +971,15 @@
 
             * :func:`~shapelets.apps.DataApp.vertical_layout`
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
-
-            * :func:`~shapelets.apps.DataApp.vertical_layout`         
+        *Currently this widget cannot be used as input in a binding function.*        
         """
         return VerticalLayoutWidget(panel_title=title, panel_id=panel_id, vertical_align=vertical_align, span=span,
                                     offset=offset,
                                     parent_data_app=self, **additional)
 
     def horizontal_layout(self,
                           title: str = None,
@@ -1017,18 +1024,15 @@
 
             * :func:`~shapelets.apps.DataApp.horizontal_layout`
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
-
-            * :func:`~shapelets.apps.DataApp.horizontal_layout`              
+        *Currently this widget cannot be used as input in a binding function.*             
         """
         return HorizontalLayoutWidget(panel_title=title,
                                       panel_id=panel_id,
                                       horizontal_align=horizontal_align,
                                       vertical_align=vertical_align,
                                       parent_data_app=self,
                                       **additional)
@@ -1082,18 +1086,15 @@
 
             * :func:`~shapelets.apps.DataApp.tabs_layout`
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
-
-            * :func:`~shapelets.apps.DataApp.tabs_layout`               
+        *Currently this widget cannot be used as input in a binding function.*              
         """
         return TabsLayoutWidget(title, parent_data_app=self, **additional)
 
     def line_chart(self,
                    data: Optional[LineChartValueType] = None,
                    title: str = None,
                    views: List[View] = [],
@@ -1130,46 +1131,62 @@
 
         Returns
         -------
         LineChart
 
         Examples
         --------
-        >>> line_chart1 = app.line_chart(title='My line Chart', data=sdf) 
+        
+        You can create a line chart using this:
+
+        >>> line_chart = app.line_chart(title="Linechart", data=df)
+
+        .. image:: /_static/linechart_img/linechart_default.png
+            :alt: Data App main page
+        
+        By default `multi_lane=True`, so if your dataframe have more than one time series will plot in a separated lanes. You can set it to `False` you can get a line chart with only one line.
+
+        >>> line_chart = app.line_chart(title="Linechart", data=df, multi_lane=False)
+        
+        .. image:: /_static/linechart_img/linechart_multilane_false.png
+            :alt: Data App main page
+
+        You can create a line chart or multiline chart using numpy using `plot()`.
+
+        >>> # Numpy Arrays
+        >>> x_axis = np.array([10, 20, 30, 40, 50, 55, 60, 75, 80, 95])
+        >>> y_axis = np.array([10, 21, 34, 12, 14, -1, 15, 28, -5, 39])
+        >>> y_axis2 = np.array([43, 21, 23, -10, 2, 15, 38, 30, -30, 12])
+        >>> y_axis3 = np.array([13, 22, 15, -5, 2, 5, 18, 25, -20, 12])
+        >>>
+        >>> line_chart = app.line_chart(title="Multi linechart from numpy")
+        >>> 
+        >>> line_chart.plot(y_axis, x_axis=x_axis, label="Line 1", lane_index=0)
+        >>> line_chart.plot(y_axis2, label="Line 2", lane_index=1)
+        >>> line_chart.plot(y_axis3, label="Line 3", lane_index=2)
 
+        .. image:: /_static/linechart_img/np_multilinechart.png
+            :alt: Data App main page
+
+            
 
         .. rubric:: Bind compatibility
 
         You can bind this widget with this:
 
         .. hlist::
             :columns: 1
 
             * :func:`~shapelets.apps.DataApp.line_chart`
-            * :func:`~shapelets.apps.DataApp.view`
-            * list
-            * list[View]
-            * list[:class:`~shapelets.DataSet`]
-            * pd.Series
-            * pd.DataFrame
 
         .. rubric:: Bindable as
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
-
-            * :func:`~shapelets.apps.DataApp.line_chart`
-            * :func:`~shapelets.apps.DataApp.view`
-            * list
-            * list[View]
-            * list[:class:`~shapelets.DataSet`]
-            * pd.Series
-            * pd.DataFrame                
+        *Currently this widget cannot be used as input in a binding function.*  
         """
         return LineChartWidget(
             data,
             title,
             views,
             temporal_context,
             filtering_context,
@@ -1326,32 +1343,27 @@
         .. rubric:: Bindable as 
 
         You can bind this widget as: 
 
         .. hlist::
             :columns: 1
 
-            * str
-            * int
-            * float
-            * list
-            * :func:`~shapelets.apps.DataApp.selector`
+            * tuple
         """
         return SelectorWidget(options=options, title=title, placeholder=placeholder, default=default,
                               allow_multi_selection=allow_multi_selection, width=width, parent_data_app=self,
                               **additional)
 
     def radio_group(self,
-                    options: List = None,
-                    title: str = None,
-                    label_by: str = None,
-                    value_by: str = None,
-                    value: Union[int, float, str, any] = None,
+                    options: Optional[List[Union[int, float, str]]] = None,
+                    title: Optional[str] = None,
+                    label_by: Optional[str] = None,
+                    value_by: Optional[str] = None,
+                    value: Optional[List[Union[int, float, str, any]]] = None,
                     style: Literal["radio", "button"] = None,
-                    allow_multi_selection: Optional[bool] = None,
                     **additional: object) -> RadioGroupWidget:
         """
         Creates a radio button group for displaying multiple choices and allows to select one value out of a set.
 
         Parameters
         ----------
         options :list, optional
@@ -1362,23 +1374,20 @@
 
         label_by : str, optional
             Selects key to use as label.
 
         value_by : str, optional
             Selects key to use as value.
 
-        value : int, float, str or any, optional
+        value : int, float or str, optional
             Default value.
 
         style : "radio" or "button" , optional
             Radio Group style.
 
-        allow_multi_selection : bool, optional
-            Allows selecting multiple values.
-
         Returns
         -------
         RadioGroup
 
         Examples
         --------
         >>> radiogroup1 = app.radio_group([1, 2, 3], value=2)
@@ -1410,19 +1419,17 @@
 
         .. hlist::
             :columns: 1
 
             * str
             * int
             * float
-            * list
-            * :func:`~shapelets.apps.DataApp.radio_group`
 
         """
-        return RadioGroupWidget(options, title, label_by, value_by, value, style, allow_multi_selection,
+        return RadioGroupWidget(options, title, label_by, value_by, value, style,
                                 parent_data_app=self, **additional)
 
     # def bar_chart(self,
     #               data: Union[List[int], List[float], NDArray, Node],
     #               categories: Union[List[str], List[int], List[float], NDArray, Node] = None,
     #               name: Union[str, Node] = None,
     #               title: Union[str, Node] = None,
@@ -1619,15 +1626,14 @@
 
         You can bind this widget as: 
 
         .. hlist::
             :columns: 1
 
             * bool
-            * :func:`~shapelets.apps.DataApp.checkbox`
 
         """
         return CheckboxWidget(title=title, checked=checked, toggle=toggle, parent_data_app=self, **additional)
 
     def text(self,
              value: Optional[Union[str, int, float]] = None,
              title: Optional[str] = None,
@@ -1779,21 +1785,15 @@
             * list
             * :func:`~shapelets.apps.DataApp.table`
 
         .. rubric:: Bindable as 
 
         You can bind this widget as: 
 
-        .. hlist::
-            :columns: 1
-
-            * Shapelets Dataset
-            * Pandas DataFrame
-            * list
-            * :func:`~shapelets.apps.DataApp.table`
+        *Currently this widget cannot be used as input in a binding function.*  
 
         """
         return TableWidget(data=data, rows_per_page=rows_per_page, tools_visible=tools_visible,
                            conditional_formats=conditional_formats, parent_data_app=self, date_format=date_format,
                            **additional)
 
     def gauge(self,
@@ -1805,23 +1805,23 @@
 
         Parameters
         ----------
         title : str, optional
             Text associated to the Gauge.
 
         value : int, float, optional
-            Param to indicate the value of the widget
+            Param to indicate the value of the widget. Must be between [0,1], cause 1 equals 100%. 
 
         Returns
         -------
         Gauge.
 
         Examples
         --------
-        >>> gauge = app.gauge(title='Title', value=25)
+        >>> gauge = app.gauge(title='Title', value=0.25)
 
         .. rubric:: Bind compatibility
 
         You can bind this widget with this:
 
         .. hlist::
             :columns: 1
@@ -1836,15 +1836,14 @@
 
         .. hlist::
             :columns: 1
 
             * int
             * float
             * string
-            * :func:`~shapelets.apps.DataApp.gauge`
 
         """
         return GaugeWidget(title=title, value=value,
                            parent_data_app=self, **additional)
 
     def metric(self,
                title: Optional[str] = None,
@@ -1899,15 +1898,14 @@
 
         .. hlist::
             :columns: 1
 
             * str
             * int
             * float
-            * :func:`~shapelets.apps.DataApp.metric`
 
             """
         return MetricWidget(title=title, value=value, unit=unit, delta=delta, align=align,
                             parent_data_app=self, **additional)
 
     def ring(self,
              title: Optional[str] = None,
@@ -1953,15 +1951,14 @@
 
         .. hlist::
             :columns: 1
 
             * int
             * float
             * string
-            * :func:`~shapelets.apps.DataApp.ring`
 
             """
 
         return RingWidget(title=title, value=value, color=color,
                           parent_data_app=self, **additional)
 
     def place(self, widget: Widget, *args, **kwargs):
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/data_app_utils.py` & `shapelets-platform-2.0.95/src/shapelets/apps/data_app_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/attribute_names.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/attribute_names.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/altair_chart.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/altair_chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import uuid
 
 from dataclasses import dataclass
-from typing import Optional, Tuple
+from typing import Optional
 
 from ..widget import Widget, AttributeNames, StateControl
 
 
 @dataclass
 class AltairChart(StateControl):
     """
@@ -44,22 +44,23 @@
 
         * :func:`~shapelets.apps.DataApp.altair_chart`
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
-    .. hlist::
-        :columns: 1
-
-        * :func:`~shapelets.apps.DataApp.altair_chart`           
+    *Currently this widget cannot be used as input in a binding function.*        
     """
     title: Optional[str] = None
     chart: any = None
 
+    def __post_init__(self):
+        if not hasattr(self, "widget_id"):
+            self.widget_id = str(uuid.uuid1())
+
     def replace_widget(self, new_widget: AltairChart):
         """
         Replace the current values of the widget for the values of a similar widget type.
         """
         self.title = new_widget.title
         self.chart = new_widget.chart
 
@@ -70,15 +71,15 @@
         if self.chart is not None:
             return self.chart
         return None
 
     def to_dict_widget(self, alt_dict: dict = None):
         if alt_dict is None:
             alt_dict = {
-                AttributeNames.ID.value: str(uuid.uuid1()),
+                AttributeNames.ID.value: self.widget_id,
                 AttributeNames.TYPE.value: AltairChart.__name__,
                 AttributeNames.DRAGGABLE.value: self.draggable,
                 AttributeNames.RESIZABLE.value: self.resizable,
                 AttributeNames.DISABLED.value: self.disabled,
                 AttributeNames.PROPERTIES.value: {}
             }
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/bar_chart.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/folium_chart.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/folium_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,18 +38,15 @@
 
         * :func:`~shapelets.apps.DataApp.folium_chart`
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
-    .. hlist::
-        :columns: 1
-
-        * :func:`~shapelets.apps.DataApp.folium_chart`                
+    *Currently this widget cannot be used as input in a binding function.*              
     """
 
     title: Optional[str] = None
     folium: any = None
 
     def to_dict_widget(self, folium_dict: dict = None):
         if folium_dict is None:
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/heatmap.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/heatmap.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/histogram.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/histogram.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/line_chart.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/line_chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,46 +103,59 @@
 
     Returns
     -------
     LineChart
 
     Examples
     --------
-    >>> line_chart1 = app.line_chart(title='My line Chart', data=sdf) 
+    You can create a line chart using this:
 
+    >>> line_chart = app.line_chart(title="Linechart", data=df)
+
+    .. image:: /_static/linechart_img/linechart_default.png
+        :alt: Data App main page
+
+    By default `multi_lane=True`, so if your dataframe have more than one time series will plot in a separated lanes. You can set it to `False` you can get a line chart with only one line.
+
+    >>> line_chart = app.line_chart(title="Linechart", data=df, multi_lane=False)
+
+    .. image:: /_static/linechart_img/linechart_multilane_false.png
+        :alt: Data App main page
+
+    You can create a line chart or multiline chart using numpy using `plot()`.
+
+    >>> # Numpy Arrays
+    >>> x_axis = np.array([10, 20, 30, 40, 50, 55, 60, 75, 80, 95])
+    >>> y_axis = np.array([10, 21, 34, 12, 14, -1, 15, 28, -5, 39])
+    >>> y_axis2 = np.array([43, 21, 23, -10, 2, 15, 38, 30, -30, 12])
+    >>> y_axis3 = np.array([13, 22, 15, -5, 2, 5, 18, 25, -20, 12])
+    >>>
+    >>> line_chart = app.line_chart(title="Multi linechart from numpy")
+    >>> 
+    >>> line_chart.plot(y_axis, x_axis=x_axis, label="Line 1", lane_index=0)
+    >>> line_chart.plot(y_axis2, label="Line 2", lane_index=1)
+    >>> line_chart.plot(y_axis3, label="Line 3", lane_index=2)
+
+    .. image:: /_static/linechart_img/np_multilinechart.png
+        :alt: Data App main page
 
     .. rubric:: Bind compatibility
 
     You can bind this widget with this: 
 
     .. hlist::
         :columns: 1
 
         * :func:`~shapelets.apps.DataApp.line_chart`
-        * :func:`~shapelets.apps.DataApp.view`
-        * list
-        * list[View]
-        * list[:class:`~shapelets.DataSet`]
-        * pd.Series
-        * pd.DataFrame
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
-    .. hlist::
-        :columns: 1
-
-        * :func:`~shapelets.apps.DataApp.line_chart`
-        * :func:`~shapelets.apps.DataApp.view`
-        * list
-        * list[View]
-        * list[:class:`~shapelets.DataSet`]
-        * pd.Series
-        * pd.DataFrame                
+    *Currently this widget cannot be used as input in a binding function.*                
     """
 
     data: Optional[LineChartValueType] = None
     title: Optional[str] = None
     views: Optional[List[View]] = field(default_factory=lambda: [])
     temporal_context: Optional[TemporalContext] = None
     filtering_context: Optional[FilteringContext] = None
@@ -381,15 +394,15 @@
                 })
         if self.sequence is None:
             self._plots.append(plot_dict)
 
     def to_dict_widget(self, line_chart_dict: dict = None):
         if line_chart_dict is None:
             line_chart_dict = {
-                AttributeNames.ID.value: str(uuid.uuid1()),
+                AttributeNames.ID.value: self.widget_id,
                 AttributeNames.TYPE.value: LineChart.__name__,
                 AttributeNames.DRAGGABLE.value: self.draggable,
                 AttributeNames.RESIZABLE.value: self.resizable,
                 AttributeNames.DISABLED.value: self.disabled,
                 AttributeNames.PROPERTIES.value: {}
             }
         if self.title is not None:
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/pie_chart.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/plotly_chart.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/polar_area.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/polar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/radar_area.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/radar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/charts/scatter_plot.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/charts/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/filtering_context.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/filtering_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/metadata_field.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_field.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/metadata_filter.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/metadata_filter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/contexts/temporal_context.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/contexts/temporal_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/button.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     >>> button = app.button("Press me") 
 
     You can bind this widget with this:
 
         .. hlist::
             :columns: 1
 
+            * str
             * :func:`~shapelets.apps.DataApp.button`
 
     Note: bind function will change button text.
 
     """
 
     def __init__(self,
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/checkbox.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 
     You can bind this widget as: 
 
     .. hlist::
         :columns: 1
 
         * bool
-        * :func:`~shapelets.apps.DataApp.checkbox`
-
+        
     """
 
     title: Optional[str] = None
     checked: Optional[bool] = None
     toggle: Optional[bool] = None
 
     def __post_init__(self):
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/collection_selector.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/collection_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/datetime_range_selector.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_range_selector.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,52 +36,56 @@
     -------
     DatetimeRangeSelectorWidget
 
     Examples
     --------
     >>> date_selector = app.datetime_range_selector()
 
-    >>> # Create sample dates using datetime
-    >>> start_date = datetime.date(2021, 1, 17)
-    >>> end_date = datetime.date(2022, 1, 28)
-    >>> min_date = datetime.date(2018, 1, 17)
-    >>> max_date = datetime.date(2023, 1, 28)
-    >>> # Create selector based on datetime objects
-    >>> dateSelector1 = app.datetime_range_selector("selector from datetime", 
-    >>>     start_datetime=start_date, 
-    >>>     end_datetime=end_date, 
-    >>>     min_datetime=min_date, 
-    >>>     max_datetime=max_date)
+    >>> # Datetime range selector with int
+    >>> dt = app.datetime_range_selector(start_datetime=1667468964,
+    >>>                                 end_datetime=1667468964,
+    >>>                                 min_datetime=1667468964,
+    >>>                                 max_datetime=1667468964)
+
+    >>> # Datetime range selector with date
+    >>> dt = app.datetime_range_selector(start_datetime=date(year=2022, month=11, day=1),
+    >>>                                 end_datetime=date(year=2022, month=11, day=10),
+    >>>                                 min_datetime=date(year=1950, month=1, day=1),
+    >>>                                 max_datetime=date(year=2050, month=1, day=1))
+
+    >>> # Datetime range selector with datetime
+    >>> dt = app.datetime_range_selector(start_datetime=datetime(year=2022, month=11, day=1, hour=21),
+    >>>                                 end_datetime=datetime(year=2022, month=11, day=10, hour=19, second=5),
+    >>>                                 min_datetime=date(year=1950, month=1, day=1),
+    >>>                                 max_datetime=date(year=2050, month=1, day=1))
+
+    >>> # Datetime range selector with string
+    >>> dt = app.datetime_range_selector(start_datetime='2022-01-01 00:05:00',
+    >>>                                 end_datetime='2022-12-31 23:59:59',
+    >>>                                 min_datetime='1955-01-01',
+    >>>                                 max_datetime='2100-01-01')
 
 
     .. rubric:: Bind compatibility
 
     You can bind this widget with this: 
 
     .. hlist::
         :columns: 1
 
-        * str
-        * int
         * :func:`~shapelets.apps.DataApp.datetime_range_selector`
-        * datetime.datetime
-        * datetime.date
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
     .. hlist::
         :columns: 1
 
-        * str
-        * int
-        * :func:`~shapelets.apps.DataApp.datetime_range_selector`
-        * datetime.datetime
-        * datetime.date
+        * tuple
     """
     title: Optional[str] = None
     start_datetime: Optional[Union[float, int, str, datetime, date, time]] = None
     end_datetime: Optional[Union[float, int, str, datetime, date, time]] = None
     min_datetime: Optional[Union[float, int, str, date]] = None
     max_datetime: Optional[Union[float, int, str, date]] = None
     _format: Optional[str] = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/datetime_selector.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/datetime_selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,18 +34,31 @@
     -------
     DateSelectorWidget
 
     Examples
     --------
     >>> date_selector = app.datetime_selector()
 
-    >>> date = datetime.date(2022, 10, 17)
-    >>> date1 = datetime.date(2009, 10, 8)
-    >>> date2 = datetime.date(2029, 10, 27)
-    >>> date_selector = app.datetime_selector("Date only", date, date1, date2)
+    >>> # Datetime selector with int
+    >>> dt = app.datetime_selector(date_time=1667468964,
+    >>>                             min_date=1667460964,
+    >>>                             max_date=1676913679)
+
+    >>> # Datetime selector with datetime
+    >>> dt = app.datetime_selector(date_time=datetime(year=2022, month=1, day=1, hour=18, minute=20))
+
+    >>> # Datetime selector with date
+    >>> dt = app.datetime_selector(date_time=date(year=2022, month=1, day=1),
+    >>>                             min_date=date(year=1950, month=1, day=1),
+    >>>                             max_date=date(year=2050, month=1, day=1))
+
+    >>> # Datetime selector with strings
+    >>> dt = app.datetime_selector(date_time='1970-01-01',
+    >>>                             min_date='1955-01-01',
+    >>>                             max_date='2100-01-01')
 
 
     .. rubric:: Bind compatibility
 
     You can bind this widget with this: 
 
     .. hlist::
@@ -61,18 +74,14 @@
 
     You can bind this widget as: 
 
     .. hlist::
         :columns: 1
 
         * str
-        * int
-        * :func:`~shapelets.apps.DataApp.datetime_selector`
-        * datetime.datetime
-        * datetime.date
     """
     title: Optional[str] = None
     date_time: Optional[Union[float, int, str, datetime, date, time]] = None
     min_date: Optional[Union[float, int, str, date]] = None
     max_date: Optional[Union[float, int, str, date]] = None
     _format: Optional[str] = None
     _date_time_str = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/gauge.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/gauge.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
     Parameters
     ----------
     title : str, optional
         Text associated to the Gauge.
 
     value : int, float, optional
-        Param to indicate the value of the widget
+        Param to indicate the value of the widget. Must be between [0,1], cause 1 equals 100%. 
 
 
     Returns
     -------
     Gauge.
 
     Examples
     --------
-    >>> gauge = app.gauge(title='Title', value=25)
+    >>> gauge = app.gauge(title='Title', value=0.25)
 
     .. rubric:: Bind compatibility
 
     You can bind this widget with this: 
 
     .. hlist::
         :columns: 1
@@ -47,15 +47,14 @@
 
     .. hlist::
         :columns: 1
 
         * int
         * float
         * string
-        * :func:`~shapelets.apps.DataApp.gauge`
 
     """
 
     title: Optional[str] = None
     value: Optional[Union[int, float]] = None
 
     def __post_init__(self):
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/image.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,22 +50,15 @@
         * :func:`~shapelets.apps.DataApp.figure`
         * :func:`~shapelets.apps.DataApp.image`   
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
-    .. hlist::
-        :columns: 1
-
-        * str
-        * bytes
-        * :func:`~shapelets.apps.DataApp.path`
-        * :func:`~shapelets.apps.DataApp.figure`
-        * :func:`~shapelets.apps.DataApp.image`                 
+    *Currently this widget cannot be used as input in a binding function.*               
 
     """
     img: Optional[Union[str, bytes, Path, Figure]] = None
     caption: Optional[str] = None
     placeholder: Optional[Union[str, bytes, Path]] = None
 
     def __post_init__(self):
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/list.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/metric.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 
     .. hlist::
         :columns: 1
 
         * str
         * int
         * float
-        * :func:`~shapelets.apps.DataApp.metric`
 
     """
 
     title: Optional[str] = None
     value: Optional[str] = None
     unit: Optional[str] = None
     delta: Optional[str] = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/number_input.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/number_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     You can bind this widget as:
 
     .. hlist::
         :columns: 1
 
         * int
         * float
-        * :func:`~shapelets.apps.DataApp.number_input`
 
     """
     title: Optional[str] = None
     value: Optional[Union[int, float]] = None
     default_value: Optional[Union[int, float]] = None
     placeholder: Optional[str] = None
     min: Optional[Union[int, float]] = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/progress.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/progress.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/radio_group.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/radio_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 
     label_by : str, optional
         Selects key to use as label.
 
     value_by : str, optional
         Selects key to use as value.
 
-    value : int, float, str or any, optional
+    value : int, float or str, optional
         Default value.
 
-    allow_multi_selection : bool, optional
-        Allows selecting multiple values.
+    style : "radio" or "button" , optional
+        Radio Group style.
 
     Returns
     -------
     RadioGroup
 
     Examples
     --------
     >>> radiogroup1 = app.radio_group([1, 2, 3], value=2)
 
     >>> # Radio group with dict values, index_by, label_by and value_by property
     >>> radiogroup2 = app.radio_group(
-    >>>     [{"id": 1, "label": "world", "value": "bar"}, 
+    >>>     [{"id": 1, "label": "world", "value": "bar"},
     >>>     {"id": 2, "label": "moon", "value": "baz"}],
     >>>     label_by="label",
     >>>     value_by="value")
 
 
     .. rubric:: Bind compatibility
 
@@ -69,25 +69,22 @@
 
     .. hlist::
         :columns: 1
 
         * str
         * int
         * float
-        * list
-        * :func:`~shapelets.apps.DataApp.radio_group`
 
     """
-    options: Optional[List[Union[int, float, str, any]]] = None
+    options: Optional[List[Union[int, float, str]]] = None
     title: Optional[str] = None
     label_by: Optional[str] = None
     value_by: Optional[str] = None
     value: Optional[List[Union[int, float, str, any]]] = None
     style: Literal["radio", "button"] = None
-    allow_multi_selection: Optional[bool] = None
 
     def __post_init__(self):
         if not hasattr(self, "widget_id"):
             self.widget_id = str(uuid.uuid1())
         # Check value is inside options
         self._check_value()
 
@@ -102,15 +99,14 @@
         Replace the current values of the widget for the values of a similar widget type.
         """
         self.options = new_widget.options
         self.title = new_widget.title
         self.label_by = new_widget.label_by
         self.value_by = new_widget.value_by
         self.value = new_widget.value
-        self.allow_multi_selection = new_widget.allow_multi_selection
 
     def get_current_value(self):
         """
         Return the current value of the widget. Return None is the widget value is not set.
         """
         if self.value is not None:
             return self.value
@@ -137,15 +133,14 @@
         return self
 
     def to_float(self) -> float:
         return float(self.value[0])
 
     def from_list(self, input_list: List) -> RadioGroup:
         self.value = input_list
-        self.allow_multi_selection = True
         self._check_value()
         return self
 
     def to_list(self) -> List:
         return list(self.value)
 
     def _check_value(self):
@@ -226,51 +221,40 @@
                 })
 
         if self.style is not None:
             radio_dict[AttributeNames.PROPERTIES.value].update({
                 AttributeNames.TYPE.value: self.style,
             })
 
-        if self.allow_multi_selection is not None:
-            if isinstance(self.allow_multi_selection, bool):
-                radio_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.ALLOW_MULTI_SELECTION.value: self.allow_multi_selection,
-                })
-            else:
-                raise ValueError(
-                    f"Error Widget {self.widget_type}: allow_multi_selection value should be a string or another widget")
-
         if _widget_providers:
             self.add_widget_providers(radio_dict, _widget_providers)
 
         return radio_dict
 
 
 class RadioGroupWidget(Widget, RadioGroup):
 
     def __init__(self,
-                 options: List = None,
-                 title: str = None,
-                 label_by: str = None,
-                 value_by: str = None,
-                 value: Union[int, float, str, any] = None,
+                 options: Optional[List[Union[int, float, str]]] = None,
+                 title: Optional[str] = None,
+                 label_by: Optional[str] = None,
+                 value_by: Optional[str] = None,
+                 value: Optional[List[Union[int, float, str, any]]] = None,
                  style: Literal["radio", "button"] = None,
-                 allow_multi_selection: Optional[bool] = None,
                  **additional):
         Widget.__init__(self, RadioGroup.__name__,
                         compatibility=tuple([str.__name__, int.__name__, float.__name__, list.__name__,
                                              List._name, RadioGroup.__name__]),
                         **additional)
         RadioGroup.__init__(self,
                             options=options,
                             title=title,
                             label_by=label_by,
                             value_by=value_by,
                             value=value,
-                            style=style,
-                            allow_multi_selection=allow_multi_selection)
+                            style=style)
         self._parent_class = self.widget_type = RadioGroup.__name__
 
     def to_dict_widget(self):
         radio_dict = Widget.to_dict_widget(self)
         radio_dict = RadioGroup.to_dict_widget(self, radio_dict)
         return radio_dict
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/ring.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/ring.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
     .. hlist::
         :columns: 1
 
         * int
         * float
         * string
-        * :func:`~shapelets.apps.DataApp.ring`
 
     """
 
     title: Optional[str] = None
     value: Optional[Union[int, float]] = None
     color: Optional[str] = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/selector.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,15 @@
     .. rubric:: Bindable as 
 
     You can bind this widget as: 
 
     .. hlist::
         :columns: 1
 
-        * str
-        * int
-        * float
-        * list
-        * :func:`~shapelets.apps.DataApp.selector`
+        * tuple
     """
 
     options: Optional[List[Union[int, float, str]]] = None
     title: Optional[str] = None
     placeholder: Optional[str] = None
     default: Optional[Union[str, int, float]] = None
     allow_multi_selection: Optional[bool] = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/sequence_list.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/sequence_list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/sequence_selector.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/slider.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,30 +51,36 @@
     .. rubric:: Bind compatibility
 
     You can bind this widget with this: 
 
     .. hlist::
         :columns: 1
 
-        * :func:`~shapelets.apps.DataApp.slider`
         * int
         * float
         * list
+        * :func:`~shapelets.apps.DataApp.slider`
+
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
+    If you are using `range=False`
     .. hlist::
         :columns: 1
 
-        * :func:`~shapelets.apps.DataApp.slider`
         * int
         * float
-        * list
+
+    If you are using `range=True`
+    .. hlist::
+        :columns: 1
+
+        * tuple 
     """
     title: str = None
     value: Union[str, int, float, List[int], List[float], List[str]] = None
     min_value: Union[int, float] = None
     max_value: Union[int, float] = None
     step: Union[int, float] = None
     range: Optional[bool] = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/table.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/table.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/text.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/text_input.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/text_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     You can bind this widget as: 
 
     .. hlist::
         :columns: 1
 
         * str
         * int
-        * :func:`~shapelets.apps.DataApp.text_input`
     """
     value: Optional[Union[str, int, float]] = None
     title: Optional[str] = None
     text_style: Optional[dict] = None
     markdown: Optional[bool] = None
     placeholder: Optional[str] = None
     multiline: Optional[bool] = None
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/controllers/timer.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/controllers/timer.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/datetime_utils.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/grid_layout.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/horizontal_layout.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/horizontal_layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,18 +47,15 @@
 
         * :func:`~shapelets.apps.DataApp.horizontal_layout`
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
-    .. hlist::
-        :columns: 1
-
-        * :func:`~shapelets.apps.DataApp.horizontal_layout`              
+    *Currently this widget cannot be used as input in a binding function.*                
     """
 
     placements: dict = field(default_factory=lambda: {})
     horizontal_align: Optional[Literal["start", "center", "end"]] = "start"
     vertical_align: Optional[Literal["start", "center", "end"]] = "start"
 
     def place(self, widget: Widget, width: Optional[float] = None, offset: Optional[int] = None):
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/panel.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/panel.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/tabs_layout.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/tabs_layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,18 +44,15 @@
 
         * :func:`~shapelets.apps.DataApp.tabs_layout`
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
-    .. hlist::
-        :columns: 1
-
-        * :func:`~shapelets.apps.DataApp.tabs_layout`               
+    *Currently this widget cannot be used as input in a binding function.*              
     """
 
     tabs: Optional[Tuple[str, StateControl]] = field(default_factory=lambda: [])
     position: Optional[Literal["top", "bottom" "left", "right"]] = "bottom"
 
     def add_tab(self, tab_title: str, component: StateControl) -> TabsLayout:
         if self.tabs is None:
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/layouts/vertical_layout.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/layouts/vertical_layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,18 +45,15 @@
 
         * :func:`~shapelets.apps.DataApp.vertical_layout`
 
     .. rubric:: Bindable as
 
     You can bind this widget as: 
 
-    .. hlist::
-        :columns: 1
-
-        * :func:`~shapelets.apps.DataApp.vertical_layout`         
+    *Currently this widget cannot be used as input in a binding function.*     
     """
     placements: dict = field(default_factory=lambda: {})
     vertical_align: Literal["start", "center", "end"] = "start"
 
     def place(self, widget: Widget, width: Optional[float] = None, offset: Optional[int] = None):
         """
         Place widget inside layout
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/util.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/util.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/apps/widgets/widget.py` & `shapelets-platform-2.0.95/src/shapelets/apps/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/functions.py` & `shapelets-platform-2.0.95/src/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/iris.csv` & `shapelets-platform-2.0.95/src/shapelets/iris.csv`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/model/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/altair.py` & `shapelets-platform-2.0.95/src/shapelets/model/altair.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/capsule.py` & `shapelets-platform-2.0.95/src/shapelets/model/capsule.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/collection.py` & `shapelets-platform-2.0.95/src/shapelets/model/collection.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/dataframe.py` & `shapelets-platform-2.0.95/src/shapelets/model/dataframe.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/function_description.py` & `shapelets-platform-2.0.95/src/shapelets/model/function_description.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/function_parameter.py` & `shapelets-platform-2.0.95/src/shapelets/model/function_parameter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/group.py` & `shapelets-platform-2.0.95/src/shapelets/model/group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/image.py` & `shapelets-platform-2.0.95/src/shapelets/model/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/metadata_item.py` & `shapelets-platform-2.0.95/src/shapelets/model/metadata_item.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/model.py` & `shapelets-platform-2.0.95/src/shapelets/model/model.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/ndarray.py` & `shapelets-platform-2.0.95/src/shapelets/model/ndarray.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/permissions.py` & `shapelets-platform-2.0.95/src/shapelets/model/permissions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/replicated_param.py` & `shapelets-platform-2.0.95/src/shapelets/model/replicated_param.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/sequence.py` & `shapelets-platform-2.0.95/src/shapelets/model/sequence.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/sequence_axis.py` & `shapelets-platform-2.0.95/src/shapelets/model/sequence_axis.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/user.py` & `shapelets-platform-2.0.95/src/shapelets/model/user.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/model/view_match.py` & `shapelets-platform-2.0.95/src/shapelets/model/view_match.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/app.py` & `shapelets-platform-2.0.95/src/shapelets/svr/app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/authn/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/authn/authhttp.py` & `shapelets-platform-2.0.95/src/shapelets/svr/authn/authhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/authn/authrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/authn/authrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/authn/authservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/authn/authservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/authn/gc_client.py` & `shapelets-platform-2.0.95/src/shapelets/svr/authn/gc_client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/authn/iauthrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/authn/iauthservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/authn/iauthservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/access_token_credentials.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/access_token_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/azure_gen1.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/azure_gen2.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/azure_gen2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/driver.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/driver.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/dynamic_credentials.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_config.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_config.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_vfs.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/fsspec_vfs_file.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/fsspec_vfs_file.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/ftp.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/ftp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/local.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/local.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/protocols.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/protocols.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/smb.py` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/smb.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/data/vfs/vfs_sample_config.toml` & `shapelets-platform-2.0.95/src/shapelets/svr/data/vfs/vfs_sample_config.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataapps_ws.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataapps_ws.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 
 @dataclass
 class Message:
     """
     Websocket message so the UI knows when to refresh the dataapp section
     """
     dataapp_name: str
-    major: int
-    minor: int
+    dataapp_id: str
+    user_id: str
     is_delete: bool
+    major: int = None
+    minor: int = None
 
     def to_string(self, root_panel_dataapp: str = None) -> str:
         """
         UI expects message in specific formats:
-        - *:delete:NAME:dataapp_name:VERSION:0.9 -> when a dataapp must be removed from the dataapp section
-        - *:NAME:dataapp_name:VERSION:0.9 -> when a dataapp must be added to the dataapp section
+        - *:delete:NAME:{dataapp_name}:VERSION:{major}.{minor} -> when a dataapp must be removed from the dataapp section
+        - *:NAME:{dataapp_id} -> when a dataapp must be added to the dataapp section
         """
         if root_panel_dataapp is not None:
             if self.is_delete:
-                return f"{root_panel_dataapp}:delete:NAME:{self.dataapp_name}:VERSION:{self.major}.{self.minor}"
-            return f"{root_panel_dataapp}:NAME:{self.dataapp_name}:VERSION:{self.major}.{self.minor}"
+                return f"{root_panel_dataapp}:delete:NAME:{self.dataapp_name}:USER:{self.user_id}:VERSION:{self.major}.{self.minor}"
+            return f"{root_panel_dataapp}:NAME:{self.dataapp_id}:USER:{self.user_id}"
         else:
             if self.is_delete:
-                return f"{self.dataapp_name}:delete:VERSION:{self.major}.{self.minor}"
-            return f"NAME:{self.dataapp_name}:VERSION:{self.major}.{self.minor}"
+                return f"{self.dataapp_name}:delete:USER:{self.user_id}:VERSION:{self.major}.{self.minor}"
+            return f"NAME:{self.dataapp_id}:USER:{self.user_id}"
 
 
 @dataclass
 class DataAppChangeListeners:
     ROOT_PANEL_DATA_APP = "*"
     by_app_name = {}
     listener_to_app_name = {}
@@ -39,27 +41,27 @@
         Add listener route to the class.
         """
         listener_ws = self.by_app_name.get(dataapp_name)
         if not listener_ws:
             self.by_app_name[dataapp_name] = listener
         self.listener_to_app_name[listener] = dataapp_name
 
-    async def notify(self, dataapp_name: str, major: int, minor: int, is_delete: bool):
+    async def notify(self, dataapp_name: str, dataapp_id: str, user_id: str, is_delete: bool, major: int = None, minor: int = None):
         """
         Server notifies that there is change in a dataapp, either created or deleted.
         """
         change_listeners = self.by_app_name.get(dataapp_name)
         if change_listeners:
-            message = Message(dataapp_name, major, minor, is_delete)
+            message = Message(dataapp_name, dataapp_id, user_id, is_delete, major, minor)
             sent = await self.send(message.to_string(), change_listeners)
             if not sent or is_delete:
                 self.remove(change_listeners)
         root_page_listeners = self.by_app_name.get(self.ROOT_PANEL_DATA_APP)
         if root_page_listeners:
-            message = Message(dataapp_name, major, minor, is_delete)
+            message = Message(dataapp_name, dataapp_id, user_id, is_delete, major, minor)
             sent = await self.send(message.to_string(self.ROOT_PANEL_DATA_APP), root_page_listeners)
             if not sent:
                 self.remove(root_page_listeners)
 
     async def send(self, message: str, listener: WebSocket) -> bool:
         """
         Send message to client.
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataappshttp.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappshttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,42 +94,47 @@
                                                    major=attributes.value.major,
                                                    minor=attributes.value.minor,
                                                    description=attributes.value.description,
                                                    specId=attributes.value.specId,
                                                    tags=attributes.value.tags,
                                                    groups=attributes.value.groups,
                                                    userId=user_id)
-            data_app = self._svr.create(dataapp_attributes, data)
-            await self.dataapp_change_listeners.notify(data_app.name, data_app.major, data_app.minor, False)
-            return data_app
+            dataapp = self._svr.create(dataapp_attributes, data)
+            await self.dataapp_change_listeners.notify(dataapp.name, dataapp.uid, user_id, False)
+            return dataapp
         except UserDoesNotBelong as e:
             return self.bad_request(str(e))
         except InvalidGroupName as e:
             return self.bad_request(str(e))
         except WritePermission as e:
             return self.bad_request(str(e))
         except Exception as e:
             return self.status_code(500, str(e))
 
+    @get("/name/{dataAppName}")
+    async def get_dataapp_by_name(self, dataAppName: str) -> DataAppAttributes:
+        return self._svr.get_dataapp_by_name(dataAppName)
+
     @get("/{id}")
-    async def get_dataapp(self, dataAppName: str) -> DataAppAttributes:
-        return self._svr.get_dataapp(dataAppName)
+    async def get_dataapp_by_id(self, id: str) -> DataAppAttributes:
+        return self._svr.get_dataapp_by_id(id)
 
     @delete("/")
     async def delete_all(self) -> bool:
         return self._svr.delete_all()
 
     @delete("/{id}")
     async def delete(self, uid: int, user: Identity) -> bool:
         if user is None:
             raise RuntimeError(f"Unable to find user. Please, login.")
         user_id = user.claims["userId"]
         dataapp = self._svr.get_dataapp_by_id(uid)
         if self._svr.delete_dataapp(uid, user_id):
-            await self.dataapp_change_listeners.notify(dataapp.name, dataapp.major, dataapp.minor, False)
+            await self.dataapp_change_listeners.notify(dataapp.name, dataapp.uid, user_id, True, dataapp.major,
+                                                       dataapp.minor)
             return self.ok("DataApp removed successfully.")
         return self.bad_request()
 
     @get("/{id}/privileges")
     async def get_dataapp_privileges(self, dataapp_id: int) -> List[DataAppAttributes]:
         return self._svr.get_dataapp_privileges(dataapp_id)
 
@@ -182,16 +187,19 @@
         if dataapp._data:
             params = [("data", dataapp._data)]
         response = self.session.post('/api/dataapps/', json=json.loads(payload.json()), params=params)
         if response.status_code != 200:
             raise RuntimeError(response.content)
         return response
 
-    def get_dataapp(self, dataAppName: str) -> DataAppAttributes:
-        return self.session.get('/api/dataapps/', params=[("dataAppName", dataAppName)])
+    def get_dataapp_by_name(self, dataAppName: str) -> DataAppAttributes:
+        return self.session.get('/api/dataapps/name/', params=[("dataAppName", dataAppName)])
+
+    def get_dataapp_by_id(self, id: str) -> DataAppAttributes:
+        return self.session.get('/api/dataapps/', params=[("id", id)])
 
     def delete_dataapp(self, uid: int):
         self.session.delete('/api/dataapps/{id}', params=[("uid", uid)])
 
     def delete_all(self) -> bool:
         self.session.delete('/api/dataapps/')
         return True
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataappsrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/dataappsservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/dataappsservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def user_group_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
         return self._dataapp_repo.user_group_dataapp_list(user_id)
 
     def create(self, attributes: DataAppAttributes, data: List[str] = None) -> DataAppProfile:
         return self._dataapp_repo.create(attributes, data)
 
-    def get_dataapp(self, dataapp_name: str):
+    def get_dataapp_by_name(self, dataapp_name: str):
         return self._dataapp_repo.load_by_name(dataapp_name)
 
     def get_dataapp_by_id(self, uid: int) -> DataAppProfile:
         return self._dataapp_repo.load_by_id(uid)
 
     def delete_dataapp(self, uid: int, user_id: int) -> bool:
         return self._dataapp_repo.delete_dataapp(uid, user_id)
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/http_docs.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/idataappsrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/dataapps/idataappsservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/dataapps/idataappsservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         pass
 
     @abstractmethod
     def create(self, attributes: DataAppAttributes, data: List[str] = None) -> DataAppProfile:
         pass
 
     @abstractmethod
-    def get_dataapp(self, dataapp_name: str) -> DataAppProfile:
+    def get_dataapp_by_name(self, dataapp_name: str) -> DataAppProfile:
         pass
 
     @abstractmethod
     def get_dataapp_by_id(self, uid: int) -> DataAppProfile:
         pass
 
     @abstractmethod
```

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/native/database.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/native/database.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/native/settings.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/native/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/schema_builder.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_builder.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v1.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v2.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v3.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v3.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/schema_v4.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/schema_v4.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/db/setup.py` & `shapelets-platform-2.0.95/src/shapelets/svr/db/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/execution/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/execution/executionhttp.py` & `shapelets-platform-2.0.95/src/shapelets/svr/execution/executionhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/execution/executionservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/execution/executionservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/execution/http_docs.py` & `shapelets-platform-2.0.95/src/shapelets/svr/execution/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/groups/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/groups/groupservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/groups/groupservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/groups/groupshttp.py` & `shapelets-platform-2.0.95/src/shapelets/svr/groups/groupshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/groups/groupsrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/groups/groupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/groups/igroupsrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/groups/igroupsservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/groups/igroupsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/model/dataapps.py` & `shapelets-platform-2.0.95/src/shapelets/svr/model/dataapps.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/model/principals.py` & `shapelets-platform-2.0.95/src/shapelets/svr/model/principals.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/model/users.py` & `shapelets-platform-2.0.95/src/shapelets/svr/model/users.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/asttranslation.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/asttranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/conversions.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/conversions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/core.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/core.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/decompiling.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/decompiling.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/exceptions.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/hashdict.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/hashdict.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/ormtypes.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/ormtypes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/prototypes/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/serialization.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/serialization.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/sqlbuilding.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqlbuilding.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/mustang/sqltranslation.py` & `shapelets-platform-2.0.95/src/shapelets/svr/mustang/sqltranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/server.py` & `shapelets-platform-2.0.95/src/shapelets/svr/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/client.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/defaults.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/functions.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/http.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/http.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/reload.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/reload.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/server.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/settings.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/settings.toml` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/ssl.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/ssl.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/telemetry.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/telemetry.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/settings/websocket.py` & `shapelets-platform-2.0.95/src/shapelets/svr/settings/websocket.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/telemetry/sysinfo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/telemetry/sysinfo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/telemetry/telemetryservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/telemetry/telemetryservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/users/__init__.py` & `shapelets-platform-2.0.95/src/shapelets/svr/users/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/users/http_docs.py` & `shapelets-platform-2.0.95/src/shapelets/svr/users/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/users/iusersrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/users/iusersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/users/iusersservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/users/iusersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/users/usershttp.py` & `shapelets-platform-2.0.95/src/shapelets/svr/users/usershttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/users/usersrepo.py` & `shapelets-platform-2.0.95/src/shapelets/svr/users/usersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/users/usersservice.py` & `shapelets-platform-2.0.95/src/shapelets/svr/users/usersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/utils/crypto.py` & `shapelets-platform-2.0.95/src/shapelets/svr/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/utils/flexbytes.py` & `shapelets-platform-2.0.95/src/shapelets/svr/utils/flexbytes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/altair.json` & `shapelets-platform-2.0.95/src/shapelets/svr/www/altair.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/asset-manifest.json` & `shapelets-platform-2.0.95/src/shapelets/svr/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/dataapp.json` & `shapelets-platform-2.0.95/src/shapelets/svr/www/dataapp.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/favicon.ico` & `shapelets-platform-2.0.95/src/shapelets/svr/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/index.html` & `shapelets-platform-2.0.95/src/shapelets/svr/www/index.html`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/2.379683b2.chunk.js` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/audit.cb539a06.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/audit.cb539a06.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/bin.7e762965.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/bin.7e762965.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/clear.27b15301.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/clear.27b15301.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/collections.06fdf54a.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/collections.06fdf54a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/date-time.a1e86419.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/date-time.a1e86419.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/download-image.87310709.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/download-image.87310709.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/filter.cec803b8.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/filter.cec803b8.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/logout.57c593a5.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/logout.57c593a5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/pdf.5d189efa.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/pdf.5d189efa.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/share.bc9a8370.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/share.bc9a8370.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/single-plot.864a583b.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/single-plot.864a583b.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets/svr/www/static/media/wave-top.6d51781b.png` & `shapelets-platform-2.0.95/src/shapelets/svr/www/static/media/wave-top.6d51781b.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets_platform.egg-info/PKG-INFO` & `shapelets-platform-2.0.95/src/shapelets_platform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.94
+Version: 2.0.95
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
@@ -15,24 +15,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Classifier: License :: Other/Proprietary License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: vfs-all
 Provides-Extra: vfs-azure
 Provides-Extra: vfs-dropbox
 Provides-Extra: vfs-google
```

### Comparing `shapelets-platform-2.0.94/src/shapelets_platform.egg-info/SOURCES.txt` & `shapelets-platform-2.0.95/src/shapelets_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.94/src/shapelets_platform.egg-info/requires.txt` & `shapelets-platform-2.0.95/src/shapelets_platform.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-altair~=4.2
+adlfs~=2023.4
 argparse~=1.4
 blacksheep~=1.2
-cloudpickle~=2.2
 dill~=0.3
-email-validator~=1.3
 folium~=0.13
-h11~=0.12
 jmespath~=0.9
-matplotlib~=3.5
-mypy~=0.990
-numpy~=1.25
+mypy~=1.4
+numpy~=1.24
 pandas~=2.0
 psutil~=5.9
 pyarrow~=12.0
 py-cpuinfo~=9.0
-pydantic==1.10.11
-pygeohash~=1.2
+pydantic~=1.10
 PyNaCl~=1.5
-requests~=2.28
-setuptools-scm~=7.1
-shapelets_native==2.0.94
-tabulate~=0.8
-tomlkit~=0.11
-tqdm~=4.64
+requests~=2.31
+shapelets_native==2.0.95
+tabulate~=0.9
+tomlkit~=0.12
 typing_extensions~=4.7
-uvicorn~=0.18
-vega-datasets~=0.9
+uvicorn~=0.23
 websocket-client~=1.5
 websockets~=10.3
 
 [:platform_system != "Windows"]
 lockfile~=0.12
 python_daemon>=2.3.2
 uvloop~=0.17
```

