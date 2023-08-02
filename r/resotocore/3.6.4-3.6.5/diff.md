# Comparing `tmp/resotocore-3.6.4.tar.gz` & `tmp/resotocore-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotocore-3.6.4.tar", last modified: Mon Jul 24 18:35:49 2023, max compression
+gzip compressed data, was "resotocore-3.6.5.tar", last modified: Wed Aug  2 19:22:31 2023, max compression
```

## Comparing `resotocore-3.6.4.tar` & `resotocore-3.6.5.tar`

### file list

```diff
@@ -1,808 +1,810 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.122703 resotocore-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 18:30:59.000000 resotocore-3.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 18:30:59.000000 resotocore-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-24 18:35:49.122703 resotocore-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-24 18:30:59.000000 resotocore-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-24 18:30:59.000000 resotocore-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.974696 resotocore-3.6.4/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.974696 resotocore-3.6.4/resotocore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.974696 resotocore-3.6.4/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.978696 resotocore-3.6.4/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31057 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   242914 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.978696 resotocore-3.6.4/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.982696 resotocore-3.6.4/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34739 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/deferredouteredgedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    65689 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/subscriberdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/system_data_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/db/usagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.986696 resotocore-3.6.4/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/graph_manager/graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.986696 resotocore-3.6.4/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.986696 resotocore-3.6.4/resotocore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.962695 resotocore-3.6.4/resotocore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.986696 resotocore-3.6.4/resotocore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-24 18:35:44.000000 resotocore-3.6.4/resotocore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.986696 resotocore-3.6.4/resotocore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 18:35:44.000000 resotocore-3.6.4/resotocore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 18:35:44.000000 resotocore-3.6.4/resotocore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.066701 resotocore-3.6.4/resotocore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1037.51967a2.js
--rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1079.cdbaf67.js
--rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1084.4cd1c89.js
--rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1113.23c9417.js
--rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1125.129d070.js
--rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1163.ac28297.js
--rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1221.c51249a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1245.be46619.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1261.199fc1d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1272.f334098.js
--rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1278.0524a4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1290.3981211.js
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1295.46e72b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1310.23bbe67.js
--rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1320.21effe3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1325.f76267c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1408.7461890.js
--rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1440.a9e7ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1483.616d9ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1489.e50b6d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1507.5705605.js
--rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/152.525d460.js
--rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1520.4e2eb21.js
--rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1555.e188f3f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1559.7c89925.js
--rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/160.5f28731.js
--rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1603.370a2a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1644.0e49167.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1667.f0afb2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1687.27f1ad6.js
--rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1725.f151c33.js
--rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1767.c8c2f26.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1806.1aaf66b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1838.1202b16.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1909.28a2def.js
--rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/1989.88d258f.js
--rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2030.1562cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2047.baed97b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2099.f4b6fcd.js
--rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2118.5b65f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/213.5769e57.js
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2161.dcb27b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2169.635c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/217.90d10e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2212.72be094.js
--rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2287.997c38e.js
--rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2303.9ff8710.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2319.6b4cbb7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2329.4c5ca6d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2351.fbd96d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2358.d5cf7c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2359.6451c3e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/237.f765e77.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2384.71782be.js
--rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/240.cddc46b.js
--rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2431.648d237.js
--rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2546.1f48267.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2557.75e9da2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/261.5f53c0e.js
--rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2629.c0e1cd6.js
--rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2788.46acc8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2834.942acc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2887.47ba752.js
--rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2956.8880209.js
--rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/2973.2a51dc4.js
--rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3004.255e79c.js
--rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/302.8bcc38f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3037.70ee38d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3042.7cfad84.js
--rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3051.34fac68.js
--rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3122.2289fca.js
--rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3151.10ef4de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/316.c850a76.js
--rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3196.4e35a17.js
--rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3265.a80440a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3277.9c04e75.js
--rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/330.126fa98.js
--rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3392.29fe6b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3413.480a49d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3444.47d5ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3469.7d14d0b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3546.fee1bd7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/362.6716970.js
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3708.410d087.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3850.903abc2.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3880.bd39dce.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3970.236586f.js
--rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3976.58893b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/3979.385527e.js
--rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/400.d72234b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4018.1a35967.js
--rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/406.9b7af92.js
--rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4117.a8107fd.js
--rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4182.e2430f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4191.02bbea8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4197.53ab10b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4206.a5f8bb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4207.0d0580b.js
--rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4262.bb73457.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4298.5ee510c.js
--rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/44.0cfa785.js
--rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4410.e4a25d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4466.64d23d1.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4507.8b41ef4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/451.d9683ad.js
--rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4535.34b060a.js
--rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4565.43bdb91.js
--rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4569.f374f9d.js
--rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4615.eb5d40a.js
--rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4658.090d4a9.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4665.aa19a41.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4668.f65690b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4690.3dd4096.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4715.e7690b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4749.46ebbb2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4750.56c06ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4856.2d7415f.js
--rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4875.375150e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/489.b981dea.js
--rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/490.c2624d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4905.667bf33.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4931.430433b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/4942.b96c164.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5016.dd2fe83.js
--rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5072.733a1b5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/509.6448878.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5096.8ed0d8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5126.eecad7a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5129.1ba4763.js
--rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5153.763d8fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5155.06b4ea9.js
--rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5193.e9f6866.js
--rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5213.3e1a360.js
--rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5227.8c8acd8.js
--rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5238.1751cc3.js
--rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/528.2262cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5292.79d4aba.js
--rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5437.31236f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5489.848a8cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5508.317fca3.js
--rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/554.ac98303.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/555.2cd31dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5573.ebcdb93.js
--rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5666.c5e5324.js
--rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5710.70d0b1d.js
--rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5747.94ad626.js
--rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/582.21b8e7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5823.5045bdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5851.30b7b2a.js
--rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5878.32d92fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5880.68f975b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5955.88508f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/5971.88c5642.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6080.aa0ff24.js
--rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/61.2808a0d.js
--rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6136.b8ba2b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6141.9831d58.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6475.6037fbb.js
--rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6493.d796aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6556.b3d9293.js
--rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6571.2c8884e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6576.3ea568e.js
--rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6591.94ed352.js
--rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6612.1632879.js
--rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6623.ae3b3cc.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6664.2160109.js
--rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6747.47be7f5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6748.be68f5f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6870.7940288.js
--rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6879.c8367a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6898.9bbc12a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6952.f68b818.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6985.321ad92.js
--rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6993.32cf9a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/6997.b06fe71.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7041.d4f561e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7058.805c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7174.6c45206.js
--rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7334.8859b1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7359.6ee65ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7364.195178b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7380.58a4413.js
--rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7427.f9c2017.js
--rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7463.18fd278.js
--rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7509.1e0189e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7526.1a303e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7537.1323a15.js
--rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7692.33d5169.js
--rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7746.5908d29.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7808.1d582a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/783.c156751.js
--rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7858.2386e4d.js
--rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/7941.01ea680.js
--rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8005.c5ad7b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8028.39e2fa1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8061.cc62561.js
--rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8101.cf46d02.js
--rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/812.9b0e86e.js
--rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/816.c8050f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8165.b2c3285.js
--rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8232.a578bf9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/824.8678196.js
--rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8270.89fe7e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/833.9cc6653.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8370.8f855e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8373.96b0b3a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8389.ffe031f.js
--rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8412.1528057.js
--rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8427.4923f43.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8542.027afdc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8594.0112f03.js
--rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8656.d5b8e92.js
--rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8685.d78bdab.js
--rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8698.9817d75.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8732.9320f73.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8741.b138cb8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8785.cf4fe95.js
--rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8828.77c71d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8883.80c7b63.js
--rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8976.3816942.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8981.99a4275.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/8990.2a453cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9035.1e45c1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9053.45b77fc.js
--rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9077.fefb6ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9128.b8fa6f0.js
--rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9156.0cefbd3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9170.0023587.js
--rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9196.315f9f9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9198.9971d70.js
--rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/920.d15c177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9253.0b31caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9266.bacd0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9307.c3a00ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9321.869e413.js
--rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9344.ba0abcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9382.9014799.js
--rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9440.1b10b8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9464.79e6ac5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9502.9a24831.js
--rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9507.1e6cc5d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9602.62bf0f1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9621.e2e8b5d.js
--rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9622.ccab065.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9626.a178bd0.js
--rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9647.ed91993.js
--rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9657.bc5c60e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/97.ad126b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9712.796a0a1.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9733.a3b2a7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9737.7dc8f98.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9777.0b8a504.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9793.6d63a85.js
--rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9806.652c162.js
--rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9865.2e3db6f.js
--rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/989.bcca86a.js
--rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9943.f3f35c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9958.25c8c06.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/9960.64cd61e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/add-above.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/add-below.svg
--rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/bug-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/build.svg
--rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/caret-down-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/caret-down-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/caret-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/caret-up-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/caret-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/case-sensitive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/circle-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/copyright.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/duplicate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/ellipses.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/extension.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/fast-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/file-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/filter-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/folder-favorite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/html5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/inspector.svg
--rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/julia.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/jupyter-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/jupyter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/keyboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.066701 resotocore-3.6.4/resotocore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/lab/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/launch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/launcher.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/line-form.svg
--rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/listings-info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/move-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/move-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/new-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/not-trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/numbering.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/offline-bolt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/palette.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/python.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/r-kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/regex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/run.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/running.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.066701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.966695 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.070701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.074701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.966695 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@retrolab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
--rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/service-worker-b2fb40a.js
--rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/spreadsheet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/table-rows.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/text-editor.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.966695 resotocore-3.6.4/resotocore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.966695 resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/toc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/tree-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/vega.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/build/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.966695 resotocore-3.6.4/resotocore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.966695 resotocore-3.6.4/resotocore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.966695 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.078701 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.082701 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.082701 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.086701 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
--rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.086701 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.086701 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
--rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-07-24 18:35:40.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.086701 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.094702 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-07-24 18:35:30.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.094702 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.094702 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-07-24 18:35:37.000000 resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.094702 resotocore-3.6.4/resotocore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-24 18:35:44.000000 resotocore-3.6.4/resotocore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.094702 resotocore-3.6.4/resotocore/jupyterlite/kernelspecs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/kernelspecs/javascript.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.098702 resotocore-3.6.4/resotocore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.098702 resotocore-3.6.4/resotocore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.098702 resotocore-3.6.4/resotocore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/service-worker-b2fb40a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.098702 resotocore-3.6.4/resotocore/jupyterlite/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.6.4/resotocore/jupyterlite/tree/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.098702 resotocore-3.6.4/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    58697 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.102702 resotocore-3.6.4/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50309 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.102702 resotocore-3.6.4/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/report/report_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.102702 resotocore-3.6.4/resotocore/static/
--rw-r--r--   0 runner    (1001) docker     (123)   130266 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/ck-unicode-truecolor.ans
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.102702 resotocore-3.6.4/resotocore/static/report/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.970696 resotocore-3.6.4/resotocore/static/report/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.102702 resotocore-3.6.4/resotocore/static/report/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.970696 resotocore-3.6.4/resotocore/static/report/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.102702 resotocore-3.6.4/resotocore/static/report/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/report/checks/aws/aws_s3.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/resoto.css
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/static/resoto_logo_and_text.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/system_start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.106703 resotocore-3.6.4/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/task_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    30387 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/task/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.106703 resotocore-3.6.4/resotocore/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/templates/create_first_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.106703 resotocore-3.6.4/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/user/user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.106703 resotocore-3.6.4/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65625 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-24 18:30:59.000000 resotocore-3.6.4/resotocore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:48.974696 resotocore-3.6.4/resotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-24 18:35:48.000000 resotocore-3.6.4/resotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-24 18:35:48.000000 resotocore-3.6.4/resotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:35:48.000000 resotocore-3.6.4/resotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 18:35:48.000000 resotocore-3.6.4/resotocore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:35:48.000000 resotocore-3.6.4/resotocore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 18:35:48.000000 resotocore-3.6.4/resotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:35:48.000000 resotocore-3.6.4/resotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-24 18:35:49.122703 resotocore-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.106703 resotocore-3.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.110703 resotocore-3.6.4/tests/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.110703 resotocore-3.6.4/tests/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/analytics/posthog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/analytics/recurrent_events_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.110703 resotocore-3.6.4/tests/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/cli/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    59677 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/cli/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/cli/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.114703 resotocore-3.6.4/tests/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/config/config_handler_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/config/config_override_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/config/core_config_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29372 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/console_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/core_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.114703 resotocore-3.6.4/tests/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/arango_query_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/arangodb_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/async_arangodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/configdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/db_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/deferredouteredgedb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/graphdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/jobdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/modeldb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/runningtaskdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/subscriberdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/system_data_db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/db/templatedb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/dependencies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.114703 resotocore-3.6.4/tests/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/graph_manager/graph_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/hypothesis_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.118703 resotocore-3.6.4/tests/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/infra_apps/local_runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/infra_apps/package_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/message_bus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.118703 resotocore-3.6.4/tests/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/adjust_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/db_updater_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/graph_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/json_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/model_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/resolve_in_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/model/typed_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.118703 resotocore-3.6.4/tests/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/query/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/query/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/query/template_expander_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.118703 resotocore-3.6.4/tests/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/report/benchnmark_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/report/inspector_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.118703 resotocore-3.6.4/tests/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/task/job_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/task/subscribers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/task/task_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/task/task_handler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.118703 resotocore-3.6.4/tests/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/user/user_management_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:49.122703 resotocore-3.6.4/tests/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/web/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/web/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/web/certificate_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/web/content_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-24 18:30:59.000000 resotocore-3.6.4/tests/resotocore/worker_task_queue_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.606728 resotocore-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 19:17:32.000000 resotocore-3.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-02 19:17:32.000000 resotocore-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-08-02 19:22:31.606728 resotocore-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-02 19:17:32.000000 resotocore-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-02 19:17:32.000000 resotocore-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.478726 resotocore-3.6.5/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.478726 resotocore-3.6.5/resotocore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.478726 resotocore-3.6.5/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.482726 resotocore-3.6.5/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31142 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   248929 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27909 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.482726 resotocore-3.6.5/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.486727 resotocore-3.6.5/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34739 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/deferredouteredgedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65689 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/subscriberdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/db/usagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.486727 resotocore-3.6.5/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.486727 resotocore-3.6.5/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.486727 resotocore-3.6.5/resotocore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.466726 resotocore-3.6.5/resotocore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.486727 resotocore-3.6.5/resotocore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-02 19:22:26.000000 resotocore-3.6.5/resotocore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.486727 resotocore-3.6.5/resotocore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 19:22:26.000000 resotocore-3.6.5/resotocore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 19:22:26.000000 resotocore-3.6.5/resotocore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.558728 resotocore-3.6.5/resotocore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1037.51967a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1079.cdbaf67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1084.4cd1c89.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1113.23c9417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1125.129d070.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1163.ac28297.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1221.c51249a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1245.be46619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1261.199fc1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1272.f334098.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1278.0524a4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1290.3981211.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1295.46e72b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1310.23bbe67.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1320.21effe3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1325.f76267c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1408.e049d91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1440.a9e7ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1483.616d9ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1489.e50b6d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1507.5705605.js
+-rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/152.525d460.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1520.4e2eb21.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1555.e188f3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1559.7c89925.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/160.5f28731.js
+-rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1603.370a2a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1644.0e49167.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1667.f0afb2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1687.27f1ad6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1725.f151c33.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1767.c8c2f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1806.1aaf66b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1838.1202b16.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1909.28a2def.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/1989.88d258f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2030.1562cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2047.baed97b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2099.f4b6fcd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2118.5b65f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/213.5769e57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2161.dcb27b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2169.635c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/217.90d10e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2212.72be094.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2287.997c38e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2303.9ff8710.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2319.6b4cbb7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2329.4c5ca6d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2351.fbd96d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2358.d5cf7c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2359.6451c3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/237.f765e77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2384.71782be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/240.cddc46b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2431.648d237.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2546.1f48267.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2557.6c85d56.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/261.5f53c0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2629.c0e1cd6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2788.46acc8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2834.942acc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2887.47ba752.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2956.8880209.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/2973.2a51dc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3004.255e79c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/302.fad99ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3037.70ee38d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3042.7cfad84.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3051.34fac68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3122.2289fca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3151.10ef4de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/316.c850a76.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3196.4e35a17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3265.a80440a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3277.9c04e75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/330.126fa98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3392.29fe6b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3413.480a49d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3444.808a22d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3469.7d14d0b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3546.fee1bd7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/362.6716970.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3708.410d087.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3850.903abc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3880.bd39dce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3970.236586f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3976.58893b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/3979.385527e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/400.d72234b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4018.1a35967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/406.9b7af92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4117.a8107fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4182.e2430f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4191.02bbea8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4197.53ab10b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4206.a5f8bb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4207.0d0580b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4262.bb73457.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4298.5ee510c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/44.0cfa785.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4410.e4a25d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4466.64d23d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4507.8b41ef4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/451.d9683ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4535.34b060a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4565.43bdb91.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4569.f374f9d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4615.eb5d40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4658.090d4a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4665.aa19a41.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4668.f65690b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4690.3dd4096.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4715.e7690b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4749.46ebbb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4750.56c06ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4856.2d7415f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4875.375150e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/489.b981dea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/490.c2624d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4905.667bf33.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4931.47d8e25.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/4942.b96c164.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5016.dd2fe83.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5072.733a1b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/509.6448878.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5096.8ed0d8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5126.eecad7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5129.1ba4763.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5153.763d8fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5155.06b4ea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5193.e9f6866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5213.3e1a360.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5227.8c8acd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5238.f0f5af0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/528.2262cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5292.79d4aba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5437.31236f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5489.848a8cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5508.317fca3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/554.ac98303.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/555.2cd31dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5573.ebcdb93.js
+-rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5666.c5e5324.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5710.70d0b1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5747.94ad626.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/582.21b8e7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5823.5045bdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5851.30b7b2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5878.32d92fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5880.68f975b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5955.88508f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/5971.88c5642.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6080.aa0ff24.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/61.2808a0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6136.b8ba2b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6141.9831d58.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6475.22d38af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6493.d796aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6556.b3d9293.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6571.2c8884e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6576.3ea568e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6591.94ed352.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6612.1632879.js
+-rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6623.ae3b3cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6664.2160109.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6747.47be7f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6748.be68f5f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6870.7940288.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6879.c8367a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6898.9bbc12a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6952.f68b818.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6985.321ad92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6993.32cf9a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/6997.b06fe71.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7041.d4f561e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7058.805c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7174.6c45206.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7334.8859b1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7359.6ee65ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7364.195178b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7380.58a4413.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7427.f9c2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7463.18fd278.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7509.1e0189e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7526.1a303e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7537.1323a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7692.33d5169.js
+-rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7746.5908d29.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7808.1d582a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/783.c156751.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7858.2386e4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/7941.01ea680.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8005.c5ad7b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8028.39e2fa1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8061.cc62561.js
+-rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8101.cf46d02.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/812.9b0e86e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/816.c8050f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8165.b2c3285.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8232.a578bf9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/824.8678196.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8270.89fe7e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/833.9cc6653.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8370.8678c18.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8373.96b0b3a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8389.ffe031f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8412.1528057.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8427.4923f43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8542.027afdc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8594.0112f03.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8656.d5b8e92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8685.13b9daf.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8698.9817d75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8732.20136c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8741.b138cb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8785.cf4fe95.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8828.77c71d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8883.80c7b63.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8976.3816942.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8981.99a4275.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/8990.2a453cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9035.1e45c1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9053.45b77fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9077.fefb6ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9128.b8fa6f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9156.0cefbd3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9170.0023587.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9196.315f9f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9198.9971d70.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/920.d15c177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9253.0b31caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9266.bacd0dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9307.c3a00ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9321.869e413.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9344.ba0abcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9382.144ed35.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9440.1b10b8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9464.79e6ac5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9502.9a24831.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9507.1e6cc5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9602.62bf0f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9621.e2e8b5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9622.ccab065.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9626.a178bd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9647.ed91993.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9657.bc5c60e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/97.ad126b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9712.796a0a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9733.a3b2a7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9737.7dc8f98.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9777.0b8a504.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9793.6d63a85.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9806.652c162.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9865.2e3db6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/989.bcca86a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9943.f3f35c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9958.25c8c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/9960.2d4eeed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/add-above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/add-below.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/bug-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/build.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/caret-down-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/caret-down-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/caret-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/caret-up-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/caret-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/case-sensitive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/circle-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/copyright.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/duplicate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/ellipses.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/extension.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/fast-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/file-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/filter-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/folder-favorite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/inspector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/julia.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/jupyter-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/jupyter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/keyboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.558728 resotocore-3.6.5/resotocore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)    54486 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/lab/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/launch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/launcher.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/line-form.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/listings-info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/move-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/move-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/new-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/not-trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/numbering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/offline-bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/palette.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/r-kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/regex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/run.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.558728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.470726 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.562728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.566728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.470726 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@retrolab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/service-worker-b2fb40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/spreadsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/table-rows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/text-editor.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.470726 resotocore-3.6.5/resotocore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.470726 resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/toc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/tree-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/vega.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/build/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.470726 resotocore-3.6.5/resotocore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.470726 resotocore-3.6.5/resotocore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.470726 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.29fb1677e9ddfbef42ef.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.5488d7441d23f13faba2.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.b0a688b88d43b80c014d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8373 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.9eaa8a846d81f5b6c8be.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.570728 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.574728 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8197 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/324.2759063405b36360da9d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/324.2759063405b36360da9d.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2534 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.ecdf94afc2748b3fc2e0.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.574728 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6513 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6718 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.9-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8222 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.9-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2338 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2338 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7925 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.703f03086e9738104706.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.574728 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-08-02 19:22:22.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.574728 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.582728 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-08-02 19:22:12.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.582728 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.582728 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-08-02 19:22:18.000000 resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.582728 resotocore-3.6.5/resotocore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-08-02 19:22:26.000000 resotocore-3.6.5/resotocore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.582728 resotocore-3.6.5/resotocore/jupyterlite/kernelspecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/kernelspecs/javascript.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.582728 resotocore-3.6.5/resotocore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.586728 resotocore-3.6.5/resotocore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.586728 resotocore-3.6.5/resotocore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/service-worker-b2fb40a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.586728 resotocore-3.6.5/resotocore/jupyterlite/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.6.5/resotocore/jupyterlite/tree/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.586728 resotocore-3.6.5/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58697 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.586728 resotocore-3.6.5/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50309 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.586728 resotocore-3.6.5/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/report/report_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.590728 resotocore-3.6.5/resotocore/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   130266 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/ck-unicode-truecolor.ans
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.590728 resotocore-3.6.5/resotocore/static/report/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.474727 resotocore-3.6.5/resotocore/static/report/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.590728 resotocore-3.6.5/resotocore/static/report/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.474727 resotocore-3.6.5/resotocore/static/report/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.590728 resotocore-3.6.5/resotocore/static/report/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/report/checks/aws/aws_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/resoto.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/static/resoto_logo_and_text.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/system_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.594728 resotocore-3.6.5/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/task_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30387 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.594728 resotocore-3.6.5/resotocore/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.594728 resotocore-3.6.5/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/user/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.594728 resotocore-3.6.5/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66905 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-08-02 19:17:32.000000 resotocore-3.6.5/resotocore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.478726 resotocore-3.6.5/resotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-08-02 19:22:31.000000 resotocore-3.6.5/resotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34671 2023-08-02 19:22:31.000000 resotocore-3.6.5/resotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:22:31.000000 resotocore-3.6.5/resotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 19:22:31.000000 resotocore-3.6.5/resotocore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:22:31.000000 resotocore-3.6.5/resotocore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 19:22:31.000000 resotocore-3.6.5/resotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 19:22:31.000000 resotocore-3.6.5/resotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-02 19:22:31.606728 resotocore-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.594728 resotocore-3.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.598728 resotocore-3.6.5/tests/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.598728 resotocore-3.6.5/tests/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/analytics/posthog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/analytics/recurrent_events_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.598728 resotocore-3.6.5/tests/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/cli/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59709 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/cli/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/cli/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.598728 resotocore-3.6.5/tests/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/config/config_handler_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/config/config_override_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/config/core_config_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29751 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/console_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/core_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.602728 resotocore-3.6.5/tests/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/arango_query_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/arangodb_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/async_arangodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/configdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/db_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/deferredouteredgedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/graphdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/jobdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/modeldb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/runningtaskdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/subscriberdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/system_data_db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/db/templatedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/dependencies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.602728 resotocore-3.6.5/tests/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/graph_manager/graph_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/hypothesis_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.602728 resotocore-3.6.5/tests/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/infra_apps/local_runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/infra_apps/package_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/message_bus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.602728 resotocore-3.6.5/tests/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/adjust_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/db_updater_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/graph_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/json_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/model_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/resolve_in_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/model/typed_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.606728 resotocore-3.6.5/tests/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/query/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/query/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/query/template_expander_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.606728 resotocore-3.6.5/tests/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/report/benchnmark_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/report/inspector_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.606728 resotocore-3.6.5/tests/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/task/job_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/task/subscribers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/task/task_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/task/task_handler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.606728 resotocore-3.6.5/tests/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/user/user_management_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:31.606728 resotocore-3.6.5/tests/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/web/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/web/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/web/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/web/certificate_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/web/content_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-02 19:17:32.000000 resotocore-3.6.5/tests/resotocore/worker_task_queue_test.py
```

### Comparing `resotocore-3.6.4/LICENSE` & `resotocore-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/PKG-INFO` & `resotocore-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.6.4
+Version: 3.6.5
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.6.4/README.md` & `resotocore-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/pyproject.toml` & `resotocore-3.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotocore"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Keeps all the things."
 license = {file="LICENSE"}
 urls = {"Homepage" = "https://resoto.com"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `resotocore-3.6.4/resotocore/__main__.py` & `resotocore-3.6.5/resotocore/__main__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/action_handlers/merge_outer_edge_handler.py` & `resotocore-3.6.5/resotocore/action_handlers/merge_outer_edge_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/analytics/__init__.py` & `resotocore-3.6.5/resotocore/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/analytics/posthog.py` & `resotocore-3.6.5/resotocore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/analytics/recurrent_events.py` & `resotocore-3.6.5/resotocore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/async_extensions.py` & `resotocore-3.6.5/resotocore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/cli/__init__.py` & `resotocore-3.6.5/resotocore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/cli/cli.py` & `resotocore-3.6.5/resotocore/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     PathRoot,
     Limit,
     Sort,
 )
 from resotocore.query.query_parser import aggregate_parameter_parser, sort_args_p, limit_parser_direct
 from resotocore.service import Service
 from resotocore.types import JsonElement
+from resotocore.user.model import Permission
 from resotocore.util import group_by
 from resotolib.parse_util import make_parser, pipe_p, semicolon_p
 
 log = logging.getLogger(__name__)
 
 
 @make_parser
@@ -205,15 +206,15 @@
             elif arg in self.infra_app_aliases:
                 result = self.infra_app_aliases[arg].rendered_help(ctx)
             else:
                 result = f"No command found with this name: {arg}"
 
             return stream.just(result)
 
-        return CLISource.single(help_command)
+        return CLISource.single(help_command, required_permissions={Permission.read})
 
 
 CLIArg = Tuple[CLICommand, Optional[str]]
 # If no sort is defined in the part, we use this default sort order
 DefaultSort = [Sort("/reported.kind"), Sort("/reported.name"), Sort("/reported.id")]
 # Default sort order for history searches
 HistorySort = [Sort("/changed_at"), Sort("/reported.kind"), Sort("/reported.name"), Sort("/reported.id")]
```

### Comparing `resotocore-3.6.4/resotocore/cli/command.py` & `resotocore-3.6.5/resotocore/cli/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,22 +92,23 @@
     ParsedCommand,
     NoTerminalOutput,
     ArgsInfo,
     ArgInfo,
     EntityProvider,
     FilePath,
 )
+from resotocore.user.model import Permission, AllowedRoleNames
 from resotocore.cli.tip_of_the_day import SuggestionPolicy, SuggestionStrategy, get_suggestion_strategy
 from resotocore.config import ConfigEntity
 from resotocore.db.async_arangodb import AsyncCursor
 from resotocore.db.graphdb import HistoryChange, GraphDB
 from resotocore.db.model import QueryModel
 from resotocore.db.runningtaskdb import RunningTaskData
 from resotocore.system_start import system_info
-from resotocore.error import CLIParseError, ClientError, CLIExecutionError
+from resotocore.error import CLIParseError, ClientError, CLIExecutionError, NotEnoughPermissions
 from resotocore.ids import ConfigId, TaskId, InfraAppName, TaskDescriptorId, GraphName, Email, Password
 from resotocore.infra_apps.manifest import AppManifest
 from resotocore.infra_apps.package_manager import Failure
 from resotocore.model.graph_access import Section, EdgeTypes
 from resotocore.model.model import (
     Model,
     Kind,
@@ -137,15 +138,15 @@
 )
 from resotocore.query.query_parser import parse_query, aggregate_parameter_parser
 from resotocore.query.template_expander import tpl_props_p
 from resotocore.report import BenchmarkConfigPrefix, ReportSeverity
 from resotocore.report.benchmark_renderer import respond_benchmark_result
 from resotocore.task.task_description import Job, TimeTrigger, EventTrigger, ExecuteCommand, Workflow, RunningTask
 from resotocore.types import Json, JsonElement, EdgeType
