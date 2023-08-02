# Comparing `tmp/glean_parser-8.1.0.tar.gz` & `tmp/glean_parser-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/glean_parser-8.1.0.tar", last modified: Mon Jul 31 15:50:21 2023, max compression
+gzip compressed data, was "dist/glean_parser-8.1.1.tar", last modified: Wed Aug  2 10:14:29 2023, max compression
```

## Comparing `glean_parser-8.1.0.tar` & `glean_parser-8.1.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6784 2023-07-31 15:50:00.000000 glean_parser-8.1.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-07-31 15:50:00.000000 glean_parser-8.1.0/.editorconfig
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/.github/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-07-31 15:50:00.000000 glean_parser-8.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-07-31 15:50:00.000000 glean_parser-8.1.0/.github/dependabot.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-07-31 15:50:00.000000 glean_parser-8.1.0/.github/pull_request_template.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-07-31 15:50:00.000000 glean_parser-8.1.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-07-31 15:50:00.000000 glean_parser-8.1.0/.swiftlint.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-07-31 15:50:00.000000 glean_parser-8.1.0/AUTHORS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25527 2023-07-31 15:50:00.000000 glean_parser-8.1.0/CHANGELOG.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-07-31 15:50:00.000000 glean_parser-8.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-07-31 15:50:00.000000 glean_parser-8.1.0/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-07-31 15:50:00.000000 glean_parser-8.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-07-31 15:50:00.000000 glean_parser-8.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-07-31 15:50:00.000000 glean_parser-8.1.0/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28673 2023-07-31 15:50:21.000000 glean_parser-8.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-07-31 15:50:00.000000 glean_parser-8.1.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/Makefile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/docs/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/_static/glean.jpeg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/authors.md
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/contributing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25527 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/history.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/installation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/metrics-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/pings-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/readme.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-31 15:50:00.000000 glean_parser-8.1.0/docs/tags-yaml.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/coverage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/data_review.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6004 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/javascript_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18248 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12431 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/rust.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser/schemas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/schemas/metrics.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25849 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/schemas/metrics.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/schemas/pings.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4363 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/schemas/pings.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/schemas/tags.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/tags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/data_review.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/javascript.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/javascript.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5246 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/javascript_server.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/kotlin.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/kotlin.geckoview.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/kotlin.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/markdown.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/qmldir.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3600 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/rust.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4809 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/templates/swift.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8148 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/translate.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/translation_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16825 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-07-31 15:50:00.000000 glean_parser-8.1.0/glean_parser/validate_ping.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28673 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3278 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-31 15:50:21.000000 glean_parser-8.1.0/glean_parser.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-31 15:50:00.000000 glean_parser-8.1.0/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-07-31 15:50:00.000000 glean_parser-8.1.0/requirements_dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-07-31 15:50:21.000000 glean_parser-8.1.0/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2286 2023-07-31 15:50:00.000000 glean_parser-8.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/all_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/all_pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/bad_ping.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/core.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/duplicate_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/duplicate_send_in_ping.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/empty.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/event_key_ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/events_with_types.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/fxa-server-metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/fxa-server-pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/gecko.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/invalid-ping-names.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/invalid.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/jwe.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/metric-with-tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/mixed-expirations.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/old_event_api.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/rate.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2577 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/schema-violation.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/send_if_empty_with_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/single_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/smaller.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/telemetry_mirror.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/text.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/text_invalid.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/unknown_ping_used.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/wrong_key.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/data/yaml_nits.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/detekt.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_javascript_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13673 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32166 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_rust.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_translate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/test_validate_ping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tests/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:50:21.000000 glean_parser-8.1.0/tools/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4715 2023-07-31 15:50:00.000000 glean_parser-8.1.0/tools/extract_data_categories.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6784 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.editorconfig
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/.github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.github/dependabot.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.github/pull_request_template.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.swiftlint.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-08-02 10:14:13.000000 glean_parser-8.1.1/AUTHORS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25674 2023-08-02 10:14:13.000000 glean_parser-8.1.1/CHANGELOG.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-08-02 10:14:13.000000 glean_parser-8.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-08-02 10:14:13.000000 glean_parser-8.1.1/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-08-02 10:14:13.000000 glean_parser-8.1.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-08-02 10:14:13.000000 glean_parser-8.1.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-08-02 10:14:13.000000 glean_parser-8.1.1/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28820 2023-08-02 10:14:29.000000 glean_parser-8.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-08-02 10:14:13.000000 glean_parser-8.1.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/Makefile
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/docs/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/_static/glean.jpeg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/authors.md
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/contributing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25674 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/history.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/installation.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/metrics-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/pings-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/readme.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/tags-yaml.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/coverage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/data_review.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6004 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/javascript_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18248 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12431 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/rust.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser/schemas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/metrics.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25849 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/metrics.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/pings.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4363 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/pings.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/tags.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/tags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/data_review.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/javascript.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/javascript.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5368 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/javascript_server.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/kotlin.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/kotlin.geckoview.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/kotlin.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/markdown.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/qmldir.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3600 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/rust.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4809 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/swift.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8148 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/translate.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/translation_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16825 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/validate_ping.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28820 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3278 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-02 10:14:13.000000 glean_parser-8.1.1/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-08-02 10:14:13.000000 glean_parser-8.1.1/requirements_dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-08-02 10:14:29.000000 glean_parser-8.1.1/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2286 2023-08-02 10:14:13.000000 glean_parser-8.1.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/all_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/all_pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/bad_ping.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/core.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/duplicate_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/duplicate_send_in_ping.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/empty.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/event_key_ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/events_with_types.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/fxa-server-metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/fxa-server-pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/gecko.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/invalid-ping-names.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/invalid.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/jwe.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/metric-with-tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/mixed-expirations.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/old_event_api.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/rate.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2577 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/schema-violation.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/send_if_empty_with_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/single_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/smaller.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/telemetry_mirror.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/text.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/text_invalid.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/unknown_ping_used.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/wrong_key.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/yaml_nits.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/detekt.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_javascript_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13673 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32166 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_rust.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_translate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_validate_ping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/tools/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4715 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tools/extract_data_categories.py
```

### Comparing `glean_parser-8.1.0/.circleci/config.yml` & `glean_parser-8.1.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/.github/pull_request_template.md` & `glean_parser-8.1.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/.gitignore` & `glean_parser-8.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/CHANGELOG.md` & `glean_parser-8.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## Unreleased
 
