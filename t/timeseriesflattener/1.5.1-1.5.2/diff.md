# Comparing `tmp/timeseriesflattener-1.5.1.tar.gz` & `tmp/timeseriesflattener-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-1.5.1.tar", last modified: Tue Aug  1 11:16:01 2023, max compression
+gzip compressed data, was "timeseriesflattener-1.5.2.tar", last modified: Wed Aug  2 09:15:35 2023, max compression
```

## Comparing `timeseriesflattener-1.5.1.tar` & `timeseriesflattener-1.5.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.079654 timeseriesflattener-1.5.1/
--rw-r--r--   0 root         (0) root         (0)      489 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.047654 timeseriesflattener-1.5.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.043654 timeseriesflattener-1.5.1/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.047654 timeseriesflattener-1.5.1/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      892 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.047654 timeseriesflattener-1.5.1/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      948 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.051654 timeseriesflattener-1.5.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      880 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3056 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    57901 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/Makefile
--rw-r--r--   0 root         (0) root         (0)    11550 2023-08-01 11:16:01.079654 timeseriesflattener-1.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9122 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.051654 timeseriesflattener-1.5.1/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.051654 timeseriesflattener-1.5.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4173 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      332 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.055654 timeseriesflattener-1.5.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   118804 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    50220 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)   111479 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.055654 timeseriesflattener-1.5.1/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-08-01 11:15:49.000000 timeseriesflattener-1.5.1/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.055654 timeseriesflattener-1.5.1/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4307 2023-08-01 11:15:51.000000 timeseriesflattener-1.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 11:16:01.079654 timeseriesflattener-1.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.055654 timeseriesflattener-1.5.1/src/
--rw-r--r--   0 root         (0) root         (0)     1996 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.059654 timeseriesflattener-1.5.1/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      309 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/column_handler.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/df_transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.059654 timeseriesflattener-1.5.1/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.059654 timeseriesflattener-1.5.1/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     7090 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     8765 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    36395 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.059654 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3043 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.059654 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8082 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.047654 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.043654 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.059654 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1505 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.063654 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.075654 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      812 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     1392 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.075654 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.075654 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3425 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.075654 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_df_transforms.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.075654 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18309 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2688 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2328 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     8134 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/text_embedding_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.079654 timeseriesflattener-1.5.1/src/timeseriesflattener/utils/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/src/timeseriesflattener/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:16:01.059654 timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11550 2023-08-01 11:16:00.000000 timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5160 2023-08-01 11:16:01.000000 timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 11:16:00.000000 timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      696 2023-08-01 11:16:00.000000 timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-01 11:16:00.000000 timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9404 2023-08-01 11:15:50.000000 timeseriesflattener-1.5.1/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.929586 timeseriesflattener-1.5.2/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.889586 timeseriesflattener-1.5.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.881585 timeseriesflattener-1.5.2/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.889586 timeseriesflattener-1.5.2/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.889586 timeseriesflattener-1.5.2/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.889586 timeseriesflattener-1.5.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      880 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    58086 2023-08-02 09:15:23.000000 timeseriesflattener-1.5.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-08-02 09:15:35.929586 timeseriesflattener-1.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.893586 timeseriesflattener-1.5.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.893586 timeseriesflattener-1.5.2/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      332 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.897585 timeseriesflattener-1.5.2/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   118804 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50220 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)   111479 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.897585 timeseriesflattener-1.5.2/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.897585 timeseriesflattener-1.5.2/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4272 2023-08-02 09:15:23.000000 timeseriesflattener-1.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 09:15:35.929586 timeseriesflattener-1.5.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.897585 timeseriesflattener-1.5.2/src/
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.901586 timeseriesflattener-1.5.2/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/column_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.905586 timeseriesflattener-1.5.2/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.905586 timeseriesflattener-1.5.2/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     8765 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    36395 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.905586 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.905586 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.881585 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.881585 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.905586 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.909586 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.925586 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      812 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.925586 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.925586 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.929586 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.929586 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18309 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/text_embedding_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.929586 timeseriesflattener-1.5.2/src/timeseriesflattener/utils/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/src/timeseriesflattener/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 09:15:35.901586 timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-08-02 09:15:35.000000 timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5160 2023-08-02 09:15:35.000000 timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 09:15:35.000000 timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      661 2023-08-02 09:15:35.000000 timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-02 09:15:35.000000 timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9404 2023-08-02 09:15:22.000000 timeseriesflattener-1.5.2/tasks.py
```

### Comparing `timeseriesflattener-1.5.1/.cruft.json` & `timeseriesflattener-1.5.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/actions/test/action.yml` & `timeseriesflattener-1.5.2/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-1.5.2/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/dependabot.yml` & `timeseriesflattener-1.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/recommended_repo_setup.md` & `timeseriesflattener-1.5.2/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/check_for_rej.yml` & `timeseriesflattener-1.5.2/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/cruft.yml` & `timeseriesflattener-1.5.2/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-1.5.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/documentation.yml` & `timeseriesflattener-1.5.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-1.5.2/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-1.5.2/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/pre-commit.yml` & `timeseriesflattener-1.5.2/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/stalebot.yml` & `timeseriesflattener-1.5.2/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.github/workflows/static_type_checks.yml` & `timeseriesflattener-1.5.2/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.gitignore` & `timeseriesflattener-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.pre-commit-config.yaml` & `timeseriesflattener-1.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/.zenodo.json` & `timeseriesflattener-1.5.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/CHANGELOG.md` & `timeseriesflattener-1.5.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.2 (2023-08-02)
+
+### Fix
+
+* Hopeful ci docs fix ([`cd78f98`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/cd78f98287664e4116515509b18be86aade08c9e))
+
 ## v1.5.1 (2023-08-01)
 
 ### Fix
 
 * Make docs render properly ([`990020d`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/990020decc75527bff80432cfe25096ba90cbc48))
 
 ## v1.5.0 (2023-08-01)