-from resotocore.user import ResotoUser, ValidRoles
+from resotocore.user import ResotoUser
 from resotocore.util import (
     uuid_str,
     utc,
     if_set,
     duration,
     identity,
     rnd_str,
@@ -1168,15 +1169,17 @@
     def info(self) -> str:
         return "Send the provided message to downstream."
 
     def args_info(self) -> ArgsInfo:
         return [ArgInfo(expects_value=True, help_text="message to send downstream")]
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLISource:
-        return CLISource.single(lambda: stream.just(strip_quotes(arg if arg else "")))
+        return CLISource.single(
+            lambda: stream.just(strip_quotes(arg if arg else "")), required_permissions={Permission.read}
+        )
 
 
 class JsonCommand(CLICommand):
     """
     ```shell
     json <json-string>
     ```
@@ -1228,15 +1231,17 @@
             raise AttributeError("json expects one argument!")
         if isinstance(js, list):
             elements = js
         elif isinstance(js, (str, int, float, bool, dict)):
             elements = [js]
         else:
             raise AttributeError(f"json does not understand {arg}.")
-        return CLISource.with_count(lambda: stream.iterate(elements), len(elements))
+        return CLISource.with_count(
+            lambda: stream.iterate(elements), len(elements), required_permissions={Permission.read}
+        )
 
 
 class SleepCommand(CLICommand):
     """
     ```shell
     sleep <seconds>
     ```
@@ -1271,15 +1276,15 @@
             sleep_time = float(arg)
 
             async def sleep() -> AsyncIterator[JsonElement]:
                 for _ in range(0, 1):
                     await asyncio.sleep(sleep_time)
                     yield ""
 
-            return CLISource.single(sleep)
+            return CLISource.single(sleep, required_permissions={Permission.read})
         except Exception as ex:
             raise AttributeError("Sleep needs the time in seconds as arg.") from ex
 
 
 class AggregateToCountCommand(CLICommand, InternalPart):
     """
     ```shell
@@ -1469,15 +1474,19 @@
                     async for e in cursor:
                         yield e
                 finally:
                     cursor.close()
 
             return cursor.count(), iterate_and_close()
 
-        return CLISource.single(explain_search) if explain else CLISource(prepare)
+        return (
+            CLISource.single(explain_search, required_permissions={Permission.read})
+            if explain
+            else CLISource(prepare, required_permissions={Permission.read})
+        )
 
 
 class EnvCommand(CLICommand):
     """
     ```shell
     env
     ```
@@ -1509,15 +1518,15 @@
     def info(self) -> str:
         return "Retrieve the environment and pass it to the output stream."
 
     def args_info(self) -> ArgsInfo:
         return []
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLISource:
-        return CLISource.with_count(lambda: stream.just(ctx.env), len(ctx.env))
+        return CLISource.with_count(lambda: stream.just(ctx.env), len(ctx.env), required_permissions={Permission.read})
 
 
 class ChunkCommand(CLICommand):
     """
     ```shell
     chunk [num]
     ```
@@ -1558,15 +1567,15 @@
         return "Chunk incoming elements in batches."
 
     def args_info(self) -> ArgsInfo:
         return [ArgInfo(expects_value=True, help_text="The number of elements to put into one chunk.")]
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         size = int(arg) if arg else 100
-        return CLIFlow(lambda in_stream: stream.chunks(in_stream, size))
+        return CLIFlow(lambda in_stream: stream.chunks(in_stream, size), required_permissions={Permission.read})
 
 
 class FlattenCommand(CLICommand):
     """
     ```shell
     flatten
     ```
@@ -1611,15 +1620,15 @@
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         def iterable(it: Any) -> bool:
             return False if isinstance(it, str) else isinstance(it, Iterable)
 
         def iterate(it: Any) -> Stream:
             return stream.iterate(it) if is_async_iterable(it) or iterable(it) else stream.just(it)
 
-        return CLIFlow(lambda in_stream: stream.flatmap(in_stream, iterate))
+        return CLIFlow(lambda in_stream: stream.flatmap(in_stream, iterate), required_permissions={Permission.read})
 
 
 class UniqCommand(CLICommand):
     """
     ```shell
     uniq
     ```
@@ -1668,15 +1677,15 @@
 
             if item in visited:
                 return False
             else:
                 visited.add(item)
                 return True
 
-        return CLIFlow(lambda in_stream: stream.filter(in_stream, has_not_seen))
+        return CLIFlow(lambda in_stream: stream.filter(in_stream, has_not_seen), required_permissions={Permission.read})
 
 
 class JqCommand(CLICommand, OutputTransformer):
     """
     ```
     jq [--no-rewrite] <filter>
     ```
@@ -1768,15 +1777,15 @@
         compiled = jq.compile(strip_quotes(in_arg))
 
         def process(in_json: Json) -> Json:
             out = compiled.input(in_json).all()
             result = out[0] if len(out) == 1 else out
             return cast(Json, result)
 
-        return CLIFlow(lambda in_stream: stream.map(in_stream, process))
+        return CLIFlow(lambda in_stream: stream.map(in_stream, process), required_permissions={Permission.read})
 
 
 class KindsCommand(CLICommand, PreserveOutputFormat):
     """
     ```shell
     kinds [-a ] [-p property_path] [name]
     ```
@@ -1930,27 +1939,30 @@
                 if appears_in := property_defined_in(model, no_section):
                     result["appears_in"] = appears_in
                 return 1, stream.just(result)
             else:
                 result = sorted([k.fqn for k in model.kinds.values() if isinstance(k, ComplexKind) and show(k)])
                 return len(model.kinds), stream.iterate(result)
 
-        return CLISource(source)
+        return CLISource(source, required_permissions={Permission.read})
 
 
 class SetDesiredStateBase(CLICommand, EntityProvider, ABC):
     @abstractmethod
     def patch(self, arg: Optional[str], ctx: CLIContext) -> Json:
         # deriving classes need to define how to patch
         pass
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         buffer_size = 1000
         func = partial(self.set_desired, arg, ctx.graph_name, self.patch(arg, ctx))
-        return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
+        return CLIFlow(
+            lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func),
+            required_permissions={Permission.write},
+        )
 
     async def set_desired(
         self, arg: Optional[str], graph_name: GraphName, patch: Json, items: List[Json]
     ) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model(graph_name)
         db = self.dependencies.db_access.get_graph_db(graph_name)
         node_ids = []
@@ -2078,15 +2090,18 @@
     def patch(self, arg: Optional[str], ctx: CLIContext) -> Json:
         # deriving classes need to define how to patch
         pass
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         buffer_size = 1000
         func = partial(self.set_metadata, ctx.graph_name, self.patch(arg, ctx))
-        return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
+        return CLIFlow(
+            lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func),
+            required_permissions={Permission.write},
+        )
 
     async def set_metadata(self, graph_name: GraphName, patch: Json, items: List[Json]) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model(graph_name)
         db = self.dependencies.db_access.get_graph_db(graph_name)
         node_ids = []
         for item in items:
             if "id" in item:
@@ -2302,15 +2317,15 @@
                     raise ValueError(f"Unknown format: {use}")
             elif formatting_string:
                 return stream.map(in_stream, ctx.formatter(arg)) if arg else in_stream
             else:
                 return in_stream
 
         produces = MediaType.Markdown if use == "benchmark_result" else MediaType.String
-        return CLIFlow(format_stream, produces=produces)
+        return CLIFlow(format_stream, produces=produces, required_permissions={Permission.read})
 
 
 @make_parser
 def list_single_arg_parse() -> Parser:
     name = yield variable_dp
     as_name = yield (space_dp >> string("as") >> space_dp >> literal_dp).optional()
     return name, as_name
@@ -2385,15 +2400,15 @@
 
     def args_info(self) -> ArgsInfo:
         return []
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         # Dump returns the same stream as provided without changing anything.
         # Since it is an OutputTransformer, the resulting transformer will be dump (not list).
-        return CLIFlow(identity)
+        return CLIFlow(identity, required_permissions={Permission.read})
 
 
 class ListCommand(CLICommand, OutputTransformer):
     """
     ```
     list [property [as <name>]] [,property ...]
     ```
@@ -2709,15 +2724,15 @@
             if parsed.csv:
                 return csv_stream(in_stream)
             elif parsed.markdown:
                 return markdown_stream(in_stream)
             else:
                 return stream.map(in_stream, lambda elem: fmt_json(elem) if isinstance(elem, dict) else str(elem))
 
-        return CLIFlow(fmt, produces=MediaType.String)
+        return CLIFlow(fmt, produces=MediaType.String, required_permissions={Permission.read})
 
 
 class JobsCommand(CLICommand, PreserveOutputFormat):
     """
     ```shell
     jobs list
     jobs show <id>
@@ -2907,16 +2922,27 @@
             arg_parser.add_argument("--wait-for-event", dest="event", type=lambda e: EventTrigger(strip_quotes(e)))
             arg_parser.add_argument(
                 "--timeout", dest="timeout", default=timedelta(hours=1), type=lambda t: timedelta(seconds=int(t))
             )
             parsed, rest = arg_parser.parse_known_args(list(args_parts_parser.parse(arg_str)))
             uid = parsed.id
             command = " ".join(rest)
-            # only here to make sure the command can be executed
-            await self.dependencies.cli.evaluate_cli_command(command, ctx)
+            # make sure the command can be executed
+            cmd_lines = await self.dependencies.cli.evaluate_cli_command(command, ctx)
+            # check that the permission required for the job exist for the current user
+            if self.dependencies.config.args.psk is not None and not all(
+                cmd_line.is_allowed_to_execute() for cmd_line in cmd_lines
+            ):
+                required = {
+                    p
+                    for cmd_line in cmd_lines
+                    for cmd in cmd_line.executable_commands
+                    for p in cmd.action.required_permissions
+                }
+                raise NotEnoughPermissions(ctx.user_permissions, required)
 
             timeout: timedelta = parsed.timeout
             if parsed.schedule and parsed.event:
                 wait = (parsed.event, timeout)
                 job = Job(uid, ExecuteCommand(command), timeout, parsed.schedule, wait, ctx.env)
             elif parsed.schedule or parsed.event:
                 trigger = parsed.schedule or parsed.event
@@ -2968,33 +2994,39 @@
 
         async def show_help() -> AsyncIterator[str]:
             yield self.rendered_help(ctx)
 
         args = re.split("\\s+", arg, maxsplit=1) if arg else []
         if arg and len(args) == 2 and args[0] in ("add", "update"):
             is_update = args[0] == "update"
-            return CLISource.single(partial(put_job, args[1].strip(), is_update))
+            return CLISource.single(
+                partial(put_job, args[1].strip(), is_update), required_permissions={Permission.write}
+            )
         elif arg and len(args) == 2 and args[0] == "delete":
-            return CLISource.single(partial(delete_job, args[1].strip()))
+            return CLISource.single(partial(delete_job, args[1].strip()), required_permissions={Permission.write})
         elif arg and len(args) == 2 and args[0] == "show":
-            return CLISource.single(partial(show_job, args[1].strip()))
+            return CLISource.single(partial(show_job, args[1].strip()), required_permissions={Permission.read})
         elif arg and len(args) == 2 and args[0] == "run":
-            return CLISource.single(partial(run_job, args[1].strip()))
+            return CLISource.single(partial(run_job, args[1].strip()), required_permissions={Permission.write})
         elif arg and len(args) == 2 and args[0] == "activate":
-            return CLISource.single(partial(activate_deactivate_job, args[1].strip(), True))
+            return CLISource.single(
+                partial(activate_deactivate_job, args[1].strip(), True), required_permissions={Permission.write}
+            )
         elif arg and len(args) == 2 and args[0] == "deactivate":
-            return CLISource.single((partial(activate_deactivate_job, args[1].strip(), False)))
+            return CLISource.single(
+                (partial(activate_deactivate_job, args[1].strip(), False)), required_permissions={Permission.write}
+            )
         elif arg and len(args) == 2:
             raise CLIParseError(f"Does not understand action {args[0]}. Allowed: add, update, delete.")
         elif arg and len(args) == 1 and args[0] == "running":
-            return CLISource(running_jobs)
+            return CLISource(running_jobs, required_permissions={Permission.read})
         elif arg and len(args) == 1 and args[0] == "list":
-            return CLISource(list_jobs)
+            return CLISource(list_jobs, required_permissions={Permission.read})
         else:
-            return CLISource.single(show_help)
+            return CLISource.single(show_help, required_permissions={Permission.read})
 
 
 class SendWorkerTaskCommand(CLICommand, ABC):
     # Abstract base for all commands that send task to the work queue
 
     # this method expects a stream of Tuple[str, Dict[str, str], Json]
     def send_to_queue_stream(
@@ -3203,15 +3235,19 @@
             dependencies = stream.call(load_model)
             return stream.flatmap(dependencies, with_dependencies)
 
         def setup_source() -> Stream:
             arg = {"args": args_parts_unquoted_parser.parse(formatter({}))}
             return self.send_to_queue_stream(stream.just((command_name, {}, arg)), self.no_update, True)
 
-        return CLISource.single(setup_source) if ctx.query is None else CLIFlow(setup_stream)
+        return (
+            CLISource.single(setup_source, required_permissions={Permission.write})
+            if ctx.query is None
+            else CLIFlow(setup_stream, required_permissions={Permission.write})
+        )
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         parser = NoExitArgumentParser()
         parser.add_argument("--command", required=True)
         parser.add_argument("--arg")
         parser.add_argument("--no-node-result", action="store_true", default=False)
         parser.add_argument("--allowed-on")
@@ -3323,28 +3359,28 @@
             async def load_model() -> Model:
                 return await self.dependencies.model_handler.load_model(ctx.graph_name)
 
             # dependencies are not resolved directly (no async function is allowed here)
             dependencies = stream.call(load_model)
             return stream.flatmap(dependencies, with_dependencies)
 
-        return CLIFlow(setup_stream)
+        return CLIFlow(setup_stream, required_permissions={Permission.write})
 
 
 class FileCommand(CLICommand, InternalPart):
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLISource:
         def file_command() -> Stream:
             if not arg:
                 raise AttributeError("file command needs a parameter!")
             elif not os.path.exists(arg):
                 raise AttributeError(f"file does not exist: {arg}!")
             else:
                 return stream.just(arg if arg else "")
 
-        return CLISource.single(file_command, MediaType.FilePath)
+        return CLISource.single(file_command, MediaType.FilePath, required_permissions={Permission.admin})
 
     @property
     def name(self) -> str:
         return "file"
 
     def info(self) -> str:
         return "only for debugging purposes..."
@@ -3362,15 +3398,17 @@
         def upload_command() -> Stream:
             if file_id in ctx.uploaded_files:
                 file = ctx.uploaded_files[file_id]
                 return stream.just(f"Received file {file} of size {os.path.getsize(file)}")
             else:
                 raise AttributeError(f"file was not uploaded: {arg}!")
 
-        return CLISource.single(upload_command, MediaType.Json, [CLIFileRequirement(file_id, arg)])
+        return CLISource.single(
+            upload_command, MediaType.Json, [CLIFileRequirement(file_id, arg)], required_permissions={Permission.admin}
+        )
 
     @property
     def name(self) -> str:
         return "upload"
 
     def info(self) -> str:
         return "only for debugging purposes..."
@@ -3600,25 +3638,30 @@
         parts = re.split(r"\s+", arg if arg else "")
         if len(parts) >= 2 and parts[0] == "backup" and parts[1] == "create":
             rest = parts[2:]
 
             def backup() -> AsyncIterator[JsonElement]:
                 return self.create_backup(" ".join(rest) if rest else None)
 
-            return CLISource.single(backup, MediaType.FilePath)
+            return CLISource.single(backup, MediaType.FilePath, required_permissions={Permission.admin})
 
         elif len(parts) == 3 and parts[0] == "backup" and parts[1] == "restore":
             backup_file = parts[2]
 
             def restore() -> AsyncIterator[JsonElement]:
                 return self.restore_backup(ctx.uploaded_files.get("backup"), ctx)
 
-            return CLISource.single(restore, MediaType.Json, [CLIFileRequirement("backup", backup_file)])
+            return CLISource.single(
+                restore,
+                MediaType.Json,
+                [CLIFileRequirement("backup", backup_file)],
+                required_permissions={Permission.admin},
+            )
         elif len(parts) == 1 and parts[0] == "info":
-            return CLISource.single(self.show_system_info)
+            return CLISource.single(self.show_system_info, required_permissions={Permission.read})
         else:
             raise CLIParseError(f"system: Can not parse {arg}")
 
 
 class WriteCommand(CLICommand, NoTerminalOutput):
     """
     ```shell
@@ -3674,15 +3717,17 @@
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         if arg is None:
             raise AttributeError("write requires a filename to write to")
         if (ex := self.get_previous_command(kwargs)) and ex.action.produces == MediaType.FilePath:
             fn = self.already_file_stream
         else:
             fn = self.write_result_to_file
-        return CLIFlow(lambda in_stream: fn(in_stream, cast(str, arg)), MediaType.FilePath)
+        return CLIFlow(
+            lambda in_stream: fn(in_stream, cast(str, arg)), MediaType.FilePath, required_permissions={Permission.read}
+        )
 
 
 class TemplatesCommand(CLICommand, PreserveOutputFormat):
     """
     ```shell
     templates
     templates <name_of_template>
@@ -3784,25 +3829,27 @@
         async def expand_template(spec: str) -> AsyncIterator[str]:
             maybe_dict, template = tpl_props_p.parse_partial(spec)
             yield self.dependencies.template_expander.render(template, maybe_dict if maybe_dict else {})
 
         args = re.split("\\s+", arg, maxsplit=1) if arg else []
         if arg and len(args) == 2 and args[0] in ("add", "update"):
             nm, tpl = re.split("\\s+", args[1], maxsplit=1)
-            return CLISource.single(partial(put_template, nm.strip(), tpl.strip()))
+            return CLISource.single(
+                partial(put_template, nm.strip(), tpl.strip()), required_permissions={Permission.admin}
+            )
         elif arg and len(args) == 2 and args[0] == "delete":
-            return CLISource.single(partial(delete_template, args[1].strip()))
+            return CLISource.single(partial(delete_template, args[1].strip()), required_permissions={Permission.admin})
         elif arg and len(args) == 2 and args[0] == "test":
-            return CLISource.single(partial(expand_template, args[1].strip()))
+            return CLISource.single(partial(expand_template, args[1].strip()), required_permissions={Permission.read})
         elif arg and len(args) == 2:
             raise CLIParseError(f"Does not understand action {args[0]}. Allowed: add, update, delete, test.")
         elif arg and len(args) == 1:
-            return CLISource.single(partial(get_template, arg.strip()))
+            return CLISource.single(partial(get_template, arg.strip()), required_permissions={Permission.read})
         elif not arg:
-            return CLISource(list_templates)
+            return CLISource(list_templates, required_permissions={Permission.read})
         else:
             raise CLIParseError(f"Can not parse arguments: {arg}")
 
 
 @define
 class HttpRequestTemplate:
     method: str
@@ -4016,15 +4063,15 @@
 
         return iterate_stream
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         # command name is the default scheme: http, https etc.
         default_scheme = kwargs.get("cmd_name", "http")
         template = self.parse_args(default_scheme, arg)
-        return CLIFlow(self.perform_requests(template))
+        return CLIFlow(self.perform_requests(template), required_permissions={Permission.read})
 
 
 class WorkflowsCommand(CLICommand):
     """
     ```shell
     workflows list
     workflows show <id>
@@ -4289,31 +4336,33 @@
             if await self.dependencies.task_handler.stop_task(task_id) is not None:
                 yield f"Workflow Task {task_id} stopped."
             else:
                 yield "No running workflow with this id."
 
         args = re.split("\\s+", arg, maxsplit=1) if arg else []
         if arg and len(args) == 2 and args[0] == "show":
-            return CLISource.single(partial(show_workflow, args[1].strip()))
+            return CLISource.single(partial(show_workflow, args[1].strip()), required_permissions={Permission.read})
         elif arg and len(args) == 1 and args[0] == "history":
-            return CLISource.single(history_aggregation)
+            return CLISource.single(history_aggregation, required_permissions={Permission.read})
         elif arg and len(args) == 2 and args[0] == "history":
-            return CLISource(partial(history_of, re.split("\\s+", args[1])))
+            return CLISource(partial(history_of, re.split("\\s+", args[1])), required_permissions={Permission.read})
         elif arg and len(args) == 2 and args[0] == "log":
-            return CLISource(partial(show_log, args[1].strip()))
+            return CLISource(partial(show_log, args[1].strip()), required_permissions={Permission.read})
         elif arg and len(args) == 2 and args[0] == "run":
-            return CLISource.single(partial(run_workflow, args[1].strip()))
+            return CLISource.single(partial(run_workflow, args[1].strip()), required_permissions={Permission.admin})
         elif arg and len(args) == 2 and args[0] == "stop":
-            return CLISource.single(partial(stop_workflow, args[1].strip()))
+            return CLISource.single(partial(stop_workflow, args[1].strip()), required_permissions={Permission.admin})
         elif arg and len(args) == 1 and args[0] == "running":
-            return CLISource(running_workflows)
+            return CLISource(running_workflows, required_permissions={Permission.read})
         elif arg and len(args) == 1 and args[0] == "list":
-            return CLISource(list_workflows)
+            return CLISource(list_workflows, required_permissions={Permission.read})
         else:
-            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+            return CLISource.single(
+                lambda: stream.just(self.rendered_help(ctx)), required_permissions={Permission.read}
+            )
 
 
 @make_parser
 def path_value_parser() -> Parser:
     key = yield variable_p
     yield equals_p
     value = yield json_value_p
@@ -4480,41 +4529,45 @@
 
         async def list_configs() -> Tuple[int, Stream]:
             ids = [i async for i in self.dependencies.config_handler.list_config_ids()]
             return len(ids), stream.iterate(ids)
 
         args = re.split("\\s+", arg, maxsplit=2) if arg else []
         if arg and len(args) == 2 and (args[0] == "show" or args[0] == "get"):
-            return CLISource.single(partial(show_config, args[1]))
+            return CLISource.single(partial(show_config, args[1]), required_permissions={Permission.admin})
         elif arg and len(args) == 2 and args[0] == "delete":
-            return CLISource.single(partial(delete_config, args[1]))
+            return CLISource.single(partial(delete_config, args[1]), required_permissions={Permission.admin})
         elif arg and len(args) == 3 and args[0] == "set":
             update = path_values_parser.parse(args[2])
-            return CLISource.single(partial(set_config, args[1], update))
+            return CLISource.single(partial(set_config, args[1], update), required_permissions={Permission.admin})
         elif arg and len(args) == 2 and args[0] == "edit":
             config_id = args[1]
             return CLISource.single(
                 partial(edit_config, config_id),
                 produces=MediaType.FilePath,
                 envelope={CLIEnvelope.action: "edit", CLIEnvelope.command: f"configs update {config_id}"},
+                required_permissions={Permission.admin},
             )
         elif arg and len(args) == 3 and args[0] == "copy":
-            return CLISource.single(partial(copy_config, args[1], args[2]))
+            return CLISource.single(partial(copy_config, args[1], args[2]), required_permissions={Permission.admin})
         elif arg and len(args) == 3 and args[0] == "update":
             config_id = args[1]
             return CLISource.single(
                 partial(update_config, config_id),
                 produces=MediaType.FilePath,
                 envelope={CLIEnvelope.action: "edit", CLIEnvelope.command: f"configs update {config_id}"},
                 requires=[CLIFileRequirement("config.yaml", args[2])],
+                required_permissions={Permission.admin},
             )
         elif arg and len(args) == 1 and args[0] == "list":
-            return CLISource(list_configs)
+            return CLISource(list_configs, required_permissions={Permission.read})
         else:
-            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+            return CLISource.single(
+                lambda: stream.just(self.rendered_help(ctx)), required_permissions={Permission.read}
+            )
 
 
 @lru_cache(maxsize=1024)
 def get_session_strategy(policy: SuggestionPolicy, session_id: str, clouds: FrozenSet[str]) -> SuggestionStrategy:
     return get_suggestion_strategy(policy, clouds)
 
 
@@ -4594,15 +4647,15 @@
                     "[b]> totd[/b] to see another tip of the day"
                 )
             )
 
             res = ctx.render_console(grid)
             return res
 
-        return CLISource.single(lambda: stream.just(welcome()))
+        return CLISource.single(lambda: stream.just(welcome()), required_permissions={Permission.read})
 
 
 class TipOfTheDayCommand(CLICommand):
     """
     ```shell
     totd
     ```
@@ -4631,15 +4684,15 @@
             else:
                 confiugured_collectors = frozenset()
             add_tod_block(info, SuggestionPolicy.NON_REPEATING, ctx.env.get("session_id", ""), confiugured_collectors)
 
             res = ctx.render_console(info)
             return res
 
-        return CLISource.single(lambda: stream.just(totd()))
+        return CLISource.single(lambda: stream.just(totd()), required_permissions={Permission.read})
 
 
 class CertificateCommand(CLICommand):
     """
     ```shell
     certificate create --common-name <common-name> [--dns-names <dns-name>...<dns-name>] \
     [--ip-addresses <ip-address>...<ip-address>] [--days-valid <days-valid>]
@@ -4705,17 +4758,20 @@
             parsed = parser.parse_args(args[1].split())
             return CLISource.with_count(
                 partial(
                     create_certificate, parsed.common_name, parsed.dns_names, parsed.ip_addresses, parsed.days_valid
                 ),
                 2,
                 produces=MediaType.FilePath,
+                required_permissions={Permission.admin},
             )
         else:
-            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+            return CLISource.single(
+                lambda: stream.just(self.rendered_help(ctx)), required_permissions={Permission.read}
+            )
 
 
 class ReportCommand(CLICommand, EntityProvider):
     """
     ```shell
     report benchmarks list
     report benchmark show <benchmark-id>
@@ -4896,29 +4952,29 @@
         run_parser.add_argument("--severity", type=ReportSeverity, choices=list(ReportSeverity))
         run_parser.add_argument("--only-failing", action="store_true", default=False)
         run_parser.add_argument("--only-check-results", action="store_true", default=False)
 
         action = self.action_from_arg(arg)
         args = re.split("\\s+", arg.strip(), maxsplit=2) if arg else []
         if action == "benchmark_list":
-            return CLISource.no_count(list_benchmarks)
+            return CLISource.no_count(list_benchmarks, required_permissions={Permission.read})
         elif action == "benchmark_show":
-            return CLISource.no_count(partial(show_benchmark, args[2].strip()))
+            return CLISource.no_count(partial(show_benchmark, args[2].strip()), required_permissions={Permission.read})
         elif action == "benchmark_run":
             parsed = run_parser.parse_args(args[2].split() if len(args) > 2 else [])
-            return CLISource.no_count(partial(run_benchmark, parsed))
+            return CLISource.no_count(partial(run_benchmark, parsed), required_permissions={Permission.read})
         elif action == "check_list":
-            return CLISource.no_count(list_checks)
+            return CLISource.no_count(list_checks, required_permissions={Permission.read})
         elif action == "check_show":
-            return CLISource.no_count(partial(show_check, args[2].strip()))
+            return CLISource.no_count(partial(show_check, args[2].strip()), required_permissions={Permission.read})
         elif action == "check_run":
             parsed = run_parser.parse_args(args[2].split() if len(args) > 2 else [])
-            return CLISource.no_count(partial(run_check, parsed))
+            return CLISource.no_count(partial(run_check, parsed), required_permissions={Permission.read})
         else:
-            return CLISource.single(show_help)
+            return CLISource.single(show_help, required_permissions={Permission.read})
 
 
 class AppsCommand(CLICommand):
     """
     ```shell
     apps search [pattern] [--index-url https://cdn.some.engineering/resoto/apps/index.json]
     app info <app_name> [--index-url https://cdn.some.engineering/resoto/apps/index.json]
@@ -5094,67 +5150,76 @@
 
         args = re.split("\\s+", arg, maxsplit=2) if arg else []
         if len(args) == 1 and args[0] == "search":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("--index-url", dest="url", type=str)
             parsed = parser.parse_args(strip_quotes(arg or "").split())
-            return CLISource.single(partial(apps_search, None, parsed.url))
+            return CLISource.single(partial(apps_search, None, parsed.url), required_permissions={Permission.read})
         elif len(args) >= 2 and args[0] == "search":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("pattern", type=str, nargs="*")
             parser.add_argument("--index-url", dest="url", type=str)
             parsed = parser.parse_args(strip_quotes(arg or "").split())
-            return CLISource.single(partial(apps_search, " ".join(parsed.pattern), parsed.url))
+            return CLISource.single(
+                partial(apps_search, " ".join(parsed.pattern), parsed.url), required_permissions={Permission.read}
+            )
         elif len(args) == 2 and args[0] == "info":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("app_name", type=str)
             parser.add_argument("--index-url", dest="url", type=str)
             parsed = parser.parse_args(strip_quotes(arg or "").split())
-            return CLISource.single(partial(app_info, InfraAppName(parsed.app_name), parsed.url))
+            return CLISource.single(
+                partial(app_info, InfraAppName(parsed.app_name), parsed.url), required_permissions={Permission.read}
+            )
         elif len(args) >= 2 and args[0] == "install":
             parser = NoExitArgumentParser()
             source_group = parser.add_mutually_exclusive_group()
             source_group.add_argument("--index-url", dest="url", type=str)
             parser.add_argument("command", type=str)
             parser.add_argument("app_name", type=str)
             parsed = parser.parse_args(strip_quotes(arg or "").split())
 
             return CLISource.single(
                 partial(
                     app_install,
                     InfraAppName(parsed.app_name),
                     parsed.url,
-                )
+                ),
+                required_permissions={Permission.admin},
             )
         elif arg and len(args) == 2 and args[0] == "edit":
             app_name = InfraAppName(args[1])
             return CLISource.single(
                 partial(edit_app, app_name),
                 produces=MediaType.FilePath,
                 envelope={CLIEnvelope.action: "edit", CLIEnvelope.command: f"apps update {app_name}"},
+                required_permissions={Permission.admin},
             )
         elif arg and len(args) == 3 and args[0] == "update":
             app_name = InfraAppName(args[1])
             return CLISource.single(
                 partial(update_app, app_name),
                 produces=MediaType.FilePath,
                 envelope={CLIEnvelope.action: "edit", CLIEnvelope.command: f"apps update {app_name}"},
                 requires=[CLIFileRequirement("manifest.yaml", args[2])],
+                required_permissions={Permission.admin},
             )
         elif len(args) == 2 and args[0] == "uninstall":
-            return CLISource.single(partial(app_uninstall, InfraAppName(args[1])))
+            return CLISource.single(
+                partial(app_uninstall, InfraAppName(args[1])), required_permissions={Permission.admin}
+            )
         elif len(args) == 2 and args[0] == "update" and args[1] == "all":
-            return CLISource.single(app_update_all)
+            return CLISource.single(app_update_all, required_permissions={Permission.admin})
         elif len(args) == 2 and args[0] == "update":
-            return CLISource.single(partial(app_update, InfraAppName(args[1])))
+            return CLISource.single(partial(app_update, InfraAppName(args[1])), required_permissions={Permission.admin})
         elif len(args) == 1 and args[0] == "list":
-            return CLISource.single(apps_list)
+            return CLISource.single(apps_list, required_permissions={Permission.read})
         elif len(args) >= 2 and args[0] == "run":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("app_name", type=str)
             parser.add_argument("--dry-run", dest="dry_run", action="store_true", default=False)
             parser.add_argument("--config", dest="config", type=str, default=None)
             parsed, argv = parser.parse_known_args(args_parts_parser.parse(arg))
@@ -5166,28 +5231,32 @@
                     partial(
                         app_run,
                         in_stream=stream.empty(),
                         app_name=InfraAppName(parsed.app_name),
                         dry_run=parsed.dry_run,
                         config=parsed.config,
                         argv=argv,
-                    )
+                    ),
+                    required_permissions={Permission.read},
                 )
             else:
                 return CLIFlow(
                     partial(
                         app_run,
                         app_name=InfraAppName(parsed.app_name),
                         dry_run=parsed.dry_run,
                         config=parsed.config,
                         argv=argv,
-                    )
+                    ),
+                    required_permissions={Permission.read},
                 )
         else:
-            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+            return CLISource.single(
+                lambda: stream.just(self.rendered_help(ctx)), required_permissions={Permission.read}
+            )
 
 
 class UserCommand(CLICommand):
     """
     ```shell
     user add <email> --fullname <name> --password <secret> --role <role> --role <role>
     user delete <email>
@@ -5271,15 +5340,15 @@
                 ArgInfo(None, True, help_text="<email>"),
                 ArgInfo("--fullname", True, help_text="<name>"),
                 ArgInfo("--password", True, help_text="<secret>"),
                 ArgInfo(
                     "--role",
                     True,
                     help_text="<role>",
-                    possible_values=list(ValidRoles),
+                    possible_values=list(AllowedRoleNames),
                     can_occur_multiple_times=True,
                 ),
             ],
             "delete": [
                 ArgInfo(None, True, help_text="<email>"),
             ],
             "role": {
@@ -5351,37 +5420,48 @@
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         args = args_parts_unquoted_parser.parse(arg.strip()) if arg else []
         if len(args) >= 2 and args[0] == "add":
             parser = NoExitArgumentParser()
             parser.add_argument("email", type=str)
             parser.add_argument("--fullname", type=str, required=True)
             parser.add_argument("--password", type=str, required=True)
-            parser.add_argument("--role", type=str, action="append", required=True)
+            parser.add_argument("--role", type=str, action="append", required=True, choices=AllowedRoleNames)
             parsed = parser.parse_args(args[1:])
             return CLISource.single(
                 partial(self.add_user, Email(parsed.email), parsed.fullname, Password(parsed.password), parsed.role),
                 envelope={CLIEnvelope.no_history: "yes"},
+                required_permissions={Permission.admin},
             )
         elif len(args) == 2 and args[0].startswith("del"):
-            return CLISource.single(partial(self.delete_user, Email(args[1])))
+            return CLISource.single(partial(self.delete_user, Email(args[1])), required_permissions={Permission.admin})
         elif len(args) > 3 and args[0] == "role" and args[1] == "add":
-            return CLISource.single(partial(self.add_roles, Email(args[2]), args[3]))
+            assert args[3] in AllowedRoleNames, "Role must be one of: " + ", ".join(AllowedRoleNames)
+            return CLISource.single(
+                partial(self.add_roles, Email(args[2]), args[3]), required_permissions={Permission.admin}
+            )
         elif len(args) > 3 and args[0] == "role" and args[1].startswith("del"):
-            return CLISource.single(partial(self.delete_role, Email(args[2]), args[3]))
+            return CLISource.single(
+                partial(self.delete_role, Email(args[2]), args[3]), required_permissions={Permission.admin}
+            )
         elif len(args) >= 3 and args[0] in ("passwd", "password"):
+            user_email = ctx.user.email if ctx.user else None
+            email = Email(args[1])
             return CLISource.single(
-                partial(self.change_password, Email(args[1]), Password(args[2])),
+                partial(self.change_password, email, Password(args[2])),
                 envelope={CLIEnvelope.no_history: "yes"},
+                required_permissions={Permission.read} if user_email == email else {Permission.admin},
             )
         elif len(args) == 1 and args[0] == "list":
-            return CLISource.no_count(self.list_users)
+            return CLISource.no_count(self.list_users, required_permissions={Permission.read})
         elif len(args) == 2 and args[0] == "show":
-            return CLISource.no_count(partial(self.show_user, args[1]))
+            return CLISource.no_count(partial(self.show_user, args[1]), required_permissions={Permission.read})
         else:
-            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+            return CLISource.single(
+                lambda: stream.just(self.rendered_help(ctx)), required_permissions={Permission.read}
+            )
 
 
 class GraphCommand(CLICommand):
     """
     ```shell
     graph list [pattern]
     graph copy [--force] [from_graph_namae] <to_graph_name>
@@ -5389,24 +5469,24 @@
     graph delete <graph_name>
     graph export [--force] [graph_name] <file_name>
     graph import [--force] [graph_name] <file_name>
     ```
 
     - `graph list [pattern]`: Lists all graphs. Supports filtering by pattern.
     - `graph copy [--force] [from_graph_name] <to_graph_name>`: Copies the graph.
-       If the target graph alearly exists, and a --force flag is provided, the graph will be overwritten.
+       If the target graph already exists, and a --force flag is provided, the graph will be overwritten.
     - `graph snapshot [from_graph_name] <snapshot_label>`: Make a graph snapshot.
     - `graph delete <graph_name>`: Delete a graph.
     - `graph export [--force] [graph_name] <file_name>`: Export the graph into a file. If the file already exists,
        and a --force flag is provided, the file will be overwritten.
-    - `graph import [--force] [graph_name] <file_name>`: Impor the graph from a file. If the graph already exists,
+    - `graph import [--force] [graph_name] <file_name>`: Import the graph from a file. If the graph already exists,
        and a --force flag is provided, the graph will be overwritten.
 
     ## Parameters
-    - `pattern` [optional]: Pattern for searching for graps. Supports regex.
+    - `pattern` [optional]: Pattern for searching for graphs. Supports regex.
     - `from_graph_name` [required]: The name of the graph to make a copy or snapshot from.
     - `to_graph_name` [optional]: The name of the target graph to make a copy.
        If not specified, the name of the current graph is used.
     - `file_name` [required]: The name of the file to save the graph to.
 
     ## Options
     - `--force`: Overwrite the target graph or file if it already exists.
@@ -5507,62 +5587,74 @@
 
         args = re.split("\\s+", arg, maxsplit=2) if arg else []
         if args[0] == "list":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("pattern", type=str, nargs="?", default=None)
             parsed = parser.parse_args(strip_quotes(arg or "").split())
-            return CLISource.single(partial(graph_list, parsed.pattern))
+            return CLISource.single(partial(graph_list, parsed.pattern), required_permissions={Permission.read})
         elif args[0] == "copy":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("source", type=str, nargs="?", default=None)
             parser.add_argument("destination", type=str)
             parser.add_argument("--force", action="store_true")
             parsed = parser.parse_args(strip_quotes(arg or "").split())
             return CLISource.single(
-                partial(graph_copy, GraphName(parsed.source), GraphName(parsed.destination), parsed.force)
+                partial(graph_copy, GraphName(parsed.source), GraphName(parsed.destination), parsed.force),
+                required_permissions={Permission.admin},
             )
         elif args[0] == "snapshot":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("source", type=str, nargs="?", default=None)
             parser.add_argument("label", type=str)
             parsed = parser.parse_args(strip_quotes(arg or "").split())
-            return CLISource.single(partial(graph_snapshot, parsed.source, parsed.label))
+            return CLISource.single(
+                partial(graph_snapshot, parsed.source, parsed.label), required_permissions={Permission.admin}
+            )
         elif args[0] == "delete":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("graph_name", type=str)
             parsed = parser.parse_args(strip_quotes(arg or "").split())
-            return CLISource.single(partial(graph_delete, GraphName(parsed.graph_name)))
+            return CLISource.single(
+                partial(graph_delete, GraphName(parsed.graph_name)), required_permissions={Permission.admin}
+            )
         elif args[0] == "export":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("graph_name", type=str, nargs="?", default=None)
             parser.add_argument("file_name", type=str)
             parser.add_argument("--force", action="store_true")
             parsed = parser.parse_args(strip_quotes(arg or "").split())
-            return CLISource.single(partial(graph_export, parsed.graph_name, parsed.file_name), MediaType.FilePath)
+            return CLISource.single(
+                partial(graph_export, parsed.graph_name, parsed.file_name),
+                MediaType.FilePath,
+                required_permissions={Permission.read},
+            )
         elif args[0] == "import":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("graph_name", type=str, nargs="?", default=None)
             parser.add_argument("file_name", type=str)
             parser.add_argument("--force", action="store_true")
             parsed = parser.parse_args(strip_quotes(arg or "").split())
 
             return CLISource.single(
                 partial(graph_import, parsed.graph_name, parsed.file_name, parsed.force),
                 MediaType.Json,
                 [CLIFileRequirement("dump", parsed.file_name)],
+                required_permissions={Permission.admin},
             )
 
         else:
