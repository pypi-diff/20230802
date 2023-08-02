# Comparing `tmp/splink-3.9.4.tar.gz` & `tmp/splink-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.9.4.tar", max compression
+gzip compressed data, was "splink-3.9.5.tar", max compression
```

## Comparing `splink-3.9.4.tar` & `splink-3.9.5.tar`

### file list

```diff
@@ -1,162 +1,163 @@
--rw-r--r--   0        0        0     1076 2023-07-19 13:19:55.452417 splink-3.9.4/LICENSE
--rw-r--r--   0        0        0     8866 2023-07-19 13:19:55.452417 splink-3.9.4/README.md
--rw-r--r--   0        0        0     2110 2023-07-19 13:19:55.492420 splink-3.9.4/pyproject.toml
--rw-r--r--   0        0        0       23 2023-07-19 13:19:55.496420 splink-3.9.4/splink/__init__.py
--rw-r--r--   0        0        0    10852 2023-07-19 13:19:55.496420 splink-3.9.4/splink/accuracy.py
--rw-r--r--   0        0        0     7765 2023-07-19 13:19:55.496420 splink-3.9.4/splink/analyse_blocking.py
--rw-r--r--   0        0        0      387 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0      396 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_comparison_template_library.py
--rw-r--r--   0        0        0     1365 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_base.py
--rw-r--r--   0        0        0      165 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_blocking_rule_imports.py
--rw-r--r--   0        0        0     3322 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_comparison_imports.py
--rw-r--r--   0        0        0      350 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_transforms.py
--rw-r--r--   0        0        0     2903 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_utils.py
--rw-r--r--   0        0        0      361 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_linker.py
--rw-r--r--   0        0        0      175 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/blocking_rule_library.py
--rw-r--r--   0        0        0      403 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/comparison_level_library.py
--rw-r--r--   0        0        0      249 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/comparison_library.py
--rw-r--r--   0        0        0      252 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/comparison_template_library.py
--rw-r--r--   0        0        0    21171 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/linker.py
--rw-r--r--   0        0        0     2867 2023-07-19 13:19:55.496420 splink-3.9.4/splink/block_from_labels.py
--rw-r--r--   0        0        0     9907 2023-07-19 13:19:55.496420 splink-3.9.4/splink/blocking.py
--rw-r--r--   0        0        0    12386 2023-07-19 13:19:55.496420 splink-3.9.4/splink/blocking_rule_composition.py
--rw-r--r--   0        0        0     2135 2023-07-19 13:19:55.496420 splink-3.9.4/splink/blocking_rules_library.py
--rw-r--r--   0        0        0     2223 2023-07-19 13:19:55.496420 splink-3.9.4/splink/cache_dict_with_logging.py
--rw-r--r--   0        0        0    11044 2023-07-19 13:19:55.496420 splink-3.9.4/splink/charts.py
--rw-r--r--   0        0        0     9155 2023-07-19 13:19:55.496420 splink-3.9.4/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison.py
--rw-r--r--   0        0        0     8766 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_helpers.py
--rw-r--r--   0        0        0      554 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_helpers_utils.py
--rw-r--r--   0        0        0    25557 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level.py
--rw-r--r--   0        0        0    16609 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    57707 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    63328 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_library.py
--rw-r--r--   0        0        0     4922 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    81390 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16699 2023-07-19 13:19:55.496420 splink-3.9.4/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-07-19 13:19:55.496420 splink-3.9.4/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-07-19 13:19:55.496420 splink-3.9.4/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-07-19 13:19:55.496420 splink-3.9.4/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0     5562 2023-07-19 13:19:55.496420 splink-3.9.4/splink/datasets/__init__.py
--rw-r--r--   0        0        0      609 2023-07-19 13:19:55.496420 splink-3.9.4/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1608 2023-07-19 13:19:55.496420 splink-3.9.4/splink/dialect_base.py
--rw-r--r--   0        0        0      175 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/blocking_rule_library.py
--rw-r--r--   0        0        0      493 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/comparison_level_library.py
--rw-r--r--   0        0        0      371 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/comparison_library.py
--rw-r--r--   0        0        0      194 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/comparison_template_library.py
--rw-r--r--   0        0        0      387 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      396 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1555 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_base.py
--rw-r--r--   0        0        0      165 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_blocking_rule_imports.py
--rw-r--r--   0        0        0     5623 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
--rw-r--r--   0        0        0     1750 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_helpers.py
--rw-r--r--   0        0        0      367 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    11906 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/linker.py
--rw-r--r--   0        0        0    17650 2023-07-19 13:19:55.496420 splink-3.9.4/splink/em_training_session.py
--rw-r--r--   0        0        0     5743 2023-07-19 13:19:55.496420 splink-3.9.4/splink/estimate_u.py
--rw-r--r--   0        0        0      269 2023-07-19 13:19:55.496420 splink-3.9.4/splink/exceptions.py
--rw-r--r--   0        0        0     9070 2023-07-19 13:19:55.496420 splink-3.9.4/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1562 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     5153 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/comparator_score_chart.json
--rw-r--r--   0        0        0     1836 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/comparator_score_threshold_chart.json
--rw-r--r--   0        0        0     2775 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     5795 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0     1111 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5691 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9113 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1714 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     2753 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1891 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/phonetic_match_chart.json
--rw-r--r--   0        0        0     1654 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1125 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1805 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     9910 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/chart_defs/tf_adjustment_chart.json
--rw-r--r--   0        0        0     2910 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-07-19 13:19:55.504420 splink-3.9.4/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0   974616 2023-07-19 13:19:55.508421 splink-3.9.4/splink/files/labelling_tool/slt.js
--rw-r--r--   0        0        0     2971 2023-07-19 13:19:55.508421 splink-3.9.4/splink/files/labelling_tool/template.j2
--rw-r--r--   0        0        0    13833 2023-07-19 13:19:55.508421 splink-3.9.4/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-07-19 13:19:55.516421 splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-07-19 13:19:55.524422 splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     5486 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-07-19 13:19:55.532422 splink-3.9.4/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-07-19 13:19:55.532422 splink-3.9.4/splink/files/templates/single_chart_template.html
--rw-r--r--   0        0        0      195 2023-07-19 13:19:55.532422 splink-3.9.4/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-07-19 13:19:55.532422 splink-3.9.4/splink/input_column.py
--rw-r--r--   0        0        0     3279 2023-07-19 13:19:55.532422 splink-3.9.4/splink/labelling_tool.py
--rw-r--r--   0        0        0   135622 2023-07-19 13:19:55.532422 splink-3.9.4/splink/linker.py
--rw-r--r--   0        0        0      300 2023-07-19 13:19:55.532422 splink-3.9.4/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-07-19 13:19:55.532422 splink-3.9.4/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-07-19 13:19:55.532422 splink-3.9.4/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-07-19 13:19:55.532422 splink-3.9.4/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-07-19 13:19:55.532422 splink-3.9.4/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-07-19 13:19:55.532422 splink-3.9.4/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-07-19 13:19:55.532422 splink-3.9.4/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     6135 2023-07-19 13:19:55.532422 splink-3.9.4/splink/misc.py
--rw-r--r--   0        0        0     2791 2023-07-19 13:19:55.532422 splink-3.9.4/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-07-19 13:19:55.532422 splink-3.9.4/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-07-19 13:19:55.532422 splink-3.9.4/splink/pipeline.py
--rw-r--r--   0        0        0      188 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/blocking_rule_library.py
--rw-r--r--   0        0        0      407 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/comparison_level_library.py
--rw-r--r--   0        0        0      253 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/comparison_library.py
--rw-r--r--   0        0        0      394 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/comparison_template_library.py
--rw-r--r--   0        0        0    11226 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/linker.py
--rw-r--r--   0        0        0      393 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_comparison_level_library.py
--rw-r--r--   0        0        0      375 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_comparison_library.py
--rw-r--r--   0        0        0      402 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_comparison_template_library.py
--rw-r--r--   0        0        0     1530 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_helpers/postgres_base.py
--rw-r--r--   0        0        0      171 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_helpers/postgres_blocking_rule_imports.py
--rw-r--r--   0        0        0     3129 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_helpers/postgres_comparison_imports.py
--rw-r--r--   0        0        0      362 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_linker.py
--rw-r--r--   0        0        0     5624 2023-07-19 13:19:55.532422 splink-3.9.4/splink/predict.py
--rw-r--r--   0        0        0     8245 2023-07-19 13:19:55.532422 splink-3.9.4/splink/profile_data.py
--rw-r--r--   0        0        0    18835 2023-07-19 13:19:55.532422 splink-3.9.4/splink/settings.py
--rw-r--r--   0        0        0    17972 2023-07-19 13:19:55.532422 splink-3.9.4/splink/settings_validator.py
--rw-r--r--   0        0        0      173 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/blocking_rule_library.py
--rw-r--r--   0        0        0      491 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/comparison_library.py
--rw-r--r--   0        0        0      192 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/comparison_template_library.py
--rw-r--r--   0        0        0      473 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/jar_location.py
--rw-r--r--   0        0        0    23599 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/linker.py
--rw-r--r--   0        0        0      384 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0      366 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      393 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0     1083 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/custom_spark_dialect.py
--rw-r--r--   0        0        0     1875 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/spark_base.py
--rw-r--r--   0        0        0      162 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/spark_blocking_rule_imports.py
--rw-r--r--   0        0        0     5584 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/spark_comparison_imports.py
--rw-r--r--   0        0        0      356 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4397 2023-07-19 13:19:55.532422 splink-3.9.4/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     4152 2023-07-19 13:19:55.532422 splink-3.9.4/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1205 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sql_transform.py
--rw-r--r--   0        0        0      175 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/blocking_rule_library.py
--rw-r--r--   0        0        0      401 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/comparison_level_library.py
--rw-r--r--   0        0        0      252 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/comparison_library.py
--rw-r--r--   0        0        0      126 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/comparison_template_library.py
--rw-r--r--   0        0        0     8562 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/linker.py
--rw-r--r--   0        0        0      387 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0      396 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_comparison_template_library.py
--rw-r--r--   0        0        0      270 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_base.py
--rw-r--r--   0        0        0      165 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_blocking_rule_imports.py
--rw-r--r--   0        0        0     3761 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
--rw-r--r--   0        0        0      361 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0     9772 2023-07-19 13:19:55.532422 splink-3.9.4/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-07-19 13:19:55.532422 splink-3.9.4/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1673 2023-07-19 13:19:55.532422 splink-3.9.4/splink/unlinkables.py
--rw-r--r--   0        0        0     2383 2023-07-19 13:19:55.532422 splink-3.9.4/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2326 2023-07-19 13:19:55.532422 splink-3.9.4/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-07-19 13:19:55.532422 splink-3.9.4/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9849 1970-01-01 00:00:00.000000 splink-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-08-02 21:04:32.351274 splink-3.9.5/LICENSE
+-rw-r--r--   0        0        0     9898 2023-08-02 21:04:32.351274 splink-3.9.5/README.md
+-rw-r--r--   0        0        0     2325 2023-08-02 21:04:32.511275 splink-3.9.5/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-08-02 21:04:32.511275 splink-3.9.5/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-08-02 21:04:32.511275 splink-3.9.5/splink/accuracy.py
+-rw-r--r--   0        0        0     7941 2023-08-02 21:04:32.511275 splink-3.9.5/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      387 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_comparison_template_library.py
+-rw-r--r--   0        0        0     1365 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_helpers/athena_base.py
+-rw-r--r--   0        0        0      165 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_helpers/athena_blocking_rule_imports.py
+-rw-r--r--   0        0        0     3322 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_helpers/athena_comparison_imports.py
+-rw-r--r--   0        0        0      350 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     2903 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0      361 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0      175 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/blocking_rule_library.py
+-rw-r--r--   0        0        0      403 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/comparison_level_library.py
+-rw-r--r--   0        0        0      249 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/comparison_library.py
+-rw-r--r--   0        0        0      252 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/comparison_template_library.py
+-rw-r--r--   0        0        0    21171 2023-08-02 21:04:32.511275 splink-3.9.5/splink/athena/linker.py
+-rw-r--r--   0        0        0     2867 2023-08-02 21:04:32.511275 splink-3.9.5/splink/block_from_labels.py
+-rw-r--r--   0        0        0     9900 2023-08-02 21:04:32.511275 splink-3.9.5/splink/blocking.py
+-rw-r--r--   0        0        0    12386 2023-08-02 21:04:32.511275 splink-3.9.5/splink/blocking_rule_composition.py
+-rw-r--r--   0        0        0     2135 2023-08-02 21:04:32.511275 splink-3.9.5/splink/blocking_rules_library.py
+-rw-r--r--   0        0        0     2223 2023-08-02 21:04:32.511275 splink-3.9.5/splink/cache_dict_with_logging.py
+-rw-r--r--   0        0        0    11044 2023-08-02 21:04:32.511275 splink-3.9.5/splink/charts.py
+-rw-r--r--   0        0        0     9155 2023-08-02 21:04:32.511275 splink-3.9.5/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison.py
+-rw-r--r--   0        0        0     8766 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_helpers.py
+-rw-r--r--   0        0        0      554 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_helpers_utils.py
+-rw-r--r--   0        0        0    25557 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_level.py
+-rw-r--r--   0        0        0    16609 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    57707 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    63328 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_library.py
+-rw-r--r--   0        0        0     4922 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    81813 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-08-02 21:04:32.511275 splink-3.9.5/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16699 2023-08-02 21:04:32.511275 splink-3.9.5/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-08-02 21:04:32.511275 splink-3.9.5/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-08-02 21:04:32.511275 splink-3.9.5/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-08-02 21:04:32.511275 splink-3.9.5/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0     9695 2023-08-02 21:04:32.511275 splink-3.9.5/splink/datasets/__init__.py
+-rw-r--r--   0        0        0      609 2023-08-02 21:04:32.511275 splink-3.9.5/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1608 2023-08-02 21:04:32.511275 splink-3.9.5/splink/dialect_base.py
+-rw-r--r--   0        0        0      175 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/blocking_rule_library.py
+-rw-r--r--   0        0        0      493 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/comparison_level_library.py
+-rw-r--r--   0        0        0      371 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/comparison_library.py
+-rw-r--r--   0        0        0      194 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/comparison_template_library.py
+-rw-r--r--   0        0        0      387 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1555 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_helpers/duckdb_base.py
+-rw-r--r--   0        0        0      165 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_helpers/duckdb_blocking_rule_imports.py
+-rw-r--r--   0        0        0     5623 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
+-rw-r--r--   0        0        0     1750 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0      361 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    11882 2023-08-02 21:04:32.511275 splink-3.9.5/splink/duckdb/linker.py
+-rw-r--r--   0        0        0    17650 2023-08-02 21:04:32.515275 splink-3.9.5/splink/em_training_session.py
+-rw-r--r--   0        0        0     5743 2023-08-02 21:04:32.515275 splink-3.9.5/splink/estimate_u.py
+-rw-r--r--   0        0        0      269 2023-08-02 21:04:32.515275 splink-3.9.5/splink/exceptions.py
+-rw-r--r--   0        0        0     9070 2023-08-02 21:04:32.515275 splink-3.9.5/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1562 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     5153 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     1836 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2775 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     5795 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0     1111 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5691 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9113 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1714 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     2753 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1891 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1654 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1125 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1805 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9910 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0     2910 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-08-02 21:04:32.515275 splink-3.9.5/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-08-02 21:04:32.519275 splink-3.9.5/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0   974616 2023-08-02 21:04:32.523275 splink-3.9.5/splink/files/labelling_tool/slt.js
+-rw-r--r--   0        0        0     2971 2023-08-02 21:04:32.523275 splink-3.9.5/splink/files/labelling_tool/template.j2
+-rw-r--r--   0        0        0    13833 2023-08-02 21:04:32.523275 splink-3.9.5/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-08-02 21:04:32.527275 splink-3.9.5/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-08-02 21:04:32.535275 splink-3.9.5/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-08-02 21:04:32.539275 splink-3.9.5/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-08-02 21:04:32.539275 splink-3.9.5/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-08-02 21:04:32.539275 splink-3.9.5/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-08-02 21:04:32.539275 splink-3.9.5/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-08-02 21:04:32.539275 splink-3.9.5/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-08-02 21:04:32.543275 splink-3.9.5/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-08-02 21:04:32.543275 splink-3.9.5/splink/files/templates/single_chart_template.html
+-rw-r--r--   0        0        0     1426 2023-08-02 21:04:32.543275 splink-3.9.5/splink/find_matches_to_new_records.py
+-rw-r--r--   0        0        0      195 2023-08-02 21:04:32.543275 splink-3.9.5/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-08-02 21:04:32.543275 splink-3.9.5/splink/input_column.py
+-rw-r--r--   0        0        0     3279 2023-08-02 21:04:32.543275 splink-3.9.5/splink/labelling_tool.py
+-rw-r--r--   0        0        0   136191 2023-08-02 21:04:32.543275 splink-3.9.5/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-08-02 21:04:32.543275 splink-3.9.5/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-08-02 21:04:32.543275 splink-3.9.5/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-08-02 21:04:32.543275 splink-3.9.5/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-08-02 21:04:32.543275 splink-3.9.5/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-08-02 21:04:32.543275 splink-3.9.5/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-08-02 21:04:32.543275 splink-3.9.5/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-08-02 21:04:32.543275 splink-3.9.5/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     6135 2023-08-02 21:04:32.543275 splink-3.9.5/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-08-02 21:04:32.543275 splink-3.9.5/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-08-02 21:04:32.543275 splink-3.9.5/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-08-02 21:04:32.543275 splink-3.9.5/splink/pipeline.py
+-rw-r--r--   0        0        0      188 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/blocking_rule_library.py
+-rw-r--r--   0        0        0      407 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/comparison_level_library.py
+-rw-r--r--   0        0        0      253 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/comparison_library.py
+-rw-r--r--   0        0        0      394 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/comparison_template_library.py
+-rw-r--r--   0        0        0    11226 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/linker.py
+-rw-r--r--   0        0        0      393 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/postgres_comparison_level_library.py
+-rw-r--r--   0        0        0      375 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/postgres_comparison_library.py
+-rw-r--r--   0        0        0      402 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/postgres_comparison_template_library.py
+-rw-r--r--   0        0        0     1530 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/postgres_helpers/postgres_base.py
+-rw-r--r--   0        0        0      171 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/postgres_helpers/postgres_blocking_rule_imports.py
+-rw-r--r--   0        0        0     3129 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/postgres_helpers/postgres_comparison_imports.py
+-rw-r--r--   0        0        0      362 2023-08-02 21:04:32.543275 splink-3.9.5/splink/postgres/postgres_linker.py
+-rw-r--r--   0        0        0     5624 2023-08-02 21:04:32.543275 splink-3.9.5/splink/predict.py
+-rw-r--r--   0        0        0     8245 2023-08-02 21:04:32.543275 splink-3.9.5/splink/profile_data.py
+-rw-r--r--   0        0        0    18835 2023-08-02 21:04:32.543275 splink-3.9.5/splink/settings.py
+-rw-r--r--   0        0        0    17972 2023-08-02 21:04:32.543275 splink-3.9.5/splink/settings_validator.py
+-rw-r--r--   0        0        0      173 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/blocking_rule_library.py
+-rw-r--r--   0        0        0      491 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/comparison_library.py
+-rw-r--r--   0        0        0      192 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/comparison_template_library.py
+-rw-r--r--   0        0        0      473 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/jar_location.py
+-rw-r--r--   0        0        0    23599 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/linker.py
+-rw-r--r--   0        0        0      384 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0      366 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      393 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0     1083 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     1875 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_helpers/spark_base.py
+-rw-r--r--   0        0        0      162 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_helpers/spark_blocking_rule_imports.py
+-rw-r--r--   0        0        0     5584 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_helpers/spark_comparison_imports.py
+-rw-r--r--   0        0        0      356 2023-08-02 21:04:32.543275 splink-3.9.5/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4397 2023-08-02 21:04:32.543275 splink-3.9.5/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     6453 2023-08-02 21:04:32.543275 splink-3.9.5/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1205 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sql_transform.py
+-rw-r--r--   0        0        0      175 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/blocking_rule_library.py
+-rw-r--r--   0        0        0      401 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/comparison_level_library.py
+-rw-r--r--   0        0        0      252 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/comparison_library.py
+-rw-r--r--   0        0        0      126 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/comparison_template_library.py
+-rw-r--r--   0        0        0     8562 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/linker.py
+-rw-r--r--   0        0        0      387 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/sqlite_comparison_template_library.py
+-rw-r--r--   0        0        0      270 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/sqlite_helpers/sqlite_base.py
+-rw-r--r--   0        0        0      165 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/sqlite_helpers/sqlite_blocking_rule_imports.py
+-rw-r--r--   0        0        0     3761 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
+-rw-r--r--   0        0        0      361 2023-08-02 21:04:32.543275 splink-3.9.5/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0     9772 2023-08-02 21:04:32.543275 splink-3.9.5/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-08-02 21:04:32.543275 splink-3.9.5/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1673 2023-08-02 21:04:32.543275 splink-3.9.5/splink/unlinkables.py
+-rw-r--r--   0        0        0     2383 2023-08-02 21:04:32.543275 splink-3.9.5/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-08-02 21:04:32.543275 splink-3.9.5/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-08-02 21:04:32.543275 splink-3.9.5/splink/waterfall_chart.py
+-rw-r--r--   0        0        0    10888 1970-01-01 00:00:00.000000 splink-3.9.5/PKG-INFO
```

### Comparing `splink-3.9.4/LICENSE` & `splink-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/README.md` & `splink-3.9.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 High correlation occurs when the value of a column is highly constrained (predictable) from the value of another column. For example, a 'city' field is almost perfectly correlated with 'postcode'. Gender is highly correlated with 'first name'. Correlation is particularly problematic if **all** of your input columns are highly correlated.
 
 Splink is not designed for linking a single column containing a 'bag of words'. For example, a table with a single 'company name' column, and no other details.
 
 ## Documentation
 