+## 8.1.1
+
+- Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
+
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
 
 ## 8.0.0
 
 - BREAKING CHANGE: Remove exposed `lint_yaml_files` function ([#580](https://github.com/mozilla/glean_parser/pull/580))
```

### Comparing `glean_parser-8.1.0/CODE_OF_CONDUCT.md` & `glean_parser-8.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/CONTRIBUTING.md` & `glean_parser-8.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/LICENSE` & `glean_parser-8.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/Makefile` & `glean_parser-8.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/PKG-INFO` & `glean_parser-8.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean_parser
-Version: 8.1.0
+Version: 8.1.1
 Summary: Parser tools for Mozilla's Glean telemetry
 Home-page: https://github.com/mozilla/glean_parser
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 Keywords: glean_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -74,14 +74,18 @@
 ```
 
 
 # Changelog
 
 ## Unreleased
 
+## 8.1.1
+
+- Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
+
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
 
 ## 8.0.0
 
 - BREAKING CHANGE: Remove exposed `lint_yaml_files` function ([#580](https://github.com/mozilla/glean_parser/pull/580))
```

### Comparing `glean_parser-8.1.0/README.md` & `glean_parser-8.1.1/README.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/docs/Makefile` & `glean_parser-8.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/docs/_static/glean.jpeg` & `glean_parser-8.1.1/docs/_static/glean.jpeg`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/docs/conf.py` & `glean_parser-8.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/docs/contributing.md` & `glean_parser-8.1.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/docs/history.md` & `glean_parser-8.1.1/docs/history.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## Unreleased
 
+## 8.1.1
+
+- Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
+
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
 
 ## 8.0.0
 
 - BREAKING CHANGE: Remove exposed `lint_yaml_files` function ([#580](https://github.com/mozilla/glean_parser/pull/580))
```

### Comparing `glean_parser-8.1.0/docs/installation.md` & `glean_parser-8.1.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/docs/make.bat` & `glean_parser-8.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/docs/readme.md` & `glean_parser-8.1.1/docs/readme.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/__init__.py` & `glean_parser-8.1.1/glean_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/__main__.py` & `glean_parser-8.1.1/glean_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/coverage.py` & `glean_parser-8.1.1/glean_parser/coverage.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/data_review.py` & `glean_parser-8.1.1/glean_parser/data_review.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/javascript.py` & `glean_parser-8.1.1/glean_parser/javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/javascript_server.py` & `glean_parser-8.1.1/glean_parser/javascript_server.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/kotlin.py` & `glean_parser-8.1.1/glean_parser/kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/lint.py` & `glean_parser-8.1.1/glean_parser/lint.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/markdown.py` & `glean_parser-8.1.1/glean_parser/markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/metrics.py` & `glean_parser-8.1.1/glean_parser/metrics.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/parser.py` & `glean_parser-8.1.1/glean_parser/parser.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/pings.py` & `glean_parser-8.1.1/glean_parser/pings.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/rust.py` & `glean_parser-8.1.1/glean_parser/rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/schemas/metrics.1-0-0.schema.yaml` & `glean_parser-8.1.1/glean_parser/schemas/metrics.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/schemas/metrics.2-0-0.schema.yaml` & `glean_parser-8.1.1/glean_parser/schemas/metrics.2-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/schemas/pings.1-0-0.schema.yaml` & `glean_parser-8.1.1/glean_parser/schemas/pings.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/schemas/pings.2-0-0.schema.yaml` & `glean_parser-8.1.1/glean_parser/schemas/pings.2-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/schemas/tags.1-0-0.schema.yaml` & `glean_parser-8.1.1/glean_parser/schemas/tags.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/swift.py` & `glean_parser-8.1.1/glean_parser/swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/tags.py` & `glean_parser-8.1.1/glean_parser/tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/data_review.jinja2` & `glean_parser-8.1.1/glean_parser/templates/data_review.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/javascript.jinja2` & `glean_parser-8.1.1/glean_parser/templates/javascript.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/javascript_server.jinja2` & `glean_parser-8.1.1/glean_parser/templates/javascript_server.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 // @types/uuid and mozlog types definitions are required in devDependencies
 // for the latter see https://github.com/mozilla/fxa/blob/85bda71cda376c417b8c850ba82aa14252208c3c/types/mozlog/index.d.ts
 {% endif %}
 import { v4 as uuidv4 } from 'uuid';
 import mozlog{% if lang == "typescript" %}, { Logger }{% endif %} from 'mozlog';
 
 const GLEAN_EVENT_MOZLOG_TYPE = 'glean-server-event';
+{% if lang == "typescript" %}
+type LoggerOptions = { app: string; fmt?: 'heka' };
+{% endif %}
 
 let _logger{% if lang == "typescript" %}: Logger{% endif %};
 
 {% for ping, metrics_by_type in pings.items() %}
 class {{ ping|event_class_name }} {
   {% if lang == "typescript" %}
   _applicationId: string;
@@ -33,15 +36,15 @@
    * @param {string} channel - The channel.
    */
   {% if lang == "typescript" %}
   constructor(
     applicationId: string,
     appDisplayVersion: string,
     channel: string,
-    logger_options: any
+    logger_options: LoggerOptions
   ) {
   {% else %}
   constructor(applicationId, appDisplayVersion, channel, logger_options) {
   {% endif %}
     this._applicationId = applicationId;
     this._appDisplayVersion = appDisplayVersion;
     this._channel = channel;
@@ -81,16 +84,16 @@
     {% for metric_type, metrics in metrics_by_type.items() %}
     {% for metric in metrics %}
     {{ metric|metric_argument_name }}: {{ metric|js_metric_type }};
     {% endfor %}
     {% endfor %}
   {% endif %}
   }) {
-    let timestamp = new Date().toISOString();
-    let eventPayload = {
+    const timestamp = new Date().toISOString();
+    const eventPayload = {
       metrics: {
         {% for metric_type, metrics in metrics_by_type.items() %}
         {{ metric_type }}: {
           {% for metric in metrics %}
           '{{ metric|metric_name }}': {{ metric|metric_argument_name }},
           {% endfor %}
         },
@@ -109,18 +112,18 @@
         os_version: 'Unknown',
         architecture: 'Unknown',
         app_build: 'Unknown',
         app_display_version: this._appDisplayVersion,
         app_channel: this._channel,
       },
     };
-    let eventPayloadSerialized = JSON.stringify(eventPayload);
+    const eventPayloadSerialized = JSON.stringify(eventPayload);
 
     // This is the message structure that Decoder expects: https://github.com/mozilla/gcp-ingestion/pull/2400
-    let ping = {
+    const ping = {
       document_namespace: this._applicationId,
       document_type: '{{ ping }}',
       document_version: '1',
       document_id: uuidv4(),
       payload: eventPayloadSerialized,
     };
 
@@ -137,15 +140,15 @@
   channel,
   logger_options
 {% if lang == "typescript" %}
 }: {
   applicationId: string;
   appDisplayVersion: string;
   channel: string;
-  logger_options: any;
+  logger_options: LoggerOptions;
 {% endif %}
 }) {
   return new {{ ping|event_class_name }}(
     applicationId,
     appDisplayVersion,
     channel,
     logger_options
```

### Comparing `glean_parser-8.1.0/glean_parser/templates/kotlin.buildinfo.jinja2` & `glean_parser-8.1.1/glean_parser/templates/kotlin.buildinfo.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/kotlin.geckoview.jinja2` & `glean_parser-8.1.1/glean_parser/templates/kotlin.geckoview.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/kotlin.jinja2` & `glean_parser-8.1.1/glean_parser/templates/kotlin.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/markdown.jinja2` & `glean_parser-8.1.1/glean_parser/templates/markdown.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/rust.jinja2` & `glean_parser-8.1.1/glean_parser/templates/rust.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/templates/swift.jinja2` & `glean_parser-8.1.1/glean_parser/templates/swift.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/translate.py` & `glean_parser-8.1.1/glean_parser/translate.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/translation_options.py` & `glean_parser-8.1.1/glean_parser/translation_options.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/util.py` & `glean_parser-8.1.1/glean_parser/util.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser/validate_ping.py` & `glean_parser-8.1.1/glean_parser/validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/glean_parser.egg-info/PKG-INFO` & `glean_parser-8.1.1/glean_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-parser
-Version: 8.1.0
+Version: 8.1.1
 Summary: Parser tools for Mozilla's Glean telemetry
 Home-page: https://github.com/mozilla/glean_parser
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 Keywords: glean_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -74,14 +74,18 @@
 ```
 
 
 # Changelog
 
 ## Unreleased
 
+## 8.1.1
+
+- Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
+
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
 
 ## 8.0.0
 
 - BREAKING CHANGE: Remove exposed `lint_yaml_files` function ([#580](https://github.com/mozilla/glean_parser/pull/580))
```

### Comparing `glean_parser-8.1.0/glean_parser.egg-info/SOURCES.txt` & `glean_parser-8.1.1/glean_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/setup.py` & `glean_parser-8.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/all_metrics.yaml` & `glean_parser-8.1.1/tests/data/all_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/all_pings.yaml` & `glean_parser-8.1.1/tests/data/all_pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/bad_ping.yamlx` & `glean_parser-8.1.1/tests/data/bad_ping.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/core.yaml` & `glean_parser-8.1.1/tests/data/core.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/duplicate_labeled.yaml` & `glean_parser-8.1.1/tests/data/duplicate_labeled.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/duplicate_send_in_ping.yaml` & `glean_parser-8.1.1/tests/data/duplicate_send_in_ping.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/event_key_ordering.yaml` & `glean_parser-8.1.1/tests/data/event_key_ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/events_with_types.yaml` & `glean_parser-8.1.1/tests/data/events_with_types.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/gecko.yaml` & `glean_parser-8.1.1/tests/data/gecko.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/invalid-ping-names.yaml` & `glean_parser-8.1.1/tests/data/invalid-ping-names.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/metric-with-tags.yaml` & `glean_parser-8.1.1/tests/data/metric-with-tags.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/mixed-expirations.yaml` & `glean_parser-8.1.1/tests/data/mixed-expirations.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/old_event_api.yamlx` & `glean_parser-8.1.1/tests/data/old_event_api.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/ordering.yaml` & `glean_parser-8.1.1/tests/data/ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/pings.yaml` & `glean_parser-8.1.1/tests/data/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/rate.yaml` & `glean_parser-8.1.1/tests/data/rate.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/schema-violation.yaml` & `glean_parser-8.1.1/tests/data/schema-violation.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/send_if_empty_with_metrics.yaml` & `glean_parser-8.1.1/tests/data/send_if_empty_with_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/smaller.yaml` & `glean_parser-8.1.1/tests/data/smaller.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/telemetry_mirror.yaml` & `glean_parser-8.1.1/tests/data/telemetry_mirror.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/text.yaml` & `glean_parser-8.1.1/tests/data/text.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/text_invalid.yaml` & `glean_parser-8.1.1/tests/data/text_invalid.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/unknown_ping_used.yaml` & `glean_parser-8.1.1/tests/data/unknown_ping_used.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/wrong_key.yamlx` & `glean_parser-8.1.1/tests/data/wrong_key.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/data/yaml_nits.yamlx` & `glean_parser-8.1.1/tests/data/yaml_nits.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_cli.py` & `glean_parser-8.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_javascript.py` & `glean_parser-8.1.1/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_javascript_server.py` & `glean_parser-8.1.1/tests/test_javascript_server.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_kotlin.py` & `glean_parser-8.1.1/tests/test_kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_lint.py` & `glean_parser-8.1.1/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_markdown.py` & `glean_parser-8.1.1/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_metrics.py` & `glean_parser-8.1.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_parser.py` & `glean_parser-8.1.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_pings.py` & `glean_parser-8.1.1/tests/test_pings.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_rust.py` & `glean_parser-8.1.1/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_swift.py` & `glean_parser-8.1.1/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_tags.py` & `glean_parser-8.1.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_translate.py` & `glean_parser-8.1.1/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_utils.py` & `glean_parser-8.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/test_validate_ping.py` & `glean_parser-8.1.1/tests/test_validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tests/util.py` & `glean_parser-8.1.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.0/tools/extract_data_categories.py` & `glean_parser-8.1.1/tools/extract_data_categories.py`

 * *Files identical despite different names*