-            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+            return CLISource.single(
+                lambda: stream.just(self.rendered_help(ctx)), required_permissions={Permission.read}
+            )
 
 
 class DbCommand(CLICommand, PreserveOutputFormat):
     """
     ```
     db sync <db-engine> --host <host> --port <port> --user <user> --password <password> --database <database>
                    --arg key=value --arg key2=value2
@@ -5795,21 +5887,23 @@
             produces = MediaType.FilePath if parsed_args.db == "sqlite" else MediaType.Json
             if in_source_position:
                 # in this position we fall back to exporting the whole graph
                 return CLISource.single(
                     fn=partial(sync_database_result, parsed_args, None),
                     envelope={CLIEnvelope.no_history: "yes"},
                     produces=produces,
+                    required_permissions={Permission.read},
                 )
             else:
                 # sync = partial(database_synchronize, db_config, p.complete_schema, p.drop_existing_tables, ctx.query)
                 return CLIFlow(
                     fn=partial(sync_database_result, parsed_args),
                     envelope={CLIEnvelope.no_history: "yes"},
                     produces=produces,
+                    required_permissions={Permission.read},
                 )
         else:
             raise AttributeError("Wrong or insufficient arguments. Execute `help db` to get more information.")
 
 
 def all_commands(d: Dependencies) -> List[CLICommand]:
     commands = [
```

### Comparing `resotocore-3.6.4/resotocore/cli/model.py` & `resotocore-3.6.5/resotocore/cli/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from rich.jupyter import JupyterMixin
 
 from resotocore.cli import JsGen, T, Sink
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 from resotocore.core_config import AliasTemplateConfig, AliasTemplateParameterConfig
 from resotocore.error import CLIParseError
 from resotocore.ids import GraphName
+from resotocore.user.model import Permission, AuthorizedUser
 from resotocore.query.model import Query, variable_to_absolute, PathRoot
 from resotocore.query.template_expander import render_template
 from resotocore.types import Json, JsonElement
 from resotocore.util import AccessJson, uuid_str, from_utc, utc, utc_str
 from resotolib.parse_util import l_curly_dp, r_curly_dp
 from resotolib.utils import get_local_tzinfo
 
@@ -104,19 +105,24 @@
     env: Dict[str, str] = field(factory=dict)
     uploaded_files: Dict[str, str] = field(factory=dict)  # id -> path
     query: Optional[Query] = None
     query_options: Dict[str, Any] = field(factory=dict)
     commands: List[ExecutableCommand] = field(factory=list)
     console_renderer: Optional[ConsoleRenderer] = None
     source: Optional[str] = None  # who is calling
+    user: Optional[AuthorizedUser] = None
 
     @property
     def graph_name(self) -> GraphName:
         return GraphName(self.env["graph"])
 
+    @property
+    def user_permissions(self) -> Set[Permission]:
+        return self.user.permissions if self.user else set()
+
     def variable_in_section(self, variable: str) -> str:
         # if there is no entity provider, always assume the root section
         section = (
             self.env.get("section")
             if self.query or self.commands and isinstance(self.commands[0].command, EntityProvider)
             else PathRoot
         )
@@ -204,88 +210,98 @@
 @define
 class CLIFileRequirement(CLICommandRequirement):
     path: str  # local client path
 
 
 class CLIAction(ABC):
     def __init__(
-        self, produces: MediaType, requires: Optional[List[CLICommandRequirement]], envelope: Optional[Dict[str, str]]
+        self,
+        produces: MediaType,
+        requires: Optional[List[CLICommandRequirement]],
+        envelope: Optional[Dict[str, str]],
+        required_permissions: Optional[Set[Permission]] = None,
     ) -> None:
         self.produces = produces
         self.required = requires or []
         self.envelope: Dict[str, str] = envelope or {}
+        self.required_permissions = required_permissions or set()
 
     @staticmethod
     def make_stream(in_stream: JsGen) -> Stream:
         return in_stream if isinstance(in_stream, Stream) else stream.iterate(in_stream)
 
 
 class CLISource(CLIAction):
     def __init__(
         self,
         fn: Callable[[], Union[Tuple[Optional[int], JsGen], Awaitable[Tuple[Optional[int], JsGen]]]],
         produces: MediaType = MediaType.Json,
         requires: Optional[List[CLICommandRequirement]] = None,
         envelope: Optional[Dict[str, str]] = None,
+        required_permissions: Optional[Set[Permission]] = None,
     ) -> None:
-        super().__init__(produces, requires, envelope)
+        super().__init__(produces, requires, envelope, required_permissions)
         self._fn = fn
 
     async def source(self) -> Tuple[Optional[int], Stream]:
         res = self._fn()
         count, gen = await res if iscoroutine(res) else res
         return count, self.make_stream(await gen if iscoroutine(gen) else gen)
 
     @staticmethod
     def no_count(
         fn: Callable[[], Union[JsGen, Awaitable[JsGen]]],
         produces: MediaType = MediaType.Json,
         requires: Optional[List[CLICommandRequirement]] = None,
         envelope: Optional[Dict[str, str]] = None,
+        required_permissions: Optional[Set[Permission]] = None,
     ) -> CLISource:
-        return CLISource.with_count(fn, None, produces, requires, envelope)
+        return CLISource.with_count(fn, None, produces, requires, envelope, required_permissions)
 
     @staticmethod
     def with_count(
         fn: Callable[[], Union[JsGen, Awaitable[JsGen]]],
         count: Optional[int],
         produces: MediaType = MediaType.Json,
         requires: Optional[List[CLICommandRequirement]] = None,
         envelope: Optional[Dict[str, str]] = None,
+        required_permissions: Optional[Set[Permission]] = None,
     ) -> CLISource:
         async def combine() -> Tuple[Optional[int], JsGen]:
             res = fn()
             gen = await res if iscoroutine(res) else res
             return count, gen
 
-        return CLISource(combine, produces, requires, envelope)
+        return CLISource(combine, produces, requires, envelope, required_permissions)
 
     @staticmethod
     def single(
         fn: Callable[[], Union[JsGen, Awaitable[JsGen]]],
         produces: MediaType = MediaType.Json,
         requires: Optional[List[CLICommandRequirement]] = None,
         envelope: Optional[Dict[str, str]] = None,
+        required_permissions: Optional[Set[Permission]] = None,
     ) -> CLISource:
-        return CLISource.with_count(fn, 1, produces, requires, envelope)
+        return CLISource.with_count(fn, 1, produces, requires, envelope, required_permissions)
 
     @staticmethod
     def empty() -> CLISource:
         return CLISource.with_count(stream.empty, 0)
 
 
 class CLIFlow(CLIAction):
     def __init__(
         self,
         fn: Callable[[JsGen], Union[JsGen, Awaitable[JsGen]]],
         produces: MediaType = MediaType.Json,
         requires: Optional[List[CLICommandRequirement]] = None,
         envelope: Optional[Dict[str, str]] = None,
+        required_permissions: Optional[Set[Permission]] = None,
     ) -> None:
-        super().__init__(produces, requires, envelope)
+        super().__init__(produces, requires, envelope, required_permissions)
         self._fn = fn
 
     async def flow(self, in_stream: JsGen) -> Stream:
         gen = self._fn(self.make_stream(in_stream))
         return self.make_stream(await gen if iscoroutine(gen) else gen)
 
 
@@ -670,14 +686,19 @@
         return [part.command for part in self.executable_commands]
 
     @property
     def produces(self) -> MediaType:
         # the last command in the chain defines the resulting media type
         return self.executable_commands[-1].action.produces if self.executable_commands else MediaType.Json
 
+    def is_allowed_to_execute(self) -> bool:
+        if self.ctx.user is None:
+            return False
+        return all(self.ctx.user.has_permission(cmd.action.required_permissions) for cmd in self.executable_commands)
+
     async def execute(self) -> Tuple[Optional[int], Stream]:
         if self.executable_commands:
             source_action = cast(CLISource, self.executable_commands[0].action)
             count, flow = await source_action.source()
             for command in self.executable_commands[1:]:
                 flow_action = cast(CLIFlow, command.action)
                 flow = await flow_action.flow(flow)
```

### Comparing `resotocore-3.6.4/resotocore/cli/tip_of_the_day.py` & `resotocore-3.6.5/resotocore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/config/__init__.py` & `resotocore-3.6.5/resotocore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/config/config_handler_service.py` & `resotocore-3.6.5/resotocore/config/config_handler_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/config/config_override_service.py` & `resotocore-3.6.5/resotocore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/config/core_config_handler.py` & `resotocore-3.6.5/resotocore/config/core_config_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/console_renderer.py` & `resotocore-3.6.5/resotocore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/constants.py` & `resotocore-3.6.5/resotocore/constants.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/core_config.py` & `resotocore-3.6.5/resotocore/core_config.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/__init__.py` & `resotocore-3.6.5/resotocore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/arango_query.py` & `resotocore-3.6.5/resotocore/db/arango_query.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/arangodb_extensions.py` & `resotocore-3.6.5/resotocore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/arangodb_functions.py` & `resotocore-3.6.5/resotocore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/async_arangodb.py` & `resotocore-3.6.5/resotocore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/configdb.py` & `resotocore-3.6.5/resotocore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/db_access.py` & `resotocore-3.6.5/resotocore/db/db_access.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/deferredouteredgedb.py` & `resotocore-3.6.5/resotocore/db/deferredouteredgedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/entitydb.py` & `resotocore-3.6.5/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/graphdb.py` & `resotocore-3.6.5/resotocore/db/graphdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/model.py` & `resotocore-3.6.5/resotocore/db/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/packagedb.py` & `resotocore-3.6.5/resotocore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/runningtaskdb.py` & `resotocore-3.6.5/resotocore/db/runningtaskdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/system_data_db.py` & `resotocore-3.6.5/resotocore/db/system_data_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/db/usagedb.py` & `resotocore-3.6.5/resotocore/db/usagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/dependencies.py` & `resotocore-3.6.5/resotocore/dependencies.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/error.py` & `resotocore-3.6.5/resotocore/error.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from typing import Set, Any
+
+from aiohttp import web
+
 from resotocore.ids import GraphName
 
 
 class CoreException(Exception):
     pass
 
 
@@ -92,7 +96,17 @@
 
 class RestartService(SystemExit):
     code = 1
 
     def __init__(self, reason: str) -> None:
         super().__init__(f"RestartService due to: {reason}")
         self.reason = reason
+
+
+class NotEnoughPermissions(web.HTTPForbidden):
+    def __init__(self, user_permissions: Set[Any], required_permissions: Set[Any]) -> None:
+        super().__init__(
+            text=f"Not allowed to perform this operation. "
+            f"Missing permission: {', '.join(a.name for a in (required_permissions-user_permissions))}"
+        )
+        self.user_permissions = user_permissions
+        self.required_permissions = required_permissions
```

### Comparing `resotocore-3.6.4/resotocore/graph_manager/graph_manager.py` & `resotocore-3.6.5/resotocore/graph_manager/graph_manager.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/infra_apps/local_runtime.py` & `resotocore-3.6.5/resotocore/infra_apps/local_runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/infra_apps/manifest.py` & `resotocore-3.6.5/resotocore/infra_apps/manifest.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/infra_apps/package_manager.py` & `resotocore-3.6.5/resotocore/infra_apps/package_manager.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/infra_apps/runtime.py` & `resotocore-3.6.5/resotocore/infra_apps/runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/api/contents/all.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.03125%*

 * *Differences: {"'additionalProperties'": 'False',*

 * * "'description'": "'Inspector settings.'",*

 * * "'jupyter.lab.menus'": "OrderedDict([('main', [OrderedDict([('id', 'jp-mainmenu-help'), ('items', "*

 * *                        "[OrderedDict([('type', 'separator'), ('rank', 0.1)]), "*

 * *                        "OrderedDict([('command', 'inspector:open'), ('rank', 0.1)]), "*

 * *                        "OrderedDict([('type', 'separator'), ('rank', 0.1)])])])])])",*

 * * "'jupyter.lab.shortcuts'": "[OrderedDict([('command', 'inspector:open'), (' […]*

```diff
@@ -1,25 +1,37 @@
 {
-    "content": [
+    "additionalProperties": false,
+    "description": "Inspector settings.",
+    "jupyter.lab.menus": {
+        "main": [
+            {
+                "id": "jp-mainmenu-help",
+                "items": [
+                    {
+                        "rank": 0.1,
+                        "type": "separator"
+                    },
+                    {
+                        "command": "inspector:open",
+                        "rank": 0.1
+                    },
+                    {
+                        "rank": 0.1,
+                        "type": "separator"
+                    }
+                ]
+            }
+        ]
+    },
+    "jupyter.lab.shortcuts": [
         {
-            "content": null,
-            "created": "2023-07-24T18:35:44.178445Z",
-            "format": null,
-            "last_modified": "2023-07-24T18:30:59.738697Z",
-            "mimetype": null,
-            "name": "example.ipynb",
-            "path": "example.ipynb",
-            "size": 7611,
-            "type": "notebook",
-            "writable": true
+            "command": "inspector:open",
+            "keys": [
+                "Accel I"
+            ],
+            "selector": "body"
         }
     ],
-    "created": "2023-07-24T18:35:44.178445Z",
-    "format": "json",
-    "last_modified": "2023-07-24T18:35:44.178445Z",
-    "mimetype": null,
-    "name": "",
-    "path": "",
-    "size": null,
-    "type": "directory",
-    "writable": true
+    "properties": {},
+    "title": "Inspector",
+    "type": "object"
 }
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/bootstrap.js` & `resotocore-3.6.5/resotocore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1037.51967a2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1037.51967a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1079.cdbaf67.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1079.cdbaf67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1084.4cd1c89.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1084.4cd1c89.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1113.23c9417.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1113.23c9417.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1125.129d070.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1125.129d070.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1163.ac28297.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1163.ac28297.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1221.c51249a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1221.c51249a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1245.be46619.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1245.be46619.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1261.199fc1d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1261.199fc1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1272.f334098.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1272.f334098.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1278.0524a4a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1278.0524a4a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt` & `resotocore-3.6.5/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1290.3981211.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1290.3981211.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1295.46e72b8.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1295.46e72b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1310.23bbe67.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1310.23bbe67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1320.21effe3.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1320.21effe3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1325.f76267c.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1325.f76267c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1408.7461890.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1408.e049d91.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,18 +2,18 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [1408], {
         31408: (e, t, o) => {
             o.r(t), o.d(t, {
                 main: () => f
             });
             var r = o(67504),
-                s = o(66737),
+                s = o(71354),
                 l = o(55941);
             const a = Promise.all([o.e(9344), o.e(8698), o.e(8005)]).then(o.bind(o, 36368)),
-                n = [o.e(5367).then(o.t.bind(o, 55367, 23))],
+                n = [o.e(3124).then(o.t.bind(o, 43124, 23))],
                 i = ["@jupyterlab/apputils-extension:workspaces", "@jupyterlab/application-extension:logo", "@jupyterlab/application-extension:main", "@jupyterlab/application-extension:tree-resolver", "@jupyterlab/apputils-extension:resolver", "@jupyterlab/docmanager-extension:download", "@jupyterlab/filebrowser-extension:download", "@jupyterlab/filebrowser-extension:share-file", "@jupyterlab/help-extension:about"];
             async function c(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (o) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${t}`), o
                 }
@@ -60,15 +60,15 @@
                 if (!b.has("@jupyterlab/vega5-extension")) try {
                     let e = o(30126);
                     for (let t of x(e)) j.push(t)
                 } catch (e) {
                     console.error(e)
                 }
                 if (!b.has("@jupyterlite/iframe-extension")) try {
-                    let e = o(41754);
+                    let e = o(19611);
                     for (let t of x(e)) j.push(t)
                 } catch (e) {
                     console.error(e)
                 }
                 if ((await Promise.allSettled(f)).forEach((e => {
                         if ("fulfilled" === e.status)
                             for (let t of x(e.value)) j.push(t);
@@ -268,15 +268,15 @@
                 if (!b.has("@jupyterlab/ui-components-extension")) try {
                     let t = o(7087);
                     for (let o of x(t)) e.push(o)
                 } catch (e) {
                     console.error(e)
                 }
                 if (!b.has("@jupyterlite/application-extension")) try {
-                    let t = o(95863);
+                    let t = o(34019);
                     for (let o of x(t)) e.push(o)
                 } catch (e) {
                     console.error(e)
                 }(await Promise.allSettled(t)).forEach((t => {
                     if ("fulfilled" === t.status)
                         for (let o of x(t.value)) e.push(o);
                     else console.error(t.reason)
@@ -303,8 +303,8 @@
                     disabled: i
                 });
                 w.name = l.PageConfig.getOption("appName") || "JupyterLite", w.registerPluginModules(e), "true" === (l.PageConfig.getOption("exposeAppInBrowser") || "").toLowerCase() && (window.jupyterapp = w), await w.start(), await w.restored
             }
         }
     }
 ]);
-//# sourceMappingURL=1408.7461890.js.map
+//# sourceMappingURL=1408.e049d91.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1440.a9e7ea1.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1440.a9e7ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1483.616d9ab.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1483.616d9ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1489.e50b6d4.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1489.e50b6d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1507.5705605.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1507.5705605.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/152.525d460.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/152.525d460.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1520.4e2eb21.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1520.4e2eb21.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1555.e188f3f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1555.e188f3f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1559.7c89925.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1559.7c89925.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/160.5f28731.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/160.5f28731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1603.370a2a6.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1603.370a2a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1644.0e49167.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1644.0e49167.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1667.f0afb2b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1667.f0afb2b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1687.27f1ad6.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1687.27f1ad6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1725.f151c33.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1725.f151c33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1767.c8c2f26.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1767.c8c2f26.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1806.1aaf66b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1806.1aaf66b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1838.1202b16.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1838.1202b16.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1909.28a2def.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1909.28a2def.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/1989.88d258f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/1989.88d258f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2030.1562cc6.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2030.1562cc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2047.baed97b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2047.baed97b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2099.f4b6fcd.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2099.f4b6fcd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2118.5b65f70.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2118.5b65f70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/213.5769e57.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/213.5769e57.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2161.dcb27b8.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2161.dcb27b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2169.635c88e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2169.635c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/217.90d10e2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/217.90d10e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2212.72be094.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2212.72be094.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2287.997c38e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2287.997c38e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt` & `resotocore-3.6.5/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2303.9ff8710.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2303.9ff8710.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2319.6b4cbb7.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2319.6b4cbb7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2329.4c5ca6d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2329.4c5ca6d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2351.fbd96d8.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2351.fbd96d8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2358.d5cf7c8.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2358.d5cf7c8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2359.6451c3e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2359.6451c3e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/237.f765e77.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/237.f765e77.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2384.71782be.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2384.71782be.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/240.cddc46b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/240.cddc46b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2431.648d237.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2431.648d237.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2546.1f48267.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2546.1f48267.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2557.75e9da2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9960.2d4eeed.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [2557, 9960], {
+    [9960, 2557], {
         2557: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => v
             });
             var a = o(67504),
                 n = o(2814),
                 r = o(55941),
                 i = o(42422),
                 c = o(83288),
                 l = o(84920),
                 s = o(49005),
                 d = o(4265),
                 p = o(59674),
-                u = o(26243),
+                u = o(58318),
                 m = o(43892),
                 b = o(94519),
                 h = o(96571),
                 f = o(62471),
                 g = o.n(f);
             const y = new RegExp("/(lab|notebooks|edit|consoles)\\/?");
             var w;
@@ -303,8 +303,8 @@
                             label: a.__("Copy Shareable Link")
                         })
                     }
                 }]
         }
     }
 ]);
-//# sourceMappingURL=2557.75e9da2.js.map
+//# sourceMappingURL=9960.2d4eeed.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/261.5f53c0e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/261.5f53c0e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2629.c0e1cd6.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2629.c0e1cd6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2788.46acc8a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2788.46acc8a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2834.942acc6.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2834.942acc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2887.47ba752.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2887.47ba752.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2956.8880209.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2956.8880209.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/2973.2a51dc4.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2973.2a51dc4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3004.255e79c.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3004.255e79c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/302.8bcc38f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/302.fad99ac.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -739,19 +739,17 @@
             }
             class I {
                 constructor(t) {
                     this.isDisposed = !1, this._onMessage = async t => {
                         if (!this._channel) return;
                         const {
                             _contents: e
-                        } = this, a = t.data, {
-                            path: s
-                        } = a;
+                        } = this, a = t.data, s = null == a ? void 0 : a.path;
                         let i, r = null;
-                        switch (a.method) {
+                        switch (null == a ? void 0 : a.method) {
                             case "readdir":
                                 i = await e.get(s, {
                                     content: !0
                                 }), r = [], "directory" === i.type && i.content && (r = i.content.map((t => t.name)));
                                 break;
                             case "rmdir":
                                 await e.delete(s);
@@ -831,8 +829,8 @@
                 dispose() {
                     this.isDisposed || (this.disable(), this.isDisposed = !0)
                 }
             }
         }
     }
 ]);
-//# sourceMappingURL=302.8bcc38f.js.map
+//# sourceMappingURL=302.fad99ac.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3037.70ee38d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3037.70ee38d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3042.7cfad84.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3042.7cfad84.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3051.34fac68.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3051.34fac68.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3122.2289fca.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3122.2289fca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3151.10ef4de.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3151.10ef4de.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/316.c850a76.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/316.c850a76.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3196.4e35a17.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3196.4e35a17.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3265.a80440a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3265.a80440a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3277.9c04e75.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3277.9c04e75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/330.126fa98.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/330.126fa98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3392.29fe6b9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3392.29fe6b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3413.480a49d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3413.480a49d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3444.47d5ea1.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3444.808a22d.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         63444: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => l
             });
             var n = o(69041),
                 a = o(55941),
                 r = o(42422),
-                i = o(26243),
+                i = o(58318),
                 s = o(94519),
                 c = o(95191);
             const l = [{
                 id: "@jupyterlite/retro-application-extension:consoles",
                 requires: [n.IConsoleTracker],
                 autoStart: !0,
                 activate: (e, t) => {
@@ -70,8 +70,8 @@
                         }))
                     }))
                 }
             }]
         }
     }
 ]);
-//# sourceMappingURL=3444.47d5ea1.js.map
+//# sourceMappingURL=3444.808a22d.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3469.7d14d0b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3469.7d14d0b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3546.fee1bd7.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3546.fee1bd7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/362.6716970.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/362.6716970.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3708.410d087.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3708.410d087.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3850.903abc2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3850.903abc2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt` & `resotocore-3.6.5/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3880.bd39dce.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3880.bd39dce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3970.236586f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3970.236586f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3976.58893b9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3976.58893b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt` & `resotocore-3.6.5/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/3979.385527e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/3979.385527e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/400.d72234b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/400.d72234b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4018.1a35967.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4018.1a35967.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/406.9b7af92.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/406.9b7af92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4117.a8107fd.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4117.a8107fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4182.e2430f9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4182.e2430f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4191.02bbea8.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4191.02bbea8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4197.53ab10b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4197.53ab10b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4206.a5f8bb0.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4206.a5f8bb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4207.0d0580b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4207.0d0580b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4262.bb73457.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4262.bb73457.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4298.5ee510c.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4298.5ee510c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/44.0cfa785.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/44.0cfa785.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt` & `resotocore-3.6.5/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4410.e4a25d3.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4410.e4a25d3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4466.64d23d1.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4466.64d23d1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/451.d9683ad.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/451.d9683ad.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4535.34b060a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4535.34b060a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4565.43bdb91.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4565.43bdb91.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4569.f374f9d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4569.f374f9d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4615.eb5d40a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4615.eb5d40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4658.090d4a9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4658.090d4a9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4690.3dd4096.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4690.3dd4096.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4715.e7690b9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4715.e7690b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4749.46ebbb2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4749.46ebbb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4750.56c06ab.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4750.56c06ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4856.2d7415f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4856.2d7415f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4875.375150e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4875.375150e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/489.b981dea.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/489.b981dea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/490.c2624d4.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/490.c2624d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4905.667bf33.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4905.667bf33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4931.430433b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8732.20136c6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [4931, 8732], {
+    [8732, 4931], {
         24931: (e, t, s) => {
             s.r(t), s.d(t, {
                 default: () => O
             });
             var n = s(55941),
-                r = s(29790),
-                a = s(79850),
-                o = s(35151),
-                i = s(66737),
-                c = s(40371),
-                u = s(73968),
-                l = s(1258),
-                p = s(88052),
+                r = s(84021),
+                a = s(51154),
+                o = s(64822),
+                i = s(71354),
+                c = s(25262),
+                u = s(94523),
+                l = s(48531),
+                p = s(70007),
                 g = s(29440),
                 y = s.n(g);
             const w = {
                     id: "@jupyterlite/server-extension:localforage",
                     autoStart: !0,
                     provides: p.ILocalForage,
                     activate: e => ({
@@ -313,8 +313,8 @@
                             return new Response(JSON.stringify(n))
                         }))
                     }
                 }]
         }
     }
 ]);
-//# sourceMappingURL=4931.430433b.js.map
+//# sourceMappingURL=8732.20136c6.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/4942.b96c164.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4942.b96c164.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5016.dd2fe83.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5016.dd2fe83.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5072.733a1b5.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5072.733a1b5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/509.6448878.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/509.6448878.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5096.8ed0d8e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5096.8ed0d8e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5126.eecad7a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5126.eecad7a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5129.1ba4763.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5129.1ba4763.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5153.763d8fa.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5153.763d8fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5155.06b4ea9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5155.06b4ea9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5193.e9f6866.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5193.e9f6866.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5213.3e1a360.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5213.3e1a360.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5227.8c8acd8.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5227.8c8acd8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5238.1751cc3.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5238.f0f5af0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -73,29 +73,29 @@
             }]);
             const a = r
         },
         77600: (e, t, n) => {
             n.r(t), n.d(t, {
                 main: () => A
             });
-            var i = n(66737),
+            var i = n(71354),
                 o = n(55941);
             n(4436);
-            const s = [n.e(5367).then(n.t.bind(n, 55367, 23))],
-                r = [n.e(1754).then(n.t.bind(n, 41754, 23)), n.e(3946).then(n.t.bind(n, 23946, 23)), n.e(9265).then(n.t.bind(n, 29265, 23)), n.e(126).then(n.t.bind(n, 30126, 23))];
+            const s = [n.e(3124).then(n.t.bind(n, 43124, 23))],
+                r = [n.e(9611).then(n.t.bind(n, 19611, 23)), n.e(3946).then(n.t.bind(n, 23946, 23)), n.e(9265).then(n.t.bind(n, 29265, 23)), n.e(126).then(n.t.bind(n, 30126, 23))];
             async function a(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (n) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${t}`), n
                 }
             }
             async function A() {
                 const e = await Promise.all(r);
-                let t = [n(95863), n(80963), n(88394).default.filter((({
+                let t = [n(34019), n(33829), n(88394).default.filter((({
                     id: e
                 }) => !["@retrolab/application-extension:logo", "@retrolab/application-extension:opener"].includes(e))), n(31161), n(61474), n(29507).default.filter((({
                     id: e
                 }) => ["@jupyterlab/application-extension:commands", "@jupyterlab/application-extension:context-menu", "@jupyterlab/application-extension:faviconbusy"].includes(e))), n(10310).default.filter((({
                     id: e
                 }) => ["@jupyterlab/apputils-extension:palette", "@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:state", "@jupyterlab/apputils-extension:themes", "@jupyterlab/apputils-extension:themes-palette-menu", "@jupyterlab/apputils-extension:toolbar-registry"].includes(e))), n(15802).default.filter((({
                     id: e
@@ -229,8 +229,8 @@
             e.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%270 0 16 16%27%3e%3cpath fill-rule=%27evenodd%27 clip-rule=%27evenodd%27 d=%27M11 7H5c-.55 0-1 .45-1 1s.45 1 1 1h6c.55 0 1-.45 1-1s-.45-1-1-1z%27 fill=%27white%27/%3e%3c/svg%3e"
         },
         79080: e => {
             e.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%270 0 16 16%27%3e%3cpath fill-rule=%27evenodd%27 clip-rule=%27evenodd%27 d=%27M12 5c-.28 0-.53.11-.71.29L7 9.59l-2.29-2.3a1.003 1.003 0 00-1.42 1.42l3 3c.18.18.43.29.71.29s.53-.11.71-.29l5-5A1.003 1.003 0 0012 5z%27 fill=%27white%27/%3e%3c/svg%3e"
         }
     }
 ]);
-//# sourceMappingURL=5238.1751cc3.js.map
+//# sourceMappingURL=5238.f0f5af0.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/528.2262cb0.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/528.2262cb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5292.79d4aba.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5292.79d4aba.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5437.31236f7.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5437.31236f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5489.848a8cf.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5489.848a8cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5508.317fca3.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5508.317fca3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/554.ac98303.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/554.ac98303.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/555.2cd31dd.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/555.2cd31dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5573.ebcdb93.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5573.ebcdb93.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5666.c5e5324.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5666.c5e5324.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5710.70d0b1d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5710.70d0b1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5747.94ad626.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5747.94ad626.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/582.21b8e7d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/582.21b8e7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5823.5045bdb.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5823.5045bdb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5851.30b7b2a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5851.30b7b2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5878.32d92fa.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5878.32d92fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5880.68f975b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5880.68f975b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5955.88508f7.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5955.88508f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/5971.88c5642.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/5971.88c5642.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6080.aa0ff24.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6080.aa0ff24.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/61.2808a0d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/61.2808a0d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6136.b8ba2b2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6136.b8ba2b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6141.9831d58.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6141.9831d58.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6475.6037fbb.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6475.22d38af.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,16 +6,16 @@
                 default: () => g
             });
             var r = o(67504),
                 n = o(2814),
                 a = o(69041),
                 i = o(4265),
                 s = o(59674),
-                c = o(84997),
-                d = o(26243),
+                c = o(75225),
+                d = o(58318),
                 l = o(94519);
             const u = "jupyterlite",
                 p = {
                     id: "@jupyterlite/console-application:buttons",
                     autoStart: !0,
                     requires: [i.ITranslator],
                     optional: [a.IConsoleTracker],
@@ -144,8 +144,8 @@
                         })), a
                     }
                 },
                 g = [p, m, w, b, h]
         }
     }
 ]);
-//# sourceMappingURL=6475.6037fbb.js.map
+//# sourceMappingURL=6475.22d38af.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6493.d796aa5.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6493.d796aa5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6556.b3d9293.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6556.b3d9293.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6571.2c8884e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6571.2c8884e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6576.3ea568e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6576.3ea568e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6591.94ed352.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6591.94ed352.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6612.1632879.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6612.1632879.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6623.ae3b3cc.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6623.ae3b3cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6664.2160109.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6664.2160109.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6747.47be7f5.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6747.47be7f5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6748.be68f5f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6748.be68f5f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6870.7940288.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6870.7940288.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6879.c8367a5.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6879.c8367a5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6898.9bbc12a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6898.9bbc12a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6952.f68b818.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6952.f68b818.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6985.321ad92.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6985.321ad92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6993.32cf9a6.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6993.32cf9a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/6997.b06fe71.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/6997.b06fe71.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7041.d4f561e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7041.d4f561e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7058.805c88e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7058.805c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7174.6c45206.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7174.6c45206.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7334.8859b1b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7334.8859b1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7359.6ee65ec.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7359.6ee65ec.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7364.195178b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7364.195178b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7380.58a4413.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7380.58a4413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7427.f9c2017.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7427.f9c2017.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7463.18fd278.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7463.18fd278.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7509.1e0189e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7509.1e0189e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7526.1a303e5.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7526.1a303e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7537.1323a15.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7537.1323a15.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7692.33d5169.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7692.33d5169.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7746.5908d29.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7746.5908d29.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7808.1d582a2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7808.1d582a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/783.c156751.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/783.c156751.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7858.2386e4d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7858.2386e4d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/7941.01ea680.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/7941.01ea680.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8005.c5ad7b2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8005.c5ad7b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8028.39e2fa1.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8028.39e2fa1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8061.cc62561.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8061.cc62561.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8101.cf46d02.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8101.cf46d02.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/812.9b0e86e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/812.9b0e86e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/816.c8050f2.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/816.c8050f2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8165.b2c3285.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8165.b2c3285.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8232.a578bf9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8232.a578bf9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/824.8678196.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/824.8678196.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8270.89fe7e1.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8270.89fe7e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/833.9cc6653.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/833.9cc6653.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8370.8f855e5.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8370.8678c18.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -6,16 +6,16 @@
                 default: () => g
             });
             var r = o(67504),
                 n = o(2814),
                 a = o(69041),
                 i = o(4265),
                 s = o(59674),
-                c = o(84997),
-                d = o(26243),
+                c = o(75225),
+                d = o(58318),
                 l = o(94519);
             const u = "jupyterlite",
                 p = {
                     id: "@jupyterlite/console-application:buttons",
                     autoStart: !0,
                     requires: [i.ITranslator],
                     optional: [a.IConsoleTracker],
@@ -144,8 +144,8 @@
                         })), a
                     }
                 },
                 g = [p, m, w, b, h]
         }
     }
 ]);
-//# sourceMappingURL=8370.8f855e5.js.map
+//# sourceMappingURL=8370.8678c18.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8373.96b0b3a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8373.96b0b3a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8389.ffe031f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8389.ffe031f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8412.1528057.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8412.1528057.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8427.4923f43.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8427.4923f43.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8542.027afdc.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8542.027afdc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8594.0112f03.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8594.0112f03.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8656.d5b8e92.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8656.d5b8e92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8685.d78bdab.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8685.13b9daf.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -91,29 +91,29 @@
             }]);
             const r = s
         },
         13242: (e, n, t) => {
             t.r(n), t.d(n, {
                 main: () => a
             });
-            var A = t(66737),
+            var A = t(71354),
                 i = t(55941);
             t(36865);
-            const o = [t.e(5367).then(t.t.bind(t, 55367, 23))],
-                s = [t.e(1754).then(t.t.bind(t, 41754, 23)), t.e(3946).then(t.t.bind(t, 23946, 23)), t.e(9265).then(t.t.bind(t, 29265, 23)), t.e(126).then(t.t.bind(t, 30126, 23))];
+            const o = [t.e(3124).then(t.t.bind(t, 43124, 23))],
+                s = [t.e(9611).then(t.t.bind(t, 19611, 23)), t.e(3946).then(t.t.bind(t, 23946, 23)), t.e(9265).then(t.t.bind(t, 29265, 23)), t.e(126).then(t.t.bind(t, 30126, 23))];
             async function r(e, n) {
                 try {
                     return (await window._JUPYTERLAB[e].get(n))()
                 } catch (t) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${n}`), t
                 }
             }
             async function a() {
                 const e = await Promise.all(s);
-                let n = [t(95863), t(97857), t(88394).default.filter((({
+                let n = [t(34019), t(85609), t(88394).default.filter((({
                     id: e
                 }) => ["@retrolab/application-extension:session-dialogs"].includes(e))), t(29507).default.filter((({
                     id: e
                 }) => ["@jupyterlab/application-extension:commands", "@jupyterlab/application-extension:context-menu", "@jupyterlab/application-extension:faviconbusy"].includes(e))), t(10310).default.filter((({
                     id: e
                 }) => ["@jupyterlab/apputils-extension:palette", "@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:state", "@jupyterlab/apputils-extension:themes", "@jupyterlab/apputils-extension:themes-palette-menu"].includes(e))), t(15802).default.filter((({
                     id: e
@@ -162,15 +162,15 @@
                 }));
                 const h = new A.JupyterLiteServer({});
                 h.registerPluginModules(u), await h.start();
                 const {
                     serviceManager: E
                 } = h, {
                     SingleWidgetApp: C
-                } = t(84997), y = new C({
+                } = t(75225), y = new C({
                     serviceManager: E,
                     mimeExtensions: e
                 });
                 y.name = i.PageConfig.getOption("appName") || "REPLite", y.registerPluginModules(a), "true" === (i.PageConfig.getOption("exposeAppInBrowser") || "").toLowerCase() && (window.jupyterapp = y), await y.start(), await y.restored
             }
         },
         36865: (e, n, t) => {
@@ -219,8 +219,8 @@
             e.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%270 0 16 16%27%3e%3cpath fill-rule=%27evenodd%27 clip-rule=%27evenodd%27 d=%27M11 7H5c-.55 0-1 .45-1 1s.45 1 1 1h6c.55 0 1-.45 1-1s-.45-1-1-1z%27 fill=%27white%27/%3e%3c/svg%3e"
         },
         79080: e => {
             e.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%270 0 16 16%27%3e%3cpath fill-rule=%27evenodd%27 clip-rule=%27evenodd%27 d=%27M12 5c-.28 0-.53.11-.71.29L7 9.59l-2.29-2.3a1.003 1.003 0 00-1.42 1.42l3 3c.18.18.43.29.71.29s.53-.11.71-.29l5-5A1.003 1.003 0 0012 5z%27 fill=%27white%27/%3e%3c/svg%3e"
         }
     }
 ]);
-//# sourceMappingURL=8685.d78bdab.js.map
+//# sourceMappingURL=8685.13b9daf.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8698.9817d75.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8698.9817d75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8732.9320f73.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/4931.47d8e25.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [8732, 4931], {
+    [4931, 8732], {
         24931: (e, t, s) => {
             s.r(t), s.d(t, {
                 default: () => O
             });
             var n = s(55941),
-                r = s(29790),
-                a = s(79850),
-                o = s(35151),
-                i = s(66737),
-                c = s(40371),
-                u = s(73968),
-                l = s(1258),
-                p = s(88052),
+                r = s(84021),
+                a = s(51154),
+                o = s(64822),
+                i = s(71354),
+                c = s(25262),
+                u = s(94523),
+                l = s(48531),
+                p = s(70007),
                 g = s(29440),
                 y = s.n(g);
             const w = {
                     id: "@jupyterlite/server-extension:localforage",
                     autoStart: !0,
                     provides: p.ILocalForage,
                     activate: e => ({
@@ -313,8 +313,8 @@
                             return new Response(JSON.stringify(n))
                         }))
                     }
                 }]
         }
     }
 ]);
-//# sourceMappingURL=8732.9320f73.js.map
+//# sourceMappingURL=4931.47d8e25.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8785.cf4fe95.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8785.cf4fe95.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8828.77c71d0.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8828.77c71d0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8883.80c7b63.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8883.80c7b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8976.3816942.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8976.3816942.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/8990.2a453cf.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/8990.2a453cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9035.1e45c1b.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9035.1e45c1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9053.45b77fc.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9053.45b77fc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9077.fefb6ca.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9077.fefb6ca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9128.b8fa6f0.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9128.b8fa6f0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9156.0cefbd3.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9156.0cefbd3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9170.0023587.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9170.0023587.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9196.315f9f9.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9196.315f9f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9198.9971d70.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9198.9971d70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/920.d15c177.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/920.d15c177.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9253.0b31caa.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9253.0b31caa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9266.bacd0dd.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9266.bacd0dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9307.c3a00ed.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9307.c3a00ed.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9321.869e413.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9321.869e413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9344.ba0abcf.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9344.ba0abcf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9382.9014799.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9382.144ed35.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         63444: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => l
             });
             var n = o(69041),
                 a = o(55941),
                 r = o(42422),
-                i = o(26243),
+                i = o(58318),
                 s = o(94519),
                 c = o(95191);
             const l = [{
                 id: "@jupyterlite/retro-application-extension:consoles",
                 requires: [n.IConsoleTracker],
                 autoStart: !0,
                 activate: (e, t) => {
@@ -70,8 +70,8 @@
                         }))
                     }))
                 }
             }]
         }
     }
 ]);
-//# sourceMappingURL=9382.9014799.js.map
+//# sourceMappingURL=9382.144ed35.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9440.1b10b8f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9440.1b10b8f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9464.79e6ac5.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9464.79e6ac5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9502.9a24831.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9502.9a24831.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9507.1e6cc5d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9507.1e6cc5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9602.62bf0f1.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9602.62bf0f1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9621.e2e8b5d.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9621.e2e8b5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9622.ccab065.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9622.ccab065.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9626.a178bd0.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9626.a178bd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9647.ed91993.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9647.ed91993.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9657.bc5c60e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9657.bc5c60e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/97.ad126b0.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/97.ad126b0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9712.796a0a1.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9712.796a0a1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9737.7dc8f98.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9737.7dc8f98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9777.0b8a504.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9777.0b8a504.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9793.6d63a85.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9793.6d63a85.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9806.652c162.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9806.652c162.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9865.2e3db6f.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9865.2e3db6f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/989.bcca86a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/989.bcca86a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9943.f3f35c7.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9943.f3f35c7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9958.25c8c06.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/9958.25c8c06.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/9960.64cd61e.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/2557.6c85d56.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [9960, 2557], {
+    [2557, 9960], {
         2557: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => v
             });
             var a = o(67504),
                 n = o(2814),
                 r = o(55941),
                 i = o(42422),
                 c = o(83288),
                 l = o(84920),
                 s = o(49005),
                 d = o(4265),
                 p = o(59674),
-                u = o(26243),
+                u = o(58318),
                 m = o(43892),
                 b = o(94519),
                 h = o(96571),
                 f = o(62471),
                 g = o.n(f);
             const y = new RegExp("/(lab|notebooks|edit|consoles)\\/?");
             var w;
@@ -303,8 +303,8 @@
                             label: a.__("Copy Shareable Link")
                         })
                     }
                 }]
         }
     }
 ]);
-//# sourceMappingURL=9960.64cd61e.js.map
+//# sourceMappingURL=2557.6c85d56.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/add-above.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/add-above.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/add-below.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/add-below.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/bug-dot.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/bug-dot.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/bug.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/bug.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/build.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/build.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/case-sensitive.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/case-sensitive.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/close.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/close.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/copyright.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/copyright.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/cut.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/cut.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/duplicate.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/duplicate.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/fa-brands-400.woff2` & `resotocore-3.6.5/resotocore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/fa-regular-400.woff2` & `resotocore-3.6.5/resotocore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/fa-solid-900.woff2` & `resotocore-3.6.5/resotocore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/html5.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/html5.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/json.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/json.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/julia.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/julia.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/jupyter-favicon.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/jupyter-favicon.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/jupyter.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/jupyter.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/jupyterlab-wordmark.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/jupyterlab-wordmark.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/lab/bundle.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/lab/bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -28,15 +28,15 @@
                                 }))
                             }(e), await l.I("default");
                             const a = window._JUPYTERLAB[t];
                             await a.init(l.S.default)
                         }(`${t}/${e.name}/${e.load}`, e.name)
                     })))).forEach((e => {
                         "rejected" === e.status && console.error(e.reason)
-                    })), (0, (await Promise.all([l.e(5941), l.e(7504), l.e(6737), l.e(2437), l.e(8402), l.e(2813), l.e(1754), l.e(126), l.e(9265), l.e(3946), l.e(1408)]).then(l.bind(l, 31408))).main)()
+                    })), (0, (await Promise.all([l.e(5941), l.e(7504), l.e(1354), l.e(2437), l.e(4810), l.e(2813), l.e(9611), l.e(126), l.e(9265), l.e(3946), l.e(1408)]).then(l.bind(l, 31408))).main)()
                 }()
             }
         },
         g = {};
 
     function v(e) {
         var t = g[e];
@@ -83,15 +83,15 @@
         178: "3951873",
         192: "1338eee",
         213: "5769e57",
         217: "90d10e2",
         237: "f765e77",
         240: "cddc46b",
         261: "5f53c0e",
-        302: "8bcc38f",
+        302: "fad99ac",
         316: "c850a76",
         330: "126fa98",
         362: "6716970",
         400: "d72234b",
         406: "9b7af92",
         432: "df26495",
         435: "2cb088b",
@@ -110,15 +110,14 @@
         833: "9cc6653",
         901: "47f584a",
         920: "d15c177",
         942: "26b642e",
         985: "33027f6",
         989: "bcca86a",
         1037: "51967a2",
-        1066: "1617b5c",
         1079: "cdbaf67",
         1084: "4cd1c89",
         1091: "8c3d33c",
         1113: "23c9417",
         1125: "129d070",
         1163: "ac28297",
         1214: "2d2e136",
@@ -129,29 +128,29 @@
         1278: "0524a4a",
         1290: "3981211",
         1295: "46e72b8",
         1310: "23bbe67",
         1313: "3d9d403",
         1320: "21effe3",
         1325: "f76267c",
-        1408: "7461890",
+        1354: "b6ea256",
+        1408: "e049d91",
         1440: "a9e7ea1",
         1452: "4f1e027",
         1483: "616d9ab",
         1489: "e50b6d4",
         1507: "5705605",
         1520: "4e2eb21",
         1555: "e188f3f",
         1559: "7c89925",
         1563: "54f7cc1",
         1603: "370a2a6",
         1644: "0e49167",
         1667: "f0afb2b",
         1725: "f151c33",
-        1754: "a8b6a73",
         1767: "c8c2f26",
         1806: "1aaf66b",
         1838: "1202b16",
         1909: "28a2def",
         1981: "1fd1910",
         1989: "88d258f",
         2030: "1562cc6",
@@ -171,15 +170,15 @@
         2384: "71782be",
         2422: "a265166",
         2431: "648d237",
         2437: "23f27ab",
         2471: "045af38",
         2538: "a82c014",
         2546: "1f48267",
-        2557: "75e9da2",
+        2557: "6c85d56",
         2584: "36f9b42",
         2629: "c0e1cd6",
         2788: "46acc8a",
         2813: "04f4f89",
         2814: "ed35af6",
         2834: "942acc6",
         2867: "7e3670f",
@@ -192,25 +191,26 @@
         3037: "70ee38d",
         3042: "7cfad84",
         3050: "52f0308",
         3051: "34fac68",
         3059: "addbf2d",
         3079: "f2d6a4c",
         3122: "2289fca",
+        3124: "29a5871",
         3151: "10ef4de",
         3196: "4e35a17",
         3231: "16e97c3",
         3265: "a80440a",
         3277: "9c04e75",
         3288: "7d1feb0",
         3349: "10324ab",
         3383: "854f5fa",
         3392: "29fe6b9",
         3413: "480a49d",
-        3444: "47d5ea1",
+        3444: "808a22d",
         3469: "7d14d0b",
         3546: "fee1bd7",
         3708: "410d087",
         3752: "8735345",
         3850: "903abc2",
         3880: "bd39dce",
         3892: "2416867",
@@ -243,35 +243,35 @@
         4668: "f65690b",
         4690: "3dd4096",
         4715: "e7690b9",
         4749: "46ebbb2",
         4750: "56c06ab",
         4761: "a121143",
         4769: "dc84614",
+        4810: "4d75364",
         4853: "848774f",
         4856: "2d7415f",
         4875: "375150e",
         4905: "667bf33",
         4920: "7ae28ae",
-        4931: "430433b",
+        4931: "47d8e25",
         4957: "8bd6324",
-        4997: "18f4688",
         5016: "dd2fe83",
         5072: "733a1b5",
         5096: "8ed0d8e",
         5126: "eecad7a",
         5129: "1ba4763",
         5153: "763d8fa",
         5155: "06b4ea9",
         5191: "32af1b6",
         5193: "e9f6866",
         5213: "3e1a360",
+        5225: "79a0c27",
         5227: "8c8acd8",
         5292: "79d4aba",
-        5367: "b54b66d",
         5437: "31236f7",
         5489: "848a8cf",
         5508: "317fca3",
         5573: "ebcdb93",
         5666: "c5e5324",
         5710: "70d0b1d",
         5747: "94ad626",
@@ -284,29 +284,27 @@
         5955: "88508f7",
         5971: "88c5642",
         6070: "083c16b",
         6080: "aa0ff24",
         6136: "b8ba2b2",
         6141: "9831d58",
         6169: "ac54f5b",
-        6243: "77d9350",
         6274: "ec582c7",
         6464: "64a242d",
         6493: "d796aa5",
         6531: "00eb3dd",
         6556: "b3d9293",
         6571: "2c8884e",
         6576: "3ea568e",
         6591: "94ed352",
         6612: "1632879",
         6623: "ae3b3cc",
         6624: "9fa7bfd",
         6664: "2160109",
         6725: "7c44a22",
-        6737: "07c3940",
         6747: "47be7f5",
         6748: "be68f5f",
         6831: "a2a3b6b",
         6870: "7940288",
         6879: "c8367a5",
         6898: "9bbc12a",
         6952: "f68b818",
@@ -340,25 +338,26 @@
         8033: "8226698",
         8061: "cc62561",
         8101: "cf46d02",
         8165: "b2c3285",
         8232: "a578bf9",
         8270: "89fe7e1",
         8300: "f084e5d",
-        8370: "8f855e5",
+        8318: "9f3a0c8",
+        8370: "8678c18",
         8373: "96b0b3a",
         8389: "ffe031f",
-        8402: "f4d40da",
         8412: "1528057",
         8427: "4923f43",
+        8504: "830cb23",
         8542: "027afdc",
         8594: "0112f03",
         8656: "d5b8e92",
         8698: "9817d75",
-        8732: "9320f73",
+        8732: "20136c6",
         8741: "b138cb8",
         8785: "cf4fe95",
         8798: "165e59c",
         8828: "77c71d0",
         8883: "80c7b63",
         8976: "3816942",
         8981: "99a4275",
@@ -381,14 +380,15 @@
         9321: "869e413",
         9344: "ba0abcf",
         9440: "1b10b8f",
         9464: "79e6ac5",
         9502: "9a24831",
         9590: "3c1d14e",
         9602: "62bf0f1",
+        9611: "9ea75ca",
         9621: "e2e8b5d",
         9622: "ccab065",
         9626: "a178bd0",
         9647: "ed91993",
         9657: "bc5c60e",
         9674: "6c13954",
         9712: "796a0a1",
@@ -398,15 +398,15 @@
         9793: "6d63a85",
         9806: "652c162",
         9865: "2e3db6f",
         9915: "78886f9",
         9943: "f3f35c7",
         9957: "2d01a2e",
         9958: "25c8c06",
-        9960: "64cd61e"
+        9960: "2d4eeed"
     } [e] + ".js", v.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -458,15 +458,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : o > i.from)) && (r[t] = {
                             get: l,
                             from: o,
                             eager: !!a
                         })
                     },
                     s = [];
-                return "default" === l && (i("@jupyterlab/application-extension", "3.5.3", (() => Promise.all([v.e(316), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(2471), v.e(5786), v.e(7504), v.e(3231), v.e(3050), v.e(4020)]).then((() => () => v(30316))))), i("@jupyterlab/application", "3.5.3", (() => Promise.all([v.e(812), v.e(9198), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(3231), v.e(40), v.e(985), v.e(1313), v.e(4064), v.e(435), v.e(9116), v.e(6070)]).then((() => () => v(79198))))), i("@jupyterlab/apputils-extension", "3.5.3", (() => Promise.all([v.e(4856), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(3231), v.e(985), v.e(9005), v.e(1313), v.e(3050), v.e(2867), v.e(4920)]).then((() => () => v(74856))))), i("@jupyterlab/apputils", "3.5.3", (() => Promise.all([v.e(6623), v.e(6169), v.e(4265), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(5786), v.e(3231), v.e(1313), v.e(3050), v.e(4064), v.e(435), v.e(9116), v.e(3349), v.e(2877), v.e(2867), v.e(7711), v.e(3752)]).then((() => () => v(96623))))), i("@jupyterlab/attachments", "3.5.3", (() => Promise.all([v.e(942), v.e(40), v.e(2877), v.e(9128)]).then((() => () => v(9128))))), i("@jupyterlab/cell-toolbar-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(5155)]).then((() => () => v(15155))))), i("@jupyterlab/cell-toolbar", "3.5.3", (() => Promise.all([v.e(2814), v.e(3892), v.e(942), v.e(2877), v.e(362)]).then((() => () => v(80362))))), i("@jupyterlab/cells", "3.5.3", (() => Promise.all([v.e(1520), v.e(5193), v.e(6169), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(40), v.e(1313), v.e(3349), v.e(4853), v.e(3383), v.e(3059), v.e(6274), v.e(178), v.e(6531)]).then((() => () => v(75193))))), i("@jupyterlab/celltags-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(3079), v.e(8981)]).then((() => () => v(98981))))), i("@jupyterlab/celltags", "3.5.3", (() => Promise.all([v.e(4265), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(3079), v.e(6997)]).then((() => () => v(96997))))), i("@jupyterlab/codeeditor", "3.5.3", (() => Promise.all([v.e(6747), v.e(6169), v.e(4265), v.e(4519), v.e(9674), v.e(942), v.e(2877), v.e(6274)]).then((() => () => v(66747))))), i("@jupyterlab/codemirror-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(5786), v.e(7504), v.e(9005), v.e(6725), v.e(4853), v.e(6624), v.e(3059), v.e(1981), v.e(6493)]).then((() => () => v(66493))))), i("@jupyterlab/codemirror", "3.5.3", (() => Promise.all([v.e(5747), v.e(8373), v.e(5878), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2471), v.e(3231), v.e(1313), v.e(6725), v.e(4853), v.e(9915), v.e(1981)]).then((() => () => v(95878))))), i("@jupyterlab/completer-extension", "3.5.3", (() => Promise.all([v.e(4519), v.e(3892), v.e(3079), v.e(9041), v.e(6624), v.e(240)]).then((() => () => v(10240))))), i("@jupyterlab/completer", "3.5.3", (() => Promise.all([v.e(4565), v.e(6169), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(3050), v.e(4064), v.e(3349)]).then((() => () => v(94565))))), i("@jupyterlab/console-extension", "3.5.3", (() => Promise.all([v.e(4117), v.e(6169), v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(5786), v.e(7504), v.e(3231), v.e(40), v.e(9005), v.e(9041), v.e(9116), v.e(4853), v.e(4920), v.e(4761)]).then((() => () => v(14117))))), i("@jupyterlab/console", "3.5.3", (() => Promise.all([v.e(3265), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(40), v.e(2877), v.e(9590), v.e(1563)]).then((() => () => v(53469))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([v.e(8101), v.e(6169), v.e(942), v.e(5126)]).then((() => () => v(54705))))), i("@jupyterlab/csvviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(942), v.e(5786), v.e(7504), v.e(985), v.e(9005), v.e(192), v.e(901), v.e(7543), v.e(5096)]).then((() => () => v(15971))))), i("@jupyterlab/csvviewer", "3.5.3", (() => Promise.all([v.e(2431), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(985), v.e(901)]).then((() => () => v(82431))))), i("@jupyterlab/docmanager-extension", "3.5.3", (() => Promise.all([v.e(3392), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(2471), v.e(5786), v.e(7504), v.e(6725), v.e(2422), v.e(3288)]).then((() => () => v(90509))))), i("@jupyterlab/docmanager", "3.5.3", (() => Promise.all([v.e(6898), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2471), v.e(3231), v.e(985), v.e(6725), v.e(4064), v.e(9116)]).then((() => () => v(66898))))), i("@jupyterlab/docprovider", "3.5.3", (() => Promise.all([v.e(6879), v.e(528), v.e(1125), v.e(6169), v.e(9915)]).then((() => () => v(51125))))), i("@jupyterlab/docregistry", "3.5.3", (() => Promise.all([v.e(7941), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(3231), v.e(40), v.e(4064), v.e(4853), v.e(3059), v.e(6274), v.e(3288)]).then((() => () => v(17941))))), i("@jupyterlab/documentsearch-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(7504), v.e(192), v.e(5880)]).then((() => () => v(59035))))), i("@jupyterlab/documentsearch", "3.5.3", (() => Promise.all([v.e(8656), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(2471), v.e(3231), v.e(1313), v.e(3079), v.e(6624), v.e(9590), v.e(3059), v.e(1981)]).then((() => () => v(38656))))), i("@jupyterlab/filebrowser-extension", "3.5.3", (() => Promise.all([v.e(9806), v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(6725), v.e(3050), v.e(2422), v.e(2867), v.e(4920)]).then((() => () => v(59806))))), i("@jupyterlab/filebrowser", "3.5.3", (() => Promise.all([v.e(1489), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(985), v.e(1313), v.e(6725), v.e(2422), v.e(4064), v.e(435), v.e(3349), v.e(3383), v.e(1563)]).then((() => () => v(21489))))), i("@jupyterlab/fileeditor-extension", "3.5.3", (() => Promise.all([v.e(6136), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(9005), v.e(6725), v.e(9041), v.e(4853), v.e(6624), v.e(4920), v.e(4761)]).then((() => () => v(46136))))), i("@jupyterlab/fileeditor", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(2471), v.e(985), v.e(6725), v.e(4853), v.e(9253)]).then((() => () => v(9253))))), i("@jupyterlab/help-extension", "3.5.3", (() => Promise.all([v.e(3979), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(7504), v.e(9005), v.e(435), v.e(3383)]).then((() => () => v(93979))))), i("@jupyterlab/htmlviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9674), v.e(5786), v.e(7504), v.e(6464), v.e(2384)]).then((() => () => v(89793))))), i("@jupyterlab/htmlviewer", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(985), v.e(4197)]).then((() => () => v(74197))))), i("@jupyterlab/imageviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(7504), v.e(8033), v.e(1290)]).then((() => () => v(25129))))), i("@jupyterlab/imageviewer", "3.5.3", (() => Promise.all([v.e(6169), v.e(2814), v.e(4519), v.e(5941), v.e(985), v.e(8165)]).then((() => () => v(58165))))), i("@jupyterlab/inspector-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9674), v.e(7504), v.e(3079), v.e(9041), v.e(4761), v.e(1452), v.e(3708)]).then((() => () => v(17174))))), i("@jupyterlab/inspector", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(942), v.e(5941), v.e(40), v.e(1313), v.e(3050), v.e(9321)]).then((() => () => v(49321))))), i("@jupyterlab/javascript-extension", "3.5.3", (() => Promise.all([v.e(40), v.e(1113)]).then((() => () => v(41113))))), i("@jupyterlab/json-extension", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(2471), v.e(7711), v.e(3880)]).then((() => () => v(63880))))), i("@jupyterlab/launcher-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(7504), v.e(4761), v.e(3042)]).then((() => () => v(79626))))), i("@jupyterlab/launcher", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(3231), v.e(9116), v.e(9053)]).then((() => () => v(79053))))), i("@jupyterlab/logconsole-extension", "3.5.3", (() => Promise.all([v.e(9266), v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(942), v.e(2471), v.e(5786), v.e(7504), v.e(40), v.e(3079), v.e(6725), v.e(2538)]).then((() => () => v(9266))))), i("@jupyterlab/logconsole", "3.5.3", (() => Promise.all([v.e(3122), v.e(6169), v.e(4265), v.e(4519), v.e(942), v.e(40), v.e(178)]).then((() => () => v(3122))))), i("@jupyterlab/mainmenu-extension", "3.5.3", (() => Promise.all([v.e(7463), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(9005), v.e(435)]).then((() => () => v(97463))))), i("@jupyterlab/mainmenu", "3.5.3", (() => Promise.all([v.e(6169), v.e(4519), v.e(3892), v.e(9674), v.e(5072)]).then((() => () => v(55072))))), i("@jupyterlab/markdownviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5941), v.e(5786), v.e(7504), v.e(40), v.e(7737), v.e(3277)]).then((() => () => v(46985))))), i("@jupyterlab/markdownviewer", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(5941), v.e(40), v.e(985), v.e(2358)]).then((() => () => v(22358))))), i("@jupyterlab/mathjax2-extension", "3.5.3", (() => Promise.all([v.e(5941), v.e(40), v.e(8798), v.e(152)]).then((() => () => v(60152))))), i("@jupyterlab/mathjax2", "3.5.3", (() => Promise.all([v.e(6169), v.e(3469)]).then((() => () => v(13469))))), i("@jupyterlab/nbformat", "3.5.3", (() => Promise.all([v.e(6169), v.e(7526)]).then((() => () => v(97526))))), i("@jupyterlab/notebook-extension", "3.5.3", (() => Promise.all([v.e(4875), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(3231), v.e(40), v.e(9005), v.e(3079), v.e(6725), v.e(3050), v.e(2422), v.e(4064), v.e(435), v.e(4853), v.e(4920), v.e(4761), v.e(9590), v.e(4020), v.e(2538), v.e(2437)]).then((() => () => v(94206))))), i("@jupyterlab/notebook", "3.5.3", (() => Promise.all([v.e(2030), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(985), v.e(6725), v.e(4064), v.e(435), v.e(9116), v.e(3349), v.e(4853), v.e(2877), v.e(3383), v.e(9590), v.e(1563), v.e(6274), v.e(2930)]).then((() => () => v(92030))))), i("@jupyterlab/observables", "4.5.3", (() => Promise.all([v.e(97), v.e(6169), v.e(3892), v.e(942), v.e(3231), v.e(4064)]).then((() => () => v(60097))))), i("@jupyterlab/outputarea", "3.5.3", (() => Promise.all([v.e(3196), v.e(6169), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(40), v.e(435), v.e(9116), v.e(2877), v.e(2930)]).then((() => () => v(13196))))), i("@jupyterlab/pdf-extension", "3.5.3", (() => Promise.all([v.e(6169), v.e(4519), v.e(3231), v.e(490)]).then((() => () => v(80490))))), i("@jupyterlab/property-inspector", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(942), v.e(1295)]).then((() => () => v(21295))))), i("@jupyterlab/rendermime-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(40), v.e(2422), v.e(824)]).then((() => () => v(40824))))), i("@jupyterlab/rendermime-interfaces", "3.5.3", (() => v.e(4668).then((() => () => v(64668))))), i("@jupyterlab/rendermime", "3.5.3", (() => Promise.all([v.e(1520), v.e(1767), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2877), v.e(3059), v.e(2930), v.e(432)]).then((() => () => v(81767))))), i("@jupyterlab/running-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(985), v.e(2584), v.e(4466)]).then((() => () => v(51667))))), i("@jupyterlab/running", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(2471), v.e(3231), v.e(2319)]).then((() => () => v(22319))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([v.e(6591), v.e(6169), v.e(3892), v.e(942), v.e(5941), v.e(3231), v.e(1313), v.e(3050), v.e(8741)]).then((() => () => v(76591))))), i("@jupyterlab/settingeditor-extension", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(5786), v.e(7504), v.e(40), v.e(3050), v.e(4853), v.e(2973)]).then((() => () => v(80989))))), i("@jupyterlab/settingeditor", "3.5.3", (() => Promise.all([v.e(4658), v.e(9865), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(2471), v.e(40), v.e(1313), v.e(3050), v.e(4853), v.e(1452), v.e(4665)]).then((() => () => v(19865))))), i("@jupyterlab/settingregistry", "3.5.3", (() => Promise.all([v.e(4658), v.e(7537), v.e(8270), v.e(6169), v.e(942), v.e(3231), v.e(2867)]).then((() => () => v(98270))))), i("@jupyterlab/shared-models", "3.5.3", (() => Promise.all([v.e(6879), v.e(528), v.e(6993), v.e(6169), v.e(942), v.e(9915)]).then((() => () => v(56993))))), i("@jupyterlab/shortcuts-extension", "3.5.3", (() => Promise.all([v.e(2212), v.e(6169), v.e(4265), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(5786), v.e(3231), v.e(3349), v.e(2867), v.e(6831), v.e(8300)]).then((() => () => v(52212))))), i("@jupyterlab/statedb", "3.5.3", (() => Promise.all([v.e(1325), v.e(6169), v.e(942), v.e(9116)]).then((() => () => v(91325))))), i("@jupyterlab/statusbar-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9674), v.e(5786), v.e(7504), v.e(3079), v.e(6725), v.e(9041), v.e(2867), v.e(6624), v.e(1806)]).then((() => () => v(54715))))), i("@jupyterlab/statusbar", "3.5.3", (() => Promise.all([v.e(2161), v.e(5573), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(3231)]).then((() => () => v(65573))))), i("@jupyterlab/theme-dark-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9307)]).then((() => () => v(59307))))), i("@jupyterlab/theme-light-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(7746)]).then((() => () => v(37746))))), i("@jupyterlab/toc-extension", "5.5.3", (() => Promise.all([v.e(4265), v.e(9674), v.e(5786), v.e(7504), v.e(40), v.e(3079), v.e(2422), v.e(6624), v.e(9590), v.e(7737), v.e(1091), v.e(2788)]).then((() => () => v(80833))))), i("@jupyterlab/toc", "5.5.3", (() => Promise.all([v.e(8828), v.e(6169), v.e(4265), v.e(4519), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(3079), v.e(3349), v.e(9590), v.e(7711)]).then((() => () => v(6598))))), i("@jupyterlab/tooltip-extension", "3.5.3", (() => Promise.all([v.e(4519), v.e(3892), v.e(5941), v.e(40), v.e(3079), v.e(9041), v.e(6624), v.e(7908), v.e(8232)]).then((() => () => v(28232))))), i("@jupyterlab/tooltip", "3.5.3", (() => Promise.all([v.e(6169), v.e(2814), v.e(4519), v.e(40), v.e(1507)]).then((() => () => v(11507))))), i("@jupyterlab/translation-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(7504), v.e(9005), v.e(1440)]).then((() => () => v(61440))))), i("@jupyterlab/translation", "3.5.3", (() => Promise.all([v.e(2047), v.e(6169), v.e(5941), v.e(3050), v.e(435)]).then((() => () => v(52047))))), i("@jupyterlab/ui-components-extension", "3.5.3", (() => Promise.all([v.e(9674), v.e(9733)]).then((() => () => v(69733))))), i("@jupyterlab/ui-components", "3.5.3", (() => Promise.all([v.e(2161), v.e(3976), v.e(6169), v.e(4265), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2471), v.e(3231), v.e(3383), v.e(7711)]).then((() => () => v(33976))))), i("@jupyterlab/vega5-extension", "3.5.3", (() => Promise.all([v.e(4519), v.e(9712)]).then((() => () => v(79712))))), i("@jupyterlite/application-extension", "0.1.0", (() => Promise.all([v.e(6571), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(2471), v.e(7504), v.e(9005), v.e(2422), v.e(4920), v.e(6243), v.e(3288), v.e(2557)]).then((() => () => v(2557))))), i("@jupyterlite/application", "0.1.0", (() => Promise.all([v.e(812), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(3231), v.e(40), v.e(985), v.e(9116), v.e(4905)]).then((() => () => v(54905))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([v.e(9737), v.e(6169), v.e(5941), v.e(302)]).then((() => () => v(40302))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([v.e(6169), v.e(4519), v.e(6141)]).then((() => () => v(86141))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(5941), v.e(435), v.e(2877), v.e(2546)]).then((() => () => v(52546))))), i("@jupyterlite/licenses", "0.1.0", (() => Promise.all([v.e(6169), v.e(5941), v.e(9777)]).then((() => () => v(89777))))), i("@jupyterlite/localforage", "0.1.0", (() => Promise.all([v.e(6169), v.e(2329)]).then((() => () => v(2329))))), i("@jupyterlite/repl-extension", "0.1.0", (() => Promise.all([v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(7504), v.e(9041), v.e(6243), v.e(4997), v.e(8370)]).then((() => () => v(8370))))), i("@jupyterlite/retro-application-extension", "0.1.0", (() => Promise.all([v.e(4519), v.e(5941), v.e(2422), v.e(9041), v.e(6243), v.e(5191), v.e(3444)]).then((() => () => v(63444))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([v.e(9440), v.e(5941), v.e(6737), v.e(1066), v.e(4931)]).then((() => () => v(24931))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(5941), v.e(435), v.e(6070), v.e(1245)]).then((() => () => v(71245))))), i("@jupyterlite/session", "0.1.0", (() => Promise.all([v.e(6169), v.e(3892), v.e(5941), v.e(4298)]).then((() => () => v(14298))))), i("@jupyterlite/settings", "0.1.0", (() => Promise.all([v.e(7537), v.e(6169), v.e(5941), v.e(3151)]).then((() => () => v(53151))))), i("@jupyterlite/translation", "0.1.0", (() => Promise.all([v.e(6169), v.e(5941), v.e(816)]).then((() => () => v(90816))))), i("@jupyterlite/ui-components", "0.1.0", (() => Promise.all([v.e(9674), v.e(9958)]).then((() => () => v(59958))))), i("@lumino/algorithm", "1.9.2", (() => v.e(9943).then((() => () => v(99943))))), i("@lumino/application", "1.31.3", (() => Promise.all([v.e(1278), v.e(6169), v.e(4519), v.e(2867)]).then((() => () => v(61278))))), i("@lumino/commands", "1.21.1", (() => Promise.all([v.e(8061), v.e(6169), v.e(3892), v.e(942), v.e(3231), v.e(3349), v.e(6831)]).then((() => () => v(38061))))), i("@lumino/coreutils", "1.12.1", (() => v.e(8883).then((() => () => v(28883))))), i("@lumino/datagrid", "0.36.6", (() => Promise.all([v.e(920), v.e(6169), v.e(4519), v.e(3892), v.e(942), v.e(4064), v.e(3349), v.e(1563), v.e(6831)]).then((() => () => v(30920))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([v.e(3892), v.e(942), v.e(5851)]).then((() => () => v(35851))))), i("@lumino/domutils", "1.8.2", (() => v.e(1310).then((() => () => v(71310))))), i("@lumino/dragdrop", "1.14.4", (() => Promise.all([v.e(1084), v.e(3231)]).then((() => () => v(51084))))), i("@lumino/keyboard", "1.8.2", (() => v.e(8990).then((() => () => v(58990))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([v.e(3850), v.e(3892)]).then((() => () => v(23850))))), i("@lumino/polling", "1.11.3", (() => Promise.all([v.e(8594), v.e(6169), v.e(942)]).then((() => () => v(36107))))), i("@lumino/properties", "1.8.2", (() => v.e(1555).then((() => () => v(21555))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([v.e(3892), v.e(9116), v.e(8389)]).then((() => () => v(38389))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([v.e(5437), v.e(3892)]).then((() => () => v(75437))))), i("@lumino/widgets", "1.37.1", (() => Promise.all([v.e(5666), v.e(6169), v.e(3892), v.e(942), v.e(3231), v.e(4064), v.e(9116), v.e(3349), v.e(2867), v.e(3383), v.e(1563), v.e(6831)]).then((() => () => v(75666))))), i("@retrolab/application-extension", "0.3.21", (() => Promise.all([v.e(1559), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(5941), v.e(5786), v.e(7504), v.e(3231), v.e(985), v.e(9005), v.e(2422), v.e(9041), v.e(5191), v.e(4769)]).then((() => () => v(91559))))), i("@retrolab/application", "0.3.21", (() => Promise.all([v.e(812), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(3231), v.e(40), v.e(985), v.e(1313), v.e(4064), v.e(9116), v.e(6556)]).then((() => () => v(36556))))), i("@retrolab/help-extension", "0.3.21", (() => Promise.all([v.e(4265), v.e(2814), v.e(2471), v.e(9005), v.e(4769), v.e(8785)]).then((() => () => v(18785))))), i("@retrolab/notebook-extension", "0.3.21", (() => Promise.all([v.e(4265), v.e(2814), v.e(4519), v.e(5941), v.e(5786), v.e(9005), v.e(1313), v.e(3079), v.e(2422), v.e(5191), v.e(2099)]).then((() => () => v(2099))))), i("@retrolab/tree-extension", "0.3.21", (() => Promise.all([v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(4920), v.e(2584), v.e(9170)]).then((() => () => v(19170))))), i("@retrolab/ui-components", "0.3.21", (() => Promise.all([v.e(1644), v.e(9674)]).then((() => () => v(11644))))), i("codemirror", "5.61.1", (() => v.e(5747).then((() => () => v(25747))))), i("react-dom", "17.0.2", (() => Promise.all([v.e(2287), v.e(2471)]).then((() => () => v(42287))))), i("react-highlighter", "0.4.3", (() => Promise.all([v.e(7058), v.e(2471)]).then((() => () => v(87058))))), i("react-json-tree", "0.15.2", (() => Promise.all([v.e(4615), v.e(2471)]).then((() => () => v(34615))))), i("react", "17.0.2", (() => v.e(7427).then((() => () => v(47427))))), i("typestyle", "2.4.0", (() => v.e(1163).then((() => () => v(91163))))), i("vega-embed", "6.21.0", (() => Promise.all([v.e(44), v.e(1214), v.e(123)]).then((() => () => v(30044))))), i("vega-lite", "5.5.0", (() => Promise.all([v.e(61), v.e(1725), v.e(1214), v.e(8542)]).then((() => () => v(71725))))), i("vega", "5.23.0", (() => Promise.all([v.e(61), v.e(1603), v.e(4191)]).then((() => () => v(91603))))), i("yjs", "13.5.43", (() => Promise.all([v.e(6879), v.e(1221), v.e(4535)]).then((() => () => v(61221)))))), e[l] = s.length ? Promise.all(s).then((() => e[l] = 1)) : 1
+                return "default" === l && (i("@jupyterlab/application-extension", "3.5.3", (() => Promise.all([v.e(316), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(2471), v.e(5786), v.e(7504), v.e(3231), v.e(3050), v.e(4020)]).then((() => () => v(30316))))), i("@jupyterlab/application", "3.5.3", (() => Promise.all([v.e(812), v.e(9198), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(3231), v.e(40), v.e(985), v.e(1313), v.e(4064), v.e(435), v.e(9116), v.e(6070)]).then((() => () => v(79198))))), i("@jupyterlab/apputils-extension", "3.5.3", (() => Promise.all([v.e(4856), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(3231), v.e(985), v.e(9005), v.e(1313), v.e(3050), v.e(2867), v.e(4920)]).then((() => () => v(74856))))), i("@jupyterlab/apputils", "3.5.3", (() => Promise.all([v.e(6623), v.e(6169), v.e(4265), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(5786), v.e(3231), v.e(1313), v.e(3050), v.e(4064), v.e(435), v.e(9116), v.e(3349), v.e(2877), v.e(2867), v.e(7711), v.e(3752)]).then((() => () => v(96623))))), i("@jupyterlab/attachments", "3.5.3", (() => Promise.all([v.e(942), v.e(40), v.e(2877), v.e(9128)]).then((() => () => v(9128))))), i("@jupyterlab/cell-toolbar-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(5155)]).then((() => () => v(15155))))), i("@jupyterlab/cell-toolbar", "3.5.3", (() => Promise.all([v.e(2814), v.e(3892), v.e(942), v.e(2877), v.e(362)]).then((() => () => v(80362))))), i("@jupyterlab/cells", "3.5.3", (() => Promise.all([v.e(1520), v.e(5193), v.e(6169), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(40), v.e(1313), v.e(3349), v.e(4853), v.e(3383), v.e(3059), v.e(6274), v.e(178), v.e(6531)]).then((() => () => v(75193))))), i("@jupyterlab/celltags-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(3079), v.e(8981)]).then((() => () => v(98981))))), i("@jupyterlab/celltags", "3.5.3", (() => Promise.all([v.e(4265), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(3079), v.e(6997)]).then((() => () => v(96997))))), i("@jupyterlab/codeeditor", "3.5.3", (() => Promise.all([v.e(6747), v.e(6169), v.e(4265), v.e(4519), v.e(9674), v.e(942), v.e(2877), v.e(6274)]).then((() => () => v(66747))))), i("@jupyterlab/codemirror-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(5786), v.e(7504), v.e(9005), v.e(6725), v.e(4853), v.e(6624), v.e(3059), v.e(1981), v.e(6493)]).then((() => () => v(66493))))), i("@jupyterlab/codemirror", "3.5.3", (() => Promise.all([v.e(5747), v.e(8373), v.e(5878), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2471), v.e(3231), v.e(1313), v.e(6725), v.e(4853), v.e(9915), v.e(1981)]).then((() => () => v(95878))))), i("@jupyterlab/completer-extension", "3.5.3", (() => Promise.all([v.e(4519), v.e(3892), v.e(3079), v.e(9041), v.e(6624), v.e(240)]).then((() => () => v(10240))))), i("@jupyterlab/completer", "3.5.3", (() => Promise.all([v.e(4565), v.e(6169), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(3050), v.e(4064), v.e(3349)]).then((() => () => v(94565))))), i("@jupyterlab/console-extension", "3.5.3", (() => Promise.all([v.e(4117), v.e(6169), v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(5786), v.e(7504), v.e(3231), v.e(40), v.e(9005), v.e(9041), v.e(9116), v.e(4853), v.e(4920), v.e(4761)]).then((() => () => v(14117))))), i("@jupyterlab/console", "3.5.3", (() => Promise.all([v.e(3265), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(40), v.e(2877), v.e(9590), v.e(1563)]).then((() => () => v(53469))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([v.e(8101), v.e(6169), v.e(942), v.e(5126)]).then((() => () => v(54705))))), i("@jupyterlab/csvviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(942), v.e(5786), v.e(7504), v.e(985), v.e(9005), v.e(192), v.e(901), v.e(7543), v.e(5096)]).then((() => () => v(15971))))), i("@jupyterlab/csvviewer", "3.5.3", (() => Promise.all([v.e(2431), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(985), v.e(901)]).then((() => () => v(82431))))), i("@jupyterlab/docmanager-extension", "3.5.3", (() => Promise.all([v.e(3392), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(2471), v.e(5786), v.e(7504), v.e(6725), v.e(2422), v.e(3288)]).then((() => () => v(90509))))), i("@jupyterlab/docmanager", "3.5.3", (() => Promise.all([v.e(6898), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2471), v.e(3231), v.e(985), v.e(6725), v.e(4064), v.e(9116)]).then((() => () => v(66898))))), i("@jupyterlab/docprovider", "3.5.3", (() => Promise.all([v.e(6879), v.e(528), v.e(1125), v.e(6169), v.e(9915)]).then((() => () => v(51125))))), i("@jupyterlab/docregistry", "3.5.3", (() => Promise.all([v.e(7941), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(3231), v.e(40), v.e(4064), v.e(4853), v.e(3059), v.e(6274), v.e(3288)]).then((() => () => v(17941))))), i("@jupyterlab/documentsearch-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(7504), v.e(192), v.e(5880)]).then((() => () => v(59035))))), i("@jupyterlab/documentsearch", "3.5.3", (() => Promise.all([v.e(8656), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(2471), v.e(3231), v.e(1313), v.e(3079), v.e(6624), v.e(9590), v.e(3059), v.e(1981)]).then((() => () => v(38656))))), i("@jupyterlab/filebrowser-extension", "3.5.3", (() => Promise.all([v.e(9806), v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(6725), v.e(3050), v.e(2422), v.e(2867), v.e(4920)]).then((() => () => v(59806))))), i("@jupyterlab/filebrowser", "3.5.3", (() => Promise.all([v.e(1489), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(985), v.e(1313), v.e(6725), v.e(2422), v.e(4064), v.e(435), v.e(3349), v.e(3383), v.e(1563)]).then((() => () => v(21489))))), i("@jupyterlab/fileeditor-extension", "3.5.3", (() => Promise.all([v.e(6136), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(9005), v.e(6725), v.e(9041), v.e(4853), v.e(6624), v.e(4920), v.e(4761)]).then((() => () => v(46136))))), i("@jupyterlab/fileeditor", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(2471), v.e(985), v.e(6725), v.e(4853), v.e(9253)]).then((() => () => v(9253))))), i("@jupyterlab/help-extension", "3.5.3", (() => Promise.all([v.e(3979), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(7504), v.e(9005), v.e(435), v.e(3383)]).then((() => () => v(93979))))), i("@jupyterlab/htmlviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9674), v.e(5786), v.e(7504), v.e(6464), v.e(2384)]).then((() => () => v(89793))))), i("@jupyterlab/htmlviewer", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(985), v.e(4197)]).then((() => () => v(74197))))), i("@jupyterlab/imageviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(7504), v.e(8033), v.e(1290)]).then((() => () => v(25129))))), i("@jupyterlab/imageviewer", "3.5.3", (() => Promise.all([v.e(6169), v.e(2814), v.e(4519), v.e(5941), v.e(985), v.e(8165)]).then((() => () => v(58165))))), i("@jupyterlab/inspector-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9674), v.e(7504), v.e(3079), v.e(9041), v.e(4761), v.e(1452), v.e(3708)]).then((() => () => v(17174))))), i("@jupyterlab/inspector", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(942), v.e(5941), v.e(40), v.e(1313), v.e(3050), v.e(9321)]).then((() => () => v(49321))))), i("@jupyterlab/javascript-extension", "3.5.3", (() => Promise.all([v.e(40), v.e(1113)]).then((() => () => v(41113))))), i("@jupyterlab/json-extension", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(2471), v.e(7711), v.e(3880)]).then((() => () => v(63880))))), i("@jupyterlab/launcher-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(7504), v.e(4761), v.e(3042)]).then((() => () => v(79626))))), i("@jupyterlab/launcher", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(3231), v.e(9116), v.e(9053)]).then((() => () => v(79053))))), i("@jupyterlab/logconsole-extension", "3.5.3", (() => Promise.all([v.e(9266), v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(942), v.e(2471), v.e(5786), v.e(7504), v.e(40), v.e(3079), v.e(6725), v.e(2538)]).then((() => () => v(9266))))), i("@jupyterlab/logconsole", "3.5.3", (() => Promise.all([v.e(3122), v.e(6169), v.e(4265), v.e(4519), v.e(942), v.e(40), v.e(178)]).then((() => () => v(3122))))), i("@jupyterlab/mainmenu-extension", "3.5.3", (() => Promise.all([v.e(7463), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(9005), v.e(435)]).then((() => () => v(97463))))), i("@jupyterlab/mainmenu", "3.5.3", (() => Promise.all([v.e(6169), v.e(4519), v.e(3892), v.e(9674), v.e(5072)]).then((() => () => v(55072))))), i("@jupyterlab/markdownviewer-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5941), v.e(5786), v.e(7504), v.e(40), v.e(7737), v.e(3277)]).then((() => () => v(46985))))), i("@jupyterlab/markdownviewer", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(5941), v.e(40), v.e(985), v.e(2358)]).then((() => () => v(22358))))), i("@jupyterlab/mathjax2-extension", "3.5.3", (() => Promise.all([v.e(5941), v.e(40), v.e(8798), v.e(152)]).then((() => () => v(60152))))), i("@jupyterlab/mathjax2", "3.5.3", (() => Promise.all([v.e(6169), v.e(3469)]).then((() => () => v(13469))))), i("@jupyterlab/nbformat", "3.5.3", (() => Promise.all([v.e(6169), v.e(7526)]).then((() => () => v(97526))))), i("@jupyterlab/notebook-extension", "3.5.3", (() => Promise.all([v.e(4875), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(5786), v.e(7504), v.e(3231), v.e(40), v.e(9005), v.e(3079), v.e(6725), v.e(3050), v.e(2422), v.e(4064), v.e(435), v.e(4853), v.e(4920), v.e(4761), v.e(9590), v.e(4020), v.e(2538), v.e(2437)]).then((() => () => v(94206))))), i("@jupyterlab/notebook", "3.5.3", (() => Promise.all([v.e(2030), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(985), v.e(6725), v.e(4064), v.e(435), v.e(9116), v.e(3349), v.e(4853), v.e(2877), v.e(3383), v.e(9590), v.e(1563), v.e(6274), v.e(2930)]).then((() => () => v(92030))))), i("@jupyterlab/observables", "4.5.3", (() => Promise.all([v.e(97), v.e(6169), v.e(3892), v.e(942), v.e(3231), v.e(4064)]).then((() => () => v(60097))))), i("@jupyterlab/outputarea", "3.5.3", (() => Promise.all([v.e(3196), v.e(6169), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(40), v.e(435), v.e(9116), v.e(2877), v.e(2930)]).then((() => () => v(13196))))), i("@jupyterlab/pdf-extension", "3.5.3", (() => Promise.all([v.e(6169), v.e(4519), v.e(3231), v.e(490)]).then((() => () => v(80490))))), i("@jupyterlab/property-inspector", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(942), v.e(1295)]).then((() => () => v(21295))))), i("@jupyterlab/rendermime-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(40), v.e(2422), v.e(824)]).then((() => () => v(40824))))), i("@jupyterlab/rendermime-interfaces", "3.5.3", (() => v.e(4668).then((() => () => v(64668))))), i("@jupyterlab/rendermime", "3.5.3", (() => Promise.all([v.e(1520), v.e(1767), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2877), v.e(3059), v.e(2930), v.e(432)]).then((() => () => v(81767))))), i("@jupyterlab/running-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(985), v.e(2584), v.e(4466)]).then((() => () => v(51667))))), i("@jupyterlab/running", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(2471), v.e(3231), v.e(2319)]).then((() => () => v(22319))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([v.e(6591), v.e(6169), v.e(3892), v.e(942), v.e(5941), v.e(3231), v.e(1313), v.e(3050), v.e(8741)]).then((() => () => v(76591))))), i("@jupyterlab/settingeditor-extension", "3.5.3", (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(9674), v.e(5786), v.e(7504), v.e(40), v.e(3050), v.e(4853), v.e(2973)]).then((() => () => v(80989))))), i("@jupyterlab/settingeditor", "3.5.3", (() => Promise.all([v.e(4658), v.e(9865), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(2471), v.e(40), v.e(1313), v.e(3050), v.e(4853), v.e(1452), v.e(4665)]).then((() => () => v(19865))))), i("@jupyterlab/settingregistry", "3.5.3", (() => Promise.all([v.e(4658), v.e(7537), v.e(8270), v.e(6169), v.e(942), v.e(3231), v.e(2867)]).then((() => () => v(98270))))), i("@jupyterlab/shared-models", "3.5.3", (() => Promise.all([v.e(6879), v.e(528), v.e(6993), v.e(6169), v.e(942), v.e(9915)]).then((() => () => v(56993))))), i("@jupyterlab/shortcuts-extension", "3.5.3", (() => Promise.all([v.e(2212), v.e(6169), v.e(4265), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(5786), v.e(3231), v.e(3349), v.e(2867), v.e(6831), v.e(8300)]).then((() => () => v(52212))))), i("@jupyterlab/statedb", "3.5.3", (() => Promise.all([v.e(1325), v.e(6169), v.e(942), v.e(9116)]).then((() => () => v(91325))))), i("@jupyterlab/statusbar-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9674), v.e(5786), v.e(7504), v.e(3079), v.e(6725), v.e(9041), v.e(2867), v.e(6624), v.e(1806)]).then((() => () => v(54715))))), i("@jupyterlab/statusbar", "3.5.3", (() => Promise.all([v.e(2161), v.e(5573), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(3231)]).then((() => () => v(65573))))), i("@jupyterlab/theme-dark-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(9307)]).then((() => () => v(59307))))), i("@jupyterlab/theme-light-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(7746)]).then((() => () => v(37746))))), i("@jupyterlab/toc-extension", "5.5.3", (() => Promise.all([v.e(4265), v.e(9674), v.e(5786), v.e(7504), v.e(40), v.e(3079), v.e(2422), v.e(6624), v.e(9590), v.e(7737), v.e(1091), v.e(2788)]).then((() => () => v(80833))))), i("@jupyterlab/toc", "5.5.3", (() => Promise.all([v.e(8828), v.e(6169), v.e(4265), v.e(4519), v.e(9674), v.e(942), v.e(5941), v.e(2471), v.e(3079), v.e(3349), v.e(9590), v.e(7711)]).then((() => () => v(6598))))), i("@jupyterlab/tooltip-extension", "3.5.3", (() => Promise.all([v.e(4519), v.e(3892), v.e(5941), v.e(40), v.e(3079), v.e(9041), v.e(6624), v.e(7908), v.e(8232)]).then((() => () => v(28232))))), i("@jupyterlab/tooltip", "3.5.3", (() => Promise.all([v.e(6169), v.e(2814), v.e(4519), v.e(40), v.e(1507)]).then((() => () => v(11507))))), i("@jupyterlab/translation-extension", "3.5.3", (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(7504), v.e(9005), v.e(1440)]).then((() => () => v(61440))))), i("@jupyterlab/translation", "3.5.3", (() => Promise.all([v.e(2047), v.e(6169), v.e(5941), v.e(3050), v.e(435)]).then((() => () => v(52047))))), i("@jupyterlab/ui-components-extension", "3.5.3", (() => Promise.all([v.e(9674), v.e(9733)]).then((() => () => v(69733))))), i("@jupyterlab/ui-components", "3.5.3", (() => Promise.all([v.e(2161), v.e(3976), v.e(6169), v.e(4265), v.e(4519), v.e(3892), v.e(942), v.e(5941), v.e(2471), v.e(3231), v.e(3383), v.e(7711)]).then((() => () => v(33976))))), i("@jupyterlab/vega5-extension", "3.5.3", (() => Promise.all([v.e(4519), v.e(9712)]).then((() => () => v(79712))))), i("@jupyterlite/application-extension", "0.1.1", (() => Promise.all([v.e(6571), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5941), v.e(2471), v.e(7504), v.e(9005), v.e(2422), v.e(4920), v.e(8318), v.e(3288), v.e(2557)]).then((() => () => v(2557))))), i("@jupyterlite/application", "0.1.1", (() => Promise.all([v.e(812), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(3231), v.e(40), v.e(985), v.e(9116), v.e(4905)]).then((() => () => v(54905))))), i("@jupyterlite/contents", "0.1.1", (() => Promise.all([v.e(9737), v.e(6169), v.e(5941), v.e(302)]).then((() => () => v(40302))))), i("@jupyterlite/iframe-extension", "0.1.1", (() => Promise.all([v.e(6169), v.e(4519), v.e(6141)]).then((() => () => v(86141))))), i("@jupyterlite/kernel", "0.1.1", (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(5941), v.e(435), v.e(2877), v.e(2546)]).then((() => () => v(52546))))), i("@jupyterlite/licenses", "0.1.1", (() => Promise.all([v.e(6169), v.e(5941), v.e(9777)]).then((() => () => v(89777))))), i("@jupyterlite/localforage", "0.1.1", (() => Promise.all([v.e(6169), v.e(2329)]).then((() => () => v(2329))))), i("@jupyterlite/repl-extension", "0.1.1", (() => Promise.all([v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(7504), v.e(9041), v.e(8318), v.e(5225), v.e(8370)]).then((() => () => v(8370))))), i("@jupyterlite/retro-application-extension", "0.1.1", (() => Promise.all([v.e(4519), v.e(5941), v.e(2422), v.e(9041), v.e(8318), v.e(5191), v.e(3444)]).then((() => () => v(63444))))), i("@jupyterlite/server-extension", "0.1.1", (() => Promise.all([v.e(9440), v.e(5941), v.e(1354), v.e(8504), v.e(4931)]).then((() => () => v(24931))))), i("@jupyterlite/server", "0.1.1", (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(5941), v.e(435), v.e(6070), v.e(1245)]).then((() => () => v(71245))))), i("@jupyterlite/session", "0.1.1", (() => Promise.all([v.e(6169), v.e(3892), v.e(5941), v.e(4298)]).then((() => () => v(14298))))), i("@jupyterlite/settings", "0.1.1", (() => Promise.all([v.e(7537), v.e(6169), v.e(5941), v.e(3151)]).then((() => () => v(53151))))), i("@jupyterlite/translation", "0.1.1", (() => Promise.all([v.e(6169), v.e(5941), v.e(816)]).then((() => () => v(90816))))), i("@jupyterlite/ui-components", "0.1.1", (() => Promise.all([v.e(9674), v.e(9958)]).then((() => () => v(59958))))), i("@lumino/algorithm", "1.9.2", (() => v.e(9943).then((() => () => v(99943))))), i("@lumino/application", "1.31.3", (() => Promise.all([v.e(1278), v.e(6169), v.e(4519), v.e(2867)]).then((() => () => v(61278))))), i("@lumino/commands", "1.21.1", (() => Promise.all([v.e(8061), v.e(6169), v.e(3892), v.e(942), v.e(3231), v.e(3349), v.e(6831)]).then((() => () => v(38061))))), i("@lumino/coreutils", "1.12.1", (() => v.e(8883).then((() => () => v(28883))))), i("@lumino/datagrid", "0.36.6", (() => Promise.all([v.e(920), v.e(6169), v.e(4519), v.e(3892), v.e(942), v.e(4064), v.e(3349), v.e(1563), v.e(6831)]).then((() => () => v(30920))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([v.e(3892), v.e(942), v.e(5851)]).then((() => () => v(35851))))), i("@lumino/domutils", "1.8.2", (() => v.e(1310).then((() => () => v(71310))))), i("@lumino/dragdrop", "1.14.4", (() => Promise.all([v.e(1084), v.e(3231)]).then((() => () => v(51084))))), i("@lumino/keyboard", "1.8.2", (() => v.e(8990).then((() => () => v(58990))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([v.e(3850), v.e(3892)]).then((() => () => v(23850))))), i("@lumino/polling", "1.11.3", (() => Promise.all([v.e(8594), v.e(6169), v.e(942)]).then((() => () => v(36107))))), i("@lumino/properties", "1.8.2", (() => v.e(1555).then((() => () => v(21555))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([v.e(3892), v.e(9116), v.e(8389)]).then((() => () => v(38389))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([v.e(5437), v.e(3892)]).then((() => () => v(75437))))), i("@lumino/widgets", "1.37.1", (() => Promise.all([v.e(5666), v.e(6169), v.e(3892), v.e(942), v.e(3231), v.e(4064), v.e(9116), v.e(3349), v.e(2867), v.e(3383), v.e(1563), v.e(6831)]).then((() => () => v(75666))))), i("@retrolab/application-extension", "0.3.21", (() => Promise.all([v.e(1559), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(5941), v.e(5786), v.e(7504), v.e(3231), v.e(985), v.e(9005), v.e(2422), v.e(9041), v.e(5191), v.e(4769)]).then((() => () => v(91559))))), i("@retrolab/application", "0.3.21", (() => Promise.all([v.e(812), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(3231), v.e(40), v.e(985), v.e(1313), v.e(4064), v.e(9116), v.e(6556)]).then((() => () => v(36556))))), i("@retrolab/help-extension", "0.3.21", (() => Promise.all([v.e(4265), v.e(2814), v.e(2471), v.e(9005), v.e(4769), v.e(8785)]).then((() => () => v(18785))))), i("@retrolab/notebook-extension", "0.3.21", (() => Promise.all([v.e(4265), v.e(2814), v.e(4519), v.e(5941), v.e(5786), v.e(9005), v.e(1313), v.e(3079), v.e(2422), v.e(5191), v.e(2099)]).then((() => () => v(2099))))), i("@retrolab/tree-extension", "0.3.21", (() => Promise.all([v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(4920), v.e(2584), v.e(9170)]).then((() => () => v(19170))))), i("@retrolab/ui-components", "0.3.21", (() => Promise.all([v.e(1644), v.e(9674)]).then((() => () => v(11644))))), i("codemirror", "5.61.1", (() => v.e(5747).then((() => () => v(25747))))), i("react-dom", "17.0.2", (() => Promise.all([v.e(2287), v.e(2471)]).then((() => () => v(42287))))), i("react-highlighter", "0.4.3", (() => Promise.all([v.e(7058), v.e(2471)]).then((() => () => v(87058))))), i("react-json-tree", "0.15.2", (() => Promise.all([v.e(4615), v.e(2471)]).then((() => () => v(34615))))), i("react", "17.0.2", (() => v.e(7427).then((() => () => v(47427))))), i("typestyle", "2.4.0", (() => v.e(1163).then((() => () => v(91163))))), i("vega-embed", "6.21.0", (() => Promise.all([v.e(44), v.e(1214), v.e(123)]).then((() => () => v(30044))))), i("vega-lite", "5.5.0", (() => Promise.all([v.e(61), v.e(1725), v.e(1214), v.e(8542)]).then((() => () => v(71725))))), i("vega", "5.23.0", (() => Promise.all([v.e(61), v.e(1603), v.e(4191)]).then((() => () => v(91603))))), i("yjs", "13.5.43", (() => Promise.all([v.e(6879), v.e(1221), v.e(4535)]).then((() => () => v(61221)))))), e[l] = s.length ? Promise.all(s).then((() => e[l] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         v.g.importScripts && (e = v.g.location + "");
         var t = v.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
@@ -561,35 +561,35 @@
         return n && n.then ? n.then(e.bind(e, t, v.S[t], l, a, r)) : e(t, v.S[t], l, a, r)
     })(((e, t, l, a, r) => t && v.o(t, l) ? d(t, 0, l, a) : r())), c = b(((e, t, l, a, r) => {
         var n = t && v.o(t, l) && m(t, l, a);
         return n ? f(n) : r()
     })), h = {}, P = {
         55941: () => p("default", "@jupyterlab/coreutils", [2, 5, 5, 3], (() => Promise.all([v.e(8101), v.e(6169), v.e(942), v.e(5126)]).then((() => () => v(54705))))),
         67504: () => p("default", "@jupyterlab/application", [2, 3, 5, 3], (() => Promise.all([v.e(812), v.e(9198), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(3231), v.e(40), v.e(985), v.e(1313), v.e(4064), v.e(435), v.e(9116), v.e(6070)]).then((() => () => v(79198))))),
-        66737: () => c("default", "@jupyterlite/server", [2, 0, 1, 0], (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(435), v.e(6070), v.e(4410)]).then((() => () => v(71245))))),
+        71354: () => c("default", "@jupyterlite/server", [2, 0, 1, 1], (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(435), v.e(6070), v.e(4410)]).then((() => () => v(71245))))),
         22437: () => c("default", "@jupyterlab/docmanager-extension", [2, 3, 5, 3], (() => Promise.all([v.e(3392), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(5786), v.e(7504), v.e(6725), v.e(2422), v.e(3288)]).then((() => () => v(90509))))),
         10310: () => c("default", "@jupyterlab/apputils-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4856), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5786), v.e(7504), v.e(3231), v.e(985), v.e(9005), v.e(1313), v.e(3050), v.e(2867), v.e(4920)]).then((() => () => v(74856))))),
         15802: () => c("default", "@jupyterlab/codemirror-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(5786), v.e(7504), v.e(9005), v.e(6725), v.e(4853), v.e(6624), v.e(3059), v.e(1981), v.e(6493)]).then((() => () => v(66493))))),
         29507: () => c("default", "@jupyterlab/application-extension", [2, 3, 5, 3], (() => Promise.all([v.e(316), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(5786), v.e(7504), v.e(3231), v.e(3050), v.e(4020)]).then((() => () => v(30316))))),
+        34019: () => c("default", "@jupyterlite/application-extension", [2, 0, 1, 1], (() => Promise.all([v.e(6571), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(7504), v.e(9005), v.e(2422), v.e(4920), v.e(8318), v.e(3288), v.e(9960)]).then((() => () => v(2557))))),
         46813: () => c("default", "@jupyterlab/mainmenu-extension", [2, 3, 5, 3], (() => Promise.all([v.e(7463), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5786), v.e(7504), v.e(9005), v.e(435)]).then((() => () => v(97463))))),
         53516: () => c("default", "@jupyterlab/mathjax2-extension", [2, 3, 5, 3], (() => Promise.all([v.e(40), v.e(8798), v.e(9622)]).then((() => () => v(60152))))),
         64948: () => c("default", "@jupyterlab/filebrowser-extension", [2, 3, 5, 3], (() => Promise.all([v.e(9806), v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(5786), v.e(7504), v.e(6725), v.e(3050), v.e(2422), v.e(2867), v.e(4920)]).then((() => () => v(59806))))),
         65540: () => c("default", "@jupyterlab/completer-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4519), v.e(3892), v.e(3079), v.e(9041), v.e(6624), v.e(240)]).then((() => () => v(10240))))),
         66325: () => c("default", "@jupyterlab/tooltip-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4519), v.e(3892), v.e(40), v.e(3079), v.e(9041), v.e(6624), v.e(7908), v.e(213)]).then((() => () => v(28232))))),
         73624: () => c("default", "@jupyterlab/translation-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(7504), v.e(9005), v.e(1440)]).then((() => () => v(61440))))),
         78036: () => c("default", "@jupyterlab/theme-light-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(2814), v.e(7746)]).then((() => () => v(37746))))),
         78042: () => c("default", "@jupyterlab/console-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4117), v.e(6169), v.e(4265), v.e(2814), v.e(3892), v.e(9674), v.e(5786), v.e(7504), v.e(3231), v.e(40), v.e(9005), v.e(9041), v.e(9116), v.e(4853), v.e(4920), v.e(4761)]).then((() => () => v(14117))))),
         85687: () => c("default", "@jupyterlab/theme-dark-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(2814), v.e(9307)]).then((() => () => v(59307))))),
         89985: () => c("default", "@jupyterlab/shortcuts-extension", [2, 3, 5, 3], (() => Promise.all([v.e(2212), v.e(6169), v.e(4265), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(5786), v.e(3231), v.e(3349), v.e(2867), v.e(6831), v.e(8300)]).then((() => () => v(52212))))),
-        95863: () => c("default", "@jupyterlite/application-extension", [2, 0, 1, 0], (() => Promise.all([v.e(6571), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(2471), v.e(7504), v.e(9005), v.e(2422), v.e(4920), v.e(6243), v.e(3288), v.e(9960)]).then((() => () => v(2557))))),
         99256: () => c("default", "@jupyterlab/rendermime-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(2814), v.e(40), v.e(2422), v.e(824)]).then((() => () => v(40824))))),
         48218: () => c("default", "@jupyterlab/cell-toolbar-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(5155)]).then((() => () => v(15155))))),
         19656: () => c("default", "@jupyterlab/fileeditor-extension", [2, 3, 5, 3], (() => Promise.all([v.e(6136), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(5786), v.e(7504), v.e(9005), v.e(6725), v.e(9041), v.e(4853), v.e(6624), v.e(4920), v.e(4761)]).then((() => () => v(46136))))),
         62570: () => c("default", "@jupyterlab/notebook-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4875), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(5786), v.e(7504), v.e(3231), v.e(40), v.e(9005), v.e(3079), v.e(6725), v.e(3050), v.e(2422), v.e(4064), v.e(435), v.e(4853), v.e(4920), v.e(4761), v.e(9590), v.e(4020), v.e(2538)]).then((() => () => v(94206))))),
-        41754: () => c("default", "@jupyterlite/iframe-extension", [2, 0, 1, 0], (() => Promise.all([v.e(6169), v.e(4519), v.e(6141)]).then((() => () => v(86141))))),
+        19611: () => c("default", "@jupyterlite/iframe-extension", [2, 0, 1, 1], (() => Promise.all([v.e(6169), v.e(4519), v.e(6141)]).then((() => () => v(86141))))),
         30126: () => c("default", "@jupyterlab/vega5-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4519), v.e(9712)]).then((() => () => v(79712))))),
         29265: () => c("default", "@jupyterlab/json-extension", [2, 3, 5, 3], (() => Promise.all([v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(2471), v.e(7711), v.e(3880)]).then((() => () => v(63880))))),
         23946: () => c("default", "@jupyterlab/javascript-extension", [2, 3, 5, 3], (() => Promise.all([v.e(40), v.e(1113)]).then((() => () => v(41113))))),
         6381: () => c("default", "@jupyterlab/running-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(3892), v.e(9674), v.e(942), v.e(985), v.e(2584), v.e(1667)]).then((() => () => v(51667))))),
         7087: () => c("default", "@jupyterlab/ui-components-extension", [2, 3, 5, 3], (() => Promise.all([v.e(9674), v.e(9733)]).then((() => () => v(69733))))),
         8075: () => c("default", "@jupyterlab/documentsearch-extension", [2, 3, 5, 3], (() => Promise.all([v.e(4265), v.e(2814), v.e(5786), v.e(192), v.e(9035)]).then((() => () => v(59035))))),
         10846: () => c("default", "@jupyterlab/help-extension", [2, 3, 5, 3], (() => Promise.all([v.e(3979), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(9674), v.e(942), v.e(2471), v.e(9005), v.e(435), v.e(3383)]).then((() => () => v(93979))))),
@@ -664,111 +664,111 @@
         72930: () => c("default", "@jupyterlab/nbformat", [1, 3, 5, 3], (() => v.e(6080).then((() => () => v(97526))))),
         70432: () => p("default", "@jupyterlab/rendermime-interfaces", [2, 3, 5, 3], (() => v.e(4668).then((() => () => v(64668))))),
         2584: () => c("default", "@jupyterlab/running", [1, 3, 5, 3], (() => Promise.all([v.e(6169), v.e(2814), v.e(2471), v.e(3231), v.e(6748)]).then((() => () => v(22319))))),
         46831: () => c("default", "@lumino/keyboard", [1, 1, 8, 1], (() => v.e(8990).then((() => () => v(58990))))),
         18300: () => c("default", "typestyle", [1, 2, 0, 4], (() => v.e(1163).then((() => () => v(91163))))),
         1091: () => c("default", "@jupyterlab/toc", [1, 5, 5, 3], (() => Promise.all([v.e(8828), v.e(6169), v.e(4519), v.e(942), v.e(5941), v.e(2471), v.e(3349), v.e(7711)]).then((() => () => v(6598))))),
         27908: () => p("default", "@jupyterlab/tooltip", [2, 3, 5, 3], (() => Promise.all([v.e(6169), v.e(2814), v.e(509)]).then((() => () => v(11507))))),
-        26243: () => c("default", "@jupyterlite/ui-components", [2, 0, 1, 0], (() => Promise.all([v.e(9674), v.e(9958)]).then((() => () => v(59958))))),
-        84997: () => c("default", "@jupyterlite/application", [2, 0, 1, 0], (() => Promise.all([v.e(812), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(3231), v.e(40), v.e(985), v.e(9116), v.e(4905)]).then((() => () => v(54905))))),
+        58318: () => c("default", "@jupyterlite/ui-components", [2, 0, 1, 1], (() => Promise.all([v.e(9674), v.e(9958)]).then((() => () => v(59958))))),
+        75225: () => c("default", "@jupyterlite/application", [2, 0, 1, 1], (() => Promise.all([v.e(812), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(5941), v.e(7504), v.e(3231), v.e(40), v.e(985), v.e(9116), v.e(4905)]).then((() => () => v(54905))))),
         95191: () => c("default", "@retrolab/application", [2, 0, 3, 21], (() => Promise.all([v.e(812), v.e(6169), v.e(4265), v.e(2814), v.e(4519), v.e(3892), v.e(9674), v.e(942), v.e(7504), v.e(3231), v.e(40), v.e(985), v.e(1313), v.e(4064), v.e(9116), v.e(783)]).then((() => () => v(36556))))),
-        1258: () => c("default", "@jupyterlite/translation", [2, 0, 1, 0], (() => Promise.all([v.e(6169), v.e(7041)]).then((() => () => v(90816))))),
-        29790: () => p("default", "@jupyterlite/contents", [2, 0, 1, 0], (() => Promise.all([v.e(9737), v.e(6169), v.e(302)]).then((() => () => v(40302))))),
-        35151: () => p("default", "@jupyterlite/licenses", [2, 0, 1, 0], (() => Promise.all([v.e(6169), v.e(9502)]).then((() => () => v(89777))))),
-        40371: () => c("default", "@jupyterlite/session", [2, 0, 1, 0], (() => Promise.all([v.e(6169), v.e(3892), v.e(2887)]).then((() => () => v(14298))))),
-        73968: () => c("default", "@jupyterlite/settings", [2, 0, 1, 0], (() => Promise.all([v.e(7537), v.e(6169), v.e(555)]).then((() => () => v(53151))))),
-        79850: () => p("default", "@jupyterlite/kernel", [2, 0, 1, 0], (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(435), v.e(2877), v.e(2546)]).then((() => () => v(52546))))),
-        88052: () => p("default", "@jupyterlite/localforage", [2, 0, 1, 0], (() => Promise.all([v.e(6169), v.e(2329)]).then((() => () => v(2329))))),
+        25262: () => c("default", "@jupyterlite/session", [2, 0, 1, 1], (() => Promise.all([v.e(6169), v.e(3892), v.e(2887)]).then((() => () => v(14298))))),
+        48531: () => c("default", "@jupyterlite/translation", [2, 0, 1, 1], (() => Promise.all([v.e(6169), v.e(7041)]).then((() => () => v(90816))))),
+        51154: () => p("default", "@jupyterlite/kernel", [2, 0, 1, 1], (() => Promise.all([v.e(1079), v.e(6169), v.e(942), v.e(435), v.e(2877), v.e(2546)]).then((() => () => v(52546))))),
+        64822: () => p("default", "@jupyterlite/licenses", [2, 0, 1, 1], (() => Promise.all([v.e(6169), v.e(9502)]).then((() => () => v(89777))))),
+        70007: () => p("default", "@jupyterlite/localforage", [2, 0, 1, 1], (() => Promise.all([v.e(6169), v.e(2329)]).then((() => () => v(2329))))),
+        84021: () => p("default", "@jupyterlite/contents", [2, 0, 1, 1], (() => Promise.all([v.e(9737), v.e(6169), v.e(302)]).then((() => () => v(40302))))),
+        94523: () => c("default", "@jupyterlite/settings", [2, 0, 1, 1], (() => Promise.all([v.e(7537), v.e(6169), v.e(555)]).then((() => () => v(53151))))),
         24769: () => c("default", "@retrolab/ui-components", [2, 0, 3, 21], (() => Promise.all([v.e(1644), v.e(9674)]).then((() => () => v(11644))))),
         11214: () => c("default", "vega", [1, 5, 20, 0], (() => Promise.all([v.e(61), v.e(1603)]).then((() => () => v(91603))))),
         40123: () => c("default", "vega-lite", [1, 5, 1, 0], (() => Promise.all([v.e(61), v.e(1725)]).then((() => () => v(71725))))),
-        55367: () => c("default", "@jupyterlite/server-extension", [2, 0, 1, 0], (() => Promise.all([v.e(9440), v.e(1066), v.e(8732)]).then((() => () => v(24931))))),
+        43124: () => c("default", "@jupyterlite/server-extension", [2, 0, 1, 1], (() => Promise.all([v.e(9440), v.e(8504), v.e(8732)]).then((() => () => v(24931))))),
         24957: () => p("default", "@jupyterlab/settingeditor", [2, 3, 5, 3], (() => Promise.all([v.e(4658), v.e(9865), v.e(4519), v.e(3892), v.e(942), v.e(2471), v.e(1313), v.e(1452)]).then((() => () => v(19865))))),
         59957: () => c("default", "vega-embed", [1, 6, 2, 1], (() => Promise.all([v.e(44), v.e(1214), v.e(123)]).then((() => () => v(30044)))))
     }, y = {
         40: [20040],
         123: [40123],
         126: [30126],
         178: [80178],
         192: [60192],
         240: [27705],
         432: [70432],
         435: [20435],
         901: [90901],
         942: [70942],
         985: [985],
-        1066: [1258, 29790, 35151, 40371, 73968, 79850, 88052],
         1091: [1091],
         1214: [11214],
         1313: [61313],
+        1354: [71354],
         1408: [6381, 7087, 8075, 10846, 10992, 29084, 33894, 44109, 51267, 57509, 64411, 64500, 73668, 81237, 88370, 94979],
         1452: [91452],
         1563: [81563],
-        1754: [41754],
         1981: [41981],
         2422: [42422],
         2437: [22437],
         2471: [62471],
         2538: [52538],
         2584: [2584],
         2813: [48218, 19656, 62570],
         2814: [2814],
         2867: [72867],
         2877: [92877],
         2930: [72930],
         3050: [63050],
         3059: [23059],
         3079: [33079],
+        3124: [43124],
         3231: [43231],
         3288: [83288],
         3349: [33349],
         3383: [93383],
         3880: [45388, 65485],
         3892: [43892],
         3946: [23946],
         4020: [4020],
         4064: [14064],
         4265: [4265],
         4519: [94519],
         4761: [44761],
         4769: [24769],
+        4810: [10310, 15802, 29507, 34019, 46813, 53516, 64948, 65540, 66325, 73624, 78036, 78042, 85687, 89985, 99256],
         4853: [84853],
         4920: [84920],
         4957: [24957],
-        4997: [84997],
         5155: [718],
         5191: [95191],
-        5367: [55367],
+        5225: [75225],
         5786: [15786],
         5941: [55941],
         6070: [76070],
         6169: [26169],
-        6243: [26243],
         6274: [56274],
         6464: [26464],
         6531: [56531],
         6624: [6624],
         6725: [16725],
-        6737: [66737],
         6831: [46831],
         7504: [67504],
         7543: [17543],
         7711: [37711],
         7737: [47737],
         7908: [27908],
         8033: [58033],
         8300: [18300],
-        8402: [10310, 15802, 29507, 46813, 53516, 64948, 65540, 66325, 73624, 78036, 78042, 85687, 89985, 95863, 99256],
+        8318: [58318],
+        8504: [25262, 48531, 51154, 64822, 70007, 84021, 94523],
         8798: [38798],
         8981: [32033],
         9005: [49005],
         9041: [69041],
         9116: [89116],
         9265: [29265],
         9590: [69590],
+        9611: [19611],
         9674: [59674],
         9915: [79915],
         9957: [59957]
     }, v.f.consumes = (e, t) => {
         v.o(y, e) && y[e].forEach((e => {
             if (v.o(h, e)) return t.push(h[e]);
             var l = t => {
@@ -793,15 +793,15 @@
         var e = {
             4109: 0
         };
         v.f.j = (t, l) => {
             var a = v.o(e, t) ? e[t] : void 0;
             if (0 !== a)
                 if (a) l.push(a[2]);
-                else if (/^(1(2(14|3|6)|066|091|313|452|563|754|78|92|981)|2(4(22|37|71)|8(13|14|67|77)|538|584|930)|3(0(50|59|79)|231|288|349|383|892|946)|4(0(|20|64)|76[19]|9(20|57|97)|265|32|35|519|853)|5(191|367|786|941)|6((27|46|62)4|[58]31|070|169|243|725|737)|7(504|543|711|737|908)|8(033|300|402|798)|9(0(05|1|41)|(26|8|91)5|116|42|590|674|957))$/.test(t)) e[t] = 0;
+                else if (/^(1(2(14|3|6)|091|313|354|452|563|78|92|981)|2(4(22|37|71)|8(13|14|67|77)|538|584|930)|3(0(50|59|79)|124|231|288|349|383|892|946)|4(0(|20|64)|76[19]|265|32|35|519|810|853|920|957)|5(191|225|786|941)|6((27|46|62)4|[58]31|070|169|725)|7(504|543|711|737|908)|8(033|300|318|504|798)|9(0(05|1|41)|(26|8|91)5|116|42|590|611|674|957))$/.test(t)) e[t] = 0;
             else {
                 var r = new Promise(((l, r) => a = e[t] = [l, r]));
                 l.push(a[2] = r);
                 var n = v.p + v.u(t),
                     o = new Error;
                 v.l(n, (l => {
                     if (v.o(e, t) && (0 !== (a = e[t]) && (e[t] = void 0), a)) {
@@ -823,8 +823,8 @@
             },
             l = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || [];
         l.forEach(t.bind(null, 0)), l.push = t.bind(null, l.push.bind(l))
     })(), v.nc = void 0;
     var x = v(304);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).CORE_OUTPUT = x
 })();
-//# sourceMappingURL=bundle.js.map?_=4a04b99
+//# sourceMappingURL=bundle.js.map?_=e57205c
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/listings-info.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/listings-info.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/move-down.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/move-down.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/move-up.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/move-up.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/not-trusted.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/not-trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/palette.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/palette.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/pdf.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/pdf.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/python.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/react.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/react.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/regex.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/regex.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/schemas/all.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/service-worker-b2fb40a.js` & `resotocore-3.6.5/resotocore/jupyterlite/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/settings.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/settings.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/tag.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/tag.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/terminal.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/terminal.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `resotocore-3.6.5/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/third-party-licenses.json` & `resotocore-3.6.5/resotocore/jupyterlite/build/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961734693877551%*

 * *Differences: {"'packages'": "{89: {'versionInfo': '0.1.1'}, 90: {'versionInfo': '0.1.1'}, 91: {'versionInfo': "*

 * *               "'0.1.1'}, 92: {'versionInfo': '0.1.1'}, 93: {'versionInfo': '0.1.1'}, 94: "*

 * *               "{'versionInfo': '0.1.1'}, 95: {'versionInfo': '0.1.1'}, 96: {'versionInfo': "*

 * *               "'0.1.1'}, 97: {'versionInfo': '0.1.1'}, 98: {'versionInfo': '0.1.1'}, 99: "*

 * *               "{'versionInfo': '0.1.1'}, 100: {'versionInfo': '0.1.1'}, 101: {'versionInfo': "*

 * *               "'0.1.1'}, 102: {'versio […]*

```diff
@@ -534,117 +534,117 @@
             "name": "@jupyterlab/vega5-extension",
             "versionInfo": "3.5.3"
         },
         {
             "extractedText": "",
             "licenseId": "",
             "name": "@jupyterlite/app-lab",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "",
             "name": "@jupyterlite/app-repl",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "",
             "name": "@jupyterlite/app-retro",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/application",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/application-extension",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/contents",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/iframe-extension",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/kernel",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/licenses",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/localforage",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/repl-extension",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/retro-application-extension",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/server",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/server-extension",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/session",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/settings",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/translation",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/ui-components",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@lumino/algorithm",
             "versionInfo": "1.9.2"
         },
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/toc.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/toc.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/build/trusted.svg` & `resotocore-3.6.5/resotocore/jupyterlite/build/trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/config-utils.js` & `resotocore-3.6.5/resotocore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9606481481481483%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/javascript-kernel': '^0.1.1', '@jupyterlite/kernel': '^0.1.1', "*

 * *                   "'@jupyterlite/server': '^0.1.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9eaa8a846d81f5b6c8be.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterLite Contributors",
     "bugs": {
         "url": "https://github.com/jupyterlite/jupyterlite/issues"
     },
     "dependencies": {
         "@jupyterlab/coreutils": "~5.5.3",
-        "@jupyterlite/javascript-kernel": "^0.1.0",
-        "@jupyterlite/kernel": "^0.1.0",
-        "@jupyterlite/server": "^0.1.0"
+        "@jupyterlite/javascript-kernel": "^0.1.1",
+        "@jupyterlite/kernel": "^0.1.1",
+        "@jupyterlite/server": "^0.1.1"
     },
     "description": "JupyterLite - JavaScript Kernel Extension",
     "devDependencies": {
         "@babel/core": "^7.11.6",
         "@babel/preset-env": "^7.12.1",
         "@jupyterlab/builder": "^3.1.0",
         "@types/jest": "^26.0.10",
@@ -28,15 +28,15 @@
         "lib/*.js.map",
         "lib/*.js"
     ],
     "homepage": "https://github.com/jupyterlite/jupyterlite",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7e46d8af7cfb9637087e.js"
+            "load": "static/remoteEntry.9eaa8a846d81f5b6c8be.js"
         },
         "extension": true,
         "outputDir": "jupyterlite_javascript_kernel/labextension"
     },
     "jupyterlite": {
         "liteExtension": true
     },
@@ -70,9 +70,9 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "yarn prettier:base --check",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.29fb1677e9ddfbef42ef.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
     [290, 322], {
         290: (e, t, r) => {
             r.r(t), r.d(t, {
                 JavaScriptKernel: () => E
             });
             var n = r(671),
-                a = r(430),
+                a = r(826),
                 s = r(526);
             const o = Symbol("Comlink.proxy"),
                 i = Symbol("Comlink.endpoint"),
                 c = Symbol("Comlink.releaseProxy"),
                 u = Symbol("Comlink.thrown"),
                 l = e => "object" == typeof e && null !== e || "function" == typeof e,
                 p = new Map([
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.5488d7441d23f13faba2.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
     [322, 290], {
         290: (e, t, r) => {
             r.r(t), r.d(t, {
                 JavaScriptKernel: () => E
             });
             var n = r(671),
-                a = r(430),
+                a = r(826),
                 s = r(526);
             const o = Symbol("Comlink.proxy"),
                 i = Symbol("Comlink.endpoint"),
                 c = Symbol("Comlink.releaseProxy"),
                 u = Symbol("Comlink.thrown"),
                 l = e => "object" == typeof e && null !== e || "function" == typeof e,
                 p = new Map([
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.b0a688b88d43b80c014d.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,16 @@
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
     [568], {
         568: (e, a, r) => {
             r.r(a), r.d(a, {
                 default: () => i
             });
             var t = r(671),
-                s = r(430),
-                n = r(199);
+                s = r(826),
+                n = r(765);
             const i = [{
                 id: "@jupyterlite/javascript-kernel-extension:kernel",
                 autoStart: !0,
                 requires: [s.IKernelSpecs],
                 activate: (e, a) => {
                     const r = t.PageConfig.getBaseUrl();
                     a.register({
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.9eaa8a846d81f5b6c8be.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, s, d, f, c, p, h, v, b, m, y, g, j, w, k = {
+    var e, r, t, n, a, o, i, l, u, s, f, d, c, p, h, v, b, m, y, g, j, w, k = {
             986: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(671), t.e(430), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(671), t.e(430), t.e(568)]).then((() => () => t(568)))
+                        "./index": () => Promise.all([t.e(671), t.e(826), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(671), t.e(826), t.e(568)]).then((() => () => t(568)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -42,62 +42,62 @@
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         102: "c877ef340ee478be48c0",
-        290: "85fbfc269929f73a8f25",
-        322: "47953449e4616f51d135",
-        430: "4ad5780ad91bfc65edda",
+        290: "29fb1677e9ddfbef42ef",
+        322: "5488d7441d23f13faba2",
         441: "4368412449ba90ea9225",
         526: "d5312df4c55fd57dbce5",
-        568: "34b49b2d3ba8db46b0cc",
+        568: "b0a688b88d43b80c014d",
         671: "11d0402aaed2182a5985",
+        826: "e39ede89416bd1f1fe66",
         866: "1ce3c77b50c9eb671961"
     } [e] + ".js?v=" + {
         102: "c877ef340ee478be48c0",
-        290: "85fbfc269929f73a8f25",
-        322: "47953449e4616f51d135",
-        430: "4ad5780ad91bfc65edda",
+        290: "29fb1677e9ddfbef42ef",
+        322: "5488d7441d23f13faba2",
         441: "4368412449ba90ea9225",
         526: "d5312df4c55fd57dbce5",
-        568: "34b49b2d3ba8db46b0cc",
+        568: "b0a688b88d43b80c014d",
         671: "11d0402aaed2182a5985",
+        826: "e39ede89416bd1f1fe66",
         866: "1ce3c77b50c9eb671961"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlite/javascript-kernel-extension:", S.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== a)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var d = u[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                    var f = u[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -119,15 +119,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlite/javascript-kernel-extension", "0.1.0", (() => Promise.all([S.e(671), S.e(430), S.e(568)]).then((() => () => S(568))))), l("@jupyterlite/javascript-kernel", "0.1.0", (() => Promise.all([S.e(526), S.e(671), S.e(430), S.e(290)]).then((() => () => S(290))))), l("@jupyterlite/kernel", "0.1.0", (() => Promise.all([S.e(441), S.e(526), S.e(671), S.e(102)]).then((() => () => S(102)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlite/javascript-kernel-extension", "0.1.1", (() => Promise.all([S.e(671), S.e(826), S.e(568)]).then((() => () => S(568))))), l("@jupyterlite/javascript-kernel", "0.1.1", (() => Promise.all([S.e(526), S.e(671), S.e(826), S.e(290)]).then((() => () => S(290))))), l("@jupyterlite/kernel", "0.1.1", (() => Promise.all([S.e(441), S.e(526), S.e(671), S.e(102)]).then((() => () => S(102)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -176,33 +176,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, d, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > n && !a : "" == f != a);
-                if ("u" == d) {
-                    if (!u || "u" != f) return !1
+                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
+                if ("u" == f) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (f == d)
+                    if (d == f)
                         if (l <= n) {
                             if (s != e[l]) return !1
                         } else {
                             if (a ? s > e[l] : s < e[l]) return !1;
                             s != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || d < f != a) return !1;
+                    if (l <= n || f < d != a) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -214,45 +214,45 @@
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
         var a = u(e, t);
         return o(n, a) || "undefined" != typeof console && console.warn && console.warn(s(e, t, a, n)), h(e[t][a])
-    }, f = (e, r, t) => {
+    }, d = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, c = (e, r, t, n) => {
         var o = e[t];
         return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, p = (e, r, t, n) => {
         "undefined" != typeof console && console.warn && console.warn(c(e, r, t, n))
     }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, n, a) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, a)) : e(r, S.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), h(f(r, t, n) || p(r, e, t, n) || l(r, t))))), m = v(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), y = v(((e, r, t, n, a) => {
-        var o = r && S.o(r, t) && f(r, t, n);
+    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || l(r, t))))), m = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), y = v(((e, r, t, n, a) => {
+        var o = r && S.o(r, t) && d(r, t, n);
         return o ? h(o) : a()
     })), g = {}, j = {
         671: () => m("default", "@jupyterlab/coreutils", [1, 5, 5, 3]),
-        430: () => y("default", "@jupyterlite/kernel", [2, 0, 1, 0], (() => Promise.all([S.e(441), S.e(526), S.e(102)]).then((() => () => S(102))))),
-        199: () => y("default", "@jupyterlite/javascript-kernel", [2, 0, 1, 0], (() => Promise.all([S.e(526), S.e(322)]).then((() => () => S(290))))),
+        826: () => y("default", "@jupyterlite/kernel", [2, 0, 1, 1], (() => Promise.all([S.e(441), S.e(526), S.e(102)]).then((() => () => S(102))))),
+        765: () => y("default", "@jupyterlite/javascript-kernel", [2, 0, 1, 1], (() => Promise.all([S.e(526), S.e(322)]).then((() => () => S(290))))),
         526: () => m("default", "@lumino/coreutils", [1, 1, 11, 0]),
         840: () => m("default", "@lumino/signaling", [1, 1, 10, 0]),
         878: () => m("default", "@jupyterlab/services", [1, 6, 5, 3]),
         911: () => b("default", "@jupyterlab/observables", [1, 4, 5, 3])
     }, w = {
         102: [840, 878, 911],
-        430: [430],
         526: [526],
-        568: [199],
-        671: [671]
+        568: [765],
+        671: [671],
+        826: [826]
     }, S.f.consumes = (e, r) => {
         S.o(w, e) && w[e].forEach((e => {
             if (S.o(g, e)) return r.push(g[e]);
             var t = r => {
                     g[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -274,15 +274,15 @@
         var e = {
             406: 0
         };
         S.f.j = (r, t) => {
             var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(430|526|671)$/.test(r)) e[r] = 0;
+                else if (/^([58]26|671)$/.test(r)) e[r] = 0;
             else {
                 var a = new Promise(((t, a) => n = e[r] = [t, a]));
                 t.push(n[2] = a);
                 var o = S.p + S.u(r),
                     i = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428572%*

 * *Differences: {"'packages'": "{1: {'versionInfo': '0.1.1'}, 2: {'versionInfo': '0.1.1'}}"}*

```diff
@@ -6,21 +6,21 @@
             "name": "@jupyterlab/services",
             "versionInfo": "6.5.3"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/javascript-kernel",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/kernel",
-            "versionInfo": "0.1.0"
+            "versionInfo": "0.1.1"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2016 Christian Speckner <cnspeckn@googlemail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "async-mutex",
             "versionInfo": "0.3.2"
         },
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971875%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/pyodide-kernel': '^0.0.9'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.703f03086e9738104706.js'}}",*

 * * "'version'": "'0.0.9'"}*

```diff
@@ -3,15 +3,15 @@
     "bugs": {
         "url": "https://github.com/jupyterlite/pyodide-kernel/issues"
     },
     "dependencies": {
         "@jupyterlab/coreutils": "^5.5.2",
         "@jupyterlite/contents": "^0.1.0-beta.18",
         "@jupyterlite/kernel": "^0.1.0-beta.18",
-        "@jupyterlite/pyodide-kernel": "^0.0.8",
+        "@jupyterlite/pyodide-kernel": "^0.0.9",
         "@jupyterlite/server": "^0.1.0-beta.18"
     },
     "description": "JupyterLite - Pyodide Kernel Extension",
     "devDependencies": {
         "@jupyterlab/builder": "^3.5.0",
         "rimraf": "~3.0.0",
         "typescript": "~4.9.4"
@@ -28,15 +28,15 @@
         "style/index.js",
         "schema/*.json"
     ],
     "homepage": "https://github.com/jupyterlite/pyodide-kernel",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b340cae4b3c1bda6a7fd.js"
+            "load": "static/remoteEntry.703f03086e9738104706.js"
         },
         "extension": true,
         "outputDir": "../../jupyterlite_pyodide_kernel/labextension",
         "sharedPackages": {
             "@jupyterlite/contents": {
                 "bundled": false,
                 "singleton": true
@@ -85,9 +85,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "types": "lib/index.d.ts",
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/324.2759063405b36360da9d.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
-/*! For license information please see 518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt */
+/*! For license information please see 324.2759063405b36360da9d.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_jupyterlite_pyodide_kernel_extension = self.webpackChunk_jupyterlite_pyodide_kernel_extension || []).push([
-    [518], {
-        2: (e, t, n) => {
+    [324], {
+        742: (e, t, n) => {
             n.r(t), n.d(t, {
                 PIPLITE_INDEX_SCHEMA: () => D,
                 PyodideKernel: () => H,
                 PyodideRemoteKernel: () => N.O,
                 allJSONUrl: () => a,
                 ipykernelWheelUrl: () => i,
                 pipliteWheelUrl: () => l,
@@ -14,17 +14,17 @@
                 widgetsnbextensionWheelUrl: () => d,
                 widgetsnbextensionWheelUrl1: () => h
             });
             const r = n.p + "pypi/all.json";
             var a = n.t(r);
             const s = n.p + "pypi/ipykernel-6.9.2-py3-none-any.whl";
             var i = n.t(s);
-            const o = n.p + "pypi/piplite-0.0.8-py3-none-any.whl";
+            const o = n.p + "pypi/piplite-0.0.9-py3-none-any.whl";
             var l = n.t(o);
-            const c = n.p + "pypi/pyodide_kernel-0.0.8-py3-none-any.whl";
+            const c = n.p + "pypi/pyodide_kernel-0.0.9-py3-none-any.whl";
             var p = n.t(c);
             const u = n.p + "pypi/widgetsnbextension-3.6.4-py3-none-any.whl";
             var d = n.t(u);
             const m = n.p + "pypi/widgetsnbextension-4.0.7-py3-none-any.whl";
             var h = n.t(m),
                 y = n(526),
                 g = n(671),
@@ -439,8 +439,8 @@
             }
             const I = n.p + "schema/piplite.v0.schema.json";
             var D = n.t(I),
                 N = n(951)
         }
     }
 ]);
-//# sourceMappingURL=518.a3c6a3ae7ee95e5158aa.js.map?v=a3c6a3ae7ee95e5158aa
+//# sourceMappingURL=324.2759063405b36360da9d.js.map?v=2759063405b36360da9d
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.ecdf94afc2748b3fc2e0.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
                 p = [{
                     id: d,
                     autoStart: !0,
                     requires: [s.IKernelSpecs],
                     optional: [i.IServiceWorkerManager, r.IBroadcastChannelWrapper],
                     activate: (e, l, i, s) => {
                         const r = JSON.parse(t.PageConfig.getOption("litePluginSettings") || "{}")[d] || {},
-                            a = r.pyodideUrl || "https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js",
+                            a = r.pyodideUrl || "https://cdn.jsdelivr.net/pyodide/v0.23.4/full/pyodide.js",
                             o = t.URLExt.parse(a).href,
                             p = r.pipliteWheelUrl ? t.URLExt.parse(r.pipliteWheelUrl).href : void 0,
                             c = (r.pipliteUrls || []).map((e => t.URLExt.parse(e).href)),
                             v = !!r.disablePyPIFallback;
                         l.register({
                             spec: {
                                 name: "python",
@@ -36,15 +36,15 @@
                                     "logo-32x32": h,
                                     "logo-64x64": h
                                 }
                             },
                             create: async e => {
                                 const {
                                     PyodideKernel: l
-                                } = await n.e(52).then(n.t.bind(n, 52, 23)), t = !(!(null == i ? void 0 : i.enabled) || !(null == s ? void 0 : s.enabled));
+                                } = await n.e(828).then(n.t.bind(n, 828, 23)), t = !(!(null == i ? void 0 : i.enabled) || !(null == s ? void 0 : s.enabled));
                                 return t ? console.info("Pyodide contents will be synced with Jupyter Contents") : console.warn("Pyodide contents will NOT be synced with Jupyter Contents"), new l({
                                     ...e,
                                     pyodideUrl: o,
                                     pipliteWheelUrl: p,
                                     pipliteUrls: c,
                                     disablePyPIFallback: v,
                                     mountDrive: t
@@ -52,8 +52,8 @@
                             }
                         })
                     }
                 }]
         }
     }
 ]);
-//# sourceMappingURL=652.07cda501733578161e13.js.map?v=07cda501733578161e13
+//# sourceMappingURL=652.ecdf94afc2748b3fc2e0.js.map?v=ecdf94afc2748b3fc2e0
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8656250000000001%*

 * *Differences: {"'ipykernel'": "{'releases': {'6.9.2': {0: {'digests': {'md5': "*

 * *                "'79e6908c1898dab331c487c46ca355bc', 'sha256': "*

 * *                "'e5bf6bf7c38ffbb71085a95f7eb55d55e89c82fab61fd9361e317fcb90360130'}, "*

 * *                "'md5_digest': '79e6908c1898dab331c487c46ca355bc', 'size': 6513, 'upload_time': "*

 * *                "'2023-08-02T12:44:14.557813Z', 'upload_time_iso_8601': "*

 * *                "'2023-08-02T12:44:14.557813Z'}}}}",*

 * * "'piplite'": "{'releases': {replace: OrderedDict([('0.0.9', [Ordere […]*

```diff
@@ -1,127 +1,127 @@
 {
     "ipykernel": {
         "releases": {
             "6.9.2": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "50b0ac28df1e02972a7ba285a5498af8",
-                        "sha256": "cc0462b5e9eb7fcbe412f1c2f716c3d13a4ad567c418afa253d974e631341f26"
+                        "md5": "79e6908c1898dab331c487c46ca355bc",
+                        "sha256": "e5bf6bf7c38ffbb71085a95f7eb55d55e89c82fab61fd9361e317fcb90360130"
                     },
                     "downloads": -1,
                     "filename": "ipykernel-6.9.2-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "50b0ac28df1e02972a7ba285a5498af8",
+                    "md5_digest": "79e6908c1898dab331c487c46ca355bc",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": ">=3.10",
-                    "size": 6512,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
+                    "size": 6513,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
                     "url": "./ipykernel-6.9.2-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     },
     "piplite": {
         "releases": {
-            "0.0.8": [
+            "0.0.9": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "653e410da79aef82d7b7dcc25500033e",
-                        "sha256": "94fb854bc4a72fd9dcdbae39d719294166dda95cdec3dadcd2468dfd5962c444"
+                        "md5": "d37090e6a13ea988333a51ab1fa865fa",
+                        "sha256": "1797f065c1e845e29960333955d0b9222d97ed0dbcae422872ac0c0713201031"
                     },
                     "downloads": -1,
-                    "filename": "piplite-0.0.8-py3-none-any.whl",
+                    "filename": "piplite-0.0.9-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "653e410da79aef82d7b7dcc25500033e",
+                    "md5_digest": "d37090e6a13ea988333a51ab1fa865fa",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 6720,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
-                    "url": "./piplite-0.0.8-py3-none-any.whl",
+                    "size": 6718,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
+                    "url": "./piplite-0.0.9-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     },
     "pyodide-kernel": {
         "releases": {
-            "0.0.8": [
+            "0.0.9": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "e7a145dc94d6973a2e5c302a354d5768",
-                        "sha256": "66d2829fb698aa2a6360871960eb8df4e661cf637ad1ba94b3e003eaefe4fcf7"
+                        "md5": "0df4ba9b821f1fa6f176ca7e4d6e382a",
+                        "sha256": "d2224fe7066ce8b372e20d7aa1f8d69e5ed1b2547340331d8ea5b01402279403"
                     },
                     "downloads": -1,
-                    "filename": "pyodide_kernel-0.0.8-py3-none-any.whl",
+                    "filename": "pyodide_kernel-0.0.9-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "e7a145dc94d6973a2e5c302a354d5768",
+                    "md5_digest": "0df4ba9b821f1fa6f176ca7e4d6e382a",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 8221,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
-                    "url": "./pyodide_kernel-0.0.8-py3-none-any.whl",
+                    "size": 8222,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
+                    "url": "./pyodide_kernel-0.0.9-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     },
     "widgetsnbextension": {
         "releases": {
             "3.6.4": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "0c562267b54decbba3df65748e8a50c1",
-                        "sha256": "508cf73575b9efb7fe405f50a52c5fbb0a4d5f7ebe3b8e5098c13f74bc58a366"
+                        "md5": "cacd42516decc405948cc366d99deeef",
+                        "sha256": "8e2dc2570bf54e61aedd2c52ebae4e048a7d860bad3f6a5eec0b2c7529807bcc"
                     },
                     "downloads": -1,
                     "filename": "widgetsnbextension-3.6.4-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "0c562267b54decbba3df65748e8a50c1",
+                    "md5_digest": "cacd42516decc405948cc366d99deeef",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 2337,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
+                    "size": 2338,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
                     "url": "./widgetsnbextension-3.6.4-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ],
             "4.0.7": [
                 {
                     "comment_text": "",
                     "digests": {
-                        "md5": "522d33a007aa29a012295f9505f093d5",
-                        "sha256": "d0fb5501925193f011d56ea7df530cff64ed90fdce2c5aa8d7cb755953694a10"
+                        "md5": "6c1bf4b38ec6a57b885322f085902e88",
+                        "sha256": "8933202971deb5120a9ebb518a640b51acbb37ae54e8623ad7883c348e6646ad"
                     },
                     "downloads": -1,
                     "filename": "widgetsnbextension-4.0.7-py3-none-any.whl",
                     "has_sig": false,
-                    "md5_digest": "522d33a007aa29a012295f9505f093d5",
+                    "md5_digest": "6c1bf4b38ec6a57b885322f085902e88",
                     "packagetype": "bdist_wheel",
                     "python_version": "py3",
                     "requires_python": "<3.12,>=3.11",
-                    "size": 2337,
-                    "upload_time": "2023-05-04T13:13:10.906368Z",
-                    "upload_time_iso_8601": "2023-05-04T13:13:10.906368Z",
+                    "size": 2338,
+                    "upload_time": "2023-08-02T12:44:14.557813Z",
+                    "upload_time_iso_8601": "2023-08-02T12:44:14.557813Z",
                     "url": "./widgetsnbextension-4.0.7-py3-none-any.whl",
                     "yanked": false,
                     "yanked_reason": null
                 }
             ]
         }
     }
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6512 bytes, number of entries: 7
--rw-r--r--  2.0 unx      133 b- defN 23-May-04 13:01 ipykernel/__init__.py
--rw-r--r--  2.0 unx     7026 b- defN 23-May-04 13:01 ipykernel/comm.py
--rw-r--r--  2.0 unx     5102 b- defN 23-May-04 13:01 ipykernel/jsonutil.py
-?rw-r--r--  2.0 unx      424 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      539 b- defN 23-May-04 13:01 ipykernel-6.9.2.dist-info/RECORD
-7 files, 14835 bytes uncompressed, 5562 bytes compressed:  62.5%
+Zip file size: 6513 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      133 b- defN 23-Aug-02 07:20 ipykernel/__init__.py
+-rw-r--r--  2.0 unx     7026 b- defN 23-Aug-02 07:20 ipykernel/comm.py
+-rw-r--r--  2.0 unx     5102 b- defN 23-Aug-02 07:20 ipykernel/jsonutil.py
+?rw-r--r--  2.0 unx      424 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      539 b- defN 23-Aug-02 07:20 ipykernel-6.9.2.dist-info/RECORD
+7 files, 14835 bytes uncompressed, 5563 bytes compressed:  62.5%
```

#### ipykernel-6.9.2.dist-info/WHEEL

```diff
@@ -1,4 +1,4 @@
 Wheel-Version: 1.0
-Generator: hatchling 1.14.1
+Generator: hatchling 1.18.0
 Root-Is-Purelib: true
 Tag: py3-none-any
```

#### ipykernel-6.9.2.dist-info/RECORD

```diff
@@ -1,7 +1,7 @@
 ipykernel/__init__.py,sha256=RJFGnC1Jf4urbq3S1FDJmGGbAkyANMuPFftZDR20d2E,133
 ipykernel/comm.py,sha256=wsdtPIjlzPI72CdFqpVn5mJBp4qAI1Ut7tEgBtQ3x8w,7026
 ipykernel/jsonutil.py,sha256=7kInhZjFl4q3WNo9tz10Gy6N5tsbiF7R6buIYh8oCBA,5102
 ipykernel-6.9.2.dist-info/METADATA,sha256=ePjA9gFWVMXeJlT7vSr5Mb7SloZmarODuFFuXRw5484,424
-ipykernel-6.9.2.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+ipykernel-6.9.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
 ipykernel-6.9.2.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
 ipykernel-6.9.2.dist-info/RECORD,,
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.9-py3-none-any.whl`

 * *Files 19% similar despite different names*

#### zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6720 bytes, number of entries: 7
--rw-r--r--  2.0 unx      155 b- defN 23-May-04 13:01 piplite/__init__.py
--rw-r--r--  2.0 unx     4720 b- defN 23-May-04 13:01 piplite/cli.py
--rw-r--r--  2.0 unx     6574 b- defN 23-May-04 13:01 piplite/piplite.py
-?rw-r--r--  2.0 unx      631 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      523 b- defN 23-May-04 13:01 piplite-0.0.8.dist-info/RECORD
-7 files, 14214 bytes uncompressed, 5802 bytes compressed:  59.2%
+Zip file size: 6718 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      155 b- defN 23-Aug-02 07:20 piplite/__init__.py
+-rw-r--r--  2.0 unx     4720 b- defN 23-Aug-02 07:20 piplite/cli.py
+-rw-r--r--  2.0 unx     6574 b- defN 23-Aug-02 07:20 piplite/piplite.py
+?rw-r--r--  2.0 unx      631 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      523 b- defN 23-Aug-02 07:20 piplite-0.0.9.dist-info/RECORD
+7 files, 14214 bytes uncompressed, 5800 bytes compressed:  59.2%
```

#### zipnote «TEMP»/diffoscope_kwcs9s51_/tmpgculi49i_.zip

```diff
@@ -3,20 +3,20 @@
 
 Filename: piplite/cli.py
 Comment: 
 
 Filename: piplite/piplite.py
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/METADATA
+Filename: piplite-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/WHEEL
+Filename: piplite-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/licenses/LICENSE
+Filename: piplite-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: piplite-0.0.8.dist-info/RECORD
+Filename: piplite-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### piplite/__init__.py

```diff
@@ -1,6 +1,6 @@
 """A configurable Python package backed by Pyodide's micropip"""
 from .piplite import install
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 __all__ = ["install", "__version__"]
```

#### Comparing `piplite-0.0.8.dist-info/METADATA` & `piplite-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piplite
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Source, https://github.com/jupyterlite/pyodide-kernel
 Author: JupyterLite Contributors
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: <3.12,>=3.11
 Description-Content-Type: text/markdown
