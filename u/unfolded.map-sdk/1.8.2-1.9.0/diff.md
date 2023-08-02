# Comparing `tmp/unfolded.map-sdk-1.8.2.tar.gz` & `tmp/unfolded.map-sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfolded.map-sdk-1.8.2.tar", last modified: Fri Jun 16 21:09:44 2023, max compression
+gzip compressed data, was "unfolded.map-sdk-1.9.0.tar", last modified: Wed Aug  2 19:05:16 2023, max compression
```

## Comparing `unfolded.map-sdk-1.8.2.tar` & `unfolded.map-sdk-1.9.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.836611 unfolded.map-sdk-1.8.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    25658 2023-06-16 21:05:07.000000 unfolded.map-sdk-1.8.2/docs/source/_static/embed-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.836611 unfolded.map-sdk-1.8.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/scripts/rename_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/dataset_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/tests/fixtures/raster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/fixtures/raster/collection/
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/fixtures/raster/item/
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/raster/item/sentinel-2-l2a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/mocks/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_iframe_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_template_rendering/map.html
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_html_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_subclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_widget_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/utils/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/unfolded/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_async_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.848611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/create_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/event_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17979 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.848611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/4.2f5ebe11a5669cad3275.js
--rw-r--r--   0 runner    (1001) docker     (123)    17474 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/480.25ce0490671eeeb9f120.js
--rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/568.caff7d3d72d44ec36b9e.js
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/remoteEntry.1f1edfc58c4b1a509424.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 21:09:42.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-06-16 21:09:38.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/templates/html_map_sdk.j2
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transfer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/action_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.json
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.326027 unfolded.map-sdk-1.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.330027 unfolded.map-sdk-1.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.330027 unfolded.map-sdk-1.9.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    25660 2023-08-02 19:00:58.000000 unfolded.map-sdk-1.9.0/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.330027 unfolded.map-sdk-1.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/scripts/rename_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/api/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/api/test_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/api/test_layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/api/test_map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/fixtures/dataset_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.330027 unfolded.map-sdk-1.9.0/tests/fixtures/raster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/fixtures/raster/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/fixtures/raster/item/
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/fixtures/raster/item/sentinel-2-l2a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/fixtures/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/mocks/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.330027 unfolded.map-sdk-1.9.0/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.330027 unfolded.map-sdk-1.9.0/tests/snapshots/test_html_map/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/snapshots/test_html_map/test_iframe_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/snapshots/test_html_map/test_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/snapshots/test_html_map/test_template_rendering/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/test_html_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/test_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/test_widget_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tests/utils/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.330027 unfolded.map-sdk-1.9.0/unfolded/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.338027 unfolded.map-sdk-1.9.0/unfolded/map_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.338027 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll_v56/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll_v56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll_v56/_async_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll_v56/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll_v56/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.338027 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/create_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/event_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/4.6f3ac46f5dc719fa042d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17474 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/480.a7a86a8fcd664bad39be.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/568.69799d2e0346a48f6a67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/747.433d4b4ef3380d99e08e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/remoteEntry.ade37fd73490b31c9a45.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 19:05:14.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/unfolded/map_sdk/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26248 2023-08-02 19:05:10.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/unfolded/map_sdk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/templates/html_map_sdk.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/transfer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.342028 unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/action_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:05:16.334027 unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 19:05:16.000000 unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/unfolded.map_sdk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 18:54:34.000000 unfolded.map-sdk-1.9.0/webpack.config.js
```

### Comparing `unfolded.map-sdk-1.8.2/MANIFEST.in` & `unfolded.map-sdk-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/PKG-INFO` & `unfolded.map-sdk-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfolded.map-sdk
-Version: 1.8.2
+Version: 1.9.0
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 License: (c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `unfolded.map-sdk-1.8.2/docs/source/_static/embed-bundle.js` & `unfolded.map-sdk-1.9.0/docs/source/_static/embed-bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,17 +25,17 @@
                                     s(e)
                                 }
                             },
                             o = e => e.done ? a(e.value) : Promise.resolve(e.value).then(r, i);
                         o((n = n.apply(e, t)).next())
                     })),
                     r = ((a = r || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a),
-                    i = class extends Error {
-                        constructor(e) {
-                            super(e), Object.setPrototypeOf(this, i.prototype)
+                    i = class e extends Error {
+                        constructor(t) {
+                            super(t), Object.setPrototypeOf(this, e.prototype)
                         }
                     },
                     o = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
 
                 function d() {
                     return s(this, arguments, (function*(e = {}, t) {
                         let n, a = "https://studio.foursquare.com/studio-bundle.js";
@@ -576,15 +576,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.9.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.9.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
     function a(e) {
         var s = n[e];
         if (void 0 !== s) return s.exports;
```

### Comparing `unfolded.map-sdk-1.8.2/package.json` & `unfolded.map-sdk-1.9.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9623015873015872%*

 * *Differences: {"'dependencies'": "{'@unfolded/map-sdk': '^1.9.0'}", "'version'": "'1.9.0'"}*

```diff
@@ -5,15 +5,15 @@
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@jupyterlab/rendermime-interfaces": "^1.3.0 || ^2.0.0 || ^3.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
-        "@unfolded/map-sdk": "^1.8.2",
+        "@unfolded/map-sdk": "^1.9.0",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0",
         "global": "^4.3.0"
     },
     "description": "JavaScript bindings for Unfolded's Jupyter Map SDK",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
@@ -76,12 +76,12 @@
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "1.8.2",
+    "version": "1.9.0",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `unfolded.map-sdk-1.8.2/scripts/rename_package.py` & `unfolded.map-sdk-1.9.0/scripts/rename_package.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/setup.cfg` & `unfolded.map-sdk-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.8.2
+current_version = 1.9.0
 commit = True
 message = chore(map-sdk): Bump version {current_version} → {new_version}
 tag = False
 tag_name = map-sdk/{new_version}
 
 [bdist_wheel]
 universal = 1
@@ -28,15 +28,15 @@
 search = "version": "{current_version}",
 replace = "version": "{new_version}",
 
 [bumpversion:file:../../../modules/map-sdk-v1/package.json]
 search = "version": "{current_version}",
 replace = "version": "{new_version}",
 
-[bumpversion:file:../../../studio/map-sdk-pro/package.json]
+[bumpversion:file:../../../apps/studio/map-sdk-pro/package.json]
 search = "version": "{current_version}
 replace = "version": "{new_version}
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `unfolded.map-sdk-1.8.2/setup.py` & `unfolded.map-sdk-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/_utils.py` & `unfolded.map-sdk-1.9.0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/api/test_dataset_api.py` & `unfolded.map-sdk-1.9.0/tests/api/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/api/test_filter_api.py` & `unfolded.map-sdk-1.9.0/tests/api/test_filter_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/api/test_layer_api.py` & `unfolded.map-sdk-1.9.0/tests/api/test_layer_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/api/test_map_api.py` & `unfolded.map-sdk-1.9.0/tests/api/test_map_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/conftest.py` & `unfolded.map-sdk-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/fixtures/dataset_api.py` & `unfolded.map-sdk-1.9.0/tests/fixtures/dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json` & `unfolded.map-sdk-1.9.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/fixtures/raster/item/sentinel-2-l2a.json` & `unfolded.map-sdk-1.9.0/tests/fixtures/raster/item/sentinel-2-l2a.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/fixtures/test_data.py` & `unfolded.map-sdk-1.9.0/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/mocks/transport.py` & `unfolded.map-sdk-1.9.0/tests/mocks/transport.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html` & `unfolded.map-sdk-1.9.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_template_rendering/map.html` & `unfolded.map-sdk-1.9.0/tests/snapshots/test_html_map/test_template_rendering/map.html`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/test_html_map.py` & `unfolded.map-sdk-1.9.0/tests/test_html_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/test_serialization.py` & `unfolded.map-sdk-1.9.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/test_subclass.py` & `unfolded.map-sdk-1.9.0/tests/test_subclass.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/test_widget_map.py` & `unfolded.map-sdk-1.9.0/tests/test_widget_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tests/utils/test_validators.py` & `unfolded.map-sdk-1.9.0/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/tsconfig.json` & `unfolded.map-sdk-1.9.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/__init__.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_async_thread.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll_v56/_async_thread.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_poll.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/_poll_v56/_poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/base.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/create_map.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/create_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/dataset_api.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/enums.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/enums.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/event_api.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/event_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/filter_api.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/filter_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/layer_api.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/layer_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import sys
 from typing import Any, Callable, Dict, List, Optional, Union
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 from pydantic import StrictBool, StrictStr
 
 from unfolded.map_sdk.api.base import Action, CamelCaseBaseModel, Number, TimeRange
 from unfolded.map_sdk.api.enums import ActionType, LayerType
 from unfolded.map_sdk.transport.base import (
     BaseInteractiveTransport,
     BaseNonInteractiveTransport,
@@ -23,22 +29,32 @@
 class _PartialLayerConfig(CamelCaseBaseModel):
     visual_channels: Optional[VisualChannels]
     """Dictionary of visualization properties that the layer supports."""
 
     vis_config: Optional[Dict[StrictStr, Any]]
     """General layer settings."""
 
+    column_mode: Optional[
+        Literal["points", "geojson", "table", "neighbors", "LAT_LNG", "H3"]
+    ]
+    """Column mode for the layer (some of the layers support multiple input data formats)."""
+
 
 class LayerConfig(_PartialLayerConfig):
     visual_channels: VisualChannels
     """Dictionary of visualization properties that the layer supports."""
 
     vis_config: Dict[StrictStr, Any]
     """General layer settings."""
 
+    column_mode: Optional[
+        Literal["points", "geojson", "table", "neighbors", "LAT_LNG", "H3"]
+    ]
+    """Column mode for the layer (some of the layers support multiple input data formats)."""
+
 
 class _LayerUpdateProps(CamelCaseBaseModel):
     type: Optional[LayerType]
     """Type of the layer."""
 
     data_id: Optional[StrictStr]
     """Unique identifier of the dataset this layer visualizes."""
@@ -101,27 +117,25 @@
     """Flag indicating whether layer is visible or not."""
 
     config: LayerConfig
     """Layer configuration specific to its type."""
 
 
 class _LayerGroupUpdateProps(CamelCaseBaseModel):
-
     label: Optional[StrictStr]
     """Canonical label of this layer group."""
 
     is_visible: Optional[StrictBool]
     """Flag indicating whether layer group is visible or not."""
 
     layer_ids: Optional[List[StrictStr]]
     """Layers that are part of this group, sorted in the order in which they are shown."""
 
 
 class _LayerGroupCreationProps(_LayerGroupUpdateProps):
-
     id: Optional[StrictStr]
     """Unique identifier of the layer group."""
 
     label: Optional[StrictStr]
     """Canonical label of this layer group."""
 
     is_visible: Optional[StrictBool]
@@ -144,15 +158,14 @@
     """Flag indicating whether layer group is visible or not."""
 
     layer_ids: List[StrictStr]
     """Layers that are part of this group, sorted in the order in which they are shown."""
 
 
 class _LayerTimelineUpdateProps(CamelCaseBaseModel):
-
     current_time: Optional[Number]
     """Current time on the timeline in milliseconds."""
 
     is_animating: Optional[StrictBool]
     """Flag indicating whether the timeline is animating or not."""
 
     is_visible: Optional[StrictBool]
@@ -171,15 +184,14 @@
     """Timezone that the timeline is using in tz format.
 
     https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
     """
 
 
 class LayerTimeline(_LayerTimelineUpdateProps):
-
     current_time: Number
     """Current time on the timeline in milliseconds."""
 
     domain: TimeRange
     """Range of time that the timeline shows."""
 
     is_animating: StrictBool
@@ -250,15 +262,14 @@
         args = ["layer_id"]
 
     type: ActionType = ActionType.REMOVE_LAYER
     layer_id: StrictStr
 
 
 class GetLayerGroupsAction(Action):
-
     type: ActionType = ActionType.GET_LAYER_GROUPS
 
 
 class GetLayerGroupByIdAction(Action):
     class Meta(Action.Meta):
         args = ["layer_group_id"]
 
@@ -435,15 +446,14 @@
         )
         return self.transport.send_action_non_null(
             action=action, response_class=LayerTimeline
         )
 
 
 class BaseInteractiveLayerApiMethods:
-
     transport: BaseInteractiveTransport
 
     def get_layers(self) -> List[Layer]:
         """Gets all the layers currently available in the map.
 
         Returns:
             List[Layer]: An array of layers.
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/map_api.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/api/map_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/environment.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/package.json` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617063492063492%*

 * *Differences: {"'dependencies'": "{'@unfolded/map-sdk': '^1.9.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ade37fd73490b31c9a45.js'}}",*

 * * "'version'": "'1.9.0'"}*

```diff
@@ -5,15 +5,15 @@
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@jupyterlab/rendermime-interfaces": "^1.3.0 || ^2.0.0 || ^3.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
-        "@unfolded/map-sdk": "^1.8.2",
+        "@unfolded/map-sdk": "^1.9.0",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0",
         "global": "^4.3.0"
     },
     "description": "JavaScript bindings for Unfolded's Jupyter Map SDK",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
@@ -35,15 +35,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1f1edfc58c4b1a509424.js",
+            "load": "static/remoteEntry.ade37fd73490b31c9a45.js",
             "mimeExtension": "./mimeExtension"
         },
         "extension": "lib/plugin",
         "mimeExtension": "lib/javascript-renderer-extension.js",
         "outputDir": "unfolded/map_sdk/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
@@ -81,12 +81,12 @@
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "1.8.2",
+    "version": "1.9.0",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/4.2f5ebe11a5669cad3275.js` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/4.6f3ac46f5dc719fa042d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
                     d((o = o.apply(e, n || [])).next())
                 }))
             };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.unfoldedRendererFactory = void 0;
             const s = t(832),
-                r = t(413),
+                r = t(541),
                 i = "application/geo+json",
                 a = "text/csv",
                 d = [i, a];
             class u extends s.Widget {
                 constructor(e) {
                     super(), this.addClass("unfolded-rendermime"), this.options = e
                 }
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/480.25ce0490671eeeb9f120.js` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/480.a7a86a8fcd664bad39be.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -337,15 +337,15 @@
                     d((s = s.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
             const a = n(565),
-                i = n(413);
+                i = n(541);
             n(204);
             const r = "unfolded-widget";
             class o extends a.DOMWidgetView {
                 initialize() {
                     return s(this, void 0, void 0, (function*() {
                         const e = {
                             style: this.model.style(),
@@ -547,11 +547,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.9.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.9.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/568.caff7d3d72d44ec36b9e.js` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/568.69799d2e0346a48f6a67.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -288,15 +288,15 @@
                     d((s = s.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
             const a = n(565),
-                i = n(413);
+                i = n(541);
             n(204);
             const r = "unfolded-widget";
             class o extends a.DOMWidgetView {
                 initialize() {
                     return s(this, void 0, void 0, (function*() {
                         const e = {
                             style: this.model.style(),
@@ -498,11 +498,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.9.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.9.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/747.433d4b4ef3380d99e08e.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -22,17 +22,17 @@
                                 r(n)
                             }
                         },
                         i = n => n.done ? a(n.value) : Promise.resolve(n.value).then(s, o);
                     i((t = t.apply(n, e)).next())
                 })),
                 s = ((a = s || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a),
-                o = class extends Error {
-                    constructor(n) {
-                        super(n), Object.setPrototypeOf(this, o.prototype)
+                o = class n extends Error {
+                    constructor(e) {
+                        super(e), Object.setPrototypeOf(this, n.prototype)
                     }
                 },
                 i = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
 
             function f() {
                 return r(this, arguments, (function*(n = {}, e) {
                     let t, a = "https://studio.foursquare.com/studio-bundle.js";
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/remoteEntry.1f1edfc58c4b1a509424.js` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/remoteEntry.ade37fd73490b31c9a45.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, d, f, l, s, p, c, h, v, m, g, b = {
+    var e, r, t, n, a, o, i, u, d, l, f, s, p, c, h, v, m, b, g = {
             768: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(413), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(413), t.e(565), t.e(480)]).then((() => () => t(480))),
-                        "./mimeExtension": () => Promise.all([t.e(413), t.e(4)]).then((() => () => t(4)))
+                        "./index": () => Promise.all([t.e(541), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(541), t.e(565), t.e(480)]).then((() => () => t(480))),
+                        "./mimeExtension": () => Promise.all([t.e(541), t.e(4)]).then((() => () => t(4)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = t.S.default,
@@ -30,51 +30,51 @@
     function w(e) {
         var r = y[e];
         if (void 0 !== r) return r.exports;
         var t = y[e] = {
             id: e,
             exports: {}
         };
-        return b[e].call(t.exports, t, t.exports, w), t.exports
+        return g[e].call(t.exports, t, t.exports, w), t.exports
     }
-    w.m = b, w.c = y, w.d = (e, r) => {
+    w.m = g, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        4: "2f5ebe11a5669cad3275",
-        413: "813f632371f69f38335a",
-        480: "25ce0490671eeeb9f120",
+        4: "6f3ac46f5dc719fa042d",
+        480: "a7a86a8fcd664bad39be",
+        541: "aa25af0e7b09d04bbfc6",
         565: "6aa0248333a228f5539f",
-        568: "caff7d3d72d44ec36b9e",
-        747: "488cf0ee36d815959581"
+        568: "69799d2e0346a48f6a67",
+        747: "433d4b4ef3380d99e08e"
     } [e] + ".js?v=" + {
-        4: "2f5ebe11a5669cad3275",
-        413: "813f632371f69f38335a",
-        480: "25ce0490671eeeb9f120",
+        4: "6f3ac46f5dc719fa042d",
+        480: "a7a86a8fcd664bad39be",
+        541: "aa25af0e7b09d04bbfc6",
         565: "6aa0248333a228f5539f",
-        568: "caff7d3d72d44ec36b9e",
-        747: "488cf0ee36d815959581"
+        568: "69799d2e0346a48f6a67",
+        747: "433d4b4ef3380d99e08e"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@unfolded/jupyter-map-sdk:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
-                for (var d = document.getElementsByTagName("script"), f = 0; f < d.length; f++) {
-                    var l = d[f];
-                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + a) {
-                        i = l;
+                for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
+                    var f = d[l];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
@@ -110,15 +110,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     d = [];
-                return "default" === t && (u("@unfolded/jupyter-map-sdk", "1.8.2", (() => Promise.all([w.e(413), w.e(568)]).then((() => () => w(568))))), u("@unfolded/map-sdk", "1.8.2", (() => w.e(747).then((() => () => w(747)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@unfolded/jupyter-map-sdk", "1.9.0", (() => Promise.all([w.e(541), w.e(568)]).then((() => () => w(568))))), u("@unfolded/map-sdk", "1.9.0", (() => w.e(747).then((() => () => w(747)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -167,31 +167,31 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, d = !0;; u++, i++) {
-                var f, l, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (l = (typeof(f = r[i]))[0])) return !d || ("u" == s ? u > n && !a : "" == s != a);
-                if ("u" == l) {
+                var l, f, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(l = r[i]))[0])) return !d || ("u" == s ? u > n && !a : "" == s != a);
+                if ("u" == f) {
                     if (!d || "u" != s) return !1
                 } else if (d)
-                    if (s == l)
+                    if (s == f)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (a ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (d = !1)
+                            if (a ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (d = !1)
                         }
                 else if ("s" != s && "n" != s) {
                     if (a || u <= n) return !1;
                     d = !1, u--
                 } else {
-                    if (u <= n || l < s != a) return !1;
+                    if (u <= n || f < s != a) return !1;
                     d = !1
                 } else "s" != s && "n" != s && (d = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
@@ -202,41 +202,41 @@
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", l = (e, r, t, n) => {
         var a = u(e, t);
         return o(n, a) || "undefined" != typeof console && console.warn && console.warn(d(e, t, a, n)), s(e[t][a])
-    }, l = (e, r, t) => {
+    }, f = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
-        var o = r && w.o(r, t) && l(r, t, n);
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
+        var o = r && w.o(r, t) && f(r, t, n);
         return o ? s(o) : a()
     })), v = {}, m = {
-        413: () => h("default", "@unfolded/map-sdk", [1, 1, 8, 2], (() => w.e(747).then((() => () => w(747))))),
+        541: () => h("default", "@unfolded/map-sdk", [1, 1, 9, 0], (() => w.e(747).then((() => () => w(747))))),
         565: () => c("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
             [1, 3, 0, 0],
             [1, 2, 0, 0],
             [1, 1, 1, 10], 1, 1, 1
         ]),
         832: () => c("default", "@lumino/widgets", [1, 1, 37, 2])
-    }, g = {
+    }, b = {
         4: [832],
-        413: [413],
+        541: [541],
         565: [565],
         568: [565]
     }, w.f.consumes = (e, r) => {
-        w.o(g, e) && g[e].forEach((e => {
+        w.o(b, e) && b[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
@@ -255,15 +255,15 @@
         var e = {
             754: 0
         };
         w.f.j = (r, t) => {
             var n = w.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(413|565)$/.test(r)) e[r] = 0;
+                else if (/^5(41|65)$/.test(r)) e[r] = 0;
             else {
                 var a = new Promise(((t, a) => n = e[r] = [t, a]));
                 t.push(n[2] = a);
                 var o = w.p + w.u(r),
                     i = new Error;
                 w.l(o, (t => {
                     if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/third-party-licenses.json` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.9.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "UNLICENSED",
             "name": "@unfolded/map-sdk",
-            "versionInfo": "1.8.2"
+            "versionInfo": "1.9.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "3.6.0"
         },
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/base.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/html.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/html.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/widget.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/map/widget.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/index.js` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,17 +25,17 @@
                                     s(e)
                                 }
                             },
                             o = e => e.done ? a(e.value) : Promise.resolve(e.value).then(r, i);
                         o((n = n.apply(e, t)).next())
                     })),
                     r = ((a = r || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a),
-                    i = class extends Error {
-                        constructor(e) {
-                            super(e), Object.setPrototypeOf(this, i.prototype)
+                    i = class e extends Error {
+                        constructor(t) {
+                            super(t), Object.setPrototypeOf(this, e.prototype)
                         }
                     },
                     o = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
 
                 function d() {
                     return s(this, arguments, (function*(e = {}, t) {
                         let n, a = "https://studio.foursquare.com/studio-bundle.js";
@@ -597,15 +597,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.9.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.9.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
     function a(e) {
         var s = n[e];
         if (void 0 !== s) return s.exports;
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/poll.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/templates/html_map_sdk.j2` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/templates/html_map_sdk.j2`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transfer_utils.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/transfer_utils.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/base.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/html.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/html.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/widget.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/transport/widget.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/types.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/types.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/action_type_mapping.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/action_type_mapping.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/encoders.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/serialization.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/validators.py` & `unfolded.map-sdk-1.9.0/unfolded/map_sdk/utils/validators.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/PKG-INFO` & `unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfolded.map-sdk
-Version: 1.8.2
+Version: 1.9.0
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 License: (c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/SOURCES.txt` & `unfolded.map-sdk-1.9.0/unfolded.map_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -59,19 +59,19 @@
 unfolded/map_sdk/api/dataset_api.py
 unfolded/map_sdk/api/enums.py
 unfolded/map_sdk/api/event_api.py
 unfolded/map_sdk/api/filter_api.py
 unfolded/map_sdk/api/layer_api.py
 unfolded/map_sdk/api/map_api.py
 unfolded/map_sdk/labextension/package.json
-unfolded/map_sdk/labextension/static/4.2f5ebe11a5669cad3275.js
-unfolded/map_sdk/labextension/static/480.25ce0490671eeeb9f120.js
-unfolded/map_sdk/labextension/static/568.caff7d3d72d44ec36b9e.js
-unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js
-unfolded/map_sdk/labextension/static/remoteEntry.1f1edfc58c4b1a509424.js
+unfolded/map_sdk/labextension/static/4.6f3ac46f5dc719fa042d.js
+unfolded/map_sdk/labextension/static/480.a7a86a8fcd664bad39be.js
+unfolded/map_sdk/labextension/static/568.69799d2e0346a48f6a67.js
+unfolded/map_sdk/labextension/static/747.433d4b4ef3380d99e08e.js
+unfolded/map_sdk/labextension/static/remoteEntry.ade37fd73490b31c9a45.js
 unfolded/map_sdk/labextension/static/style.js
 unfolded/map_sdk/labextension/static/third-party-licenses.json
 unfolded/map_sdk/map/__init__.py
 unfolded/map_sdk/map/base.py
 unfolded/map_sdk/map/html.py
 unfolded/map_sdk/map/widget.py
 unfolded/map_sdk/nbextension/extension.js
```

### Comparing `unfolded.map-sdk-1.8.2/webpack.config.js` & `unfolded.map-sdk-1.9.0/webpack.config.js`

 * *Files identical despite different names*