```

### Comparing `timeseriesflattener-1.5.1/CODE_OF_CONDUCT.md` & `timeseriesflattener-1.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/CONTRIBUTING.md` & `timeseriesflattener-1.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/LICENSE` & `timeseriesflattener-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/PKG-INFO` & `timeseriesflattener-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.5.1
+Version: 1.5.2
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.5.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.5.2 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.5.1/README.md` & `timeseriesflattener-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/citation.cff` & `timeseriesflattener-1.5.2/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/Makefile` & `timeseriesflattener-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/_static/favicon.ico` & `timeseriesflattener-1.5.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/_static/icon.png` & `timeseriesflattener-1.5.2/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/_static/icon_dark.png` & `timeseriesflattener-1.5.2/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/_static/terminology_figure.png` & `timeseriesflattener-1.5.2/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/conf.py` & `timeseriesflattener-1.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/faq.rst` & `timeseriesflattener-1.5.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/index.rst` & `timeseriesflattener-1.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-1.5.2/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-1.5.2/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/tutorials/03_text.ipynb` & `timeseriesflattener-1.5.2/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/tutorials/img/term_a.png` & `timeseriesflattener-1.5.2/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/tutorials/img/term_b.png` & `timeseriesflattener-1.5.2/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/tutorials/img/term_c.png` & `timeseriesflattener-1.5.2/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/docs/tutorials/img/term_d.png` & `timeseriesflattener-1.5.2/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/icon.png` & `timeseriesflattener-1.5.2/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/paper/paper.bib` & `timeseriesflattener-1.5.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/paper/paper.md` & `timeseriesflattener-1.5.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/pyproject.toml` & `timeseriesflattener-1.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "1.5.1"
+version = "1.5.2"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
@@ -48,20 +48,20 @@
 test = [
   "pytest>=7.1.3,<7.3.0",
   "pytest-cov>=3.0.0,<3.1.0",
   "pytest-xdist>=3.0.0,<3.2.0",
   "pytest-sugar>=0.9.4,<0.10.0",
 ]
 docs = [
-    "sphinx>=5.3.0,<7.2.0",
-    "furo==2023.7.26",
-    "sphinx-copybutton>=0.5.1,<0.5.3",
-    "sphinxext-opengraph>=0.7.3,<0.8.3",
-    "myst-nb>=0.6.0,<1.17.0",
-    "sphinx_design>=0.3.0,<0.5.1",
+    "sphinx==5.3.0",
+    "furo==2023.3.27",
+    "sphinx-copybutton==0.5.2",
+    "sphinxext-opengraph==0.8.2",
+    "myst-nb==0.17.2",
+    "sphinx_design==0.3.0",
 ]
 tutorials = [
     "jupyter>=1.0.0,<1.1.0",
     "skimpy>=0.0.7,<0.1.0",
 ]
 text = [
     "transformers>=4.26.0",
```

### Comparing `timeseriesflattener-1.5.1/src/conftest.py` & `timeseriesflattener-1.5.2/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/aggregation_fns.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/df_transforms.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/feature_specs/group_specs.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/feature_specs/single_specs.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/logger.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/misc_utils.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_df_transforms.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener/utils/pydantic_basemodel.py` & `timeseriesflattener-1.5.2/src/timeseriesflattener/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.5.1
+Version: 1.5.2
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.5.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.5.2 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.5.1/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-1.5.2/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.5.1/tasks.py` & `timeseriesflattener-1.5.2/tasks.py`

 * *Files identical despite different names*