```

#### Comparing `piplite-0.0.8.dist-info/licenses/LICENSE` & `piplite-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.9-py3-none-any.whl`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8221 bytes, number of entries: 11
--rw-r--r--  2.0 unx      712 b- defN 23-May-04 13:01 pyodide_kernel/__init__.py
--rw-r--r--  2.0 unx     2269 b- defN 23-May-04 13:01 pyodide_kernel/display.py
--rw-r--r--  2.0 unx     2454 b- defN 23-May-04 13:01 pyodide_kernel/interpreter.py
--rw-r--r--  2.0 unx     3992 b- defN 23-May-04 13:01 pyodide_kernel/kernel.py
--rw-r--r--  2.0 unx     3197 b- defN 23-May-04 13:01 pyodide_kernel/litetransform.py
--rw-r--r--  2.0 unx     1290 b- defN 23-May-04 13:01 pyodide_kernel/mocks.py
--rw-r--r--  2.0 unx      404 b- defN 23-May-04 13:01 pyodide_kernel/patches.py
-?rw-r--r--  2.0 unx      480 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      910 b- defN 23-May-04 13:01 pyodide_kernel-0.0.8.dist-info/RECORD
-11 files, 17319 bytes uncompressed, 6679 bytes compressed:  61.4%
+Zip file size: 8222 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      712 b- defN 23-Aug-02 07:20 pyodide_kernel/__init__.py
+-rw-r--r--  2.0 unx     2269 b- defN 23-Aug-02 07:20 pyodide_kernel/display.py
+-rw-r--r--  2.0 unx     2454 b- defN 23-Aug-02 07:20 pyodide_kernel/interpreter.py
+-rw-r--r--  2.0 unx     3992 b- defN 23-Aug-02 07:20 pyodide_kernel/kernel.py
+-rw-r--r--  2.0 unx     3197 b- defN 23-Aug-02 07:20 pyodide_kernel/litetransform.py
+-rw-r--r--  2.0 unx     1290 b- defN 23-Aug-02 07:20 pyodide_kernel/mocks.py
+-rw-r--r--  2.0 unx      404 b- defN 23-Aug-02 07:20 pyodide_kernel/patches.py
+?rw-r--r--  2.0 unx      480 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      910 b- defN 23-Aug-02 07:20 pyodide_kernel-0.0.9.dist-info/RECORD
+11 files, 17319 bytes uncompressed, 6680 bytes compressed:  61.4%
```

