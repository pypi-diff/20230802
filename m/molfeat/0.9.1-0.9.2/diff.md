# Comparing `tmp/molfeat-0.9.1.tar.gz` & `tmp/molfeat-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.9.1.tar", last modified: Thu Jul 27 20:47:45 2023, max compression
+gzip compressed data, was "molfeat-0.9.2.tar", last modified: Wed Aug  2 21:06:34 2023, max compression
```

## Comparing `molfeat-0.9.1.tar` & `molfeat-0.9.2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.907130 molfeat-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.879130 molfeat-0.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.883130 molfeat-0.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/5_community_contribution.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.883130 molfeat-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-27 20:43:14.000000 molfeat-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-27 20:43:14.000000 molfeat-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-07-27 20:43:14.000000 molfeat-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-27 20:47:45.907130 molfeat-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-27 20:43:14.000000 molfeat-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.883130 molfeat-0.9.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.875130 molfeat-0.9.1/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)   110397 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/community/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/community/contributions.md
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/community/get_involved.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.891130 molfeat-0.9.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/custom_model_store.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60168 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-27 20:43:14.000000 molfeat-0.9.1/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-27 20:43:14.000000 molfeat-0.9.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.891130 molfeat-0.9.1/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.895130 molfeat-0.9.1/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.895130 molfeat-0.9.1/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33979 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.903130 molfeat-0.9.1/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.891130 molfeat-0.9.1/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:47:38.000000 molfeat-0.9.1/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.879130 molfeat-0.9.1/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.903130 molfeat-0.9.1/nb/etl/
--rw-r--r--   0 runner    (1001) docker     (123)    29350 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/chemberta-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/chemgpt-fix-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/dgl-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/entropy-transforner-zinc-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/featurizer-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/molt5-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 20:43:14.000000 molfeat-0.9.1/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-27 20:43:14.000000 molfeat-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:47:45.907130 molfeat-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.907130 molfeat-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.723981 molfeat-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.707981 molfeat-0.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.707981 molfeat-0.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/ISSUE_TEMPLATE/5_community_contribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.707981 molfeat-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-02 21:02:56.000000 molfeat-0.9.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-02 21:02:56.000000 molfeat-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-02 21:02:56.000000 molfeat-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-08-02 21:02:56.000000 molfeat-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-08-02 21:06:34.723981 molfeat-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-08-02 21:02:56.000000 molfeat-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.707981 molfeat-0.9.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.711981 molfeat-0.9.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.pretrained.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.703981 molfeat-0.9.2/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.711981 molfeat-0.9.2/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.711981 molfeat-0.9.2/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.711981 molfeat-0.9.2/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/community/contributions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/community/get_involved.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.711981 molfeat-0.9.2/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.711981 molfeat-0.9.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.715981 molfeat-0.9.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/custom_model_store.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60168 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-08-02 21:02:56.000000 molfeat-0.9.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 21:02:56.000000 molfeat-0.9.2/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-02 21:02:56.000000 molfeat-0.9.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.715981 molfeat-0.9.2/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.715981 molfeat-0.9.2/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.715981 molfeat-0.9.2/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.719981 molfeat-0.9.2/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.719981 molfeat-0.9.2/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.719981 molfeat-0.9.2/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33867 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.719981 molfeat-0.9.2/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.719981 molfeat-0.9.2/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.719981 molfeat-0.9.2/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.719981 molfeat-0.9.2/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-08-02 21:02:56.000000 molfeat-0.9.2/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.715981 molfeat-0.9.2/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-08-02 21:06:34.000000 molfeat-0.9.2/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-08-02 21:06:34.000000 molfeat-0.9.2/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:06:34.000000 molfeat-0.9.2/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:06:29.000000 molfeat-0.9.2/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 21:06:34.000000 molfeat-0.9.2/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 21:06:34.000000 molfeat-0.9.2/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.707981 molfeat-0.9.2/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.723981 molfeat-0.9.2/nb/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)    29350 2023-08-02 21:02:56.000000 molfeat-0.9.2/nb/etl/chemberta-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-08-02 21:02:56.000000 molfeat-0.9.2/nb/etl/chemgpt-fix-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-08-02 21:02:56.000000 molfeat-0.9.2/nb/etl/dgl-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-08-02 21:02:56.000000 molfeat-0.9.2/nb/etl/entropy-transforner-zinc-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-08-02 21:02:56.000000 molfeat-0.9.2/nb/etl/featurizer-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-02 21:02:56.000000 molfeat-0.9.2/nb/etl/molt5-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-02 21:02:56.000000 molfeat-0.9.2/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-02 21:02:56.000000 molfeat-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:06:34.723981 molfeat-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:06:34.723981 molfeat-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 21:02:56.000000 molfeat-0.9.2/tests/test_viz.py
```

### Comparing `molfeat-0.9.1/.github/CODE_OF_CONDUCT.md` & `molfeat-0.9.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.9.2/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.9.2/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.9.2/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.9.2/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/ISSUE_TEMPLATE/5_community_contribution.yaml` & `molfeat-0.9.2/.github/ISSUE_TEMPLATE/5_community_contribution.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.9.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/PULL_REQUEST_TEMPLATE.md` & `molfeat-0.9.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/workflows/doc.yml` & `molfeat-0.9.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/workflows/release.yml` & `molfeat-0.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.github/workflows/test.yml` & `molfeat-0.9.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/.gitignore` & `molfeat-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/CHANGELOG.md` & `molfeat-0.9.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/LICENSE` & `molfeat-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/PKG-INFO` & `molfeat-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.9.1
+Version: 0.9.2
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -27,14 +27,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dgl
 Provides-Extra: graphormer
 Provides-Extra: transformer
 Provides-Extra: fcd
 Provides-Extra: viz
 Provides-Extra: all
+Provides-Extra: test
+Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
     <img src="docs/images/logo-title.svg" width="100%">
 </div>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.9.1 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.9.2 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -13,15 +13,16 @@
 Science Apps. Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dgl Provides-Extra: graphormer
 Provides-Extra: transformer Provides-Extra: fcd Provides-Extra: viz Provides-
