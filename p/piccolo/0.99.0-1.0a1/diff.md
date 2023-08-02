# Comparing `tmp/piccolo-0.99.0.tar.gz` & `tmp/piccolo-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/piccolo-0.99.0.tar", last modified: Fri Dec  2 13:06:22 2022, max compression
+gzip compressed data, was "piccolo-1.0a1.tar", last modified: Wed Aug  2 21:41:11 2023, max compression
```

## Comparing `piccolo-0.99.0.tar` & `piccolo-1.0a1.tar`

### file list

```diff
@@ -1,439 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2022-12-02 13:06:22.000000 piccolo-0.99.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3460 2022-12-02 13:06:06.000000 piccolo-0.99.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/new.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/app/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      428 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/templates/tables.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      340 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlite_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     2855 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_xpresso_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      387 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      497 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      510 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      530 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_starlite_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      402 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_xpresso_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      351 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      505 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      197 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (122)      421 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      379 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      235 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      152 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/
--rw-r--r--   0 runner    (1001) docker     (122)     7406 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/main.css
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     2130 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      224 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    29004 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/operations.py
--rw-r--r--   0 runner    (1001) docker     (122)    20546 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (122)     4439 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (122)    23745 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6533 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/backwards.py
--rw-r--r--   0 runner    (1001) docker     (122)     4473 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     2834 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     5362 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/forwards.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      681 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/templates/migration.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      593 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/playground/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/playground/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6949 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      222 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/project/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/project/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      408 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/schema/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    30631 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3190 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/schema/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      432 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      221 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/tester/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2431 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/user/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      649 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/change_password.py
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2273 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (122)      729 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
--rw-r--r--   0 runner    (1001) docker     (122)      982 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8203 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/columns/
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29532 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/choices.py
--rw-r--r--   0 runner    (1001) docker     (122)    77060 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/column_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     5262 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/columns/defaults/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/interval.py
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     3526 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2057 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (122)      443 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/uuid.py
--rw-r--r--   0 runner    (1001) docker     (122)      372 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/indexes.py
--rw-r--r--   0 runner    (1001) docker     (122)    13943 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/m2m.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/columns/operators/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/math.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/string.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/readable.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17145 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/conf/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/engine/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3702 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/cockroach.py
--rw-r--r--   0 runner    (1001) docker     (122)       44 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/finder.py
--rw-r--r--   0 runner    (1001) docker     (122)    14653 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)    18699 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (122)     5024 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/query/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16091 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/query/methods/
--rw-r--r--   0 runner    (1001) docker     (122)      421 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14890 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/alter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/count.py
--rw-r--r--   0 runner    (1001) docker     (122)     1636 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2594 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/create_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/drop_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/exists.py
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/indexes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/insert.py
--rw-r--r--   0 runner    (1001) docker     (122)     8814 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/raw.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/refresh.py
--rw-r--r--   0 runner    (1001) docker     (122)    21796 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/table_exists.py
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    14631 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     5859 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/querystring.py
--rw-r--r--   0 runner    (1001) docker     (122)    46497 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     7094 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/table_reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/testing/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/testing/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/testing/random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1886 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/utils/graphlib/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/graphlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/graphlib/_graphlib.py
--rw-r--r--   0 runner    (1001) docker     (122)     1912 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      310 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (122)    10749 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (122)      787 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/sql_values.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12783 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      386 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/profiling/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2022-12-02 13:06:06.000000 piccolo-0.99.0/profiling/run_profile.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2022-12-02 13:06:06.000000 piccolo-0.99.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 13:06:22.000000 piccolo-0.99.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2022-12-02 13:06:06.000000 piccolo-0.99.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (122)      551 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/commands/test_show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3097 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/asgi/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7464 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/commands/test_dump_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/commands/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/meta/commands/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/auto/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32788 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/integration/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2932 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33919 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    16245 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (122)     6196 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (122)    14170 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     7029 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_forwards_backwards.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/test_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/project/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/project/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/sql_shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/user/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/test_change_password.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/test_change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2250 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/test_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     7583 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/columns/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_bigint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1527 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_bytea.py
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_date.py
--rw-r--r--   0 runner    (1001) docker     (122)     7567 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_db_column_name.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_double_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (122)     3814 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     6821 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_jsonb.py
--rw-r--r--   0 runner    (1001) docker     (122)    24609 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_primary_key.py
--rw-r--r--   0 runner    (1001) docker     (122)      802 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_readable.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1507 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_reserved_column_names.py
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_smallint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_time.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_varchar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/conf/example.py
--rw-r--r--   0 runner    (1001) docker     (122)     7370 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/conf/test_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_extra_nodes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2175 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_nested_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     7339 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)      793 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_version_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/mega/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)    11834 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2359 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/music/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      568 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     2267 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/tables_detailed.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/query/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/query/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/mixins/test_columns_delegate.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/mixins/test_order_by_delegate.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_await.py
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_camelcase.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_querystring.py
--rw-r--r--   0 runner    (1001) docker     (122)      994 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/table/instance/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_get_related.py
--rw-r--r--   0 runner    (1001) docker     (122)     4690 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_get_related_readable.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4388 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_save.py
--rw-r--r--   0 runner    (1001) docker     (122)     3262 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_all_columns.py
--rw-r--r--   0 runner    (1001) docker     (122)    10728 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_alter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6381 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_count.py
--rw-r--r--   0 runner    (1001) docker     (122)     1431 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      903 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_create_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_create_table_class.py
--rw-r--r--   0 runner    (1001) docker     (122)     1252 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_drop_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (122)      840 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1990 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (122)    14109 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_join.py
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (122)     7895 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (122)     2695 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    34014 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_select.py
--rw-r--r--   0 runner    (1001) docker     (122)     1731 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_str.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_table_exists.py
--rw-r--r--   0 runner    (1001) docker     (122)    17748 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4236 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/testing/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/testing/test_random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      661 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (122)    20917 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_sql_values.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_table_reflection.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.623783 piccolo-1.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 21:40:53.000000 piccolo-1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-02 21:41:11.623783 piccolo-1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-08-02 21:40:53.000000 piccolo-1.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/app/commands/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/app/commands/show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo/apps/app/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/app/commands/templates/tables.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/app/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.579783 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/main.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/asgi/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/fixtures/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/fixtures/commands/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/fixtures/commands/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/fixtures/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/meta/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/meta/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.595783 piccolo-1.0a1/piccolo/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31765 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25348 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23938 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/auto/serialisation_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/backwards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/forwards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/migrations/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/commands/templates/migration.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/migrations/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/playground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/playground/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/playground/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/playground/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/playground/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/project/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/project/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/project/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/schema/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/schema/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/schema/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30480 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/schema/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/schema/commands/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/schema/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/schema/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.599783 piccolo-1.0a1/piccolo/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/sql_shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/sql_shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.603783 piccolo-1.0a1/piccolo/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.603783 piccolo-1.0a1/piccolo/apps/tester/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/tester/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/tester/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/tester/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.603783 piccolo-1.0a1/piccolo/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.603783 piccolo-1.0a1/piccolo/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/commands/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/commands/change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.603783 piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/apps/user/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.603783 piccolo-1.0a1/piccolo/columns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31392 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77243 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.603783 piccolo-1.0a1/piccolo/columns/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/defaults/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/m2m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.607783 piccolo-1.0a1/piccolo/columns/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/operators/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/operators/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/operators/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/columns/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.607783 piccolo-1.0a1/piccolo/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/conf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.607783 piccolo-1.0a1/piccolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/engine/cockroach.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/engine/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/engine/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/engine/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.607783 piccolo-1.0a1/piccolo/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/piccolo/query/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/drop_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/methods/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/query/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/table_reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/piccolo/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/testing/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/testing/random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/piccolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/piccolo/utils/graphlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/graphlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/graphlib/_graphlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-02 21:40:53.000000 piccolo-1.0a1/piccolo/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.591783 piccolo-1.0a1/piccolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-02 21:41:11.000000 piccolo-1.0a1/piccolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12896 2023-08-02 21:41:11.000000 piccolo-1.0a1/piccolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:11.000000 piccolo-1.0a1/piccolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 21:41:11.000000 piccolo-1.0a1/piccolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-02 21:41:11.000000 piccolo-1.0a1/piccolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 21:41:11.000000 piccolo-1.0a1/piccolo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 21:40:53.000000 piccolo-1.0a1/profiling/run_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-02 21:40:53.000000 piccolo-1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:41:11.623783 piccolo-1.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-02 21:40:53.000000 piccolo-1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.587783 piccolo-1.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/app/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/app/commands/test_show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/asgi/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/fixtures/commands/test_dump_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/fixtures/commands/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/meta/commands/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.611783 piccolo-1.0a1/tests/apps/migrations/auto/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42960 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/integration/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/test_diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34692 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/test_migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/test_schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/test_schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/auto/test_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/test_forwards_backwards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/migrations/commands/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/test_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/migrations/test_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/project/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/sql_shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/user/commands/test_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/user/commands/test_change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/user/commands/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/apps/user/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/columns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.615783 piccolo-1.0a1/tests/columns/m2m/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/m2m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14145 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/m2m/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/m2m/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/m2m/test_m2m_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_bytea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_db_column_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_double_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_jsonb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_primary_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_reserved_column_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_smallint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/columns/test_varchar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/conf/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/conf/test_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/engine/test_extra_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/engine/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/engine/test_nested_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/engine/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/engine/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/engine/test_version_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/example_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/example_apps/mega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/mega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/mega/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/example_apps/mega/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/mega/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/mega/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/example_apps/music/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/music/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/music/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/example_apps/music/tables_detailed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.619783 piccolo-1.0a1/tests/query/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/mixins/test_columns_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/mixins/test_order_by_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/test_camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/test_querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/query/test_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.623783 piccolo-1.0a1/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.623783 piccolo-1.0a1/tests/table/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/test_get_related.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/test_get_related_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/test_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/instance/test_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_all_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_create_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_create_table_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_drop_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_join_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39678 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/table/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.623783 piccolo-1.0a1/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/testing/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/testing/test_random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:11.623783 piccolo-1.0a1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_table_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-02 21:40:53.000000 piccolo-1.0a1/tests/utils/test_warnings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `piccolo-0.99.0/PKG-INFO` & `piccolo-1.0a1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,139 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 0.99.0
+Version: 1.0a1
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
 Project-URL: Tracker, https://github.com/piccolo-orm/piccolo/issues
-Description: ![Logo](https://raw.githubusercontent.com/piccolo-orm/piccolo/master/docs/logo_hero.png "Piccolo Logo")
-        
-        ![Tests](https://github.com/piccolo-orm/piccolo/actions/workflows/tests.yaml/badge.svg)
-        ![Release](https://github.com/piccolo-orm/piccolo/actions/workflows/release.yaml/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/piccolo-orm/badge/?version=latest)](https://piccolo-orm.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/piccolo?color=%2334D058&label=pypi)](https://pypi.org/project/piccolo/)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/piccolo-orm/piccolo.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/piccolo-orm/piccolo/context:python)
-        [![Total alerts](https://img.shields.io/lgtm/alerts/g/piccolo-orm/piccolo.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/piccolo-orm/piccolo/alerts/)
-        [![codecov](https://codecov.io/gh/piccolo-orm/piccolo/branch/master/graph/badge.svg?token=V19CWH7MXX)](https://codecov.io/gh/piccolo-orm/piccolo)
-        
-        Piccolo is a fast, user friendly ORM and query builder which supports asyncio. [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/).
-        
-        ## Features
-        
-        Some of it’s stand out features are:
-        
-        - Support for sync and async.
-        - A builtin playground, which makes learning a breeze.
-        - Tab completion support - works great with iPython and VSCode.
-        - Batteries included - a User model, authentication, migrations, an [admin GUI](https://github.com/piccolo-orm/piccolo_admin), and more.
-        - Modern Python - fully type annotated.
-        - Make your codebase modular and scalable with Piccolo apps (similar to Django apps).
-        
-        ## Syntax
-        
-        The syntax is clean and expressive.
-        
-        You can use it as a query builder:
-        
-        ```python
-        # Select:
-        await Band.select(
-            Band.name
-        ).where(
-            Band.popularity > 100
-        )
-        
-        # Join:
-        await Band.select(
-            Band.name,
-            Band.manager.name
-        )
-        
-        # Delete:
-        await Band.delete().where(
-            Band.popularity < 1000
-        )
-        
-        # Update:
-        await Band.update({Band.popularity: 10000}).where(
-            Band.name == 'Pythonistas'
-        )
-        ```
-        
-        Or like a typical ORM:
-        
-        ```python
-        # To create a new object:
-        b = Band(name='C-Sharps', popularity=100)
-        await b.save()
-        
-        # To fetch an object from the database, and update it:
-        b = await Band.objects().get(Band.name == 'Pythonistas')
-        b.popularity = 10000
-        await b.save()
-        
-        # To delete:
-        await b.remove()
-        ```
-        
-        ## Installation
-        
-        Installing with PostgreSQL driver:
-        
-        ```bash
-        pip install 'piccolo[postgres]'
-        ```
-        
-        Installing with SQLite driver:
-        
-        ```bash
-        pip install 'piccolo[sqlite]'
-        ```
-        
-        Installing with all optional dependencies (easiest):
-        
-        ```bash
-        pip install 'piccolo[all]'
-        ```
-        
-        ## Building a web app?
-        
-        Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
-        
-        ```bash
-        piccolo asgi new
-        ```
-        
-        [Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Xpresso](https://xpresso-api.dev/) and [Starlite](https://starlite-api.github.io/starlite/) are currently supported.
-        
-        ## Are you a Django user?
-        
-        We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
-        
-        ## Documentation
-        
-        Our documentation is on [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/piccolo/getting_started/index.html).
-        
-        We also have some great [tutorial videos on YouTube](https://www.youtube.com/channel/UCE7x5nm1Iy9KDfXPNrNQ5lA).
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Framework :: AsyncIO
 Classifier: Typing :: Typed
 Classifier: Topic :: Database
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: orjson
 Provides-Extra: playground
 Provides-Extra: postgres
 Provides-Extra: sqlite
 Provides-Extra: uvloop
 Provides-Extra: all
+License-File: LICENSE
+
+![Logo](https://raw.githubusercontent.com/piccolo-orm/piccolo/master/docs/logo_hero.png "Piccolo Logo")
+
+![Tests](https://github.com/piccolo-orm/piccolo/actions/workflows/tests.yaml/badge.svg)
+![Release](https://github.com/piccolo-orm/piccolo/actions/workflows/release.yaml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/piccolo-orm/badge/?version=latest)](https://piccolo-orm.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/piccolo?color=%2334D058&label=pypi)](https://pypi.org/project/piccolo/)
+[![codecov](https://codecov.io/gh/piccolo-orm/piccolo/branch/master/graph/badge.svg?token=V19CWH7MXX)](https://codecov.io/gh/piccolo-orm/piccolo)
+
+Piccolo is a fast, user friendly ORM and query builder which supports asyncio. [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/).
+
+## Features
+
+Some of it’s stand out features are:
+
+- Support for sync and async.
+- A builtin playground, which makes learning a breeze.
+- Tab completion support - works great with iPython and VSCode.
+- Batteries included - a User model, authentication, migrations, an [admin GUI](https://github.com/piccolo-orm/piccolo_admin), and more.
+- Modern Python - fully type annotated.
+- Make your codebase modular and scalable with Piccolo apps (similar to Django apps).
+
+## Syntax
+
+The syntax is clean and expressive.
+
+You can use it as a query builder:
+
+```python
+# Select:
+await Band.select(
+    Band.name
+).where(
+    Band.popularity > 100
+)
+
+# Join:
+await Band.select(
+    Band.name,
+    Band.manager.name
+)
+
+# Delete:
+await Band.delete().where(
+    Band.popularity < 1000
+)
+
+# Update:
+await Band.update({Band.popularity: 10000}).where(
+    Band.name == 'Pythonistas'
+)
+```
+
+Or like a typical ORM:
+
+```python
+# To create a new object:
+b = Band(name='C-Sharps', popularity=100)
+await b.save()
+
+# To fetch an object from the database, and update it:
+b = await Band.objects().get(Band.name == 'Pythonistas')
+b.popularity = 10000
+await b.save()
+
+# To delete:
+await b.remove()
+```
+
+## Installation
+
+Installing with PostgreSQL driver:
+
+```bash
+pip install 'piccolo[postgres]'
+```
+
+Installing with SQLite driver:
+
+```bash
+pip install 'piccolo[sqlite]'
+```
+
+Installing with all optional dependencies (easiest):
+
+```bash
+pip install 'piccolo[all]'
+```
+
+## Building a web app?
+
+Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
+
+```bash
+piccolo asgi new
+```
+
+[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/) and [Litestar](https://litestar.dev/) are currently supported.
+
+## Are you a Django user?
+
+We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
+
+## Documentation
+
+Our documentation is on [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/piccolo/getting_started/index.html).
+
+We also have some great [tutorial videos on YouTube](https://www.youtube.com/channel/UCE7x5nm1Iy9KDfXPNrNQ5lA).
```

### Comparing `piccolo-0.99.0/README.md` & `piccolo-1.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 ![Logo](https://raw.githubusercontent.com/piccolo-orm/piccolo/master/docs/logo_hero.png "Piccolo Logo")
 
 ![Tests](https://github.com/piccolo-orm/piccolo/actions/workflows/tests.yaml/badge.svg)
 ![Release](https://github.com/piccolo-orm/piccolo/actions/workflows/release.yaml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/piccolo-orm/badge/?version=latest)](https://piccolo-orm.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/piccolo?color=%2334D058&label=pypi)](https://pypi.org/project/piccolo/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/piccolo-orm/piccolo.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/piccolo-orm/piccolo/context:python)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/piccolo-orm/piccolo.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/piccolo-orm/piccolo/alerts/)
 [![codecov](https://codecov.io/gh/piccolo-orm/piccolo/branch/master/graph/badge.svg?token=V19CWH7MXX)](https://codecov.io/gh/piccolo-orm/piccolo)
 
 Piccolo is a fast, user friendly ORM and query builder which supports asyncio. [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/).
 
 ## Features
 
 Some of it’s stand out features are:
@@ -92,15 +90,15 @@
 
 Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
 
 ```bash
 piccolo asgi new
 ```
 
-[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Xpresso](https://xpresso-api.dev/) and [Starlite](https://starlite-api.github.io/starlite/) are currently supported.
+[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/) and [Litestar](https://litestar.dev/) are currently supported.
 
 ## Are you a Django user?
 
 We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
 
 ## Documentation
```

### Comparing `piccolo-0.99.0/piccolo/apps/app/commands/new.py` & `piccolo-1.0a1/piccolo/apps/app/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/new.py` & `piccolo-1.0a1/piccolo/apps/asgi/commands/new.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 
 import black
 import colorama
 from jinja2 import Environment, FileSystemLoader
 
 TEMPLATE_DIR = os.path.join(os.path.dirname(__file__), "templates/app/")
 SERVERS = ["uvicorn", "Hypercorn"]
-ROUTERS = ["starlette", "fastapi", "blacksheep", "xpresso", "starlite"]
+ROUTERS = ["starlette", "fastapi", "blacksheep", "litestar"]
 ROUTER_DEPENDENCIES = {
-    "starlite": ["starlite==1.23.0"],
-    "xpresso": ["xpresso==0.43.0", "di==0.72.1"],
+    "fastapi": ["fastapi>=0.100.0"],
 }
 
 
 def print_instruction(message: str):
     print(f"{colorama.Fore.CYAN}{message}{colorama.Fore.RESET}")
```

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlite_app.py.jinja` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,68 @@
 import typing as t
 
-from piccolo.engine import engine_finder
-from piccolo_admin.endpoints import create_admin
-from starlette.routing import Mount, Router
-from starlite import (
-    MediaType,
-    Response,
-    Starlite,
-    StaticFilesConfig,
-    TemplateConfig,
-    asgi,
-    delete,
-    get,
-    patch,
-    post,
-)
-from starlite.plugins.piccolo_orm import PiccoloORMPlugin
-from starlite.template.jinja import JinjaTemplateEngine
-from starlite.types import Receive, Scope, Send
-
 from home.endpoints import home
 from home.piccolo_app import APP_CONFIG
 from home.tables import Task
+from litestar import Litestar, asgi, delete, get, patch, post
+from litestar.contrib.jinja import JinjaTemplateEngine
+from litestar.exceptions import NotFoundException
+from litestar.static_files import StaticFilesConfig
+from litestar.template import TemplateConfig
+from litestar.types import Receive, Scope, Send
+from piccolo.engine import engine_finder
+from piccolo.utils.pydantic import create_pydantic_model
+from piccolo_admin.endpoints import create_admin
+
+TaskModelIn: t.Any = create_pydantic_model(
+    table=Task,
+    model_name="TaskModelIn",
+)
+TaskModelOut: t.Any = create_pydantic_model(
+    table=Task,
+    include_default_columns=True,
+    model_name="TaskModelOut",
+)
 
 
-@asgi(path="/{admin:path}")
-async def admin(scope: Scope, receive: Receive, send: Send) -> None:
-    router = Router(
-        [
-            Mount(
-                path="/admin",
-                app=create_admin(tables=APP_CONFIG.table_classes),
-            ),
-        ]
-    )
-    await router(scope=scope, receive=receive, send=send)
+# mounting Piccolo Admin
+@asgi("/admin/", is_mount=True)
+async def admin(scope: "Scope", receive: "Receive", send: "Send") -> None:
+    await create_admin(tables=APP_CONFIG.table_classes)(scope, receive, send)
 
 
 @get("/tasks", tags=["Task"])
-async def tasks() -> t.List[Task]:
-    tasks = await Task.select().order_by(Task.id, ascending=False)
-    return tasks
+async def tasks() -> t.List[TaskModelOut]:
+    return await Task.select().order_by(Task.id, ascending=False)
 
 
 @post("/tasks", tags=["Task"])
-async def create_task(data: Task) -> Task:
-    task = Task(**data.to_dict())
+async def create_task(data: TaskModelIn) -> TaskModelOut:
+    task = Task(**data.dict())
     await task.save()
-    return task
+    return task.to_dict()
 
 
 @patch("/tasks/{task_id:int}", tags=["Task"])
-async def update_task(task_id: int, data: Task) -> Task:
+async def update_task(task_id: int, data: TaskModelIn) -> TaskModelOut:
     task = await Task.objects().get(Task.id == task_id)
     if not task:
-        return Response(
-            content={},
-            media_type=MediaType.JSON,
-            status_code=404,
-        )
-    for key, value in data.to_dict().items():
-        task.id = task_id
+        raise NotFoundException("Task does not exist")
+    for key, value in data.dict().items():
         setattr(task, key, value)
 
     await task.save()
-    return task
+    return task.to_dict()
 
 
 @delete("/tasks/{task_id:int}", tags=["Task"])
 async def delete_task(task_id: int) -> None:
     task = await Task.objects().get(Task.id == task_id)
     if not task:
-        return Response(
-            content={},
-            media_type=MediaType.JSON,
-            status_code=404,
-        )
+        raise NotFoundException("Task does not exist")
     await task.remove()
 
 
 async def open_database_connection_pool():
     try:
         engine = engine_finder()
         await engine.start_connection_pool()
@@ -91,24 +74,23 @@
     try:
         engine = engine_finder()
         await engine.close_connection_pool()
     except Exception:
         print("Unable to connect to the database")
 
 
-app = Starlite(
+app = Litestar(
     route_handlers=[
         admin,
         home,
         tasks,
         create_task,
         update_task,
         delete_task,
     ],
-    plugins=[PiccoloORMPlugin()],
     template_config=TemplateConfig(
         directory="home/templates", engine=JinjaTemplateEngine
     ),
     static_files_config=[
         StaticFilesConfig(directories=["static"], path="/static/"),
     ],
     on_startup=[open_database_connection_pool],
```

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_starlite_endpoints.py.jinja` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 
 import jinja2
-from starlite import MediaType, Request, Response, get
+from litestar import MediaType, Request, Response, get
 
 ENVIRONMENT = jinja2.Environment(
     loader=jinja2.FileSystemLoader(
         searchpath=os.path.join(os.path.dirname(__file__), "templates")
     )
 )
 
 
-@get(path="/", include_in_schema=False)
+@get(path="/", include_in_schema=False, sync_to_thread=False)
 def home(request: Request) -> Response:
     template = ENVIRONMENT.get_template("home.html.jinja")
     content = template.render(title="Piccolo + ASGI")
     return Response(
         content,
         media_type=MediaType.HTML,
         status_code=200,
     )
+
```

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw`

 * *Files 9% similar despite different names*

```diff
@@ -47,20 +47,15 @@
                 <li><a href="/tasks/">JSON endpoint</a></li>
             </ul>
             <h3>BlackSheep</h3>
             <ul>
                 <li><a href="/admin/">Admin</a></li>
                 <li><a href="/docs/">Swagger API</a></li>
             </ul>
-            <h3>Xpresso</h3>
+            <h3>Litestar</h3>
             <ul>
                 <li><a href="/admin/">Admin</a></li>
-                <li><a href="/docs/">Swagger API</a></li>
-            </ul>
-            <h3>Starlite</h3>
-            <ul>
-                <li><a href="/admin">Admin</a></li>
                 <li><a href="/schema/swagger">Swagger API</a></li>
             </ul>
         </section>
     </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -23,14 +23,11 @@
     * Swagger_API
 **** Starlette ****
     * Admin
     * JSON_endpoint
 **** BlackSheep ****
     * Admin
     * Swagger_API
-**** Xpresso ****
-    * Admin
-    * Swagger_API
-**** Starlite ****
+**** Litestar ****
     * Admin
     * Swagger_API
 {% endblock content %}
```

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/main.css` & `piccolo-1.0a1/piccolo/apps/asgi/commands/templates/app/static/main.css`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/fixtures/commands/dump.py` & `piccolo-1.0a1/piccolo/apps/fixtures/commands/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """
     Dumps all of the data for the given tables into a JSON string.
     """
     dump = await get_dump(fixture_configs=fixture_configs)
     pydantic_model = create_pydantic_fixture_model(
         fixture_configs=fixture_configs
     )
-    return pydantic_model(**dump).json()
+    return pydantic_model(**dump).model_dump_json(indent=4)
 
 
 def parse_args(apps: str, tables: str) -> t.List[FixtureConfig]:
     """
     Works out which apps and tables the user is referring to.
     """
     finder = Finder()
```

### Comparing `piccolo-0.99.0/piccolo/apps/fixtures/commands/shared.py` & `piccolo-1.0a1/piccolo/apps/fixtures/commands/shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/auto/diffable_table.py` & `piccolo-1.0a1/piccolo/apps/migrations/auto/diffable_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,27 +12,32 @@
     deserialise_params,
     serialise_params,
 )
 from piccolo.columns.base import Column
 from piccolo.table import Table, create_table_class
 
 
-def compare_dicts(dict_1, dict_2) -> t.Dict[str, t.Any]:
+def compare_dicts(
+    dict_1: t.Dict[str, t.Any], dict_2: t.Dict[str, t.Any]
+) -> t.Dict[str, t.Any]:
     """
     Returns a new dictionary which only contains key, value pairs which are in
     the first dictionary and not the second.
 
-    For example:
-        dict_1 = {'a': 1, 'b': 2}
-        dict_2 = {'a': 1}
-        returns {'b': 2}
-
-        dict_1 = {'a': 2, 'b': 2}
-        dict_2 = {'a': 1}
-        returns {'a': 2, 'b': 2}
+    For example::
+
+        >>> dict_1 = {'a': 1, 'b': 2}
+        >>> dict_2 = {'a': 1}
+        >>> compare_dicts(dict_1, dict_2)
+        {'b': 2}
+
+        >>> dict_1 = {'a': 2, 'b': 2}
+        >>> dict_2 = {'a': 1}
+        >>> compare_dicts(dict_1, dict_2)
+        {'a': 2, 'b': 2}
 
     """
     output = {}
 
     for key, value in dict_1.items():
 
         dict_2_value = dict_2.get(key, ...)
@@ -86,14 +91,15 @@
     """
     Represents a Table. When we substract two instances, it returns the
     changes.
     """
 
     class_name: str
     tablename: str
+    schema: t.Optional[str] = None
     columns: t.List[Column] = field(default_factory=list)
     previous_class_name: t.Optional[str] = None
 
     def __post_init__(self):
         self.columns_map: t.Dict[str, Column] = {
             i._meta.name: i for i in self.columns
         }
@@ -208,12 +214,12 @@
 
     def to_table_class(self) -> t.Type[Table]:
         """
         Converts the DiffableTable into a Table subclass.
         """
         return create_table_class(
             class_name=self.class_name,
-            class_kwargs={"tablename": self.tablename},
+            class_kwargs={"tablename": self.tablename, "schema": self.schema},
             class_members={
                 column._meta.name: column for column in self.columns
             },
         )
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/auto/migration_manager.py` & `piccolo-1.0a1/piccolo/apps/migrations/auto/migration_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import inspect
 import typing as t
 from dataclasses import dataclass, field
 
 from piccolo.apps.migrations.auto.diffable_table import DiffableTable
 from piccolo.apps.migrations.auto.operations import (
     AlterColumn,
+    ChangeTableSchema,
     DropColumn,
     RenameColumn,
     RenameTable,
 )
 from piccolo.apps.migrations.auto.serialisation import deserialise_params
 from piccolo.columns import Column, column_types
 from piccolo.columns.column_types import Serial
@@ -131,14 +132,17 @@
     migration_id: str = ""
     app_name: str = ""
     description: str = ""
     preview: bool = False
     add_tables: t.List[DiffableTable] = field(default_factory=list)
     drop_tables: t.List[DiffableTable] = field(default_factory=list)
     rename_tables: t.List[RenameTable] = field(default_factory=list)
+    change_table_schemas: t.List[ChangeTableSchema] = field(
+        default_factory=list
+    )
     add_columns: AddColumnCollection = field(
         default_factory=AddColumnCollection
     )
     drop_columns: DropColumnCollection = field(
         default_factory=DropColumnCollection
     )
     rename_columns: RenameColumnCollection = field(
@@ -152,28 +156,52 @@
         default_factory=list
     )
 
     def add_table(
         self,
         class_name: str,
         tablename: str,
+        schema: t.Optional[str] = None,
         columns: t.Optional[t.List[Column]] = None,
     ):
         if not columns:
             columns = []
 
         self.add_tables.append(
             DiffableTable(
-                class_name=class_name, tablename=tablename, columns=columns
+                class_name=class_name,
+                tablename=tablename,
+                columns=columns,
+                schema=schema,
             )
         )
 
-    def drop_table(self, class_name: str, tablename: str):
+    def drop_table(
+        self, class_name: str, tablename: str, schema: t.Optional[str] = None
+    ):
         self.drop_tables.append(
-            DiffableTable(class_name=class_name, tablename=tablename)
+            DiffableTable(
+                class_name=class_name, tablename=tablename, schema=schema
+            )
+        )
+
+    def change_table_schema(
+        self,
+        class_name: str,
+        tablename: str,
+        new_schema: t.Optional[str] = None,
+        old_schema: t.Optional[str] = None,
+    ):
+        self.change_table_schemas.append(
+            ChangeTableSchema(
+                class_name=class_name,
+                tablename=tablename,
+                new_schema=new_schema,
+                old_schema=old_schema,
+            )
         )
 
     def rename_table(
         self,
         old_class_name: str,
         old_tablename: str,
         new_class_name: str,
@@ -678,15 +706,18 @@
         table_classes: t.List[t.Type[Table]] = []
         for add_table in self.add_tables:
             add_columns: t.List[
                 AddColumnClass
             ] = self.add_columns.for_table_class_name(add_table.class_name)
             _Table: t.Type[Table] = create_table_class(
                 class_name=add_table.class_name,
-                class_kwargs={"tablename": add_table.tablename},
+                class_kwargs={
+                    "tablename": add_table.tablename,
+                    "schema": add_table.schema,
+                },
                 class_members={
                     add_column.column._meta.name: add_column.column
                     for add_column in add_columns
                 },
             )
             table_classes.append(_Table)
 
@@ -753,14 +784,57 @@
                         )
                     )
                     if add_column.column._meta.index:
                         await self._run_query(
                             _Table.create_index([add_column.column])
                         )
 
+    async def _run_change_table_schema(self, backwards=False):
+        from piccolo.schema import SchemaManager
+
+        schema_manager = SchemaManager()
+
+        for change_table_schema in self.change_table_schemas:
+            if backwards:
+                # Note, we don't try dropping any schemas we may have created.
+                # It's dangerous to do so, just in case the user manually
+                # added tables etc to the scheme, and we delete them.
+
+                if change_table_schema.old_schema not in (None, "public"):
+                    await self._run_query(
+                        schema_manager.create_schema(
+                            schema_name=change_table_schema.old_schema,
+                            if_not_exists=True,
+                        )
+                    )
+                await self._run_query(
+                    schema_manager.move_table(
+                        table_name=change_table_schema.tablename,
+                        new_schema=change_table_schema.old_schema or "public",
+                        current_schema=change_table_schema.new_schema,
+                    )
+                )
+
+            else:
+                if change_table_schema.new_schema not in (None, "public"):
+                    await self._run_query(
+                        schema_manager.create_schema(
+                            schema_name=change_table_schema.new_schema,
+                            if_not_exists=True,
+                        )
+                    )
+
+                await self._run_query(
+                    schema_manager.move_table(
+                        table_name=change_table_schema.tablename,
+                        new_schema=change_table_schema.new_schema or "public",
+                        current_schema=change_table_schema.old_schema,
+                    )
+                )
+
     async def run(self, backwards=False):
         direction = "backwards" if backwards else "forwards"
         if self.preview:
             direction = "preview " + direction
         print(f"  - {self.migration_id} [{direction}]... ", end="")
 
         engine = engine_finder()
@@ -779,14 +853,15 @@
                 for raw in raw_list:
                     if inspect.iscoroutinefunction(raw):
                         await raw()
                     else:
                         raw()
 
             await self._run_add_tables(backwards=backwards)
+            await self._run_change_table_schema(backwards=backwards)
             await self._run_rename_tables(backwards=backwards)
             await self._run_add_columns(backwards=backwards)
             await self._run_drop_columns(backwards=backwards)
             await self._run_drop_tables(backwards=backwards)
             await self._run_rename_columns(backwards=backwards)
             # We can remove this for cockroach when resolved.
             # https://github.com/cockroachdb/cockroach/issues/49351
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/auto/operations.py` & `piccolo-1.0a1/piccolo/apps/migrations/auto/operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,22 @@
     old_class_name: str
     old_tablename: str
     new_class_name: str
     new_tablename: str
 
 
 @dataclass
+class ChangeTableSchema:
+    class_name: str
+    tablename: str
+    old_schema: t.Optional[str]
+    new_schema: t.Optional[str]
+
+
+@dataclass
 class RenameColumn:
     table_class_name: str
     tablename: str
     old_column_name: str
     new_column_name: str
     old_db_column_name: str
     new_db_column_name: str
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/auto/schema_differ.py` & `piccolo-1.0a1/piccolo/apps/migrations/auto/schema_differ.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from __future__ import annotations
 
+import inspect
 import typing as t
 from copy import deepcopy
 from dataclasses import dataclass, field
 
 from piccolo.apps.migrations.auto.diffable_table import (
     DiffableTable,
     TableDelta,
 )
-from piccolo.apps.migrations.auto.operations import RenameColumn, RenameTable
+from piccolo.apps.migrations.auto.migration_manager import MigrationManager
+from piccolo.apps.migrations.auto.operations import (
+    ChangeTableSchema,
+    RenameColumn,
+    RenameTable,
+)
 from piccolo.apps.migrations.auto.serialisation import (
     Definition,
     Import,
     UniqueGlobalNames,
     serialise_params,
 )
 from piccolo.utils.printing import get_fixed_length_string
@@ -29,25 +35,42 @@
     def old_class_names(self):
         return [i.old_class_name for i in self.rename_tables]
 
     @property
     def new_class_names(self):
         return [i.new_class_name for i in self.rename_tables]
 
+    def was_renamed_from(self, old_class_name: str) -> bool:
+        """
+        Returns ``True`` if the given class name was renamed.
+        """
+        for rename_table in self.rename_tables:
+            if rename_table.old_class_name == old_class_name:
+                return True
+        return False
+
     def renamed_from(self, new_class_name: str) -> t.Optional[str]:
         """
         Returns the old class name, if it exists.
         """
         rename = [
             i for i in self.rename_tables if i.new_class_name == new_class_name
         ]
         return rename[0].old_class_name if rename else None
 
 
 @dataclass
+class ChangeTableSchemaCollection:
+    collection: t.List[ChangeTableSchema] = field(default_factory=list)
+
+    def append(self, change_table_schema: ChangeTableSchema):
+        self.collection.append(change_table_schema)
+
+
+@dataclass
 class RenameColumnCollection:
     rename_columns: t.List[RenameColumn] = field(default_factory=list)
 
     def append(self, rename_column: RenameColumn):
         self.rename_columns.append(rename_column)
 
     def for_table_class_name(
@@ -66,18 +89,24 @@
     @property
     def new_column_names(self):
         return [i.new_column_name for i in self.rename_columns]
 
 
 @dataclass
 class AlterStatements:
-    statements: t.List[str]
+    statements: t.List[str] = field(default_factory=list)
     extra_imports: t.List[Import] = field(default_factory=list)
     extra_definitions: t.List[Definition] = field(default_factory=list)
 
+    def extend(self, alter_statements: AlterStatements):
+        self.statements.extend(alter_statements.statements)
+        self.extra_imports.extend(alter_statements.extra_imports)
+        self.extra_definitions.extend(alter_statements.extra_definitions)
+        return self
+
 
 @dataclass
 class SchemaDiffer:
     """
     Compares two lists of DiffableTables, and returns the list of alter
     statements required to make them match. Asks for user input when it isn't
     sure - for example, whether a column was renamed.
@@ -94,14 +123,17 @@
 
     ###########################################################################
 
     def __post_init__(self):
         self.schema_snapshot_map: t.Dict[str, DiffableTable] = {
             i.class_name: i for i in self.schema_snapshot
         }
+        self.table_schema_changes_collection = (
+            self.check_table_schema_changes()
+        )
         self.rename_tables_collection = self.check_rename_tables()
         self.rename_columns_collection = self.check_renamed_columns()
 
     def check_rename_tables(self) -> RenameTableCollection:
         """
         Work out whether any of the tables were renamed.
         """
@@ -125,14 +157,24 @@
         # A renamed table should have at least one column remaining with the
         # same name.
         for new_table in new_tables:
             new_column_names = [
                 i._meta.db_column_name for i in new_table.columns
             ]
             for drop_table in drop_tables:
+                if collection.was_renamed_from(
+                    old_class_name=drop_table.class_name
+                ):
+                    # We've already detected a table that was renamed from
+                    # this, so we can continue.
+                    # This can happen if we're renaming lots of tables in a
+                    # single migration.
+                    # https://github.com/piccolo-orm/piccolo/discussions/832
+                    continue
+
                 drop_column_names = [
                     i._meta.db_column_name for i in new_table.columns
                 ]
                 same_column_names = set(new_column_names).intersection(
                     drop_column_names
                 )
                 if len(same_column_names) > 0:
@@ -147,15 +189,15 @@
                             RenameTable(
                                 old_class_name=drop_table.class_name,
                                 old_tablename=drop_table.tablename,
                                 new_class_name=new_table.class_name,
                                 new_tablename=new_table.tablename,
                             )
                         )
-                        continue
+                        break
 
                     user_response = (
                         self.auto_input
                         if self.auto_input
                         else input(
                             f"Did you rename {drop_table.class_name} "
                             f"(tablename: {drop_table.tablename}) to "
@@ -168,14 +210,37 @@
                             RenameTable(
                                 old_class_name=drop_table.class_name,
                                 old_tablename=drop_table.tablename,
                                 new_class_name=new_table.class_name,
                                 new_tablename=new_table.tablename,
                             )
                         )
+                        break
+
+        return collection
+
+    def check_table_schema_changes(self) -> ChangeTableSchemaCollection:
+        collection = ChangeTableSchemaCollection()
+
+        for table in self.schema:
+            snapshot_table = self.schema_snapshot_map.get(
+                table.class_name, None
+            )
+            if not snapshot_table:
+                continue
+
+            if table.schema != snapshot_table.schema:
+                collection.append(
+                    ChangeTableSchema(
+                        class_name=table.class_name,
+                        tablename=table.tablename,
+                        new_schema=table.schema,
+                        old_schema=snapshot_table.schema,
+                    )
+                )
 
         return collection
 
     def check_renamed_columns(self) -> RenameColumnCollection:
         """
         Work out whether any of the columns were renamed.
         """
@@ -227,34 +292,92 @@
                         )
                         break
 
         return collection
 
     ###########################################################################
 
+    def _stringify_func(
+        self,
+        func: t.Callable,
+        params: t.Dict[str, t.Any],
+        prefix: t.Optional[str] = None,
+    ) -> AlterStatements:
+        """
+        Generates a string representing how to call the given function with the
+        give params. For example::
+
+            def my_callable(arg_1: str, arg_2: str):
+                ...
+
+            >>> _stringify_func(
+            ...     my_callable,
+            ...     {"arg_1": "a", "arg_2": "b"}
+            ... ).statements
+            ['my_callable(arg_1="a", arg_2="b")']
+
+        """
+        signature = inspect.signature(func)
+
+        if "self" in signature.parameters.keys():
+            params["self"] = None
+
+        serialised_params = serialise_params(params)
+
+        func_name = func.__name__
+
+        # This will raise an exception is we're missing parameters, which helps
+        # with debugging:
+        bound = signature.bind(**serialised_params.params)
+        bound.apply_defaults()
+
+        args = bound.arguments
+        if "self" in args:
+            args.pop("self")
+
+        args_str = ", ".join(f"{i}={repr(j)}" for i, j in args.items())
+
+        return AlterStatements(
+            statements=[f"{prefix or ''}{func_name}({args_str})"],
+            extra_definitions=serialised_params.extra_definitions,
+            extra_imports=serialised_params.extra_imports,
+        )
+
+    ###########################################################################
+
     @property
     def create_tables(self) -> AlterStatements:
         new_tables: t.List[DiffableTable] = list(
             set(self.schema) - set(self.schema_snapshot)
         )
 
         # Remove any which are renames
         new_tables = [
             i
             for i in new_tables
             if i.class_name
             not in self.rename_tables_collection.new_class_names
         ]
 
-        return AlterStatements(
-            statements=[
-                f"manager.add_table('{i.class_name}', tablename='{i.tablename}')"  # noqa: E501
-                for i in new_tables
-            ]
-        )
+        alter_statements = AlterStatements()
+
+        for i in new_tables:
+            alter_statements.extend(
+                self._stringify_func(
+                    func=MigrationManager.add_table,
+                    params={
+                        "class_name": i.class_name,
+                        "tablename": i.tablename,
+                        "schema": i.schema,
+                    },
+                    prefix="manager.",
+                )
+            )
+
+        return alter_statements
 
     @property
     def drop_tables(self) -> AlterStatements:
         drop_tables: t.List[DiffableTable] = list(
             set(self.schema_snapshot) - set(self.schema)
         )
 
@@ -262,29 +385,60 @@
         drop_tables = [
             i
             for i in drop_tables
             if i.class_name
             not in self.rename_tables_collection.old_class_names
         ]
 
-        return AlterStatements(
-            statements=[
-                f"manager.drop_table(class_name='{i.class_name}', tablename='{i.tablename}')"  # noqa: E501
-                for i in drop_tables
-            ]
-        )
+        alter_statements = AlterStatements()
+
+        for i in drop_tables:
+            alter_statements.extend(
+                self._stringify_func(
+                    func=MigrationManager.drop_table,
+                    params={
+                        "class_name": i.class_name,
+                        "tablename": i.tablename,
+                        "schema": i.schema,
+                    },
+                    prefix="manager.",
+                )
+            )
+
+        return alter_statements
 
     @property
     def rename_tables(self) -> AlterStatements:
-        return AlterStatements(
-            statements=[
-                f"manager.rename_table(old_class_name='{renamed_table.old_class_name}', old_tablename='{renamed_table.old_tablename}', new_class_name='{renamed_table.new_class_name}', new_tablename='{renamed_table.new_tablename}')"  # noqa
-                for renamed_table in self.rename_tables_collection.rename_tables  # noqa: E501
-            ]
-        )
+        alter_statements = AlterStatements()
+
+        for i in self.rename_tables_collection.rename_tables:
+            alter_statements.extend(
+                self._stringify_func(
+                    func=MigrationManager.rename_table,
+                    params=i.__dict__,
+                    prefix="manager.",
+                )
+            )
+
+        return alter_statements
+
+    @property
+    def change_table_schemas(self) -> AlterStatements:
+        alter_statements = AlterStatements()
+
+        for i in self.table_schema_changes_collection.collection:
+            alter_statements.extend(
+                self._stringify_func(
+                    func=MigrationManager.change_table_schema,
+                    params=i.__dict__,
+                    prefix="manager.",
+                )
+            )
+
+        return alter_statements
 
     ###########################################################################
 
     def _get_snapshot_table(
         self, table_class_name: str
     ) -> t.Optional[DiffableTable]:
         snapshot_table = self.schema_snapshot_map.get(table_class_name, None)
@@ -438,20 +592,26 @@
             statements=response,
             extra_imports=extra_imports,
             extra_definitions=extra_definitions,
         )
 
     @property
     def rename_columns(self) -> AlterStatements:
-        return AlterStatements(
-            statements=[
-                f"manager.rename_column(table_class_name='{i.table_class_name}', tablename='{i.tablename}', old_column_name='{i.old_column_name}', new_column_name='{i.new_column_name}', old_db_column_name='{i.old_db_column_name}', new_db_column_name='{i.new_db_column_name}')"  # noqa: E501
-                for i in self.rename_columns_collection.rename_columns
-            ]
-        )
+        alter_statements = AlterStatements()
+
+        for i in self.rename_columns_collection.rename_columns:
+            alter_statements.extend(
+                self._stringify_func(
+                    func=MigrationManager.rename_column,
+                    params=i.__dict__,
+                    prefix="manager.",
+                )
+            )
+
+        return alter_statements
 
     ###########################################################################
 
     @property
     def new_table_columns(self) -> AlterStatements:
         new_tables: t.List[DiffableTable] = list(
             set(self.schema) - set(self.schema_snapshot)
@@ -502,14 +662,15 @@
         """
         Call to execute the necessary alter commands on the database.
         """
         alter_statements: t.Dict[str, AlterStatements] = {
             "Created tables": self.create_tables,
             "Dropped tables": self.drop_tables,
             "Renamed tables": self.rename_tables,
+            "Tables which changed schema": self.change_table_schemas,
             "Created table columns": self.new_table_columns,
             "Dropped columns": self.drop_columns,
             "Columns added to existing tables": self.add_columns,
             "Renamed columns": self.rename_columns,
             "Altered columns": self.alter_columns,
         }
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/auto/schema_snapshot.py` & `piccolo-1.0a1/piccolo/apps/migrations/auto/schema_snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,20 @@
             for rename_table in manager.rename_tables:
                 for table in tables:
                     if table.class_name == rename_table.old_class_name:
                         table.class_name = rename_table.new_class_name
                         table.tablename = rename_table.new_tablename
                         break
 
+            for change_table_schema in manager.change_table_schemas:
+                for table in tables:
+                    if table.tablename == change_table_schema.tablename:
+                        table.schema = change_table_schema.new_schema
+                        break
+
             for table in tables:
                 add_columns = manager.add_columns.columns_for_table_class_name(
                     table.class_name
                 )
                 table.columns.extend(add_columns)
 
                 ###############################################################
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation.py` & `piccolo-1.0a1/piccolo/apps/migrations/auto/serialisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,17 +388,23 @@
                         params=column._meta.params
                     ),
                 )
             )
 
         #######################################################################
 
+        schema_str = (
+            "None"
+            if self.table_type._meta.schema is None
+            else f'"{self.table_type._meta.schema}"'
+        )
+
         definition = (
             f"class {self.table_class_name}"
-            f'({UniqueGlobalNames.TABLE}, tablename="{tablename}"): '
+            f'({UniqueGlobalNames.TABLE}, tablename="{tablename}", schema={schema_str}): '  # noqa: E501
             f"{pk_column_name} = {serialised_pk_column}"
         )
 
         for serialised_target_column in serialised_target_columns:
             definition += f"; {serialised_target_column.instance._meta.name} = {serialised_target_column}"  # noqa: E501
 
         return definition
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation_legacy.py` & `piccolo-1.0a1/piccolo/apps/migrations/auto/serialisation_legacy.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/commands/backwards.py` & `piccolo-1.0a1/piccolo/apps/migrations/commands/backwards.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import os
 import sys
+import typing as t
 
 from piccolo.apps.migrations.auto.migration_manager import MigrationManager
 from piccolo.apps.migrations.commands.base import (
     BaseMigrationManager,
     MigrationResult,
 )
 from piccolo.apps.migrations.tables import Migration
+from piccolo.conf.apps import AppConfig, MigrationModule
+from piccolo.utils.printing import print_heading
 
 
 class BackwardsMigrationManager(BaseMigrationManager):
     def __init__(
         self,
         app_name: str,
         migration_id: str,
@@ -23,28 +26,18 @@
         self.migration_id = migration_id
         self.app_name = app_name
         self.auto_agree = auto_agree
         self.clean = clean
         self.preview = preview
         super().__init__()
 
-    async def run(self) -> MigrationResult:
-        await self.create_migration_table()
-
-        app_modules = self.get_app_modules()
-
-        migration_modules = {}
-
-        for app_module in app_modules:
-            app_config = getattr(app_module, "APP_CONFIG")
-            if app_config.app_name == self.app_name:
-                migration_modules = self.get_migration_modules(
-                    app_config.migrations_folder_path
-                )
-                break
+    async def run_migrations_backwards(self, app_config: AppConfig):
+        migration_modules: t.Dict[
+            str, MigrationModule
+        ] = self.get_migration_modules(app_config.migrations_folder_path)
 
         ran_migration_ids = await Migration.get_migrations_which_ran(
             app_name=self.app_name
         )
         if len(ran_migration_ids) == 0:
             # Make sure a success is returned, as we don't want this
             # to appear as an error in automated scripts.
@@ -108,14 +101,19 @@
             return MigrationResult(success=True)
 
         else:  # pragma: no cover
             message = "Not proceeding."
             print(message, file=sys.stderr)
             return MigrationResult(success=False, message=message)
 
+    async def run(self) -> MigrationResult:
+        await self.create_migration_table()
+        app_config = self.get_app_config(self.app_name)
+        return await self.run_migrations_backwards(app_config=app_config)
+
 
 async def run_backwards(
     app_name: str,
     migration_id: str = "1",
     auto_agree: bool = False,
     clean: bool = False,
     preview: bool = False,
@@ -135,16 +133,15 @@
                 "Are you sure you want to continue? [y/N] "
             )
         )
 
         if _continue not in "yY":
             return MigrationResult(success=False, message="user cancelled")
         for _app_name in sorted_app_names:
-            print(f"\n{_app_name.upper():^64}")
-            print("-" * 64)
+            print_heading(_app_name)
             manager = BackwardsMigrationManager(
                 app_name=_app_name,
                 migration_id="all",
                 auto_agree=auto_agree,
                 preview=preview,
             )
             await manager.run()
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/commands/base.py` & `piccolo-1.0a1/piccolo/apps/migrations/commands/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/commands/check.py` & `piccolo-1.0a1/piccolo/apps/migrations/commands/check.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/commands/clean.py` & `piccolo-1.0a1/piccolo/apps/migrations/commands/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             .where(Migration.app_name == self.app_name)
             .output(as_list=True)
         )
 
         if len(migration_ids) > 0:
             query = query.where(Migration.name.not_in(migration_ids))
 
-        return query.run_sync()
+        return t.cast(t.List[str], query.run_sync())
 
     async def run(self):
         print("Checking the migration table ...")
 
         # Make sure the migration table exists, otherwise we'll get an error.
         await self.create_migration_table()
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/commands/forwards.py` & `piccolo-1.0a1/piccolo/apps/migrations/commands/forwards.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from piccolo.apps.migrations.auto.migration_manager import MigrationManager
 from piccolo.apps.migrations.commands.base import (
     BaseMigrationManager,
     MigrationResult,
 )
 from piccolo.apps.migrations.tables import Migration
 from piccolo.conf.apps import AppConfig, MigrationModule
+from piccolo.utils.printing import print_heading
 
 
 class ForwardsMigrationManager(BaseMigrationManager):
     def __init__(
         self,
         app_name: str,
         migration_id: str = "all",
@@ -105,16 +106,15 @@
     """
     Run the migrations. This function can be used to programatically run
     migrations - for example, in a unit test.
     """
     if app_name == "all":
         sorted_app_names = BaseMigrationManager().get_sorted_app_names()
         for _app_name in sorted_app_names:
-            print(f"\n{_app_name.upper():^64}")
-            print("-" * 64)
+            print_heading(_app_name)
             manager = ForwardsMigrationManager(
                 app_name=_app_name,
                 migration_id="all",
                 fake=fake,
                 preview=preview,
             )
             response = await manager.run()
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/commands/new.py` & `piccolo-1.0a1/piccolo/apps/migrations/commands/new.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import datetime
 import os
+import string
 import sys
 import typing as t
 from dataclasses import dataclass
 from itertools import chain
 from types import ModuleType
 
 import black
@@ -16,28 +17,30 @@
     AlterStatements,
     DiffableTable,
     SchemaDiffer,
     SchemaSnapshot,
 )
 from piccolo.conf.apps import AppConfig, Finder
 from piccolo.engine import SQLiteEngine
+from piccolo.utils.printing import print_heading
 
 from .base import BaseMigrationManager
 
 TEMPLATE_DIRECTORY = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "templates"
 )
 
 JINJA_ENV = jinja2.Environment(
     loader=jinja2.FileSystemLoader(searchpath=TEMPLATE_DIRECTORY),
 )
 
-
 MIGRATION_MODULES: t.Dict[str, ModuleType] = {}
 
+VALID_PYTHON_MODULE_CHARACTERS = string.ascii_lowercase + string.digits + "_"
+
 
 def render_template(**kwargs):
     template = JINJA_ENV.get_template("migration.py.jinja")
     return template.render(version=__VERSION__, **kwargs)
 
 
 def _create_migrations_folder(migrations_path: str) -> bool:
@@ -56,29 +59,48 @@
 @dataclass
 class NewMigrationMeta:
     migration_id: str
     migration_filename: str
     migration_path: str
 
 
+def now():
+    """
+    In a separate function so it's easier to patch in tests.
+    """
+    return datetime.datetime.now()
+
+
 def _generate_migration_meta(app_config: AppConfig) -> NewMigrationMeta:
     """
     Generates the migration ID and filename.
     """
     # The microseconds originally weren't part of the ID, but there was a
     # chance that the IDs would clash if the migrations are generated
     # programatically in quick succession (e.g. in a unit test), so they had
     # to be added. The trade off is a longer ID.
-    _id = datetime.datetime.now().strftime("%Y-%m-%dT%H:%M:%S:%f")
+    _id = now().strftime("%Y-%m-%dT%H:%M:%S:%f")
 
     # Originally we just used the _id as the filename, but colons aren't
     # supported in Windows, so we need to sanitize it. We don't want to
     # change the _id format though, as it would break existing migrations.
     # The filename doesn't have any special significance - only the id matters.
-    filename = _id.replace(":", "-")
+    cleaned_id = _id.replace(":", "_").replace("-", "_").lower()
+
+    # Just in case the app name contains characters which aren't valid for
+    # a Python module.
+    cleaned_app_name = "".join(
+        [
+            i
+            for i in app_config.app_name.lower().replace("-", "_")
+            if i in VALID_PYTHON_MODULE_CHARACTERS
+        ]
+    )
+
+    filename = f"{cleaned_app_name}_{cleaned_id}"
 
     path = os.path.join(app_config.migrations_folder_path, f"{filename}.py")
 
     return NewMigrationMeta(
         migration_id=_id, migration_filename=filename, migration_path=path
     )
 
@@ -165,14 +187,15 @@
 
         # Now get the current schema:
         current_diffable_tables = [
             DiffableTable(
                 class_name=i.__name__,
                 tablename=i._meta.tablename,
                 columns=i._meta.non_default_columns,
+                schema=i._meta.schema,
             )
             for i in app_config.table_classes
         ]
 
         # Compare the current schema with the snapshot
         differ = SchemaDiffer(
             schema=current_diffable_tables,
@@ -191,37 +214,57 @@
     desc: str = "",
     auto_input: t.Optional[str] = None,
 ):
     """
     Creates a new migration file in the migrations folder.
 
     :param app_name:
-        The app to create a migration for.
+        The app to create a migration for. Specify a value of 'all' to create
+        migrations for all apps (use in conjunction with --auto).
     :param auto:
         Auto create the migration contents.
     :param desc:
         A description of what the migration does, for example --desc='adding
         name column'.
     :param auto_input:
         If provided, all prompts for user input will automatically have this
         entered. For example, --auto_input='y'.
 
     """
-    print("Creating new migration ...")
-
     engine = Finder().get_engine()
     if auto and isinstance(engine, SQLiteEngine):
         sys.exit("Auto migrations aren't currently supported by SQLite.")
 
-    app_config = Finder().get_app_config(app_name=app_name)
+    if app_name == "all" and not auto:
+        raise ValueError(
+            "Only use `--app_name=all` in conjunction with `--auto`."
+        )
+
+    app_names = (
+        sorted(
+            BaseMigrationManager().get_app_names(
+                sort_by_migration_dependencies=False
+            )
+        )
+        if app_name == "all"
+        else [app_name]
+    )
+
+    for app_name in app_names:
+        print_heading(app_name)
+        print("🚀 Creating new migration ...")
+
+        app_config = Finder().get_app_config(app_name=app_name)
+
+        _create_migrations_folder(app_config.migrations_folder_path)
+
+        try:
+            await _create_new_migration(
+                app_config=app_config,
+                auto=auto,
+                description=desc,
+                auto_input=auto_input,
+            )
+        except NoChanges:
+            print("🏁 No changes detected.")
 
-    _create_migrations_folder(app_config.migrations_folder_path)
-    try:
-        await _create_new_migration(
-            app_config=app_config,
-            auto=auto,
-            description=desc,
-            auto_input=auto_input,
-        )
-    except NoChanges:
-        print("No changes detected - exiting.")
-        sys.exit(0)
+    print("\n✅ Finished\n")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/commands/templates/migration.py.jinja` & `piccolo-1.0a1/piccolo/apps/migrations/commands/templates/migration.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/piccolo_app.py` & `piccolo-1.0a1/piccolo/apps/migrations/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/migrations/tables.py` & `piccolo-1.0a1/piccolo/apps/migrations/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/playground/commands/run.py` & `piccolo-1.0a1/piccolo/apps/playground/commands/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,16 +132,15 @@
 
 def populate():
     """
     Drop then recreate the tables, and populate with data.
     """
     for _table in reversed(TABLES):
         try:
-            if _table.table_exists().run_sync():
-                _table.alter().drop_table().run_sync()
+            _table.alter().drop_table(if_exists=True).run_sync()
         except Exception as e:
             print(e)
 
     for _table in TABLES:
         try:
             _table.create_table().run_sync()
         except Exception as e:
@@ -176,21 +175,38 @@
         duration=datetime.timedelta(hours=2),
     )
     concert.save().run_sync()
 
     ticket = Ticket(concert=concert.id, price=Decimal("50.0"))
     ticket.save().run_sync()
 
-    discount_code = DiscountCode(code=uuid.uuid4())
-    discount_code.save().run_sync()
-
-    recording_studio = RecordingStudio(
-        name="Abbey Road", facilities={"restaurant": True, "mixing_desk": True}
-    )
-    recording_studio.save().run_sync()
+    DiscountCode.insert(
+        *[DiscountCode({DiscountCode.code: uuid.uuid4()}) for _ in range(5)]
+    ).run_sync()
+
+    RecordingStudio.insert(
+        RecordingStudio(
+            {
+                RecordingStudio.name: "Abbey Road",
+                RecordingStudio.facilities: {
+                    "restaurant": True,
+                    "mixing_desk": True,
+                },
+            }
+        ),
+        RecordingStudio(
+            {
+                RecordingStudio.name: "Electric Lady",
+                RecordingStudio.facilities: {
+                    "restaurant": False,
+                    "mixing_desk": True,
+                },
+            },
+        ),
+    ).run_sync()
 
 
 def run(
     engine: str = "sqlite",
     user: str = "piccolo",
     password: str = "piccolo",
     database: str = "piccolo_playground",
```

### Comparing `piccolo-0.99.0/piccolo/apps/project/commands/new.py` & `piccolo-1.0a1/piccolo/apps/project/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/schema/commands/generate.py` & `piccolo-1.0a1/piccolo/apps/schema/commands/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import json
 import re
 import typing as t
 import uuid
 from datetime import date, datetime
 
 import black
-from typing_extensions import Literal
 
 from piccolo.apps.migrations.auto.serialisation import serialise_params
 from piccolo.apps.schema.commands.exceptions import GenerateError
 from piccolo.columns import defaults
 from piccolo.columns.base import Column, OnDelete, OnUpdate
 from piccolo.columns.column_types import (
     JSON,
@@ -58,30 +57,30 @@
     schema: str = ""
 
 
 @dataclasses.dataclass
 class RowMeta:
     column_default: str
     column_name: str
-    is_nullable: Literal["YES", "NO"]
+    is_nullable: t.Literal["YES", "NO"]
     table_name: str
     character_maximum_length: t.Optional[int]
     data_type: str
     numeric_precision: t.Optional[t.Union[int, str]]
     numeric_scale: t.Optional[t.Union[int, str]]
-    numeric_precision_radix: t.Optional[Literal[2, 10]]
+    numeric_precision_radix: t.Optional[t.Literal[2, 10]]
 
     @classmethod
     def get_column_name_str(cls) -> str:
         return ", ".join(i.name for i in dataclasses.fields(cls))
 
 
 @dataclasses.dataclass
 class Constraint:
-    constraint_type: Literal["PRIMARY KEY", "UNIQUE", "FOREIGN KEY", "CHECK"]
+    constraint_type: t.Literal["PRIMARY KEY", "UNIQUE", "FOREIGN KEY", "CHECK"]
     constraint_name: str
     constraint_schema: t.Optional[str] = None
     column_name: t.Optional[str] = None
 
 
 @dataclasses.dataclass
 class TableConstraints:
@@ -137,15 +136,15 @@
 @dataclasses.dataclass
 class Trigger:
     constraint_name: str
     constraint_type: str
     table_name: str
     column_name: str
     on_update: str
-    on_delete: Literal[
+    on_delete: t.Literal[
         "NO ACTION", "RESTRICT", "CASCADE", "SET NULL", "SET_DEFAULT"
     ]
     references_table: str
     references_column: str
 
 
 @dataclasses.dataclass
@@ -662,18 +661,14 @@
         return ConstraintTable(
             name=response[0]["table_name"], schema=response[0]["table_schema"]
         )
     else:
         return ConstraintTable()
 
 
-def get_table_name(name: str, schema: str) -> str:
-    return name if schema == "public" else f"{schema}.{name}"
-
-
 async def create_table_class_from_db(
     table_class: t.Type[Table],
     tablename: str,
     schema_name: str,
     engine_type: str,
 ) -> OutputSchema:
     output_schema = OutputSchema()
@@ -808,15 +803,15 @@
         for extra_import in serialised_params.extra_imports:
             output_schema.imports.append(extra_import.__repr__())
 
         columns[column_name] = column
 
     table = create_table_class(
         class_name=_snake_to_camel(tablename),
-        class_kwargs={"tablename": get_table_name(tablename, schema_name)},
+        class_kwargs={"tablename": tablename, "schema": schema_name},
         class_members=columns,
     )
     output_schema.tables.append(table)
     return output_schema
 
 
 async def get_output_schema(
```

### Comparing `piccolo-0.99.0/piccolo/apps/schema/commands/graph.py` & `piccolo-1.0a1/piccolo/apps/schema/commands/graph.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja` & `piccolo-1.0a1/piccolo/apps/schema/commands/templates/graphviz.dot.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/shell/commands/run.py` & `piccolo-1.0a1/piccolo/apps/shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/sql_shell/commands/run.py` & `piccolo-1.0a1/piccolo/apps/sql_shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/tester/commands/run.py` & `piccolo-1.0a1/piccolo/apps/tester/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/commands/change_password.py` & `piccolo-1.0a1/piccolo/apps/user/commands/change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/commands/change_permissions.py` & `piccolo-1.0a1/piccolo/apps/user/commands/change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/commands/create.py` & `piccolo-1.0a1/piccolo/apps/user/commands/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/piccolo_app.py` & `piccolo-1.0a1/piccolo/apps/user/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py` & `piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py` & `piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py` & `piccolo-1.0a1/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/apps/user/tables.py` & `piccolo-1.0a1/piccolo/apps/user/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/__init__.py` & `piccolo-1.0a1/piccolo/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/base.py` & `piccolo-1.0a1/piccolo/columns/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -340,14 +340,18 @@
         We override deepcopy, as it's too slow if it has to recreate
         everything.
         """
         return self.copy()
 
 
 class Selectable(metaclass=ABCMeta):
+    """
+    Anything which inherits from this can be used in a select query.
+    """
+
     _alias: t.Optional[str]
 
     @abstractmethod
     def get_select_string(
         self, engine_type: str, with_alias: bool = True
     ) -> str:
         """
@@ -566,26 +570,33 @@
 
     def _validate_choices(
         self, choices: t.Type[Enum], allowed_type: t.Type[t.Any]
     ) -> bool:
         """
         Make sure the choices value has values of the allowed_type.
         """
+        if getattr(self, "_validated_choices", None):
+            # If it has previously been validated by a subclass, don't
+            # validate again.
+            return True
+
         for element in choices:
             if isinstance(element.value, allowed_type):
                 continue
             elif isinstance(element.value, Choice) and isinstance(
                 element.value.value, allowed_type
             ):
                 continue
             else:
                 raise ValueError(
                     f"{element.name} doesn't have the correct type"
                 )
 
+        self._validated_choices = True
+
         return True
 
     def is_in(self, values: t.List[t.Any]) -> Where:
         if len(values) == 0:
             raise ValueError(
                 "The `values` list argument must contain at least one value."
             )
@@ -744,14 +755,59 @@
             {'title': 'Pythonistas'}
 
         """
         column = copy.deepcopy(self)
         column._alias = name
         return column
 
+    def join_on(self, column: Column) -> ForeignKey:
+        """
+        Joins are typically performed via foreign key columns. For example,
+        here we get the band's name and the manager's name::
+
+            class Manager(Table):
+                name = Varchar()
+
+            class Band(Table):
+                name = Varchar()
+                manager = ForeignKey(Manager)
+
+            >>> await Band.select(Band.name, Band.manager.name)
+
+        The ``join_on`` method lets you join tables even when foreign keys
+        don't exist, by joining on a column in another table.
+
+        For example, here we want to get the manager's email, but no foreign
+        key exists::
+
+            class Manager(Table):
+                name = Varchar(unique=True)
+                email = Varchar()
+
+            class Band(Table):
+                name = Varchar()
+                manager_name = Varchar()
+
+            >>> await Band.select(
+            ...     Band.name,
+            ...     Band.manager_name.join_on(Manager.name).email
+            ... )
+
+        """
+        from piccolo.columns.column_types import ForeignKey
+
+        virtual_foreign_key = ForeignKey(
+            references=column._meta.table, target_column=column
+        )
+        virtual_foreign_key._meta._name = self._meta.name
+        virtual_foreign_key._meta.call_chain = [*self._meta.call_chain]
+        virtual_foreign_key._meta._table = self._meta.table
+        virtual_foreign_key.set_proxy_columns()
+        return virtual_foreign_key
+
     def get_default_value(self) -> t.Any:
         """
         If the column has a default attribute, return it. If it's callable,
         return the response instead.
         """
         default = getattr(self, "default", ...)
         if default is not ...:
@@ -849,20 +905,21 @@
         if self._meta.primary_key:
             query += " PRIMARY KEY"
         if self._meta.unique:
             query += " UNIQUE"
         if not self._meta.null:
             query += " NOT NULL"
 
-        foreign_key_meta: t.Optional[ForeignKeyMeta] = getattr(
-            self, "_foreign_key_meta", None
+        foreign_key_meta = t.cast(
+            t.Optional[ForeignKeyMeta],
+            getattr(self, "_foreign_key_meta", None),
         )
         if foreign_key_meta:
             references = foreign_key_meta.resolved_references
-            tablename = references._meta.tablename
+            tablename = references._meta.get_formatted_tablename()
             on_delete = foreign_key_meta.on_delete.value
             on_update = foreign_key_meta.on_update.value
             target_column_name = (
                 foreign_key_meta.resolved_target_column._meta.name
             )
             query += (
                 f" REFERENCES {tablename} ({target_column_name})"
```

### Comparing `piccolo-0.99.0/piccolo/columns/choices.py` & `piccolo-1.0a1/piccolo/columns/choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/column_types.py` & `piccolo-1.0a1/piccolo/columns/column_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 import inspect
 import typing as t
 import uuid
 from dataclasses import dataclass
 from datetime import date, datetime, time, timedelta
 from enum import Enum
 
-from typing_extensions import Literal
-
 from piccolo.columns.base import Column, ForeignKeyMeta, OnDelete, OnUpdate
 from piccolo.columns.combination import Where
 from piccolo.columns.defaults.date import DateArg, DateCustom, DateNow
 from piccolo.columns.defaults.interval import IntervalArg, IntervalCustom
 from piccolo.columns.defaults.time import TimeArg, TimeCustom, TimeNow
 from piccolo.columns.defaults.timestamp import (
     TimestampArg,
@@ -127,15 +125,15 @@
         await Band.update({Band.popularity: Band.popularity + 100})
 
     """
 
     def get_querystring(
         self,
         column_name: str,
-        operator: Literal["+", "-", "/", "*"],
+        operator: t.Literal["+", "-", "/", "*"],
         value: t.Union[int, float, Integer],
         reverse: bool = False,
     ) -> QueryString:
         if isinstance(value, Integer):
             column: Integer = value
             if len(column._meta.call_chain) > 0:
                 raise ValueError(
@@ -223,15 +221,15 @@
 
         output_string = ", ".join(output)
         return output_string
 
     def get_querystring(
         self,
         column: Column,
-        operator: Literal["+", "-"],
+        operator: t.Literal["+", "-"],
         value: timedelta,
         engine_type: str,
     ) -> QueryString:
         column_name = column._meta.name
 
         if not isinstance(value, timedelta):
             raise ValueError("Only timedelta values can be added.")
@@ -1213,15 +1211,15 @@
     def __get__(self, obj, objtype=None):
         return obj.__dict__[self._meta.name] if obj else self
 
     def __set__(self, obj, value: t.Union[time, None]):
         obj.__dict__[self._meta.name] = value
 
 
-class Interval(Column):  # lgtm [py/missing-equals]
+class Interval(Column):
     """
     Used for storing timedeltas. Uses the ``timedelta`` type for values.
 
     **Example**
 
     .. code-block:: python
 
@@ -1633,15 +1631,15 @@
 
 
 @dataclass
 class ForeignKeySetupResponse:
     is_lazy: bool
 
 
-class ForeignKey(Column):  # lgtm [py/missing-equals]
+class ForeignKey(Column):
     """
     Used to reference another table. Uses the same type as the primary key
     column on the table it references.
 
     **Example**
 
     .. code-block:: python
@@ -1780,15 +1778,15 @@
                 name = ForeignKey(
                     references=Manager,
                     on_delete=OnDelete.cascade
                 )
 
     :param on_update:
         Determines what the database should do when a row has it's primary key
-        updated. If set to ``OnDelete.cascade``, any rows referencing the
+        updated. If set to ``OnUpdate.cascade``, any rows referencing the
         updated row will have their references updated to point to the new
         primary key.
 
         Options:
 
         * ``OnUpdate.cascade`` (default)
         * ``OnUpdate.restrict``
@@ -1796,15 +1794,15 @@
         * ``OnUpdate.set_null``
         * ``OnUpdate.set_default``
 
         To learn more about the different options, see the `Postgres docs <https://www.postgresql.org/docs/current/ddl-constraints.html#DDL-CONSTRAINTS-FK>`_.
 
         .. code-block:: python
 
-            from piccolo.columns import OnDelete
+            from piccolo.columns import OnUpdate
 
             class Band(Table):
                 name = ForeignKey(
                     references=Manager,
                     on_update=OnUpdate.cascade
                 )
 
@@ -2121,23 +2119,25 @@
             # When querying a call chain more than 10 levels deep, an error
             # will be raised. Often there are more effective ways of
             # structuring a query than joining so many tables anyway.
             if len(new_column._meta.call_chain) >= 10:
                 raise Exception("Call chain too long!")
 
             foreign_key_meta: ForeignKeyMeta = object.__getattribute__(
-                self, "_foreign_key_meta"
+                new_column, "_foreign_key_meta"
             )
 
             for proxy_column in foreign_key_meta.proxy_columns:
                 try:
                     delattr(new_column, proxy_column._meta.name)
                 except Exception:
                     pass
 
+            foreign_key_meta.proxy_columns = []
+
             for (
                 column
             ) in value._foreign_key_meta.resolved_references._meta.columns:
                 _column: Column = column.copy()
                 _column._meta.call_chain = list(new_column._meta.call_chain)
                 setattr(new_column, _column._meta.name, _column)
                 foreign_key_meta.proxy_columns.append(_column)
@@ -2175,15 +2175,15 @@
     def __set__(self, obj, value: t.Any):
         obj.__dict__[self._meta.name] = value
 
 
 ###############################################################################
 
 
-class JSON(Column):  # lgtm[py/missing-equals]
+class JSON(Column):
     """
     Used for storing JSON strings. The data is stored as text. This can be
     preferable to JSONB if you just want to store and retrieve JSON without
     querying it directly. It works with SQLite and Postgres.
 
     :param default:
         Either a JSON string can be provided, or a Python ``dict`` or ``list``
@@ -2468,16 +2468,23 @@
         # This is a workaround because having `list` as a default breaks
         # Sphinx's autodoc.
         if isinstance(default, ListProxy):
             default = list
 
         self._validate_default(default, (list, None))
 
+        choices = kwargs.get("choices")
+        if choices is not None:
+            self._validate_choices(
+                choices, allowed_type=base_column.value_type
+            )
+            self._validated_choices = True
+
         # Usually columns are given a name by the Table metaclass, but in this
-        # case we have to assign one manually.
+        # case we have to assign one manually to the base column.
         base_column._meta._name = base_column.__class__.__name__
 
         self.base_column = base_column
         self.default = default
         self.index: t.Optional[int] = None
         kwargs.update({"base_column": base_column, "default": default})
         super().__init__(**kwargs)
```

### Comparing `piccolo-0.99.0/piccolo/columns/combination.py` & `piccolo-1.0a1/piccolo/columns/combination.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from __future__ import annotations
 
 import typing as t
 
-from piccolo.columns.operators.comparison import ComparisonOperator, Equal
+from piccolo.columns.operators.comparison import (
+    ComparisonOperator,
+    Equal,
+    IsNull,
+)
 from piccolo.custom_types import Combinable, Iterable
 from piccolo.querystring import QueryString
 from piccolo.utils.sql_values import convert_to_sql_value
 
 if t.TYPE_CHECKING:
     from piccolo.columns.base import Column
 
@@ -36,45 +40,59 @@
     def querystring(self) -> QueryString:
         return QueryString(
             "({} " + self.operator + " {})",
             self.first.querystring,
             self.second.querystring,
         )
 
+    @property
+    def querystring_for_update(self) -> QueryString:
+        return QueryString(
+            "({} " + self.operator + " {})",
+            self.first.querystring_for_update,
+            self.second.querystring_for_update,
+        )
+
     def __str__(self):
         return self.querystring.__str__()
 
 
 class And(Combination):
     operator = "AND"
 
     def get_column_values(self) -> t.Dict[Column, t.Any]:
         """
         This is used by `get_or_create` to know which values to assign if
         the row doesn't exist in the database.
 
-        For example, if we have:
+        For example, if we have::
+
+            (Band.name == 'Pythonistas') & (Band.popularity == 1000)
 
-        (Band.name == 'Pythonistas') & (Band.popularity == 1000)
+        We will return::
 
-        We will return {Band.name: 'Pythonistas', Band.popularity: 1000}.
+            {Band.name: 'Pythonistas', Band.popularity: 1000}.
 
         If the operator is anything besides equals, we don't return it, for
-        example:
+        example::
+
+            (Band.name == 'Pythonistas') & (Band.popularity > 1000)
 
-        (Band.name == 'Pythonistas') & (Band.popularity > 1000)
+        Returns::
 
-        Returns {Band.name: 'Pythonistas'}
+            {Band.name: 'Pythonistas'}
 
         """
         output = {}
         for combinable in (self.first, self.second):
             if isinstance(combinable, Where):
                 if combinable.operator == Equal:
                     output[combinable.column] = combinable.value
+                elif combinable.operator == IsNull:
+                    output[combinable.column] = None
             elif isinstance(combinable, And):
                 output.update(combinable.get_column_values())
 
         return output
 
 
 class Or(Combination):
@@ -91,26 +109,35 @@
 class WhereRaw(CombinableMixin):
     __slots__ = ("querystring",)
 
     def __init__(self, sql: str, *args: t.Any) -> None:
         """
         Execute raw SQL queries in your where clause. Use with caution!
 
-        await Band.where(
-            WhereRaw("name = 'Pythonistas'")
-        )
+        .. code-block:: python
+
+            await Band.where(
+                WhereRaw("name = 'Pythonistas'")
+            )
 
         Or passing in parameters:
 
-        await Band.where(
-            WhereRaw("name = {}", 'Pythonistas')
-        )
+        .. code-block:: python
+
+            await Band.where(
+                WhereRaw("name = {}", 'Pythonistas')
+            )
+
         """
         self.querystring = QueryString(sql, *args)
 
+    @property
+    def querystring_for_update(self) -> QueryString:
+        return self.querystring
+
     def __str__(self):
         return self.querystring.__str__()
 
 
 class Where(CombinableMixin):
 
     __slots__ = ("column", "value", "values", "operator")
@@ -186,9 +213,41 @@
             ),
             value="{}",
             values="{}",
         )
 
         return QueryString(template, *args)
 
+    @property
+    def querystring_for_update(self) -> QueryString:
+        args: t.List[t.Any] = []
+        if self.value != UNDEFINED:
+            args.append(self.value)
+
+        if self.values != UNDEFINED:
+            args.append(self.values_querystring)
+
+        column = self.column
+
+        if column._meta.call_chain:
+            # Use a sub select to find the correct ID.
+            root_column = column._meta.call_chain[0]
+            sub_query = root_column._meta.table.select(root_column).where(self)
+
+            column_name = column._meta.call_chain[0]._meta.name
+            return QueryString(
+                f"{column_name} IN ({{}})",
+                sub_query.querystrings[0],
+            )
+        else:
+            template = self.operator.template.format(
+                name=self.column.get_where_string(
+                    engine_type=self.column._meta.engine_type
+                ),
+                value="{}",
+                values="{}",
+            )
+
+            return QueryString(template, *args)
+
     def __str__(self):
         return self.querystring.__str__()
```

### Comparing `piccolo-0.99.0/piccolo/columns/defaults/base.py` & `piccolo-1.0a1/piccolo/columns/defaults/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/defaults/date.py` & `piccolo-1.0a1/piccolo/columns/defaults/date.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/defaults/interval.py` & `piccolo-1.0a1/piccolo/columns/defaults/interval.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 import typing as t
 from enum import Enum
 
 from .base import Default
 
 
-class IntervalCustom(Default):  # lgtm [py/missing-equals]
+class IntervalCustom(Default):
     def __init__(
         self,
         weeks: int = 0,
         days: int = 0,
         hours: int = 0,
         minutes: int = 0,
         seconds: int = 0,
```

### Comparing `piccolo-0.99.0/piccolo/columns/defaults/time.py` & `piccolo-1.0a1/piccolo/columns/defaults/time.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/defaults/timestamp.py` & `piccolo-1.0a1/piccolo/columns/defaults/timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/defaults/timestamptz.py` & `piccolo-1.0a1/piccolo/columns/defaults/timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/m2m.py` & `piccolo-1.0a1/piccolo/columns/m2m.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from piccolo.columns.column_types import (
     JSON,
     JSONB,
     Column,
     ForeignKey,
     LazyTableReference,
 )
+from piccolo.utils.list import flatten
 from piccolo.utils.sync import run_sync
 
 if t.TYPE_CHECKING:
     from piccolo.table import Table
 
 
 class M2MSelect(Selectable):
@@ -41,49 +42,53 @@
 
         """
         self.as_list = as_list
         self.columns = columns
         self.m2m = m2m
         self.load_json = load_json
 
-        safe_types = [int, str]
+        safe_types = (int, str)
 
-        # If the columns can be serialised / deserialise as JSON, then we
+        # If the columns can be serialised / deserialised as JSON, then we
         # can fetch the data all in one go.
         self.serialisation_safe = all(
             (column.__class__.value_type in safe_types)
             and (type(column) not in (JSON, JSONB))
             for column in columns
         )
 
     def get_select_string(self, engine_type: str, with_alias=True) -> str:
-        m2m_table_name = self.m2m._meta.resolved_joining_table._meta.tablename
+        m2m_table_name_with_schema = (
+            self.m2m._meta.resolved_joining_table._meta.get_formatted_tablename()  # noqa: E501
+        )  # noqa: E501
         m2m_relationship_name = self.m2m._meta.name
 
         fk_1 = self.m2m._meta.primary_foreign_key
         fk_1_name = fk_1._meta.db_column_name
         table_1 = fk_1._foreign_key_meta.resolved_references
         table_1_name = table_1._meta.tablename
+        table_1_name_with_schema = table_1._meta.get_formatted_tablename()
         table_1_pk_name = table_1._meta.primary_key._meta.db_column_name
 
         fk_2 = self.m2m._meta.secondary_foreign_key
         fk_2_name = fk_2._meta.db_column_name
         table_2 = fk_2._foreign_key_meta.resolved_references
         table_2_name = table_2._meta.tablename
+        table_2_name_with_schema = table_2._meta.get_formatted_tablename()
         table_2_pk_name = table_2._meta.primary_key._meta.db_column_name
 
         inner_select = f"""
-            "{m2m_table_name}"
-            JOIN "{table_1_name}" "inner_{table_1_name}" ON (
-                "{m2m_table_name}"."{fk_1_name}" = "inner_{table_1_name}"."{table_1_pk_name}"
+            {m2m_table_name_with_schema}
+            JOIN {table_1_name_with_schema} "inner_{table_1_name}" ON (
+                {m2m_table_name_with_schema}."{fk_1_name}" = "inner_{table_1_name}"."{table_1_pk_name}"
             )
-            JOIN "{table_2_name}" "inner_{table_2_name}" ON (
-                "{m2m_table_name}"."{fk_2_name}" = "inner_{table_2_name}"."{table_2_pk_name}"
+            JOIN {table_2_name_with_schema} "inner_{table_2_name}" ON (
+                {m2m_table_name_with_schema}."{fk_2_name}" = "inner_{table_2_name}"."{table_2_pk_name}"
             )
-            WHERE "{m2m_table_name}"."{fk_1_name}" = "{table_1_name}"."{table_1_pk_name}"
+            WHERE {m2m_table_name_with_schema}."{fk_1_name}" = "{table_1_name}"."{table_1_pk_name}"
         """  # noqa: E501
 
         if engine_type in ("postgres", "cockroach"):
             if self.as_list:
                 column_name = self.columns[0]._meta.db_column_name
                 return f"""
                     ARRAY(
@@ -404,30 +409,35 @@
 
         self._meta = M2MMeta(
             joining_table=joining_table,
             _foreign_key_columns=foreign_key_columns,
         )
 
     def __call__(
-        self, *columns: Column, as_list: bool = False, load_json: bool = False
+        self,
+        *columns: t.Union[Column, t.List[Column]],
+        as_list: bool = False,
+        load_json: bool = False,
     ) -> M2MSelect:
         """
         :param columns:
             Which columns to include from the related table. If none are
             specified, then all of the columns are returned.
         :param as_list:
             If a single column is provided, and ``as_list`` is ``True`` a
             flattened list will be returned, rather than a list of objects.
         :param load_json:
             If ``True``, any JSON strings are loaded as Python objects.
         """
-        if not columns:
-            columns = tuple(self._meta.secondary_table._meta.columns)
+        columns_ = flatten(columns)
+
+        if not columns_:
+            columns_ = self._meta.secondary_table._meta.columns
 
-        if as_list and len(columns) != 1:
+        if as_list and len(columns_) != 1:
             raise ValueError(
                 "`as_list` is only valid with a single column argument"
             )
 
         return M2MSelect(
-            *columns, m2m=self, as_list=as_list, load_json=load_json
+            *columns_, m2m=self, as_list=as_list, load_json=load_json
         )
```

### Comparing `piccolo-0.99.0/piccolo/columns/operators/comparison.py` & `piccolo-1.0a1/piccolo/columns/operators/comparison.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/readable.py` & `piccolo-1.0a1/piccolo/columns/readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/columns/reference.py` & `piccolo-1.0a1/piccolo/columns/reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/conf/apps.py` & `piccolo-1.0a1/piccolo/conf/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
-import functools
 import inspect
 import itertools
 import os
 import pathlib
 import traceback
 import typing as t
 from dataclasses import dataclass, field
 from importlib import import_module
 from types import ModuleType
 
 from piccolo.engine.base import Engine
 from piccolo.table import Table
+from piccolo.utils.graphlib import TopologicalSorter
 from piccolo.utils.warnings import Level, colored_warning
 
 
 class MigrationModule(ModuleType):
     ID: str
     VERSION: str
     DESCRIPTION: str
@@ -155,34 +155,46 @@
         self.commands = [
             i if isinstance(i, Command) else Command(i) for i in self.commands
         ]
 
         if isinstance(self.migrations_folder_path, pathlib.Path):
             self.migrations_folder_path = str(self.migrations_folder_path)
 
+        self._migration_dependency_app_configs: t.Optional[
+            t.List[AppConfig]
+        ] = None
+
     def register_table(self, table_class: t.Type[Table]):
         self.table_classes.append(table_class)
         return table_class
 
     @property
     def migration_dependency_app_configs(self) -> t.List[AppConfig]:
         """
-        Get all of the AppConfig instances from this app's migration
+        Get all of the ``AppConfig`` instances from this app's migration
         dependencies.
         """
-        modules: t.List[PiccoloAppModule] = [
-            t.cast(PiccoloAppModule, import_module(module_path))
-            for module_path in self.migration_dependencies
-        ]
-        return [i.APP_CONFIG for i in modules]
+        # We cache the value so it's more efficient, and also so we can set the
+        # underlying value in unit tests for easier mocking.
+        if self._migration_dependency_app_configs is None:
+
+            modules: t.List[PiccoloAppModule] = [
+                t.cast(PiccoloAppModule, import_module(module_path))
+                for module_path in self.migration_dependencies
+            ]
+            self._migration_dependency_app_configs = [
+                i.APP_CONFIG for i in modules
+            ]
+
+        return self._migration_dependency_app_configs
 
     def get_table_with_name(self, table_class_name: str) -> t.Type[Table]:
         """
-        Returns a Table subclass with the given name from this app, if it
-        exists. Otherwise raises a ValueError.
+        Returns a ``Table`` subclass with the given name from this app, if it
+        exists. Otherwise raises a ``ValueError``.
         """
         filtered = [
             table_class
             for table_class in self.table_classes
             if table_class.__name__ == table_class_name
         ]
         if not filtered:
@@ -422,52 +434,77 @@
         app_modules = self._import_app_modules(app_registry.apps)
 
         # Now deduplicate any dependencies
         app_modules = self._deduplicate(app_modules)
 
         return app_modules
 
-    def get_app_names(self, sort: bool = True) -> t.List[str]:
+    def get_app_names(
+        self, sort_by_migration_dependencies: bool = True
+    ) -> t.List[str]:
         """
         Return all of the app names.
 
-        :param sort:
+        :param sort_by_migration_dependencies:
             If True, sorts the app names using the migration dependencies, so
             dependencies are before dependents in the list.
 
         """
-        modules = self.get_app_modules()
-        configs: t.List[AppConfig] = [module.APP_CONFIG for module in modules]
-
-        if not sort:
-            return [i.app_name for i in configs]
-
-        def sort_app_configs(app_config_1: AppConfig, app_config_2: AppConfig):
-            return (
-                app_config_1 in app_config_2.migration_dependency_app_configs
+        return [
+            i.app_name
+            for i in self.get_app_configs(
+                sort_by_migration_dependencies=sort_by_migration_dependencies
             )
-
-        sorted_configs = sorted(
-            configs, key=functools.cmp_to_key(sort_app_configs)
-        )
-        return [i.app_name for i in sorted_configs]
+        ]
 
     def get_sorted_app_names(self) -> t.List[str]:
         """
-        Just here for backwards compatibility.
+        Just here for backwards compatibility - use ``get_app_names`` directly.
+        """
+        return self.get_app_names(sort_by_migration_dependencies=True)
+
+    def sort_app_configs(
+        self, app_configs: t.List[AppConfig]
+    ) -> t.List[AppConfig]:
+        app_config_map = {
+            app_config.app_name: app_config for app_config in app_configs
+        }
+
+        sorted_app_names = TopologicalSorter(
+            {
+                app_config.app_name: [
+                    i.app_name
+                    for i in app_config.migration_dependency_app_configs
+                ]
+                for app_config in app_config_map.values()
+            }
+        ).static_order()
+
+        return [app_config_map[i] for i in sorted_app_names]
+
+    def get_app_configs(
+        self, sort_by_migration_dependencies: bool = True
+    ) -> t.List[AppConfig]:
         """
-        return self.get_app_names(sort=True)
+        Returns a list of ``AppConfig``, optionally sorted by migration
+        dependencies.
+        """
+        app_configs = [i.APP_CONFIG for i in self.get_app_modules()]
+
+        return (
+            self.sort_app_configs(app_configs=app_configs)
+            if sort_by_migration_dependencies
+            else app_configs
+        )
 
     def get_app_config(self, app_name: str) -> AppConfig:
         """
         Returns an ``AppConfig`` for the given app name.
         """
-        modules = self.get_app_modules()
-        for module in modules:
-            app_config = module.APP_CONFIG
+        for app_config in self.get_app_configs():
             if app_config.app_name == app_name:
                 return app_config
         raise ValueError(f"No app found with name {app_name}")
 
     def get_table_with_name(
         self, app_name: str, table_class_name: str
     ) -> t.Type[Table]:
@@ -483,15 +520,15 @@
     def get_table_classes(
         self,
         include_apps: t.Optional[t.List[str]] = None,
         exclude_apps: t.Optional[t.List[str]] = None,
     ) -> t.List[t.Type[Table]]:
         """
         Returns all ``Table`` classes registered with the given apps. If
-        ``app_names`` is ``None``, then ``Table`` classes will be returned
+        ``include_apps`` is ``None``, then ``Table`` classes will be returned
         for all apps.
         """
         if include_apps and exclude_apps:
             raise ValueError("Only specify `include_apps` or `exclude_apps`.")
 
         if include_apps:
             app_names = include_apps
```

### Comparing `piccolo-0.99.0/piccolo/engine/base.py` & `piccolo-1.0a1/piccolo/engine/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import contextvars
 import logging
+import pprint
 import typing as t
 from abc import ABCMeta, abstractmethod
 
 from piccolo.querystring import QueryString
 from piccolo.utils.sync import run_sync
-from piccolo.utils.warnings import Level, colored_warning
+from piccolo.utils.warnings import Level, colored_string, colored_warning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.query.base import Query
 
 
 logger = logging.getLogger(__name__)
 
@@ -21,19 +22,20 @@
 
 
 TransactionClass = t.TypeVar("TransactionClass")
 
 
 class Engine(t.Generic[TransactionClass], metaclass=ABCMeta):
 
-    __slots__ = ()
+    __slots__ = ("query_id",)
 
     def __init__(self):
         run_sync(self.check_version())
         run_sync(self.prep_database())
+        self.query_id = 0
 
     @property
     @abstractmethod
     def engine_type(self) -> str:
         pass
 
     @property
@@ -133,7 +135,24 @@
             ``True`` if a transaction is already active for the current
             asyncio task. This is useful to know, because nested transactions
             aren't currently supported, so you can check if an existing
             transaction is already active, before creating a new one.
 
         """
         return self.current_transaction.get() is not None
+
+    ###########################################################################
+    # Logging queries and responses
+
+    def get_query_id(self) -> int:
+        self.query_id += 1
+        return self.query_id
+
+    def print_query(self, query_id: int, query: str):
+        print(colored_string(f"\nQuery {query_id}:"))
+        print(query)
+
+    def print_response(self, query_id: int, response: t.List):
+        print(
+            colored_string(f"\nQuery {query_id} response:", level=Level.high)
+        )
+        pprint.pprint(response)
```

### Comparing `piccolo-0.99.0/piccolo/engine/cockroach.py` & `piccolo-1.0a1/piccolo/engine/cockroach.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,22 @@
     min_version_number = 0  # Doesn't seem to work with cockroach versioning.
 
     def __init__(
         self,
         config: t.Dict[str, t.Any],
         extensions: t.Sequence[str] = (),
         log_queries: bool = False,
+        log_responses: bool = False,
         extra_nodes: t.Dict[str, CockroachEngine] = None,
     ) -> None:
         super().__init__(
             config=config,
             extensions=extensions,
             log_queries=log_queries,
+            log_responses=log_responses,
             extra_nodes=extra_nodes,
         )
 
     async def prep_database(self):
         try:
             await self._run_in_new_connection(
                 "SET CLUSTER SETTING sql.defaults.experimental_alter_column_type.enabled = true;"  # noqa: E501
```

### Comparing `piccolo-0.99.0/piccolo/engine/postgres.py` & `piccolo-1.0a1/piccolo/engine/postgres.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import contextvars
 import typing as t
 from dataclasses import dataclass
 
 from piccolo.engine.base import Batch, Engine
 from piccolo.engine.exceptions import TransactionError
 from piccolo.query.base import DDL, Query
-from piccolo.query.methods.objects import Create, GetOrCreate
 from piccolo.querystring import QueryString
 from piccolo.utils.lazy_loader import LazyLoader
 from piccolo.utils.sync import run_sync
 from piccolo.utils.warnings import Level, colored_warning
 
 asyncpg = LazyLoader("asyncpg", globals(), "asyncpg")
 
@@ -96,14 +95,16 @@
         self.engine = engine
         self.queries: t.List[Query] = []
 
     def add(self, *query: Query):
         self.queries += list(query)
 
     async def run(self):
+        from piccolo.query.methods.objects import Create, GetOrCreate
+
         try:
             async with self.engine.transaction():
                 for query in self.queries:
                     if isinstance(query, (Query, DDL, Create, GetOrCreate)):
                         await query.run()
                     else:
                         raise ValueError("Unrecognised query")
@@ -118,58 +119,144 @@
     def __await__(self):
         return self.run().__await__()
 
 
 ###############################################################################
 
 
+class Savepoint:
+    def __init__(self, name: str, transaction: PostgresTransaction):
+        self.name = name
+        self.transaction = transaction
+
+    async def rollback_to(self):
+        await self.transaction.connection.execute(
+            f"ROLLBACK TO SAVEPOINT {self.name}"
+        )
+
+    async def release(self):
+        await self.transaction.connection.execute(
+            f"RELEASE SAVEPOINT {self.name}"
+        )
+
+
 class PostgresTransaction:
     """
     Used for wrapping queries in a transaction, using a context manager.
     Currently it's async only.
 
     Usage::
 
         async with engine.transaction():
             # Run some queries:
             await Band.select().run()
 
     """
 
-    __slots__ = ("engine", "transaction", "context", "connection")
+    __slots__ = (
+        "engine",
+        "transaction",
+        "context",
+        "connection",
+        "_savepoint_id",
+        "_parent",
+        "_committed",
+        "_rolled_back",
+    )
 
-    def __init__(self, engine: PostgresEngine):
+    def __init__(self, engine: PostgresEngine, allow_nested: bool = True):
+        """
+        :param allow_nested:
+            If ``True`` then if we try creating a new transaction when another
+            is already active, we treat this as a no-op::
+
+                async with DB.transaction():
+                    async with DB.transaction():
+                        pass
+
+            If we want to disallow this behaviour, then setting
+            ``allow_nested=False`` will cause a ``TransactionError`` to be
+            raised.
+
+        """
         self.engine = engine
-        if self.engine.current_transaction.get():
-            raise TransactionError(
-                "A transaction is already active - nested transactions aren't "
-                "currently supported."
-            )
+        current_transaction = self.engine.current_transaction.get()
 
-    async def __aenter__(self):
+        self._savepoint_id = 0
+        self._parent = None
+        self._committed = False
+        self._rolled_back = False
+
+        if current_transaction:
+            if allow_nested:
+                self._parent = current_transaction
+            else:
+                raise TransactionError(
+                    "A transaction is already active - nested transactions "
+                    "aren't allowed."
+                )
+
+    async def __aenter__(self) -> PostgresTransaction:
+        if self._parent is not None:
+            return self._parent
+
+        self.connection = await self.get_connection()
+        self.transaction = self.connection.transaction()
+        await self.begin()
+        self.context = self.engine.current_transaction.set(self)
+        return self
+
+    async def get_connection(self):
         if self.engine.pool:
-            self.connection = await self.engine.pool.acquire()
+            return await self.engine.pool.acquire()
         else:
-            self.connection = await self.engine.get_new_connection()
+            return await self.engine.get_new_connection()
 
-        self.transaction = self.connection.transaction()
+    async def begin(self):
         await self.transaction.start()
-        self.context = self.engine.current_transaction.set(self)
 
     async def commit(self):
         await self.transaction.commit()
+        self._committed = True
 
     async def rollback(self):
         await self.transaction.rollback()
+        self._rolled_back = True
+
+    async def rollback_to(self, savepoint_name: str):
+        """
+        Used to rollback to a savepoint just using the name.
+        """
+        await Savepoint(name=savepoint_name, transaction=self).rollback_to()
+
+    ###########################################################################
+
+    def get_savepoint_id(self) -> int:
+        self._savepoint_id += 1
+        return self._savepoint_id
+
+    async def savepoint(self, name: t.Optional[str] = None) -> Savepoint:
+        name = name or f"savepoint_{self.get_savepoint_id()}"
+        await self.connection.execute(f"SAVEPOINT {name}")
+        return Savepoint(name=name, transaction=self)
+
+    ###########################################################################
 
     async def __aexit__(self, exception_type, exception, traceback):
+        if self._parent:
+            return exception is None
+
         if exception:
-            await self.rollback()
+            # The user may have manually rolled it back.
+            if not self._rolled_back:
+                await self.rollback()
         else:
-            await self.commit()
+            # The user may have manually committed it.
+            if not self._committed and not self._rolled_back:
+                await self.commit()
 
         if self.engine.pool:
             await self.engine.pool.release(self.connection)
         else:
             await self.connection.close()
 
         self.engine.current_transaction.reset(self.context)
@@ -204,14 +291,18 @@
         in Postgres. If you're using a read only database, set this value to an
         empty tuple ``()``.
 
     :param log_queries:
         If ``True``, all SQL and DDL statements are printed out before being
         run. Useful for debugging.
 
+    :param log_responses:
+        If ``True``, the raw response from each query is printed out. Useful
+        for debugging.
+
     :param extra_nodes:
         If you have additional database nodes (e.g. read replicas) for the
         server, you can specify them here. It's a mapping of a memorable name
         to a ``PostgresEngine`` instance. For example::
 
             DB = PostgresEngine(
                 config={'database': 'main_db'},
@@ -235,35 +326,38 @@
 
     """  # noqa: E501
 
     __slots__ = (
         "config",
         "extensions",
         "log_queries",
+        "log_responses",
         "extra_nodes",
         "pool",
         "current_transaction",
     )
 
     engine_type = "postgres"
     min_version_number = 10
 
     def __init__(
         self,
         config: t.Dict[str, t.Any],
         extensions: t.Sequence[str] = ("uuid-ossp",),
         log_queries: bool = False,
+        log_responses: bool = False,
         extra_nodes: t.Mapping[str, PostgresEngine] = None,
     ) -> None:
         if extra_nodes is None:
             extra_nodes = {}
 
         self.config = config
         self.extensions = extensions
         self.log_queries = log_queries
+        self.log_responses = log_responses
         self.extra_nodes = extra_nodes
         self.pool: t.Optional[Pool] = None
         database_name = config.get("database", "Unknown")
         self.current_transaction = contextvars.ContextVar(
             f"pg_current_transaction_{database_name}", default=None
         )
         super().__init__()
@@ -317,15 +411,15 @@
                     "extensions, or add it manually using "
                     f'`CREATE EXTENSION "{extension}";`',
                     level=Level.medium,
                 )
 
     ###########################################################################
     # These typos existed in the codebase for a while, so leaving these proxy
-    # methods for now to ensure backwards compatility.
+    # methods for now to ensure backwards compatibility.
 
     async def start_connnection_pool(self, **kwargs) -> None:
         colored_warning(
             "`start_connnection_pool` is a typo - please change it to "
             "`start_connection_pool`.",
             category=DeprecationWarning,
         )
@@ -422,39 +516,53 @@
     async def run_querystring(
         self, querystring: QueryString, in_pool: bool = True
     ):
         query, query_args = querystring.compile_string(
             engine_type=self.engine_type
         )
 
+        query_id = self.get_query_id()
+
         if self.log_queries:
-            print(querystring)
+            self.print_query(query_id=query_id, query=querystring.__str__())
 
         # If running inside a transaction:
         current_transaction = self.current_transaction.get()
         if current_transaction:
-            return await current_transaction.connection.fetch(
+            response = await current_transaction.connection.fetch(
                 query, *query_args
             )
         elif in_pool and self.pool:
-            return await self._run_in_pool(query, query_args)
+            response = await self._run_in_pool(query, query_args)
         else:
-            return await self._run_in_new_connection(query, query_args)
+            response = await self._run_in_new_connection(query, query_args)
+
+        if self.log_responses:
+            self.print_response(query_id=query_id, response=response)
+
+        return response
 
     async def run_ddl(self, ddl: str, in_pool: bool = True):
+        query_id = self.get_query_id()
+
         if self.log_queries:
-            print(ddl)
+            self.print_query(query_id=query_id, query=ddl)
 
         # If running inside a transaction:
         current_transaction = self.current_transaction.get()
         if current_transaction:
-            return await current_transaction.connection.fetch(ddl)
+            response = await current_transaction.connection.fetch(ddl)
         elif in_pool and self.pool:
-            return await self._run_in_pool(ddl)
+            response = await self._run_in_pool(ddl)
         else:
-            return await self._run_in_new_connection(ddl)
+            response = await self._run_in_new_connection(ddl)
+
+        if self.log_responses:
+            self.print_response(query_id=query_id, response=response)
+
+        return response
 
     def atomic(self) -> Atomic:
         return Atomic(engine=self)
 
-    def transaction(self) -> PostgresTransaction:
-        return PostgresTransaction(engine=self)
+    def transaction(self, allow_nested: bool = True) -> PostgresTransaction:
+        return PostgresTransaction(engine=self, allow_nested=allow_nested)
```

### Comparing `piccolo-0.99.0/piccolo/engine/sqlite.py` & `piccolo-1.0a1/piccolo/engine/sqlite.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import uuid
 from dataclasses import dataclass
 from decimal import Decimal
 
 from piccolo.engine.base import Batch, Engine
 from piccolo.engine.exceptions import TransactionError
 from piccolo.query.base import DDL, Query
-from piccolo.query.methods.objects import Create, GetOrCreate
 from piccolo.querystring import QueryString
 from piccolo.utils.encoding import dump_json, load_json
 from piccolo.utils.lazy_loader import LazyLoader
 from piccolo.utils.sync import run_sync
 
 aiosqlite = LazyLoader("aiosqlite", globals(), "aiosqlite")
 
@@ -274,14 +273,16 @@
         self.transaction_type = transaction_type
         self.queries: t.List[Query] = []
 
     def add(self, *query: Query):
         self.queries += list(query)
 
     async def run(self):
+        from piccolo.query.methods.objects import Create, GetOrCreate
+
         try:
             async with self.engine.transaction(
                 transaction_type=self.transaction_type
             ):
                 for query in self.queries:
                     if isinstance(query, (Query, DDL, Create, GetOrCreate)):
                         await query.run()
@@ -298,60 +299,141 @@
     def __await__(self):
         return self.run().__await__()
 
 
 ###############################################################################
 
 
+class Savepoint:
+    def __init__(self, name: str, transaction: SQLiteTransaction):
+        self.name = name
+        self.transaction = transaction
+
+    async def rollback_to(self):
+        await self.transaction.connection.execute(
+            f"ROLLBACK TO SAVEPOINT {self.name}"
+        )
+
+    async def release(self):
+        await self.transaction.connection.execute(
+            f"RELEASE SAVEPOINT {self.name}"
+        )
+
+
 class SQLiteTransaction:
     """
     Used for wrapping queries in a transaction, using a context manager.
     Currently it's async only.
 
     Usage::
 
         async with engine.transaction():
             # Run some queries:
             await Band.select().run()
 
     """
 
-    __slots__ = ("engine", "context", "connection", "transaction_type")
+    __slots__ = (
+        "engine",
+        "context",
+        "connection",
+        "transaction_type",
+        "allow_nested",
+        "_savepoint_id",
+        "_parent",
+        "_committed",
+        "_rolled_back",
+    )
 
     def __init__(
         self,
         engine: SQLiteEngine,
         transaction_type: TransactionType = TransactionType.deferred,
+        allow_nested: bool = True,
     ):
         """
         :param transaction_type:
             If your transaction just contains ``SELECT`` queries, then use
             ``TransactionType.deferred``. This will give you the best
             performance. When performing ``INSERT``, ``UPDATE``, ``DELETE``
             queries, we recommend using ``TransactionType.immediate`` to
             avoid database locks.
         """
         self.engine = engine
         self.transaction_type = transaction_type
-        if self.engine.current_transaction.get():
-            raise TransactionError(
-                "A transaction is already active - nested transactions aren't "
-                "currently supported."
-            )
+        current_transaction = self.engine.current_transaction.get()
 
-    async def __aenter__(self):
-        self.connection = await self.engine.get_connection()
-        await self.connection.execute(f"BEGIN {self.transaction_type.value}")
+        self._savepoint_id = 0
+        self._parent = None
+        self._committed = False
+        self._rolled_back = False
+
+        if current_transaction:
+            if allow_nested:
+                self._parent = current_transaction
+            else:
+                raise TransactionError(
+                    "A transaction is already active - nested transactions "
+                    "aren't allowed."
+                )
+
+    async def __aenter__(self) -> SQLiteTransaction:
+        if self._parent is not None:
+            return self._parent
+
+        self.connection = await self.get_connection()
+        await self.begin()
         self.context = self.engine.current_transaction.set(self)
+        return self
+
+    async def get_connection(self):
+        return await self.engine.get_connection()
+
+    async def begin(self):
+        await self.connection.execute(f"BEGIN {self.transaction_type.value}")
+
+    async def commit(self):
+        await self.connection.execute("COMMIT")
+        self._committed = True
+
+    async def rollback(self):
+        await self.connection.execute("ROLLBACK")
+        self._rolled_back = True
+
+    async def rollback_to(self, savepoint_name: str):
+        """
+        Used to rollback to a savepoint just using the name.
+        """
+        await Savepoint(name=savepoint_name, transaction=self).rollback_to()
+
+    ###########################################################################
+
+    def get_savepoint_id(self) -> int:
+        self._savepoint_id += 1
+        return self._savepoint_id
+
+    async def savepoint(self, name: t.Optional[str] = None) -> Savepoint:
+        name = name or f"savepoint_{self.get_savepoint_id()}"
+        await self.connection.execute(f"SAVEPOINT {name}")
+        return Savepoint(name=name, transaction=self)
+
+    ###########################################################################
 
     async def __aexit__(self, exception_type, exception, traceback):
+        if self._parent:
+            return exception is None
+
         if exception:
-            await self.connection.execute("ROLLBACK")
+            # The user may have manually rolled it back.
+            if not self._rolled_back:
+                await self.rollback()
         else:
-            await self.connection.execute("COMMIT")
+            # The user may have manually committed it.
+            if not self._committed and not self._rolled_back:
+                await self.commit()
 
         await self.connection.close()
         self.engine.current_transaction.reset(self.context)
 
         return exception is None
 
 
@@ -360,32 +442,41 @@
 
 def dict_factory(cursor, row) -> t.Dict:
     return {col[0]: row[idx] for idx, col in enumerate(cursor.description)}
 
 
 class SQLiteEngine(Engine[t.Optional[SQLiteTransaction]]):
 
-    __slots__ = ("connection_kwargs", "current_transaction", "log_queries")
+    __slots__ = (
+        "connection_kwargs",
+        "current_transaction",
+        "log_queries",
+        "log_responses",
+    )
 
     engine_type = "sqlite"
     min_version_number = 3.25
 
     def __init__(
         self,
         path: str = "piccolo.sqlite",
         log_queries: bool = False,
+        log_responses: bool = False,
         **connection_kwargs,
     ) -> None:
         """
         :param path:
             A relative or absolute path to the the SQLite database file (it
             will be created if it doesn't already exist).
         :param log_queries:
             If ``True``, all SQL and DDL statements are printed out before
             being run. Useful for debugging.
+        :param log_responses:
+            If ``True``, the raw response from each query is printed out.
+            Useful for debugging.
         :param connection_kwargs:
             These are passed directly to the database adapter. We recommend
             setting ``timeout`` if you expect your application to process a
             large number of concurrent writes, to prevent queries timing out.
             See Python's `sqlite3 docs <https://docs.python.org/3/library/sqlite3.html#sqlite3.connect>`_
             for more info.
 
@@ -393,14 +484,15 @@
         default_connection_kwargs = {
             "database": path,
             "detect_types": sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
             "isolation_level": None,
         }
 
         self.log_queries = log_queries
+        self.log_responses = log_responses
         self.connection_kwargs = {
             **default_connection_kwargs,
             **connection_kwargs,
         }
 
         self.current_transaction = contextvars.ContextVar(
             f"sqlite_current_transaction_{path}", default=None
@@ -543,66 +635,84 @@
     async def run_querystring(
         self, querystring: QueryString, in_pool: bool = False
     ):
         """
         Connection pools aren't currently supported - the argument is there
         for consistency with other engines.
         """
+        query_id = self.get_query_id()
+
         if self.log_queries:
-            print(querystring)
+            self.print_query(query_id=query_id, query=querystring.__str__())
 
         query, query_args = querystring.compile_string(
             engine_type=self.engine_type
         )
 
         # If running inside a transaction:
         current_transaction = self.current_transaction.get()
         if current_transaction:
-            return await self._run_in_existing_connection(
+            response = await self._run_in_existing_connection(
                 connection=current_transaction.connection,
                 query=query,
                 args=query_args,
                 query_type=querystring.query_type,
                 table=querystring.table,
             )
+        else:
+            response = await self._run_in_new_connection(
+                query=query,
+                args=query_args,
+                query_type=querystring.query_type,
+                table=querystring.table,
+            )
 
-        return await self._run_in_new_connection(
-            query=query,
-            args=query_args,
-            query_type=querystring.query_type,
-            table=querystring.table,
-        )
+        if self.log_responses:
+            self.print_response(query_id=query_id, response=response)
+
+        return response
 
     async def run_ddl(self, ddl: str, in_pool: bool = False):
         """
         Connection pools aren't currently supported - the argument is there
         for consistency with other engines.
         """
+        query_id = self.get_query_id()
+
         if self.log_queries:
-            print(ddl)
+            self.print_query(query_id=query_id, query=ddl)
 
         # If running inside a transaction:
         current_transaction = self.current_transaction.get()
         if current_transaction:
-            return await self._run_in_existing_connection(
+            response = await self._run_in_existing_connection(
                 connection=current_transaction.connection,
                 query=ddl,
             )
+        else:
+            response = await self._run_in_new_connection(
+                query=ddl,
+            )
 
-        return await self._run_in_new_connection(
-            query=ddl,
-        )
+        if self.log_responses:
+            self.print_response(query_id=query_id, response=response)
+
+        return response
 
     def atomic(
         self, transaction_type: TransactionType = TransactionType.deferred
     ) -> Atomic:
         return Atomic(engine=self, transaction_type=transaction_type)
 
     def transaction(
-        self, transaction_type: TransactionType = TransactionType.deferred
+        self,
+        transaction_type: TransactionType = TransactionType.deferred,
+        allow_nested: bool = True,
     ) -> SQLiteTransaction:
         """
         Create a new database transaction. See :class:`Transaction`.
         """
         return SQLiteTransaction(
-            engine=self, transaction_type=transaction_type
+            engine=self,
+            transaction_type=transaction_type,
+            allow_nested=allow_nested,
         )
```

### Comparing `piccolo-0.99.0/piccolo/main.py` & `piccolo-1.0a1/piccolo/main.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/query/base.py` & `piccolo-1.0a1/piccolo/query/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from __future__ import annotations
 
-import itertools
 import typing as t
 from time import time
 
 from piccolo.columns.column_types import JSON, JSONB
-from piccolo.query.mixins import CallbackType, ColumnsDelegate
+from piccolo.custom_types import QueryResponseType, TableInstance
+from piccolo.query.mixins import ColumnsDelegate
 from piccolo.querystring import QueryString
-from piccolo.utils.encoding import dump_json, load_json
+from piccolo.utils.encoding import load_json
 from piccolo.utils.objects import make_nested_object
 from piccolo.utils.sync import run_sync
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from piccolo.query.mixins import CallbackDelegate, OutputDelegate
+    from piccolo.query.mixins import OutputDelegate
     from piccolo.table import Table  # noqa
 
 
 class Timer:
     def __enter__(self):
         self.start = time()
 
     def __exit__(self, exception_type, exception, traceback):
         self.end = time()
         print(f"Duration: {self.end - self.start}s")
 
 
-class Query:
+class Query(t.Generic[TableInstance, QueryResponseType]):
 
     __slots__ = ("table", "_frozen_querystrings")
 
     def __init__(
         self,
-        table: t.Type[Table],
+        table: t.Type[TableInstance],
         frozen_querystrings: t.Optional[t.Sequence[QueryString]] = None,
     ):
         self.table = table
         self._frozen_querystrings = frozen_querystrings
 
     @property
     def engine_type(self) -> str:
         engine = self.table._meta.db
         if engine:
             return engine.engine_type
         else:
             raise ValueError("Engine isn't defined.")
 
-    async def _process_results(self, results):  # noqa: C901
+    async def _process_results(self, results):
         if results:
             keys = results[0].keys()
             keys = [i.replace("$", ".") for i in keys]
             if self.engine_type in ("postgres", "cockroach"):
                 # asyncpg returns a special Record object. We can pass it
                 # directly into zip without calling `values` on it. This can
                 # save us hundreds of microseconds, depending on the number of
@@ -113,62 +113,42 @@
 
         #######################################################################
 
         raw = await self.response_handler(raw)
 
         if output:
             if output._output.as_objects:
-                # When using .first() we get a single row, not a list
-                # of rows.
-                if type(raw) is list:
-                    if output._output.nested:
-                        raw = [
-                            make_nested_object(row, self.table) for row in raw
-                        ]
-                    else:
-                        raw = [
-                            self.table(**columns, _exists_in_db=True)
-                            for columns in raw
-                        ]
-                elif raw is not None:
-                    if output._output.nested:
-                        raw = make_nested_object(raw, self.table)
-                    else:
-                        raw = self.table(**raw, _exists_in_db=True)
-            elif type(raw) is list:
-                if output._output.as_list:
-                    if len(raw) == 0:
-                        return []
-                    if len(raw[0].keys()) != 1:
-                        raise ValueError(
-                            "Each row returned more than one value"
-                        )
-                    else:
-                        raw = list(itertools.chain(*[j.values() for j in raw]))
-                if output._output.as_json:
-                    raw = dump_json(raw)
+                if output._output.nested:
+                    raw = [make_nested_object(row, self.table) for row in raw]
+                else:
+                    raw = [
+                        self.table(**columns, _exists_in_db=True)
+                        for columns in raw
+                    ]
 
         return raw
 
     def _validate(self):
         """
         Override in any subclasses if validation needs to be run before
         executing a query - for example, warning a user if they're about to
         delete all the data from a table.
         """
         pass
 
-    def __await__(self):
+    def __await__(self) -> t.Generator[None, None, QueryResponseType]:
         """
         If the user doesn't explicity call .run(), proxy to it as a
         convenience.
         """
         return self.run().__await__()
 
-    async def run(self, node: t.Optional[str] = None, in_pool: bool = True):
+    async def _run(
+        self, node: t.Optional[str] = None, in_pool: bool = True
+    ) -> QueryResponseType:
         """
         Run the query on the database.
 
         :param node:
             If specified, run this query against another database node. Only
             available in Postgres. See :class:`PostgresEngine <piccolo.engine.postgres.PostgresEngine>`.
         :param in_pool:
@@ -191,61 +171,55 @@
             from piccolo.engine.postgres import PostgresEngine
 
             if isinstance(engine, PostgresEngine):
                 engine = engine.extra_nodes[node]
 
         querystrings = self.querystrings
 
-        callback: t.Optional[CallbackDelegate] = getattr(
-            self, "callback_delegate", None
-        )
-
         if len(querystrings) == 1:
             results = await engine.run_querystring(
                 querystrings[0], in_pool=in_pool
             )
-            processed_results = await self._process_results(results)
-
-            if callback:
-                processed_results = await callback.invoke(
-                    processed_results, kind=CallbackType.success
-                )
-
-            return processed_results
+            return await self._process_results(results)
         else:
             responses = []
             for querystring in querystrings:
                 results = await engine.run_querystring(
                     querystring, in_pool=in_pool
                 )
                 processed_results = await self._process_results(results)
 
-                if callback:
-                    processed_results = await callback.invoke(
-                        processed_results, kind=CallbackType.success
-                    )
-
                 responses.append(processed_results)
-            return responses
+            return t.cast(QueryResponseType, responses)
 
-    def run_sync(self, timed=False, in_pool=False, *args, **kwargs):
+    async def run(
+        self, node: t.Optional[str] = None, in_pool: bool = True
+    ) -> QueryResponseType:
+        return await self._run(node=node, in_pool=in_pool)
+
+    def run_sync(
+        self,
+        node: t.Optional[str] = None,
+        timed: bool = False,
+        in_pool: bool = False,
+    ) -> QueryResponseType:
         """
         A convenience method for running the coroutine synchronously.
 
         :param timed:
             If ``True``, the time taken to run the query is printed out. Useful
             for debugging.
         :param in_pool:
             Whether to run this in a connection pool if one is available. Set
             to ``False`` by default, because if an app uses ``run`` and
             ``run_sync`` in the same app, it can cause errors. See
             `issue 505 <https://github.com/piccolo-orm/piccolo/issues/505>`_.
 
         """
-        coroutine = self.run(in_pool=in_pool, *args, **kwargs)
+        coroutine = self.run(node=node, in_pool=in_pool)
 
         if not timed:
             return run_sync(coroutine)
         with Timer():
             return run_sync(coroutine)
 
     async def response_handler(self, response):
@@ -362,14 +336,17 @@
 
     ###########################################################################
 
     def __str__(self) -> str:
         return "; ".join([i.__str__() for i in self.querystrings])
 
 
+###############################################################################
+
+
 class FrozenQuery:
     def __init__(self, query: Query):
         self.query = query
 
     async def run(self, *args, **kwargs):
         return await self.query.run(*args, **kwargs)
 
@@ -385,14 +362,17 @@
         else:
             raise AttributeError("Unrecognised attribute name.")
 
     def __str__(self) -> str:
         return self.query.__str__()
 
 
+###############################################################################
+
+
 class DDL:
 
     __slots__ = ("table",)
 
     def __init__(self, table: t.Type[Table], **kwargs):
         self.table = table
 
@@ -460,15 +440,14 @@
                 f"Table {self.table._meta.tablename} has no db defined in "
                 "_meta"
             )
 
         if len(self.ddl) == 1:
             return await engine.run_ddl(self.ddl[0], in_pool=in_pool)
         responses = []
-        # TODO - run in a transaction
         for ddl in self.ddl:
             response = await engine.run_ddl(ddl, in_pool=in_pool)
             responses.append(response)
         return responses
 
     def run_sync(self, timed=False, *args, **kwargs):
         """
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/alter.py` & `piccolo-1.0a1/piccolo/query/methods/alter.py`

 * *Files 9% similar despite different names*

```diff
@@ -236,27 +236,38 @@
         return (
             f'ALTER COLUMN "{self.column_name}" TYPE '
             f"{self.column_type}({precision}, {scale})"
         )
 
 
 @dataclass
+class SetSchema(AlterStatement):
+    __slots__ = ("schema_name",)
+
+    schema_name: str
+
+    @property
+    def ddl(self) -> str:
+        return f'SET SCHEMA "{self.schema_name}"'
+
+
+@dataclass
 class DropTable:
-    tablename: str
+    table: t.Type[Table]
     cascade: bool
     if_exists: bool
 
     @property
     def ddl(self) -> str:
         query = "DROP TABLE"
 
         if self.if_exists:
             query += " IF EXISTS"
 
-        query += f" {self.tablename}"
+        query += f" {self.table._meta.get_formatted_tablename()}"
 
         if self.cascade:
             query += " CASCADE"
 
         return query
 
 
@@ -271,14 +282,15 @@
         "_rename_columns",
         "_rename_table",
         "_set_column_type",
         "_set_default",
         "_set_digits",
         "_set_length",
         "_set_null",
+        "_set_schema",
         "_set_unique",
     )
 
     def __init__(self, table: t.Type[Table], **kwargs):
         super().__init__(table, **kwargs)
         self._add_foreign_key_constraint: t.List[AddForeignKeyConstraint] = []
         self._add: t.List[AddColumn] = []
@@ -289,129 +301,174 @@
         self._rename_columns: t.List[RenameColumn] = []
         self._rename_table: t.List[RenameTable] = []
         self._set_column_type: t.List[SetColumnType] = []
         self._set_default: t.List[SetDefault] = []
         self._set_digits: t.List[SetDigits] = []
         self._set_length: t.List[SetLength] = []
         self._set_null: t.List[SetNull] = []
+        self._set_schema: t.List[SetSchema] = []
         self._set_unique: t.List[SetUnique] = []
 
-    def add_column(self, name: str, column: Column) -> Alter:
+    def add_column(self: Self, name: str, column: Column) -> Self:
         """
-        Band.alter().add_column(‘members’, Integer())
+        Add a column to the table::
+
+            >>> await Band.alter().add_column('members', Integer())
+
         """
         column._meta._table = self.table
         column._meta._name = name
         column._meta.db_column_name = name
 
         if isinstance(column, ForeignKey):
             column._setup(table_class=self.table)
 
         self._add.append(AddColumn(column, name))
         return self
 
     def drop_column(self, column: t.Union[str, Column]) -> Alter:
         """
-        Band.alter().drop_column(Band.popularity)
+        Drop a column from the table::
+
+            >>> await Band.alter().drop_column(Band.popularity)
+
         """
         self._drop.append(DropColumn(column))
         return self
 
     def drop_default(self, column: t.Union[str, Column]) -> Alter:
         """
-        Band.alter().drop_default(Band.popularity)
+        Drop the default from a column::
+
+            >>> await Band.alter().drop_default(Band.popularity)
+
         """
         self._drop_default.append(DropDefault(column=column))
         return self
 
     def drop_table(
         self, cascade: bool = False, if_exists: bool = False
     ) -> Alter:
         """
-        Band.alter().drop_table()
+        Drop the table::
+
+            >>> await Band.alter().drop_table()
+
         """
         self._drop_table = DropTable(
-            tablename=self.table._meta.tablename,
+            table=self.table,
             cascade=cascade,
             if_exists=if_exists,
         )
         return self
 
     def rename_table(self, new_name: str) -> Alter:
         """
-        Band.alter().rename_table('musical_group')
+        Rename the table::
+
+            >>> await Band.alter().rename_table('musical_group')
+
         """
         # We override the existing one rather than appending.
         self._rename_table = [RenameTable(new_name=new_name)]
         return self
 
     def rename_column(
         self, column: t.Union[str, Column], new_name: str
     ) -> Alter:
         """
-        Band.alter().rename_column(Band.popularity, ‘rating’)
-        Band.alter().rename_column('popularity', ‘rating’)
+        Rename a column on the table::
+
+            # Specify the column with a `Column` instance:
+            >>> await Band.alter().rename_column(Band.popularity, 'rating')
+
+            # Or by name:
+            >>> await Band.alter().rename_column('popularity', 'rating')
+
         """
         self._rename_columns.append(RenameColumn(column, new_name))
         return self
 
     def set_column_type(
         self,
         old_column: Column,
         new_column: Column,
         using_expression: t.Optional[str] = None,
     ) -> Alter:
         """
-        Change the type of a column.
+        Change the type of a column::
+
+            >>> await Band.alter().set_column_type(Band.popularity, BigInt())
+
+        :param using_expression:
+            When changing a column's type, the database doesn't always know how
+            to convert the existing data in that column to the new type. You
+            can provide a hint to the database on what to do. For example
+            ``'name::integer'``.
+
         """
         self._set_column_type.append(
             SetColumnType(
                 old_column=old_column,
                 new_column=new_column,
                 using_expression=using_expression,
             )
         )
         return self
 
     def set_default(self, column: Column, value: t.Any) -> Alter:
         """
-        Set the default for a column.
+        Set the default for a column::
+
+            >>> await Band.alter().set_default(Band.popularity, 0)
 
-        Band.alter().set_default(Band.popularity, 0)
         """
         self._set_default.append(SetDefault(column=column, value=value))
         return self
 
     def set_null(
         self, column: t.Union[str, Column], boolean: bool = True
     ) -> Alter:
         """
-        Band.alter().set_null(Band.name, True)
-        Band.alter().set_null('name', True)
+        Change a column to be nullable or not::
+
+            # Specify the column using a `Column` instance:
+            >>> await Band.alter().set_null(Band.name, True)
+
+            # Or using a string:
+            >>> await Band.alter().set_null('name', True)
+
         """
         self._set_null.append(SetNull(column, boolean))
         return self
 
     def set_unique(
         self, column: t.Union[str, Column], boolean: bool = True
     ) -> Alter:
         """
-        Band.alter().set_unique(Band.name, True)
-        Band.alter().set_unique('name', True)
+        Make a column unique or not::
+
+            # Specify the column using a `Column` instance:
+            >>> await Band.alter().set_unique(Band.name, True)
+
+            # Or using a string:
+            >>> await Band.alter().set_unique('name', True)
+
         """
         self._set_unique.append(SetUnique(column, boolean))
         return self
 
     def set_length(self, column: t.Union[str, Varchar], length: int) -> Alter:
         """
         Change the max length of a varchar column. Unfortunately, this isn't
         supported by SQLite, but SQLite also doesn't enforce any length limits
-        on varchar columns anyway.
+        on varchar columns anyway::
+
+            >>> await Band.alter().set_length('name', 512)
 
-        Band.alter().set_length('name', 512)
         """
         if self.engine_type == "sqlite":
             colored_warning(
                 (
                     "SQLITE doesn't support changes in length. It also "
                     "doesn't enforce any length limits, so your code will "
                     "still work as expected. Skipping."
@@ -450,21 +507,22 @@
         column: t.Union[str, ForeignKey],
         referenced_table_name: str,
         on_delete: t.Optional[OnDelete] = None,
         on_update: t.Optional[OnUpdate] = None,
         referenced_column_name: str = "id",
     ) -> Alter:
         """
-        This will add a new foreign key constraint.
+        Add a new foreign key constraint::
+
+            >>> await Band.alter().add_foreign_key_constraint(
+            ...     Band.manager,
+            ...     referenced_table_name='manager',
+            ...     on_delete=OnDelete.cascade
+            ... )
 
-        Band.alter().add_foreign_key_constraint(
-            Band.manager,
-            referenced_table_name='manager',
-            on_delete=OnDelete.cascade
-        )
         """
         constraint_name = self._get_constraint_name(column=column)
         column_name = AlterColumnStatement(column=column).column_name
 
         self._add_foreign_key_constraint.append(
             AddForeignKeyConstraint(
                 constraint_name=constraint_name,
@@ -479,15 +537,15 @@
 
     def set_digits(
         self,
         column: t.Union[str, Numeric],
         digits: t.Optional[t.Tuple[int, int]],
     ) -> Alter:
         """
-        Alter the precision and scale for a Numeric column.
+        Alter the precision and scale for a ``Numeric`` column.
         """
         column_type = (
             column.__class__.__name__.upper()
             if isinstance(column, Numeric)
             else "NUMERIC"
         )
         self._set_digits.append(
@@ -495,20 +553,31 @@
                 digits=digits,
                 column=column,
                 column_type=column_type,
             )
         )
         return self
 
+    def set_schema(self, schema_name: str) -> Alter:
+        """
+        Move the table to a different schema.
+
+        :param schema_name:
+            The schema to move the table to.
+
+        """
+        self._set_schema.append(SetSchema(schema_name=schema_name))
+        return self
+
     @property
     def default_ddl(self) -> t.Sequence[str]:
         if self._drop_table is not None:
             return [self._drop_table.ddl]
 
-        query = f"ALTER TABLE {self.table._meta.tablename}"
+        query = f"ALTER TABLE {self.table._meta.get_formatted_tablename()}"
 
         alterations = [
             i.ddl
             for i in itertools.chain(
                 self._add,
                 self._rename_columns,
                 self._rename_table,
@@ -516,18 +585,22 @@
                 self._drop_default,
                 self._set_column_type,
                 self._set_unique,
                 self._set_null,
                 self._set_length,
                 self._set_default,
                 self._set_digits,
+                self._set_schema,
             )
         ]
 
         if self.engine_type == "sqlite":
             # Can only perform one alter statement at a time.
             return [f"{query} {i}" for i in alterations]
 
         # Postgres can perform them all at once:
         query += ",".join(f" {i}" for i in alterations)
 
         return [query]
+
+
+Self = t.TypeVar("Self", bound=Alter)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/count.py` & `piccolo-1.0a1/piccolo/query/methods/count.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,61 @@
 from __future__ import annotations
 
 import typing as t
 
 from piccolo.custom_types import Combinable
 from piccolo.query.base import Query
+from piccolo.query.methods.select import Count as SelectCount
 from piccolo.query.mixins import WhereDelegate
 from piccolo.querystring import QueryString
 
-from .select import Select
-
 if t.TYPE_CHECKING:  # pragma: no cover
+    from piccolo.columns import Column
     from piccolo.table import Table
 
 
 class Count(Query):
-    __slots__ = ("where_delegate",)
 
-    def __init__(self, table: t.Type[Table], **kwargs):
+    __slots__ = ("where_delegate", "column", "_distinct")
+
+    def __init__(
+        self,
+        table: t.Type[Table],
+        column: t.Optional[Column] = None,
+        distinct: t.Optional[t.Sequence[Column]] = None,
+        **kwargs,
+    ):
         super().__init__(table, **kwargs)
+        self.column = column
+        self._distinct = distinct
         self.where_delegate = WhereDelegate()
 
-    def where(self, *where: Combinable) -> Count:
+    ###########################################################################
+    # Clauses
+
+    def where(self: Self, *where: Combinable) -> Self:
         self.where_delegate.where(*where)
         return self
 
+    def distinct(self: Self, columns: t.Optional[t.Sequence[Column]]) -> Self:
+        self._distinct = columns
+        return self
+
+    ###########################################################################
+
     async def response_handler(self, response) -> bool:
         return response[0]["count"]
 
     @property
     def default_querystrings(self) -> t.Sequence[QueryString]:
-        select = Select(self.table)
-        select.where_delegate._where = self.where_delegate._where
-        return [
-            QueryString(
-                'SELECT COUNT(*) AS "count" FROM ({}) AS "subquery"',
-                select.querystrings[0],
-            )
-        ]
+        table: t.Type[Table] = self.table
+
+        query = table.select(
+            SelectCount(column=self.column, distinct=self._distinct)
+        )
+
+        query.where_delegate._where = self.where_delegate._where
+
+        return query.querystrings
+
+
+Self = t.TypeVar("Self", bound=Count)
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/create.py` & `piccolo-1.0a1/piccolo/query/methods/create.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,48 +10,81 @@
 
 
 class Create(DDL):
     """
     Creates a database table.
     """
 
-    __slots__ = ("if_not_exists", "only_default_columns")
+    __slots__ = ("if_not_exists", "only_default_columns", "auto_create_schema")
 
     def __init__(
         self,
         table: t.Type[Table],
         if_not_exists: bool = False,
         only_default_columns: bool = False,
+        auto_create_schema: bool = True,
         **kwargs,
     ):
+        """
+        :param table:
+            The table to create.
+        :param if_not_exists:
+            If ``True``, no error will be raised if this table already exists.
+        :param only_default_columns:
+            If ``True``, just the basic table and default primary key are
+            created, rather than all columns. Not typically needed.
+        :param auto_create_schema:
+            If the table belongs to a database schema, then make sure the
+            schema exists before creating the table.
+
+        """
         super().__init__(table, **kwargs)
         self.if_not_exists = if_not_exists
         self.only_default_columns = only_default_columns
+        self.auto_create_schema = auto_create_schema
 
     @property
     def default_ddl(self) -> t.Sequence[str]:
+        ddl: t.List[str] = []
+
+        schema_name = self.table._meta.schema
+        if (
+            self.auto_create_schema
+            and schema_name is not None
+            and schema_name != "public"
+            and self.engine_type != "sqlite"
+        ):
+            from piccolo.schema import CreateSchema
+
+            ddl.append(
+                CreateSchema(
+                    schema_name=schema_name,
+                    if_not_exists=True,
+                    db=self.table._meta.db,
+                ).ddl
+            )
+
         prefix = "CREATE TABLE"
         if self.if_not_exists:
             prefix += " IF NOT EXISTS"
 
         if self.only_default_columns:
             columns = self.table._meta.non_default_columns
         else:
             columns = self.table._meta.columns
 
-        base = f"{prefix} {self.table._meta.tablename}"
+        base = f"{prefix} {self.table._meta.get_formatted_tablename()}"
         columns_sql = ", ".join(i.ddl for i in columns)
-        create_table_ddl = f"{base} ({columns_sql})"
+        ddl.append(f"{base} ({columns_sql})")
 
-        create_indexes: t.List[str] = []
         for column in columns:
             if column._meta.index is True:
-                create_indexes.extend(
+                ddl.extend(
                     CreateIndex(
                         table=self.table,
                         columns=[column],
                         method=column._meta.index_method,
                         if_not_exists=self.if_not_exists,
                     ).ddl
                 )
 
-        return [create_table_ddl] + create_indexes
+        return ddl
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/create_index.py` & `piccolo-1.0a1/piccolo/query/methods/create_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,43 +38,33 @@
             prefix += " IF NOT EXISTS"
         return prefix
 
     @property
     def postgres_ddl(self) -> t.Sequence[str]:
         column_names = self.column_names
         index_name = self.table._get_index_name(column_names)
-        tablename = self.table._meta.tablename
+        tablename = self.table._meta.get_formatted_tablename()
         method_name = self.method.value
         column_names_str = ", ".join([f'"{i}"' for i in self.column_names])
         return [
             (
                 f"{self.prefix} {index_name} ON {tablename} USING "
                 f"{method_name} ({column_names_str})"
             )
         ]
 
     @property
     def cockroach_ddl(self) -> t.Sequence[str]:
-        column_names = self.column_names
-        index_name = self.table._get_index_name(column_names)
-        tablename = self.table._meta.tablename
-        method_name = self.method.value
-        column_names_str = ", ".join([f'"{i}"' for i in self.column_names])
-        return [
-            (
-                f"{self.prefix} {index_name} ON {tablename} USING "
-                f"{method_name} ({column_names_str})"
-            )
-        ]
+        return self.postgres_ddl
 
     @property
     def sqlite_ddl(self) -> t.Sequence[str]:
         column_names = self.column_names
         index_name = self.table._get_index_name(column_names)
-        tablename = self.table._meta.tablename
+        tablename = self.table._meta.get_formatted_tablename()
 
         method_name = self.method.value
         if method_name != "btree":
             raise ValueError("SQLite only support btree indexes.")
 
         column_names_str = ", ".join([f'"{i}"' for i in self.column_names])
         return [
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/delete.py` & `piccolo-1.0a1/piccolo/query/methods/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
     def __init__(self, table: t.Type[Table], force: bool = False, **kwargs):
         super().__init__(table, **kwargs)
         self.force = force
         self.returning_delegate = ReturningDelegate()
         self.where_delegate = WhereDelegate()
 
-    def where(self, *where: Combinable) -> Delete:
+    def where(self: Self, *where: Combinable) -> Self:
         self.where_delegate.where(*where)
         return self
 
-    def returning(self, *columns: Column) -> Delete:
+    def returning(self: Self, *columns: Column) -> Self:
         self.returning_delegate.returning(columns)
         return self
 
     def _validate(self):
         """
         Don't let a deletion happen unless it has a where clause, or is
         explicitly forced.
@@ -49,15 +49,15 @@
                 "Do you really want to delete all the data from "
                 f"{classname}? If so, use {classname}.delete(force=True). "
                 "Otherwise, add a where clause."
             )
 
     @property
     def default_querystrings(self) -> t.Sequence[QueryString]:
-        query = f"DELETE FROM {self.table._meta.tablename}"
+        query = f"DELETE FROM {self.table._meta.get_formatted_tablename()}"
 
         querystring = QueryString(query)
 
         if self.where_delegate._where:
             querystring = QueryString(
                 "{} WHERE {}",
                 querystring,
@@ -68,7 +68,10 @@
             querystring = QueryString(
                 "{}{}",
                 querystring,
                 self.returning_delegate._returning.querystring,
             )
 
         return [querystring]
+
+
+Self = t.TypeVar("Self", bound=Delete)
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/drop_index.py` & `piccolo-1.0a1/piccolo/query/methods/drop_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/query/methods/exists.py` & `piccolo-1.0a1/piccolo/query/methods/exists.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from __future__ import annotations
 
 import typing as t
 
-from piccolo.custom_types import Combinable
+from piccolo.custom_types import Combinable, TableInstance
 from piccolo.query.base import Query
 from piccolo.query.methods.select import Select
 from piccolo.query.mixins import WhereDelegate
 from piccolo.querystring import QueryString
 
-if t.TYPE_CHECKING:  # pragma: no cover
-    from piccolo.table import Table
 
-
-class Exists(Query):
+class Exists(Query[TableInstance, bool]):
     __slots__ = ("where_delegate",)
 
-    def __init__(self, table: t.Type[Table], **kwargs):
+    def __init__(self, table: t.Type[TableInstance], **kwargs):
         super().__init__(table, **kwargs)
         self.where_delegate = WhereDelegate()
 
-    def where(self, *where: Combinable) -> Exists:
+    def where(self: Self, *where: Combinable) -> Self:
         self.where_delegate.where(*where)
         return self
 
     async def response_handler(self, response) -> bool:
         # Convert to a bool - postgres returns True, and sqlite return 1.
         return bool(response[0]["exists"])
 
@@ -32,7 +29,10 @@
         select = Select(table=self.table)
         select.where_delegate._where = self.where_delegate._where
         return [
             QueryString(
                 'SELECT EXISTS({}) AS "exists"', select.querystrings[0]
             )
         ]
+
+
+Self = t.TypeVar("Self", bound=Exists)
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/insert.py` & `piccolo-1.0a1/piccolo/query/methods/insert.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,88 @@
 from __future__ import annotations
 
 import typing as t
 
+from piccolo.custom_types import Combinable, TableInstance
 from piccolo.query.base import Query
-from piccolo.query.mixins import AddDelegate, ReturningDelegate
+from piccolo.query.mixins import (
+    AddDelegate,
+    OnConflictAction,
+    OnConflictDelegate,
+    ReturningDelegate,
+)
 from piccolo.querystring import QueryString
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.columns.base import Column
     from piccolo.table import Table
 
 
-class Insert(Query):
-    __slots__ = ("add_delegate", "returning_delegate")
-
-    def __init__(self, table: t.Type[Table], *instances: Table, **kwargs):
+class Insert(
+    t.Generic[TableInstance], Query[TableInstance, t.List[t.Dict[str, t.Any]]]
+):
+    __slots__ = ("add_delegate", "on_conflict_delegate", "returning_delegate")
+
+    def __init__(
+        self, table: t.Type[TableInstance], *instances: TableInstance, **kwargs
+    ):
         super().__init__(table, **kwargs)
         self.add_delegate = AddDelegate()
         self.returning_delegate = ReturningDelegate()
+        self.on_conflict_delegate = OnConflictDelegate()
         self.add(*instances)
 
     ###########################################################################
     # Clauses
 
-    def add(self, *instances: Table) -> Insert:
+    def add(self: Self, *instances: Table) -> Self:
         self.add_delegate.add(*instances, table_class=self.table)
         return self
 
-    def returning(self, *columns: Column) -> Insert:
+    def returning(self: Self, *columns: Column) -> Self:
         self.returning_delegate.returning(columns)
         return self
 
+    def on_conflict(
+        self: Self,
+        target: t.Optional[t.Union[str, Column, t.Tuple[Column, ...]]] = None,
+        action: t.Union[
+            OnConflictAction, t.Literal["DO NOTHING", "DO UPDATE"]
+        ] = OnConflictAction.do_nothing,
+        values: t.Optional[
+            t.Sequence[t.Union[Column, t.Tuple[Column, t.Any]]]
+        ] = None,
+        where: t.Optional[Combinable] = None,
+    ) -> Self:
+        if (
+            self.engine_type == "sqlite"
+            and self.table._meta.db.get_version_sync() < 3.24
+        ):
+            raise NotImplementedError(
+                "SQLite versions lower than 3.24 don't support ON CONFLICT"
+            )
+
+        if (
+            self.engine_type in ("postgres", "cockroach")
+            and len(self.on_conflict_delegate._on_conflict.on_conflict_items)
+            == 1
+        ):
+            raise NotImplementedError(
+                "Postgres and Cockroach only support a single ON CONFLICT "
+                "clause."
+            )
+
+        self.on_conflict_delegate.on_conflict(
+            target=target,
+            action=action,
+            values=values,
+            where=where,
+        )
+        return self
+
     ###########################################################################
 
     def _raw_response_callback(self, results):
         """
         Assign the ids of the created rows to the model instances.
         """
         for index, row in enumerate(results):
@@ -46,38 +94,52 @@
                     self.table._meta.primary_key._meta.db_column_name, None
                 ),
             )
             table_instance._exists_in_db = True
 
     @property
     def default_querystrings(self) -> t.Sequence[QueryString]:
-        base = f'INSERT INTO "{self.table._meta.tablename}"'
+        base = f"INSERT INTO {self.table._meta.get_formatted_tablename()}"
         columns = ",".join(
             f'"{i._meta.db_column_name}"' for i in self.table._meta.columns
         )
         values = ",".join("{}" for _ in self.add_delegate._add)
         query = f"{base} ({columns}) VALUES {values}"
         querystring = QueryString(
             query,
             *[i.querystring for i in self.add_delegate._add],
             query_type="insert",
             table=self.table,
         )
 
         engine_type = self.engine_type
 
+        on_conflict = self.on_conflict_delegate._on_conflict
+        if on_conflict.on_conflict_items:
+            querystring = QueryString(
+                "{}{}",
+                querystring,
+                on_conflict.querystring,
+                query_type="insert",
+                table=self.table,
+            )
+
         if engine_type in ("postgres", "cockroach") or (
             engine_type == "sqlite"
             and self.table._meta.db.get_version_sync() >= 3.35
         ):
-            if self.returning_delegate._returning:
+            returning = self.returning_delegate._returning
+            if returning:
                 return [
                     QueryString(
                         "{}{}",
                         querystring,
-                        self.returning_delegate._returning.querystring,
+                        returning.querystring,
                         query_type="insert",
                         table=self.table,
                     )
                 ]
 
         return [querystring]
+
+
+Self = t.TypeVar("Self", bound=Insert)
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/raw.py` & `piccolo-1.0a1/piccolo/query/methods/raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/query/methods/refresh.py` & `piccolo-1.0a1/piccolo/query/methods/refresh.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,17 @@
         if self.columns:
             return self.columns
 
         return [
             i for i in self.instance._meta.columns if not i._meta.primary_key
         ]
 
-    async def run(self) -> Table:
+    async def run(
+        self, in_pool: bool = True, node: t.Optional[str] = None
+    ) -> Table:
         """
         Run it asynchronously. For example::
 
             await my_instance.refresh().run()
 
             # or for convenience:
             await my_instance.refresh()
@@ -66,17 +68,18 @@
             raise ValueError("The instance's primary key value isn't defined.")
 
         columns = self._columns
         if not columns:
             raise ValueError("No columns to fetch.")
 
         updated_values = (
-            await instance.select(*columns)
+            await instance.__class__.select(*columns)
             .where(pk_column == primary_key_value)
             .first()
+            .run(node=node, in_pool=in_pool)
         )
 
         if updated_values is None:
             raise ValueError(
                 "The object doesn't exist in the database any more."
             )
 
@@ -88,15 +91,15 @@
     def __await__(self):
         """
         If the user doesn't explicity call :meth:`run`, proxy to it as a
         convenience.
         """
         return self.run().__await__()
 
-    def run_sync(self) -> Table:
+    def run_sync(self, *args, **kwargs) -> Table:
         """
         Run it synchronously. For example::
 
             my_instance.refresh().run_sync()
 
         """
-        return run_sync(self.run())
+        return run_sync(self.run(*args, **kwargs))
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/select.py` & `piccolo-1.0a1/piccolo/query/mixins.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,666 +1,786 @@
 from __future__ import annotations
 
-import decimal
+import asyncio
+import collections.abc
 import itertools
 import typing as t
-from collections import OrderedDict
+from dataclasses import dataclass, field
+from enum import Enum, auto
 
-from piccolo.columns import Column, Selectable
-from piccolo.columns.column_types import JSON, JSONB, PrimaryKey
-from piccolo.columns.m2m import M2MSelect
-from piccolo.columns.readable import Readable
-from piccolo.engine.base import Batch
-from piccolo.query.base import Query
-from piccolo.query.mixins import (
-    AsOfDelegate,
-    CallbackDelegate,
-    CallbackType,
-    ColumnsDelegate,
-    DistinctDelegate,
-    GroupByDelegate,
-    LimitDelegate,
-    OffsetDelegate,
-    OrderByDelegate,
-    OrderByRaw,
-    OutputDelegate,
-    WhereDelegate,
-)
+from piccolo.columns import And, Column, Or, Where
+from piccolo.columns.column_types import ForeignKey
+from piccolo.custom_types import Combinable
 from piccolo.querystring import QueryString
-from piccolo.utils.dictionary import make_nested
-from piccolo.utils.encoding import load_json
-from piccolo.utils.warnings import colored_warning
+from piccolo.utils.list import flatten
+from piccolo.utils.sql_values import convert_to_sql_value
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from piccolo.custom_types import Combinable
+    from piccolo.columns.base import Selectable
     from piccolo.table import Table  # noqa
 
 
-def is_numeric_column(column: Column) -> bool:
-    return column.value_type in (int, decimal.Decimal, float)
+class DistinctOnError(ValueError):
+    """
+    Raised when ``DISTINCT ON`` queries are malformed.
+    """
 
+    pass
 
-class Avg(Selectable):
-    """
-    ``AVG()`` SQL function. Column type must be numeric to run the query.
 
-    .. code-block:: python
+@dataclass
+class Distinct:
+    __slots__ = ("enabled", "on")
 
-        await Band.select(Avg(Band.popularity)).run()
+    enabled: bool
+    on: t.Optional[t.Sequence[Column]]
 
-        # We can use an alias. These two are equivalent:
+    @property
+    def querystring(self) -> QueryString:
+        if self.enabled:
+            if self.on:
+                column_names = ", ".join(
+                    i._meta.get_full_name(with_alias=False) for i in self.on
+                )
+                return QueryString(f" DISTINCT ON ({column_names})")
+            else:
+                return QueryString(" DISTINCT")
+        else:
+            return QueryString(" ALL")
 
-        await Band.select(
-            Avg(Band.popularity, alias="popularity_avg")
-        ).run()
+    def validate_on(self, order_by: OrderBy):
+        """
+        When using the `on` argument, the first column must match the first
+        order by column.
 
-        await Band.select(
-            Avg(Band.popularity).as_alias("popularity_avg")
-        ).run()
+        :raises DistinctOnError:
+            If the columns don't match.
 
-    """
+        """
+        validated = True
 
-    def __init__(self, column: Column, alias: str = "avg"):
-        if is_numeric_column(column):
-            self.column = column
+        try:
+            first_order_column = order_by.order_by_items[0].columns[0]
+        except IndexError:
+            validated = False
         else:
-            raise ValueError("Column type must be numeric to run the query.")
-        self._alias = alias
+            if not self.on:
+                validated = False
+            elif isinstance(first_order_column, Column) and not self.on[
+                0
+            ]._equals(first_order_column):
+                validated = False
+
+        if not validated:
+            raise DistinctOnError(
+                "The first `order_by` column must match the first column "
+                "passed to `on`."
+            )
 
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'AVG({column_name}) AS "{self._alias}"'
+    def __str__(self) -> str:
+        return self.querystring.__str__()
 
+    def copy(self) -> Distinct:
+        return self.__class__(enabled=self.enabled, on=self.on)
 
-class Count(Selectable):
-    """
-    Used in conjunction with the ``group_by`` clause in ``Select`` queries.
 
-    If a column is specified, the count is for non-null values in that
-    column. If no column is specified, the count is for all rows, whether
-    they have null values or not.
+@dataclass
+class Limit:
+    __slots__ = ("number",)
 
-    .. code-block:: python
+    number: int
 
-        await Band.select(Band.name, Count()).group_by(Band.name)
+    def __post_init__(self):
+        if type(self.number) != int:
+            raise TypeError("Limit must be an integer")
 
-        # We can use an alias. These two are equivalent:
+    @property
+    def querystring(self) -> QueryString:
+        return QueryString(f" LIMIT {self.number}")
 
-        await Band.select(
-            Band.name, Count(alias="total")
-        ).group_by(Band.name)
+    def __str__(self) -> str:
+        return self.querystring.__str__()
 
-        await Band.select(
-            Band.name,
-            Count().as_alias("total")
-        ).group_by(Band.name)
+    def copy(self) -> Limit:
+        return self.__class__(number=self.number)
 
-    """
 
-    def __init__(
-        self, column: t.Optional[Column] = None, alias: str = "count"
-    ):
-        self.column = column
-        self._alias = alias
+@dataclass
+class AsOf:
+    __slots__ = ("interval",)
 
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        if self.column is None:
-            column_name = "*"
-        else:
-            column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'COUNT({column_name}) AS "{self._alias}"'
+    interval: str
 
+    def __post_init__(self):
+        if type(self.interval) != str:
+            raise TypeError("As Of must be a string. Example: '-1s'")
 
-class Max(Selectable):
-    """
-    ``MAX()`` SQL function.
+    @property
+    def querystring(self) -> QueryString:
+        return QueryString(f" AS OF SYSTEM TIME '{self.interval}'")
 
-    .. code-block:: python
+    def __str__(self) -> str:
+        return self.querystring.__str__()
 
-        await Band.select(
-            Max(Band.popularity)
-        ).run()
 
-        # We can use an alias. These two are equivalent:
+@dataclass
+class Offset:
+    __slots__ = ("number",)
 
-        await Band.select(
-            Max(Band.popularity, alias="popularity_max")
-        ).run()
+    number: int
 
-        await Band.select(
-            Max(Band.popularity).as_alias("popularity_max")
-        ).run()
+    def __post_init__(self):
+        if type(self.number) != int:
+            raise TypeError("Limit must be an integer")
 
-    """
+    @property
+    def querystring(self) -> QueryString:
+        return QueryString(f" OFFSET {self.number}")
 
-    def __init__(self, column: Column, alias: str = "max"):
-        self.column = column
-        self._alias = alias
+    def __str__(self) -> str:
+        return self.querystring.__str__()
 
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'MAX({column_name}) AS "{self._alias}"'
 
+@dataclass
+class OrderByRaw:
+    __slots__ = ("sql",)
 
-class Min(Selectable):
-    """
-    ``MIN()`` SQL function.
+    sql: str
 
-    .. code-block:: python
 
-        await Band.select(Min(Band.popularity)).run()
+@dataclass
+class OrderByItem:
+    __slots__ = ("columns", "ascending")
 
-        # We can use an alias. These two are equivalent:
+    columns: t.Sequence[t.Union[Column, OrderByRaw]]
+    ascending: bool
 
-        await Band.select(
-            Min(Band.popularity, alias="popularity_min")
-        ).run()
 
-        await Band.select(
-            Min(Band.popularity).as_alias("popularity_min")
-        ).run()
+@dataclass
+class OrderBy:
+    order_by_items: t.List[OrderByItem] = field(default_factory=list)
 
-    """
+    @property
+    def querystring(self) -> QueryString:
+        order_by_strings: t.List[str] = []
+        for order_by_item in self.order_by_items:
+            order = "ASC" if order_by_item.ascending else "DESC"
+            for column in order_by_item.columns:
+                if isinstance(column, Column):
+                    expression = column._meta.get_full_name(with_alias=False)
+                elif isinstance(column, OrderByRaw):
+                    expression = column.sql
+                else:
+                    raise ValueError("Unrecognised order_by")
 
-    def __init__(self, column: Column, alias: str = "min"):
-        self.column = column
-        self._alias = alias
+                order_by_strings.append(f"{expression} {order}")
 
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'MIN({column_name}) AS "{self._alias}"'
+        return QueryString(f" ORDER BY {', '.join(order_by_strings)}")
 
+    def __str__(self):
+        return self.querystring.__str__()
 
-class Sum(Selectable):
-    """
-    ``SUM()`` SQL function. Column type must be numeric to run the query.
 
-    .. code-block:: python
+@dataclass
+class Returning:
+    __slots__ = ("columns",)
+
+    columns: t.List[Column]
+
+    @property
+    def querystring(self) -> QueryString:
+        column_names = []
+        for column in self.columns:
+            column_names.append(
+                f'"{column._meta.db_column_name}" AS "{column._alias}"'
+                if column._alias
+                else f'"{column._meta.db_column_name}"'
+            )
+
+        columns_string = ", ".join(column_names)
+
+        return QueryString(f" RETURNING {columns_string}")
+
+    def __str__(self):
+        return self.querystring.__str__()
+
+
+@dataclass
+class Output:
+
+    as_json: bool = False
+    as_list: bool = False
+    as_objects: bool = False
+    load_json: bool = False
+    nested: bool = False
+
+    def copy(self) -> Output:
+        return self.__class__(
+            as_json=self.as_json,
+            as_list=self.as_list,
+            as_objects=self.as_objects,
+            load_json=self.load_json,
+            nested=self.nested,
+        )
+
+
+class CallbackType(Enum):
+    success = auto()
+
+
+@dataclass
+class Callback:
+    kind: CallbackType
+    target: t.Callable
+
+
+@dataclass
+class WhereDelegate:
+
+    _where: t.Optional[Combinable] = None
+    _where_columns: t.List[Column] = field(default_factory=list)
 
-        await Band.select(
-            Sum(Band.popularity)
-        ).run()
+    def get_where_columns(self):
+        """
+        Retrieves all columns used in the where clause - in case joins are
+        needed.
+        """
+        self._where_columns = []
+        self._extract_columns(self._where)
+        return self._where_columns
+
+    def _extract_columns(self, combinable: Combinable):
+        if isinstance(combinable, Where):
+            self._where_columns.append(combinable.column)
+        elif isinstance(combinable, (And, Or)):
+            self._extract_columns(combinable.first)
+            self._extract_columns(combinable.second)
+
+    def where(self, *where: Combinable):
+        for arg in where:
+            if isinstance(arg, bool):
+                raise ValueError(
+                    "A boolean value has been passed in to a where clause. "
+                    "This is probably a mistake. For example "
+                    "`.where(MyTable.some_column is None)` instead of "
+                    "`.where(MyTable.some_column.is_null())`."
+                )
+
+            self._where = And(self._where, arg) if self._where else arg
+
+
+@dataclass
+class OrderByDelegate:
+
+    _order_by: OrderBy = field(default_factory=OrderBy)
 
-        # We can use an alias. These two are equivalent:
+    def get_order_by_columns(self) -> t.List[Column]:
+        """
+        Used to work out which columns are needed for joins.
+        """
+        return [
+            i
+            for i in itertools.chain(
+                *[i.columns for i in self._order_by.order_by_items]
+            )
+            if isinstance(i, Column)
+        ]
 
-        await Band.select(
-            Sum(Band.popularity, alias="popularity_sum")
-        ).run()
+    def order_by(self, *columns: t.Union[Column, OrderByRaw], ascending=True):
+        if len(columns) < 1:
+            raise ValueError("At least one column must be passed to order_by.")
 
-        await Band.select(
-            Sum(Band.popularity).as_alias("popularity_sum")
-        ).run()
+        self._order_by.order_by_items.append(
+            OrderByItem(columns=columns, ascending=ascending)
+        )
 
+
+@dataclass
+class LimitDelegate:
+
+    _limit: t.Optional[Limit] = None
+    _first: bool = False
+
+    def limit(self, number: int):
+        self._limit = Limit(number)
+
+    def copy(self) -> LimitDelegate:
+        _limit = self._limit.copy() if self._limit is not None else None
+        return self.__class__(_limit=_limit, _first=self._first)
+
+
+@dataclass
+class AsOfDelegate:
+    """
+    Time travel queries using "As Of" syntax.
+    Currently supports Cockroach using AS OF SYSTEM TIME.
     """
 
-    def __init__(self, column: Column, alias: str = "sum"):
-        if is_numeric_column(column):
-            self.column = column
-        else:
-            raise ValueError("Column type must be numeric to run the query.")
-        self._alias = alias
+    _as_of: t.Optional[AsOf] = None
+
+    def as_of(self, interval: str = "-1s"):
+        self._as_of = AsOf(interval)
+
+
+@dataclass
+class DistinctDelegate:
 
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'SUM({column_name}) AS "{self._alias}"'
-
-
-class Select(Query):
-    __slots__ = (
-        "columns_list",
-        "exclude_secrets",
-        "as_of_delegate",
-        "columns_delegate",
-        "distinct_delegate",
-        "group_by_delegate",
-        "limit_delegate",
-        "offset_delegate",
-        "order_by_delegate",
-        "output_delegate",
-        "callback_delegate",
-        "where_delegate",
+    _distinct: Distinct = field(
+        default_factory=lambda: Distinct(enabled=False, on=None)
     )
 
-    def __init__(
+    def distinct(
+        self, enabled: bool, on: t.Optional[t.Sequence[Column]] = None
+    ):
+        if on and not isinstance(on, collections.abc.Sequence):
+            # Check a sequence is passed in, otherwise the user will get some
+            # unuseful errors later on.
+            raise ValueError("`on` must be a sequence of `Column` instances")
+
+        self._distinct = Distinct(enabled=enabled, on=on)
+
+
+@dataclass
+class ReturningDelegate:
+    _returning: t.Optional[Returning] = None
+
+    def returning(self, columns: t.Sequence[Column]):
+        self._returning = Returning(columns=list(columns))
+
+
+@dataclass
+class CountDelegate:
+
+    _count: bool = False
+
+    def count(self):
+        self._count = True
+
+
+@dataclass
+class AddDelegate:
+
+    _add: t.List[Table] = field(default_factory=list)
+
+    def add(self, *instances: Table, table_class: t.Type[Table]):
+        for instance in instances:
+            if not isinstance(instance, table_class):
+                raise TypeError("Incompatible type added.")
+
+        self._add += instances
+
+
+@dataclass
+class OutputDelegate:
+    """
+    Example usage:
+
+    .output(as_list=True)
+    .output(as_json=True)
+    .output(as_json=True, as_list=True)
+    """
+
+    _output: Output = field(default_factory=Output)
+
+    def output(
         self,
-        table: t.Type[Table],
-        columns_list: t.Sequence[t.Union[Selectable, str]] = None,
-        exclude_secrets: bool = False,
-        **kwargs,
+        as_list: t.Optional[bool] = None,
+        as_json: t.Optional[bool] = None,
+        load_json: t.Optional[bool] = None,
+        nested: t.Optional[bool] = None,
     ):
-        if columns_list is None:
-            columns_list = []
-        super().__init__(table, **kwargs)
-        self.exclude_secrets = exclude_secrets
-
-        self.as_of_delegate = AsOfDelegate()
-        self.columns_delegate = ColumnsDelegate()
-        self.distinct_delegate = DistinctDelegate()
-        self.group_by_delegate = GroupByDelegate()
-        self.limit_delegate = LimitDelegate()
-        self.offset_delegate = OffsetDelegate()
-        self.order_by_delegate = OrderByDelegate()
-        self.output_delegate = OutputDelegate()
-        self.callback_delegate = CallbackDelegate()
-        self.where_delegate = WhereDelegate()
-
-        self.columns(*columns_list)
-
-    def columns(self, *columns: t.Union[Selectable, str]) -> Select:
-        _columns = self.table._process_column_args(*columns)
-        self.columns_delegate.columns(*_columns)
-        return self
-
-    def distinct(self) -> Select:
-        self.distinct_delegate.distinct()
-        return self
+        """
+        :param as_list:
+            If each row only returns a single value, compile all of the results
+            into a single list.
+        :param as_json:
+            The results are serialised into JSON. It's equivalent to running
+            `json.dumps` on the result.
+        :param load_json:
+            If True, any JSON fields will have the JSON values returned from
+            the database loaded as Python objects.
+        """
+        # We do it like this, so output can be called multiple times, without
+        # overriding any existing values if they're not specified.
+        if as_list is not None:
+            self._output.as_list = bool(as_list)
 
-    def group_by(self, *columns: t.Union[Column, str]) -> Select:
-        _columns: t.List[Column] = [
-            i
-            for i in self.table._process_column_args(*columns)
-            if isinstance(i, Column)
-        ]
-        self.group_by_delegate.group_by(*_columns)
-        return self
+        if as_json is not None:
+            self._output.as_json = bool(as_json)
+
+        if load_json is not None:
+            self._output.load_json = bool(load_json)
 
-    def as_of(self, interval: str = "-1s") -> Select:
-        self.as_of_delegate.as_of(interval)
-        return self
-
-    def limit(self, number: int) -> Select:
-        self.limit_delegate.limit(number)
-        return self
-
-    def first(self) -> Select:
-        self.limit_delegate.first()
-        return self
-
-    def offset(self, number: int) -> Select:
-        self.offset_delegate.offset(number)
-        return self
+        if nested is not None:
+            self._output.nested = bool(nested)
 
-    async def _splice_m2m_rows(
+    def copy(self) -> OutputDelegate:
+        _output = self._output.copy() if self._output is not None else None
+        return self.__class__(_output=_output)
+
+
+@dataclass
+class CallbackDelegate:
+    """
+    Example usage:
+
+    .callback(my_handler_function)
+    .callback(print, on=CallbackType.success)
+    .callback(my_handler_coroutine)
+    .callback([handler1, handler2])
+    """
+
+    _callbacks: t.Dict[CallbackType, t.List[Callback]] = field(
+        default_factory=lambda: {kind: [] for kind in CallbackType}
+    )
+
+    def callback(
         self,
-        response: t.List[t.Dict[str, t.Any]],
-        secondary_table: t.Type[Table],
-        secondary_table_pk: PrimaryKey,
-        m2m_name: str,
-        m2m_select: M2MSelect,
-        as_list: bool = False,
+        callbacks: t.Union[t.Callable, t.List[t.Callable]],
+        *,
+        on: CallbackType,
     ):
-        row_ids = list(
-            set(itertools.chain(*[row[m2m_name] for row in response]))
-        )
-        extra_rows = (
-            (
-                await secondary_table.select(
-                    *m2m_select.columns,
-                    secondary_table_pk.as_alias("mapping_key"),
-                )
-                .where(secondary_table_pk.is_in(row_ids))
-                .output(load_json=m2m_select.load_json)
-                .run()
+        if isinstance(callbacks, list):
+            self._callbacks[on].extend(
+                Callback(kind=on, target=callback) for callback in callbacks
             )
-            if row_ids
-            else []
-        )
-        if as_list:
-            column_name = m2m_select.columns[0]._meta.name
-            extra_rows_map = {
-                row["mapping_key"]: row[column_name] for row in extra_rows
-            }
         else:
-            extra_rows_map = {
-                row["mapping_key"]: {
-                    key: value
-                    for key, value in row.items()
-                    if key != "mapping_key"
-                }
-                for row in extra_rows
-            }
-        for row in response:
-            row[m2m_name] = [extra_rows_map.get(i) for i in row[m2m_name]]
-        return response
-
-    async def response_handler(self, response):
-        m2m_selects = [
-            i
-            for i in self.columns_delegate.selected_columns
-            if isinstance(i, M2MSelect)
-        ]
-        for m2m_select in m2m_selects:
-            m2m_name = m2m_select.m2m._meta.name
-            secondary_table = m2m_select.m2m._meta.secondary_table
-            secondary_table_pk = secondary_table._meta.primary_key
-
-            if self.engine_type == "sqlite":
-                # With M2M queries in SQLite, we always get the value back as a
-                # list of strings, so we need to do some type conversion.
-                value_type = (
-                    m2m_select.columns[0].__class__.value_type
-                    if m2m_select.as_list and m2m_select.serialisation_safe
-                    else secondary_table_pk.value_type
-                )
-                try:
-                    for row in response:
-                        data = row[m2m_name]
-                        row[m2m_name] = (
-                            [value_type(i) for i in row[m2m_name]]
-                            if data
-                            else []
-                        )
-                except ValueError:
-                    colored_warning(
-                        "Unable to do type conversion for the "
-                        f"{m2m_name} relation"
-                    )
-
-                # If the user requested a single column, we just return that
-                # from the database. Otherwise we request the primary key
-                # value, so we can fetch the rest of the data in a subsequent
-                # SQL query - see below.
-                if m2m_select.as_list:
-                    if m2m_select.serialisation_safe:
-                        pass
-                    else:
-                        response = await self._splice_m2m_rows(
-                            response,
-                            secondary_table,
-                            secondary_table_pk,
-                            m2m_name,
-                            m2m_select,
-                            as_list=True,
-                        )
-                else:
-                    if (
-                        len(m2m_select.columns) == 1
-                        and m2m_select.serialisation_safe
-                    ):
-                        column_name = m2m_select.columns[0]._meta.name
-                        for row in response:
-                            row[m2m_name] = [
-                                {column_name: i} for i in row[m2m_name]
-                            ]
-                    else:
-                        response = await self._splice_m2m_rows(
-                            response,
-                            secondary_table,
-                            secondary_table_pk,
-                            m2m_name,
-                            m2m_select,
-                        )
-
-            elif self.engine_type in ("postgres", "cockroach"):
-                if m2m_select.as_list:
-                    # We get the data back as an array, and can just return it
-                    # unless it's JSON.
-                    if (
-                        type(m2m_select.columns[0]) in (JSON, JSONB)
-                        and m2m_select.load_json
-                    ):
-                        for row in response:
-                            data = row[m2m_name]
-                            row[m2m_name] = [load_json(i) for i in data]
-                elif m2m_select.serialisation_safe:
-                    # If the columns requested can be safely serialised, they
-                    # are returned as a JSON string, so we need to deserialise
-                    # it.
-                    for row in response:
-                        data = row[m2m_name]
-                        row[m2m_name] = load_json(data) if data else []
-                else:
-                    # If the data can't be safely serialised as JSON, we get
-                    # back an array of primary key values, and need to
-                    # splice in the correct values using Python.
-                    response = await self._splice_m2m_rows(
-                        response,
-                        secondary_table,
-                        secondary_table_pk,
-                        m2m_name,
-                        m2m_select,
-                    )
-
-        #######################################################################
-
-        # If no columns were specified, it's a select *, so we know that
-        # no columns were selected from related tables.
-        was_select_star = len(self.columns_delegate.selected_columns) == 0
-
-        if self.limit_delegate._first:
-            if len(response) == 0:
-                return None
+            self._callbacks[on].append(Callback(kind=on, target=callbacks))
 
-            if self.output_delegate._output.nested and not was_select_star:
-                return make_nested(response[0])
+    async def invoke(self, results: t.Any, *, kind: CallbackType) -> t.Any:
+        """
+        Utility function that invokes the registered callbacks in the correct
+        way, handling both sync and async callbacks. Only callbacks of the
+        given kind are invoked.
+        Results are passed through the callbacks in the order they were added,
+        with each callback able to transform them. This function returns the
+        transformed results.
+        """
+        for callback in self._callbacks[kind]:
+            if asyncio.iscoroutinefunction(callback.target):
+                results = await callback.target(results)
             else:
-                return response[0]
-        elif self.output_delegate._output.nested and not was_select_star:
-            return [make_nested(i) for i in response]
-        else:
-            return response
+                results = callback.target(results)
+
+        return results
+
+
+@dataclass
+class PrefetchDelegate:
+    """
+    Example usage:
+
+    .prefetch(MyTable.column_a, MyTable.column_b)
+    """
+
+    fk_columns: t.List[ForeignKey] = field(default_factory=list)
 
-    def order_by(
-        self, *columns: t.Union[Column, str, OrderByRaw], ascending=True
-    ) -> Select:
+    def prefetch(self, *fk_columns: t.Union[ForeignKey, t.List[ForeignKey]]):
         """
         :param columns:
-            Either a :class:`piccolo.columns.base.Column` instance, a string
-            representing a column name, or :class:`piccolo.query.OrderByRaw`
-            which allows you for complex use cases like
-            ``OrderByRaw('random()')``.
-        """
-        _columns: t.List[t.Union[Column, OrderByRaw]] = []
-        for column in columns:
-            if isinstance(column, str):
-                _columns.append(self.table._meta.get_column_by_name(column))
+            We accept ``ForeignKey`` and ``List[ForeignKey]`` here, in case
+            someone passes in a list by accident when using ``all_related()``,
+            in which case we flatten the list.
+
+        """
+        _fk_columns: t.List[ForeignKey] = []
+        for column in fk_columns:
+            if isinstance(column, list):
+                _fk_columns.extend(column)
             else:
-                _columns.append(column)
+                _fk_columns.append(column)
 
-        self.order_by_delegate.order_by(*_columns, ascending=ascending)
-        return self
+        combined = self.fk_columns + _fk_columns
+        self.fk_columns = combined
 
-    def output(
-        self,
-        as_list: bool = False,
-        as_json: bool = False,
-        load_json: bool = False,
-        nested: bool = False,
-    ) -> Select:
-        self.output_delegate.output(
-            as_list=as_list,
-            as_json=as_json,
-            load_json=load_json,
-            nested=nested,
-        )
-        return self
 
-    def callback(
-        self,
-        callbacks: t.Union[t.Callable, t.List[t.Callable]],
-        *,
-        on: CallbackType = CallbackType.success,
-    ) -> Select:
-        self.callback_delegate.callback(callbacks, on=on)
-        return self
-
-    def where(self, *where: Combinable) -> Select:
-        self.where_delegate.where(*where)
-        return self
+@dataclass
+class ColumnsDelegate:
+    """
+    Example usage:
 
-    async def batch(
-        self,
-        batch_size: t.Optional[int] = None,
-        node: t.Optional[str] = None,
-        **kwargs,
-    ) -> Batch:
-        if batch_size:
-            kwargs.update(batch_size=batch_size)
-        if node:
-            kwargs.update(node=node)
-        return await self.table._meta.db.batch(self, **kwargs)
-
-    ###########################################################################
-
-    def _get_joins(self, columns: t.Sequence[Selectable]) -> t.List[str]:
+    .columns(MyTable.column_a, MyTable.column_b)
+    """
+
+    selected_columns: t.Sequence[Selectable] = field(default_factory=list)
+
+    def columns(self, *columns: t.Union[Selectable, t.List[Selectable]]):
         """
-        A call chain is a sequence of foreign keys representing joins which
-        need to be made to retrieve a column in another table.
+        :param columns:
+            We accept ``Selectable`` and ``List[Selectable]`` here, in case
+            someone passes in a list by accident when using ``all_columns()``,
+            in which case we flatten the list.
+
         """
-        joins: t.List[str] = []
+        _columns = flatten(columns)
+        combined = list(self.selected_columns) + _columns
+        self.selected_columns = combined
 
-        readables: t.List[Readable] = [
-            i for i in columns if isinstance(i, Readable)
+    def remove_secret_columns(self):
+        non_secret = [
+            i
+            for i in self.selected_columns
+            if not isinstance(i, Column) or not i._meta.secret
         ]
 
-        columns = list(columns)
-        for readable in readables:
-            columns += readable.columns
-
-        for column in columns:
-            if not isinstance(column, Column):
-                continue
-
-            _joins: t.List[str] = []
-            for index, key in enumerate(column._meta.call_chain, 0):
-                table_alias = "$".join(
-                    f"{_key._meta.table._meta.tablename}${_key._meta.name}"
-                    for _key in column._meta.call_chain[: index + 1]
-                )
+        self.selected_columns = non_secret
 
-                key._meta.table_alias = table_alias
 
-                if index > 0:
-                    left_tablename = column._meta.call_chain[
-                        index - 1
-                    ]._meta.table_alias
-                else:
-                    left_tablename = key._meta.table._meta.tablename
+@dataclass
+class ValuesDelegate:
+    """
+    Used to specify new column values - primarily used in update queries.
+    """
 
-                right_tablename = (
-                    key._foreign_key_meta.resolved_references._meta.tablename
-                )
+    table: t.Type[Table]
+    _values: t.Dict[Column, t.Any] = field(default_factory=dict)
 
-                pk_name = column._meta.call_chain[
-                    index
-                ]._foreign_key_meta.resolved_target_column._meta.name
-
-                _joins.append(
-                    f'LEFT JOIN "{right_tablename}" "{table_alias}"'
-                    " ON "
-                    f'("{left_tablename}"."{key._meta.name}" = "{table_alias}"."{pk_name}")'  # noqa: E501
-                )
+    def values(self, values: t.Dict[t.Union[Column, str], t.Any]):
+        """
+        Example usage:
+
+        .. code-block:: python
 
-            joins.extend(_joins)
+            .values({MyTable.column_a: 1})
 
-        # Remove duplicates
-        return list(OrderedDict.fromkeys(joins))
+            # Or:
+            .values({'column_a': 1})
 
-    def _check_valid_call_chain(self, keys: t.Sequence[Selectable]) -> bool:
-        for column in keys:
-            if not isinstance(column, Column):
-                continue
-            if column._meta.call_chain and len(column._meta.call_chain) > 10:
-                # Make sure the call_chain isn't too large to discourage
-                # very inefficient queries.
-                raise Exception(
-                    "Joining more than 10 tables isn't supported - "
-                    "please restructure your query."
+            # Or:
+            .values(column_a=1})
+
+        """
+        cleaned_values: t.Dict[Column, t.Any] = {}
+        for key, value in values.items():
+            if isinstance(key, Column):
+                column = key
+            elif isinstance(key, str):
+                column = self.table._meta.get_column_by_name(key)
+            else:
+                raise ValueError(
+                    f"Unrecognised key - {key} is neither a Column or the "
+                    "name of a Column."
                 )
-        return True
+            cleaned_values[column] = value
 
-    @property
-    def default_querystrings(self) -> t.Sequence[QueryString]:
-        # JOIN
-        self._check_valid_call_chain(self.columns_delegate.selected_columns)
+        self._values.update(cleaned_values)
 
-        select_joins = self._get_joins(self.columns_delegate.selected_columns)
-        where_joins = self._get_joins(self.where_delegate.get_where_columns())
-        order_by_joins = self._get_joins(
-            self.order_by_delegate.get_order_by_columns()
-        )
+    def get_sql_values(self) -> t.List[t.Any]:
+        """
+        Convert any Enums into values, and serialise any JSON.
+        """
+        return [
+            convert_to_sql_value(value=value, column=column)
+            for column, value in self._values.items()
+        ]
 
-        # Combine all joins, and remove duplicates
-        joins: t.List[str] = list(
-            OrderedDict.fromkeys(select_joins + where_joins + order_by_joins)
-        )
 
-        #######################################################################
+@dataclass
+class OffsetDelegate:
+    """
+    Used to offset the results - for example, to return row 100 and onward.
+
+    Typically used in conjunction with order_by and limit.
 
-        # If no columns have been specified for selection, select all columns
-        # on the table:
-        if len(self.columns_delegate.selected_columns) == 0:
-            self.columns_delegate.selected_columns = self.table._meta.columns
-
-        # If secret fields need to be omitted, remove them from the list.
-        if self.exclude_secrets:
-            self.columns_delegate.remove_secret_columns()
-
-        engine_type = self.table._meta.db.engine_type
-
-        select_strings: t.List[str] = [
-            c.get_select_string(engine_type=engine_type)
-            for c in self.columns_delegate.selected_columns
-        ]
-        columns_str = ", ".join(select_strings)
+    Example usage::
+
+        .offset(100)
+
+    """
+
+    _offset: t.Optional[Offset] = None
+
+    def offset(self, number: int = 0):
+        self._offset = Offset(number)
 
-        #######################################################################
 
-        select = (
-            "SELECT DISTINCT" if self.distinct_delegate._distinct else "SELECT"
+@dataclass
+class GroupBy:
+    __slots__ = ("columns",)
+
+    columns: t.Sequence[Column]
+
+    @property
+    def querystring(self) -> QueryString:
+        columns_names = ", ".join(
+            i._meta.get_full_name(with_alias=False) for i in self.columns
         )
-        query = f"{select} {columns_str} FROM {self.table._meta.tablename}"
 
-        for join in joins:
-            query += f" {join}"
+        return QueryString(f" GROUP BY {columns_names}")
+
+    def __str__(self):
+        return self.querystring.__str__()
+
+
+@dataclass
+class GroupByDelegate:
+    """
+    Used to group results - needed when doing aggregation::
+
+        .group_by(Band.name)
+
+    """
+
+    _group_by: t.Optional[GroupBy] = None
+
+    def group_by(self, *columns: Column):
+        self._group_by = GroupBy(columns=columns)
+
+
+class OnConflictAction(str, Enum):
+    """
+    Specify which action to take on conflict.
+    """
+
+    do_nothing = "DO NOTHING"
+    do_update = "DO UPDATE"
+
+
+@dataclass
+class OnConflictItem:
+    target: t.Optional[t.Union[str, Column, t.Tuple[Column, ...]]] = None
+    action: t.Optional[OnConflictAction] = None
+    values: t.Optional[
+        t.Sequence[t.Union[Column, t.Tuple[Column, t.Any]]]
+    ] = None
+    where: t.Optional[Combinable] = None
+
+    @property
+    def target_string(self) -> str:
+        target = self.target
+        assert target
+
+        def to_string(value) -> str:
+            if isinstance(value, Column):
+                return f'"{value._meta.db_column_name}"'
+            else:
+                raise ValueError("OnConflict.target isn't a valid type")
+
+        if isinstance(target, str):
+            return f'ON CONSTRAINT "{target}"'
+        elif isinstance(target, Column):
+            return f"({to_string(target)})"
+        elif isinstance(target, tuple):
+            columns_str = ", ".join([to_string(i) for i in target])
+            return f"({columns_str})"
+        else:
+            raise ValueError("OnConflict.target isn't a valid type")
 
-        #######################################################################
+    @property
+    def action_string(self) -> QueryString:
+        action = self.action
+        if isinstance(action, OnConflictAction):
+            if action == OnConflictAction.do_nothing:
+                return QueryString(OnConflictAction.do_nothing.value)
+            elif action == OnConflictAction.do_update:
+                values = []
+                query = f"{OnConflictAction.do_update.value} SET"
+
+                if not self.values:
+                    raise ValueError("No values specified for `on conflict`")
+
+                for value in self.values:
+                    if isinstance(value, Column):
+                        column_name = value._meta.db_column_name
+                        query += f' "{column_name}"=EXCLUDED."{column_name}",'
+                    elif isinstance(value, tuple):
+                        column = value[0]
+                        value_ = value[1]
+                        if isinstance(column, Column):
+                            column_name = column._meta.db_column_name
+                        else:
+                            raise ValueError("Unsupported column type")
 
-        args: t.List[t.Any] = []
+                        query += f' "{column_name}"={{}},'
+                        values.append(value_)
 
-        if self.as_of_delegate._as_of:
-            query += "{}"
-            args.append(self.as_of_delegate._as_of.querystring)
+                return QueryString(query.rstrip(","), *values)
+
+        raise ValueError("OnConflict.action isn't a valid type")
+
+    @property
+    def querystring(self) -> QueryString:
+        query = " ON CONFLICT"
+        values = []
+
+        if self.target:
+            query += f" {self.target_string}"
+
+        if self.action:
+            query += " {}"
+            values.append(self.action_string)
 
-        if self.where_delegate._where:
+        if self.where:
             query += " WHERE {}"
-            args.append(self.where_delegate._where.querystring)
+            values.append(self.where.querystring)
 
-        if self.group_by_delegate._group_by:
-            query += "{}"
-            args.append(self.group_by_delegate._group_by.querystring)
-
-        if self.order_by_delegate._order_by.order_by_items:
-            query += "{}"
-            args.append(self.order_by_delegate._order_by.querystring)
-
-        if (
-            engine_type == "sqlite"
-            and self.offset_delegate._offset
-            and not self.limit_delegate._limit
-        ):
-            raise ValueError(
-                "A limit clause must be provided when doing an offset with "
-                "SQLite."
-            )
+        return QueryString(query, *values)
+
+    def __str__(self) -> str:
+        return self.querystring.__str__()
+
+
+@dataclass
+class OnConflict:
+    """
+    Multiple `ON CONFLICT` statements are allowed - which is why we have this
+    parent class.
+    """
 
-        if self.limit_delegate._limit:
-            query += "{}"
-            args.append(self.limit_delegate._limit.querystring)
+    on_conflict_items: t.List[OnConflictItem] = field(default_factory=list)
+
+    @property
+    def querystring(self) -> QueryString:
+        query = "".join("{}" for i in self.on_conflict_items)
+        return QueryString(
+            query, *[i.querystring for i in self.on_conflict_items]
+        )
+
+    def __str__(self) -> str:
+        return self.querystring.__str__()
+
+
+@dataclass
+class OnConflictDelegate:
+    """
+    Used with insert queries to specify what to do when a query fails due to
+    a constraint::
 
-        if self.offset_delegate._offset:
-            query += "{}"
-            args.append(self.offset_delegate._offset.querystring)
+        .on_conflict(action='DO NOTHING')
 
-        querystring = QueryString(query, *args)
+        .on_conflict(action='DO UPDATE', values=[Band.popularity])
 
-        return [querystring]
+        .on_conflict(action='DO UPDATE', values=[(Band.popularity, 1)])
+
+    """
+
+    _on_conflict: OnConflict = field(default_factory=OnConflict)
+
+    def on_conflict(
+        self,
+        target: t.Optional[t.Union[str, Column, t.Tuple[Column, ...]]] = None,
+        action: t.Union[
+            OnConflictAction, t.Literal["DO NOTHING", "DO UPDATE"]
+        ] = OnConflictAction.do_nothing,
+        values: t.Optional[
+            t.Sequence[t.Union[Column, t.Tuple[Column, t.Any]]]
+        ] = None,
+        where: t.Optional[Combinable] = None,
+    ):
+        action_: OnConflictAction
+        if isinstance(action, OnConflictAction):
+            action_ = action
+        elif isinstance(action, str):
+            action_ = OnConflictAction(action.upper())
+        else:
+            raise ValueError("Unrecognised `on conflict` action.")
+
+        if where and action_ == OnConflictAction.do_nothing:
+            raise ValueError(
+                "The `where` option can only be used with DO NOTHING."
+            )
+
+        self._on_conflict.on_conflict_items.append(
+            OnConflictItem(
+                target=target, action=action_, values=values, where=where
+            )
+        )
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/table_exists.py` & `piccolo-1.0a1/piccolo/query/methods/table_exists.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from __future__ import annotations
 
 import typing as t
 
+from piccolo.custom_types import TableInstance
 from piccolo.query.base import Query
 from piccolo.querystring import QueryString
 
 
-class TableExists(Query):
+class TableExists(Query[TableInstance, bool]):
 
     __slots__: t.Tuple = ()
 
     async def response_handler(self, response):
         return bool(response[0]["exists"])
 
     @property
     def sqlite_querystrings(self) -> t.Sequence[QueryString]:
         return [
             QueryString(
                 "SELECT EXISTS(SELECT * FROM sqlite_master WHERE "
-                f"name = '{self.table._meta.tablename}') AS 'exists'"
+                "name = {}) AS 'exists'",
+                self.table._meta.tablename,
             )
         ]
 
     @property
     def postgres_querystrings(self) -> t.Sequence[QueryString]:
-        return [
-            QueryString(
-                "SELECT EXISTS(SELECT * FROM information_schema.tables WHERE "
-                f"table_name = '{self.table._meta.tablename}')"
+        subquery = QueryString(
+            "SELECT * FROM information_schema.tables WHERE table_name = {}",
+            self.table._meta.tablename,
+        )
+
+        if self.table._meta.schema:
+            subquery = QueryString(
+                "{} AND table_schema = {}", subquery, self.table._meta.schema
             )
-        ]
+
+        query = QueryString("SELECT EXISTS({})", subquery)
+
+        return [query]
 
     @property
     def cockroach_querystrings(self) -> t.Sequence[QueryString]:
-        return [
-            QueryString(
-                "SELECT EXISTS(SELECT * FROM information_schema.tables WHERE "
-                f"table_name = '{self.table._meta.tablename}')"
-            )
-        ]
+        return self.postgres_querystrings
```

### Comparing `piccolo-0.99.0/piccolo/query/methods/update.py` & `piccolo-1.0a1/piccolo/query/methods/update.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from __future__ import annotations
 
 import typing as t
 
-from piccolo.custom_types import Combinable
+from piccolo.custom_types import Combinable, TableInstance
 from piccolo.query.base import Query
 from piccolo.query.mixins import (
     ReturningDelegate,
     ValuesDelegate,
     WhereDelegate,
 )
 from piccolo.querystring import QueryString
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.columns import Column
-    from piccolo.table import Table
 
 
 class UpdateError(Exception):
     pass
 
 
-class Update(Query):
+class Update(Query[TableInstance, t.List[t.Any]]):
 
     __slots__ = (
         "force",
         "returning_delegate",
         "values_delegate",
         "where_delegate",
     )
 
-    def __init__(self, table: t.Type[Table], force: bool = False, **kwargs):
+    def __init__(
+        self, table: t.Type[TableInstance], force: bool = False, **kwargs
+    ):
         super().__init__(table, **kwargs)
         self.force = force
         self.returning_delegate = ReturningDelegate()
         self.values_delegate = ValuesDelegate(table=table)
         self.where_delegate = WhereDelegate()
 
     ###########################################################################
@@ -85,25 +86,28 @@
     @property
     def default_querystrings(self) -> t.Sequence[QueryString]:
         columns_str = ", ".join(
             f'"{col._meta.db_column_name}" = {{}}'
             for col, _ in self.values_delegate._values.items()
         )
 
-        query = f"UPDATE {self.table._meta.tablename} SET {columns_str}"
+        query = f"UPDATE {self.table._meta.get_formatted_tablename()} SET {columns_str}"  # noqa: E501
 
         querystring = QueryString(
             query, *self.values_delegate.get_sql_values()
         )
 
         if self.where_delegate._where:
+            # The JOIN syntax isn't allowed in SQL UPDATE queries, so we need
+            # to write the WHERE clause differently, using a sub select.
+
             querystring = QueryString(
                 "{} WHERE {}",
                 querystring,
-                self.where_delegate._where.querystring,
+                self.where_delegate._where.querystring_for_update,
             )
 
         if self.returning_delegate._returning:
             querystring = QueryString(
                 "{}{}",
                 querystring,
                 self.returning_delegate._returning.querystring,
```

### Comparing `piccolo-0.99.0/piccolo/querystring.py` & `piccolo-1.0a1/piccolo/querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/table.py` & `piccolo-1.0a1/piccolo/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import inspect
 import itertools
 import types
 import typing as t
+import warnings
 from dataclasses import dataclass, field
 
 from piccolo.columns import Column
 from piccolo.columns.column_types import (
     JSON,
     JSONB,
     Array,
@@ -22,14 +23,15 @@
     M2M,
     M2MAddRelated,
     M2MGetRelated,
     M2MRemoveRelated,
 )
 from piccolo.columns.readable import Readable
 from piccolo.columns.reference import LAZY_COLUMN_REFERENCES
+from piccolo.custom_types import TableInstance
 from piccolo.engine import Engine, engine_finder
 from piccolo.query import (
     Alter,
     Count,
     Create,
     Delete,
     DropIndex,
@@ -39,26 +41,31 @@
     Raw,
     Select,
     TableExists,
     Update,
 )
 from piccolo.query.methods.create_index import CreateIndex
 from piccolo.query.methods.indexes import Indexes
+from piccolo.query.methods.objects import First
 from piccolo.query.methods.refresh import Refresh
 from piccolo.querystring import QueryString, Unquoted
 from piccolo.utils import _camel_to_snake
 from piccolo.utils.graphlib import TopologicalSorter
 from piccolo.utils.sql_values import convert_to_sql_value
 from piccolo.utils.sync import run_sync
 from piccolo.utils.warnings import colored_warning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.columns import Selectable
 
 PROTECTED_TABLENAMES = ("user",)
+TABLENAME_WARNING = (
+    "We recommend giving your table a different name as `{tablename}` is a "
+    "reserved keyword. It should still work, but avoid if possible."
+)
 
 
 TABLE_REGISTRY: t.List[t.Type[Table]] = []
 
 
 @dataclass
 class TableMeta:
@@ -76,20 +83,44 @@
     json_columns: t.List[t.Union[JSON, JSONB]] = field(default_factory=list)
     secret_columns: t.List[Secret] = field(default_factory=list)
     auto_update_columns: t.List[Column] = field(default_factory=list)
     tags: t.List[str] = field(default_factory=list)
     help_text: t.Optional[str] = None
     _db: t.Optional[Engine] = None
     m2m_relationships: t.List[M2M] = field(default_factory=list)
+    schema: t.Optional[str] = None
 
     # Records reverse foreign key relationships - i.e. when the current table
     # is the target of a foreign key. Used by external libraries such as
     # Piccolo API.
     _foreign_key_references: t.List[ForeignKey] = field(default_factory=list)
 
+    def get_formatted_tablename(
+        self, include_schema: bool = True, quoted: bool = True
+    ) -> str:
+        """
+        Returns the tablename, in the desired format.
+
+        :param include_schema:
+            If ``True``, the Postgres schema is included. For example,
+            'my_schema.my_table'.
+        :param quote:
+            If ``True``, the name is wrapped in double quotes. For example,
+            '"my_schema"."my_table"'.
+
+        """
+        components = [self.tablename]
+        if include_schema and self.schema:
+            components.insert(0, self.schema)
+
+        if quoted:
+            return ".".join(f'"{i}"' for i in components)
+        else:
+            return ".".join(components)
+
     @property
     def foreign_key_references(self) -> t.List[ForeignKey]:
         foreign_keys: t.List[ForeignKey] = list(self._foreign_key_references)
         lazy_column_references = LAZY_COLUMN_REFERENCES.for_tablename(
             tablename=self.tablename
         )
         foreign_keys.extend(lazy_column_references)
@@ -191,14 +222,15 @@
 
     def __init_subclass__(
         cls,
         tablename: t.Optional[str] = None,
         db: t.Optional[Engine] = None,
         tags: t.List[str] = None,
         help_text: t.Optional[str] = None,
+        schema: t.Optional[str] = None,
     ):  # sourcery no-metrics
         """
         Automatically populate the _meta, which includes the tablename, and
         columns.
 
         :param tablename:
             Specify a custom tablename. By default the classname is converted
@@ -209,25 +241,31 @@
             imported from piccolo_conf.py using ``engine_finder``.
         :param tags:
             Used for filtering, for example by ``table_finder``.
         :param help_text:
             A user friendly description of what the table is used for. It isn't
             used in the database, but will be used by tools such a Piccolo
             Admin for tooltips.
+        :param schema:
+            The Postgres schema to use for this table.
 
         """
         if tags is None:
             tags = []
         tablename = tablename or _camel_to_snake(cls.__name__)
 
-        if tablename in PROTECTED_TABLENAMES:
-            raise ValueError(
-                f"{tablename} is a protected name, please give your table a "
-                "different name."
+        if "." in tablename:
+            warnings.warn(
+                "There's a '.' in the tablename - please use the `schema` "
+                "argument instead."
             )
+            schema, tablename = tablename.split(".", maxsplit=1)
+
+        if tablename in PROTECTED_TABLENAMES:
+            warnings.warn(TABLENAME_WARNING.format(tablename=tablename))
 
         columns: t.List[Column] = []
         default_columns: t.List[Column] = []
         non_default_columns: t.List[Column] = []
         foreign_key_columns: t.List[ForeignKey] = []
         secret_columns: t.List[Secret] = []
         json_columns: t.List[t.Union[JSON, JSONB]] = []
@@ -304,14 +342,15 @@
             json_columns=json_columns,
             secret_columns=secret_columns,
             auto_update_columns=auto_update_columns,
             tags=tags,
             help_text=help_text,
             _db=db,
             m2m_relationships=m2m_relationships,
+            schema=schema,
         )
 
         for foreign_key_column in foreign_key_columns:
             # ForeignKey columns require additional setup based on their
             # parent Table.
             foreign_key_setup_response = foreign_key_column._setup(
                 table_class=cls
@@ -359,14 +398,18 @@
             Used internally to track whether this row exists in the database.
 
         """
         _data = _data or {}
 
         self._exists_in_db = _exists_in_db
 
+        # This is used by get_or_create to indicate to the user whether it
+        # was an existing row or not.
+        self._was_created: t.Optional[bool] = None
+
         for column in self._meta.columns:
             value = _data.get(column, ...)
 
             if kwargs:
                 if value is ...:
                     value = kwargs.pop(column._meta.name, ...)
 
@@ -400,15 +443,17 @@
         pk = Serial(index=False, primary_key=True, db_column_name="id")
         pk._meta._name = "id"
         pk._meta._table = cls
 
         return pk
 
     @classmethod
-    def from_dict(cls, data: t.Dict[str, t.Any]) -> Table:
+    def from_dict(
+        cls: t.Type[TableInstance], data: t.Dict[str, t.Any]
+    ) -> TableInstance:
         """
         Used when loading fixtures. It can be overriden by subclasses in case
         they have specific logic / validation which needs running when loading
         fixtures.
         """
         return cls(**data)
 
@@ -509,15 +554,17 @@
 
             # Alternatively, running it synchronously:
             instance.refresh().run_sync()
 
         """
         return Refresh(instance=self, columns=columns)
 
-    def get_related(self, foreign_key: t.Union[ForeignKey, str]) -> Objects:
+    def get_related(
+        self: TableInstance, foreign_key: t.Union[ForeignKey, str]
+    ) -> First[Table]:
         """
         Used to fetch a ``Table`` instance, for the target of a foreign key.
 
         .. code-block:: python
 
             band = await Band.objects().first()
             manager = await band.get_related(Band.manager)
@@ -891,15 +938,17 @@
         _reference_column = reference_column.copy()
         _reference_column._meta.name = (
             f"{local_column_name}.{reference_column_name}"
         )
         return _reference_column
 
     @classmethod
-    def insert(cls, *rows: "Table") -> Insert:
+    def insert(
+        cls: t.Type[TableInstance], *rows: TableInstance
+    ) -> Insert[TableInstance]:
         """
         Insert rows into the database.
 
         .. code-block:: python
 
             await Band.insert(
                 Band(name="Pythonistas", popularity=500, manager=1)
@@ -920,15 +969,15 @@
 
             await Band.raw('select * from band')
 
         Or passing in parameters:
 
         .. code-block:: python
 
-            await Band.raw("select * from band where name = {}", 'Pythonistas')
+            await Band.raw("SELECT * FROM band WHERE name = {}", 'Pythonistas')
 
         """
         return Raw(table=cls, querystring=QueryString(sql, *args))
 
     @classmethod
     def _process_column_args(
         cls, *columns: t.Union[Selectable, str]
@@ -988,28 +1037,32 @@
             ``where`` clause, to prevent accidental mass deletions.
 
         """
         return Delete(table=cls, force=force)
 
     @classmethod
     def create_table(
-        cls, if_not_exists=False, only_default_columns=False
+        cls,
+        if_not_exists=False,
+        only_default_columns=False,
+        auto_create_schema: bool = True,
     ) -> Create:
         """
         Create table, along with all columns.
 
         .. code-block:: python
 
             await Band.create_table()
 
         """
         return Create(
             table=cls,
             if_not_exists=if_not_exists,
             only_default_columns=only_default_columns,
+            auto_create_schema=auto_create_schema,
         )
 
     @classmethod
     def alter(cls) -> Alter:
         """
         Used to modify existing tables and columns.
 
@@ -1018,16 +1071,17 @@
             await Band.alter().rename_column(Band.popularity, 'rating')
 
         """
         return Alter(table=cls)
 
     @classmethod
     def objects(
-        cls, *prefetch: t.Union[ForeignKey, t.List[ForeignKey]]
-    ) -> Objects:
+        cls: t.Type[TableInstance],
+        *prefetch: t.Union[ForeignKey, t.List[ForeignKey]],
+    ) -> Objects[TableInstance]:
         """
         Returns a list of table instances (each representing a row), which you
         can modify and then call 'save' on, or can delete by calling 'remove'.
 
         .. code-block:: python
 
             pythonistas = await Band.objects().where(
@@ -1054,27 +1108,65 @@
 
                 # With nested
                 band = await Band.objects(Band.manager).first()
                 >>> band.manager
                 <Band 1>
 
         """
-        return Objects(table=cls, prefetch=prefetch)
+        return Objects[TableInstance](table=cls, prefetch=prefetch)
 
     @classmethod
-    def count(cls) -> Count:
-        """
-        Count the number of matching rows.
+    def count(
+        cls,
+        column: t.Optional[Column] = None,
+        distinct: t.Optional[t.Sequence[Column]] = None,
+    ) -> Count:
 
-        .. code-block:: python
+        """
+        Count the number of matching rows::
 
             await Band.count().where(Band.popularity > 1000)
 
+        :param column:
+            If specified, just count rows where this column isn't null.
+
+        :param distinct:
+            Counts the number of distinct values for these columns. For
+            example, if we have a concerts table::
+
+                class Concert(Table):
+                    band = Varchar()
+                    start_date = Date()
+
+            With this data:
+
+            .. table::
+                :widths: auto
+
+                ===========  ==========
+                band         start_date
+                ===========  ==========
+                Pythonistas  2023-01-01
+                Pythonistas  2023-02-03
+                Rustaceans   2023-01-01
+                ===========  ==========
+
+            Without the ``distinct`` argument, we get the count of all
+            rows::
+
+                >>> await Concert.count()
+                3
+
+            To get the number of unique concert dates::
+
+                >>> await Concert.count(distinct=[Concert.start_date])
+                2
+
         """
-        return Count(table=cls)
+        return Count(table=cls, column=column, distinct=distinct)
 
     @classmethod
     def exists(cls) -> Exists:
         """
         Use it to check if a row exists, not if the table exists.
 
         .. code-block:: python
```

### Comparing `piccolo-0.99.0/piccolo/table_reflection.py` & `piccolo-1.0a1/piccolo/table_reflection.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/testing/model_builder.py` & `piccolo-1.0a1/piccolo/testing/model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import json
 import typing as t
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from uuid import UUID
 
-from piccolo.columns import Array, Column
-from piccolo.table import Table
+from piccolo.columns import Array, Column, ForeignKey
+from piccolo.custom_types import TableInstance
 from piccolo.testing.random_builder import RandomBuilder
 from piccolo.utils.sync import run_sync
 
 
 class ModelBuilder:
     __DEFAULT_MAPPER: t.Dict[t.Type, t.Callable] = {
         bool: RandomBuilder.next_bool,
@@ -23,19 +25,19 @@
         timedelta: RandomBuilder.next_timedelta,
         UUID: RandomBuilder.next_uuid,
     }
 
     @classmethod
     async def build(
         cls,
-        table_class: t.Type[Table],
+        table_class: t.Type[TableInstance],
         defaults: t.Dict[t.Union[Column, str], t.Any] = None,
         persist: bool = True,
         minimal: bool = False,
-    ) -> Table:
+    ) -> TableInstance:
         """
         Build a ``Table`` instance with random data and save async.
         If the ``Table`` has any foreign keys, then the related rows are also
         created automatically.
 
         :param table_class:
             Table class to randomize.
@@ -74,19 +76,19 @@
             persist=persist,
             minimal=minimal,
         )
 
     @classmethod
     def build_sync(
         cls,
-        table_class: t.Type[Table],
+        table_class: t.Type[TableInstance],
         defaults: t.Dict[t.Union[Column, str], t.Any] = None,
         persist: bool = True,
         minimal: bool = False,
-    ) -> Table:
+    ) -> TableInstance:
         """
         A sync wrapper around :meth:`build`.
         """
         return run_sync(
             cls.build(
                 table_class=table_class,
                 defaults=defaults,
@@ -94,19 +96,19 @@
                 minimal=minimal,
             )
         )
 
     @classmethod
     async def _build(
         cls,
-        table_class: t.Type[Table],
+        table_class: t.Type[TableInstance],
         defaults: t.Dict[t.Union[Column, str], t.Any] = None,
         minimal: bool = False,
         persist: bool = True,
-    ) -> Table:
+    ) -> TableInstance:
         model = table_class(_ignore_missing=True)
         defaults = {} if not defaults else defaults
 
         for column, value in defaults.items():
             if isinstance(column, str):
                 column = model._meta.get_column_by_name(column)
 
@@ -116,17 +118,17 @@
 
             if column._meta.null and minimal:
                 continue
 
             if column._meta.name in defaults:
                 continue  # Column value exists
 
-            if "references" in column._meta.params and persist:
+            if isinstance(column, ForeignKey) and persist:
                 reference_model = await cls._build(
-                    column._meta.params["references"],
+                    column._foreign_key_meta.resolved_references,
                     persist=True,
                 )
                 random_value = getattr(
                     reference_model,
                     reference_model._meta.primary_key._meta.name,
                 )
             else:
@@ -146,15 +148,15 @@
 
         :param column:
             Column class to randomize.
 
         """
         random_value: t.Any
         if column.value_type == Decimal:
-            precision, scale = column._meta.params["digits"]
+            precision, scale = column._meta.params["digits"] or (4, 2)
             random_value = RandomBuilder.next_float(
                 maximum=10 ** (precision - scale), scale=scale
             )
         elif column.value_type == list:
             length = RandomBuilder.next_int(maximum=10)
             base_type = t.cast(Array, column).base_column.value_type
             random_value = [
```

### Comparing `piccolo-0.99.0/piccolo/testing/random_builder.py` & `piccolo-1.0a1/piccolo/testing/random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/dictionary.py` & `piccolo-1.0a1/piccolo/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/encoding.py` & `piccolo-1.0a1/piccolo/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/graphlib/_graphlib.py` & `piccolo-1.0a1/piccolo/utils/graphlib/_graphlib.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/lazy_loader.py` & `piccolo-1.0a1/piccolo/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/objects.py` & `piccolo-1.0a1/piccolo/utils/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/repr.py` & `piccolo-1.0a1/piccolo/utils/repr.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/sync.py` & `piccolo-1.0a1/piccolo/utils/sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo/utils/warnings.py` & `piccolo-1.0a1/piccolo/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/piccolo.egg-info/PKG-INFO` & `piccolo-1.0a1/piccolo.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,139 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 0.99.0
+Version: 1.0a1
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
 Project-URL: Tracker, https://github.com/piccolo-orm/piccolo/issues
-Description: ![Logo](https://raw.githubusercontent.com/piccolo-orm/piccolo/master/docs/logo_hero.png "Piccolo Logo")
-        
-        ![Tests](https://github.com/piccolo-orm/piccolo/actions/workflows/tests.yaml/badge.svg)
-        ![Release](https://github.com/piccolo-orm/piccolo/actions/workflows/release.yaml/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/piccolo-orm/badge/?version=latest)](https://piccolo-orm.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/piccolo?color=%2334D058&label=pypi)](https://pypi.org/project/piccolo/)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/piccolo-orm/piccolo.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/piccolo-orm/piccolo/context:python)
-        [![Total alerts](https://img.shields.io/lgtm/alerts/g/piccolo-orm/piccolo.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/piccolo-orm/piccolo/alerts/)
-        [![codecov](https://codecov.io/gh/piccolo-orm/piccolo/branch/master/graph/badge.svg?token=V19CWH7MXX)](https://codecov.io/gh/piccolo-orm/piccolo)
-        
-        Piccolo is a fast, user friendly ORM and query builder which supports asyncio. [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/).
-        
-        ## Features
-        
-        Some of it’s stand out features are:
-        
-        - Support for sync and async.
-        - A builtin playground, which makes learning a breeze.
-        - Tab completion support - works great with iPython and VSCode.
-        - Batteries included - a User model, authentication, migrations, an [admin GUI](https://github.com/piccolo-orm/piccolo_admin), and more.
-        - Modern Python - fully type annotated.
-        - Make your codebase modular and scalable with Piccolo apps (similar to Django apps).
-        
-        ## Syntax
-        
-        The syntax is clean and expressive.
-        
-        You can use it as a query builder:
-        
-        ```python
-        # Select:
-        await Band.select(
-            Band.name
-        ).where(
-            Band.popularity > 100
-        )
-        
-        # Join:
-        await Band.select(
-            Band.name,
-            Band.manager.name
-        )
-        
-        # Delete:
-        await Band.delete().where(
-            Band.popularity < 1000
-        )
-        
-        # Update:
-        await Band.update({Band.popularity: 10000}).where(
-            Band.name == 'Pythonistas'
-        )
-        ```
-        
-        Or like a typical ORM:
-        
-        ```python
-        # To create a new object:
-        b = Band(name='C-Sharps', popularity=100)
-        await b.save()
-        
-        # To fetch an object from the database, and update it:
-        b = await Band.objects().get(Band.name == 'Pythonistas')
-        b.popularity = 10000
-        await b.save()
-        
-        # To delete:
-        await b.remove()
-        ```
-        
-        ## Installation
-        
-        Installing with PostgreSQL driver:
-        
-        ```bash
-        pip install 'piccolo[postgres]'
-        ```
-        
-        Installing with SQLite driver:
-        
-        ```bash
-        pip install 'piccolo[sqlite]'
-        ```
-        
-        Installing with all optional dependencies (easiest):
-        
-        ```bash
-        pip install 'piccolo[all]'
-        ```
-        
-        ## Building a web app?
-        
-        Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
-        
-        ```bash
-        piccolo asgi new
-        ```
-        
-        [Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Xpresso](https://xpresso-api.dev/) and [Starlite](https://starlite-api.github.io/starlite/) are currently supported.
-        
-        ## Are you a Django user?
-        
-        We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
-        
-        ## Documentation
-        
-        Our documentation is on [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/piccolo/getting_started/index.html).
-        
-        We also have some great [tutorial videos on YouTube](https://www.youtube.com/channel/UCE7x5nm1Iy9KDfXPNrNQ5lA).
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Framework :: AsyncIO
 Classifier: Typing :: Typed
 Classifier: Topic :: Database
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: orjson
 Provides-Extra: playground
 Provides-Extra: postgres
 Provides-Extra: sqlite
 Provides-Extra: uvloop
 Provides-Extra: all
+License-File: LICENSE
+
+![Logo](https://raw.githubusercontent.com/piccolo-orm/piccolo/master/docs/logo_hero.png "Piccolo Logo")
+
+![Tests](https://github.com/piccolo-orm/piccolo/actions/workflows/tests.yaml/badge.svg)
+![Release](https://github.com/piccolo-orm/piccolo/actions/workflows/release.yaml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/piccolo-orm/badge/?version=latest)](https://piccolo-orm.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/piccolo?color=%2334D058&label=pypi)](https://pypi.org/project/piccolo/)
+[![codecov](https://codecov.io/gh/piccolo-orm/piccolo/branch/master/graph/badge.svg?token=V19CWH7MXX)](https://codecov.io/gh/piccolo-orm/piccolo)
+
+Piccolo is a fast, user friendly ORM and query builder which supports asyncio. [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/).
+
+## Features
+
+Some of it’s stand out features are:
+
+- Support for sync and async.
+- A builtin playground, which makes learning a breeze.
+- Tab completion support - works great with iPython and VSCode.
+- Batteries included - a User model, authentication, migrations, an [admin GUI](https://github.com/piccolo-orm/piccolo_admin), and more.
+- Modern Python - fully type annotated.
+- Make your codebase modular and scalable with Piccolo apps (similar to Django apps).
+
+## Syntax
+
+The syntax is clean and expressive.
+
+You can use it as a query builder:
+
+```python
+# Select:
+await Band.select(
+    Band.name
+).where(
+    Band.popularity > 100
+)
+
+# Join:
+await Band.select(
+    Band.name,
+    Band.manager.name
+)
+
+# Delete:
+await Band.delete().where(
+    Band.popularity < 1000
+)
+
+# Update:
+await Band.update({Band.popularity: 10000}).where(
+    Band.name == 'Pythonistas'
+)
+```
+
+Or like a typical ORM:
+
+```python
+# To create a new object:
+b = Band(name='C-Sharps', popularity=100)
+await b.save()
+
+# To fetch an object from the database, and update it:
+b = await Band.objects().get(Band.name == 'Pythonistas')
+b.popularity = 10000
+await b.save()
+
+# To delete:
+await b.remove()
+```
+
+## Installation
+
+Installing with PostgreSQL driver:
+
+```bash
+pip install 'piccolo[postgres]'
+```
+
+Installing with SQLite driver:
+
+```bash
+pip install 'piccolo[sqlite]'
+```
+
+Installing with all optional dependencies (easiest):
+
+```bash
+pip install 'piccolo[all]'
+```
+
+## Building a web app?
+
+Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
+
+```bash
+piccolo asgi new
+```
+
+[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/) and [Litestar](https://litestar.dev/) are currently supported.
+
+## Are you a Django user?
+
+We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
+
+## Documentation
+
+Our documentation is on [Read the docs](https://piccolo-orm.readthedocs.io/en/latest/piccolo/getting_started/index.html).
+
+We also have some great [tutorial videos on YouTube](https://www.youtube.com/channel/UCE7x5nm1Iy9KDfXPNrNQ5lA).
```

### Comparing `piccolo-0.99.0/piccolo.egg-info/SOURCES.txt` & `piccolo-1.0a1/piccolo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 piccolo/__init__.py
 piccolo/custom_types.py
 piccolo/main.py
 piccolo/py.typed
 piccolo/querystring.py
+piccolo/schema.py
 piccolo/table.py
 piccolo/table_reflection.py
 piccolo.egg-info/PKG-INFO
 piccolo.egg-info/SOURCES.txt
 piccolo.egg-info/dependency_links.txt
 piccolo.egg-info/entry_points.txt
 piccolo.egg-info/requires.txt
@@ -25,28 +27,26 @@
 piccolo/apps/asgi/__init__.py
 piccolo/apps/asgi/piccolo_app.py
 piccolo/apps/asgi/commands/__init__.py
 piccolo/apps/asgi/commands/new.py
 piccolo/apps/asgi/commands/templates/app/README.md.jinja
 piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
+piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
-piccolo/apps/asgi/commands/templates/app/_starlite_app.py.jinja
-piccolo/apps/asgi/commands/templates/app/_xpresso_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/app.py.jinja
 piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
 piccolo/apps/asgi/commands/templates/app/main.py.jinja
 piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
 piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
 piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
 piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
+piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
-piccolo/apps/asgi/commands/templates/app/home/_starlite_endpoints.py.jinja
-piccolo/apps/asgi/commands/templates/app/home/_xpresso_endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
 piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
 piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
 piccolo/apps/asgi/commands/templates/app/static/favicon.ico
@@ -149,14 +149,15 @@
 piccolo/engine/exceptions.py
 piccolo/engine/finder.py
 piccolo/engine/postgres.py
 piccolo/engine/sqlite.py
 piccolo/query/__init__.py
 piccolo/query/base.py
 piccolo/query/mixins.py
+piccolo/query/proxy.py
 piccolo/query/methods/__init__.py
 piccolo/query/methods/alter.py
 piccolo/query/methods/count.py
 piccolo/query/methods/create.py
 piccolo/query/methods/create_index.py
 piccolo/query/methods/delete.py
 piccolo/query/methods/drop_index.py
@@ -172,14 +173,15 @@
 piccolo/testing/__init__.py
 piccolo/testing/model_builder.py
 piccolo/testing/random_builder.py
 piccolo/utils/__init__.py
 piccolo/utils/dictionary.py
 piccolo/utils/encoding.py
 piccolo/utils/lazy_loader.py
+piccolo/utils/list.py
 piccolo/utils/naming.py
 piccolo/utils/objects.py
 piccolo/utils/printing.py
 piccolo/utils/pydantic.py
 piccolo/utils/repr.py
 piccolo/utils/sql_values.py
 piccolo/utils/sync.py
@@ -249,32 +251,36 @@
 tests/columns/test_date.py
 tests/columns/test_db_column_name.py
 tests/columns/test_defaults.py
 tests/columns/test_double_precision.py
 tests/columns/test_interval.py
 tests/columns/test_json.py
 tests/columns/test_jsonb.py
-tests/columns/test_m2m.py
 tests/columns/test_numeric.py
 tests/columns/test_primary_key.py
 tests/columns/test_readable.py
 tests/columns/test_real.py
 tests/columns/test_reference.py
 tests/columns/test_reserved_column_names.py
 tests/columns/test_smallint.py
 tests/columns/test_time.py
 tests/columns/test_timestamp.py
 tests/columns/test_timestamptz.py
 tests/columns/test_uuid.py
 tests/columns/test_varchar.py
+tests/columns/m2m/__init__.py
+tests/columns/m2m/base.py
+tests/columns/m2m/test_m2m.py
+tests/columns/m2m/test_m2m_schema.py
 tests/conf/__init__.py
 tests/conf/example.py
 tests/conf/test_apps.py
 tests/engine/__init__.py
 tests/engine/test_extra_nodes.py
+tests/engine/test_logging.py
 tests/engine/test_nested_transaction.py
 tests/engine/test_pool.py
 tests/engine/test_transaction.py
 tests/engine/test_version_parsing.py
 tests/example_apps/__init__.py
 tests/example_apps/mega/__init__.py
 tests/example_apps/mega/piccolo_app.py
@@ -309,14 +315,15 @@
 tests/table/test_drop_db_tables.py
 tests/table/test_exists.py
 tests/table/test_from_dict.py
 tests/table/test_indexes.py
 tests/table/test_inheritance.py
 tests/table/test_insert.py
 tests/table/test_join.py
+tests/table/test_join_on.py
 tests/table/test_metaclass.py
 tests/table/test_objects.py
 tests/table/test_output.py
 tests/table/test_raw.py
 tests/table/test_ref.py
 tests/table/test_refresh.py
 tests/table/test_repr.py
@@ -335,14 +342,15 @@
 tests/testing/__init__.py
 tests/testing/test_model_builder.py
 tests/testing/test_random_builder.py
 tests/utils/__init__.py
 tests/utils/test_dictionary.py
 tests/utils/test_encoding.py
 tests/utils/test_lazy_loader.py
+tests/utils/test_list.py
 tests/utils/test_naming.py
 tests/utils/test_printing.py
 tests/utils/test_pydantic.py
 tests/utils/test_sql_values.py
 tests/utils/test_sync.py
 tests/utils/test_table_reflection.py
 tests/utils/test_warnings.py
```

### Comparing `piccolo-0.99.0/profiling/run_profile.py` & `piccolo-1.0a1/profiling/run_profile.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/pyproject.toml` & `piccolo-1.0a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 line-length = 79
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310']
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.mypy]
 [[tool.mypy.overrides]]
@@ -20,21 +20,23 @@
 ]
 ignore_missing_imports = true
 
 
 [tool.pytest.ini_options]
 markers = [
     "integration",
+    "speed"
 ]
 
 [tool.coverage.run]
 omit = [
     "*.jinja",
     "**/piccolo_migrations/*",
-    "**/piccolo_app.py"
+    "**/piccolo_app.py",
+    "**/utils/graphlib/*",
 ]
 
 [tool.coverage.report]
 # Note, we have to re-specify "pragma: no cover"
 # https://coverage.readthedocs.io/en/6.3.3/excluding.html#advanced-exclusion
 exclude_lines = [
     "raise NotImplementedError",
```

### Comparing `piccolo-0.99.0/setup.py` & `piccolo-1.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     description=(
         "A fast, user friendly ORM and query builder which supports asyncio."
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author="Daniel Townsend",
     author_email="dan@dantownsend.co.uk",
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     url="https://github.com/piccolo-orm/piccolo",
     packages=find_packages(exclude=("tests",)),
     package_data={
         "": [
             "templates/*",
             "templates/**/*",
             "templates/**/**/*",
@@ -80,15 +80,14 @@
     install_requires=parse_requirement("requirements.txt"),
     extras_require=extras_require(),
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Framework :: AsyncIO",
         "Typing :: Typed",
```

### Comparing `piccolo-0.99.0/tests/apps/app/commands/test_new.py` & `piccolo-1.0a1/tests/apps/app/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/app/commands/test_show_all.py` & `piccolo-1.0a1/tests/apps/app/commands/test_show_all.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/asgi/commands/test_new.py` & `piccolo-1.0a1/tests/apps/asgi/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/fixtures/commands/test_dump_load.py` & `piccolo-1.0a1/tests/apps/fixtures/commands/test_dump_load.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import datetime
 import decimal
+import os
+import tempfile
+import typing as t
 import uuid
 from unittest import TestCase
 
 from piccolo.apps.fixtures.commands.dump import (
     FixtureConfig,
     dump_to_json_string,
 )
-from piccolo.apps.fixtures.commands.load import load_json_string
+from piccolo.apps.fixtures.commands.load import load, load_json_string
 from piccolo.utils.sync import run_sync
 from tests.base import engines_only
 from tests.example_apps.mega.tables import MegaTable, SmallTable
 
 
 class TestDumpLoad(TestCase):
     """
@@ -25,18 +28,20 @@
         for table_class in (SmallTable, MegaTable):
             table_class.create_table().run_sync()
 
     def tearDown(self):
         for table_class in (MegaTable, SmallTable):
             table_class.alter().drop_table().run_sync()
 
-    def insert_row(self):
+    def insert_rows(self):
         small_table = SmallTable(varchar_col="Test")
         small_table.save().run_sync()
 
+        SmallTable(varchar_col="Test 2").save().run_sync()
+
         mega_table = MegaTable(
             bigint_col=1,
             boolean_col=True,
             bytea_col="hello".encode("utf8"),
             date_col=datetime.date(year=2021, month=1, day=1),
             foreignkey_col=small_table,
             integer_col=1,
@@ -56,44 +61,42 @@
             varchar_col="hello",
             unique_col="hello",
             null_col=None,
             not_null_col="hello",
         )
         mega_table.save().run_sync()
 
-    @engines_only("postgres", "sqlite")
-    def test_dump_load(self):
-        """
-        Make sure we can dump some rows into a JSON fixture, then load them
-        back into the database.
-        """
-        self.insert_row()
+    def _run_comparison(self, table_class_names: t.List[str]):
+        self.insert_rows()
 
         json_string = run_sync(
             dump_to_json_string(
                 fixture_configs=[
                     FixtureConfig(
                         app_name="mega",
-                        table_class_names=["SmallTable", "MegaTable"],
+                        table_class_names=table_class_names,
                     )
                 ]
             )
         )
 
         # We need to clear the data out now, otherwise when loading the data
-        # back in, there will be a constraint errors over clashing primary
+        # back in, there will be constraint errors over clashing primary
         # keys.
         SmallTable.delete(force=True).run_sync()
         MegaTable.delete(force=True).run_sync()
 
         run_sync(load_json_string(json_string))
 
         self.assertEqual(
             SmallTable.select().run_sync(),
-            [{"id": 1, "varchar_col": "Test"}],
+            [
+                {"id": 1, "varchar_col": "Test"},
+                {"id": 2, "varchar_col": "Test 2"},
+            ],
         )
 
         mega_table_data = MegaTable.select().run_sync()
 
         # Real numbers don't have perfect precision when coming back from the
         # database, so we need to round them to be able to compare them.
         mega_table_data[0]["real_col"] = round(
@@ -134,35 +137,54 @@
                 "varchar_col": "hello",
                 "unique_col": "hello",
                 "null_col": None,
                 "not_null_col": "hello",
             },
         )
 
-    @engines_only("cockroach")
-    def test_dump_load_alt(self):
+        # Make sure subsequent inserts work.
+        SmallTable().save().run_sync()
+
+    @engines_only("postgres", "sqlite")
+    def test_dump_load(self):
         """
         Make sure we can dump some rows into a JSON fixture, then load them
         back into the database.
         """
-        self.insert_row()
+        self._run_comparison(table_class_names=["SmallTable", "MegaTable"])
+
+    @engines_only("postgres", "sqlite")
+    def test_dump_load_ordering(self):
+        """
+        Similar to `test_dump_load` - but we need to make sure it inserts
+        the data in the correct order, so foreign key constraints don't fail.
+        """
+        self._run_comparison(table_class_names=["MegaTable", "SmallTable"])
+
+    @engines_only("cockroach")
+    def test_dump_load_cockroach(self):
+        """
+        Similar to `test_dump_load`, except the schema is slightly different
+        for CockroachDB.
+        """
+        self.insert_rows()
 
         json_string = run_sync(
             dump_to_json_string(
                 fixture_configs=[
                     FixtureConfig(
                         app_name="mega",
                         table_class_names=["SmallTable", "MegaTable"],
                     )
                 ]
             )
         )
 
         # We need to clear the data out now, otherwise when loading the data
-        # back in, there will be a constraint errors over clashing primary
+        # back in, there will be constraint errors over clashing primary
         # keys.
         SmallTable.delete(force=True).run_sync()
         MegaTable.delete(force=True).run_sync()
 
         run_sync(load_json_string(json_string))
 
         result = SmallTable.select().run_sync()[0]
@@ -216,7 +238,43 @@
                 "uuid_col": uuid.UUID("12783854-c012-4c15-8183-8eecb46f2c4e"),
                 "varchar_col": "hello",
                 "unique_col": "hello",
                 "null_col": None,
                 "not_null_col": "hello",
             },
         )
+
+
+class TestOnConflict(TestCase):
+    def setUp(self) -> None:
+        SmallTable.create_table().run_sync()
+        SmallTable({SmallTable.varchar_col: "Test"}).save().run_sync()
+
+    def tearDown(self) -> None:
+        SmallTable.alter().drop_table().run_sync()
+
+    def test_on_conflict(self):
+        temp_dir = tempfile.gettempdir()
+
+        json_file_path = os.path.join(temp_dir, "fixture.json")
+
+        json_string = run_sync(
+            dump_to_json_string(
+                fixture_configs=[
+                    FixtureConfig(
+                        app_name="mega",
+                        table_class_names=["SmallTable"],
+                    )
+                ]
+            )
+        )
+
+        if os.path.exists(json_file_path):
+            os.unlink(json_file_path)
+
+        with open(json_file_path, "w") as f:
+            f.write(json_string)
+
+        run_sync(load(path=json_file_path, on_conflict="DO NOTHING"))
+        run_sync(load(path=json_file_path, on_conflict="DO UPDATE"))
+        run_sync(load(path=json_file_path, on_conflict="do nothing"))
+        run_sync(load(path=json_file_path, on_conflict="do update"))
```

### Comparing `piccolo-0.99.0/tests/apps/fixtures/commands/test_shared.py` & `piccolo-1.0a1/tests/apps/fixtures/commands/test_shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/migrations/auto/integration/test_migrations.py` & `piccolo-1.0a1/tests/apps/migrations/auto/test_migration_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1029 +1,1053 @@
-from __future__ import annotations
-
-import datetime
-import decimal
-import os
+import asyncio
 import random
-import shutil
-import tempfile
-import time
-import typing as t
-import uuid
+from io import StringIO
+from unittest import TestCase
 from unittest.mock import MagicMock, patch
 
-from piccolo.apps.migrations.commands.forwards import ForwardsMigrationManager
-from piccolo.apps.migrations.commands.new import (
-    _create_migrations_folder,
-    _create_new_migration,
-)
-from piccolo.apps.migrations.tables import Migration
-from piccolo.apps.schema.commands.generate import RowMeta
-from piccolo.columns.column_types import (
-    JSON,
-    JSONB,
-    UUID,
-    Array,
-    BigInt,
-    BigSerial,
-    Boolean,
-    Date,
-    Decimal,
-    DoublePrecision,
-    ForeignKey,
-    Integer,
-    Interval,
-    Numeric,
-    Real,
-    Serial,
-    SmallInt,
-    Text,
-    Time,
-    Timestamp,
-    Timestamptz,
-    Varchar,
-)
-from piccolo.columns.defaults.uuid import UUID4
-from piccolo.columns.m2m import M2M
-from piccolo.columns.reference import LazyTableReference
+from piccolo.apps.migrations.auto.migration_manager import MigrationManager
+from piccolo.apps.migrations.commands.base import BaseMigrationManager
+from piccolo.columns import Text, Varchar
+from piccolo.columns.base import OnDelete, OnUpdate
+from piccolo.columns.column_types import ForeignKey
 from piccolo.conf.apps import AppConfig
-from piccolo.table import Table, create_table_class, drop_db_tables_sync
-from piccolo.utils.sync import run_sync
-from tests.base import DBTestCase, engines_only, engines_skip
+from piccolo.table import Table, sort_table_classes
+from piccolo.utils.lazy_loader import LazyLoader
+from tests.base import AsyncMock, DBTestCase, engine_is, engines_only
+from tests.example_apps.music.tables import Band, Concert, Manager, Venue
 
-if t.TYPE_CHECKING:
-    from piccolo.columns.base import Column
+asyncpg = LazyLoader("asyncpg", globals(), "asyncpg")
 
 
-def string_default():
-    return "hello world"
+class TestSortTableClasses(TestCase):
+    def test_sort_table_classes(self):
+        """
+        Make sure simple use cases work correctly.
+        """
+        self.assertListEqual(
+            sort_table_classes([Manager, Band]), [Manager, Band]
+        )
+        self.assertListEqual(
+            sort_table_classes([Band, Manager]), [Manager, Band]
+        )
 
+        sorted_tables = sort_table_classes([Manager, Venue, Concert, Band])
+        self.assertTrue(
+            sorted_tables.index(Manager) < sorted_tables.index(Band)
+        )
+        self.assertTrue(
+            sorted_tables.index(Venue) < sorted_tables.index(Concert)
+        )
+        self.assertTrue(
+            sorted_tables.index(Band) < sorted_tables.index(Concert)
+        )
 
-def integer_default():
-    return 1
+    def test_sort_unrelated_tables(self):
+        """
+        Make sure there are no weird edge cases with tables with no foreign
+        key relationships with each other.
+        """
 
+        class TableA(Table):
+            pass
 
-def uuid_default():
-    return uuid.uuid4()
+        class TableB(Table):
+            pass
 
+        self.assertListEqual(
+            sort_table_classes([TableA, TableB]), [TableA, TableB]
+        )
 
-def datetime_default():
-    return datetime.datetime.now()
+    def test_single_table(self):
+        """
+        Make sure that sorting a list with only a single table in it still
+        works.
+        """
+        self.assertListEqual(sort_table_classes([Band]), [Band])
 
+    def test_recursive_table(self):
+        """
+        Make sure that a table with a foreign key to itself sorts without
+        issues.
+        """
 
-def time_default():
-    return datetime.datetime.now().time()
+        class TableA(Table):
+            table_a = ForeignKey("self")
 
+        class TableB(Table):
+            table_a = ForeignKey(TableA)
 
-def date_default():
-    return datetime.datetime.now().date()
+        self.assertListEqual(
+            sort_table_classes([TableA, TableB]), [TableA, TableB]
+        )
 
+    def test_long_chain(self):
+        """
+        Make sure sorting works when there are a lot of tables with foreign
+        keys to each other.
 
-def timedelta_default():
-    return datetime.timedelta(days=1)
+        https://github.com/piccolo-orm/piccolo/issues/616
 
+        """
 
-def boolean_default():
-    return True
+        class TableA(Table):
+            pass
 
+        class TableB(Table):
+            fk = ForeignKey(TableA)
 
-def numeric_default():
-    return decimal.Decimal("1.2")
+        class TableC(Table):
+            fk = ForeignKey(TableB)
 
+        class TableD(Table):
+            fk = ForeignKey(TableC)
 
-def array_default_integer():
-    return [4, 5, 6]
+        class TableE(Table):
+            fk = ForeignKey(TableD)
 
+        tables = [TableA, TableB, TableC, TableD, TableE]
 
-def array_default_varchar():
-    return ["x", "y", "z"]
+        shuffled_tables = random.sample(tables, len(tables))
 
+        self.assertListEqual(sort_table_classes(shuffled_tables), tables)
 
-class MigrationTestCase(DBTestCase):
-    def run_migrations(self, app_config: AppConfig):
-        manager = ForwardsMigrationManager(app_name=app_config.app_name)
-        run_sync(manager.create_migration_table())
-        run_sync(manager.run_migrations(app_config=app_config))
 
-    def _test_migrations(
-        self,
-        table_snapshots: t.List[t.List[t.Type[Table]]],
-        test_function: t.Optional[t.Callable[[RowMeta], None]] = None,
-    ):
+class TestMigrationManager(DBTestCase):
+    @engines_only("postgres", "cockroach")
+    def test_rename_column(self):
         """
-        Writes a migration file to disk and runs it.
+        Test running a MigrationManager which contains a column rename
+        operation.
+        """
+        self.insert_row()
 
-        :param table_snapshots:
-            A list of lists. Each sub list represents a snapshot of the table
-            state. Migrations will be created and run based each snapshot.
-        :param test_function:
-            After the migrations are run, this function is called. It is passed
-            a ``RowMeta`` instance which can be used to check the column was
-            created correctly in the database. It should return ``True`` if the
-            test passes, otherwise ``False``.
+        manager = MigrationManager()
+        manager.rename_column(
+            table_class_name="Band",
+            tablename="band",
+            old_column_name="name",
+            new_column_name="title",
+        )
+        asyncio.run(manager.run())
 
+        response = self.run_sync("SELECT * FROM band;")
+        self.assertTrue("title" in response[0].keys())
+        self.assertTrue("name" not in response[0].keys())
+
+        # Reverse
+        asyncio.run(manager.run(backwards=True))
+        response = self.run_sync("SELECT * FROM band;")
+        self.assertTrue("title" not in response[0].keys())
+        self.assertTrue("name" in response[0].keys())
+
+        # Preview
+        manager.preview = True
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            asyncio.run(manager.run())
+            self.assertEqual(
+                fake_out.getvalue(),
+                """  -  [preview forwards]... \n ALTER TABLE "band" RENAME COLUMN "name" TO "title";\n""",  # noqa: E501
+            )
+        response = self.run_sync("SELECT * FROM band;")
+        self.assertTrue("title" not in response[0].keys())
+        self.assertTrue("name" in response[0].keys())
+
+    def test_raw_function(self):
         """
-        temp_directory_path = tempfile.gettempdir()
-        migrations_folder_path = os.path.join(
-            temp_directory_path, "piccolo_migrations"
-        )
+        Test adding raw functions to a MigrationManager.
+        """
+
+        class HasRun(Exception):
+            pass
+
+        class HasRunBackwards(Exception):
+            pass
+
+        def run():
+            raise HasRun("I was run!")
+
+        def run_back():
+            raise HasRunBackwards("I was run backwards!")
+
+        manager = MigrationManager()
+        manager.add_raw(run)
+        manager.add_raw_backwards(run_back)
+
+        with self.assertRaises(HasRun):
+            asyncio.run(manager.run())
+
+        # Reverse
+        with self.assertRaises(HasRunBackwards):
+            asyncio.run(manager.run(backwards=True))
+
+    def test_raw_coroutine(self):
+        """
+        Test adding raw coroutines to a MigrationManager.
+        """
+
+        class HasRun(Exception):
+            pass
+
+        class HasRunBackwards(Exception):
+            pass
+
+        async def run():
+            raise HasRun("I was run!")
+
+        async def run_back():
+            raise HasRunBackwards("I was run backwards!")
+
+        manager = MigrationManager()
+        manager.add_raw(run)
+        manager.add_raw_backwards(run_back)
 
-        if os.path.exists(migrations_folder_path):
-            shutil.rmtree(migrations_folder_path)
+        with self.assertRaises(HasRun):
+            asyncio.run(manager.run())
 
-        _create_migrations_folder(migrations_folder_path)
+        # Reverse
+        with self.assertRaises(HasRunBackwards):
+            asyncio.run(manager.run(backwards=True))
 
-        app_config = AppConfig(
-            app_name="test_app",
-            migrations_folder_path=migrations_folder_path,
-            table_classes=[],
+    @engines_only("postgres", "cockroach")
+    @patch.object(BaseMigrationManager, "get_app_config")
+    def test_add_table(self, get_app_config: MagicMock):
+        """
+        Test adding a table to a MigrationManager.
+        """
+        self.run_sync("DROP TABLE IF EXISTS musician;")
+
+        manager = MigrationManager()
+        manager.add_table(class_name="Musician", tablename="musician")
+        manager.add_column(
+            table_class_name="Musician",
+            tablename="musician",
+            column_name="name",
+            column_class_name="Varchar",
         )
+        asyncio.run(manager.run())
 
-        for table_snapshot in table_snapshots:
-            app_config.table_classes = table_snapshot
-            meta = run_sync(
-                _create_new_migration(
-                    app_config=app_config, auto=True, auto_input="y"
-                )
+        if engine_is("postgres"):
+            self.run_sync(
+                "INSERT INTO musician VALUES (default, 'Bob Jones');"
             )
-            self.assertTrue(os.path.exists(meta.migration_path))
-            self.run_migrations(app_config=app_config)
+            response = self.run_sync("SELECT * FROM musician;")
+            self.assertEqual(response, [{"id": 1, "name": "Bob Jones"}])
 
-            # It's kind of absurd sleeping for 1 microsecond, but it guarantees
-            # the migration IDs will be unique, and just in case computers
-            # and / or Python get insanely fast in the future :)
-            time.sleep(1e-6)
-
-        if test_function:
-            column_name = (
-                table_snapshots[-1][-1]
-                ._meta.non_default_columns[0]
-                ._meta.db_column_name
+        if engine_is("cockroach"):
+            id = self.run_sync(
+                "INSERT INTO musician VALUES (default, 'Bob Jones') RETURNING id;"  # noqa: E501
             )
-            row_meta = self.get_postgres_column_definition(
-                tablename="my_table",
-                column_name=column_name,
+            response = self.run_sync("SELECT * FROM musician;")
+            self.assertEqual(
+                response, [{"id": id[0]["id"], "name": "Bob Jones"}]
+            )
+
+        # Reverse
+        get_app_config.return_value = AppConfig(
+            app_name="music", migrations_folder_path=""
+        )
+        asyncio.run(manager.run(backwards=True))
+        self.assertEqual(self.table_exists("musician"), False)
+        self.run_sync("DROP TABLE IF EXISTS musician;")
+
+        # Preview
+        manager.preview = True
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            asyncio.run(manager.run())
+
+            if engine_is("postgres"):
+                self.assertEqual(
+                    fake_out.getvalue(),
+                    """  -  [preview forwards]... \n CREATE TABLE "musician" ("id" SERIAL PRIMARY KEY NOT NULL, "name" VARCHAR(255) NOT NULL DEFAULT '');\n""",  # noqa: E501
+                )
+            if engine_is("cockroach"):
+                self.assertEqual(
+                    fake_out.getvalue(),
+                    """  -  [preview forwards]... \n CREATE TABLE "musician" ("id" INTEGER PRIMARY KEY NOT NULL DEFAULT unique_rowid(), "name" VARCHAR(255) NOT NULL DEFAULT '');\n""",  # noqa: E501
+                )
+        self.assertEqual(self.table_exists("musician"), False)
+
+    @engines_only("postgres", "cockroach")
+    def test_add_column(self):
+        """
+        Test adding a column to a MigrationManager.
+        """
+        manager = MigrationManager()
+        manager.add_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="email",
+            column_class=Varchar,
+            column_class_name="Varchar",
+            params={
+                "length": 100,
+                "default": "",
+                "null": True,
+                "primary": False,
+                "key": False,
+                "unique": True,
+                "index": False,
+            },
+        )
+        asyncio.run(manager.run())
+
+        if engine_is("postgres"):
+            self.run_sync(
+                "INSERT INTO \"manager\" VALUES (default, 'Dave', 'dave@me.com');"  # noqa: E501
             )
-            self.assertTrue(
-                test_function(row_meta),
-                msg=f"Meta is incorrect: {row_meta}",
+            response = self.run_sync("SELECT * FROM manager;")
+            self.assertEqual(
+                response, [{"id": 1, "name": "Dave", "email": "dave@me.com"}]
             )
 
+            # Reverse
+            asyncio.run(manager.run(backwards=True))
+            response = self.run_sync("SELECT * FROM manager;")
+            self.assertEqual(response, [{"id": 1, "name": "Dave"}])
+
+        id = 0
+        if engine_is("cockroach"):
+            id = self.run_sync(
+                "INSERT INTO manager VALUES (default, 'Dave', 'dave@me.com') RETURNING id;"  # noqa: E501
+            )
+            response = self.run_sync("SELECT * FROM manager;")
+            self.assertEqual(
+                response,
+                [{"id": id[0]["id"], "name": "Dave", "email": "dave@me.com"}],
+            )
 
-@engines_only("postgres", "cockroach")
-class TestMigrations(MigrationTestCase):
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        create_table_class("MyTable").alter().drop_table(
-            if_exists=True
-        ).run_sync()
-        Migration.alter().drop_table(if_exists=True).run_sync()
+            # Reverse
+            asyncio.run(manager.run(backwards=True))
+            response = self.run_sync("SELECT * FROM manager;")
+            self.assertEqual(response, [{"id": id[0]["id"], "name": "Dave"}])
+
+        # Preview
+        manager.preview = True
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            asyncio.run(manager.run())
+            self.assertEqual(
+                fake_out.getvalue(),
+                """  -  [preview forwards]... \n ALTER TABLE "manager" ADD COLUMN "email" VARCHAR(100) UNIQUE DEFAULT '';\n""",  # noqa: E501
+            )
 
-    ###########################################################################
+        response = self.run_sync("SELECT * FROM manager;")
+        if engine_is("postgres"):
+            self.assertEqual(response, [{"id": 1, "name": "Dave"}])
+        if engine_is("cockroach"):
+            self.assertEqual(response, [{"id": id[0]["id"], "name": "Dave"}])
+
+    @engines_only("postgres", "cockroach")
+    def test_add_column_with_index(self):
+        """
+        Test adding a column with an index to a MigrationManager.
+        """
+        manager = MigrationManager()
+        manager.add_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="email",
+            column_class=Varchar,
+            column_class_name="Varchar",
+            params={
+                "length": 100,
+                "default": "",
+                "null": True,
+                "primary": False,
+                "key": False,
+                "unique": True,
+                "index": True,
+            },
+        )
+        index_name = Manager._get_index_name(["email"])
+
+        asyncio.run(manager.run())
+        self.assertTrue(index_name in Manager.indexes().run_sync())
+
+        # Reverse
+        asyncio.run(manager.run(backwards=True))
+        self.assertTrue(index_name not in Manager.indexes().run_sync())
+
+        # Preview
+        manager.preview = True
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            asyncio.run(manager.run())
+            self.assertEqual(
+                fake_out.getvalue(),
+                (
+                    """  -  [preview forwards]... \n ALTER TABLE "manager" ADD COLUMN "email" VARCHAR(100) UNIQUE DEFAULT '';\n"""  # noqa: E501
+                    """\n CREATE INDEX manager_email ON "manager" USING btree ("email");\n"""  # noqa: E501
+                ),
+            )
+        self.assertTrue(index_name not in Manager.indexes().run_sync())
 
-    def table(self, column: Column):
+    @engines_only("postgres")
+    def test_add_foreign_key_self_column(self):
         """
-        A utility for creating Piccolo tables with the given column.
+        Test adding a ForeignKey column to a MigrationManager, with a
+        references argument of 'self'.
         """
-        return create_table_class(
-            class_name="MyTable", class_members={"my_column": column}
-        )
-
-    @engines_skip("cockroach")
-    def test_varchar_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Varchar(),
-                    Varchar(length=100),
-                    Varchar(default="hello world"),
-                    Varchar(default=string_default),
-                    Varchar(null=True),
-                    Varchar(null=False),
-                    Varchar(index=True),
-                    Varchar(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "character varying",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in ("''::character varying", "'':::STRING"),
-                ]
-            ),
-        )
+        manager = MigrationManager()
+        manager.add_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="advisor",
+            column_class=ForeignKey,
+            column_class_name="ForeignKey",
+            params={
+                "references": "self",
+                "on_delete": OnDelete.cascade,
+                "on_update": OnUpdate.cascade,
+                "default": None,
+                "null": True,
+                "primary": False,
+                "key": False,
+                "unique": False,
+                "index": False,
+            },
+        )
+        asyncio.run(manager.run())
+
+        self.run_sync("INSERT INTO manager VALUES (default, 'Alice', null);")
+        self.run_sync("INSERT INTO manager VALUES (default, 'Dave', 1);")
+
+        response = self.run_sync("SELECT * FROM manager;")
+        self.assertEqual(
+            response,
+            [
+                {"id": 1, "name": "Alice", "advisor": None},
+                {"id": 2, "name": "Dave", "advisor": 1},
+            ],
+        )
+
+        # Reverse
+        asyncio.run(manager.run(backwards=True))
+        response = self.run_sync("SELECT * FROM manager;")
+        self.assertEqual(
+            response,
+            [{"id": 1, "name": "Alice"}, {"id": 2, "name": "Dave"}],
+        )
+
+    @engines_only("cockroach")
+    def test_add_foreign_key_self_column_alt(self):
+        """
+        Test adding a ForeignKey column to a MigrationManager, with a
+        references argument of 'self'.
+        """
+        manager = MigrationManager()
+        manager.add_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="advisor",
+            column_class=ForeignKey,
+            column_class_name="ForeignKey",
+            params={
+                "references": "self",
+                "on_delete": OnDelete.cascade,
+                "on_update": OnUpdate.cascade,
+                "default": None,
+                "null": True,
+                "primary": False,
+                "key": False,
+                "unique": False,
+                "index": False,
+            },
+        )
+        asyncio.run(manager.run())
+
+        id = self.run_sync(
+            "INSERT INTO manager VALUES (default, 'Alice', null) RETURNING id;"
+        )
+        id2 = Manager.raw(
+            "INSERT INTO manager VALUES (default, 'Dave', {}) RETURNING id;",
+            id[0]["id"],
+        ).run_sync()
 
-    def test_text_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Text(),
-                    Text(default="hello world"),
-                    Text(default=string_default),
-                    Text(null=True),
-                    Text(null=False),
-                    Text(index=True),
-                    Text(index=False),
-                ]
+        response = self.run_sync("SELECT * FROM manager;")
+        self.assertEqual(
+            response,
+            [
+                {"id": id[0]["id"], "name": "Alice", "advisor": None},
+                {"id": id2[0]["id"], "name": "Dave", "advisor": id[0]["id"]},
             ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "text",
-                    x.is_nullable == "NO",
-                    x.column_default in ("''::text", "'':::STRING"),
-                ]
-            ),
         )
 
-    def test_integer_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Integer(),
-                    Integer(default=1),
-                    Integer(default=integer_default),
-                    Integer(null=True),
-                    Integer(null=False),
-                    Integer(index=True),
-                    Integer(index=False),
-                ]
+        # Reverse
+        asyncio.run(manager.run(backwards=True))
+        response = self.run_sync("SELECT * FROM manager;")
+        self.assertEqual(
+            response,
+            [
+                {"id": id[0]["id"], "name": "Alice"},
+                {"id": id2[0]["id"], "name": "Dave"},
             ],
-            test_function=lambda x: all(
-                [
-                    x.data_type in ("integer", "bigint"),  # Cockroach DB.
-                    x.is_nullable == "NO",
-                    x.column_default in ("0", "0:::INT8"),  # Cockroach DB.
-                ]
-            ),
         )
 
-    def test_real_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Real(),
-                    Real(default=1.1),
-                    Real(null=True),
-                    Real(null=False),
-                    Real(index=True),
-                    Real(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "real",
-                    x.is_nullable == "NO",
-                    x.column_default in ("0.0", "0.0:::FLOAT8"),
-                ]
-            ),
-        )
+    @engines_only("postgres", "cockroach")
+    def test_add_non_nullable_column(self):
+        """
+        Test adding a non nullable column to a MigrationManager.
+
+        Need to handle it gracefully if rows already exist.
+        """
+        self.run_sync("INSERT INTO manager VALUES (default, 'Dave');")
+
+        manager = MigrationManager()
+        manager.add_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="email",
+            column_class=Varchar,
+            column_class_name="Varchar",
+            params={
+                "length": 100,
+                "default": "",
+                "null": False,
+                "primary": False,
+                "key": False,
+                "unique": True,
+                "index": False,
+            },
+        )
+        asyncio.run(manager.run())
+
+    @engines_only("postgres", "cockroach")
+    @patch.object(
+        BaseMigrationManager, "get_migration_managers", new_callable=AsyncMock
+    )
+    @patch.object(BaseMigrationManager, "get_app_config")
+    def test_drop_column(
+        self, get_app_config: MagicMock, get_migration_managers: MagicMock
+    ):
+        """
+        Test dropping a column with MigrationManager.
+        """
+        manager_1 = MigrationManager()
+        manager_1.add_table(class_name="Musician", tablename="musician")
+        manager_1.add_column(
+            table_class_name="Musician",
+            tablename="musician",
+            column_name="name",
+            column_class_name="Varchar",
+        )
+        asyncio.run(manager_1.run())
+
+        if engine_is("postgres"):
+            self.run_sync("INSERT INTO musician VALUES (default, 'Dave');")
+            response = self.run_sync("SELECT * FROM musician;")
+            self.assertEqual(response, [{"id": 1, "name": "Dave"}])
+
+        id = 0
+        if engine_is("cockroach"):
+            id = self.run_sync(
+                "INSERT INTO musician VALUES (default, 'Dave') RETURNING id;"
+            )
+            response = self.run_sync("SELECT * FROM musician;")
+            self.assertEqual(
+                response, [{"id": id[0]["id"], "name": "Dave"}]  # type: ignore
+            )
 
-    def test_double_precision_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    DoublePrecision(),
-                    DoublePrecision(default=1.1),
-                    DoublePrecision(null=True),
-                    DoublePrecision(null=False),
-                    DoublePrecision(index=True),
-                    DoublePrecision(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "double precision",
-                    x.is_nullable == "NO",
-                    x.column_default in ("0.0", "0.0:::FLOAT8"),
-                ]
-            ),
-        )
+        manager_2 = MigrationManager()
+        manager_2.drop_column(
+            table_class_name="Musician",
+            tablename="musician",
+            column_name="name",
+        )
+        asyncio.run(manager_2.run())
+
+        if engine_is("postgres"):
+            response = self.run_sync("SELECT * FROM musician;")
+            self.assertEqual(response, [{"id": 1}])
+
+        if engine_is("cockroach"):
+            response = self.run_sync("SELECT * FROM musician;")
+            self.assertEqual(response, [{"id": id[0]["id"]}])  # type: ignore
+
+        # Reverse
+        get_migration_managers.return_value = [manager_1]
+        app_config = AppConfig(app_name="music", migrations_folder_path="")
+        get_app_config.return_value = app_config
+        asyncio.run(manager_2.run(backwards=True))
+        response = self.run_sync("SELECT * FROM musician;")
+        if engine_is("postgres"):
+            self.assertEqual(response, [{"id": 1, "name": ""}])
+
+        if engine_is("cockroach"):
+            self.assertEqual(
+                response, [{"id": id[0]["id"], "name": ""}]  # type: ignore
+            )
 
-    def test_smallint_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    SmallInt(),
-                    SmallInt(default=1),
-                    SmallInt(default=integer_default),
-                    SmallInt(null=True),
-                    SmallInt(null=False),
-                    SmallInt(index=True),
-                    SmallInt(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "smallint",
-                    x.is_nullable == "NO",
-                    x.column_default in ("0", "0:::INT8"),  # Cockroach DB.
-                ]
-            ),
-        )
+    @engines_only("postgres", "cockroach")
+    def test_rename_table(self):
+        """
+        Test renaming a table with MigrationManager.
+        """
+        manager = MigrationManager()
 
-    def test_bigint_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    BigInt(),
-                    BigInt(default=1),
-                    BigInt(default=integer_default),
-                    BigInt(null=True),
-                    BigInt(null=False),
-                    BigInt(index=True),
-                    BigInt(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "bigint",
-                    x.is_nullable == "NO",
-                    x.column_default in ("0", "0:::INT8"),  # Cockroach DB.
-                ]
-            ),
+        manager.rename_table(
+            old_class_name="Manager",
+            old_tablename="manager",
+            new_class_name="Director",
+            new_tablename="director",
         )
 
-    def test_uuid_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    UUID(),
-                    UUID(default="ecf338cd-6da7-464c-b31e-4b2e3e12f0f0"),
-                    UUID(
-                        default=uuid.UUID(
-                            "2dfc9c47-adab-4692-b804-f692f3b0fc07"
-                        )
-                    ),
-                    UUID(default=uuid.uuid4),
-                    UUID(default=uuid_default),
-                    UUID(default=UUID4()),
-                    UUID(null=True, default=None),
-                    UUID(null=False),
-                    UUID(index=True),
-                    UUID(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "uuid",
-                    x.is_nullable == "NO",
-                    x.column_default == "uuid_generate_v4()",
-                ]
-            ),
-        )
+        asyncio.run(manager.run())
 
-    def test_timestamp_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Timestamp(),
-                    Timestamp(
-                        default=datetime.datetime(year=2021, month=1, day=1)
-                    ),
-                    Timestamp(default=datetime.datetime.now),
-                    Timestamp(default=datetime_default),
-                    Timestamp(null=True, default=None),
-                    Timestamp(null=False),
-                    Timestamp(index=True),
-                    Timestamp(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "timestamp without time zone",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in (
-                        "now()",
-                        "CURRENT_TIMESTAMP",
-                        "current_timestamp():::TIMESTAMPTZ::TIMESTAMP",
-                    ),
-                ]
-            ),
-        )
+        if engine_is("postgres"):
+            self.run_sync("INSERT INTO director VALUES (default, 'Dave');")
 
-    @engines_skip("cockroach")
-    def test_time_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Time(),
-                    Time(default=datetime.time(hour=12, minute=0)),
-                    Time(default=datetime.time),
-                    Time(default=time_default),
-                    Time(null=True, default=None),
-                    Time(null=False),
-                    Time(index=True),
-                    Time(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "time without time zone",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in ("('now'::text)::time with time zone", "CURRENT_TIME"),
-                ]
-            ),
-        )
+            response = self.run_sync("SELECT * FROM director;")
+            self.assertEqual(response, [{"id": 1, "name": "Dave"}])
 
-    def test_date_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Date(),
-                    Date(default=datetime.date(year=2021, month=1, day=1)),
-                    Date(default=datetime.date.today),
-                    Date(default=date_default),
-                    Date(null=True, default=None),
-                    Date(null=False),
-                    Date(index=True),
-                    Date(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "date",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in (
-                        "('now'::text)::date",
-                        "CURRENT_DATE",
-                        "current_date()",
-                    ),
-                ]
-            ),
-        )
+            # Reverse
+            asyncio.run(manager.run(backwards=True))
+            response = self.run_sync("SELECT * FROM manager;")
+            self.assertEqual(response, [{"id": 1, "name": "Dave"}])
 
-    def test_interval_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Interval(),
-                    Interval(default=datetime.timedelta(days=1)),
-                    Interval(default=timedelta_default),
-                    Interval(null=True, default=None),
-                    Interval(null=False),
-                    Interval(index=True),
-                    Interval(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "interval",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in ("'00:00:00'::interval", "'00:00:00':::INTERVAL"),
-                ]
-            ),
-        )
+        if engine_is("cockroach"):
+            id = 0
+            id = self.run_sync(
+                "INSERT INTO director VALUES (default, 'Dave') RETURNING id;"
+            )
 
-    def test_boolean_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Boolean(),
-                    Boolean(default=True),
-                    Boolean(default=boolean_default),
-                    Boolean(null=True, default=None),
-                    Boolean(null=False),
-                    Boolean(index=True),
-                    Boolean(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "boolean",
-                    x.is_nullable == "NO",
-                    x.column_default == "false",
-                ]
-            ),
-        )
+            response = self.run_sync("SELECT * FROM director;")
+            self.assertEqual(response, [{"id": id[0]["id"], "name": "Dave"}])
 
-    @engines_skip("cockroach")
-    def test_numeric_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Numeric(),
-                    Numeric(digits=(4, 2)),
-                    Numeric(digits=None),
-                    Numeric(default=decimal.Decimal("1.2")),
-                    Numeric(default=numeric_default),
-                    Numeric(null=True, default=None),
-                    Numeric(null=False),
-                    Numeric(index=True),
-                    Numeric(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "numeric",
-                    x.is_nullable == "NO",
-                    x.column_default == "0",
-                ]
-            ),
-        )
+            # Reverse
+            asyncio.run(manager.run(backwards=True))
+            response = self.run_sync("SELECT * FROM manager;")
+            self.assertEqual(response, [{"id": id[0]["id"], "name": "Dave"}])
 
-    @engines_skip("cockroach")
-    def test_decimal_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Decimal(),
-                    Decimal(digits=(4, 2)),
-                    Decimal(digits=None),
-                    Decimal(default=decimal.Decimal("1.2")),
-                    Decimal(default=numeric_default),
-                    Decimal(null=True, default=None),
-                    Decimal(null=False),
-                    Decimal(index=True),
-                    Decimal(index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "numeric",
-                    x.is_nullable == "NO",
-                    x.column_default == "0",
-                ]
-            ),
-        )
-
-    @engines_skip("cockroach")
-    def test_array_column_integer(self):
+    @engines_only("postgres")
+    def test_alter_column_unique(self):
         """
-        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/35730 "column my_column is of type int[] and thus is not indexable"
+        Test altering a column uniqueness with MigrationManager.
+        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/42840 "unimplemented: cannot drop UNIQUE constraint "manager_name_key" using ALTER TABLE DROP CONSTRAINT, use DROP INDEX CASCADE instead"
         """  # noqa: E501
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Array(base_column=Integer()),
-                    Array(base_column=Integer(), default=[1, 2, 3]),
-                    Array(
-                        base_column=Integer(), default=array_default_integer
-                    ),
-                    Array(base_column=Integer(), null=True, default=None),
-                    Array(base_column=Integer(), null=False),
-                    Array(base_column=Integer(), index=True),
-                    Array(base_column=Integer(), index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "ARRAY",
-                    x.is_nullable == "NO",
-                    x.column_default == "'{}'::integer[]",
-                ]
-            ),
+        manager = MigrationManager()
+
+        manager.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"unique": True},
+            old_params={"unique": False},
+        )
+
+        asyncio.run(manager.run())
+
+        with self.assertRaises(asyncpg.exceptions.UniqueViolationError):
+            self.run_sync(
+                "INSERT INTO manager VALUES "
+                "(default, 'Dave'), (default, 'Dave');"
+            )
+
+        # Reverse
+        asyncio.run(manager.run(backwards=True))
+        self.run_sync(
+            "INSERT INTO manager VALUES (default, 'Dave'), (default, 'Dave');"
         )
+        response = self.run_sync("SELECT name FROM manager;")
+        self.assertEqual(response, [{"name": "Dave"}, {"name": "Dave"}])
 
-    @engines_skip("cockroach")
-    def test_array_column_varchar(self):
+    @engines_only("postgres", "cockroach")
+    def test_alter_column_set_null(self):
         """
-        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/35730 "column my_column is of type varchar[] and thus is not indexable"
-        """  # noqa: E501
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Array(base_column=Varchar()),
-                    Array(base_column=Varchar(), default=["a", "b", "c"]),
-                    Array(
-                        base_column=Varchar(), default=array_default_varchar
-                    ),
-                    Array(base_column=Varchar(), null=True, default=None),
-                    Array(base_column=Varchar(), null=False),
-                    Array(base_column=Varchar(), index=True),
-                    Array(base_column=Varchar(), index=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "ARRAY",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in ("'{}'::character varying[]", "'':::STRING"),
-                ]
-            ),
+        Test altering whether a column is nullable with MigrationManager.
+        """
+        manager = MigrationManager()
+
+        manager.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"null": True},
+            old_params={"null": False},
         )
 
-    def test_array_column_bigint(self):
-        """
-        There was a bug with using an array of ``BigInt`` - see issue 500 on
-        GitHub. It's because ``BigInt`` requires access to the parent table to
-        determine what the column type is.
-        """
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Array(base_column=BigInt()),
-                ]
-            ]
-        )
-
-    ###########################################################################
-
-    # We deliberately don't test setting JSON or JSONB columns as indexes, as
-    # we know it'll fail.
-
-    @engines_skip("cockroach")
-    def test_json_column(self):
-        """
-        Cockroach sees all json as jsonb, so we can skip this.
-        """
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    JSON(),
-                    JSON(default=["a", "b", "c"]),
-                    JSON(default={"name": "bob"}),
-                    JSON(default='{"name": "Sally"}'),
-                    JSON(null=True, default=None),
-                    JSON(null=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "json",
-                    x.is_nullable == "NO",
-                    x.column_default == "'{}'::json",
-                ]
-            ),
+        asyncio.run(manager.run())
+        self.assertTrue(
+            self.get_postgres_is_nullable(
+                tablename="manager", column_name="name"
+            )
         )
 
-    def test_jsonb_column(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    JSONB(),
-                    JSONB(default=["a", "b", "c"]),
-                    JSONB(default={"name": "bob"}),
-                    JSONB(default='{"name": "Sally"}'),
-                    JSONB(null=True, default=None),
-                    JSONB(null=False),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "jsonb",
-                    x.is_nullable == "NO",
-                    x.column_default in ("'{}'::jsonb", "'{}':::JSONB"),
-                ]
-            ),
+        # Reverse
+        asyncio.run(manager.run(backwards=True))
+        self.assertFalse(
+            self.get_postgres_is_nullable(
+                tablename="manager", column_name="name"
+            )
         )
 
-    ###########################################################################
+    def _get_column_precision_and_scale(
+        self, tablename="ticket", column_name="price"
+    ):
+        return self.run_sync(
+            "SELECT numeric_precision, numeric_scale "
+            "FROM information_schema.COLUMNS "
+            f"WHERE table_name = '{tablename}' AND "
+            f"column_name = '{column_name}';"
+        )
 
-    def test_db_column_name(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Varchar(),
-                    Varchar(db_column_name="custom_name"),
-                    Varchar(),
-                    Varchar(db_column_name="custom_name_2"),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "character varying",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in ("''::character varying", "'':::STRING"),
-                ]
-            ),
+    def _get_column_default(self, tablename="manager", column_name="name"):
+        return self.run_sync(
+            "SELECT column_default "
+            "FROM information_schema.COLUMNS "
+            f"WHERE table_name = '{tablename}' "
+            f"AND column_name = '{column_name}';"
         )
 
-    def test_db_column_name_initial(self):
-        """
-        Make sure that if a new table is created which contains a column with
-        ``db_column_name`` specified, then the column has the correct name.
+    @engines_only("postgres")
+    def test_alter_column_digits(self):
         """
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Varchar(db_column_name="custom_name"),
-                ]
-            ],
-            test_function=lambda x: all(
-                [
-                    x.data_type == "character varying",
-                    x.is_nullable == "NO",
-                    x.column_default
-                    in ("''::character varying", "'':::STRING"),
-                ]
-            ),
+        Test altering a column digits with MigrationManager.
+        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/49351 "ALTER COLUMN TYPE is not supported inside a transaction"
+        """  # noqa: E501
+        manager = MigrationManager()
+
+        manager.alter_column(
+            table_class_name="Ticket",
+            tablename="ticket",
+            column_name="price",
+            params={"digits": (6, 2)},
+            old_params={"digits": (5, 2)},
         )
 
-    ###########################################################################
+        asyncio.run(manager.run())
+        self.assertEqual(
+            self._get_column_precision_and_scale(),
+            [{"numeric_precision": 6, "numeric_scale": 2}],
+        )
 
-    # Column type conversion
+        asyncio.run(manager.run(backwards=True))
+        self.assertEqual(
+            self._get_column_precision_and_scale(),
+            [{"numeric_precision": 5, "numeric_scale": 2}],
+        )
 
-    def test_column_type_conversion_string(self):
+    @engines_only("postgres")
+    def test_alter_column_set_default(self):
         """
-        We can't manage all column type conversions, but should be able to
-        manage most simple ones (e.g. Varchar to Text).
+        Test altering a column default with MigrationManager.
         """
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Varchar(),
-                    Text(),
-                    Varchar(),
-                ]
-            ]
+        manager = MigrationManager()
+
+        manager.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"default": "Unknown"},
+            old_params={"default": ""},
         )
 
-    @engines_skip("cockroach")
-    def test_column_type_conversion_integer(self):
-        """
-        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/49351 "ALTER COLUMN TYPE is not supported inside a transaction"
-        """  # noqa: E501
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Integer(),
-                    BigInt(),
-                    SmallInt(),
-                    BigInt(),
-                    Integer(),
-                ]
-            ]
+        asyncio.run(manager.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Unknown'::character varying"}],
         )
 
-    @engines_skip("cockroach")
-    def test_column_type_conversion_string_to_integer(self):
-        """
-        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/49351 "ALTER COLUMN TYPE is not supported inside a transaction"
-        """  # noqa: E501
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Varchar(default="1"),
-                    Integer(default=1),
-                    Varchar(default="1"),
-                ]
-            ]
+        asyncio.run(manager.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "''::character varying"}],
         )
 
-    @engines_skip("cockroach")
-    def test_column_type_conversion_float_decimal(self):
+    @engines_only("cockroach")
+    def test_alter_column_set_default_alt(self):
         """
-        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/49351 "ALTER COLUMN TYPE is not supported inside a transaction"
-        """  # noqa: E501
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Real(default=1.0),
-                    DoublePrecision(default=1.0),
-                    Real(default=1.0),
-                    Numeric(),
-                    Real(default=1.0),
-                ]
-            ]
+        Test altering a column default with MigrationManager.
+        """
+        manager = MigrationManager()
+
+        manager.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"default": "Unknown"},
+            old_params={"default": ""},
         )
 
-    def test_column_type_conversion_json(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    JSON(),
-                    JSONB(),
-                    JSON(),
-                ]
-            ]
+        asyncio.run(manager.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Unknown':::STRING"}],
         )
 
-    def test_column_type_conversion_timestamp(self):
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Timestamp(),
-                    Timestamptz(),
-                    Timestamp(),
-                ]
-            ]
+        asyncio.run(manager.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'':::STRING"}],
         )
 
-    @patch("piccolo.apps.migrations.auto.migration_manager.colored_warning")
-    def test_column_type_conversion_serial(self, colored_warning: MagicMock):
+    @engines_only("postgres")
+    def test_alter_column_drop_default(self):
         """
-        This isn't possible, as neither SERIAL or BIGSERIAL are actual types.
-        They're just shortcuts. Make sure the migration doesn't crash - it
-        should just output a warning.
+        Test setting a column default to None with MigrationManager.
         """
-        self._test_migrations(
-            table_snapshots=[
-                [self.table(column)]
-                for column in [
-                    Serial(),
-                    BigSerial(),
-                ]
-            ]
+        # Make sure it has a non-null default to start with.
+        manager_1 = MigrationManager()
+        manager_1.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"default": "Mr Manager"},
+            old_params={"default": None},
         )
-
-        colored_warning.assert_called_once_with(
-            "Unable to migrate Serial to BigSerial and vice versa. This must "
-            "be done manually."
+        asyncio.run(manager_1.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Mr Manager'::character varying"}],
         )
 
+        # Drop the default.
+        manager_2 = MigrationManager()
+        manager_2.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"default": None},
+            old_params={"default": "Mr Manager"},
+        )
+        asyncio.run(manager_2.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": None}],
+        )
 
-###############################################################################
+        # And add it back once more to be sure.
+        manager_3 = manager_1
+        asyncio.run(manager_3.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Mr Manager'::character varying"}],
+        )
 
+        # Run them all backwards
+        asyncio.run(manager_3.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": None}],
+        )
 
-class Band(Table):
-    name = Varchar()
-    genres = M2M(LazyTableReference("GenreToBand", module_path=__name__))
+        asyncio.run(manager_2.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Mr Manager'::character varying"}],
+        )
 
+        asyncio.run(manager_1.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": None}],
+        )
 
-class Genre(Table):
-    name = Varchar()
-    bands = M2M(LazyTableReference("GenreToBand", module_path=__name__))
+    @engines_only("cockroach")
+    def test_alter_column_drop_default_alt(self):
+        """
+        Test setting a column default to None with MigrationManager.
+        """
+        # Make sure it has a non-null default to start with.
+        manager_1 = MigrationManager()
+        manager_1.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"default": "Mr Manager"},
+            old_params={"default": None},
+        )
+        asyncio.run(manager_1.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Mr Manager':::STRING"}],
+        )
 
+        # Drop the default.
+        manager_2 = MigrationManager()
+        manager_2.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"default": None},
+            old_params={"default": "Mr Manager"},
+        )
+        asyncio.run(manager_2.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": None}],
+        )
 
-class GenreToBand(Table):
-    band = ForeignKey(Band)
-    genre = ForeignKey(Genre)
+        # And add it back once more to be sure.
+        manager_3 = manager_1
+        asyncio.run(manager_3.run())
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Mr Manager':::STRING"}],
+        )
 
+        # Run them all backwards
+        asyncio.run(manager_3.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": None}],
+        )
 
-@engines_only("postgres", "cockroach")
-class TestM2MMigrations(MigrationTestCase):
-    def setUp(self):
-        pass
+        asyncio.run(manager_2.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": "'Mr Manager':::STRING"}],
+        )
 
-    def tearDown(self):
-        drop_db_tables_sync(Migration, Band, Genre, GenreToBand)
+        asyncio.run(manager_1.run(backwards=True))
+        self.assertEqual(
+            self._get_column_default(),
+            [{"column_default": None}],
+        )
 
-    def test_m2m(self):
+    @engines_only("postgres", "cockroach")
+    def test_alter_column_add_index(self):
         """
-        Make sure M2M relations can be created.
+        Test altering a column to add an index with MigrationManager.
         """
+        manager = MigrationManager()
 
-        self._test_migrations(
-            table_snapshots=[[Band, Genre, GenreToBand]],
+        manager.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"index": True},
+            old_params={"index": False},
         )
 
-        for table_class in [Band, Genre, GenreToBand]:
-            self.assertTrue(table_class.table_exists().run_sync())
-
-
-###############################################################################
-
-
-@engines_only("postgres", "cockroach")
-class TestForeignKeys(MigrationTestCase):
-    def setUp(self):
-        class TableA(Table):
-            pass
-
-        class TableB(Table):
-            fk = ForeignKey(TableA)
+        asyncio.run(manager.run())
+        self.assertTrue(
+            Manager._get_index_name(["name"]) in Manager.indexes().run_sync()
+        )
 
-        class TableC(Table):
-            fk = ForeignKey(TableB)
+        asyncio.run(manager.run(backwards=True))
+        self.assertTrue(
+            Manager._get_index_name(["name"])
+            not in Manager.indexes().run_sync()
+        )
 
-        class TableD(Table):
-            fk = ForeignKey(TableC)
+    @engines_only("postgres", "cockroach")
+    def test_alter_column_set_type(self):
+        """
+        Test altering a column to change it's type with MigrationManager.
+        """
+        manager = MigrationManager()
 
-        class TableE(Table):
-            fk = ForeignKey(TableD)
+        manager.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={},
+            old_params={},
+            column_class=Text,
+            old_column_class=Varchar,
+        )
 
-        self.table_classes = [TableA, TableB, TableC, TableD, TableE]
+        asyncio.run(manager.run())
+        column_type_str = self.get_postgres_column_type(
+            tablename="manager", column_name="name"
+        )
+        self.assertEqual(column_type_str, "TEXT")
 
-    def tearDown(self):
-        drop_db_tables_sync(Migration, *self.table_classes)
+        asyncio.run(manager.run(backwards=True))
+        column_type_str = self.get_postgres_column_type(
+            tablename="manager", column_name="name"
+        )
+        self.assertEqual(column_type_str, "CHARACTER VARYING")
 
-    def test_foreign_keys(self):
+    @engines_only("postgres")
+    def test_alter_column_set_length(self):
         """
-        Make sure that if we try creating tables with lots of foreign keys
-        to each other it runs successfully.
-
-        https://github.com/piccolo-orm/piccolo/issues/616
+        Test altering a Varchar column's length with MigrationManager.
+        🐛 Cockroach bug: https://github.com/cockroachdb/cockroach/issues/49351 "ALTER COLUMN TYPE is not supported inside a transaction"
+        """  # noqa: E501
+        manager = MigrationManager()
 
-        """
-        # We'll shuffle them, to make it a more thorough test.
-        table_classes = random.sample(
-            self.table_classes, len(self.table_classes)
+        manager.alter_column(
+            table_class_name="Manager",
+            tablename="manager",
+            column_name="name",
+            params={"length": 500},
+            old_params={"length": 200},
+            column_class=Text,
+            old_column_class=Varchar,
         )
 
-        self._test_migrations(table_snapshots=[table_classes])
-        for table_class in table_classes:
-            self.assertTrue(table_class.table_exists().run_sync())
-
-
-@engines_only("postgres", "cockroach")
-class TestTargetColumn(MigrationTestCase):
-    def setUp(self):
-        class TableA(Table):
-            name = Varchar(unique=True)
+        asyncio.run(manager.run())
+        self.assertEqual(
+            self.get_postgres_varchar_length(
+                tablename="manager", column_name="name"
+            ),
+            500,
+        )
 
-        class TableB(Table):
-            table_a = ForeignKey(TableA, target_column=TableA.name)
+        asyncio.run(manager.run(backwards=True))
+        self.assertEqual(
+            self.get_postgres_varchar_length(
+                tablename="manager", column_name="name"
+            ),
+            200,
+        )
 
-        self.table_classes = [TableA, TableB]
+    @engines_only("postgres", "cockroach")
+    @patch.object(
+        BaseMigrationManager, "get_migration_managers", new_callable=AsyncMock
+    )
+    @patch.object(BaseMigrationManager, "get_app_config")
+    def test_drop_table(
+        self, get_app_config: MagicMock, get_migration_managers: MagicMock
+    ):
+        self.run_sync("DROP TABLE IF EXISTS musician;")
 
-    def tearDown(self):
-        drop_db_tables_sync(Migration, *self.table_classes)
+        name_column = Varchar()
+        name_column._meta.name = "name"
 
-    def test_target_column(self):
-        """
-        Make sure migrations still work when a foreign key references a column
-        other than the primary key.
-        """
-        self._test_migrations(
-            table_snapshots=[self.table_classes],
+        manager_1 = MigrationManager(migration_id="1", app_name="music")
+        manager_1.add_table(
+            class_name="Musician", tablename="musician", columns=[name_column]
         )
+        asyncio.run(manager_1.run())
 
-        for table_class in self.table_classes:
-            self.assertTrue(table_class.table_exists().run_sync())
-
-        # Make sure the constraint was created correctly.
-        response = self.run_sync(
-            """
-            SELECT EXISTS(
-                SELECT 1
-                FROM INFORMATION_SCHEMA.CONSTRAINT_COLUMN_USAGE CCU
-                JOIN INFORMATION_SCHEMA.TABLE_CONSTRAINTS TC ON
-                    CCU.CONSTRAINT_NAME = TC.CONSTRAINT_NAME
-                WHERE CONSTRAINT_TYPE = 'FOREIGN KEY'
-                    AND TC.TABLE_NAME = 'table_b'
-                    AND CCU.TABLE_NAME = 'table_a'
-                    AND CCU.COLUMN_NAME = 'name'
-            )
-            """
-        )
-        self.assertTrue(response[0]["exists"])
+        manager_2 = MigrationManager(migration_id="2", app_name="music")
+        manager_2.drop_table(class_name="Musician", tablename="musician")
+        asyncio.run(manager_2.run())
 
+        self.assertTrue(not self.table_exists("musician"))
 
-@engines_only("postgres", "cockroach")
-class TestTargetColumnString(MigrationTestCase):
-    def setUp(self):
-        class TableA(Table):
-            name = Varchar(unique=True)
+        # Reverse
+        get_migration_managers.return_value = [manager_1]
+        app_config = AppConfig(app_name="music", migrations_folder_path="")
+        get_app_config.return_value = app_config
+        asyncio.run(manager_2.run(backwards=True))
 
-        class TableB(Table):
-            table_a = ForeignKey(TableA, target_column="name")
+        get_migration_managers.assert_called_with(
+            app_config=app_config, max_migration_id="2", offset=-1
+        )
+        self.assertTrue(self.table_exists("musician"))
 
-        self.table_classes = [TableA, TableB]
+        self.run_sync("DROP TABLE IF EXISTS musician;")
 
-    def tearDown(self):
-        drop_db_tables_sync(Migration, *self.table_classes)
+    @engines_only("postgres", "cockroach")
+    def test_change_table_schema(self):
+        manager = MigrationManager(migration_id="1", app_name="music")
 
-    def test_target_column(self):
-        """
-        Make sure migrations still work when a foreign key references a column
-        other than the primary key.
-        """
-        self._test_migrations(
-            table_snapshots=[self.table_classes],
+        manager.change_table_schema(
+            class_name="Manager",
+            tablename="manager",
+            new_schema="schema_1",
+            old_schema=None,
         )
 
-        for table_class in self.table_classes:
-            self.assertTrue(table_class.table_exists().run_sync())
+        # Preview
+        manager.preview = True
+        with patch("sys.stdout", new=StringIO()) as fake_out:
+            asyncio.run(manager.run())
+
+            output = fake_out.getvalue()
 
-        # Make sure the constraint was created correctly.
-        response = self.run_sync(
-            """
-            SELECT EXISTS(
-                SELECT 1
-                FROM INFORMATION_SCHEMA.CONSTRAINT_COLUMN_USAGE CCU
-                JOIN INFORMATION_SCHEMA.TABLE_CONSTRAINTS TC ON
-                    CCU.CONSTRAINT_NAME = TC.CONSTRAINT_NAME
-                WHERE CONSTRAINT_TYPE = 'FOREIGN KEY'
-                    AND TC.TABLE_NAME = 'table_b'
-                    AND CCU.TABLE_NAME = 'table_a'
-                    AND CCU.COLUMN_NAME = 'name'
+            self.assertEqual(
+                output,
+                '  - 1 [preview forwards]... CREATE SCHEMA IF NOT EXISTS "schema_1"\nALTER TABLE "manager" SET SCHEMA "schema_1"\n',  # noqa: E501
             )
-            """
-        )
-        self.assertTrue(response[0]["exists"])
```

### Comparing `piccolo-0.99.0/tests/apps/migrations/auto/test_diffable_table.py` & `piccolo-1.0a1/tests/apps/migrations/auto/test_diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/migrations/auto/test_schema_differ.py` & `piccolo-1.0a1/tests/apps/migrations/auto/test_schema_differ.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from __future__ import annotations
 
 import typing as t
 from unittest import TestCase
 from unittest.mock import MagicMock, call, patch
 
-from piccolo.apps.migrations.auto import DiffableTable, SchemaDiffer
+from piccolo.apps.migrations.auto.schema_differ import (
+    DiffableTable,
+    RenameColumn,
+    RenameColumnCollection,
+    RenameTable,
+    RenameTableCollection,
+    SchemaDiffer,
+)
 from piccolo.columns.column_types import Numeric, Varchar
 
 
 class TestSchemaDiffer(TestCase):
 
     maxDiff = None
 
@@ -28,15 +35,15 @@
             schema=schema, schema_snapshot=schema_snapshot, auto_input="y"
         )
 
         create_tables = schema_differ.create_tables
         self.assertTrue(len(create_tables.statements) == 1)
         self.assertEqual(
             create_tables.statements[0],
-            "manager.add_table('Band', tablename='band')",
+            "manager.add_table(class_name='Band', tablename='band', schema=None, columns=None)",  # noqa: E501
         )
 
         new_table_columns = schema_differ.new_table_columns
         self.assertTrue(len(new_table_columns.statements) == 1)
         self.assertEqual(
             new_table_columns.statements[0],
             "manager.add_column(table_class_name='Band', tablename='band', column_name='name', db_column_name='name', column_class_name='Varchar', column_class=Varchar, params={'length': 255, 'default': '', 'null': False, 'primary_key': False, 'unique': False, 'index': False, 'index_method': IndexMethod.btree, 'choices': None, 'db_column_name': None, 'secret': False})",  # noqa
@@ -53,15 +60,15 @@
         schema_differ = SchemaDiffer(
             schema=schema, schema_snapshot=schema_snapshot, auto_input="y"
         )
 
         self.assertTrue(len(schema_differ.drop_tables.statements) == 1)
         self.assertEqual(
             schema_differ.drop_tables.statements[0],
-            "manager.drop_table(class_name='Band', tablename='band')",
+            "manager.drop_table(class_name='Band', tablename='band', schema=None)",  # noqa: E501
         )
 
     def test_rename_table(self):
         """
         Test renaming a table.
         """
         name_column = Varchar()
@@ -81,20 +88,55 @@
         schema_differ = SchemaDiffer(
             schema=schema, schema_snapshot=schema_snapshot, auto_input="y"
         )
 
         self.assertTrue(len(schema_differ.rename_tables.statements) == 1)
         self.assertEqual(
             schema_differ.rename_tables.statements[0],
-            "manager.rename_table(old_class_name='Band', old_tablename='band', new_class_name='Act', new_tablename='act')",  # noqa
+            "manager.rename_table(old_class_name='Band', old_tablename='band', new_class_name='Act', new_tablename='act')",  # noqa: E501
         )
 
         self.assertEqual(schema_differ.create_tables.statements, [])
         self.assertEqual(schema_differ.drop_tables.statements, [])
 
+    def test_change_schema(self):
+        """
+        Testing changing the schema.
+        """
+        schema: t.List[DiffableTable] = [
+            DiffableTable(
+                class_name="Band",
+                tablename="band",
+                columns=[],
+                schema="schema_1",
+            )
+        ]
+        schema_snapshot: t.List[DiffableTable] = [
+            DiffableTable(
+                class_name="Band",
+                tablename="band",
+                columns=[],
+                schema=None,
+            )
+        ]
+
+        schema_differ = SchemaDiffer(
+            schema=schema, schema_snapshot=schema_snapshot, auto_input="y"
+        )
+
+        self.assertEqual(len(schema_differ.change_table_schemas.statements), 1)
+
+        self.assertEqual(
+            schema_differ.change_table_schemas.statements[0],
+            "manager.change_table_schema(class_name='Band', tablename='band', new_schema='schema_1', old_schema=None)",  # noqa: E501
+        )
+
+        self.assertListEqual(schema_differ.create_tables.statements, [])
+        self.assertListEqual(schema_differ.drop_tables.statements, [])
+
     def test_add_column(self):
         """
         Test adding a column to an existing table.
         """
         name_column = Varchar()
         name_column._meta.name = "name"
 
@@ -119,15 +161,15 @@
         schema_differ = SchemaDiffer(
             schema=schema, schema_snapshot=schema_snapshot, auto_input="y"
         )
 
         self.assertTrue(len(schema_differ.add_columns.statements) == 1)
         self.assertEqual(
             schema_differ.add_columns.statements[0],
-            "manager.add_column(table_class_name='Band', tablename='band', column_name='genre', db_column_name='genre', column_class_name='Varchar', column_class=Varchar, params={'length': 255, 'default': '', 'null': False, 'primary_key': False, 'unique': False, 'index': False, 'index_method': IndexMethod.btree, 'choices': None, 'db_column_name': None, 'secret': False})",  # noqa
+            "manager.add_column(table_class_name='Band', tablename='band', column_name='genre', db_column_name='genre', column_class_name='Varchar', column_class=Varchar, params={'length': 255, 'default': '', 'null': False, 'primary_key': False, 'unique': False, 'index': False, 'index_method': IndexMethod.btree, 'choices': None, 'db_column_name': None, 'secret': False})",  # noqa: E501
         )
 
     def test_drop_column(self):
         """
         Test dropping a column from an existing table.
         """
         name_column = Varchar()
@@ -154,15 +196,15 @@
         schema_differ = SchemaDiffer(
             schema=schema, schema_snapshot=schema_snapshot, auto_input="y"
         )
 
         self.assertTrue(len(schema_differ.drop_columns.statements) == 1)
         self.assertEqual(
             schema_differ.drop_columns.statements[0],
-            "manager.drop_column(table_class_name='Band', tablename='band', column_name='genre', db_column_name='genre')",  # noqa
+            "manager.drop_column(table_class_name='Band', tablename='band', column_name='genre', db_column_name='genre')",  # noqa: E501
         )
 
     def test_rename_column(self):
         """
         Test renaming a column in an existing table.
         """
         # We're going to rename the 'name' column to 'title'
@@ -192,15 +234,15 @@
             schema=schema, schema_snapshot=schema_snapshot, auto_input="y"
         )
         self.assertEqual(schema_differ.add_columns.statements, [])
         self.assertEqual(schema_differ.drop_columns.statements, [])
         self.assertEqual(
             schema_differ.rename_columns.statements,
             [
-                "manager.rename_column(table_class_name='Band', tablename='band', old_column_name='title', new_column_name='name', old_db_column_name='title', new_db_column_name='name')"  # noqa
+                "manager.rename_column(table_class_name='Band', tablename='band', old_column_name='title', new_column_name='name', old_db_column_name='title', new_db_column_name='name')"  # noqa: E501
             ],
         )
 
         # Test 2 - Tell Piccolo the column wasn't renamed
         schema_differ = SchemaDiffer(
             schema=schema, schema_snapshot=schema_snapshot, auto_input="n"
         )
@@ -445,7 +487,58 @@
         self.assertEqual(
             schema_differ.alter_columns.statements[0],
             "manager.alter_column(table_class_name='Ticket', tablename='ticket', column_name='price', db_column_name='custom', params={'digits': (4, 2)}, old_params={'digits': (5, 2)}, column_class=Numeric, old_column_class=Numeric)",  # noqa
         )
 
     def test_alter_default(self):
         pass
+
+
+class TestRenameTableCollection(TestCase):
+    collection = RenameTableCollection(
+        rename_tables=[
+            RenameTable(
+                old_class_name="Manager",
+                old_tablename="manager",
+                new_class_name="Manager1",
+                new_tablename="manager_1",
+            )
+        ]
+    )
+
+    def test_was_renamed_from(self):
+        self.assertTrue(
+            self.collection.was_renamed_from(old_class_name="Manager")
+        )
+        self.assertFalse(
+            self.collection.was_renamed_from(old_class_name="Band")
+        )
+
+    def test_renamed_from(self):
+        self.assertEqual(
+            self.collection.renamed_from(new_class_name="Manager1"), "Manager"
+        )
+        self.assertIsNone(
+            self.collection.renamed_from(new_class_name="Band"),
+        )
+
+
+class TestRenameColumnCollection(TestCase):
+    def test_for_table_class_name(self):
+        rename_column = RenameColumn(
+            table_class_name="Manager",
+            tablename="manager",
+            old_column_name="name",
+            new_column_name="full_name",
+            old_db_column_name="name",
+            new_db_column_name="full_name",
+        )
+
+        collection = RenameColumnCollection(rename_columns=[rename_column])
+
+        self.assertListEqual(
+            collection.for_table_class_name(table_class_name="Manager"),
+            [rename_column],
+        )
+        self.assertListEqual(
+            collection.for_table_class_name(table_class_name="Band"), []
+        )
```

### Comparing `piccolo-0.99.0/tests/apps/migrations/auto/test_schema_snapshot.py` & `piccolo-1.0a1/tests/apps/migrations/auto/test_schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/migrations/auto/test_serialisation.py` & `piccolo-1.0a1/tests/apps/migrations/auto/test_serialisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     serialise_params,
 )
 from piccolo.columns.base import OnDelete
 from piccolo.columns.choices import Choice
 from piccolo.columns.column_types import Varchar
 from piccolo.columns.defaults import UUID4, DateNow, TimeNow, TimestampNow
 from piccolo.columns.reference import LazyTableReference
-from tests.base import engine_is
 
 
 class TestUniqueGlobalNamesMeta:
     def test_duplicate_class_attribute_values_raises_error(self):
         with pytest.raises(ValueError):
 
             class IncorrectUniqueGlobalNames(metaclass=UniqueGlobalNamesMeta):
@@ -239,35 +238,23 @@
             self.assertEqual(
                 serialised.extra_imports[0].__str__(),
                 "from piccolo.table import Table",
             )
 
             self.assertTrue(len(serialised.extra_definitions) == 1)
 
-            if engine_is("postgres"):
-                self.assertEqual(
-                    serialised.extra_definitions[0].__str__(),
-                    (
-                        'class Manager(Table, tablename="manager"): '
-                        "id = Serial(null=False, primary_key=True, unique=False, "  # noqa: E501
-                        "index=False, index_method=IndexMethod.btree, "
-                        "choices=None, db_column_name='id', secret=False)"
-                    ),
-                )
-
-            if engine_is("cockroach"):
-                self.assertEqual(
-                    serialised.extra_definitions[0].__str__(),
-                    (
-                        'class Manager(Table, tablename="manager"): '
-                        "id = Serial(null=False, primary_key=True, unique=False, "  # noqa: E501
-                        "index=False, index_method=IndexMethod.btree, "
-                        "choices=None, db_column_name='id', secret=False)"
-                    ),
-                )
+            self.assertEqual(
+                serialised.extra_definitions[0].__str__(),
+                (
+                    'class Manager(Table, tablename="manager", schema=None): '
+                    "id = Serial(null=False, primary_key=True, unique=False, "
+                    "index=False, index_method=IndexMethod.btree, "
+                    "choices=None, db_column_name='id', secret=False)"
+                ),
+            )
 
     def test_function(self):
         serialised = serialise_params(params={"default": example_function})
         self.assertTrue(
             serialised.params["default"].__repr__() == "example_function"
         )
```

### Comparing `piccolo-0.99.0/tests/apps/migrations/commands/test_base.py` & `piccolo-1.0a1/tests/apps/migrations/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/migrations/commands/test_check.py` & `piccolo-1.0a1/tests/apps/migrations/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/migrations/commands/test_clean.py` & `piccolo-1.0a1/tests/apps/migrations/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/migrations/commands/test_forwards_backwards.py` & `piccolo-1.0a1/tests/apps/migrations/commands/test_forwards_backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py` & `piccolo-1.0a1/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/shell/commands/test_run.py` & `piccolo-1.0a1/tests/apps/shell/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/user/commands/test_change_password.py` & `piccolo-1.0a1/tests/apps/user/commands/test_change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/user/commands/test_change_permissions.py` & `piccolo-1.0a1/tests/apps/user/commands/test_change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/user/commands/test_create.py` & `piccolo-1.0a1/tests/apps/user/commands/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/apps/user/test_tables.py` & `piccolo-1.0a1/tests/apps/user/test_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_array.py` & `piccolo-1.0a1/tests/columns/test_array.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_base.py` & `piccolo-1.0a1/tests/columns/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_bigint.py` & `piccolo-1.0a1/tests/columns/test_bigint.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_boolean.py` & `piccolo-1.0a1/tests/columns/test_boolean.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_bytea.py` & `piccolo-1.0a1/tests/columns/test_bytea.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_date.py` & `piccolo-1.0a1/tests/columns/test_date.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_db_column_name.py` & `piccolo-1.0a1/tests/columns/test_db_column_name.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_defaults.py` & `piccolo-1.0a1/tests/columns/test_defaults.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_double_precision.py` & `piccolo-1.0a1/tests/columns/test_double_precision.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_interval.py` & `piccolo-1.0a1/tests/columns/test_interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_json.py` & `piccolo-1.0a1/tests/columns/test_json.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_jsonb.py` & `piccolo-1.0a1/tests/columns/test_jsonb.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_numeric.py` & `piccolo-1.0a1/tests/columns/test_numeric.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_primary_key.py` & `piccolo-1.0a1/tests/columns/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_readable.py` & `piccolo-1.0a1/tests/columns/test_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_real.py` & `piccolo-1.0a1/tests/columns/test_real.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_reference.py` & `piccolo-1.0a1/tests/columns/test_reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_reserved_column_names.py` & `piccolo-1.0a1/tests/columns/test_reserved_column_names.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_smallint.py` & `piccolo-1.0a1/tests/columns/test_smallint.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_time.py` & `piccolo-1.0a1/tests/columns/test_time.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_timestamp.py` & `piccolo-1.0a1/tests/columns/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_timestamptz.py` & `piccolo-1.0a1/tests/columns/test_timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/columns/test_varchar.py` & `piccolo-1.0a1/tests/columns/test_varchar.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/conf/test_apps.py` & `piccolo-1.0a1/tests/conf/test_apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pathlib
 from unittest import TestCase
 
 from piccolo.apps.user.tables import BaseUser
 from piccolo.conf.apps import AppConfig, AppRegistry, Finder, table_finder
 from tests.example_apps.mega.tables import MegaTable, SmallTable
 from tests.example_apps.music.tables import (
@@ -217,50 +219,88 @@
 class TestFinder(TestCase):
     def test_get_table_classes(self):
         """
         Make sure ``Table`` classes can be retrieved.
         """
         finder = Finder()
 
-        self.assertEqual(
-            finder.get_table_classes(),
+        self.assertListEqual(
+            sorted(finder.get_table_classes(), key=lambda i: i.__name__),
             [
-                Manager,
                 Band,
-                Venue,
                 Concert,
-                Ticket,
+                Manager,
+                MegaTable,
                 Poster,
-                Shirt,
                 RecordingStudio,
-                MegaTable,
+                Shirt,
                 SmallTable,
+                Ticket,
+                Venue,
             ],
         )
 
-        self.assertEqual(
-            finder.get_table_classes(include_apps=["music"]),
+        self.assertListEqual(
+            sorted(
+                finder.get_table_classes(include_apps=["music"]),
+                key=lambda i: i.__name__,
+            ),
             [
-                Manager,
                 Band,
-                Venue,
                 Concert,
-                Ticket,
+                Manager,
                 Poster,
-                Shirt,
                 RecordingStudio,
+                Shirt,
+                Ticket,
+                Venue,
             ],
         )
 
-        self.assertEqual(
-            finder.get_table_classes(exclude_apps=["music"]),
+        self.assertListEqual(
+            sorted(
+                finder.get_table_classes(exclude_apps=["music"]),
+                key=lambda i: i.__name__,
+            ),
             [
                 MegaTable,
                 SmallTable,
             ],
         )
 
         with self.assertRaises(ValueError):
             # You shouldn't be allowed to specify both include and exclude.
             finder.get_table_classes(
                 exclude_apps=["music"], include_apps=["mega"]
             )
+
+    def test_sort_app_configs(self):
+        """
+        Make sure we can sort ``AppConfig`` based on their migration
+        dependencies.
+        """
+        app_config_1 = AppConfig(
+            app_name="app_1",
+            migrations_folder_path="",
+        )
+
+        app_config_1._migration_dependency_app_configs = [
+            AppConfig(
+                app_name="app_2",
+                migrations_folder_path="",
+            )
+        ]
+
+        app_config_2 = AppConfig(
+            app_name="app_2",
+            migrations_folder_path="",
+        )
+
+        app_config_2._migration_dependency_app_configs = []
+
+        sorted_app_configs = Finder().sort_app_configs(
+            [app_config_2, app_config_1]
+        )
+
+        self.assertListEqual(
+            [i.app_name for i in sorted_app_configs], ["app_2", "app_1"]
+        )
```

### Comparing `piccolo-0.99.0/tests/engine/test_extra_nodes.py` & `piccolo-1.0a1/tests/engine/test_extra_nodes.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/engine/test_nested_transaction.py` & `piccolo-1.0a1/tests/engine/test_nested_transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,16 +56,29 @@
 
 
 class TestSameDB(DBTestCase):
     async def run_nested(self):
         """
         Nested transactions currently aren't permitted in a connection.
         """
+        # allow_nested=False
         with self.assertRaises(TransactionError):
             async with Manager._meta.db.transaction():
                 await Manager(name="Bob").save().run()
 
-                async with Manager._meta.db.transaction():
-                    await Manager(name="Dave").save().run()
+                async with Manager._meta.db.transaction(allow_nested=False):
+                    pass
+
+        # allow_nested=True
+        async with Manager._meta.db.transaction():
+            async with Manager._meta.db.transaction():
+                # Shouldn't raise an exception
+                pass
+
+        # Utilise returned transaction.
+        async with Manager._meta.db.transaction():
+            async with Manager._meta.db.transaction() as transaction:
+                await Manager(name="Dave").save().run()
+                await transaction.rollback()
 
     def test_nested(self):
         asyncio.run(self.run_nested())
```

### Comparing `piccolo-0.99.0/tests/engine/test_pool.py` & `piccolo-1.0a1/tests/engine/test_pool.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/engine/test_transaction.py` & `piccolo-1.0a1/tests/engine/test_transaction.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,14 +105,42 @@
                 await Band.create_table().run()
 
         asyncio.run(run_transaction())
 
         self.assertTrue(Band.table_exists().run_sync())
         self.assertTrue(Manager.table_exists().run_sync())
 
+    def test_manual_commit(self):
+        """
+        The context manager automatically commits changes, but we also
+        allow the user to do it manually.
+        """
+
+        async def run_transaction():
+            async with Band._meta.db.transaction() as transaction:
+                await Manager.create_table()
+                await transaction.commit()
+
+        asyncio.run(run_transaction())
+        self.assertTrue(Manager.table_exists().run_sync())
+
+    def test_manual_rollback(self):
+        """
+        The context manager will automatically rollback changes if an exception
+        is raised, but we also allow the user to do it manually.
+        """
+
+        async def run_transaction():
+            async with Band._meta.db.transaction() as transaction:
+                await Manager.create_table()
+                await transaction.rollback()
+
+        asyncio.run(run_transaction())
+        self.assertFalse(Manager.table_exists().run_sync())
+
     @engines_only("postgres")
     def test_transaction_id(self):
         """
         An extra sanity check, that the transaction id is the same for each
         query inside the transaction block.
         """
 
@@ -228,7 +256,43 @@
         self.assertListEqual(
             Manager.select(Manager.name)
             .order_by(Manager.name)
             .output(as_list=True)
             .run_sync(),
             manager_names,
         )
+
+
+class TestSavepoint(TestCase):
+    def setUp(self):
+        Manager.create_table().run_sync()
+
+    def tearDown(self):
+        Manager.alter().drop_table().run_sync()
+
+    def test_savepoint(self):
+        async def run_test():
+            async with Manager._meta.db.transaction() as transaction:
+                await Manager.insert(Manager(name="Manager 1"))
+                savepoint = await transaction.savepoint()
+                await Manager.insert(Manager(name="Manager 2"))
+                await savepoint.rollback_to()
+
+        run_sync(run_test())
+
+        self.assertListEqual(
+            Manager.select(Manager.name).run_sync(), [{"name": "Manager 1"}]
+        )
+
+    def test_named_savepoint(self):
+        async def run_test():
+            async with Manager._meta.db.transaction() as transaction:
+                await Manager.insert(Manager(name="Manager 1"))
+                await transaction.savepoint("my_savepoint")
+                await Manager.insert(Manager(name="Manager 2"))
+                await transaction.rollback_to("my_savepoint")
+
+        run_sync(run_test())
+
+        self.assertListEqual(
+            Manager.select(Manager.name).run_sync(), [{"name": "Manager 1"}]
+        )
```

### Comparing `piccolo-0.99.0/tests/engine/test_version_parsing.py` & `piccolo-1.0a1/tests/engine/test_version_parsing.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py` & `piccolo-1.0a1/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/example_apps/mega/tables.py` & `piccolo-1.0a1/tests/example_apps/mega/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/example_apps/music/tables.py` & `piccolo-1.0a1/tests/example_apps/music/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/example_apps/music/tables_detailed.py` & `piccolo-1.0a1/tests/example_apps/music/tables_detailed.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/query/mixins/test_columns_delegate.py` & `piccolo-1.0a1/tests/query/mixins/test_columns_delegate.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/query/test_camelcase.py` & `piccolo-1.0a1/tests/query/test_camelcase.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/query/test_freeze.py` & `piccolo-1.0a1/tests/query/test_freeze.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import timeit
 import typing as t
 from dataclasses import dataclass
+from unittest import mock
 
+from piccolo.columns import Integer, Varchar
 from piccolo.query.base import Query
-from tests.base import DBTestCase, sqlite_only
+from piccolo.table import Table
+from tests.base import AsyncMock, DBTestCase, sqlite_only
 from tests.example_apps.music.tables import Band
 
 
 @dataclass
 class QueryResponse:
     query: Query
     response: t.Any
@@ -75,33 +78,47 @@
 
     @sqlite_only
     def test_frozen_performance(self):
         """
         The frozen query performance should exceed the non-frozen. If not,
         there's a problem.
 
-        Only test this on SQLite, as the latency from the database itself
-        is more predictable than with Postgres, and the test runs quickly.
+        We mock out the database to make the performance more predictable.
 
         """
+        db = mock.MagicMock()
+        db.engine_type = "sqlite"
+        db.run_querystring = AsyncMock()
+        db.run_querystring.return_value = [
+            {"name": "Pythonistas", "popularity": 1000}
+        ]
+
+        class Band(Table, db=db):
+            name = Varchar()
+            popularity = Integer()
+
         iterations = 50
-        query = Band.select().where(Band.name == "Pythonistas").first()
+        query = (
+            Band.select(Band.name)
+            .where(Band.popularity > 900)
+            .order_by(Band.name)
+        )
         query_duration = timeit.repeat(
             lambda: query.run_sync(), repeat=iterations, number=1
         )
 
         frozen_query = query.freeze()
         frozen_query_duration = timeit.repeat(
             lambda: frozen_query.run_sync(), repeat=iterations, number=1
         )
 
         # Remove the outliers before comparing
         self.assertGreater(
-            sum(sorted(query_duration)[5:-5]),
-            sum(sorted(frozen_query_duration)[5:-5]),
+            sum(sorted(query_duration)[10:-10]),
+            sum(sorted(frozen_query_duration)[10:-10]),
         )
 
     def test_attribute_access(self):
         """
         Once frozen, you shouldn't be able to call additional methods on the
         query (for example `.where`).
         """
```

### Comparing `piccolo-0.99.0/tests/query/test_gather.py` & `piccolo-1.0a1/tests/query/test_gather.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/query/test_querystring.py` & `piccolo-1.0a1/tests/query/test_querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/query/test_slots.py` & `piccolo-1.0a1/tests/query/test_slots.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/instance/test_create.py` & `piccolo-1.0a1/tests/table/instance/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/instance/test_get_related.py` & `piccolo-1.0a1/tests/table/instance/test_get_related.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/instance/test_get_related_readable.py` & `piccolo-1.0a1/tests/table/instance/test_get_related_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/instance/test_instantiate.py` & `piccolo-1.0a1/tests/table/instance/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/instance/test_remove.py` & `piccolo-1.0a1/tests/table/instance/test_remove.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/instance/test_save.py` & `piccolo-1.0a1/tests/table/instance/test_save.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/instance/test_to_dict.py` & `piccolo-1.0a1/tests/table/instance/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_all_columns.py` & `piccolo-1.0a1/tests/table/test_all_columns.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_alter.py` & `piccolo-1.0a1/tests/table/test_alter.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from unittest import TestCase
 
 import pytest
 
 from piccolo.columns import BigInt, Integer, Numeric, Varchar
 from piccolo.columns.base import Column
 from piccolo.columns.column_types import ForeignKey, Text
+from piccolo.schema import SchemaManager
 from piccolo.table import Table
 from tests.base import (
     DBTestCase,
     engine_version_lt,
     engines_only,
     is_running_sqlite,
 )
@@ -319,14 +320,73 @@
             "INSERT INTO manager (id, name) VALUES (DEFAULT, DEFAULT);"
         ).run_sync()
 
         manager = Manager.objects().first().run_sync()
         self.assertEqual(manager.name, "Pending")
 
 
+@engines_only("postgres", "cockroach")
+class TestSetSchema(TestCase):
+
+    schema_manager = SchemaManager()
+    schema_name = "schema_1"
+
+    def setUp(self):
+        Manager.create_table().run_sync()
+        self.schema_manager.create_schema(
+            schema_name=self.schema_name
+        ).run_sync()
+
+    def tearDown(self):
+        Manager.alter().drop_table(if_exists=True).run_sync()
+        self.schema_manager.drop_schema(
+            schema_name=self.schema_name, cascade=True
+        ).run_sync()
+
+    def test_set_schema(self):
+        Manager.alter().set_schema(schema_name=self.schema_name).run_sync()
+
+        self.assertIn(
+            Manager._meta.tablename,
+            self.schema_manager.list_tables(
+                schema_name=self.schema_name
+            ).run_sync(),
+        )
+
+
+@engines_only("postgres", "cockroach")
+class TestDropTable(TestCase):
+    class Manager(Table, schema="schema_1"):
+        pass
+
+    schema_manager = SchemaManager()
+
+    def tearDown(self):
+        self.schema_manager.drop_schema(
+            schema_name="schema_1", if_exists=True, cascade=True
+        ).run_sync()
+
+    def test_drop_table_with_schema(self):
+        Manager = self.Manager
+
+        Manager.create_table().run_sync()
+
+        self.assertIn(
+            "manager",
+            self.schema_manager.list_tables(schema_name="schema_1").run_sync(),
+        )
+
+        Manager.alter().drop_table().run_sync()
+
+        self.assertNotIn(
+            "manager",
+            self.schema_manager.list_tables(schema_name="schema_1").run_sync(),
+        )
+
+
 ###############################################################################
 
 
 class Ticket(Table):
     price = Numeric(digits=(5, 2))
```

### Comparing `piccolo-0.99.0/tests/table/test_batch.py` & `piccolo-1.0a1/tests/table/test_batch.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_callback.py` & `piccolo-1.0a1/tests/table/test_callback.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_constructor.py` & `piccolo-1.0a1/tests/table/test_constructor.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_create_db_tables.py` & `piccolo-1.0a1/tests/table/test_create_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_delete.py` & `piccolo-1.0a1/tests/table/test_delete.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_drop_db_tables.py` & `piccolo-1.0a1/tests/table/test_drop_db_tables.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     def setUp(self):
         create_db_tables_sync(Band, Manager)
 
     def test_drop_db_tables(self):
         """
         Make sure the tables are dropped.
         """
-        self.assertEqual(Manager.table_exists().run_sync(), True)
-        self.assertEqual(Band.table_exists().run_sync(), True)
+        self.assertTrue(Manager.table_exists().run_sync())
+        self.assertTrue(Band.table_exists().run_sync())
 
         drop_db_tables_sync(Manager, Band)
 
-        self.assertEqual(Manager.table_exists().run_sync(), False)
-        self.assertEqual(Band.table_exists().run_sync(), False)
+        self.assertFalse(Manager.table_exists().run_sync())
+        self.assertFalse(Band.table_exists().run_sync())
 
     def test_drop_tables(self):
         """
         This is a deprecated function, which just acts as a proxy.
         """
-        self.assertEqual(Manager.table_exists().run_sync(), True)
-        self.assertEqual(Band.table_exists().run_sync(), True)
+        self.assertTrue(Manager.table_exists().run_sync())
+        self.assertTrue(Band.table_exists().run_sync())
 
         drop_tables(Manager, Band)
 
-        self.assertEqual(Manager.table_exists().run_sync(), False)
-        self.assertEqual(Band.table_exists().run_sync(), False)
+        self.assertFalse(Manager.table_exists().run_sync())
+        self.assertFalse(Band.table_exists().run_sync())
```

### Comparing `piccolo-0.99.0/tests/table/test_from_dict.py` & `piccolo-1.0a1/tests/table/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_indexes.py` & `piccolo-1.0a1/tests/table/test_indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_inheritance.py` & `piccolo-1.0a1/tests/table/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_join.py` & `piccolo-1.0a1/tests/table/test_join.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,32 @@
                     "band_1.manager.id": 1,
                     "band_1.manager.name": "Guido",
                     "band_2.manager.id": 2,
                     "band_2.manager.name": "Graydon",
                 },
             )
 
+    def test_proxy_columns(self):
+        """
+        Make sure that ``proxy_columns`` are set correctly.
+
+        There used to be a bug which meant queries got slower over time:
+
+        https://github.com/piccolo-orm/piccolo/issues/691
+
+        """
+        # We call it multiple times to make sure it doesn't change with time.
+        for _ in range(2):
+            self.assertEqual(
+                len(Concert.band_1.manager._foreign_key_meta.proxy_columns), 2
+            )
+            self.assertEqual(
+                len(Concert.band_1._foreign_key_meta.proxy_columns), 4
+            )
+
     def test_select_all_columns_root(self):
         """
         Make sure that using ``all_columns`` at the root doesn't interfere
         with using it for referenced tables.
         """
         result = (
             Band.select(
```

### Comparing `piccolo-0.99.0/tests/table/test_objects.py` & `piccolo-1.0a1/tests/table/test_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,20 @@
 class TestOffset(DBTestCase):
     @engines_only("postgres", "cockroach")
     def test_offset_postgres(self):
         """
         Postgres can do an offset without a limit clause.
         """
         self.insert_rows()
+
         response = Band.objects().order_by(Band.name).offset(1).run_sync()
+
         self.assertEqual(
-            [i.name for i in response], ["Pythonistas", "Rustaceans"]
+            [i.name for i in response],
+            ["Pythonistas", "Rustaceans"],
         )
 
     @sqlite_only
     def test_offset_sqlite(self):
         """
         SQLite requires a limit clause for offset to work.
         """
```

### Comparing `piccolo-0.99.0/tests/table/test_output.py` & `piccolo-1.0a1/tests/table/test_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,10 +97,10 @@
 
         response = (
             Band.select(Band.name, Band.manager.name)
             .first()
             .output(nested=True)
             .run_sync()
         )
-        self.assertEqual(
+        self.assertDictEqual(
             response, {"name": "Pythonistas", "manager": {"name": "Guido"}}
         )
```

### Comparing `piccolo-0.99.0/tests/table/test_raw.py` & `piccolo-1.0a1/tests/table/test_raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tests.example_apps.music.tables import Band
 
 
 class TestRaw(DBTestCase):
     def test_raw_without_args(self):
         self.insert_row()
 
-        response = Band.raw("select * from band").run_sync()
+        response = Band.raw("SELECT * FROM band").run_sync()
 
         if engine_is("cockroach"):
             self.assertDictEqual(
                 response[0],
                 {
                     "id": response[0]["id"],
                     "name": "Pythonistas",
@@ -29,15 +29,15 @@
                 },
             )
 
     def test_raw_with_args(self):
         self.insert_rows()
 
         response = Band.raw(
-            "select * from band where name = {}", "Pythonistas"
+            "SELECT * FROM band WHERE name = {}", "Pythonistas"
         ).run_sync()
 
         self.assertEqual(len(response), 1)
 
         if engine_is("cockroach"):
             self.assertDictEqual(
                 response[0],
```

### Comparing `piccolo-0.99.0/tests/table/test_refresh.py` & `piccolo-1.0a1/tests/table/test_refresh.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class TestRefresh(DBTestCase):
     def setUp(self):
         super().setUp()
         self.insert_rows()
 
     def test_refresh(self):
         """
-        Make sure ``refresh`` works, with not columns specified.
+        Make sure ``refresh`` works, with no columns specified.
         """
         # Fetch an instance from the database.
         band: Band = Band.objects().get(Band.name == "Pythonistas").run_sync()
         initial_data = band.to_dict()
 
         # Modify the data in the database.
         Band.update(
```

### Comparing `piccolo-0.99.0/tests/table/test_select.py` & `piccolo-1.0a1/tests/table/test_select.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+import datetime
 from unittest import TestCase
 
+import pytest
+
 from piccolo.apps.user.tables import BaseUser
+from piccolo.columns import Date, Varchar
 from piccolo.columns.combination import WhereRaw
 from piccolo.query import OrderByRaw
-from piccolo.query.methods.select import Avg, Count, Max, Min, Sum
-from piccolo.table import create_db_tables_sync, drop_db_tables_sync
+from piccolo.query.methods.select import Avg, Count, Max, Min, SelectRaw, Sum
+from piccolo.query.mixins import DistinctOnError
+from piccolo.table import Table, create_db_tables_sync, drop_db_tables_sync
 from tests.base import (
     DBTestCase,
     engine_is,
+    engine_version_lt,
     engines_only,
     engines_skip,
+    is_running_cockroach,
+    is_running_sqlite,
     sqlite_only,
 )
 from tests.example_apps.music.tables import Band, Concert, Manager, Venue
 
 
 class TestSelect(DBTestCase):
     def test_query_all_columns(self):
@@ -512,14 +520,35 @@
 
         query = query.distinct()
         self.assertIn("DISTINCT", query.__str__())
 
         response = query.run_sync()
         self.assertEqual(response, [{"name": "Pythonistas"}])
 
+    def test_distinct_on(self):
+        """
+        Make sure the distinct clause works, with the ``on`` param.
+        """
+        self.insert_rows()
+        self.insert_rows()
+
+        query = Band.select(Band.name).where(Band.name == "Pythonistas")
+        self.assertNotIn("DISTINCT", query.__str__())
+
+        response = query.run_sync()
+        self.assertEqual(
+            response, [{"name": "Pythonistas"}, {"name": "Pythonistas"}]
+        )
+
+        query = query.distinct()
+        self.assertIn("DISTINCT", query.__str__())
+
+        response = query.run_sync()
+        self.assertEqual(response, [{"name": "Pythonistas"}])
+
     def test_count_group_by(self):
         """
         Test grouping and counting all rows.
         """
         self.insert_rows()
         self.insert_rows()
 
@@ -956,14 +985,36 @@
             .where(Band.manager.name == "Guido")
             .run_sync()
         )
         self.assertEqual(
             response, [{"name": "Pythonistas", "manager_name": "Guido"}]
         )
 
+    @pytest.mark.skipif(
+        is_running_sqlite() and engine_version_lt(3.35),
+        reason="SQLite doesn't have math functions in this version.",
+    )
+    @pytest.mark.skipif(
+        is_running_cockroach(),
+        reason=(
+            "Cockroach raises an error when trying to use the log function."
+        ),
+    )
+    def test_select_raw(self):
+        """
+        Make sure ``SelectRaw`` can be used in select queries.
+        """
+        self.insert_row()
+        response = Band.select(
+            Band.name, SelectRaw("round(log(popularity)) AS popularity_log")
+        ).run_sync()
+        self.assertListEqual(
+            response, [{"name": "Pythonistas", "popularity_log": 3.0}]
+        )
+
 
 class TestSelectSecret(TestCase):
     def setUp(self):
         BaseUser.create_table().run_sync()
 
     def tearDown(self):
         BaseUser.alter().drop_table().run_sync()
@@ -1206,7 +1257,142 @@
             [
                 {"name": "C-Sharps"},
                 {"name": "Pythonistas"},
                 {"name": "Rubyists"},
                 {"name": "Rustaceans"},
             ],
         )
+
+
+class Album(Table):
+    band = Varchar()
+    title = Varchar()
+    release_date = Date()
+
+
+class TestDistinctOn(TestCase):
+    def setUp(self):
+        Album.create_table().run_sync()
+
+    def tearDown(self):
+        Album.alter().drop_table().run_sync()
+
+    @engines_only("postgres", "cockroach")
+    def test_distinct_on(self):
+        """
+        Make sure the ``distinct`` method can be used to create a
+        ``DISTINCT ON`` clause.
+        """
+        Album.insert(
+            Album(
+                {
+                    Album.band: "Pythonistas",
+                    Album.title: "P1",
+                    Album.release_date: datetime.date(
+                        year=2022, month=1, day=1
+                    ),
+                }
+            ),
+            Album(
+                {
+                    Album.band: "Pythonistas",
+                    Album.title: "P2",
+                    Album.release_date: datetime.date(
+                        year=2023, month=1, day=1
+                    ),
+                }
+            ),
+            Album(
+                {
+                    Album.band: "Rustaceans",
+                    Album.title: "R1",
+                    Album.release_date: datetime.date(
+                        year=2022, month=1, day=1
+                    ),
+                }
+            ),
+            Album(
+                {
+                    Album.band: "Rustaceans",
+                    Album.title: "R2",
+                    Album.release_date: datetime.date(
+                        year=2023, month=1, day=1
+                    ),
+                }
+            ),
+            Album(
+                {
+                    Album.band: "C-Sharps",
+                    Album.title: "C1",
+                    Album.release_date: datetime.date(
+                        year=2022, month=1, day=1
+                    ),
+                }
+            ),
+            Album(
+                {
+                    Album.band: "C-Sharps",
+                    Album.title: "C2",
+                    Album.release_date: datetime.date(
+                        year=2023, month=1, day=1
+                    ),
+                }
+            ),
+        ).run_sync()
+
+        # Get the most recent album for each band.
+        query = (
+            Album.select(Album.band, Album.title)
+            .distinct(on=[Album.band])
+            .order_by(Album.band)
+            .order_by(Album.release_date, ascending=False)
+        )
+        self.assertIn("DISTINCT ON", query.__str__())
+        response = query.run_sync()
+
+        self.assertEqual(
+            response,
+            [
+                {"band": "C-Sharps", "title": "C2"},
+                {"band": "Pythonistas", "title": "P2"},
+                {"band": "Rustaceans", "title": "R2"},
+            ],
+        )
+
+    @engines_only("sqlite")
+    def test_distinct_on_sqlite(self):
+        """
+        SQLite doesn't support ``DISTINCT ON``, so a ``ValueError`` should be
+        raised.
+        """
+        with self.assertRaises(NotImplementedError) as manager:
+            Album.select().distinct(on=[Album.band])
+
+        self.assertEqual(
+            manager.exception.__str__(),
+            "SQLite doesn't support DISTINCT ON",
+        )
+
+    @engines_only("postgres", "cockroach")
+    def test_distinct_on_error(self):
+        """
+        If we pass in something other than a sequence of columns, it should
+        raise a ValueError.
+        """
+        with self.assertRaises(ValueError) as manager:
+            Album.select().distinct(on=Album.band)
+
+        self.assertEqual(
+            manager.exception.__str__(),
+            "`on` must be a sequence of `Column` instances",
+        )
+
+    @engines_only("postgres", "cockroach")
+    def test_distinct_on_order_by_error(self):
+        """
+        The first column passed to `order_by` must match the first column
+        passed to `on`, otherwise an exception is raised.
+        """
+        with self.assertRaises(DistinctOnError):
+            Album.select().distinct(on=[Album.band]).order_by(
+                Album.release_date
+            ).run_sync()
```

### Comparing `piccolo-0.99.0/tests/table/test_str.py` & `piccolo-1.0a1/tests/table/test_str.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/table/test_update.py` & `piccolo-1.0a1/tests/table/test_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from tests.base import (
     DBTestCase,
     engine_version_lt,
     engines_skip,
     is_running_sqlite,
     sqlite_only,
 )
-from tests.example_apps.music.tables import Band
+from tests.example_apps.music.tables import Band, Manager
 
 
 class TestUpdate(DBTestCase):
     def check_response(self):
         response = (
             Band.select(Band.name)
             .where(Band.name == "Pythonistas3")
@@ -624,7 +624,93 @@
                 AutoUpdateTable.name, AutoUpdateTable.modified_on
             )
             .first()
             .run_sync()
         )
         self.assertIsInstance(updated_row["modified_on"], datetime.datetime)
         self.assertEqual(updated_row["name"], "test 2")
+
+
+###############################################################################
+# Test update with joins
+
+
+class TestUpdateWithJoin(DBTestCase):
+    def test_join(self):
+        """
+        Make sure updates work when the where clause needs a join.
+        """
+        self.insert_rows()
+        Band.update({Band.name: "New name"}).where(
+            Band.manager.name == "Guido"
+        ).run_sync()
+
+        self.assertEqual(
+            Band.count().where(Band.name == "New name").run_sync(), 1
+        )
+
+    def test_multiple_matches(self):
+        """
+        Make sure it works when the join has multiple matching values.
+        """
+        self.insert_rows()
+
+        # Create an additional band with the same manager.
+        manager = Manager.objects().get(Manager.name == "Guido").run_sync()
+        band = Band(name="Pythonistas 2", manager=manager)
+        band.save().run_sync()
+
+        Band.update({Band.name: "New name"}).where(
+            Band.manager.name == "Guido"
+        ).run_sync()
+
+        self.assertEqual(
+            Band.count().where(Band.name == "New name").run_sync(), 2
+        )
+
+    def test_no_matches(self):
+        """
+        Make sure it works when the join has no matching values.
+        """
+        self.insert_rows()
+
+        Band.update({Band.name: "New name"}).where(
+            Band.manager.name == "Mr Manager"
+        ).run_sync()
+
+        self.assertEqual(
+            Band.count().where(Band.name == "New name").run_sync(), 0
+        )
+
+    def test_and(self):
+        """
+        Make sure it works when combined with other where clauses using AND.
+        """
+        self.insert_rows()
+
+        # Create an additional band with the same manager, and different
+        # popularity.
+        manager = Manager.objects().get(Manager.name == "Guido").run_sync()
+        band = Band(name="Pythonistas 2", manager=manager, popularity=10000)
+        band.save().run_sync()
+
+        Band.update({Band.name: "New name"}).where(
+            Band.manager.name == "Guido", Band.popularity == 10000
+        ).run_sync()
+
+        self.assertEqual(
+            Band.count().where(Band.name == "New name").run_sync(), 1
+        )
+
+    def test_or(self):
+        """
+        Make sure it works when combined with other where clauses using OR.
+        """
+        self.insert_rows()
+
+        Band.update({Band.name: "New name"}).where(
+            (Band.manager.name == "Guido") | (Band.manager.name == "Graydon")
+        ).run_sync()
+
+        self.assertEqual(
+            Band.count().where(Band.name == "New name").run_sync(), 2
+        )
```

### Comparing `piccolo-0.99.0/tests/testing/test_model_builder.py` & `piccolo-1.0a1/tests/testing/test_model_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import asyncio
+import typing as t
 import unittest
 
-from piccolo.columns import Array, Integer, Real, Varchar
-from piccolo.table import Table
+from piccolo.columns import (
+    Array,
+    Decimal,
+    ForeignKey,
+    Integer,
+    LazyTableReference,
+    Numeric,
+    Real,
+    Varchar,
+)
+from piccolo.table import Table, create_db_tables_sync, drop_db_tables_sync
 from piccolo.testing.model_builder import ModelBuilder
 from tests.base import engines_skip
 from tests.example_apps.music.tables import (
     Band,
     Concert,
     Manager,
     Poster,
@@ -19,131 +29,137 @@
 
 class TableWithArrayField(Table):
     strings = Array(Varchar(30))
     integers = Array(Integer())
     floats = Array(Real())
 
 
+class TableWithDecimal(Table):
+    numeric = Numeric()
+    numeric_with_digits = Numeric(digits=(4, 2))
+    decimal = Decimal()
+    decimal_with_digits = Decimal(digits=(4, 2))
+
+
+class BandWithLazyReference(Table):
+    manager = ForeignKey(
+        references=LazyTableReference(
+            "Manager", module_path="tests.example_apps.music.tables"
+        )
+    )
+
+
+TABLES = (
+    Manager,
+    Band,
+    Poster,
+    RecordingStudio,
+    Shirt,
+    Venue,
+    Concert,
+    Ticket,
+    TableWithArrayField,
+    TableWithDecimal,
+    BandWithLazyReference,
+)
+
+
 # Cockroach Bug: Can turn ON when resolved: https://github.com/cockroachdb/cockroach/issues/71908  # noqa: E501
 @engines_skip("cockroach")
 class TestModelBuilder(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-
-        for table_class in (
-            Manager,
-            Band,
-            Poster,
-            RecordingStudio,
-            Shirt,
-            Venue,
-            Concert,
-            Ticket,
-            TableWithArrayField,
-        ):
-            table_class.create_table().run_sync()
+        create_db_tables_sync(*TABLES)
 
     @classmethod
     def tearDownClass(cls) -> None:
-        for table_class in (
-            TableWithArrayField,
-            Ticket,
-            Concert,
-            Venue,
-            Shirt,
-            RecordingStudio,
-            Poster,
-            Band,
-            Manager,
-        ):
-            table_class.alter().drop_table().run_sync()
-
-    def test_model_builder_async(self):
-        async def build_model(model):
-            return await ModelBuilder.build(model)
-
-        asyncio.run(build_model(Manager))
-        asyncio.run(build_model(Ticket))
-        asyncio.run(build_model(Poster))
-        asyncio.run(build_model(RecordingStudio))
-        asyncio.run(build_model(TableWithArrayField))
-
-    def test_model_builder_sync(self):
-        ModelBuilder.build_sync(Manager)
-        ModelBuilder.build_sync(Ticket)
-        ModelBuilder.build_sync(Poster)
-        ModelBuilder.build_sync(RecordingStudio)
-        ModelBuilder.build_sync(TableWithArrayField)
+        drop_db_tables_sync(*TABLES)
+
+    def test_async(self):
+        async def build_model(table_class: t.Type[Table]):
+            return await ModelBuilder.build(table_class)
+
+        for table_class in TABLES:
+            asyncio.run(build_model(table_class))
+
+    def test_sync(self):
+        for table_class in TABLES:
+            ModelBuilder.build_sync(table_class)
 
-    def test_model_builder_with_choices(self):
+    def test_choices(self):
         shirt = ModelBuilder.build_sync(Shirt)
         queried_shirt = (
             Shirt.objects().where(Shirt.id == shirt.id).first().run_sync()
         )
 
         self.assertIn(
             queried_shirt.size,
             ["s", "l", "m"],
         )
 
-    def test_model_builder_with_foreign_key(self):
-        ModelBuilder.build_sync(Band)
+    def test_foreign_key(self):
+        model = ModelBuilder.build_sync(Band, persist=True)
 
-    def test_model_builder_with_invalid_column(self):
+        self.assertTrue(
+            Manager.exists().where(Manager.id == model.manager).run_sync()
+        )
+
+    def test_lazy_foreign_key(self):
+        model = ModelBuilder.build_sync(BandWithLazyReference, persist=True)
+
+        self.assertTrue(
+            Manager.exists().where(Manager.id == model.manager).run_sync()
+        )
+
+    def test_invalid_column(self):
         with self.assertRaises(ValueError):
             ModelBuilder.build_sync(Band, defaults={"X": 1})
 
-    def test_model_builder_with_minimal(self):
+    def test_minimal(self):
         band = ModelBuilder.build_sync(Band, minimal=True)
 
-        self.assertEqual(
-            Band.exists().where(Band.id == band.id).run_sync(),
-            True,
-        )
+        self.assertTrue(Band.exists().where(Band.id == band.id).run_sync())
 
-    def test_model_builder_with_no_persist(self):
+    def test_persist_false(self):
         band = ModelBuilder.build_sync(Band, persist=False)
 
-        self.assertEqual(
-            Band.exists().where(Band.id == band.id).run_sync(),
-            False,
-        )
+        self.assertFalse(Band.exists().where(Band.id == band.id).run_sync())
 
-    def test_model_builder_with_valid_column(self):
+    def test_valid_column(self):
         manager = ModelBuilder.build_sync(
             Manager, defaults={Manager.name: "Guido"}
         )
 
         queried_manager = (
             Manager.objects()
             .where(Manager.id == manager.id)
             .first()
             .run_sync()
         )
 
         self.assertEqual(queried_manager.name, "Guido")
 
-    def test_model_builder_with_valid_column_string(self):
+    def test_valid_column_string(self):
         manager = ModelBuilder.build_sync(Manager, defaults={"name": "Guido"})
 
         queried_manager = (
             Manager.objects()
             .where(Manager.id == manager.id)
             .first()
             .run_sync()
         )
 
         self.assertEqual(queried_manager.name, "Guido")
 
-    def test_model_builder_with_valid_foreign_key(self):
+    def test_valid_foreign_key(self):
         manager = ModelBuilder.build_sync(Manager)
 
         band = ModelBuilder.build_sync(Band, defaults={Band.manager: manager})
 
         self.assertEqual(manager._meta.primary_key, band.manager)
 
-    def test_model_builder_with_valid_foreign_key_string(self):
+    def test_valid_foreign_key_string(self):
         manager = ModelBuilder.build_sync(Manager)
 
         band = ModelBuilder.build_sync(Band, defaults={"manager": manager})
 
         self.assertEqual(manager._meta.primary_key, band.manager)
```

### Comparing `piccolo-0.99.0/tests/testing/test_random_builder.py` & `piccolo-1.0a1/tests/testing/test_random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/utils/test_dictionary.py` & `piccolo-1.0a1/tests/utils/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/utils/test_lazy_loader.py` & `piccolo-1.0a1/tests/utils/test_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/utils/test_naming.py` & `piccolo-1.0a1/tests/utils/test_naming.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/utils/test_printing.py` & `piccolo-1.0a1/tests/utils/test_printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/utils/test_pydantic.py` & `piccolo-1.0a1/tests/utils/test_pydantic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import decimal
+import typing as t
 from unittest import TestCase
 
 import pydantic
+import pydantic_core
+import pytest
 from pydantic import ValidationError
 
 from piccolo.columns import (
     JSON,
     JSONB,
+    UUID,
     Array,
     Email,
     Integer,
     Numeric,
     Secret,
     Text,
+    Time,
     Varchar,
 )
 from piccolo.columns.column_types import ForeignKey
 from piccolo.table import Table
 from piccolo.utils.pydantic import create_pydantic_model
 
 
@@ -37,15 +42,17 @@
     def test_email(self):
         class Director(Table):
             email = Email()
 
         pydantic_model = create_pydantic_model(table=Director)
 
         self.assertEqual(
-            pydantic_model.schema()["properties"]["email"]["format"],
+            pydantic_model.model_json_schema()["properties"]["email"]["anyOf"][
+                0
+            ]["format"],
             "email",
         )
 
         with self.assertRaises(ValidationError):
             pydantic_model(email="not a valid email")
 
         # Shouldn't raise an exception:
@@ -92,30 +99,32 @@
 class TestSecretColumn(TestCase):
     def test_secret_param(self):
         class TopSecret(Table):
             confidential = Secret()
 
         pydantic_model = create_pydantic_model(table=TopSecret)
         self.assertEqual(
-            pydantic_model.schema()["properties"]["confidential"]["extra"][
-                "secret"
-            ],
+            pydantic_model.model_json_schema()["properties"]["confidential"][
+                "extra"
+            ]["secret"],
             True,
         )
 
 
 class TestArrayColumn(TestCase):
     def test_array_param(self):
         class Band(Table):
             members = Array(base_column=Varchar(length=16))
 
         pydantic_model = create_pydantic_model(table=Band)
 
         self.assertEqual(
-            pydantic_model.schema()["properties"]["members"]["items"]["type"],
+            pydantic_model.model_json_schema()["properties"]["members"][
+                "anyOf"
+            ][0]["items"]["type"],
             "string",
         )
 
 
 class TestForeignKeyColumn(TestCase):
     def test_target_column(self):
         """
@@ -131,84 +140,136 @@
         class BandB(Table):
             manager = ForeignKey(Manager, target_column="name")
 
         class BandC(Table):
             manager = ForeignKey(Manager)
 
         self.assertEqual(
-            create_pydantic_model(table=BandA).schema()["properties"][
-                "manager"
-            ]["extra"]["target_column"],
+            create_pydantic_model(table=BandA).model_json_schema()[
+                "properties"
+            ]["manager"]["extra"]["target_column"],
             "name",
         )
 
         self.assertEqual(
-            create_pydantic_model(table=BandB).schema()["properties"][
-                "manager"
-            ]["extra"]["target_column"],
+            create_pydantic_model(table=BandB).model_json_schema()[
+                "properties"
+            ]["manager"]["extra"]["target_column"],
             "name",
         )
 
         self.assertEqual(
-            create_pydantic_model(table=BandC).schema()["properties"][
-                "manager"
-            ]["extra"]["target_column"],
+            create_pydantic_model(table=BandC).model_json_schema()[
+                "properties"
+            ]["manager"]["extra"]["target_column"],
             "id",
         )
 
 
 class TestTextColumn(TestCase):
     def test_text_format(self):
         class Band(Table):
             bio = Text()
 
         pydantic_model = create_pydantic_model(table=Band)
 
         self.assertEqual(
-            pydantic_model.schema()["properties"]["bio"]["format"],
+            pydantic_model.model_json_schema()["properties"]["bio"]["format"],
             "text-area",
         )
 
 
+class TestTimeColumn(TestCase):
+    def test_time_format(self):
+        class Concert(Table):
+            start_time = Time()
+
+        pydantic_model = create_pydantic_model(table=Concert)
+
+        self.assertEqual(
+            pydantic_model.model_json_schema()["properties"]["start_time"][
+                "anyOf"
+            ][0]["format"],
+            "time",
+        )
+
+
+class TestUUIDColumn(TestCase):
+    class Ticket(Table):
+        code = UUID()
+
+    def setUp(self):
+        self.Ticket.create_table().run_sync()
+
+    def tearDown(self):
+        self.Ticket.alter().drop_table().run_sync()
+
+    def test_uuid_format(self):
+        class Ticket(Table):
+            code = UUID()
+
+        pydantic_model = create_pydantic_model(table=Ticket)
+
+        ticket = Ticket()
+        ticket.save().run_sync()
+
+        # We'll also fetch it from the DB in case the database adapter's UUID
+        # is used.
+        ticket_from_db = Ticket.objects().first().run_sync()
+
+        for ticket_ in (ticket, ticket_from_db):
+            json = pydantic_model(**ticket_.to_dict()).model_dump_json()
+            self.assertEqual(json, '{"code":"' + str(ticket_.code) + '"}')
+
+        self.assertEqual(
+            pydantic_model.model_json_schema()["properties"]["code"]["anyOf"][
+                0
+            ]["format"],
+            "uuid",
+        )
+
+
 class TestColumnHelpText(TestCase):
     """
     Make sure that columns with `help_text` attribute defined have the
     relevant text appear in the schema.
     """
 
-    def test_help_text_present(self):
+    def test_column_help_text_present(self):
         help_text = "In millions of US dollars."
 
         class Movie(Table):
             box_office = Numeric(digits=(5, 1), help_text=help_text)
 
         pydantic_model = create_pydantic_model(table=Movie)
+
         self.assertEqual(
-            pydantic_model.schema()["properties"]["box_office"]["extra"][
-                "help_text"
-            ],
+            pydantic_model.model_json_schema()["properties"]["box_office"][
+                "extra"
+            ]["help_text"],
             help_text,
         )
 
 
 class TestTableHelpText(TestCase):
     """
     Make sure that tables with `help_text` attribute defined have the
     relevant text appear in the schema.
     """
 
-    def test_help_text_present(self):
+    def test_table_help_text_present(self):
         help_text = "Movies which were released in cinemas."
 
         class Movie(Table, help_text=help_text):
             name = Varchar()
 
         pydantic_model = create_pydantic_model(table=Movie)
+
         self.assertEqual(
-            pydantic_model.schema()["help_text"],
+            pydantic_model.model_json_schema()["help_text"],
             help_text,
         )
 
 
 class TestJSONColumn(TestCase):
     def test_default(self):
         class Movie(Table):
@@ -257,15 +318,17 @@
     def test_json_format(self):
         class Movie(Table):
             features = JSON()
 
         pydantic_model = create_pydantic_model(table=Movie)
 
         self.assertEqual(
-            pydantic_model.schema()["properties"]["features"]["format"],
+            pydantic_model.model_json_schema()["properties"]["features"][
+                "format"
+            ],
             "json",
         )
 
     def test_null_value(self):
         class Movie(Table):
             meta = JSON(null=True)
             meta_b = JSONB(null=True)
@@ -281,55 +344,55 @@
     def test_all(self):
         class Computer(Table):
             CPU = Varchar()
             GPU = Varchar()
 
         pydantic_model = create_pydantic_model(Computer, exclude_columns=())
 
-        properties = pydantic_model.schema()["properties"]
+        properties = pydantic_model.model_json_schema()["properties"]
         self.assertIsInstance(properties["GPU"], dict)
         self.assertIsInstance(properties["CPU"], dict)
 
     def test_exclude(self):
         class Computer(Table):
             CPU = Varchar()
             GPU = Varchar()
 
         pydantic_model = create_pydantic_model(
             Computer,
             exclude_columns=(Computer.CPU,),
         )
 
-        properties = pydantic_model.schema()["properties"]
+        properties = pydantic_model.model_json_schema()["properties"]
         self.assertIsInstance(properties.get("GPU"), dict)
         self.assertIsNone(properties.get("CPU"))
 
     def test_exclude_all_manually(self):
         class Computer(Table):
             GPU = Varchar()
             CPU = Varchar()
 
         pydantic_model = create_pydantic_model(
             Computer,
             exclude_columns=(Computer.GPU, Computer.CPU),
         )
 
-        self.assertEqual(pydantic_model.schema()["properties"], {})
+        self.assertEqual(pydantic_model.model_json_schema()["properties"], {})
 
     def test_exclude_all_meta(self):
         class Computer(Table):
             GPU = Varchar()
             CPU = Varchar()
 
         pydantic_model = create_pydantic_model(
             Computer,
             exclude_columns=tuple(Computer._meta.columns),
         )
 
-        self.assertEqual(pydantic_model.schema()["properties"], {})
+        self.assertEqual(pydantic_model.model_json_schema()["properties"], {})
 
     def test_invalid_column_str(self):
         class Computer(Table):
             CPU = Varchar()
             GPU = Varchar()
 
         with self.assertRaises(ValueError):
@@ -379,15 +442,15 @@
             nested=(Band.manager,),
         )
 
         model_instance = pydantic_model(
             name="Pythonistas", manager={"name": "Guido"}
         )
         self.assertEqual(
-            model_instance.dict(),
+            model_instance.model_dump(),
             {"name": "Pythonistas", "manager": {"name": "Guido"}},
         )
 
 
 class TestIncludeColumns(TestCase):
     def test_include(self):
         class Band(Table):
@@ -395,15 +458,15 @@
             popularity = Integer()
 
         pydantic_model = create_pydantic_model(
             Band,
             include_columns=(Band.name,),
         )
 
-        properties = pydantic_model.schema()["properties"]
+        properties = pydantic_model.model_json_schema()["properties"]
         self.assertIsInstance(properties.get("name"), dict)
         self.assertIsNone(properties.get("popularity"))
 
     def test_include_exclude_error(self):
         """
         An exception should be raised if both `include_columns` and
         `exclude_columns` are provided.
@@ -443,15 +506,15 @@
             nested=(Band.manager,),
         )
 
         model_instance = pydantic_model(
             name="Pythonistas", manager={"name": "Guido"}
         )
         self.assertEqual(
-            model_instance.dict(),
+            model_instance.model_dump(),
             {"name": "Pythonistas", "manager": {"name": "Guido"}},
         )
 
 
 class TestNestedModel(TestCase):
     def test_true(self):
         """
@@ -470,25 +533,27 @@
             name = Varchar(length=10)
             manager = ForeignKey(Manager)
 
         BandModel = create_pydantic_model(table=Band, nested=True)
 
         #######################################################################
 
-        ManagerModel = BandModel.__fields__["manager"].type_
+        ManagerModel = BandModel.model_fields["manager"].annotation
         self.assertTrue(issubclass(ManagerModel, pydantic.BaseModel))
         self.assertEqual(
-            [i for i in ManagerModel.__fields__.keys()], ["name", "country"]
+            [i for i in ManagerModel.model_fields.keys()], ["name", "country"]
         )
 
         #######################################################################
 
-        CountryModel = ManagerModel.__fields__["country"].type_
+        CountryModel = ManagerModel.model_fields["country"].annotation
         self.assertTrue(issubclass(CountryModel, pydantic.BaseModel))
-        self.assertEqual([i for i in CountryModel.__fields__.keys()], ["name"])
+        self.assertEqual(
+            [i for i in CountryModel.model_fields.keys()], ["name"]
+        )
 
     def test_tuple(self):
         """
         Make sure only the specified foreign key columns are converted to
         nested models.
         """
 
@@ -513,91 +578,99 @@
             venue = ForeignKey(Venue)
 
         #######################################################################
         # Test one level deep
 
         BandModel = create_pydantic_model(table=Band, nested=(Band.manager,))
 
-        ManagerModel = BandModel.__fields__["manager"].type_
+        ManagerModel = BandModel.model_fields["manager"].annotation
         self.assertTrue(issubclass(ManagerModel, pydantic.BaseModel))
         self.assertEqual(
-            [i for i in ManagerModel.__fields__.keys()], ["name", "country"]
+            [i for i in ManagerModel.model_fields.keys()], ["name", "country"]
         )
         self.assertEqual(ManagerModel.__qualname__, "Band.manager")
 
-        AssistantManagerType = BandModel.__fields__["assistant_manager"].type_
-        self.assertIs(AssistantManagerType, int)
+        AssistantManagerType = BandModel.model_fields[
+            "assistant_manager"
+        ].annotation
+        self.assertIs(AssistantManagerType, t.Optional[int])
 
         #######################################################################
         # Test two levels deep
 
         BandModel = create_pydantic_model(
             table=Band, nested=(Band.manager.country,)
         )
 
-        ManagerModel = BandModel.__fields__["manager"].type_
+        ManagerModel = BandModel.model_fields["manager"].annotation
         self.assertTrue(issubclass(ManagerModel, pydantic.BaseModel))
         self.assertEqual(
-            [i for i in ManagerModel.__fields__.keys()], ["name", "country"]
+            [i for i in ManagerModel.model_fields.keys()], ["name", "country"]
         )
         self.assertEqual(ManagerModel.__qualname__, "Band.manager")
 
-        AssistantManagerType = BandModel.__fields__["assistant_manager"].type_
-        self.assertIs(AssistantManagerType, int)
+        AssistantManagerType = BandModel.model_fields[
+            "assistant_manager"
+        ].annotation
+        self.assertIs(AssistantManagerType, t.Optional[int])
 
-        CountryModel = ManagerModel.__fields__["country"].type_
+        CountryModel = ManagerModel.model_fields["country"].annotation
         self.assertTrue(issubclass(CountryModel, pydantic.BaseModel))
-        self.assertEqual([i for i in CountryModel.__fields__.keys()], ["name"])
+        self.assertEqual(
+            [i for i in CountryModel.model_fields.keys()], ["name"]
+        )
         self.assertEqual(CountryModel.__qualname__, "Band.manager.country")
 
         #######################################################################
         # Test three levels deep
 
         ConcertModel = create_pydantic_model(
             Concert, nested=(Concert.band_1.manager,)
         )
 
-        VenueModel = ConcertModel.__fields__["venue"].type_
-        self.assertIs(VenueModel, int)
+        VenueModel = ConcertModel.model_fields["venue"].annotation
+        self.assertIs(VenueModel, t.Optional[int])
 
-        BandModel = ConcertModel.__fields__["band_1"].type_
+        BandModel = ConcertModel.model_fields["band_1"].annotation
         self.assertTrue(issubclass(BandModel, pydantic.BaseModel))
         self.assertEqual(
-            [i for i in BandModel.__fields__.keys()],
+            [i for i in BandModel.model_fields.keys()],
             ["name", "manager", "assistant_manager"],
         )
         self.assertEqual(BandModel.__qualname__, "Concert.band_1")
 
-        ManagerModel = BandModel.__fields__["manager"].type_
+        ManagerModel = BandModel.model_fields["manager"].annotation
         self.assertTrue(issubclass(ManagerModel, pydantic.BaseModel))
         self.assertEqual(
-            [i for i in ManagerModel.__fields__.keys()],
+            [i for i in ManagerModel.model_fields.keys()],
             ["name", "country"],
         )
         self.assertEqual(ManagerModel.__qualname__, "Concert.band_1.manager")
 
-        AssistantManagerType = BandModel.__fields__["assistant_manager"].type_
-        self.assertIs(AssistantManagerType, int)
+        AssistantManagerType = BandModel.model_fields[
+            "assistant_manager"
+        ].annotation
+        self.assertIs(AssistantManagerType, t.Optional[int])
 
-        CountryModel = ManagerModel.__fields__["country"].type_
-        self.assertIs(CountryModel, int)
+        CountryModel = ManagerModel.model_fields["country"].annotation
+        self.assertIs(CountryModel, t.Optional[int])
 
         #######################################################################
         # Test with `model_name` arg
 
         MyConcertModel = create_pydantic_model(
             Concert,
             nested=(Concert.band_1.manager,),
             model_name="MyConcertModel",
         )
 
-        BandModel = MyConcertModel.__fields__["band_1"].type_
+        BandModel = MyConcertModel.model_fields["band_1"].annotation
         self.assertEqual(BandModel.__qualname__, "MyConcertModel.band_1")
 
-        ManagerModel = BandModel.__fields__["manager"].type_
+        ManagerModel = BandModel.model_fields["manager"].annotation
         self.assertEqual(
             ManagerModel.__qualname__, "MyConcertModel.band_1.manager"
         )
 
     def test_cascaded_args(self):
         """
         Make sure that arguments passed to ``create_pydantic_model`` are
@@ -615,25 +688,25 @@
             name = Varchar(length=10)
             manager = ForeignKey(Manager)
 
         BandModel = create_pydantic_model(
             table=Band, nested=True, include_default_columns=True
         )
 
-        ManagerModel = BandModel.__fields__["manager"].type_
+        ManagerModel = BandModel.model_fields["manager"].annotation
         self.assertTrue(issubclass(ManagerModel, pydantic.BaseModel))
         self.assertEqual(
-            [i for i in ManagerModel.__fields__.keys()],
+            [i for i in ManagerModel.model_fields.keys()],
             ["id", "name", "country"],
         )
 
-        CountryModel = ManagerModel.__fields__["country"].type_
+        CountryModel = ManagerModel.model_fields["country"].annotation
         self.assertTrue(issubclass(CountryModel, pydantic.BaseModel))
         self.assertEqual(
-            [i for i in CountryModel.__fields__.keys()], ["id", "name"]
+            [i for i in CountryModel.model_fields.keys()], ["id", "name"]
         )
 
 
 class TestRecursionDepth(TestCase):
     def test_max(self):
         class Country(Table):
             name = Varchar()
@@ -654,26 +727,26 @@
             band = ForeignKey(Band)
             venue = ForeignKey(Venue)
 
         ConcertModel = create_pydantic_model(
             table=Concert, nested=True, max_recursion_depth=2
         )
 
-        VenueModel = ConcertModel.__fields__["venue"].type_
+        VenueModel = ConcertModel.model_fields["venue"].annotation
         self.assertTrue(issubclass(VenueModel, pydantic.BaseModel))
 
-        BandModel = ConcertModel.__fields__["band"].type_
+        BandModel = ConcertModel.model_fields["band"].annotation
         self.assertTrue(issubclass(BandModel, pydantic.BaseModel))
 
-        ManagerModel = BandModel.__fields__["manager"].type_
+        ManagerModel = BandModel.model_fields["manager"].annotation
         self.assertTrue(issubclass(ManagerModel, pydantic.BaseModel))
 
         # We should have hit the recursion depth:
-        CountryModel = ManagerModel.__fields__["country"].type_
-        self.assertIs(CountryModel, int)
+        CountryModel = ManagerModel.model_fields["country"].annotation
+        self.assertIs(CountryModel, t.Optional[int])
 
 
 class TestDBColumnName(TestCase):
     def test_db_column_name(self):
         """
         Make sure that the Pydantic model has an alias if ``db_column_name``
         is specified for a column.
@@ -696,8 +769,40 @@
         Pydantic model's schema.
         """
 
         class Band(Table):
             name = Varchar()
 
         model = create_pydantic_model(Band, visible_columns=("name",))
-        self.assertEqual(model.schema()["visible_columns"], ("name",))
+        self.assertEqual(
+            model.model_json_schema()["visible_columns"], ("name",)
+        )
+
+
+class TestPydanticExtraFields(TestCase):
+    def test_pydantic_extra_fields(self):
+        """
+        Make sure that the value of ``extra`` in the config class
+        is correctly propagated to the generated model.
+        """
+
+        class Band(Table):
+            name = Varchar()
+
+        config: pydantic.config.ConfigDict = {"extra": "forbid"}
+        model = create_pydantic_model(Band, pydantic_config=config)
+
+        self.assertEqual(model.model_config["extra"], "forbid")
+
+    def test_pydantic_invalid_extra_fields(self):
+        """
+        Make sure that invalid values for ``extra`` in the config class
+        are rejected.
+        """
+
+        class Band(Table):
+            name = Varchar()
+
+        config: pydantic.config.ConfigDict = {"extra": "foobar"}
+
+        with pytest.raises(pydantic_core._pydantic_core.SchemaError):
+            create_pydantic_model(Band, pydantic_config=config)
```

### Comparing `piccolo-0.99.0/tests/utils/test_sync.py` & `piccolo-1.0a1/tests/utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.99.0/tests/utils/test_table_reflection.py` & `piccolo-1.0a1/tests/utils/test_table_reflection.py`

 * *Files identical despite different names*