#### zipnote «TEMP»/diffoscope_kwcs9s51_/tmpm1udb18y_.zip

```diff
@@ -15,20 +15,20 @@
 
 Filename: pyodide_kernel/mocks.py
 Comment: 
 
 Filename: pyodide_kernel/patches.py
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/METADATA
+Filename: pyodide_kernel-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/WHEEL
+Filename: pyodide_kernel-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/licenses/LICENSE
+Filename: pyodide_kernel-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pyodide_kernel-0.0.8.dist-info/RECORD
+Filename: pyodide_kernel-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### pyodide_kernel/__init__.py

```diff
@@ -1,10 +1,10 @@
 """A Python kernel backed by Pyodide"""
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import sys
 
 # 0. do early mocks that change `sys.modules`
 from . import mocks
 
 mocks.apply_mocks()
```

#### Comparing `pyodide_kernel-0.0.8.dist-info/licenses/LICENSE` & `pyodide_kernel-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

#### Comparing `pyodide_kernel-0.0.8.dist-info/RECORD` & `pyodide_kernel-0.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyodide_kernel/__init__.py,sha256=dYfAxEhgAibmjAiInRjyrR3pcJf_wRJEJxoGXvwKlAM,712
+pyodide_kernel/__init__.py,sha256=Qnl9_48L6uB-riqcyTHIlruB8qq2ZT0wjThLStcnh4A,712
 pyodide_kernel/display.py,sha256=j_iSs9w55XmCy9XpHReCQR2OGFUMnkMoAKMp_sqBT5I,2269
 pyodide_kernel/interpreter.py,sha256=YFyEXcTpjQqPWExo0MQa8COVraO8Ihz8bobon5Ye-48,2454
 pyodide_kernel/kernel.py,sha256=0ofEqk2yimW6J8wpnCeIdxz6BujUOLxbmeUT3zdaCRo,3992
 pyodide_kernel/litetransform.py,sha256=Iqlxj39Y-P0O1Wjk3kXi1Sqo--IL4ROLV-L_s2jPVbE,3197
 pyodide_kernel/mocks.py,sha256=X49fD89PBn-rVNvkDcbGrDhMpg3Ybc1mhc-Bo0tqI8o,1290
 pyodide_kernel/patches.py,sha256=ApUGlW0FYBdKrLQx8wiqt0jLxrJnm5CxYBVHmlCnSVQ,404