-Extra: all License-File: LICENSE
+Extra: all Provides-Extra: test Provides-Extra: docs Provides-Extra: dev
+License-File: LICENSE
                          [docs/images/logo-title.svg]
              molfeat - the hub for all your molecular featurizers
                                 Docs | Homepage
 --- [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/
 latestdoi/613548667) [![PyPI](https://img.shields.io/pypi/v/molfeat)](https://
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/v/conda-
 forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/
```

### Comparing `molfeat-0.9.1/README.md` & `molfeat-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/api/molfeat.calc.md` & `molfeat-0.9.2/docs/api/molfeat.calc.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/assets/css/custom-molfeat.css` & `molfeat-0.9.2/docs/assets/css/custom-molfeat.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/assets/css/custom.css` & `molfeat-0.9.2/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/community/contributions.md` & `molfeat-0.9.2/docs/community/contributions.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/community/get_involved.md` & `molfeat-0.9.2/docs/community/get_involved.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/developers/create-plugin.md` & `molfeat-0.9.2/docs/developers/create-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/developers/register-plugin.md` & `molfeat-0.9.2/docs/developers/register-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/images/logo-black.png` & `molfeat-0.9.2/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/images/logo-black.svg` & `molfeat-0.9.2/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/images/logo-title.svg` & `molfeat-0.9.2/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/images/logo.png` & `molfeat-0.9.2/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/images/logo.svg` & `molfeat-0.9.2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/index.md` & `molfeat-0.9.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/add_your_own.ipynb` & `molfeat-0.9.2/docs/tutorials/add_your_own.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/custom_model_store.ipynb` & `molfeat-0.9.2/docs/tutorials/custom_model_store.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/datacache.ipynb` & `molfeat-0.9.2/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/graphs.ipynb` & `molfeat-0.9.2/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/integrations.ipynb` & `molfeat-0.9.2/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.9.2/docs/tutorials/pyg_integration.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/save_and_load.ipynb` & `molfeat-0.9.2/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.9.2/docs/tutorials/transformer_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.9.2/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/docs/usage.md` & `molfeat-0.9.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/env.yml` & `molfeat-0.9.2/env.yml`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
   - matplotlib
   - pydantic >=2.0.0
 
   # Chemistry
   - datamol >=0.8.0
   - rdkit >=2021.09
   - pmapper
+  - mordredcommunity
 
   # ML
   - pytorch =1.12
   - scikit-learn
   - fcd_torch
 
   # Optional: featurizers
@@ -52,14 +53,15 @@
   # Dev
   - pytest >=6.0
   - pytest-dotenv
   - pytest-cov
   - pytest-timeout
   - pytest-xdist
   - black >=22
+  - ruff
   - jupyterlab
   - nbconvert
 
   # Doc
   - mkdocs
   - mkdocs-material >=7.1.1
   - mkdocs-material-extensions
```

### Comparing `molfeat-0.9.1/mkdocs.yml` & `molfeat-0.9.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/__init__.py` & `molfeat-0.9.2/molfeat/calc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .base import SerializableCalculator, _CALCULATORS
 from .cats import CATS
-from .descriptors import RDKitDescriptors2D, RDKitDescriptors3D
+from .descriptors import RDKitDescriptors2D, RDKitDescriptors3D, MordredDescriptors
 from .fingerprints import FPCalculator, FP_FUNCS
 from .pharmacophore import Pharmacophore2D, Pharmacophore3D
 from .shape import ElectroShapeDescriptors, USRDescriptors
 from .skeys import ScaffoldKeyCalculator
 
 
 def get_calculator(name: str, **params):
@@ -27,14 +27,16 @@
     name = name.lower()
     if name in FP_FUNCS.keys():
         featurizer = FPCalculator(name, **params)
     elif name == "desc3d":
         featurizer = RDKitDescriptors3D(**params)
     elif name == "desc2d":
         featurizer = RDKitDescriptors2D(**params)
+    elif name == "mordred":
+        featurizer = MordredDescriptors(**params)
     elif name == "cats":
         featurizer = CATS(**params)
     elif name == "cats2d":
         params["use_3d_distances"] = False
         featurizer = CATS(**params)
     elif name == "cats3d":
         params["use_3d_distances"] = True
```

### Comparing `molfeat-0.9.1/molfeat/calc/_atom_bond_features.py` & `molfeat-0.9.2/molfeat/calc/_atom_bond_features.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/_map4.py` & `molfeat-0.9.2/molfeat/calc/_map4.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/_mhfp.py` & `molfeat-0.9.2/molfeat/calc/_mhfp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/atom.py` & `molfeat-0.9.2/molfeat/calc/atom.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/base.py` & `molfeat-0.9.2/molfeat/calc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import abc
 import importlib
 import inspect
 import json
 import joblib
 import yaml
 import fsspec
-import importlib
 from loguru import logger
 from molfeat._version import __version__ as MOLFEAT_VERSION
 
 
 _CALCULATORS = {}
```

### Comparing `molfeat-0.9.1/molfeat/calc/bond.py` & `molfeat-0.9.2/molfeat/calc/bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from molfeat.calc.base import SerializableCalculator
 from molfeat.calc._atom_bond_features import bond_type_one_hot
 from molfeat.calc._atom_bond_features import bond_is_conjugated
 from molfeat.calc._atom_bond_features import bond_is_in_ring
 from molfeat.calc._atom_bond_features import bond_direction_one_hot
 from molfeat.calc._atom_bond_features import bond_stereo_one_hot
 from molfeat.calc._atom_bond_features import pairwise_ring_membership
-from molfeat.calc._atom_bond_features import pairwise_3D_dist
 from molfeat.calc._atom_bond_features import pairwise_2D_dist
 from molfeat.calc._atom_bond_features import pairwise_bond_indicator
 from molfeat.calc._atom_bond_features import pairwise_dist_indicator
 from molfeat.utils import datatype
 from molfeat.utils.commons import concat_dict
 from molfeat.utils.commons import hex_to_fn
 from molfeat.utils.commons import fn_to_hex
```

### Comparing `molfeat-0.9.1/molfeat/calc/cats.py` & `molfeat-0.9.2/molfeat/calc/cats.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/descriptors.py` & `molfeat-0.9.2/molfeat/calc/descriptors.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,23 @@
     Descriptors3D,
     FindMolChiralCenters,
     rdMolDescriptors,
     rdPartialCharges,
 )
 from rdkit.Chem.QED import properties
 
+from molfeat.utils import requires
+
+if requires.check("mordred"):
+    from mordred import Calculator as MordredCalculator
+    from mordred import descriptors as mordred_descriptors
+
+else:
+    MordredCalculator = requires.mock("mordred")
+
 from molfeat.calc.base import SerializableCalculator
 from molfeat.utils.commons import requires_conformer, requires_standardization
 from molfeat.utils.datatype import to_numpy
 
 
 def _charge_descriptors_computation(mol: dm.Mol):
     """Recompute properly the RDKIT 2D Descriptors related to charge
@@ -42,43 +51,54 @@
     return descrs
 
 
 class RDKitDescriptors2D(SerializableCalculator):
     r"""
     Compute a list of available  rdkit 2D descriptors for a molecule.
     The descriptor calculator does not mask errors in featurization and will propagate them
+
+    !!! note
+        Due to recent RDKit changes, this calculator could hang for a while for large molecules (>900).
+        The main culprit is the `Ipc` descriptor which requires some computation on the full adjacency matrix.
+        You may also consider using `ignore_descrs=['AvgIpc', 'Ipc']` as a workaround when you have large molecules.
+        Alternatively, You may wish to use an alternative featurizer
+
     """
 
     DESCRIPTORS_FN = {name: fn for (name, fn) in Descriptors.descList}
 
     def __init__(
         self,
         replace_nan: Optional[bool] = False,
         augment: Optional[bool] = True,
         descrs: List = None,
         avg_ipc: Optional[bool] = True,
         do_not_standardize: Optional[bool] = False,
+        ignore_descrs: Optional[List] = None,
         **kwargs,
     ):
         """RDKit descriptor computation
 
         Args:
             replace_nan: Whether to replace nan or infinite values. Defaults to False.
             augment: Whether to augment the descriptors with some additional custom features
             descrs: Subset of available features to consider if not None
             avg_ipc: Whether to average IPC values or to use rdkit original
+            ignore_descrs: optional list of descriptors to ignore. You can get the full list of default descriptors
+                by calling `calculator.columns`.
             do_not_standardize: Whether to force standardization of molecule before computation of the descriptor.
                 Set to True if you want molfeat<=0.5.3 behaviour
         """
         self.replace_nan = replace_nan
         self.augment = augment
         self.descrs = descrs
         self.avg_ipc = avg_ipc
         self.do_not_standardize = do_not_standardize
         all_features = [d[0] for d in Descriptors.descList]
+        self.ignore_descrs = ignore_descrs or []
         if self.augment:
             all_features += [
                 "NumAtomStereoCenters",
                 "NumUnspecifiedAtomStereoCenters",
                 "NumBridgeheadAtoms",
                 "NumAmideBonds",
                 "NumSpiroAtoms",
@@ -88,14 +108,16 @@
             self._columns = [x for x in descrs if x in all_features]
             unknown_descrs = set(descrs) - set(all_features)
             if len(unknown_descrs) > 0:
                 logger.warning(f"Following features are not supported: {unknown_descrs}")
         else:
             self._columns = all_features
 
+        self._columns = [x for x in self._columns if x not in self.ignore_descrs]
+
     def __getstate__(self):
         """Serialize the class for pickling."""
         state = {}
         state["replace_nan"] = self.replace_nan
         state["augment"] = self.augment
         state["descrs"] = self.descrs
         state["_columns"] = self._columns
@@ -253,23 +275,102 @@
         mol = dm.to_mol(mol)
         desc_val = []
         for desc in self._descr:
             val = float("nan")
             if desc not in self.ignore_descrs:
                 try:
                     val = getattr(Descriptors3D.rdMolDescriptors, desc)(mol, confId=conformer_id)
-                except:
+                except Exception:
                     pass
                 desc_val.append(val)
         for i, desc in enumerate(self._vec_descr):
             val = [float("nan")] * self._vec_descr_length[i]
             if desc not in self.ignore_descrs:
                 try:
                     val = getattr(Descriptors3D.rdMolDescriptors, desc)(mol, confId=conformer_id)
-                except:
+                except Exception:
                     pass
                 desc_val.extend(val)
 
         desc_val = to_numpy(desc_val)
         if self.replace_nan:
             desc_val = np.nan_to_num(desc_val)
         return desc_val
+
+
+class MordredDescriptors(SerializableCalculator):
+    r"""
+    Compute mordred descriptors.
+    The descriptor calculator does not mask errors in featurization and will propagate them.
+    !!! note
+        Mordred descriptors can results in undefined or nan behaviour depending on your input molecule.
+        It is recommended that the user handles those nan values themself by either removing the descriptor
+        or imputing the missing values.
+    """
+
+    def __init__(
+        self,
+        ignore_3D: bool = True,
+        replace_nan: bool = False,
+        do_not_standardize: bool = False,
+        **kwargs,
+    ):
+        """Mordred descriptor computation
+        Args:
+            ignore_3D (bool, optional): Whether to ignore 3D descriptors or include them
+            replace_nan (bool, optional): Whether to replace nan or infinite values. Defaults to False.
+            do_not_standardize: Whether to force standardize molecules or keep it the same
+        """
+        if not requires.check("mordred"):
+            logger.error(
+                "`mordred` is not available, please install it `pip install 'mordred[full]'`"
+            )
+            raise ImportError("Cannot import `mordred`")
+        self.replace_nan = replace_nan
+        self.ignore_3D = ignore_3D
+        self.do_not_standardize = do_not_standardize
+        self._calc = None
+        self._init_calc()
+
+    def _init_calc(self):
+        """Initialize mordred calculator"""
+        self._calc = MordredCalculator(mordred_descriptors, ignore_3D=self.ignore_3D)
+
+    @property
+    def columns(self):
+        """
+        Get the name of all the descriptors of this calculator
+        """
+        return [str(x) for x in self._calc.descriptors]
+
+    def __len__(self):
+        """Return the length of the calculator"""
+        return len(self._calc)
+
+    def __getstate__(self):
+        """Serialize the class for pickling."""
+        state = {}
+        state["ignore_3D"] = self.ignore_3D
+        state["replace_nan"] = self.replace_nan
+        state["do_not_standardize"] = getattr(self, "do_not_standardize", False)
+        return state
+
+    def __setstate__(self, state: dict):
+        """Reload the class from pickling."""
+        self.__dict__.update(state)
+        self._init_calc()
+
+    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1):
+        r"""
+        Get rdkit basic descriptors for a molecule
+        Args:
+            mol: the molecule of interest
+            conformer_id (int, optional): Optional
+        Returns:
+            props (np.ndarray): list of computed mordred molecular descriptors
+        """
+        mol = dm.to_mol(mol)
+        vals = self._calc(mol, conformer_id).fill_missing()
+        vals = to_numpy(vals)
+        if self.replace_nan:
+            vals = np.nan_to_num(vals)
+        return vals
```

### Comparing `molfeat-0.9.1/molfeat/calc/fingerprints.py` & `molfeat-0.9.2/molfeat/calc/fingerprints.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                 The default corresponds to the fingerpint default.
             counting (bool, optional): Whether to use the count version of the fingerprint
             method_params (dict): any parameters to the fingerprint algorithm.
                 See FPCalculator.default_parameters(method) for all the parameters required by a given method.
         """
         self.method = method.lower()
         self.counting = counting or "-count" in self.method
-        if self.counting and not "-count" in self.method:
+        if self.counting and "-count" not in self.method:
             self.method = self.method + "-count"
         self.input_length = length
         if self.method not in FP_FUNCS:
             raise ValueError(f"Method {self.method} is not a supported featurizer")
         default_params = copy.deepcopy(FP_DEF_PARAMS[method])
         unknown_params = set(method_params.keys()).difference(set(default_params.keys()))
         if unknown_params:
```

### Comparing `molfeat-0.9.1/molfeat/calc/pharmacophore.py` & `molfeat-0.9.2/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/shape.py` & `molfeat-0.9.2/molfeat/calc/shape.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/skeys.py` & `molfeat-0.9.2/molfeat/calc/skeys.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/calc/tree.py` & `molfeat-0.9.2/molfeat/calc/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from typing import Iterable
 from typing import List
 from typing import Union
-from typing import Tuple
 from typing import Optional
 from collections import defaultdict
 
 import os
 import pathlib
 import platformdirs
 import fsspec
```

### Comparing `molfeat-0.9.1/molfeat/data/cats_features.fdef` & `molfeat-0.9.2/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/data/elements.xz` & `molfeat-0.9.2/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/data/elements_completed.xz` & `molfeat-0.9.2/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/data/origin.xz` & `molfeat-0.9.2/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/data/skey_parameters.csv` & `molfeat-0.9.2/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/plugins/entry_point.py` & `molfeat-0.9.2/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/plugins/factories.py` & `molfeat-0.9.2/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/store/loader.py` & `molfeat-0.9.2/molfeat/store/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             name: name
         """
         if store is None:
             store = ModelStore()
         try:
             modelcard = store.search(name=name)[0]
             artifact_dir = store.download(modelcard, download_path, **kwargs)
-        except Exception as e:
+        except Exception:
             mess = f"Can't retrieve model {name} from the store !"
             raise ModelStoreError(mess)
         return artifact_dir
 
     def load(self):
         """Load the model"""
         raise NotImplementedError
```

### Comparing `molfeat-0.9.1/molfeat/store/modelcard.py` & `molfeat-0.9.2/molfeat/store/modelcard.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,25 @@
     Args:
         card: model card to use
     """
     if card.group == "all" and card.type != "pretrained":
         import_statement = "from molfeat.trans import MoleculeTransformer"
         loader_statement = f"MoleculeTransformer(featurizer='{card.name}', dtype=float)"
     elif card.group in ["rdkit", "fp", "shape"]:
-        import_statement = f"from molfeat.trans.fp import FPVecTransformer"
+        import_statement = "from molfeat.trans.fp import FPVecTransformer"
         loader_statement = f"FPVecTransformer(kind='{card.name}', dtype=float)"
     elif card.group == "dgllife":
         import_statement = "from molfeat.trans.pretrained import PretrainedDGLTransformer"
         loader_statement = f"PretrainedDGLTransformer(kind='{card.name}', dtype=float)"
     elif card.group == "graphormer":
         import_statement = "from molfeat.trans.pretrained import GraphormerTransformer"
         loader_statement = f"GraphormerTransformer(kind='{card.name}', dtype=float)"
     elif card.group == "fcd":
         import_statement = "from molfeat.trans.pretrained import FCDTransformer"
-        loader_statement = f"FCDTransformer()"
+        loader_statement = "FCDTransformer()"
     elif card.group == "pharmacophore":
         name = card.name.split("-")[-1]
         if card.require_3D:
             import_class = "Pharmacophore3D"
         else:
             import_class = "Pharmacophore2D"
         import_statement = f"from molfeat.trans.base import MoleculeTransformer\nfrom molfeat.calc.pharmacophore import {import_class}"
```

### Comparing `molfeat-0.9.1/molfeat/store/modelstore.py` & `molfeat-0.9.2/molfeat/store/modelstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         model_upload_path = dm.fs.join(model_root_dir, self.MODEL_PATH_NAME)
         model_metadata_upload_path = dm.fs.join(model_root_dir, self.METADATA_PATH_NAME)
 
         save_fn_kwargs = save_fn_kwargs or {}
         if save_fn is None:
             if not isinstance(model, (pathlib.Path, os.PathLike)):
                 local_model_path = tempfile.NamedTemporaryFile(delete=False)
-                with local_model_path as f:
+                with local_model_path:
                     joblib.dump(model, local_model_path)
                 model_path = local_model_path.name
             # Upload the artifact to the bucket
             dm.fs.copy_file(
                 model_path,
                 model_upload_path,
                 progress=True,
@@ -148,18 +148,18 @@
 
     def _filelock(self, lock_name: str):
         """Create an empty lock file into `cache_dir_path/locks/lock_name`"""
 
         lock_path = dm.fs.join(
             str(platformdirs.user_cache_dir("molfeat")), "_lock_files", lock_name
         )
-        mapper = dm.fs.get_mapper(lock_path)
+        dm.fs.get_mapper(lock_path)
         # ensure file is created
         # out = mapper.fs.touch(lock_path) # does not work  -_-
-        with fsspec.open(lock_path, "w", auto_mkdir=True) as f:
+        with fsspec.open(lock_path, "w", auto_mkdir=True):
             pass
 
         return filelock.FileLock(lock_path)
 
     def download(
         self,
         modelcard: ModelInfo,
```

### Comparing `molfeat-0.9.1/molfeat/trans/base.py` & `molfeat-0.9.2/molfeat/trans/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 from molfeat.utils.cache import CacheList
 from molfeat.utils.commons import fn_to_hex
 from molfeat.utils.commons import hex_to_fn
 from molfeat.utils.commons import is_callable
 from molfeat.utils.parsing import get_input_args
 from molfeat.utils.parsing import import_from_string
 from molfeat.utils.state import map_dtype
-from molfeat.utils.state import ATOM_FEATURIZER_MAPPING
-from molfeat.utils.state import BOND_FEATURIZER_MAPPING
 from molfeat.utils.state import ATOM_FEATURIZER_MAPPING_REVERSE
 from molfeat.utils.state import BOND_FEATURIZER_MAPPING_REVERSE
 
 _TRANSFORMERS = {}
 
 
 class _TransformerMeta(abc.ABCMeta):
```

### Comparing `molfeat-0.9.1/molfeat/trans/concat.py` & `molfeat-0.9.2/molfeat/trans/concat.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/trans/fp.py` & `molfeat-0.9.2/molfeat/trans/fp.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         For counting fingerprints, you just need to add the '-count' suffix to the name of the fingerprint. For example:
         "morgan-count:2"
     """
 
     AVAILABLE_FPS = list(FP_FUNCS.keys()) + [
         "desc3D",
         "desc2D",
+        "mordred",
         "cats2D",
         "cats3D",
         "pharm2D",
         "pharm3D",
         "scaffoldkeys",
         "skeys",
         "electroshape",
```

### Comparing `molfeat-0.9.1/molfeat/trans/graph/adj.py` & `molfeat-0.9.2/molfeat/trans/graph/adj.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from rdkit.Chem.rdmolops import Get3DDistanceMatrix
 from molfeat.trans.base import MoleculeTransformer
 from molfeat.utils import datatype
 from molfeat.utils import requires
 from molfeat.utils.commons import requires_conformer
 from molfeat.utils.commons import pack_graph
 from molfeat.calc.atom import AtomCalculator
-from molfeat.calc.bond import BondCalculator
 from molfeat.calc.bond import EdgeMatCalculator
 
 if requires.check("dgl"):
     import dgl
 
 if requires.check("dgllife"):
     from dgllife import utils as dgllife_utils
@@ -99,15 +98,15 @@
         inputs, labels = super().preprocess(inputs, labels)
         new_inputs = []
         for m in inputs:
             try:
                 mol = dm.to_mol(
                     m, add_hs=self.explicit_hydrogens, ordered=self.canonical_atom_order
                 )
-            except:
+            except Exception:
                 mol = None
             new_inputs.append(mol)
 
         return new_inputs, labels
 
     def fit(self, **fit_params):
         """Fit the current transformer on given dataset."""
@@ -122,15 +121,15 @@
 
         Returns:
             atom_dim (int): Number of atom features
         """
         if self._atom_dim is None:
             try:
                 self._atom_dim = len(self.atom_featurizer)
-            except:
+            except Exception:
                 _toy_mol = dm.to_mol("C")
                 out = self.atom_featurizer(_toy_mol)
                 self._atom_dim = sum([x.shape[-1] for x in out.values()])
         return self._atom_dim
 
     @property
     def bond_dim(self):
@@ -141,15 +140,15 @@
             bond_dim (int): Number of bond features
         """
         if self.bond_featurizer is None:
             self._bond_dim = 0
         if self._bond_dim is None:
             try:
                 self._bond_dim = len(self.bond_featurizer)
-            except:
+            except Exception:
                 _toy_mol = dm.to_mol("CO")
                 out = self.bond_featurizer(_toy_mol)
                 self._bond_dim = sum([x.shape[-1] for x in out.values()])
         return self._bond_dim
 
     def _transform(self, mol: dm.Mol):
         r"""
```

### Comparing `molfeat-0.9.1/molfeat/trans/graph/tree.py` & `molfeat-0.9.2/molfeat/trans/graph/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/trans/pretrained/base.py` & `molfeat-0.9.2/molfeat/trans/pretrained/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional
 from typing import Union
 from typing import Callable
 from typing import List
 from collections.abc import Iterable
-from functools import lru_cache
 
 import copy
 import datamol as dm
 
 from loguru import logger
 from molfeat.utils.commons import _parse_to_evaluable_str
 from molfeat.trans.base import MoleculeTransformer
@@ -127,15 +126,15 @@
             inputs: list of input molecules
             labels: list of labels
         """
         out = super().preprocess(inputs, labels)
         if self.precompute_cache not in [False, None]:
             try:
                 self.transform(inputs)
-            except:
+            except Exception:
                 pass
         return out
 
     def _transform(self, mol: dm.Mol, **kwargs):
         r"""
         Compute features for a single molecule.
         This method would potentially need to be reimplemented by any child class
```

### Comparing `molfeat-0.9.1/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.9.2/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/trans/pretrained/fcd.py` & `molfeat-0.9.2/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/trans/pretrained/graphormer.py` & `molfeat-0.9.2/molfeat/trans/pretrained/graphormer.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.9.2/molfeat/trans/pretrained/hf_transformers.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/trans/struct/esm.py` & `molfeat-0.9.2/molfeat/trans/struct/esm.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.repr_layers = layers
         self.repo_or_dir = loader_repo_or_dir
         self.contact = contact
         max_layer_pattern = re.compile(".*_t([0-9]+)_.*")
         self._max_layers = int(max_layer_pattern.match(featurizer).group(1))
         if layers is None:
             self.repr_layers = [self._max_layers]
-        if any(l > self._max_layers for l in self.repr_layers):
+        if any(lay > self._max_layers for lay in self.repr_layers):
             raise ValueError(
                 "You are requesting more layers than available for this pretrained model"
             )
         self._representation = "seq"
         self.pooling = Pooling(dim=0, name=pooling)
         if pooling is None:
             self._representation = "token"
```

### Comparing `molfeat-0.9.1/molfeat/trans/struct/prot1D.py` & `molfeat-0.9.2/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/utils/cache.py` & `molfeat-0.9.2/molfeat/utils/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         if isinstance(mols, str) or not isinstance(mols, Iterable):
             mols = [mols]
 
         # copy if possible to prevent parallel issues
         try:
             cacher = copy.deepcopy(self)
             n_jobs = self.n_jobs
-        except:  # noqa
+        except Exception:  # noqa
             # cannot parallelize process, ensure n_jobs is 0
             cacher = self
             n_jobs = 0
         return dm.parallelized(
             cacher.get, mols, n_jobs=n_jobs, progress=self.verbose, tqdm_kwargs=dict(leave=False)
         )
 
@@ -353,15 +353,15 @@
             # this needs to be done to prevent operating on close files
             self.cache = {}
         if delete:
             if self.cache_file is not None:
                 for path in glob.glob(str(self.cache_file) + "*"):
                     try:
                         os.unlink(path)
-                    except:  # noqa
+                    except Exception:  # noqa
                         pass
         else:
             self._initialize_cache()
 
     def update(self, new_cache: Mapping[Any, Any]):
         """Update the cache with new values
```

### Comparing `molfeat-0.9.1/molfeat/utils/commons.py` & `molfeat-0.9.2/molfeat/utils/commons.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/utils/const.py` & `molfeat-0.9.2/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/utils/converters.py` & `molfeat-0.9.2/molfeat/utils/converters.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,24 +41,24 @@
         """
         if self.converter is None:
             return inp
         with dm.without_rdkit_log():
             try:
                 decoded = self.converter.decode(inp)
                 return decoded.strip()
-            except:  # (deepsmiles.DecodeError, ValueError, AttributeError, IndexError):
+            except Exception:  # (deepsmiles.DecodeError, ValueError, AttributeError, IndexError):
                 return None
 
     def encode(self, smiles: str):
         """Encode a input smiles into target line notation
 
         Args:
             smiles: input smiles to encode
         """
         if self.converter is None:
             return smiles
         with dm.without_rdkit_log():
             try:
                 encoded = self.converter.encode(smiles)
                 return encoded.strip()
-            except:
+            except Exception:
                 return None
```

### Comparing `molfeat-0.9.1/molfeat/utils/datatype.py` & `molfeat-0.9.2/molfeat/utils/datatype.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     Returns:
         New torch.Tensor
     """
     if not torch.is_tensor(x):
         try:
             if torch.is_tensor(x[0]):
                 x = torch.stack(x)
-        except:
+        except Exception:
             pass
         x = torch.as_tensor(x)
     if dtype is not None:
         x = x.to(dtype=dtype)
     if gpu and torch.cuda.is_available():
         x = x.cuda()
     return x
@@ -201,19 +201,19 @@
 def is_null(obj):
     """Check if an obj is null (nan, None or array of nan)"""
     array_nan = False
     all_none = False
     try:
         tmp = to_numpy(obj)
         array_nan = np.all(np.isnan(tmp))
-    except:
+    except Exception:
         pass
     try:
         all_none = all(x is None for x in obj)
-    except:
+    except Exception:
         pass
     return obj is None or all_none or array_nan
 
 
 def cast(fp, dtype: Optional[Callable] = None, columns: Optional[Iterable] = None):
     """Change the datatype of a list of input array
```

### Comparing `molfeat-0.9.1/molfeat/utils/log.py` & `molfeat-0.9.2/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/utils/parsing.py` & `molfeat-0.9.2/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/utils/pooler.py` & `molfeat-0.9.2/molfeat/utils/pooler.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/utils/requires.py` & `molfeat-0.9.2/molfeat/utils/requires.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     imported_module = None
     version = None
     min_version = pkg_version.parse(min_version) if min_version is not None else None
     max_version = pkg_version.parse(max_version) if max_version is not None else None
     try:
         imported_module = importlib.import_module(module)
         version = getattr(imported_module, "__version__", None)
-    except ImportError as _:
+    except ImportError:
         return False
     if version is not None:
         try:
             version = pkg_version.parse(version)
-        except pkg_version.InvalidVersion as _:
+        except pkg_version.InvalidVersion:
             # EN: packaging v22 removed LegacyVersion which has consequences
             version = None
     return version is None or (
         (min_version is None or version >= min_version)
         and (max_version is None or version <= max_version)
     )
```

### Comparing `molfeat-0.9.1/molfeat/utils/state.py` & `molfeat-0.9.2/molfeat/utils/state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat/viz.py` & `molfeat-0.9.2/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/molfeat.egg-info/PKG-INFO` & `molfeat-0.9.2/molfeat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.9.1
+Version: 0.9.2
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -27,14 +27,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dgl
 Provides-Extra: graphormer
 Provides-Extra: transformer
 Provides-Extra: fcd
 Provides-Extra: viz
 Provides-Extra: all
+Provides-Extra: test
+Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
     <img src="docs/images/logo-title.svg" width="100%">
 </div>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.9.1 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.9.2 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -13,15 +13,16 @@
 Science Apps. Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dgl Provides-Extra: graphormer
 Provides-Extra: transformer Provides-Extra: fcd Provides-Extra: viz Provides-
-Extra: all License-File: LICENSE
+Extra: all Provides-Extra: test Provides-Extra: docs Provides-Extra: dev
+License-File: LICENSE
                          [docs/images/logo-title.svg]
              molfeat - the hub for all your molecular featurizers
                                 Docs | Homepage
 --- [![DOI](https://zenodo.org/badge/613548667.svg)](https://zenodo.org/badge/
 latestdoi/613548667) [![PyPI](https://img.shields.io/pypi/v/molfeat)](https://
 pypi.org/project/molfeat/) [![Conda](https://img.shields.io/conda/v/conda-
 forge/molfeat?label=conda&color=success)](https://anaconda.org/conda-forge/
```

### Comparing `molfeat-0.9.1/molfeat.egg-info/SOURCES.txt` & `molfeat-0.9.2/molfeat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/nb/etl/chemberta-etl.ipynb` & `molfeat-0.9.2/nb/etl/chemberta-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/nb/etl/chemgpt-fix-etl.ipynb` & `molfeat-0.9.2/nb/etl/chemgpt-fix-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/nb/etl/dgl-etl.ipynb` & `molfeat-0.9.2/nb/etl/dgl-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/nb/etl/entropy-transforner-zinc-etl.ipynb` & `molfeat-0.9.2/nb/etl/entropy-transforner-zinc-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/nb/etl/featurizer-etl.ipynb` & `molfeat-0.9.2/nb/etl/featurizer-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/nb/etl/molt5-etl.ipynb` & `molfeat-0.9.2/nb/etl/molt5-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/pyproject.toml` & `molfeat-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "molfeat"
 description = "molfeat - the hub for all your molecular featurizers"
 dynamic = ["version"]
-authors = [
-    { name = "Emmanuel Noutahi", email = "emmanuel.noutahi@hotmail.ca" },
-]
+authors = [{ name = "Emmanuel Noutahi", email = "emmanuel.noutahi@hotmail.ca" }]
 readme = "README.md"
 license = { text = "Apache" }
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Healthcare Industry",
@@ -49,53 +47,43 @@
     "h5py",
     "pyarrow",
     "pydantic",
     "platformdirs",
     "scikit-learn",
     "packaging",
     "pmapper",
-
+    "mordredcommunity",
 ]
 
 [project.optional-dependencies]
-dgl = [
-    "dgl",
-    "dgllife",
-]
+dgl = ["dgl", "dgllife"]
 
-graphormer = [
-    "graphormer-pretrained",
-]
+graphormer = ["graphormer-pretrained"]
 
-transformer = [
-    "tokenizers <0.13.2",
-    "transformers",
-    "sentencepiece",
-]
+transformer = ["tokenizers <0.13.2", "transformers", "sentencepiece"]
 
-fcd = [
-    "fcd_torch"
-]
+fcd = ["fcd_torch"]
 
-viz = [
-    "nglview",
-    "ipywidgets"
-]
+viz = ["nglview", "ipywidgets"]
 
 all = [
     "dgl",
     "dgllife",
     "graphormer-pretrained",
     "tokenizers <0.13.2",
     "transformers",
     "fcd_torch",
     "nglview",
     "ipywidgets",
 ]
 
+test = ["pytest >=6.0","pytest-dotenv", "pytest-cov", "pytest-xdist", "black >=22", "ruff"]
+docs = ["mkdocs", "mike", "mdx_truly_sane_lists", "mkdocs-material >=7.1.1", "mkdocs-jupyter", "mkdocstrings", "mkdocstrings-python", "markdown-include"]
+dev = ["molfeat[test]", "molfeat[all]", "molfeat[docs]"]
+
 [project.urls]
 Website = "https://molfeat.datamol.io"
 "Source Code" = "https://github.com/datamol-io/molfeat"
 "Bug Tracker" = "https://github.com/datamol-io/molfeat/issues"
 Documentation = "https://molfeat-docs.datamol.io/"
 
 [tool.setuptools]
@@ -116,14 +104,31 @@
 "molfeat.data" = ["**/*"]
 
 [tool.black]
 line-length = 100
 target-version = ['py39', 'py310']
 include = '\.pyi?$'
 
+[tool.ruff]
+ignore = [
+    "E501", # Never enforce `E501` (line length violations).
+    "E731", # Do not assign a lambda expression, use a def
+]
+line-length = 110
+target-version = "py311"
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = [
+    "F401", # imported but unused
+    "E402", # Module level import not at top of file
+]
+
+[tool.ruff.pycodestyle]
+max-doc-length = 150
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose --cov-report xml --cov-report term --color yes"
 testpaths = ["tests"]
 norecursedirs = "tests/helpers"
 
 [tool.coverage.run]
```

### Comparing `molfeat-0.9.1/tests/test_atom_bond_calculator.py` & `molfeat-0.9.2/tests/test_atom_bond_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,25 +82,25 @@
     mols = [dm.to_mol(x) for x in smiles]
 
     def test_atom_calculator(self):
         atom_calc = AtomCalculator()
         dgl_atom_calc = DGLCanonicalAtomCalculator()
         true_dgl_atom_calc = CanonicalAtomFeaturizer(atom_data_field="hv")
         for mol in self.mols:
-            a1 = atom_calc(mol)
+            atom_calc(mol)
             a2 = dgl_atom_calc(mol)
             a3 = true_dgl_atom_calc(mol)
             np.testing.assert_allclose(a2["hv"], a3["hv"])
 
     def test_bond_calculator(self):
         bond_calc = BondCalculator()
         dgl_bond_calc = DGLCanonicalBondCalculator()
         true_dgl_bond_calc = CanonicalBondFeaturizer(bond_data_field="he")
         for mol in self.mols:
-            b1 = bond_calc(mol)
+            bond_calc(mol)
             b2 = dgl_bond_calc(mol)
             b3 = true_dgl_bond_calc(mol)
             if "he" in b3:
                 np.testing.assert_allclose(b2["he"], b3["he"])
 
     def test_weave_atom_calculator(self):
         true_dgl_weave_calc = WeaveAtomFeaturizer(atom_data_field="hv")
```

### Comparing `molfeat-0.9.1/tests/test_descriptors.py` & `molfeat-0.9.2/tests/test_descriptors.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,54 +9,63 @@
 from molfeat.calc import (
     CATS,
     ElectroShapeDescriptors,
     RDKitDescriptors2D,
     RDKitDescriptors3D,
     ScaffoldKeyCalculator,
     USRDescriptors,
+    MordredDescriptors,
 )
 from molfeat.calc.skeys import skdistance
 
+from molfeat.utils import requires
+
 
 class TestDescPharm(ut.TestCase):
     r"""Test cases for descriptors and pharmacophore generation"""
     smiles = [
         "CCOc1c(OC)cc(CCN)cc1OC",
         "COc1cc(CCN)cc(OC)c1OC",
         "C[C@@H]([NH3+])Cc1c2ccoc2c(Br)c2ccoc12",
     ]
     EXTRA_LARGE_MOL = "CC(C)CC(NCCNC(=O)C(CCC(O)=O)NC(C)=O)C(=O)NC(Cc1ccc(O)cc1)C(=O)NC(CC(C)C)C(=O)NC(C(C)C)C(=O)NC(C)C(=O)NCC(=O)NC(CCC(O)=O)C(=O)NC(CCCNC(N)=N)C(=O)NCC(=O)NC(Cc1ccccc1)C(=O)NC(Cc1ccccc1)C(=O)NC(Cc1ccc(O)cc1)C(=O)NC(C(C)O)C(=O)N1CCCC1C(=O)NC(C)C(O)=O"
 
+    @pytest.mark.xfail(not requires.check("mordred"), reason="3rd party module mordred is missing")
+    def test_mordred(self):
+        calc = MordredDescriptors()
+        fps = calc(self.smiles[0])
+        self.assertEqual(len(fps), len(calc))
+
     def test_rdkit2d(self):
         calc = RDKitDescriptors2D()
         fps = calc(self.smiles[0])
         self.assertEqual(len(fps), len(calc))
 
         sm = "CC[C@@H]1[C@@H]2C[C@H](O)CC[C@]2(C)[C@H]2CC[C@@]3(C)[C@@H](CC[C@@H]3[C@H](C)CCOS(=O)(=O)O[Na])[C@@H]2[C@@H]1O"
         sm_disconnected = "CC[C@@H]1[C@@H]2C[C@H](O)CC[C@]2(C)[C@H]2CC[C@@]3(C)[C@@H](CC[C@@H]3[C@H](C)CCOS(=O)(=O)[O-])[C@@H]2[C@@H]1O.[Na+]"
         # force sanitization would return same descriptors for both of this
         fps = calc(sm)
         fps2 = calc(sm_disconnected)
         np.testing.assert_allclose(fps, fps2)
-
         # with the fix we should not have any value that is nan after sanitization
         # neither for Charge related or BCut2D properties
         self.assertFalse(np.isnan(fps).any())
 
         # we should have nan values at all bcut columns
         # if we do not standardize
         calc_nan = RDKitDescriptors2D(do_not_standardize=True)
         fps = calc_nan(sm)
         bcut_cols = [i for i, x in enumerate(calc.columns) if "bcut" in x.lower()]
         self.assertTrue(np.isnan(fps[bcut_cols]).all())
 
-        # sanity check for large molecules
-        ipc_colums = calc.columns.index("Ipc")
+    def test_rdkit2d_large_mol_no_ipc(self):
+        # sanity check for large molecules that will hang forerever
+        calc = RDKitDescriptors2D(ignore_descrs=["Ipc", "AvgIpc"])
         fps = calc(self.EXTRA_LARGE_MOL)
-        self.assertLessEqual(fps[ipc_colums], 1e3)
+        self.assertEqual(len(fps), len(calc))
 
     def test_rdkit3d(self):
         calc = RDKitDescriptors3D()
         mol = dm.conformers.generate(dm.to_mol(self.smiles[0]))
         fps = calc(mol)
         self.assertEqual(len(fps), len(calc))
 
@@ -105,15 +114,15 @@
         fp2 = calc(mol)
 
         # check
         assert np.allclose(fp1, fp2)
 
     def test_shape_descriptors(self):
         calc = USRDescriptors("usrcat")
-        with self.assertRaises(ValueError) as context:
+        with self.assertRaises(ValueError):
             calc(self.smiles[0])
         mol_with_conf = dm.conformers.generate(dm.to_mol(self.smiles[0]))
         out = calc(mol_with_conf)
         self.assertEqual(out.shape[-1], len(calc))
 
         calc2 = ElectroShapeDescriptors("mmff94")
         out2 = calc2(mol_with_conf)
```

### Comparing `molfeat-0.9.1/tests/test_fp.py` & `molfeat-0.9.2/tests/test_fp.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import datamol as dm
 import joblib
 import numpy as np
 import pandas as pd
 import torch
 from rdkit.DataStructs.cDataStructs import ExplicitBitVect
 
-from molfeat.calc import RDKitDescriptors2D, SerializableCalculator
+from molfeat.calc import SerializableCalculator
 from molfeat.calc.fingerprints import FPCalculator
 from molfeat.calc.pharmacophore import Pharmacophore2D
+from molfeat.calc.descriptors import MordredDescriptors
 from molfeat.trans import MoleculeTransformer
 from molfeat.trans.base import PrecomputedMolTransformer
 from molfeat.trans.concat import FeatConcat
 from molfeat.trans.fp import FPVecFilteredTransformer, FPVecTransformer
 from molfeat.utils.cache import DataCache, FileCache, MPDataCache
 
 
@@ -90,19 +91,19 @@
             self.assertEqual(len(unique_len), 1)
 
     def test_transformer_parallel_mol(self):
         for fpkind in ["atompair", "pharm2D"]:
             transf1 = MoleculeTransformer(featurizer=fpkind, n_jobs=1)
             transf2 = MoleculeTransformer(featurizer=fpkind, n_jobs=-1)
             smiles = dm.freesolv()["smiles"].sample(n=2000, replace=True).values
-            t0 = time.time()
+            time.time()
             out1 = transf1.transform(smiles)
-            t1 = time.time()
+            time.time()
             out2 = transf2.transform(smiles)
-            t2 = time.time()
+            time.time()
             np.testing.assert_allclose(out1, out2)
             # we should be technically saving time with parallelization
             # self.assertLessEqual(t2 - t1, t1 - t0)
 
     def test_fp_parallel(self):
         for fpkind in self.fp_list:
             transf = FPVecTransformer(fpkind, length=1024, n_jobs=2)
@@ -127,21 +128,21 @@
                 n_jobs=-1,
                 parallel_kwargs={"scheduler": "processes"},
             )
             transformer(self.smiles)
 
     def test_unknown_kind_exception(self):
         with self.assertRaises(ValueError) as context:
-            transf = FPVecTransformer(kind="notakind", length=300)
+            FPVecTransformer(kind="notakind", length=300)
             self.assertTrue("is not a valid" in str(context.exception))
 
     def test_none_mol_exception(self):
         transf = MoleculeTransformer("rdkit")
         with self.assertRaises(ValueError) as context:
-            fps = transf.transform([None])
+            transf.transform([None])
             self.assertTrue("transform molecule at" in str(context.exception))
         feat = transf.transform([None], ignore_errors=True)
         self.assertEqual(feat[0], None)
 
     def test_pickling(self):
         for fpkind in self.fp_list:
             transf = FPVecTransformer(fpkind, length=1024, n_jobs=2)
@@ -162,15 +163,15 @@
 
         fp, ids = transf2(self.smiles, enforce_dtype=True, ignore_errors=True)
         self.assertTrue(type(fp[0]) == ExplicitBitVect)
 
     def test_3d_exception(self):
         with self.assertRaises(ValueError) as context:
             transf = MoleculeTransformer("desc3D", verbose=True)
-            fp = transf.transform(self.smiles, ignore_errors=False)
+            transf.transform(self.smiles, ignore_errors=False)
             self.assertTrue("molecule with conformer" in str(context.exception))
 
     def test_fp_filtering(self):
         data = dm.data.freesolv().sample(n=100)
         smiles = data["smiles"].values
         transf = FPVecFilteredTransformer(
             "rdkit", length=4000, del_invariant=True, occ_threshold=0.1
@@ -229,17 +230,17 @@
         out1, ids = concat_transf1(self.smiles, enforce_dtype=True, ignore_errors=True)
         out2, ids = concat_transf1(self.smiles, enforce_dtype=True, ignore_errors=True)
         np.testing.assert_allclose(out1, out2)
 
     def test_caching(self):
         # check performance when cache is added from existing cache
         smiles = dm.data.freesolv().smiles.values[:50]
-        desc = RDKitDescriptors2D(replace_nan=False, ignore_3D=True)
+        desc = MordredDescriptors(replace_nan=False, ignore_3D=True)
         transff = MoleculeTransformer(desc, verbose=True)
-        cache = DataCache(name="rdkit2d")
+        cache = DataCache(name="mordred")
 
         t1 = time.time()
         out1 = transff(smiles)
         elapsed1 = time.time() - t1
         # let's cache only a part of the dataset
         cache(smiles[: len(smiles) // 2], transff)
 
@@ -305,13 +306,13 @@
             self.assertEqual(len(transf_reloaded.cache), len(smiles_list))
             feat_cache_reloaded = transf_reloaded(smiles_list)
             np.testing.assert_array_equal(feat_cache_reloaded, feats)
             np.testing.assert_array_equal(feat_cache_reloaded, feat_cache)
 
             try:
                 os.unlink(parquet_out)
-            except:
+            except Exception:
                 shutil.rmtree(parquet_out)
 
 
 if __name__ == "__main__":
     ut.main()
```

### Comparing `molfeat-0.9.1/tests/test_graphs.py` & `molfeat-0.9.2/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/tests/test_pharmacophore.py` & `molfeat-0.9.2/tests/test_pharmacophore.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,23 +59,23 @@
         shortestPathsOnly=False,
         skipFeats=[
             "A",
         ],
         includeBondOrder=True,
     )
 
-    assert featurizer.useCounts == True
+    assert featurizer.useCounts is True
     assert featurizer.minPointCount == 3
     assert featurizer.maxPointCount == 4
-    assert featurizer.trianglePruneBins == True
-    assert featurizer.shortestPathsOnly == False
+    assert featurizer.trianglePruneBins is True
+    assert featurizer.shortestPathsOnly is False
     assert featurizer.skipFeats == [
         "A",
     ]
-    assert featurizer.includeBondOrder == True
+    assert featurizer.includeBondOrder is True
 
     assert featurizer.useCounts == featurizer.sig_factory.useCounts
     assert featurizer.minPointCount == featurizer.sig_factory.minPointCount
     assert featurizer.maxPointCount == featurizer.sig_factory.maxPointCount
     assert featurizer.trianglePruneBins == featurizer.sig_factory.trianglePruneBins
     assert featurizer.shortestPathsOnly == featurizer.sig_factory.shortestPathsOnly
     assert featurizer.skipFeats == featurizer.sig_factory.skipFeats
```

### Comparing `molfeat-0.9.1/tests/test_pretrained.py` & `molfeat-0.9.2/tests/test_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/tests/test_prot_embed.py` & `molfeat-0.9.2/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.1/tests/test_state.py` & `molfeat-0.9.2/tests/test_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,40 +153,40 @@
 
     # check from_state
     featurizer = MoleculeTransformer.from_state_dict(state)
     state2 = featurizer.to_state_dict()
     featurizer2 = MoleculeTransformer.from_state_dict(state2)
     to_remove = []
     for key in state["args"]:
-        if key.endswith("is_pickled") and state["args"][key] == True:
+        if key.endswith("is_pickled") and state["args"][key] is True:
             to_remove.append(key.replace("is_pickled", "").strip("_"))
     for key_val in to_remove:
         state["args"].pop(key_val, None)
         state2["args"].pop(key_val, None)
     assert state == state2
     mols = dm.freesolv().smiles.iloc[:10]
     out = featurizer(mols)
     out2 = featurizer2(mols)
     assert len(out) == len(out2) == len(mols)
     for o1, o2 in zip(out, out2):
         if isinstance(o1, (list, tuple)):
-            assert np.all([np.allclose(i, j, atol=2) for i, j in zip(o1, o2)]) == True
+            assert bool(np.all([np.allclose(i, j, atol=2) for i, j in zip(o1, o2)])) is True
         else:
             np.testing.assert_array_equal(o1, o2)
 
 
 def test_PrecomputedMolTransformer_state(tmp_path):
     cache_path = tmp_path / "cache.parquet"
     smiles_list = ["[NH3+]CCSc1cc(-c2ccc[nH]2)c2c3c(ccc(F)c13)NC2=O", "CCCO"]
 
     featurizer = FPVecTransformer(kind="ecfp", length=2048)
     cache = FileCache(cache_file=cache_path, file_type="parquet", n_jobs=-1)
 
     featurizer_cache = PrecomputedMolTransformer(cache=cache, featurizer=featurizer)
-    fps = featurizer_cache(smiles_list)
+    featurizer_cache(smiles_list)
 
     # sanity check
     assert len(featurizer_cache.cache.cache) == 2
 
     # serialize to state
     state = featurizer_cache.to_state_dict()
 
@@ -210,15 +210,15 @@
     cache_path = str(tmp_path / "cache.parquet")
     smiles_list = ["[NH3+]CCSc1cc(-c2ccc[nH]2)c2c3c(ccc(F)c13)NC2=O", "CCCO"]
 
     featurizer = FPVecTransformer(kind="ecfp", length=2048)
     cache = FileCache(cache_file=cache_path, file_type="parquet", n_jobs=-1)
 
     featurizer_cache = PrecomputedMolTransformer(cache=cache, featurizer=featurizer)
-    fps = featurizer_cache(smiles_list)
+    featurizer_cache(smiles_list)
 
     # sanity check
     assert len(featurizer_cache.cache.cache) == 2
 
     # serialize to state
     state = featurizer_cache.to_state_dict()
```

### Comparing `molfeat-0.9.1/tests/test_utils.py` & `molfeat-0.9.2/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         save_file = save_file.name
         disk_cache.save_to_file(save_file)
         new_cache = DataCache.load_from_file(save_file)
         self.assertTrue(first_smiles in new_cache)
         np.testing.assert_array_equal(new_cache[first_smiles], first_smiles_val)
         try:
             os.unlink(save_file)
-        except:
+        except Exception:
             pass
 
     def test_filecache(self):
         mol_data = dm.data.freesolv().iloc[:100]
         # in memory cache
         smiles_list = mol_data["smiles"].values
         hash_fn = dm.unique_id
@@ -192,15 +192,15 @@
             self.assertFalse("FAKE" in reloaded_cache)
             np.testing.assert_array_equal(reloaded_cache[first_smiles], first_smiles_val)
             np.testing.assert_array_equal(reloaded_cache_parquet[first_smiles], first_smiles_val)
             np.testing.assert_array_equal(reloaded_cache_csv[first_smiles], first_smiles_val)
             for path in [parquet_out, csv_out]:
                 try:
                     os.unlink(path)
-                except:
+                except Exception:
                     shutil.rmtree(path)
 
     def test_cache_list(self):
         # Test multiple cache simultaneously
         mol_data = dm.data.freesolv().iloc[:200]
         smiles_list = mol_data["smiles"].values
         featurizer = FPVecTransformer(kind="rdkit", length=10)
```