-The homepage for the Splink documentation can be found [here](https://moj-analytical-services.github.io/splink/). Interactive demos can be found [here](https://github.com/moj-analytical-services/splink_demos/tree/splink3_demos), or by clicking the following Binder link:
+The homepage for the Splink documentation can be found [here](https://moj-analytical-services.github.io/splink/). Interactive demos can be found [here](https://github.com/moj-analytical-services/splink/tree/master/docs/demos), or by clicking the following Binder link:
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/moj-analytical-services/splink_demos/master?urlpath=lab)
 
 The specification of the Fellegi Sunter statistical model behind `splink` is similar as that used in the R [fastLink package](https://github.com/kosukeimai/fastLink). Accompanying the fastLink package is an [academic paper](http://imai.fas.harvard.edu/research/files/linkage.pdf) that describes this model. The [Splink documentation site](https://moj-analytical-services.github.io/splink/topic_guides/fellegi_sunter.html) and a [series of interactive articles](https://www.robinlinacre.com/probabilistic_linkage/) also explores the theory behind Splink.
 
 The Office for National Statistics have written a [case study about using Splink](https://github.com/Data-Linkage/Splink-census-linkage/blob/main/SplinkCaseStudy.pdf) to link 2021 Census data to itself.
 
@@ -93,15 +93,15 @@
         brl.exact_match_rule("surname"),
     ],
     "comparisons": [
         ctl.name_comparison("first_name"),
         ctl.name_comparison("surname"),
         ctl.date_comparison("dob", cast_strings_to_date=True),
         cl.exact_match("city", term_frequency_adjustments=True),
-        ctl.email_comparison("email"),
+        ctl.email_comparison("email", include_username_fuzzy_level=False),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
 blocking_rule_for_training = brl.and_(
@@ -158,7 +158,16 @@
 ```
 
 ## Acknowledgements
 
 We are very grateful to [ADR UK](https://www.adruk.org/) (Administrative Data Research UK) for providing the initial funding for this work as part of the [Data First](https://www.adruk.org/our-work/browse-all-projects/data-first-harnessing-the-potential-of-linked-administrative-data-for-the-justice-system-169/) project.
 
 We are extremely grateful to professors Katie Harron, James Doidge and Peter Christen for their expert advice and guidance in the development of Splink. We are also very grateful to colleagues at the UK's Office for National Statistics for their expert advice and peer review of this work. Any errors remain our own.
+
+## Related Repositories
+
+While Splink is a standalone package, there are a number of repositories in the Splink ecosystem:
+
+- [splink_demos](https://github.com/moj-analytical-services/splink_demos) contains a copy of the Splink tutorial and example notebooks that are hosted via [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/moj-analytical-services/splink_demos/master?urlpath=lab)
+- [splink_scalaudfs](https://github.com/moj-analytical-services/splink_scalaudfs) contains the code to generate [User Defined Functions](https://moj-analytical-services.github.io/splink/dev_guides/udfs.html#spark) in scala which are then callable in Spark.
+- [splink_datasets](https://github.com/moj-analytical-services/splink_datasets) contains datasets that can be installed automatically as a part of Splink through the [In-build datasets](https://moj-analytical-services.github.io/splink/datasets.html) functionality.
+- [splink_synthetic_data] contains code to generate synthetic data.
```

### Comparing `splink-3.9.4/pyproject.toml` & `splink-3.9.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "splink"
-version = "3.9.4"
+version = "3.9.5"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.7,<4.0.0"
 jsonschema = ">=3.2,<5.0"
 pandas = ">=1.0.0"
 duckdb = ">=0.8.0"
 # normalize issue in sqlglot - temporarily exclude updates
 sqlglot = ">=7.0.0,<11.4.2"
 altair = "^5.0.1"
 Jinja2 = ">=3.0.3"
@@ -42,14 +42,24 @@
 
 [tool.poetry.group.benchmarking]
 optional = true
 [tool.poetry.group.benchmarking.dependencies]
 pytest-benchmark = "^4"
 lzstring = "1.0.4"
 
+[tool.poetry.group.demos]
+[tool.poetry.group.demos.dependencies]
+importlib-resources = "5.4.0"
+jupyterlab = "3.6.1"
+pyarrow = "7.0.0"
+ipywidgets = "8.0.4"
+nbmake = "1.3.4"
+pytest = "^7.0"
+pyspark = "^3.2.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `splink-3.9.4/splink/accuracy.py` & `splink-3.9.5/splink/accuracy.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/analyse_blocking.py` & `splink-3.9.5/splink/analyse_blocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,20 @@
         from __splink__df_blocked_data
         group by match_key
         order by cast(match_key as int) asc
     """
     linker._enqueue_sql(sql, "__splink__df_count_cumulative_blocks")
     cumulative_blocking_rule_count = linker._execute_sql_pipeline([concat])
     br_n = cumulative_blocking_rule_count.as_pandas_dataframe()
+    # not all dialects return column names when frame is empty (e.g. sqlite, postgres)
+    if br_n.empty:
+        br_n["row_count"] = []
+        br_n["match_key"] = []
     cumulative_blocking_rule_count.drop_table_from_database_and_remove_from_cache()
-    br_count, br_keys = list(br_n.row_count), list(br_n["match_key"].astype("int"))
+    br_count, br_keys = list(br_n["row_count"]), list(br_n["match_key"].astype("int"))
 
     if len(br_count) != len(brs_as_objs):
         missing_br = [x for x in range(len(brs_as_objs)) if x not in br_keys]
         for n in missing_br:
             br_count.insert(n, 0)
 
     br_comparisons = []
@@ -143,15 +147,15 @@
 
 def count_comparisons_from_blocking_rule_pre_filter_conditions_sqls(
     linker: "Linker", blocking_rule: Union[str, "BlockingRule"]
 ):
     if isinstance(blocking_rule, str):
         blocking_rule = BlockingRule(blocking_rule, sqlglot_dialect=linker._sql_dialect)
 
-    join_conditions = blocking_rule._join_conditions
+    join_conditions = blocking_rule._equi_join_conditions
 
     l_cols_sel = []
     r_cols_sel = []
     l_cols_gb = []
     r_cols_gb = []
     using = []
     for (
```

### Comparing `splink-3.9.4/splink/athena/athena_helpers/athena_base.py` & `splink-3.9.5/splink/athena/athena_helpers/athena_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/athena/athena_helpers/athena_comparison_imports.py` & `splink-3.9.5/splink/athena/athena_helpers/athena_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/athena/athena_helpers/athena_utils.py` & `splink-3.9.5/splink/athena/athena_helpers/athena_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/athena/linker.py` & `splink-3.9.5/splink/athena/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/block_from_labels.py` & `splink-3.9.5/splink/block_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/blocking.py` & `splink-3.9.5/splink/blocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 class BlockingRule:
     def __init__(
         self,
         blocking_rule: BlockingRule | dict | str,
         salting_partitions=1,
         sqlglot_dialect: str = None,
     ):
-
         if sqlglot_dialect:
             self._sql_dialect = sqlglot_dialect
 
         self.blocking_rule = blocking_rule
         self.preceding_rules = []
         self.sqlglot_dialect = sqlglot_dialect
         self.salting_partitions = salting_partitions
@@ -86,18 +85,18 @@
     def _parsed_join_condition(self):
         br = self.blocking_rule
         return parse_one("INNER JOIN r", into=Join).on(
             br, dialect=self.sqlglot_dialect
         )  # using sqlglot==11.4.1
 
     @property
-    def _join_conditions(self):
+    def _equi_join_conditions(self):
         """
-        Extract the join conditions from the blocking rule as a tuple:
-        source_keys, join_keys, condition_expr
+        Extract the equi join conditions from the blocking rule as a tuple:
+        source_keys, join_keys
 
         Returns:
             list of tuples like [(name, name), (substr(name,1,2), substr(name,2,3))]
         """
 
         def remove_table_prefix(tree):
             for c in tree.find_all(Column):
```

### Comparing `splink-3.9.4/splink/blocking_rule_composition.py` & `splink-3.9.5/splink/blocking_rule_composition.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/blocking_rules_library.py` & `splink-3.9.5/splink/blocking_rules_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/cache_dict_with_logging.py` & `splink-3.9.5/splink/cache_dict_with_logging.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/charts.py` & `splink-3.9.5/splink/charts.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/cluster_studio.py` & `splink-3.9.5/splink/cluster_studio.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison.py` & `splink-3.9.5/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_helpers.py` & `splink-3.9.5/splink/comparison_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_helpers_utils.py` & `splink-3.9.5/splink/comparison_helpers_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_level.py` & `splink-3.9.5/splink/comparison_level.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_level_composition.py` & `splink-3.9.5/splink/comparison_level_composition.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_level_library.py` & `splink-3.9.5/splink/comparison_level_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_level_sql.py` & `splink-3.9.5/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_library.py` & `splink-3.9.5/splink/comparison_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_library_utils.py` & `splink-3.9.5/splink/comparison_library_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_template_library.py` & `splink-3.9.5/splink/comparison_template_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -1381,14 +1381,15 @@
         self,
         col_name: str,
         invalid_emails_as_null: bool = False,
         valid_email_regex: str = "^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+[.][a-zA-Z]{2,}$",
         term_frequency_adjustments_full: bool = False,
         include_exact_match_level: bool = True,
         include_username_match_level: bool = True,
+        include_username_fuzzy_level: bool = True,
         include_domain_match_level: bool = False,
         levenshtein_thresholds: int | list = [],
         damerau_levenshtein_thresholds: int | list = [],
         jaro_winkler_thresholds: float | list = [0.88],
         jaro_thresholds: float | list = [],
         m_probability_full_match: bool = None,
         m_probability_username_match: bool = None,
@@ -1426,14 +1427,16 @@
             term_frequency_adjustments_full (bool, optional): If True, apply
                 term frequency adjustments to the full email exact match level.
                 Defaults to False.
             include_exact_match_level (bool, optional): If True, include an exact
                 match on full email level. Defaults to True.
             include_username_match_level (bool, optional): If True, include an exact
                 match on username only level. Defaults to True.
+            include_username_fuzzy_level (bool, optional): If True, include a level
+                for fuzzy match on username. Defaults to True.
             include_domain_match_level (bool, optional): If True, include an exact
                 match on domain only level. Defaults to True.
             levenshtein_thresholds (Union[int, list], optional): The thresholds
                 to use for levenshtein similarity level(s).
                 Defaults to []
             damerau_levenshtein_thresholds (Union[int, list], optional): The thresholds
                 to use for damerau-levenshtein similarity level(s).
@@ -1604,63 +1607,64 @@
                 distance_threshold_or_thresholds=jaro_thresholds,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_email_jar,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         # Fuzzy match on username only
-        if len(levenshtein_thresholds) > 0:
-            threshold_levels = distance_threshold_comparison_levels(
-                self,
-                col_name,
-                regex_extract="^[^@]+",
-                distance_function_name="levenshtein",
-                distance_threshold_or_thresholds=levenshtein_thresholds,
-                m_probability_or_probabilities_thres=m_probability_or_probabilities_username_lev,
-                include_colname_in_charts_label=True,
-                manual_col_name_for_charts_label="Username",
-            )
-            comparison_levels = comparison_levels + threshold_levels
-
-        if len(damerau_levenshtein_thresholds) > 0:
-            threshold_levels = distance_threshold_comparison_levels(
-                self,
-                col_name,
-                regex_extract="^[^@]+",
-                distance_function_name="damerau-levenshtein",
-                distance_threshold_or_thresholds=damerau_levenshtein_thresholds,
-                m_probability_or_probabilities_thres=m_probability_or_probabilities_username_dl,
-                include_colname_in_charts_label=True,
-                manual_col_name_for_charts_label="Username",
-            )
-            comparison_levels = comparison_levels + threshold_levels
-
-        if len(jaro_winkler_thresholds) > 0:
-            threshold_levels = distance_threshold_comparison_levels(
-                self,
-                col_name,
-                regex_extract="^[^@]+",
-                distance_function_name="jaro-winkler",
-                distance_threshold_or_thresholds=jaro_winkler_thresholds,
-                m_probability_or_probabilities_thres=m_probability_or_probabilities_username_jw,
-                include_colname_in_charts_label=True,
-                manual_col_name_for_charts_label="Username",
-            )
-            comparison_levels = comparison_levels + threshold_levels
-
-        if len(jaro_thresholds) > 0:
-            threshold_levels = distance_threshold_comparison_levels(
-                self,
-                col_name,
-                distance_function_name="jaro",
-                distance_threshold_or_thresholds=jaro_thresholds,
-                m_probability_or_probabilities_thres=m_probability_or_probabilities_email_jar,
-                include_colname_in_charts_label=True,
-            )
-            comparison_levels = comparison_levels + threshold_levels
+        if include_username_fuzzy_level:
+            if len(levenshtein_thresholds) > 0:
+                threshold_levels = distance_threshold_comparison_levels(
+                    self,
+                    col_name,
+                    regex_extract="^[^@]+",
+                    distance_function_name="levenshtein",
+                    distance_threshold_or_thresholds=levenshtein_thresholds,
+                    m_probability_or_probabilities_thres=m_probability_or_probabilities_username_lev,
+                    include_colname_in_charts_label=True,
+                    manual_col_name_for_charts_label="Username",
+                )
+                comparison_levels = comparison_levels + threshold_levels
+
+            if len(damerau_levenshtein_thresholds) > 0:
+                threshold_levels = distance_threshold_comparison_levels(
+                    self,
+                    col_name,
+                    regex_extract="^[^@]+",
+                    distance_function_name="damerau-levenshtein",
+                    distance_threshold_or_thresholds=damerau_levenshtein_thresholds,
+                    m_probability_or_probabilities_thres=m_probability_or_probabilities_username_dl,
+                    include_colname_in_charts_label=True,
+                    manual_col_name_for_charts_label="Username",
+                )
+                comparison_levels = comparison_levels + threshold_levels
+
+            if len(jaro_winkler_thresholds) > 0:
+                threshold_levels = distance_threshold_comparison_levels(
+                    self,
+                    col_name,
+                    regex_extract="^[^@]+",
+                    distance_function_name="jaro-winkler",
+                    distance_threshold_or_thresholds=jaro_winkler_thresholds,
+                    m_probability_or_probabilities_thres=m_probability_or_probabilities_username_jw,
+                    include_colname_in_charts_label=True,
+                    manual_col_name_for_charts_label="Username",
+                )
+                comparison_levels = comparison_levels + threshold_levels
+
+            if len(jaro_thresholds) > 0:
+                threshold_levels = distance_threshold_comparison_levels(
+                    self,
+                    col_name,
+                    distance_function_name="jaro",
+                    distance_threshold_or_thresholds=jaro_thresholds,
+                    m_probability_or_probabilities_thres=m_probability_or_probabilities_email_jar,
+                    include_colname_in_charts_label=True,
+                )
+                comparison_levels = comparison_levels + threshold_levels
 
         # Domain-only match
 
         if include_domain_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
                 regex_extract="@([^@]+)$",
```

### Comparing `splink-3.9.4/splink/comparison_vector_distribution.py` & `splink-3.9.5/splink/comparison_vector_distribution.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/comparison_vector_values.py` & `splink-3.9.5/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/connected_components.py` & `splink-3.9.5/splink/connected_components.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/convert_v2_to_v3.py` & `splink-3.9.5/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/databricks/enable_splink.py` & `splink-3.9.5/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/default_from_jsonschema.py` & `splink-3.9.5/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/dialect_base.py` & `splink-3.9.5/splink/dialect_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_base.py` & `splink-3.9.5/splink/duckdb/duckdb_helpers/duckdb_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py` & `splink-3.9.5/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_helpers.py` & `splink-3.9.5/splink/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/duckdb/linker.py` & `splink-3.9.5/splink/duckdb/linker.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     duckdb_load_from_file,
     validate_duckdb_connection,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class DuckDBLinkerDataFrame(SplinkDataFrame):
+class DuckDBDataFrame(SplinkDataFrame):
     linker: DuckDBLinker
 
     @property
     def columns(self) -> list[InputColumn]:
         d = self.as_record_dict(1)[0]
 
         col_strings = list(d.keys())
@@ -200,30 +200,30 @@
                     CREATE SCHEMA IF NOT EXISTS {output_schema};
                     SET schema '{output_schema}';
                 """
             )
 
     def _table_to_splink_dataframe(
         self, templated_name, physical_name
-    ) -> DuckDBLinkerDataFrame:
-        return DuckDBLinkerDataFrame(templated_name, physical_name, self)
+    ) -> DuckDBDataFrame:
+        return DuckDBDataFrame(templated_name, physical_name, self)
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
         # In the case of a table already existing in the database,
         # execute sql is only reached if the user has explicitly turned off the cache
         self._delete_table_from_database(physical_name)
 
         sql = f"""
         CREATE TABLE {physical_name}
         AS
         ({sql})
         """
         self._log_and_run_sql_execution(sql, templated_name, physical_name)
 
-        return DuckDBLinkerDataFrame(templated_name, physical_name, self)
+        return DuckDBDataFrame(templated_name, physical_name, self)
 
     def _run_sql_execution(self, final_sql, templated_name, physical_name):
         self._con.execute(final_sql)
 
     def register_table(self, input, table_name, overwrite=False):
         # If the user has provided a table name, return it as a SplinkDataframe
         if isinstance(input, str):
```

### Comparing `splink-3.9.4/splink/em_training_session.py` & `splink-3.9.5/splink/em_training_session.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/estimate_u.py` & `splink-3.9.5/splink/estimate_u.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/expectation_maximisation.py` & `splink-3.9.5/splink/expectation_maximisation.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.9.5/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/comparator_score_chart.json` & `splink-3.9.5/splink/files/chart_defs/comparator_score_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/comparator_score_threshold_chart.json` & `splink-3.9.5/splink/files/chart_defs/comparator_score_threshold_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/completeness.json` & `splink-3.9.5/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.9.5/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.9.5/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.9.5/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.9.5/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/missingness.json` & `splink-3.9.5/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.9.5/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/phonetic_match_chart.json` & `splink-3.9.5/splink/files/chart_defs/phonetic_match_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/precision_recall.json` & `splink-3.9.5/splink/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-3.9.5/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/profile_data.json` & `splink-3.9.5/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/roc.json` & `splink-3.9.5/splink/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/tf_adjustment_chart.json` & `splink-3.9.5/splink/files/chart_defs/tf_adjustment_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.9.5/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/external_js/vega-embed@6.20.2` & `splink-3.9.5/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/external_js/vega-lite@5.2.0` & `splink-3.9.5/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/external_js/vega@5.21.0` & `splink-3.9.5/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/labelling_tool/slt.js` & `splink-3.9.5/splink/files/labelling_tool/slt.js`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/labelling_tool/template.j2` & `splink-3.9.5/splink/files/labelling_tool/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/settings_jsonschema.json` & `splink-3.9.5/splink/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.9.5/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.9.5/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-3.9.5/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.9.5/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/splink_cluster_studio/custom.css` & `splink-3.9.5/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/splink_comparison_viewer/custom.css` & `splink-3.9.5/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/splink_comparison_viewer/template.j2` & `splink-3.9.5/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.9.5/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/input_column.py` & `splink-3.9.5/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/labelling_tool.py` & `splink-3.9.5/splink/labelling_tool.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/linker.py` & `splink-3.9.5/splink/linker.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 from .connected_components import (
     _cc_create_unique_id_cols,
     solve_connected_components,
 )
 from .em_training_session import EMTrainingSession
 from .estimate_u import estimate_u_values
 from .exceptions import SplinkException
+from .find_matches_to_new_records import add_unique_id_and_source_dataset_cols_if_needed
 from .labelling_tool import (
     generate_labelling_tool_comparisons,
     render_labelling_tool_html,
 )
 from .logging_messages import execute_sql_logging_message_info, log_sql
 from .m_from_labels import estimate_m_from_pairwise_labels
 from .m_training import estimate_m_values_from_label_column
@@ -1284,77 +1285,77 @@
         are strict enough to generate only true links.
 
         Deterministic linkage, however, is likely to result in missed links
         (false negatives).
 
         Examples:
             === ":simple-duckdb: DuckDB"
-            ```py
-            from splink.duckdb.linker import DuckDBLinker
+                ```py
+                from splink.duckdb.linker import DuckDBLinker
 
-            settings = {
-                "link_type": "dedupe_only",
-                "blocking_rules_to_generate_predictions": [
-                    "l.first_name = r.first_name",
-                    "l.surname = r.surname",
-                ],
-                "comparisons": []
-            }
-            >>>
-            linker = DuckDBLinker(df, settings)
-            df = linker.deterministic_link()
-            ```
+                settings = {
+                    "link_type": "dedupe_only",
+                    "blocking_rules_to_generate_predictions": [
+                        "l.first_name = r.first_name",
+                        "l.surname = r.surname",
+                    ],
+                    "comparisons": []
+                }
+                >>>
+                linker = DuckDBLinker(df, settings)
+                df = linker.deterministic_link()
+                ```
             === ":simple-apachespark: Spark"
-            ```py
-            from splink.spark.linker import SparkLinker
+                ```py
+                from splink.spark.linker import SparkLinker
 
-            settings = {
-                "link_type": "dedupe_only",
-                "blocking_rules_to_generate_predictions": [
-                    "l.first_name = r.first_name",
-                    "l.surname = r.surname",
-                ],
-                "comparisons": []
-            }
-            >>>
-            linker = SparkLinker(df, settings)
-            df = linker.deterministic_link()
-            ```
+                settings = {
+                    "link_type": "dedupe_only",
+                    "blocking_rules_to_generate_predictions": [
+                        "l.first_name = r.first_name",
+                        "l.surname = r.surname",
+                    ],
+                    "comparisons": []
+                }
+                >>>
+                linker = SparkLinker(df, settings)
+                df = linker.deterministic_link()
+                ```
             === ":simple-amazonaws: Athena"
-            ```py
-            from splink.athena.linker import AthenaLinker
+                ```py
+                from splink.athena.linker import AthenaLinker
 
-            settings = {
-                "link_type": "dedupe_only",
-                "blocking_rules_to_generate_predictions": [
-                    "l.first_name = r.first_name",
-                    "l.surname = r.surname",
-                ],
-                "comparisons": []
-            }
-            >>>
-            linker = AthenaLinker(df, settings)
-            df = linker.deterministic_link()
-            ```
+                settings = {
+                    "link_type": "dedupe_only",
+                    "blocking_rules_to_generate_predictions": [
+                        "l.first_name = r.first_name",
+                        "l.surname = r.surname",
+                    ],
+                    "comparisons": []
+                }
+                >>>
+                linker = AthenaLinker(df, settings)
+                df = linker.deterministic_link()
+                ```
             === ":simple-sqlite: SQLite"
-            ```py
-            from splink.sqlite.linker import SQLiteLinker
+                ```py
+                from splink.sqlite.linker import SQLiteLinker
 
-            settings = {
-                "link_type": "dedupe_only",
-                "blocking_rules_to_generate_predictions": [
-                    "l.first_name = r.first_name",
-                    "l.surname = r.surname",
-                ],
-                "comparisons": []
-            }
-            >>>
-            linker = SQLiteLinker(df, settings)
-            df = linker.deterministic_link()
-            ```
+                settings = {
+                    "link_type": "dedupe_only",
+                    "blocking_rules_to_generate_predictions": [
+                        "l.first_name = r.first_name",
+                        "l.surname = r.surname",
+                    ],
+                    "comparisons": []
+                }
+                >>>
+                linker = SQLiteLinker(df, settings)
+                df = linker.deterministic_link()
+                ```
 
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons.  This
                 represents a table materialised in the database. Methods on the
                 SplinkDataFrame allow you to access the underlying data.
         """
 
@@ -1771,18 +1772,22 @@
             self.register_table(
                 records_or_tablename, new_records_tablename, overwrite=True
             )
 
         else:
             new_records_tablename = records_or_tablename
 
+        new_records_df = self._table_to_splink_dataframe(
+            "__splink__df_new_records", new_records_tablename
+        )
+
         cache = self._intermediate_table_cache
         input_dfs = []
-        # If our df_concat_with_tf table already exists, use backwards inference to
-        # find all underlying term frequency tables.
+        # If our df_concat_with_tf table already exists, derive the term frequency
+        # tables from df_concat_with_tf rather than computing them
         if "__splink__df_concat_with_tf" in cache:
             concat_with_tf = cache["__splink__df_concat_with_tf"]
             tf_tables = compute_term_frequencies_from_concat_with_tf(self)
             # This queues up our tf tables, rather materialising them
             for tf in tf_tables:
                 # if tf is a SplinkDataFrame, then the table already exists
                 if isinstance(tf, SplinkDataFrame):
@@ -1802,15 +1807,17 @@
 
         self._settings_obj._blocking_rules_to_generate_predictions = blocking_rules
 
         self._find_new_matches_mode = True
 
         sql = _join_tf_to_input_df_sql(self)
         sql = sql.replace("__splink__df_concat", new_records_tablename)
-        self._enqueue_sql(sql, "__splink__df_new_records_with_tf")
+        self._enqueue_sql(sql, "__splink__df_new_records_with_tf_before_uid_fix")
+
+        add_unique_id_and_source_dataset_cols_if_needed(self, new_records_df)
 
         sql = block_using_rules_sql(self)
         self._enqueue_sql(sql, "__splink__df_blocked")
 
         sql = compute_comparison_vector_values_sql(self._settings_obj)
         self._enqueue_sql(sql, "__splink__df_comparison_vectors")
 
@@ -2523,15 +2530,16 @@
                 the title of the output chart.
             as_dict (bool, optional): If True, return a dict version of the chart.
 
         Examples:
             For the simplest code pipeline, load a pre-trained model
             and run this against the test data.
             ```py
-            df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
+            from splink.datasets import splink_datasets
+            df = splink_datasets.fake_1000
             linker = DuckDBLinker(df)
             linker.load_settings("saved_settings.json")
             linker.unlinkables_chart()
             ```
             For more complex code pipelines, you can run an entire pipeline
             that estimates your m and u values, before `unlinkables_chart().
```

### Comparing `splink-3.9.4/splink/lower_id_on_lhs.py` & `splink-3.9.5/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/m_from_labels.py` & `splink-3.9.5/splink/m_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/m_training.py` & `splink-3.9.5/splink/m_training.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/m_u_records_to_parameters.py` & `splink-3.9.5/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/match_key_analysis.py` & `splink-3.9.5/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/match_weights_histogram.py` & `splink-3.9.5/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/misc.py` & `splink-3.9.5/splink/misc.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/missingness.py` & `splink-3.9.5/splink/missingness.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/parse_sql.py` & `splink-3.9.5/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/pipeline.py` & `splink-3.9.5/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/postgres/linker.py` & `splink-3.9.5/splink/postgres/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/postgres/postgres_helpers/postgres_base.py` & `splink-3.9.5/splink/postgres/postgres_helpers/postgres_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/postgres/postgres_helpers/postgres_comparison_imports.py` & `splink-3.9.5/splink/postgres/postgres_helpers/postgres_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/predict.py` & `splink-3.9.5/splink/predict.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/profile_data.py` & `splink-3.9.5/splink/profile_data.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/settings.py` & `splink-3.9.5/splink/settings.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/settings_validator.py` & `splink-3.9.5/splink/settings_validator.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/spark/linker.py` & `splink-3.9.5/splink/spark/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .spark_helpers.custom_spark_dialect import Dialect
 
 logger = logging.getLogger(__name__)
 
 Dialect["customspark"]
 
 
-class SparkDataframe(SplinkDataFrame):
+class SparkDataFrame(SplinkDataFrame):
     linker: SparkLinker
 
     @property
     def columns(self) -> list[InputColumn]:
         sql = f"select * from {self.physical_name} limit 1"
         spark_df = self.linker.spark.sql(sql)
 
@@ -303,15 +303,15 @@
                 "You can find the location of the jar by calling the following function"
                 ":\nfrom splink.spark.jar_location import similarity_jar_location"
                 "\n\nFull error:\n"
                 f"{e}"
             )
 
     def _table_to_splink_dataframe(self, templated_name, physical_name):
-        return SparkDataframe(templated_name, physical_name, self)
+        return SparkDataFrame(templated_name, physical_name, self)
 
     def _repartition_if_needed(self, spark_df, templated_name):
         # Repartitioning has two effects:
         # 1. When we persist out results to disk, it results in a predictable
         #    number of output files.  Some splink operations result in a very large
         #    number of output files, so this reduces the number of files and therefore
         #    avoids slow reads and writes
```

### Comparing `splink-3.9.4/splink/spark/spark_helpers/custom_spark_dialect.py` & `splink-3.9.5/splink/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/spark/spark_helpers/spark_base.py` & `splink-3.9.5/splink/spark/spark_helpers/spark_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/spark/spark_helpers/spark_comparison_imports.py` & `splink-3.9.5/splink/spark/spark_helpers/spark_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/splink_comparison_viewer.py` & `splink-3.9.5/splink/splink_comparison_viewer.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/sql_transform.py` & `splink-3.9.5/splink/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/sqlite/linker.py` & `splink-3.9.5/splink/sqlite/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py` & `splink-3.9.5/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/term_frequencies.py` & `splink-3.9.5/splink/term_frequencies.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/unique_id_concat.py` & `splink-3.9.5/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/unlinkables.py` & `splink-3.9.5/splink/unlinkables.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/validate_jsonschema.py` & `splink-3.9.5/splink/validate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/vertically_concatenate.py` & `splink-3.9.5/splink/vertically_concatenate.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/splink/waterfall_chart.py` & `splink-3.9.5/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.4/PKG-INFO` & `splink-3.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.9.4
+Version: 3.9.5
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -68,15 +68,15 @@
 
 High correlation occurs when the value of a column is highly constrained (predictable) from the value of another column. For example, a 'city' field is almost perfectly correlated with 'postcode'. Gender is highly correlated with 'first name'. Correlation is particularly problematic if **all** of your input columns are highly correlated.
 
 Splink is not designed for linking a single column containing a 'bag of words'. For example, a table with a single 'company name' column, and no other details.
 
 ## Documentation
 
-The homepage for the Splink documentation can be found [here](https://moj-analytical-services.github.io/splink/). Interactive demos can be found [here](https://github.com/moj-analytical-services/splink_demos/tree/splink3_demos), or by clicking the following Binder link:
+The homepage for the Splink documentation can be found [here](https://moj-analytical-services.github.io/splink/). Interactive demos can be found [here](https://github.com/moj-analytical-services/splink/tree/master/docs/demos), or by clicking the following Binder link:
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/moj-analytical-services/splink_demos/master?urlpath=lab)
 
 The specification of the Fellegi Sunter statistical model behind `splink` is similar as that used in the R [fastLink package](https://github.com/kosukeimai/fastLink). Accompanying the fastLink package is an [academic paper](http://imai.fas.harvard.edu/research/files/linkage.pdf) that describes this model. The [Splink documentation site](https://moj-analytical-services.github.io/splink/topic_guides/fellegi_sunter.html) and a [series of interactive articles](https://www.robinlinacre.com/probabilistic_linkage/) also explores the theory behind Splink.
 
 The Office for National Statistics have written a [case study about using Splink](https://github.com/Data-Linkage/Splink-census-linkage/blob/main/SplinkCaseStudy.pdf) to link 2021 Census data to itself.
 
@@ -119,15 +119,15 @@
         brl.exact_match_rule("surname"),
     ],
     "comparisons": [
         ctl.name_comparison("first_name"),
         ctl.name_comparison("surname"),
         ctl.date_comparison("dob", cast_strings_to_date=True),
         cl.exact_match("city", term_frequency_adjustments=True),
-        ctl.email_comparison("email"),
+        ctl.email_comparison("email", include_username_fuzzy_level=False),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
 blocking_rule_for_training = brl.and_(
@@ -185,7 +185,16 @@
 
 ## Acknowledgements
 
 We are very grateful to [ADR UK](https://www.adruk.org/) (Administrative Data Research UK) for providing the initial funding for this work as part of the [Data First](https://www.adruk.org/our-work/browse-all-projects/data-first-harnessing-the-potential-of-linked-administrative-data-for-the-justice-system-169/) project.
 
 We are extremely grateful to professors Katie Harron, James Doidge and Peter Christen for their expert advice and guidance in the development of Splink. We are also very grateful to colleagues at the UK's Office for National Statistics for their expert advice and peer review of this work. Any errors remain our own.
 
+## Related Repositories
+
+While Splink is a standalone package, there are a number of repositories in the Splink ecosystem:
+
+- [splink_demos](https://github.com/moj-analytical-services/splink_demos) contains a copy of the Splink tutorial and example notebooks that are hosted via [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/moj-analytical-services/splink_demos/master?urlpath=lab)
+- [splink_scalaudfs](https://github.com/moj-analytical-services/splink_scalaudfs) contains the code to generate [User Defined Functions](https://moj-analytical-services.github.io/splink/dev_guides/udfs.html#spark) in scala which are then callable in Spark.
+- [splink_datasets](https://github.com/moj-analytical-services/splink_datasets) contains datasets that can be installed automatically as a part of Splink through the [In-build datasets](https://moj-analytical-services.github.io/splink/datasets.html) functionality.
+- [splink_synthetic_data] contains code to generate synthetic data.
+
```