-pyodide_kernel-0.0.8.dist-info/METADATA,sha256=cqQONeS_vb2-now9zyPMLSeS83mDAntDbx41bSUW4PQ,480
-pyodide_kernel-0.0.8.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-pyodide_kernel-0.0.8.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
-pyodide_kernel-0.0.8.dist-info/RECORD,,
+pyodide_kernel-0.0.9.dist-info/METADATA,sha256=SMhPNseQ3MfZP5r3P25ugDZH6fmAfHni7VtbTl79XF8,480
+pyodide_kernel-0.0.9.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+pyodide_kernel-0.0.9.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
+pyodide_kernel-0.0.9.dist-info/RECORD,,
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2337 bytes, number of entries: 5
--rw-r--r--  2.0 unx       55 b- defN 23-May-04 13:01 widgetsnbextension/__init__.py
-?rw-r--r--  2.0 unx      492 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      431 b- defN 23-May-04 13:01 widgetsnbextension-3.6.4.dist-info/RECORD
-5 files, 2589 bytes uncompressed, 1525 bytes compressed:  41.1%
+Zip file size: 2338 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       55 b- defN 23-Aug-02 07:20 widgetsnbextension/__init__.py
+?rw-r--r--  2.0 unx      492 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      431 b- defN 23-Aug-02 07:20 widgetsnbextension-3.6.4.dist-info/RECORD
+5 files, 2589 bytes uncompressed, 1526 bytes compressed:  41.1%
```

#### widgetsnbextension-3.6.4.dist-info/WHEEL

```diff
@@ -1,4 +1,4 @@
 Wheel-Version: 1.0
-Generator: hatchling 1.14.1
+Generator: hatchling 1.18.0
 Root-Is-Purelib: true
 Tag: py3-none-any
```

#### widgetsnbextension-3.6.4.dist-info/RECORD

```diff
@@ -1,5 +1,5 @@
 widgetsnbextension/__init__.py,sha256=Ehhe-iBe2kPDIVP1GNDa2H2FK8miBEV6ZRcDdsXCwa0,55
 widgetsnbextension-3.6.4.dist-info/METADATA,sha256=POvFnV5PBUrTYnef8n-JNTGFvU2fCsQal6LZSB6cLcg,492
-widgetsnbextension-3.6.4.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+widgetsnbextension-3.6.4.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
 widgetsnbextension-3.6.4.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
 widgetsnbextension-3.6.4.dist-info/RECORD,,
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2337 bytes, number of entries: 5
--rw-r--r--  2.0 unx       55 b- defN 23-May-04 13:01 widgetsnbextension/__init__.py
-?rw-r--r--  2.0 unx      493 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1524 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      431 b- defN 23-May-04 13:01 widgetsnbextension-4.0.7.dist-info/RECORD
-5 files, 2590 bytes uncompressed, 1525 bytes compressed:  41.1%
+Zip file size: 2338 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       55 b- defN 23-Aug-02 07:20 widgetsnbextension/__init__.py
+?rw-r--r--  2.0 unx      493 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1524 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      431 b- defN 23-Aug-02 07:20 widgetsnbextension-4.0.7.dist-info/RECORD
+5 files, 2590 bytes uncompressed, 1526 bytes compressed:  41.1%
```

#### widgetsnbextension-4.0.7.dist-info/WHEEL

```diff
@@ -1,4 +1,4 @@
 Wheel-Version: 1.0
-Generator: hatchling 1.14.1
+Generator: hatchling 1.18.0
 Root-Is-Purelib: true
 Tag: py3-none-any
```

#### widgetsnbextension-4.0.7.dist-info/RECORD

```diff
@@ -1,5 +1,5 @@
 widgetsnbextension/__init__.py,sha256=FUS4iRrSk7iROOXwaTdKPfC1CChNMdht0P2bZQaBVys,55
 widgetsnbextension-4.0.7.dist-info/METADATA,sha256=ggM19V05p03L7JurOviHELE2nzokq4fT1yrTMODRjlo,493
-widgetsnbextension-4.0.7.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+widgetsnbextension-4.0.7.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
 widgetsnbextension-4.0.7.dist-info/licenses/LICENSE,sha256=UC6Zzk30zZ_gsU9qy3yVVTpd2WFZgvskbCMzMPMX7_Q,1524
 widgetsnbextension-4.0.7.dist-info/RECORD,,
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.703f03086e9738104706.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, u, d, f, s, p, c, h, b, v, y, m, g, j = {
+    var e, r, t, n, o, i, a, l, u, d, f, s, c, p, h, b, v, y, m, g, j = {
             405: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(694), t.e(652)]).then((() => () => t(763))),
                         "./extension": () => Promise.all([t.e(694), t.e(652)]).then((() => () => t(763)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -49,26 +49,26 @@
         return i.default = () => t, k.d(o, i), o
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        52: "354648418987bd848171",
-        518: "a3c6a3ae7ee95e5158aa",
+        324: "2759063405b36360da9d",
         568: "371c75f0cd43fa31532d",
-        652: "07cda501733578161e13",
+        652: "ecdf94afc2748b3fc2e0",
         694: "e063d498fa9e311b3f30",
+        828: "18cd1cea0272a9fd42b1",
         951: "b9fa6250974e699a3731"
     } [e] + ".js?v=" + {
-        52: "354648418987bd848171",
-        518: "a3c6a3ae7ee95e5158aa",
+        324: "2759063405b36360da9d",
         568: "371c75f0cd43fa31532d",
-        652: "07cda501733578161e13",
+        652: "ecdf94afc2748b3fc2e0",
         694: "e063d498fa9e311b3f30",
+        828: "18cd1cea0272a9fd42b1",
         951: "b9fa6250974e699a3731"
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -83,19 +83,19 @@
                     if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == n + o) {
                         a = f;
                         break
                     }
                 }
             a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, k.nc && a.setAttribute("nonce", k.nc), a.setAttribute("data-webpack", n + o), a.src = e), t[e] = [r];
             var s = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+                    a.onerror = a.onload = null, clearTimeout(c);
                     var o = t[e];
                     if (delete t[e], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -121,15 +121,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : a > l.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlite/pyodide-kernel-extension", "0.0.8", (() => Promise.all([k.e(694), k.e(652)]).then((() => () => k(763))))), l("@jupyterlite/pyodide-kernel", "0.0.8", (() => Promise.all([k.e(951), k.e(518), k.e(694)]).then((() => () => k(2)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlite/pyodide-kernel-extension", "0.0.9", (() => Promise.all([k.e(694), k.e(652)]).then((() => () => k(763))))), l("@jupyterlite/pyodide-kernel", "0.0.9", (() => Promise.all([k.e(951), k.e(324), k.e(694)]).then((() => () => k(742)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -199,52 +199,52 @@
                     u = !1, a--
                 } else {
                     if (a <= t || f < s != n) return !1;
                     u = !1
                 } else "s" != s && "n" != s && (u = !1, a--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? l(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, u = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && i(e, r) ? r : e), 0)
     }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
         var o = d(e, t);
-        return l(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), c(e[t][o])
-    }, p = (e, r, t) => {
+        return l(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), p(e[t][o])
+    }, c = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !l(t, r) || e && !i(e, r) ? e : r), 0)) && n[r]
-    }, c = e => (e.loaded = 1, e.get()), b = (h = e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), b = (h = e => function(r, t, n, o) {
         var i = k.I(r);
         return i && i.then ? i.then(e.bind(e, r, k.S[r], t, n, o)) : e(r, k.S[r], t, n, o)
     })(((e, r, t, n) => (u(e, t), s(r, 0, t, n)))), v = h(((e, r, t, n, o) => {
-        var i = r && k.o(r, t) && p(r, t, n);
-        return i ? c(i) : o()
+        var i = r && k.o(r, t) && c(r, t, n);
+        return i ? p(i) : o()
     })), y = {}, m = {
         289: () => b("default", "@jupyterlite/kernel", [2, 0, 1, 0, , "beta", 18]),
         671: () => b("default", "@jupyterlab/coreutils", [1, 5, 5, 3]),
         174: () => b("default", "@jupyterlite/server", [2, 0, 1, 0, , "beta", 18]),
         685: () => b("default", "@jupyterlite/contents", [2, 0, 1, 0, , "beta", 18]),
         526: () => b("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        52: () => v("default", "@jupyterlite/pyodide-kernel", [3, 0, 0, 8], (() => Promise.all([k.e(951), k.e(518)]).then((() => () => k(2)))))
+        828: () => v("default", "@jupyterlite/pyodide-kernel", [3, 0, 0, 9], (() => Promise.all([k.e(951), k.e(324)]).then((() => () => k(742)))))
     }, g = {
-        52: [52],
-        518: [526],
+        324: [526],
         652: [174, 685],
-        694: [289, 671]
+        694: [289, 671],
+        828: [828]
     }, k.f.consumes = (e, r) => {
         k.o(g, e) && g[e].forEach((e => {
             if (k.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, k.m[e] = t => {
                         delete k.c[e], t.exports = r()
                     }
@@ -266,15 +266,15 @@
         var e = {
             335: 0
         };
         k.f.j = (r, t) => {
             var n = k.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(52|694)$/.test(r)) e[r] = 0;
+                else if (/^(694|828)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
                 var i = k.p + k.u(r),
                     a = new Error;
                 k.l(i, (t => {
                     if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
@@ -296,8 +296,8 @@
             },
             t = self.webpackChunk_jupyterlite_pyodide_kernel_extension = self.webpackChunk_jupyterlite_pyodide_kernel_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var P = k(405);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlite/pyodide-kernel-extension"] = P
 })();
-//# sourceMappingURL=remoteEntry.b340cae4b3c1bda6a7fd.js.map
+//# sourceMappingURL=remoteEntry.703f03086e9738104706.js.map
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'properties'": "{'pyodideUrl': {'default': "*

 * *                 "'https://cdn.jsdelivr.net/pyodide/v0.23.4/full/pyodide.js'}}"}*

```diff
@@ -14,15 +14,15 @@
             "format": "uri",
             "items": {
                 "type": "string"
             },
             "type": "array"
         },
         "pyodideUrl": {
-            "default": "https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js",
+            "default": "https://cdn.jsdelivr.net/pyodide/v0.23.4/full/pyodide.js",
             "description": "The path to the main pyodide.js entry point",
             "format": "uri",
             "type": "string"
         }
     },
     "title": "Pyodide Kernel Settings Schema v0",
     "type": "object"
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '0.0.9'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "BSD 3-Clause License\n\nCopyright (c) 2022, JupyterLite Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/pyodide-kernel",
-            "versionInfo": "0.0.8"
+            "versionInfo": "0.0.9"
         },
         {
             "extractedText": "\n                                 Apache License\n                           Version 2.0, January 2004\n                        http://www.apache.org/licenses/\n\n   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION\n\n   1. Definitions.\n\n      \"License\" shall mean the terms and conditions for use, reproduction,\n      and distribution as defined by Sections 1 through 9 of this document.\n\n      \"Licensor\" shall mean the copyright owner or entity authorized by\n      the copyright owner that is granting the License.\n\n      \"Legal Entity\" shall mean the union of the acting entity and all\n      other entities that control, are controlled by, or are under common\n      control with that entity. For the purposes of this definition,\n      \"control\" means (i) the power, direct or indirect, to cause the\n      direction or management of such entity, whether by contract or\n      otherwise, or (ii) ownership of fifty percent (50%) or more of the\n      outstanding shares, or (iii) beneficial ownership of such entity.\n\n      \"You\" (or \"Your\") shall mean an individual or Legal Entity\n      exercising permissions granted by this License.\n\n      \"Source\" form shall mean the preferred form for making modifications,\n      including but not limited to software source code, documentation\n      source, and configuration files.\n\n      \"Object\" form shall mean any form resulting from mechanical\n      transformation or translation of a Source form, including but\n      not limited to compiled object code, generated documentation,\n      and conversions to other media types.\n\n      \"Work\" shall mean the work of authorship, whether in Source or\n      Object form, made available under the License, as indicated by a\n      copyright notice that is included in or attached to the work\n      (an example is provided in the Appendix below).\n\n      \"Derivative Works\" shall mean any work, whether in Source or Object\n      form, that is based on (or derived from) the Work and for which the\n      editorial revisions, annotations, elaborations, or other modifications\n      represent, as a whole, an original work of authorship. For the purposes\n      of this License, Derivative Works shall not include works that remain\n      separable from, or merely link (or bind by name) to the interfaces of,\n      the Work and Derivative Works thereof.\n\n      \"Contribution\" shall mean any work of authorship, including\n      the original version of the Work and any modifications or additions\n      to that Work or Derivative Works thereof, that is intentionally\n      submitted to Licensor for inclusion in the Work by the copyright owner\n      or by an individual or Legal Entity authorized to submit on behalf of\n      the copyright owner. For the purposes of this definition, \"submitted\"\n      means any form of electronic, verbal, or written communication sent\n      to the Licensor or its representatives, including but not limited to\n      communication on electronic mailing lists, source code control systems,\n      and issue tracking systems that are managed by, or on behalf of, the\n      Licensor for the purpose of discussing and improving the Work, but\n      excluding communication that is conspicuously marked or otherwise\n      designated in writing by the copyright owner as \"Not a Contribution.\"\n\n      \"Contributor\" shall mean Licensor and any individual or Legal Entity\n      on behalf of whom a Contribution has been received by Licensor and\n      subsequently incorporated within the Work.\n\n   2. Grant of Copyright License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      copyright license to reproduce, prepare Derivative Works of,\n      publicly display, publicly perform, sublicense, and distribute the\n      Work and such Derivative Works in Source or Object form.\n\n   3. Grant of Patent License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      (except as stated in this section) patent license to make, have made,\n      use, offer to sell, sell, import, and otherwise transfer the Work,\n      where such license applies only to those patent claims licensable\n      by such Contributor that are necessarily infringed by their\n      Contribution(s) alone or by combination of their Contribution(s)\n      with the Work to which such Contribution(s) was submitted. If You\n      institute patent litigation against any entity (including a\n      cross-claim or counterclaim in a lawsuit) alleging that the Work\n      or a Contribution incorporated within the Work constitutes direct\n      or contributory patent infringement, then any patent licenses\n      granted to You under this License for that Work shall terminate\n      as of the date such litigation is filed.\n\n   4. Redistribution. You may reproduce and distribute copies of the\n      Work or Derivative Works thereof in any medium, with or without\n      modifications, and in Source or Object form, provided that You\n      meet the following conditions:\n\n      (a) You must give any other recipients of the Work or\n          Derivative Works a copy of this License; and\n\n      (b) You must cause any modified files to carry prominent notices\n          stating that You changed the files; and\n\n      (c) You must retain, in the Source form of any Derivative Works\n          that You distribute, all copyright, patent, trademark, and\n          attribution notices from the Source form of the Work,\n          excluding those notices that do not pertain to any part of\n          the Derivative Works; and\n\n      (d) If the Work includes a \"NOTICE\" text file as part of its\n          distribution, then any Derivative Works that You distribute must\n          include a readable copy of the attribution notices contained\n          within such NOTICE file, excluding those notices that do not\n          pertain to any part of the Derivative Works, in at least one\n          of the following places: within a NOTICE text file distributed\n          as part of the Derivative Works; within the Source form or\n          documentation, if provided along with the Derivative Works; or,\n          within a display generated by the Derivative Works, if and\n          wherever such third-party notices normally appear. The contents\n          of the NOTICE file are for informational purposes only and\n          do not modify the License. You may add Your own attribution\n          notices within Derivative Works that You distribute, alongside\n          or as an addendum to the NOTICE text from the Work, provided\n          that such additional attribution notices cannot be construed\n          as modifying the License.\n\n      You may add Your own copyright statement to Your modifications and\n      may provide additional or different license terms and conditions\n      for use, reproduction, or distribution of Your modifications, or\n      for any such Derivative Works as a whole, provided Your use,\n      reproduction, and distribution of the Work otherwise complies with\n      the conditions stated in this License.\n\n   5. Submission of Contributions. Unless You explicitly state otherwise,\n      any Contribution intentionally submitted for inclusion in the Work\n      by You to the Licensor shall be under the terms and conditions of\n      this License, without any additional terms or conditions.\n      Notwithstanding the above, nothing herein shall supersede or modify\n      the terms of any separate license agreement you may have executed\n      with Licensor regarding such Contributions.\n\n   6. Trademarks. This License does not grant permission to use the trade\n      names, trademarks, service marks, or product names of the Licensor,\n      except as required for reasonable and customary use in describing the\n      origin of the Work and reproducing the content of the NOTICE file.\n\n   7. Disclaimer of Warranty. Unless required by applicable law or\n      agreed to in writing, Licensor provides the Work (and each\n      Contributor provides its Contributions) on an \"AS IS\" BASIS,\n      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or\n      implied, including, without limitation, any warranties or conditions\n      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A\n      PARTICULAR PURPOSE. You are solely responsible for determining the\n      appropriateness of using or redistributing the Work and assume any\n      risks associated with Your exercise of permissions under this License.\n\n   8. Limitation of Liability. In no event and under no legal theory,\n      whether in tort (including negligence), contract, or otherwise,\n      unless required by applicable law (such as deliberate and grossly\n      negligent acts) or agreed to in writing, shall any Contributor be\n      liable to You for damages, including any direct, indirect, special,\n      incidental, or consequential damages of any character arising as a\n      result of this License or out of the use or inability to use the\n      Work (including but not limited to damages for loss of goodwill,\n      work stoppage, computer failure or malfunction, or any and all\n      other commercial damages or losses), even if such Contributor\n      has been advised of the possibility of such damages.\n\n   9. Accepting Warranty or Additional Liability. While redistributing\n      the Work or Derivative Works thereof, You may choose to offer,\n      and charge a fee for, acceptance of support, warranty, indemnity,\n      or other liability obligations and/or rights consistent with this\n      License. However, in accepting such obligations, You may act only\n      on Your own behalf and on Your sole responsibility, not on behalf\n      of any other Contributor, and only if You agree to indemnify,\n      defend, and hold each Contributor harmless for any liability\n      incurred by, or claims asserted against, such Contributor by reason\n      of your accepting any such warranty or additional liability.\n\n   END OF TERMS AND CONDITIONS\n\n   APPENDIX: How to apply the Apache License to your work.\n\n      To apply the Apache License to your work, attach the following\n      boilerplate notice, with the fields enclosed by brackets \"[]\"\n      replaced with your own identifying information. (Don't include\n      the brackets!)  The text should be enclosed in the appropriate\n      comment syntax for the file format. We also recommend that a\n      file or class name and description of purpose be included on the\n      same \"printed page\" as the copyright notice for easier\n      identification within third-party archives.\n\n   Copyright 2017 Google Inc.\n\n   Licensed under the Apache License, Version 2.0 (the \"License\");\n   you may not use this file except in compliance with the License.\n   You may obtain a copy of the License at\n\n       http://www.apache.org/licenses/LICENSE-2.0\n\n   Unless required by applicable law or agreed to in writing, software\n   distributed under the License is distributed on an \"AS IS\" BASIS,\n   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n   See the License for the specific language governing permissions and\n   limitations under the License.",
             "licenseId": "Apache-2.0",
             "name": "comlink",
             "versionInfo": "4.4.1"
         },
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `resotocore-3.6.5/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/files/example.ipynb` & `resotocore-3.6.5/resotocore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/icon-120x120.png` & `resotocore-3.6.5/resotocore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/icon-512x512.png` & `resotocore-3.6.5/resotocore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/index.html` & `resotocore-3.6.5/resotocore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/jupyter-lite.ipynb` & `resotocore-3.6.5/resotocore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/jupyter-lite.json` & `resotocore-3.6.5/resotocore/jupyterlite/jupyter-lite.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98828125%*

 * *Differences: {"'jupyter-config-data'": "{'appVersion': '0.1.1', 'federated_extensions': {0: {'load': "*

 * *                          "'static/remoteEntry.9eaa8a846d81f5b6c8be.js'}, 1: {'load': "*

 * *                          "'static/remoteEntry.703f03086e9738104706.js'}}, 'litePluginSettings': "*

 * *                          "{'@jupyterlite/pyodide-kernel-extension:kernel': {'pipliteUrls': "*

 * *                          "['./extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json?sha256=c34f9fdb521c609edea81ebbb122612d7 […]*

```diff
@@ -1,26 +1,26 @@
 {
     "jupyter-config-data": {
         "appName": "JupyterLite",
         "appUrl": "./lab",
-        "appVersion": "0.1.0",
+        "appVersion": "0.1.1",
         "baseUrl": "./",
         "defaultKernelName": "python",
         "faviconUrl": "./lab/favicon.ico",
         "federated_extensions": [
             {
                 "extension": "./extension",
                 "liteExtension": true,
-                "load": "static/remoteEntry.7e46d8af7cfb9637087e.js",
+                "load": "static/remoteEntry.9eaa8a846d81f5b6c8be.js",
                 "name": "@jupyterlite/javascript-kernel-extension"
             },
             {
                 "extension": "./extension",
                 "liteExtension": true,
-                "load": "static/remoteEntry.b340cae4b3c1bda6a7fd.js",
+                "load": "static/remoteEntry.703f03086e9738104706.js",
                 "name": "@jupyterlite/pyodide-kernel-extension"
             },
             {
                 "extension": "./extension",
                 "liteExtension": false,
                 "load": "static/remoteEntry.d87fbfbef62a029ce69b.js",
                 "mimeExtension": "./mimeExtension",
@@ -310,15 +310,15 @@
         "fullLabextensionsUrl": "./extensions",
         "fullMathjaxUrl": "https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js",
         "fullStaticUrl": "./build",
         "licensesUrl": "./lab/api/licenses",
         "litePluginSettings": {
             "@jupyterlite/pyodide-kernel-extension:kernel": {
                 "pipliteUrls": [
-                    "./extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json?sha256=55f1d3982adfce14adaebe30c941e4857226d00982e31d3c3a92acf14de17eac"
+                    "./extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json?sha256=c34f9fdb521c609edea81ebbb122612d7d7c9e2ad738d791fa77622d0f03be12"
                 ]
             }
         },
         "mathjaxConfig": "TeX-AMS_CHTML-full,Safe"
     },
     "jupyter-lite-schema-version": 0
 }
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/jupyterlite.schema.v0.json` & `resotocore-3.6.5/resotocore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/kernelspecs/javascript.svg` & `resotocore-3.6.5/resotocore/jupyterlite/kernelspecs/javascript.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/lab/favicon.ico` & `resotocore-3.6.5/resotocore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/lab/index.html` & `resotocore-3.6.5/resotocore/jupyterlite/lab/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <meta name="Description" content="WASM powered Jupyter running in the browser." />
     <link rel="manifest" href="../manifest.webmanifest" />
     <link
       id="jupyter-lite-main"
       rel="preload"
-      href="../build/lab/bundle.js?_=4a04b99"
+      href="../build/lab/bundle.js?_=e57205c"
       main="index"
       as="script"
     />
     <script
       id="jupyter-config-data"
       type="application/json"
       data-jupyter-lite-root=".."
@@ -24,13 +24,13 @@
       (async function () {
         const { pathname, origin, search, hash } = window.location;
         if (pathname.match(/(index.html|\/)$/) == null) {
           window.location.href = `${origin}${pathname}/${search}${hash}`;
           return;
         }
         await import(
-          '../config-utils.js?_=4a04b99'
+          '../config-utils.js?_=e57205c'
         );
       }.call(this));
     </script>
   </head>
 </html>
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/lab/jupyter-lite.ipynb` & `resotocore-3.6.5/resotocore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/lab/package.json` & `resotocore-3.6.5/resotocore/jupyterlite/lab/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9192489495798319%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/application-extension': '^0.1.1', "*

 * *                   "'@jupyterlite/iframe-extension': '^0.1.1', '@jupyterlite/licenses': '^0.1.1', "*

 * *                   "'@jupyterlite/localforage': '^0.1.1', '@jupyterlite/server': '^0.1.1', "*

 * *                   "'@jupyterlite/server-extension': '^0.1.1', '@jupyterlite/types': '^0.1.1', "*

 * *                   "'@jupyterlite/ui-components': '^0.1.1'}",*

 * * "'resolutions'": "{'@jupyterlite/application-extension': '~0.1.1', '@jupyterlite/content […]*

```diff
@@ -35,22 +35,22 @@
         "@jupyterlab/theme-dark-extension": "~3.5.3",
         "@jupyterlab/theme-light-extension": "~3.5.3",
         "@jupyterlab/toc-extension": "~5.5.3",
         "@jupyterlab/tooltip-extension": "~3.5.3",
         "@jupyterlab/translation-extension": "~3.5.3",
         "@jupyterlab/ui-components-extension": "~3.5.3",
         "@jupyterlab/vega5-extension": "~3.5.3",
-        "@jupyterlite/application-extension": "^0.1.0",
-        "@jupyterlite/iframe-extension": "^0.1.0",
-        "@jupyterlite/licenses": "^0.1.0",
-        "@jupyterlite/localforage": "^0.1.0",
-        "@jupyterlite/server": "^0.1.0",
-        "@jupyterlite/server-extension": "^0.1.0",
-        "@jupyterlite/types": "^0.1.0",
-        "@jupyterlite/ui-components": "^0.1.0",
+        "@jupyterlite/application-extension": "^0.1.1",
+        "@jupyterlite/iframe-extension": "^0.1.1",
+        "@jupyterlite/licenses": "^0.1.1",
+        "@jupyterlite/localforage": "^0.1.1",
+        "@jupyterlite/server": "^0.1.1",
+        "@jupyterlite/server-extension": "^0.1.1",
+        "@jupyterlite/types": "^0.1.1",
+        "@jupyterlite/ui-components": "^0.1.1",
         "es6-promise": "~4.2.8",
         "react": "^17.0.1",
         "react-dom": "^17.0.1",
         "yjs": "^13.5.6"
     },
     "jupyterlab": {
         "extensions": [
@@ -230,24 +230,24 @@
         "@jupyterlab/tooltip": "~3.5.3",
         "@jupyterlab/tooltip-extension": "~3.5.3",
         "@jupyterlab/translation": "~3.5.3",
         "@jupyterlab/translation-extension": "~3.5.3",
         "@jupyterlab/ui-components": "~3.5.3",
         "@jupyterlab/ui-components-extension": "~3.5.3",
         "@jupyterlab/vega5-extension": "~3.5.3",
-        "@jupyterlite/application-extension": "~0.1.0",
-        "@jupyterlite/contents": "~0.1.0",
-        "@jupyterlite/iframe-extension": "~0.1.0",
-        "@jupyterlite/kernel": "~0.1.0",
-        "@jupyterlite/licenses": "~0.1.0",
-        "@jupyterlite/localforage": "~0.1.0",
-        "@jupyterlite/server": "~0.1.0",
-        "@jupyterlite/server-extension": "~0.1.0",
-        "@jupyterlite/types": "~0.1.0",
-        "@jupyterlite/ui-components": "~0.1.0",
+        "@jupyterlite/application-extension": "~0.1.1",
+        "@jupyterlite/contents": "~0.1.1",
+        "@jupyterlite/iframe-extension": "~0.1.1",
+        "@jupyterlite/kernel": "~0.1.1",
+        "@jupyterlite/licenses": "~0.1.1",
+        "@jupyterlite/localforage": "~0.1.1",
+        "@jupyterlite/server": "~0.1.1",
+        "@jupyterlite/server-extension": "~0.1.1",
+        "@jupyterlite/types": "~0.1.1",
+        "@jupyterlite/ui-components": "~0.1.1",
         "@lumino/algorithm": "~1.9.2",
         "@lumino/application": "~1.31.3",
         "@lumino/commands": "~1.21.1",
         "@lumino/coreutils": "~1.12.1",
         "@lumino/disposable": "~1.10.4",
         "@lumino/domutils": "~1.8.2",
         "@lumino/dragdrop": "~1.14.4",
@@ -257,9 +257,9 @@
         "@lumino/virtualdom": "~1.14.3",
         "@lumino/widgets": "~1.37.1",
         "es6-promise": "^4.2.8",
         "react": "^17.0.2",
         "react-dom": "^17.0.2",
         "yjs": "^13.5.43"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/manifest.webmanifest` & `resotocore-3.6.5/resotocore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/package.json` & `resotocore-3.6.5/resotocore/jupyterlite/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -42,9 +42,9 @@
     },
     "scripts": {
         "build": "webpack",
         "build:prod": "yarn clean && yarn build --mode=production",
         "clean": "rimraf build **/build",
         "watch": "webpack --config webpack.config.watch.js"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `resotocore-3.6.4/resotocore/jupyterlite/service-worker-b2fb40a.js` & `resotocore-3.6.5/resotocore/jupyterlite/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/message_bus.py` & `resotocore-3.6.5/resotocore/message_bus.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/metrics.py` & `resotocore-3.6.5/resotocore/metrics.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/adjust_node.py` & `resotocore-3.6.5/resotocore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/db_updater.py` & `resotocore-3.6.5/resotocore/model/db_updater.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/graph_access.py` & `resotocore-3.6.5/resotocore/model/graph_access.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/json_schema.py` & `resotocore-3.6.5/resotocore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/model.py` & `resotocore-3.6.5/resotocore/model/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/model_handler.py` & `resotocore-3.6.5/resotocore/model/model_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/resolve_in_graph.py` & `resotocore-3.6.5/resotocore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/transform_kind_convert.py` & `resotocore-3.6.5/resotocore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/model/typed_model.py` & `resotocore-3.6.5/resotocore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/query/__init__.py` & `resotocore-3.6.5/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/query/model.py` & `resotocore-3.6.5/resotocore/query/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/query/query_parser.py` & `resotocore-3.6.5/resotocore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/query/template_expander.py` & `resotocore-3.6.5/resotocore/query/template_expander.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/query/template_expander_service.py` & `resotocore-3.6.5/resotocore/query/template_expander_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/report/__init__.py` & `resotocore-3.6.5/resotocore/report/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/report/benchmark_renderer.py` & `resotocore-3.6.5/resotocore/report/benchmark_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/report/inspector_service.py` & `resotocore-3.6.5/resotocore/report/inspector_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/report/report_config.py` & `resotocore-3.6.5/resotocore/report/report_config.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/api-doc.yaml` & `resotocore-3.6.5/resotocore/static/api-doc.yaml`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/ck-unicode-truecolor.ans` & `resotocore-3.6.5/resotocore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/benchmark/aws/aws_cis_1_5.json` & `resotocore-3.6.5/resotocore/static/report/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/check_template.json` & `resotocore-3.6.5/resotocore/static/report/check_template.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_apigateway.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_cloudtrail.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_config.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_ec2.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_efs.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_iam.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_kms.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_lambda.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_rds.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/report/checks/aws/aws_s3.json` & `resotocore-3.6.5/resotocore/static/report/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/static/resoto_logo_and_text.svg` & `resotocore-3.6.5/resotocore/static/resoto_logo_and_text.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/system_start.py` & `resotocore-3.6.5/resotocore/system_start.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/task/__init__.py` & `resotocore-3.6.5/resotocore/task/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/task/model.py` & `resotocore-3.6.5/resotocore/task/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/task/scheduler.py` & `resotocore-3.6.5/resotocore/task/scheduler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/task/start_workflow_on_first_subscriber.py` & `resotocore-3.6.5/resotocore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/task/subscribers.py` & `resotocore-3.6.5/resotocore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/task/task_description.py` & `resotocore-3.6.5/resotocore/task/task_description.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/task/task_handler.py` & `resotocore-3.6.5/resotocore/task/task_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/templates/base.html` & `resotocore-3.6.5/resotocore/templates/base.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/templates/create_first_user.html` & `resotocore-3.6.5/resotocore/templates/create_first_user.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/templates/login.html` & `resotocore-3.6.5/resotocore/templates/login.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/types.py` & `resotocore-3.6.5/resotocore/types.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/user/__init__.py` & `resotocore-3.6.5/resotocore/user/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,19 @@
 from resotocore.service import Service
 from resotolib.core.model_export import dataclasses_to_resotocore_model
 
 UsersConfigRoot = "resoto_users"
 UsersConfigId = ConfigId("resoto.users")
 
 
-ValidRoles = {"admin", "readwrite", "readonly"}
-
-
 @define
 class ResotoUser:
     kind: ClassVar[str] = "resoto_user"
     fullname: str = field(metadata={"description": "The full name of the user."})
-    password_hash: str = field(metadata={"description": "The sha256 hash of the user's password."})
+    password_hash: str = field(metadata={"description": "The hash of the user's password."})
     roles: Set[str] = field(factory=set, metadata={"description": "The roles of the user."})
 
 
 @define
 class ResotoUsersConfig:
     kind: ClassVar[str] = UsersConfigRoot
     users: Dict[str, ResotoUser] = field(factory=lambda: {}, metadata={"description": "A map of email to user data."})
```

### Comparing `resotocore-3.6.4/resotocore/user/user_management.py` & `resotocore-3.6.5/resotocore/user/user_management.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/util.py` & `resotocore-3.6.5/resotocore/util.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/validator.py` & `resotocore-3.6.5/resotocore/validator.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/web/api.py` & `resotocore-3.6.5/resotocore/web/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,27 +69,28 @@
     InfraAppAlias,
     FilePath,
 )
 from resotocore.config import ConfigValidation, ConfigEntity
 from resotocore.console_renderer import ConsoleColorSystem, ConsoleRenderer
 from resotocore.db.graphdb import GraphDB, HistoryChange
 from resotocore.db.model import QueryModel
-from resotocore.error import NotFoundError
+from resotocore.error import NotFoundError, NotEnoughPermissions
 from resotocore.ids import TaskId, ConfigId, NodeId, SubscriberId, WorkerId, GraphName, Email, Password
 from resotocore.message_bus import Message, ActionDone, Action, ActionError, ActionInfo, ActionProgress
 from resotocore.metrics import timed
 from resotocore.model.graph_access import Section
 from resotocore.model.json_schema import json_schema
 from resotocore.model.model import Kind, Model
 from resotocore.model.typed_model import to_json, from_js, to_js_str, to_js
 from resotocore.service import Service
 from resotocore.task.model import Subscription
 from resotocore.types import Json, JsonElement
+from resotocore.user.model import Permission, AuthorizedUser
 from resotocore.util import uuid_str, force_gen, rnd_str, if_set, duration, utc_str, parse_utc, async_noop, utc
-from resotocore.web.auth import raw_jwt_from_auth_message, AuthorizedUser, AuthHandler
+from resotocore.web.auth import raw_jwt_from_auth_message, LoginWithCode, AuthHandler
 from resotocore.web.content_renderer import result_binary_gen, single_result
 from resotocore.web.directives import (
     metrics_handler,
     error_handler,
     on_response_prepare,
     cors_handler,
     enable_compression,
@@ -174,101 +175,107 @@
         return self._session
 
     def __add_routes(self, prefix: str) -> None:
         static_path = os.path.abspath(os.path.dirname(__file__) + "/../static")
         jupyterlite_path = Path(os.path.abspath(os.path.dirname(__file__) + "/../jupyterlite"))
         if not jupyterlite_path.exists():
             jupyterlite_path.mkdir(parents=True, exist_ok=True)
+        require = self.auth_handler.allow_with
+        r = Permission.read
+        a = Permission.admin
+
         self.app.add_routes(
             [
                 # Model operations (backwards compatible)
-                web.get(prefix + "/model", self.get_model),
-                web.patch(prefix + "/model", self.update_model),
-                web.get(prefix + "/model/uml", self.model_uml),
+                web.get(prefix + "/model", require(self.get_model, r)),
+                web.patch(prefix + "/model", require(self.update_model, a)),
+                web.get(prefix + "/model/uml", require(self.model_uml, r)),
                 # Graph based model operations
-                web.get(prefix + "/graph/{graph_id}/model", self.get_model),
-                web.patch(prefix + "/graph/{graph_id}/model", self.update_model),
-                web.get(prefix + "/graph/{graph_id}/model/uml", self.model_uml),
+                web.get(prefix + "/graph/{graph_id}/model", require(self.get_model, r)),
+                web.patch(prefix + "/graph/{graph_id}/model", require(self.update_model, a)),
+                web.get(prefix + "/graph/{graph_id}/model/uml", require(self.model_uml, r)),
                 # CRUD Graph operations
-                web.get(prefix + "/graph", self.list_graphs),
-                web.get(prefix + "/graph/{graph_id}", self.get_node),
-                web.post(prefix + "/graph/{graph_id}", self.create_graph),
-                web.delete(prefix + "/graph/{graph_id}", self.wipe),
+                web.get(prefix + "/graph", require(self.list_graphs, r)),
+                web.get(prefix + "/graph/{graph_id}", require(self.get_node, r)),
+                web.post(prefix + "/graph/{graph_id}", require(self.create_graph, a)),
+                web.delete(prefix + "/graph/{graph_id}", require(self.wipe, a)),
                 # search the graph
-                web.post(prefix + "/graph/{graph_id}/search/raw", self.raw),
-                web.post(prefix + "/graph/{graph_id}/search/structure", self.query_structure),
-                web.post(prefix + "/graph/{graph_id}/search/explain", self.explain),
-                web.post(prefix + "/graph/{graph_id}/search/list", self.query_list),
-                web.post(prefix + "/graph/{graph_id}/search/graph", self.query_graph_stream),
-                web.post(prefix + "/graph/{graph_id}/search/aggregate", self.query_aggregation),
-                web.post(prefix + "/graph/{graph_id}/search/history/list", self.query_history),
-                web.post(prefix + "/graph/{graph_id}/search/history/aggregate", self.query_history),
+                web.post(prefix + "/graph/{graph_id}/search/raw", require(self.raw, r)),
+                web.post(prefix + "/graph/{graph_id}/search/structure", require(self.query_structure, r)),
+                web.post(prefix + "/graph/{graph_id}/search/explain", require(self.explain, r)),
+                web.post(prefix + "/graph/{graph_id}/search/list", require(self.query_list, r)),
+                web.post(prefix + "/graph/{graph_id}/search/graph", require(self.query_graph_stream, r)),
+                web.post(prefix + "/graph/{graph_id}/search/aggregate", require(self.query_aggregation, r)),
+                web.post(prefix + "/graph/{graph_id}/search/history/list", require(self.query_history, r)),
+                web.post(prefix + "/graph/{graph_id}/search/history/aggregate", require(self.query_history, r)),
                 # maintain the graph
-                web.patch(prefix + "/graph/{graph_id}/nodes", self.update_nodes),
-                web.post(prefix + "/graph/{graph_id}/merge", self.merge_graph),
-                web.post(prefix + "/graph/{graph_id}/batch/merge", self.update_merge_graph_batch),
-                web.get(prefix + "/graph/{graph_id}/batch", self.list_batches),
-                web.post(prefix + "/graph/{graph_id}/batch/{batch_id}", self.commit_batch),
-                web.delete(prefix + "/graph/{graph_id}/batch/{batch_id}", self.abort_batch),
+                web.patch(prefix + "/graph/{graph_id}/nodes", require(self.update_nodes, a)),
+                web.post(prefix + "/graph/{graph_id}/merge", require(self.merge_graph, a)),
+                web.post(prefix + "/graph/{graph_id}/batch/merge", require(self.update_merge_graph_batch, a)),
+                web.get(prefix + "/graph/{graph_id}/batch", require(self.list_batches, a)),
+                web.post(prefix + "/graph/{graph_id}/batch/{batch_id}", require(self.commit_batch, a)),
+                web.delete(prefix + "/graph/{graph_id}/batch/{batch_id}", require(self.abort_batch, a)),
                 # node specific actions
-                web.post(prefix + "/graph/{graph_id}/node/{node_id}/under/{parent_node_id}", self.create_node),
-                web.get(prefix + "/graph/{graph_id}/node/{node_id}", self.get_node),
-                web.patch(prefix + "/graph/{graph_id}/node/{node_id}", self.update_node),
-                web.delete(prefix + "/graph/{graph_id}/node/{node_id}", self.delete_node),
-                web.patch(prefix + "/graph/{graph_id}/node/{node_id}/section/{section}", self.update_node),
+                web.post(
+                    prefix + "/graph/{graph_id}/node/{node_id}/under/{parent_node_id}", require(self.create_node, a)
+                ),
+                web.get(prefix + "/graph/{graph_id}/node/{node_id}", require(self.get_node, r)),
+                web.patch(prefix + "/graph/{graph_id}/node/{node_id}", require(self.update_node, a)),
+                web.delete(prefix + "/graph/{graph_id}/node/{node_id}", require(self.delete_node, a)),
+                web.patch(prefix + "/graph/{graph_id}/node/{node_id}/section/{section}", require(self.update_node, a)),
                 # Subscriptions
-                web.get(prefix + "/subscribers", self.list_all_subscriptions),
-                web.get(prefix + "/subscribers/for/{event_type}", self.list_subscription_for_event),
+                web.get(prefix + "/subscribers", require(self.list_all_subscriptions, a)),
+                web.get(prefix + "/subscribers/for/{event_type}", require(self.list_subscription_for_event, a)),
                 # Subscription
-                web.get(prefix + "/subscriber/{subscriber_id}", self.get_subscriber),
-                web.put(prefix + "/subscriber/{subscriber_id}", self.update_subscriber),
-                web.delete(prefix + "/subscriber/{subscriber_id}", self.delete_subscriber),
-                web.post(prefix + "/subscriber/{subscriber_id}/{event_type}", self.add_subscription),
-                web.delete(prefix + "/subscriber/{subscriber_id}/{event_type}", self.delete_subscription),
-                web.get(prefix + "/subscriber/{subscriber_id}/handle", self.handle_subscribed),
+                web.get(prefix + "/subscriber/{subscriber_id}", require(self.get_subscriber, a)),
+                web.put(prefix + "/subscriber/{subscriber_id}", require(self.update_subscriber, a)),
+                web.delete(prefix + "/subscriber/{subscriber_id}", require(self.delete_subscriber, a)),
+                web.post(prefix + "/subscriber/{subscriber_id}/{event_type}", require(self.add_subscription, a)),
+                web.delete(prefix + "/subscriber/{subscriber_id}/{event_type}", require(self.delete_subscription, a)),
+                web.get(prefix + "/subscriber/{subscriber_id}/handle", require(self.handle_subscribed, a)),
                 # report checks
-                web.get(prefix + "/report/checks", self.inspection_checks),
-                web.get(prefix + "/report/checks/graph/{graph_id}", self.perform_benchmark_on_checks),
-                web.get(prefix + "/report/check/{check_id}/graph/{graph_id}", self.inspection_results),
-                web.get(prefix + "/report/benchmark/{benchmark}/graph/{graph_id}", self.perform_benchmark),
+                web.get(prefix + "/report/checks", require(self.inspection_checks, r)),
+                web.get(prefix + "/report/checks/graph/{graph_id}", require(self.perform_benchmark_on_checks, r)),
+                web.get(prefix + "/report/check/{check_id}/graph/{graph_id}", require(self.inspection_results, r)),
+                web.get(prefix + "/report/benchmark/{benchmark}/graph/{graph_id}", require(self.perform_benchmark, r)),
                 # CLI
-                web.post(prefix + "/cli/evaluate", self.evaluate),
-                web.post(prefix + "/cli/execute", self.execute),
-                web.get(prefix + "/cli/info", self.cli_info),
+                web.post(prefix + "/cli/evaluate", require(self.evaluate, r)),
+                web.post(prefix + "/cli/execute", require(self.execute, r)),
+                web.get(prefix + "/cli/info", require(self.cli_info, r)),
                 # Event operations
-                web.get(prefix + "/events", self.handle_events),
+                web.get(prefix + "/events", require(self.handle_events, a)),
                 web.post(prefix + "/analytics", self.send_analytics_events),
                 # Worker operations
-                web.get(prefix + "/work/queue", self.handle_work_tasks),
-                web.get(prefix + "/work/list", self.list_work),
+                web.get(prefix + "/work/queue", require(self.handle_work_tasks, a)),
+                web.get(prefix + "/work/list", require(self.list_work, a)),
                 # Serve static filed
                 web.get(prefix, self.forward("/ui/index.html")),
                 web.static(prefix + "/static", static_path),
                 web.get(prefix + "/notebook", self.forward("/notebook/index.html")),
                 web.static(prefix + "/notebook", jupyterlite_path),
                 # metrics
                 web.get(prefix + "/metrics", self.metrics),
                 # config operations
-                web.get(prefix + "/configs", self.list_configs),
-                web.patch(prefix + "/config/{config_id:[^{}]+}", self.patch_config),
-                web.delete(prefix + "/config/{config_id:[^{}]+}", self.delete_config),
+                web.get(prefix + "/configs", require(self.list_configs, r)),
+                web.patch(prefix + "/config/{config_id:[^{}]+}", require(self.patch_config, a)),
+                web.delete(prefix + "/config/{config_id:[^{}]+}", require(self.delete_config, a)),
                 # config model operations
-                web.get(prefix + "/configs/validation", self.list_config_models),
-                web.get(prefix + "/configs/model", self.get_configs_model),
-                web.patch(prefix + "/configs/model", self.update_configs_model),
-                web.put(prefix + "/config_validation/{config_id:[^{}]+}", self.put_config_validation),
-                web.get(prefix + "/config_validation/{config_id:[^{}]+}", self.get_config_validation),
-                web.put(prefix + "/config/{config_id:[^{}]+}/validation", self.put_config_validation),
-                web.get(prefix + "/config/{config_id:[^{}]+}/validation", self.get_config_validation),
+                web.get(prefix + "/configs/validation", require(self.list_config_models, r)),
+                web.get(prefix + "/configs/model", require(self.get_configs_model, r)),
+                web.patch(prefix + "/configs/model", require(self.update_configs_model, a)),
+                web.put(prefix + "/config_validation/{config_id:[^{}]+}", require(self.put_config_validation, a)),
+                web.get(prefix + "/config_validation/{config_id:[^{}]+}", require(self.get_config_validation, a)),
+                web.put(prefix + "/config/{config_id:[^{}]+}/validation", require(self.put_config_validation, a)),
+                web.get(prefix + "/config/{config_id:[^{}]+}/validation", require(self.get_config_validation, a)),
                 # config operations, moved here to avoid early matching
-                web.put(prefix + "/config/{config_id:[^{}]+}", self.put_config),
-                web.get(prefix + "/config/{config_id:[^{}]+}", self.get_config),
+                web.put(prefix + "/config/{config_id:[^{}]+}", require(self.put_config, a)),
+                web.get(prefix + "/config/{config_id:[^{}]+}", require(self.get_config, a)),
                 # ca operations
                 web.get(prefix + "/ca/cert", self.certificate),
-                web.post(prefix + "/ca/sign", self.sign_certificate),
+                web.post(prefix + "/ca/sign", require(self.sign_certificate, a)),
                 # system operations
                 web.get(prefix + "/system/ping", self.ping),
                 web.get(prefix + "/system/ready", self.ready),
                 # forwards
                 web.get(prefix + "/tsdb", self.forward("/tsdb/")),
                 web.get(prefix + "/ui", self.forward("/ui/index.html")),
                 web.get(prefix + "/ui/", self.forward("/ui/index.html")),
@@ -366,15 +373,15 @@
         post_data = await request.post()
         email = Email(str(post_data.get("email", "")))
         password = Password(str(post_data.get("password", "")))
         redirect = str(post_data.get("redirect", ""))
         if email and password and (user := await self.deps.user_management.login(email, password)):
             params: Dict[str, List[str]] = {}
             if self.deps.config.args.psk:
-                code = await self.auth_handler.add_authorized_user(AuthorizedUser(email, user.roles, utc()))
+                code = await self.auth_handler.add_login_with_code(LoginWithCode(email, user.roles, utc()))
                 params["code"] = [code]
             if redirect:
                 if params:
                     parsed = urlparse(redirect)
                     query_params = parse_qs(parsed.query)
                     query_params.update(params)
                     parsed = parsed._replace(query=urlencode(query_params, doseq=True))
@@ -393,15 +400,15 @@
             return web.json_response(jwt)
         else:
             return web.HTTPNoContent()
 
     async def renew_authorization(self, request: Request) -> StreamResponse:
         if jwt_raw := request.get("jwt"):
             exp = datetime.fromtimestamp(int(jwt_raw["exp"]), tz=timezone.utc)
-            user = AuthorizedUser(jwt_raw["email"], set(jwt_raw["roles"].split(",")), exp)
+            user = LoginWithCode(jwt_raw["email"], set(jwt_raw["roles"].split(",")), exp)
             renewed, data = self.auth_handler.user_jwt(user)
             return web.json_response(data, headers={"Authorization": f"Bearer {renewed}"})
         else:
             return HTTPNoContent()  # no psk, no renewal
 
     async def list_configs(self, request: Request) -> StreamResponse:
         return await self.stream_response_from_gen(request, self.deps.config_handler.list_config_ids())
@@ -1078,15 +1085,16 @@
     def cli_context_from_request(request: Request) -> CLIContext:
         try:
             columns = int(request.headers.get("Resoto-Shell-Columns", "120"))
             rows = int(request.headers.get("Resoto-Shell-Rows", "50"))
             terminal = request.headers.get("Resoto-Shell-Terminal", "false") == "true"
             colors = ConsoleColorSystem.from_name(request.headers.get("Resoto-Shell-Color-System", "monochrome"))
             renderer = ConsoleRenderer(width=columns, height=rows, color_system=colors, terminal=terminal)
-            return CLIContext(env=dict(request.query), console_renderer=renderer, source="api")
+            user = request.get("user", None)
+            return CLIContext(env=dict(request.query), console_renderer=renderer, source="api", user=user)
         except Exception as ex:
             log.debug("Could not create CLI context.", exc_info=ex)
             return CLIContext(
                 env=dict(request.query), console_renderer=ConsoleRenderer.default_renderer(), source="api"
             )
 
     async def evaluate(self, request: Request) -> StreamResponse:
@@ -1133,24 +1141,26 @@
         finally:
             if temp_dir:
                 shutil.rmtree(temp_dir)
 
     async def execute_parsed(
         self, request: Request, command: str, parsed: List[ParsedCommandLine], ctx: CLIContext
     ) -> StreamResponse:
-        # make sure, all requirements are fulfilled
-        not_met_requirements = [not_met for line in parsed for not_met in line.unmet_requirements]
         # what is the accepted content type
         # only required for multipart requests
         boundary = "cli-part"
         mp_response = web.StreamResponse(
             status=200, reason="OK", headers={"Content-Type": f"multipart/mixed;boundary={boundary}"}
         )
 
-        if not_met_requirements:
+        if self.auth_handler.psk is not None and not all(line.is_allowed_to_execute() for line in parsed):
+            user: Optional[AuthorizedUser] = request.get("user", None)
+            required = {d for line in parsed for c in line.executable_commands for d in c.action.required_permissions}
+            raise NotEnoughPermissions(user.permissions if user else set(), required)
+        elif [not_met for line in parsed for not_met in line.unmet_requirements]:
             requirements = [req for line in parsed for cmd in line.executable_commands for req in cmd.action.required]
             data = {"command": command, "env": dict(request.query), "required": to_json(requirements)}
             return web.json_response(data, status=424)
         elif len(parsed) == 1:
             first_result = parsed[0]
             count, generator = await first_result.execute()
             # flat the results from 0 or 1
```

### Comparing `resotocore-3.6.4/resotocore/web/auth.py` & `resotocore-3.6.5/resotocore/web/auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,44 +15,47 @@
 from attr import define
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey, RSAPrivateKey
 from cryptography.x509 import Certificate
 from jwt import PyJWTError
 
 from resotocore.core_config import CoreConfig
 from resotocore.db.system_data_db import SystemDataDb
+from resotocore.error import NotEnoughPermissions
+from resotocore.service import Service
+from resotocore.user.model import AuthorizedUser, Permission
 from resotocore.util import uuid_str
 from resotocore.web.certificate_handler import CertificateHandler
 from resotolib import jwt as ck_jwt
 from resotolib.asynchronous.web import RequestHandler, Middleware
 from resotolib.jwt import encode_jwt, create_jwk_dict
 from resotolib.types import Json
 from resotolib.utils import utc
 from resotolib.x509 import gen_rsa_key, gen_csr, key_to_bytes, cert_to_bytes, load_key_from_bytes, load_cert_from_bytes
 
 log = logging.getLogger(__name__)
 JWT = Dict[str, Any]
-_JWT_Context: ContextVar[JWT] = ContextVar("JWT", default={})
+_AuthorizedUserContext: ContextVar[Optional[AuthorizedUser]] = ContextVar("JWT", default=None)
 CodeLifeTime = timedelta(minutes=5)
 
 
 @define
-class AuthorizedUser:
+class LoginWithCode:
     email: str
     roles: Set[str]
     authorized_at: datetime
 
     def is_valid(self) -> bool:
         return utc() - self.authorized_at < CodeLifeTime
 
 
-async def jwt_from_context() -> JWT:
+async def authorized_user_from_context() -> Optional[AuthorizedUser]:
     """
-    Inside a request handler, this value retrieves the current jwt.
+    Inside a request handler, this value retrieves the current authorized user.
     """
-    return _JWT_Context.get()
+    return _AuthorizedUserContext.get()
 
 
 def raw_jwt_from_auth_message(msg: str) -> Optional[str]:
     """
     Expected message: json object with type kind="authorization" and a jwt field
     { "kind": "authorization", "jwt": "Bearer <jwt>" }
     """
@@ -67,30 +70,30 @@
 @middleware
 async def no_check(request: Request, handler: RequestHandler) -> StreamResponse:
     # all requests are authorized automatically
     request["authorized"] = True
     return await handler(request)
 
 
-class AuthHandler:
+class AuthHandler(Service):
     def __init__(
         self,
         system_db: SystemDataDb,
         config: CoreConfig,
         cert_handler: CertificateHandler,
         always_allowed_paths: Set[str],
         not_allowed: Optional[Callable[[Request], Awaitable[StreamResponse]]] = None,
     ) -> None:
         self.system_db = system_db
         self.config = config
         self.psk = config.args.psk
         self.cert_handler = cert_handler
         self.always_allowed_paths = always_allowed_paths
         self.not_allowed = not_allowed
-        self.authorization_codes: Dict[str, AuthorizedUser] = {}
+        self.authorization_codes: Dict[str, LoginWithCode] = {}
         self.signing_key_private: Optional[RSAPrivateKey] = None  # set on start
         self.signing_key_certificate: Optional[Certificate] = None  # set on start
         self.signing_key_jwk: Optional[Json] = None  # set on start
 
     async def start(self) -> None:
         keys = await self.system_db.jwt_signing_keys()
         # check if the signing key is already in the database
@@ -127,30 +130,32 @@
         def set_valid_jwt(psk_or_cert: Union[str, Certificate, RSAPublicKey]) -> Optional[JWT]:
             try:
                 # note: the expiration is already checked by this function
                 jwt_token = ck_jwt.decode_jwt_from_header_value(auth_header, psk_or_cert)
             except PyJWTError:
                 return None
             if jwt_token:
+                user = AuthorizedUser.from_jwt(jwt_token)
+                _AuthorizedUserContext.set(user)
                 request["authorized"] = True  # deferred check in websocket handler
                 request["jwt"] = jwt_token
-                _JWT_Context.set(jwt_token)
+                request["user"] = user
             return jwt_token
 
         assert self.signing_key_certificate is not None, "AuthHandler not started"
         # based on the jwt, we either use the PSK or the public key
         _, token = auth_header.split(" ", maxsplit=1)
         jwt_header = jwt.get_unverified_header(token)
         # in case of RS256, the public key is used to verify the signature
         secret = self.signing_key_certificate if jwt_header.get("alg") == "RS256" else self.psk
         authorized = set_valid_jwt(secret) is not None
         return authorized
 
     async def validate_code(self, code: str, request: Request) -> bool:
-        if (user := await self.authorized_user(code)) and user.is_valid():
+        if (user := await self.login_with_code(code)) and user.is_valid():
             jwt_token, data = self.user_jwt(user)
             # this will be picked up in on_response_prepare and sent as a header
             request["send_auth_response_header"] = f"Bearer {jwt_token}"
             # set encoded data the same way as if it was a jwt
             request["jwt"] = data
             request["authorized"] = True
             return True
@@ -180,32 +185,57 @@
             if auth_head := (request.headers.get("Authorization") or request.cookies.get("resoto_authorization")):
                 allowed = await self.validate_jwt(auth_head, request)
             elif code := request.query.get("code"):
                 allowed = await self.validate_code(code, request)
             elif always_allowed(request):
                 allowed = True
             if allowed:
-                return await handler(request)
+                result = await handler(request)
+                _AuthorizedUserContext.set(None)  # unset the context
+                return result
             else:
                 if self.not_allowed:
                     return await self.not_allowed(request)
                 else:
                     raise web.HTTPUnauthorized()
 
         return valid_auth_handler
 
-    async def authorized_user(self, code: str) -> Optional[AuthorizedUser]:
+    async def requires_permission(self, request: Request, *permission: Union[Permission, Set[Permission]]) -> None:
+        if self.psk:  # only require permissions if authentication is enabled
+            required_permissions = set()
+            for p in permission:
+                if isinstance(p, Permission):
+                    required_permissions.add(p)
+                elif isinstance(p, set):
+                    required_permissions.update(p)
+                else:
+                    raise ValueError(f"Invalid permission {p}")
+            if current_user := request.get("user"):
+                if not current_user.has_permission(required_permissions):
+                    raise NotEnoughPermissions(current_user.permissions, required_permissions)
+            else:
+                raise web.HTTPUnauthorized()
+
+    def allow_with(self, handler: RequestHandler, *permission: Union[Permission, Set[Permission]]) -> RequestHandler:
+        async def wrapper(request: Request) -> StreamResponse:
+            await self.requires_permission(request, *permission)
+            return await handler(request)
+
+        return wrapper
+
+    async def login_with_code(self, code: str) -> Optional[LoginWithCode]:
         for invalid_code in [k for k, v in self.authorization_codes.items() if not v.is_valid()]:
             self.authorization_codes.pop(invalid_code, None)
         return self.authorization_codes.get(code)
 
-    async def add_authorized_user(self, user: AuthorizedUser) -> str:
+    async def add_login_with_code(self, user: LoginWithCode) -> str:
         code = str(uuid_str())
         self.authorization_codes[code] = user
         return code
 
-    def user_jwt(self, user: AuthorizedUser) -> Tuple[str, Json]:
+    def user_jwt(self, user: LoginWithCode) -> Tuple[str, Json]:
         assert self.signing_key_private is not None, "AuthHandler not started"
         assert self.signing_key_certificate is not None, "AuthHandler not started"
         exp = int(time.time() + self.config.api.access_token_expiration_seconds)
         data = {"email": user.email, "roles": ",".join(user.roles), "exp": exp}
         return encode_jwt(data, self.signing_key_private, cert=self.signing_key_certificate), data
```

### Comparing `resotocore-3.6.4/resotocore/web/certificate_handler.py` & `resotocore-3.6.5/resotocore/web/certificate_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/web/content_renderer.py` & `resotocore-3.6.5/resotocore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/web/directives.py` & `resotocore-3.6.5/resotocore/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/web/tsdb.py` & `resotocore-3.6.5/resotocore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore/worker_task_queue.py` & `resotocore-3.6.5/resotocore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/resotocore.egg-info/PKG-INFO` & `resotocore-3.6.5/resotocore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.6.4
+Version: 3.6.5
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.6.4/resotocore.egg-info/SOURCES.txt` & `resotocore-3.6.5/resotocore.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 resotocore/jupyterlite/build/1278.0524a4a.js
 resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
 resotocore/jupyterlite/build/1290.3981211.js
 resotocore/jupyterlite/build/1295.46e72b8.js
 resotocore/jupyterlite/build/1310.23bbe67.js
 resotocore/jupyterlite/build/1320.21effe3.js
 resotocore/jupyterlite/build/1325.f76267c.js
-resotocore/jupyterlite/build/1408.7461890.js
+resotocore/jupyterlite/build/1408.e049d91.js
 resotocore/jupyterlite/build/1440.a9e7ea1.js
 resotocore/jupyterlite/build/1483.616d9ab.js
 resotocore/jupyterlite/build/1489.e50b6d4.js
 resotocore/jupyterlite/build/1507.5705605.js
 resotocore/jupyterlite/build/152.525d460.js
 resotocore/jupyterlite/build/1520.4e2eb21.js
 resotocore/jupyterlite/build/1555.e188f3f.js
@@ -137,37 +137,37 @@
 resotocore/jupyterlite/build/2358.d5cf7c8.js
 resotocore/jupyterlite/build/2359.6451c3e.js
 resotocore/jupyterlite/build/237.f765e77.js
 resotocore/jupyterlite/build/2384.71782be.js
 resotocore/jupyterlite/build/240.cddc46b.js
 resotocore/jupyterlite/build/2431.648d237.js
 resotocore/jupyterlite/build/2546.1f48267.js
-resotocore/jupyterlite/build/2557.75e9da2.js
+resotocore/jupyterlite/build/2557.6c85d56.js
 resotocore/jupyterlite/build/261.5f53c0e.js
 resotocore/jupyterlite/build/2629.c0e1cd6.js
 resotocore/jupyterlite/build/2788.46acc8a.js
 resotocore/jupyterlite/build/2834.942acc6.js
 resotocore/jupyterlite/build/2887.47ba752.js
 resotocore/jupyterlite/build/2956.8880209.js
 resotocore/jupyterlite/build/2973.2a51dc4.js
 resotocore/jupyterlite/build/3004.255e79c.js
-resotocore/jupyterlite/build/302.8bcc38f.js
+resotocore/jupyterlite/build/302.fad99ac.js
 resotocore/jupyterlite/build/3037.70ee38d.js
 resotocore/jupyterlite/build/3042.7cfad84.js
 resotocore/jupyterlite/build/3051.34fac68.js
 resotocore/jupyterlite/build/3122.2289fca.js
 resotocore/jupyterlite/build/3151.10ef4de.js
 resotocore/jupyterlite/build/316.c850a76.js
 resotocore/jupyterlite/build/3196.4e35a17.js
 resotocore/jupyterlite/build/3265.a80440a.js
 resotocore/jupyterlite/build/3277.9c04e75.js
 resotocore/jupyterlite/build/330.126fa98.js
 resotocore/jupyterlite/build/3392.29fe6b9.js
 resotocore/jupyterlite/build/3413.480a49d.js
-resotocore/jupyterlite/build/3444.47d5ea1.js
+resotocore/jupyterlite/build/3444.808a22d.js
 resotocore/jupyterlite/build/3469.7d14d0b.js
 resotocore/jupyterlite/build/3546.fee1bd7.js
 resotocore/jupyterlite/build/362.6716970.js
 resotocore/jupyterlite/build/3708.410d087.js
 resotocore/jupyterlite/build/3752.8735345.js
 resotocore/jupyterlite/build/3850.903abc2.js
 resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
@@ -206,28 +206,28 @@
 resotocore/jupyterlite/build/4749.46ebbb2.js
 resotocore/jupyterlite/build/4750.56c06ab.js
 resotocore/jupyterlite/build/4856.2d7415f.js
 resotocore/jupyterlite/build/4875.375150e.js
 resotocore/jupyterlite/build/489.b981dea.js
 resotocore/jupyterlite/build/490.c2624d4.js
 resotocore/jupyterlite/build/4905.667bf33.js
-resotocore/jupyterlite/build/4931.430433b.js
+resotocore/jupyterlite/build/4931.47d8e25.js
 resotocore/jupyterlite/build/4942.b96c164.js
 resotocore/jupyterlite/build/5016.dd2fe83.js
 resotocore/jupyterlite/build/5072.733a1b5.js
 resotocore/jupyterlite/build/509.6448878.js
 resotocore/jupyterlite/build/5096.8ed0d8e.js
 resotocore/jupyterlite/build/5126.eecad7a.js
 resotocore/jupyterlite/build/5129.1ba4763.js
 resotocore/jupyterlite/build/5153.763d8fa.js
 resotocore/jupyterlite/build/5155.06b4ea9.js
 resotocore/jupyterlite/build/5193.e9f6866.js
 resotocore/jupyterlite/build/5213.3e1a360.js
 resotocore/jupyterlite/build/5227.8c8acd8.js
-resotocore/jupyterlite/build/5238.1751cc3.js
+resotocore/jupyterlite/build/5238.f0f5af0.js
 resotocore/jupyterlite/build/528.2262cb0.js
 resotocore/jupyterlite/build/5292.79d4aba.js
 resotocore/jupyterlite/build/5437.31236f7.js
 resotocore/jupyterlite/build/5489.848a8cf.js
 resotocore/jupyterlite/build/5508.317fca3.js
 resotocore/jupyterlite/build/554.ac98303.js
 resotocore/jupyterlite/build/555.2cd31dd.js
@@ -242,15 +242,15 @@
 resotocore/jupyterlite/build/5880.68f975b.js
 resotocore/jupyterlite/build/5955.88508f7.js
 resotocore/jupyterlite/build/5971.88c5642.js
 resotocore/jupyterlite/build/6080.aa0ff24.js
 resotocore/jupyterlite/build/61.2808a0d.js
 resotocore/jupyterlite/build/6136.b8ba2b2.js
 resotocore/jupyterlite/build/6141.9831d58.js
-resotocore/jupyterlite/build/6475.6037fbb.js
+resotocore/jupyterlite/build/6475.22d38af.js
 resotocore/jupyterlite/build/6493.d796aa5.js
 resotocore/jupyterlite/build/6556.b3d9293.js
 resotocore/jupyterlite/build/6571.2c8884e.js
 resotocore/jupyterlite/build/6576.3ea568e.js
 resotocore/jupyterlite/build/6591.94ed352.js
 resotocore/jupyterlite/build/6612.1632879.js
 resotocore/jupyterlite/build/6623.ae3b3cc.js
@@ -293,25 +293,25 @@
 resotocore/jupyterlite/build/812.9b0e86e.js
 resotocore/jupyterlite/build/816.c8050f2.js
 resotocore/jupyterlite/build/8165.b2c3285.js
 resotocore/jupyterlite/build/8232.a578bf9.js
 resotocore/jupyterlite/build/824.8678196.js
 resotocore/jupyterlite/build/8270.89fe7e1.js
 resotocore/jupyterlite/build/833.9cc6653.js
-resotocore/jupyterlite/build/8370.8f855e5.js
+resotocore/jupyterlite/build/8370.8678c18.js
 resotocore/jupyterlite/build/8373.96b0b3a.js
 resotocore/jupyterlite/build/8389.ffe031f.js
 resotocore/jupyterlite/build/8412.1528057.js
 resotocore/jupyterlite/build/8427.4923f43.js
 resotocore/jupyterlite/build/8542.027afdc.js
 resotocore/jupyterlite/build/8594.0112f03.js
 resotocore/jupyterlite/build/8656.d5b8e92.js
-resotocore/jupyterlite/build/8685.d78bdab.js
+resotocore/jupyterlite/build/8685.13b9daf.js
 resotocore/jupyterlite/build/8698.9817d75.js
-resotocore/jupyterlite/build/8732.9320f73.js
+resotocore/jupyterlite/build/8732.20136c6.js
 resotocore/jupyterlite/build/8741.b138cb8.js
 resotocore/jupyterlite/build/8785.cf4fe95.js
 resotocore/jupyterlite/build/8828.77c71d0.js
 resotocore/jupyterlite/build/8883.80c7b63.js
 resotocore/jupyterlite/build/8976.3816942.js
 resotocore/jupyterlite/build/8981.99a4275.js
 resotocore/jupyterlite/build/8990.2a453cf.js
@@ -325,15 +325,15 @@
 resotocore/jupyterlite/build/9198.9971d70.js
 resotocore/jupyterlite/build/920.d15c177.js
 resotocore/jupyterlite/build/9253.0b31caa.js
 resotocore/jupyterlite/build/9266.bacd0dd.js
 resotocore/jupyterlite/build/9307.c3a00ed.js
 resotocore/jupyterlite/build/9321.869e413.js
 resotocore/jupyterlite/build/9344.ba0abcf.js
-resotocore/jupyterlite/build/9382.9014799.js
+resotocore/jupyterlite/build/9382.144ed35.js
 resotocore/jupyterlite/build/9440.1b10b8f.js
 resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
 resotocore/jupyterlite/build/9464.79e6ac5.js
 resotocore/jupyterlite/build/9502.9a24831.js
 resotocore/jupyterlite/build/9507.1e6cc5d.js
 resotocore/jupyterlite/build/9602.62bf0f1.js
 resotocore/jupyterlite/build/9621.e2e8b5d.js
@@ -349,15 +349,15 @@
 resotocore/jupyterlite/build/9793.6d63a85.js
 resotocore/jupyterlite/build/9806.652c162.js
 resotocore/jupyterlite/build/9865.2e3db6f.js
 resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
 resotocore/jupyterlite/build/989.bcca86a.js
 resotocore/jupyterlite/build/9943.f3f35c7.js
 resotocore/jupyterlite/build/9958.25c8c06.js
-resotocore/jupyterlite/build/9960.64cd61e.js
+resotocore/jupyterlite/build/9960.2d4eeed.js
 resotocore/jupyterlite/build/add-above.svg
 resotocore/jupyterlite/build/add-below.svg
 resotocore/jupyterlite/build/add.svg
 resotocore/jupyterlite/build/bug-dot.svg
 resotocore/jupyterlite/build/bug.svg
 resotocore/jupyterlite/build/build.svg
 resotocore/jupyterlite/build/caret-down-empty-thin.svg
@@ -517,38 +517,38 @@
 resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
 resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
 resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
 resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
 resotocore/jupyterlite/doc/workspaces/index.html
 resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
 resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
-resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
-resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
+resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.29fb1677e9ddfbef42ef.js
+resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.5488d7441d23f13faba2.js
 resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
-resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
+resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.b0a688b88d43b80c014d.js
 resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
-resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
+resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.9eaa8a846d81f5b6c8be.js
 resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
 resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
-resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
-resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
+resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/324.2759063405b36360da9d.js
+resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/324.2759063405b36360da9d.js.LICENSE.txt
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
-resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
+resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.ecdf94afc2748b3fc2e0.js
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
-resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
+resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.703f03086e9738104706.js
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
-resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
-resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
+resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.9-py3-none-any.whl
+resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.9-py3-none-any.whl
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
 resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
 resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
 resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
 resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
@@ -623,14 +623,15 @@
 resotocore/task/task_dependencies.py
 resotocore/task/task_description.py
 resotocore/task/task_handler.py
 resotocore/templates/base.html
 resotocore/templates/create_first_user.html
 resotocore/templates/login.html
 resotocore/user/__init__.py
+resotocore/user/model.py
 resotocore/user/user_management.py
 resotocore/web/__init__.py
 resotocore/web/api.py
 resotocore/web/auth.py
 resotocore/web/certificate_handler.py
 resotocore/web/content_renderer.py
 resotocore/web/directives.py
@@ -701,9 +702,10 @@
 tests/resotocore/task/task_description_test.py
 tests/resotocore/task/task_handler_test.py
 tests/resotocore/user/__init__.py
 tests/resotocore/user/user_management_service_test.py
 tests/resotocore/web/__init__.py
 tests/resotocore/web/api_client.py
 tests/resotocore/web/api_test.py
+tests/resotocore/web/auth_test.py
 tests/resotocore/web/certificate_handler_test.py
 tests/resotocore/web/content_renderer_test.py
```

### Comparing `resotocore-3.6.4/tests/resotocore/__init__.py` & `resotocore-3.6.5/tests/resotocore/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/analytics/posthog_test.py` & `resotocore-3.6.5/tests/resotocore/analytics/posthog_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/analytics/recurrent_events_test.py` & `resotocore-3.6.5/tests/resotocore/analytics/recurrent_events_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/cli/cli_test.py` & `resotocore-3.6.5/tests/resotocore/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/cli/command_test.py` & `resotocore-3.6.5/tests/resotocore/cli/command_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1132,29 +1132,29 @@
         all_results = await cli.execute_cli_command(cmd, stream.list)
         return all_results[0]  # type: ignore
 
     # remove all existing users
     await cli.dependencies.config_handler.delete_config(UsersConfigId)
 
     # create new user
-    result = await execute('user add john@test.de --fullname "John Doe" --password test --role test')
-    assert result == [{"email": "john@test.de", "fullname": "John Doe", "roles": ["test"]}]
+    result = await execute('user add john@test.de --fullname "John Doe" --password test --role readonly')
+    assert result == [{"email": "john@test.de", "fullname": "John Doe", "roles": ["readonly"]}]
 
     # get user
     result = await execute("user show john@test.de")
-    assert result == [{"email": "john@test.de", "fullname": "John Doe", "roles": ["test"]}]
+    assert result == [{"email": "john@test.de", "fullname": "John Doe", "roles": ["readonly"]}]
 
     # add role to user
-    result = await execute("user role add john@test.de test2")
+    result = await execute("user role add john@test.de readwrite")
     roles = set(result[0]["roles"])  # type: ignore
-    assert roles == {"test", "test2"}
+    assert roles == {"readonly", "readwrite"}
 
     # remove role from user
-    result = await execute("user role delete john@test.de test2")
-    assert result == [{"email": "john@test.de", "fullname": "John Doe", "roles": ["test"]}]
+    result = await execute("user role delete john@test.de readwrite")
+    assert result == [{"email": "john@test.de", "fullname": "John Doe", "roles": ["readonly"]}]
 
     # Change password
     result = await execute("user password john@test.de bombproof")
     assert result == ["Password for john@test.de updated"]
 
     # create another user
     result = await execute('user add jane@test.de --fullname "Jane Doe" --password test --role admin')
```

### Comparing `resotocore-3.6.4/tests/resotocore/cli/model_test.py` & `resotocore-3.6.5/tests/resotocore/cli/model_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from textwrap import dedent
 
+import pytest
+
+from resotocore.cli.cli import CLIService
 from resotocore.cli.model import (
     CLIContext,
     AliasTemplate,
     AliasTemplateParameter,
     InfraAppAlias,
     InfraAppAliasParameter,
 )
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
+from resotocore.user.model import AuthorizedUser, Permission
 
 
 def test_format() -> None:
     context = CLIContext()
     fn = context.formatter("foo={foo} and bla={bla}: {bar}")
     assert fn({}) == "foo=null and bla=null: null"
     assert fn({"foo": 1, "bla": 2, "bar": 3}) == "foo=1 and bla=2: 3"
@@ -115,7 +119,30 @@
         ```
 
         readme
         ## Parameters
         - `--param-a` [required]: some a
         - `--param-b` [default: default_b]: some b"""
     )
+
+
+@pytest.mark.asyncio
+async def test_is_allowed(cli: CLIService) -> None:
+    # no user provided
+    res = (await cli.evaluate_cli_command("config show resoto.core"))[0]
+    assert res.is_allowed_to_execute() is False
+    res = (await cli.evaluate_cli_command("search all"))[0]
+    assert res.is_allowed_to_execute() is False
+    # user with read access
+    readonly = CLIContext(user=AuthorizedUser("test@test.de", {"readonly"}, {Permission.read}, True))
+    res = (await cli.evaluate_cli_command("config show resoto.core", context=readonly))[0]
+    assert res.is_allowed_to_execute() is False
+    res = (await cli.evaluate_cli_command("search all", context=readonly))[0]
+    assert res.is_allowed_to_execute() is True
+    # admin with all access
+    admin = CLIContext(
+        user=AuthorizedUser("test@test.de", {"admin"}, {Permission.read, Permission.write, Permission.admin}, True)
+    )
+    res = (await cli.evaluate_cli_command("config show resoto.core", context=admin))[0]
+    assert res.is_allowed_to_execute() is True
+    res = (await cli.evaluate_cli_command("search all", context=admin))[0]
+    assert res.is_allowed_to_execute() is True
```

### Comparing `resotocore-3.6.4/tests/resotocore/config/config_handler_service_test.py` & `resotocore-3.6.5/tests/resotocore/config/config_handler_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/config/config_override_service_test.py` & `resotocore-3.6.5/tests/resotocore/config/config_override_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/config/core_config_handler_test.py` & `resotocore-3.6.5/tests/resotocore/config/core_config_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/conftest.py` & `resotocore-3.6.5/tests/resotocore/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     WaitForCollectDone,
 )
 from resotocore.task.task_handler import TaskHandlerService
 from resotocore.types import Json
 from resotocore.user import UserManagement
 from resotocore.user.user_management import UserManagementService
 from resotocore.util import value_in_path, uuid_str, utc
+from resotocore.web.auth import AuthHandler
 from resotocore.web.certificate_handler import CertificateHandler
 from resotocore.worker_task_queue import WorkerTaskQueue, WorkerTaskDescription, WorkerTask, WorkerTaskName
 from resotolib.x509 import bootstrap_ca
 from tests.resotocore import create_graph
 from tests.resotocore.db.entitydb import InMemoryDb
 from tests.resotocore.model import ModelHandlerStatic
 from tests.resotocore.query.template_expander_test import InMemoryTemplateExpander
@@ -822,7 +823,16 @@
     with suppress(Exception):
         test_db.insert_document(
             "system_data", {"_key": "ca", "key": "private_key", "certificate": "some cert"}, overwrite=False
         )
     async_db = AsyncArangoDB(test_db)
     yield SystemDataDb(async_db)
     test_db.collection("system_data").delete({"_key": "ca"})
+
+
+@fixture
+async def auth_handler(
+    system_data_db: SystemDataDb, default_config: CoreConfig, cert_handler: CertificateHandler
+) -> AsyncIterator[AuthHandler]:
+    config = evolve(default_config, args=parse_args(["--psk", "test"]))
+    async with AuthHandler(system_data_db, config, cert_handler, set()) as auth:
+        yield auth
```

### Comparing `resotocore-3.6.4/tests/resotocore/console_renderer_test.py` & `resotocore-3.6.5/tests/resotocore/console_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/core_config_test.py` & `resotocore-3.6.5/tests/resotocore/core_config_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/arango_query_test.py` & `resotocore-3.6.5/tests/resotocore/db/arango_query_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/arangodb_functions_test.py` & `resotocore-3.6.5/tests/resotocore/db/arangodb_functions_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/async_arangodb_test.py` & `resotocore-3.6.5/tests/resotocore/db/async_arangodb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/configdb_test.py` & `resotocore-3.6.5/tests/resotocore/db/configdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/db_access_test.py` & `resotocore-3.6.5/tests/resotocore/db/db_access_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/deferredouteredgedb_test.py` & `resotocore-3.6.5/tests/resotocore/db/deferredouteredgedb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/entitydb.py` & `resotocore-3.6.5/tests/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/graphdb_test.py` & `resotocore-3.6.5/tests/resotocore/db/graphdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/jobdb_test.py` & `resotocore-3.6.5/tests/resotocore/db/jobdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/modeldb_test.py` & `resotocore-3.6.5/tests/resotocore/db/modeldb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/runningtaskdb_test.py` & `resotocore-3.6.5/tests/resotocore/db/runningtaskdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/subscriberdb_test.py` & `resotocore-3.6.5/tests/resotocore/db/subscriberdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/system_data_db_test.py` & `resotocore-3.6.5/tests/resotocore/db/system_data_db_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/db/templatedb_test.py` & `resotocore-3.6.5/tests/resotocore/db/templatedb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/dependencies_test.py` & `resotocore-3.6.5/tests/resotocore/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/graph_manager/graph_manager_test.py` & `resotocore-3.6.5/tests/resotocore/graph_manager/graph_manager_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/hypothesis_extension.py` & `resotocore-3.6.5/tests/resotocore/hypothesis_extension.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/infra_apps/local_runtime_test.py` & `resotocore-3.6.5/tests/resotocore/infra_apps/local_runtime_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/infra_apps/package_manager_test.py` & `resotocore-3.6.5/tests/resotocore/infra_apps/package_manager_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/message_bus_test.py` & `resotocore-3.6.5/tests/resotocore/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/__init__.py` & `resotocore-3.6.5/tests/resotocore/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/adjust_node_test.py` & `resotocore-3.6.5/tests/resotocore/model/adjust_node_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/db_updater_test.py` & `resotocore-3.6.5/tests/resotocore/model/db_updater_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/graph_access_test.py` & `resotocore-3.6.5/tests/resotocore/model/graph_access_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/json_schema_test.py` & `resotocore-3.6.5/tests/resotocore/model/json_schema_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/model_handler_test.py` & `resotocore-3.6.5/tests/resotocore/model/model_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/model_test.py` & `resotocore-3.6.5/tests/resotocore/model/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/model/typed_model_test.py` & `resotocore-3.6.5/tests/resotocore/model/typed_model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/query/__init__.py` & `resotocore-3.6.5/tests/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/query/model_test.py` & `resotocore-3.6.5/tests/resotocore/query/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/query/query_parser_test.py` & `resotocore-3.6.5/tests/resotocore/query/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/query/template_expander_test.py` & `resotocore-3.6.5/tests/resotocore/query/template_expander_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/report/benchnmark_renderer_test.py` & `resotocore-3.6.5/tests/resotocore/report/benchnmark_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/report/inspector_service_test.py` & `resotocore-3.6.5/tests/resotocore/report/inspector_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/task/job_handler_test.py` & `resotocore-3.6.5/tests/resotocore/task/job_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/task/start_workflow_on_first_subscriber_test.py` & `resotocore-3.6.5/tests/resotocore/task/start_workflow_on_first_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/task/subscribers_test.py` & `resotocore-3.6.5/tests/resotocore/task/subscribers_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/task/task_description_test.py` & `resotocore-3.6.5/tests/resotocore/task/task_description_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/task/task_handler_test.py` & `resotocore-3.6.5/tests/resotocore/task/task_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/user/user_management_service_test.py` & `resotocore-3.6.5/tests/resotocore/user/user_management_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/util_test.py` & `resotocore-3.6.5/tests/resotocore/util_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/utils.py` & `resotocore-3.6.5/tests/resotocore/utils.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/validator_test.py` & `resotocore-3.6.5/tests/resotocore/validator_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/web/api_client.py` & `resotocore-3.6.5/tests/resotocore/web/api_client.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/web/api_test.py` & `resotocore-3.6.5/tests/resotocore/web/api_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/web/certificate_handler_test.py` & `resotocore-3.6.5/tests/resotocore/web/certificate_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/web/content_renderer_test.py` & `resotocore-3.6.5/tests/resotocore/web/content_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.4/tests/resotocore/worker_task_queue_test.py` & `resotocore-3.6.5/tests/resotocore/worker_task_queue_test.py`

 * *Files identical despite different names*

