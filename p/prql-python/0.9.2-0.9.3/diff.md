# Comparing `tmp/prql_python-0.9.2.tar.gz` & `tmp/prql_python-0.9.3.tar.gz`

## Comparing `prql_python-0.9.2.tar` & `prql_python-0.9.3.tar`

### file list

```diff
@@ -1,183 +1,184 @@
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 prql_python-0.9.2/local_dependencies/prql-ast/Cargo.toml
--rw-r--r--   0     1001      123     1452 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/generic.rs
--rw-r--r--   0     1001      123     4890 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ident.rs
--rw-r--r--   0     1001      123      654 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/literal.rs
--rw-r--r--   0     1001      123     1214 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ops.rs
--rw-r--r--   0     1001      123     3390 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr.rs
--rw-r--r--   0     1001      123       59 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/lib.rs
--rw-r--r--   0     1001      123     2571 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/span.rs
--rw-r--r--   0     1001      123     1552 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/stmt.rs
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 prql_python-0.9.2/local_dependencies/prql-parser/Cargo.toml
--rw-r--r--   0     1001      123    13388 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/expr.rs
--rw-r--r--   0     1001      123     1916 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/interpolation.rs
--rw-r--r--   0     1001      123    11984 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/lexer.rs
--rw-r--r--   0     1001      123    63208 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/lib.rs
--rw-r--r--   0     1001      123     5385 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap
--rw-r--r--   0     1001      123     1110 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/span.rs
--rw-r--r--   0     1001      123     5411 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/stmt.rs
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 prql_python-0.9.2/local_dependencies/prql-compiler/Cargo.toml
--rw-r--r--   0     1001      123     2691 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/ARCHITECTURE.md
--rw-r--r--   0     1001      123      869 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/README.md
--rw-r--r--   0     1001      123     1223 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/benches/bench.rs
--rw-r--r--   0     1001      123    15010 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/ast.rs
--rw-r--r--   0     1001      123     2729 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/literal.rs
--rw-r--r--   0     1001      123     4411 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/mod.rs
--rw-r--r--   0     1001      123     3017 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/pl.rs
--rw-r--r--   0     1001      123    12249 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/error.rs
--rw-r--r--   0     1001      123     1114 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/generic.rs
--rw-r--r--   0     1001      123      143 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/mod.rs
--rw-r--r--   0     1001      123     4957 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/expr.rs
--rw-r--r--   0     1001      123     3897 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs
--rw-r--r--   0     1001      123       28 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/mod.rs
--rw-r--r--   0     1001      123      568 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs
--rw-r--r--   0     1001      123    10962 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/fold.rs
--rw-r--r--   0     1001      123     2632 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/lineage.rs
--rw-r--r--   0     1001      123     3840 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/mod.rs
--rw-r--r--   0     1001      123     1386 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/stmt.rs
--rw-r--r--   0     1001      123     6176 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/types.rs
--rw-r--r--   0     1001      123      418 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/utils.rs
--rw-r--r--   0     1001      123     1508 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/expr.rs
--rw-r--r--   0     1001      123     8954 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/fold.rs
--rw-r--r--   0     1001      123      874 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/ids.rs
--rw-r--r--   0     1001      123     2371 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/mod.rs
--rw-r--r--   0     1001      123     1530 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/transform.rs
--rw-r--r--   0     1001      123      683 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/utils.rs
--rw-r--r--   0     1001      123    12931 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/lib.rs
--rw-r--r--   0     1001      123     8442 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/parser.rs
--rw-r--r--   0     1001      123    10998 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/ast_expand.rs
--rw-r--r--   0     1001      123     6064 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/context.rs
--rw-r--r--   0     1001      123    17337 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/eval/mod.rs
--rw-r--r--   0     1001      123    36124 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/lowering.rs
--rw-r--r--   0     1001      123     9621 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/mod.rs
--rw-r--r--   0     1001      123    15641 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/module.rs
--rw-r--r--   0     1001      123     7472 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/reporting.rs
--rw-r--r--   0     1001      123    12386 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs
--rw-r--r--   0     1001      123     5455 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs
--rw-r--r--   0     1001      123    40705 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs
--rw-r--r--   0     1001      123      478 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-2.snap
--rw-r--r--   0     1001      123      806 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap
--rw-r--r--   0     1001      123      694 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap
--rw-r--r--   0     1001      123     1956 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap
--rw-r--r--   0     1001      123     2976 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap
--rw-r--r--   0     1001      123     2356 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap
--rw-r--r--   0     1001      123      654 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap
--rw-r--r--   0     1001      123     2672 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap
--rw-r--r--   0     1001      123     3639 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap
--rw-r--r--   0     1001      123     5367 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap
--rw-r--r--   0     1001      123    36088 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs
--rw-r--r--   0     1001      123    12039 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs
--rw-r--r--   0     1001      123     4165 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/static_analysis.rs
--rw-r--r--   0     1001      123     6208 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/std.prql
--rw-r--r--   0     1001      123    10042 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/dialect.rs
--rw-r--r--   0     1001      123    35825 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_expr.rs
--rw-r--r--   0     1001      123     7284 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_projection.rs
--rw-r--r--   0     1001      123    21640 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_query.rs
--rw-r--r--   0     1001      123     3127 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/keywords.rs
--rw-r--r--   0     1001      123     4566 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/mod.rs
--rw-r--r--   0     1001      123     5176 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/operators.rs
--rw-r--r--   0     1001      123    20817 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/anchor.rs
--rw-r--r--   0     1001      123     7166 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/ast.rs
--rw-r--r--   0     1001      123    10595 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/context.rs
--rw-r--r--   0     1001      123     9660 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs
--rw-r--r--   0     1001      123     2188 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/mod.rs
--rw-r--r--   0     1001      123     7101 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs
--rw-r--r--   0     1001      123    20042 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs
--rw-r--r--   0     1001      123     5461 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/std.sql.prql
--rw-r--r--   0     1001      123       88 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/mod.rs
--rw-r--r--   0     1001      123    75720 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test.rs
--rw-r--r--   0     1001      123     4090 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs
--rw-r--r--   0     1001      123     6630 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_error_messages.rs
--rw-r--r--   0     1001      123     1912 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/id_gen.rs
--rw-r--r--   0     1001      123     3180 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/mod.rs
--rw-r--r--   0     1001      123     3892 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/toposort.rs
--rw-r--r--   0     1001      123     1612 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/README.md
--rw-r--r--   0     1001      123    10021 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/connection.rs
--rw-r--r--   0     1001      123    10818 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv
--rw-r--r--   0     1001      123     7017 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv
--rw-r--r--   0     1001      123     6743 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv
--rw-r--r--   0     1001      123     1690 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv
--rw-r--r--   0     1001      123      329 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/genres.csv
--rw-r--r--   0     1001      123    44678 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv
--rw-r--r--   0     1001      123    35719 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv
--rw-r--r--   0     1001      123      138 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/media_types.csv
--rw-r--r--   0     1001      123    58709 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv
--rw-r--r--   0     1001      123      299 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/playlists.csv
--rw-r--r--   0     1001      123     2193 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql
--rw-r--r--   0     1001      123   241743 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv
--rw-r--r--   0     1001      123     2076 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/docker-compose.yml
--rw-r--r--   0     1001      123    14665 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/main.rs
--rw-r--r--   0     1001      123      188 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/aggregation.prql
--rw-r--r--   0     1001      123      813 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql
--rw-r--r--   0     1001      123      106 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/cast.prql
--rw-r--r--   0     1001      123       66 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/constants_only.prql
--rw-r--r--   0     1001      123       91 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/distinct.prql
--rw-r--r--   0     1001      123      160 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/distinct_on.prql
--rw-r--r--   0     1001      123      231 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/genre_counts.prql
--rw-r--r--   0     1001      123      148 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/group_all.prql
--rw-r--r--   0     1001      123      151 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/group_sort.prql
--rw-r--r--   0     1001      123      718 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql
--rw-r--r--   0     1001      123      143 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/loop.prql
--rw-r--r--   0     1001      123      298 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/pipelines.prql
--rw-r--r--   0     1001      123      246 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/set_ops_remove.prql
--rw-r--r--   0     1001      123      272 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/sort.prql
--rw-r--r--   0     1001      123      179 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/switch.prql
--rw-r--r--   0     1001      123      481 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/window.prql
--rw-r--r--   0     1001      123      450 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@aggregation.prql.snap
--rw-r--r--   0     1001      123     1806 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap
--rw-r--r--   0     1001      123      317 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@cast.prql.snap
--rw-r--r--   0     1001      123      282 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@constants_only.prql.snap
--rw-r--r--   0     1001      123      298 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct.prql.snap
--rw-r--r--   0     1001      123      457 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct_on.prql.snap
--rw-r--r--   0     1001      123      493 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@genre_counts.prql.snap
--rw-r--r--   0     1001      123      428 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_all.prql.snap
--rw-r--r--   0     1001      123      403 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_sort.prql.snap
--rw-r--r--   0     1001      123     1518 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      426 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@loop.prql.snap
--rw-r--r--   0     1001      123      654 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap
--rw-r--r--   0     1001      123      660 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      609 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap
--rw-r--r--   0     1001      123      471 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@switch.prql.snap
--rw-r--r--   0     1001      123      895 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap
--rw-r--r--   0     1001      123      301 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@aggregation.prql.snap
--rw-r--r--   0     1001      123     1185 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap
--rw-r--r--   0     1001      123      775 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap
--rw-r--r--   0     1001      123      245 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@constants_only.prql.snap
--rw-r--r--   0     1001      123     2389 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap
--rw-r--r--   0     1001      123      640 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap
--rw-r--r--   0     1001      123      261 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@genre_counts.prql.snap
--rw-r--r--   0     1001      123      632 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap
--rw-r--r--   0     1001      123      347 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_sort.prql.snap
--rw-r--r--   0     1001      123     1721 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      366 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@loop.prql.snap
--rw-r--r--   0     1001      123     1177 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap
--rw-r--r--   0     1001      123      389 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      571 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap
--rw-r--r--   0     1001      123      438 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@switch.prql.snap
--rw-r--r--   0     1001      123     1020 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap
--rw-r--r--   0     1001      123      525 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap
--rw-r--r--   0     1001      123     2369 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap
--rw-r--r--   0     1001      123      440 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@cast.prql.snap
--rw-r--r--   0     1001      123      417 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@constants_only.prql.snap
--rw-r--r--   0     1001      123      380 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct.prql.snap
--rw-r--r--   0     1001      123      715 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap
--rw-r--r--   0     1001      123      503 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@genre_counts.prql.snap
--rw-r--r--   0     1001      123      615 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap
--rw-r--r--   0     1001      123      616 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap
--rw-r--r--   0     1001      123     1741 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      582 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap
--rw-r--r--   0     1001      123      872 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap
--rw-r--r--   0     1001      123      752 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      755 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap
--rw-r--r--   0     1001      123      622 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap
--rw-r--r--   0     1001      123     1314 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 prql_python-0.9.2/Cargo.toml
--rw-r--r--   0     1001      123      647 2023-07-25 21:04:44.000000 prql_python-0.9.2/.gitignore
--rw-r--r--   0     1001      123      889 2023-07-25 21:04:44.000000 prql_python-0.9.2/README.md
--rw-r--r--   0     1001      123      257 2023-07-25 21:04:44.000000 prql_python-0.9.2/build.rs
--rw-r--r--   0     1001      123      974 2023-07-25 21:04:44.000000 prql_python-0.9.2/noxfile.py
--rw-r--r--   0     1001      123      482 2023-07-25 21:04:44.000000 prql_python-0.9.2/prql_python.pyi
--rw-r--r--   0     1001      123     1007 2023-07-25 21:04:44.000000 prql_python-0.9.2/pyproject.toml
--rw-r--r--   0     1001      123     2019 2023-07-25 21:04:44.000000 prql_python-0.9.2/python/tests/test_all.py
--rw-r--r--   0     1001      123       56 2023-07-25 21:04:44.000000 prql_python-0.9.2/requirements.txt
--rw-r--r--   0     1001      123     4104 2023-07-25 21:04:44.000000 prql_python-0.9.2/src/lib.rs
--rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 prql_python-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 prql_python-0.9.3/local_dependencies/prql-ast/Cargo.toml
+-rw-r--r--   0     1001      123     1800 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/expr/generic.rs
+-rw-r--r--   0     1001      123     4890 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/expr/ident.rs
+-rw-r--r--   0     1001      123      654 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/expr/literal.rs
+-rw-r--r--   0     1001      123     1214 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/expr/ops.rs
+-rw-r--r--   0     1001      123     3390 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/expr.rs
+-rw-r--r--   0     1001      123       59 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/lib.rs
+-rw-r--r--   0     1001      123     2571 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/span.rs
+-rw-r--r--   0     1001      123     1552 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-ast/src/stmt.rs
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 prql_python-0.9.3/local_dependencies/prql-parser/Cargo.toml
+-rw-r--r--   0     1001      123    13388 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-parser/src/expr.rs
+-rw-r--r--   0     1001      123     1916 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-parser/src/interpolation.rs
+-rw-r--r--   0     1001      123    11984 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-parser/src/lexer.rs
+-rw-r--r--   0     1001      123    63208 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-parser/src/lib.rs
+-rw-r--r--   0     1001      123     5385 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap
+-rw-r--r--   0     1001      123     1110 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-parser/src/span.rs
+-rw-r--r--   0     1001      123     5411 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-parser/src/stmt.rs
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 prql_python-0.9.3/local_dependencies/prql-compiler/Cargo.toml
+-rw-r--r--   0     1001      123     2691 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/ARCHITECTURE.md
+-rw-r--r--   0     1001      123      869 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/README.md
+-rw-r--r--   0     1001      123     1223 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/benches/bench.rs
+-rw-r--r--   0     1001      123    15010 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/ast.rs
+-rw-r--r--   0     1001      123     2729 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/literal.rs
+-rw-r--r--   0     1001      123     4411 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/mod.rs
+-rw-r--r--   0     1001      123     3017 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/pl.rs
+-rw-r--r--   0     1001      123    12249 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/error.rs
+-rw-r--r--   0     1001      123     1114 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/generic.rs
+-rw-r--r--   0     1001      123      143 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/mod.rs
+-rw-r--r--   0     1001      123     4280 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/expr.rs
+-rw-r--r--   0     1001      123     3897 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs
+-rw-r--r--   0     1001      123       28 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/extra/mod.rs
+-rw-r--r--   0     1001      123      568 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs
+-rw-r--r--   0     1001      123    10270 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/fold.rs
+-rw-r--r--   0     1001      123     2632 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/lineage.rs
+-rw-r--r--   0     1001      123     3831 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/mod.rs
+-rw-r--r--   0     1001      123     1386 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/stmt.rs
+-rw-r--r--   0     1001      123     6176 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/types.rs
+-rw-r--r--   0     1001      123      584 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/utils.rs
+-rw-r--r--   0     1001      123     1508 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/expr.rs
+-rw-r--r--   0     1001      123     9015 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/fold.rs
+-rw-r--r--   0     1001      123      874 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/ids.rs
+-rw-r--r--   0     1001      123     2381 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/mod.rs
+-rw-r--r--   0     1001      123     1530 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/transform.rs
+-rw-r--r--   0     1001      123      683 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/utils.rs
+-rw-r--r--   0     1001      123    13060 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/lib.rs
+-rw-r--r--   0     1001      123     8442 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/parser.rs
+-rw-r--r--   0     1001      123    13587 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/ast_expand.rs
+-rw-r--r--   0     1001      123     3671 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/decl.rs
+-rw-r--r--   0     1001      123    16427 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/eval/mod.rs
+-rw-r--r--   0     1001      123    35989 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/lowering.rs
+-rw-r--r--   0     1001      123     9698 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/mod.rs
+-rw-r--r--   0     1001      123    15638 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/module.rs
+-rw-r--r--   0     1001      123     7478 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/reporting.rs
+-rw-r--r--   0     1001      123     5455 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs
+-rw-r--r--   0     1001      123    39133 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs
+-rw-r--r--   0     1001      123    12389 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/root_module_impl.rs
+-rw-r--r--   0     1001      123      478 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-2.snap
+-rw-r--r--   0     1001      123      806 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap
+-rw-r--r--   0     1001      123      694 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap
+-rw-r--r--   0     1001      123     1956 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap
+-rw-r--r--   0     1001      123     2976 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap
+-rw-r--r--   0     1001      123     2356 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap
+-rw-r--r--   0     1001      123      654 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap
+-rw-r--r--   0     1001      123     2672 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap
+-rw-r--r--   0     1001      123     3639 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap
+-rw-r--r--   0     1001      123     5367 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap
+-rw-r--r--   0     1001      123    35660 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs
+-rw-r--r--   0     1001      123    12015 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs
+-rw-r--r--   0     1001      123     2640 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/root_module.rs
+-rw-r--r--   0     1001      123     4165 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/static_analysis.rs
+-rw-r--r--   0     1001      123     6169 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/std.prql
+-rw-r--r--   0     1001      123    10042 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/dialect.rs
+-rw-r--r--   0     1001      123    35825 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/gen_expr.rs
+-rw-r--r--   0     1001      123     7284 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/gen_projection.rs
+-rw-r--r--   0     1001      123    21660 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/gen_query.rs
+-rw-r--r--   0     1001      123     3127 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/keywords.rs
+-rw-r--r--   0     1001      123     4626 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/mod.rs
+-rw-r--r--   0     1001      123     5176 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/operators.rs
+-rw-r--r--   0     1001      123    20817 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/anchor.rs
+-rw-r--r--   0     1001      123     7166 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/ast.rs
+-rw-r--r--   0     1001      123    10625 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/context.rs
+-rw-r--r--   0     1001      123     9680 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs
+-rw-r--r--   0     1001      123     2188 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/mod.rs
+-rw-r--r--   0     1001      123     7101 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs
+-rw-r--r--   0     1001      123    20042 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs
+-rw-r--r--   0     1001      123     5461 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/std.sql.prql
+-rw-r--r--   0     1001      123       88 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/tests/mod.rs
+-rw-r--r--   0     1001      123    75720 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/tests/test.rs
+-rw-r--r--   0     1001      123     4929 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs
+-rw-r--r--   0     1001      123     7307 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/tests/test_error_messages.rs
+-rw-r--r--   0     1001      123     1942 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/utils/id_gen.rs
+-rw-r--r--   0     1001      123     3180 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/utils/mod.rs
+-rw-r--r--   0     1001      123     3892 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/src/utils/toposort.rs
+-rw-r--r--   0     1001      123     1612 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/README.md
+-rw-r--r--   0     1001      123    10021 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/connection.rs
+-rw-r--r--   0     1001      123    10818 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv
+-rw-r--r--   0     1001      123     7017 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv
+-rw-r--r--   0     1001      123     6743 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv
+-rw-r--r--   0     1001      123     1690 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv
+-rw-r--r--   0     1001      123      329 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/genres.csv
+-rw-r--r--   0     1001      123    44678 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv
+-rw-r--r--   0     1001      123    35719 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv
+-rw-r--r--   0     1001      123      138 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/media_types.csv
+-rw-r--r--   0     1001      123    58709 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv
+-rw-r--r--   0     1001      123      299 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/playlists.csv
+-rw-r--r--   0     1001      123     2193 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql
+-rw-r--r--   0     1001      123   241743 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv
+-rw-r--r--   0     1001      123     2076 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/docker-compose.yml
+-rw-r--r--   0     1001      123    14665 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/main.rs
+-rw-r--r--   0     1001      123      188 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/aggregation.prql
+-rw-r--r--   0     1001      123      813 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql
+-rw-r--r--   0     1001      123      106 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/cast.prql
+-rw-r--r--   0     1001      123       66 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/constants_only.prql
+-rw-r--r--   0     1001      123       91 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/distinct.prql
+-rw-r--r--   0     1001      123      160 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/distinct_on.prql
+-rw-r--r--   0     1001      123      231 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/genre_counts.prql
+-rw-r--r--   0     1001      123      148 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/group_all.prql
+-rw-r--r--   0     1001      123      151 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/group_sort.prql
+-rw-r--r--   0     1001      123      718 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql
+-rw-r--r--   0     1001      123      143 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/loop.prql
+-rw-r--r--   0     1001      123      298 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/pipelines.prql
+-rw-r--r--   0     1001      123      246 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/set_ops_remove.prql
+-rw-r--r--   0     1001      123      272 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/sort.prql
+-rw-r--r--   0     1001      123      179 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/switch.prql
+-rw-r--r--   0     1001      123      481 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/window.prql
+-rw-r--r--   0     1001      123      450 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@aggregation.prql.snap
+-rw-r--r--   0     1001      123     1806 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      317 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@cast.prql.snap
+-rw-r--r--   0     1001      123      282 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@constants_only.prql.snap
+-rw-r--r--   0     1001      123      298 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct.prql.snap
+-rw-r--r--   0     1001      123      457 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      493 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      428 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_all.prql.snap
+-rw-r--r--   0     1001      123      403 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1518 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      426 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@loop.prql.snap
+-rw-r--r--   0     1001      123      654 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap
+-rw-r--r--   0     1001      123      660 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      609 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap
+-rw-r--r--   0     1001      123      471 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@switch.prql.snap
+-rw-r--r--   0     1001      123      895 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap
+-rw-r--r--   0     1001      123      301 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@aggregation.prql.snap
+-rw-r--r--   0     1001      123     1185 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      775 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap
+-rw-r--r--   0     1001      123      245 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@constants_only.prql.snap
+-rw-r--r--   0     1001      123     2389 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap
+-rw-r--r--   0     1001      123      640 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      261 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      632 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap
+-rw-r--r--   0     1001      123      347 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1721 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      366 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@loop.prql.snap
+-rw-r--r--   0     1001      123     1177 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap
+-rw-r--r--   0     1001      123      389 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      571 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap
+-rw-r--r--   0     1001      123      438 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@switch.prql.snap
+-rw-r--r--   0     1001      123     1020 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap
+-rw-r--r--   0     1001      123      525 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap
+-rw-r--r--   0     1001      123     2369 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      440 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@cast.prql.snap
+-rw-r--r--   0     1001      123      417 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@constants_only.prql.snap
+-rw-r--r--   0     1001      123      380 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct.prql.snap
+-rw-r--r--   0     1001      123      715 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      503 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      615 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap
+-rw-r--r--   0     1001      123      616 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1741 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      582 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap
+-rw-r--r--   0     1001      123      872 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap
+-rw-r--r--   0     1001      123      752 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      755 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap
+-rw-r--r--   0     1001      123      622 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap
+-rw-r--r--   0     1001      123     1314 2023-08-02 18:48:36.000000 prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 prql_python-0.9.3/Cargo.toml
+-rw-r--r--   0     1001      123      647 2023-08-02 18:48:36.000000 prql_python-0.9.3/.gitignore
+-rw-r--r--   0     1001      123      889 2023-08-02 18:48:36.000000 prql_python-0.9.3/README.md
+-rw-r--r--   0     1001      123      257 2023-08-02 18:48:36.000000 prql_python-0.9.3/build.rs
+-rw-r--r--   0     1001      123      964 2023-08-02 18:48:36.000000 prql_python-0.9.3/noxfile.py
+-rw-r--r--   0     1001      123      482 2023-08-02 18:48:36.000000 prql_python-0.9.3/prql_python.pyi
+-rw-r--r--   0     1001      123     1007 2023-08-02 18:48:36.000000 prql_python-0.9.3/pyproject.toml
+-rw-r--r--   0     1001      123     2019 2023-08-02 18:48:36.000000 prql_python-0.9.3/python/tests/test_all.py
+-rw-r--r--   0     1001      123       56 2023-08-02 18:48:36.000000 prql_python-0.9.3/requirements.txt
+-rw-r--r--   0     1001      123     4104 2023-08-02 18:48:36.000000 prql_python-0.9.3/src/lib.rs
+-rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 prql_python-0.9.3/PKG-INFO
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/generic.rs` & `prql_python-0.9.3/local_dependencies/prql-ast/src/expr/generic.rs`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,24 @@
             Self::String(s) => InterpolateItem::String(s),
             Self::Expr { expr, format } => InterpolateItem::Expr {
                 expr: Box::new(f(*expr)),
                 format,
             },
         }
     }
+
+    pub fn try_map<U, E, F: Fn(T) -> Result<U, E>>(self, f: F) -> Result<InterpolateItem<U>, E> {
+        Ok(match self {
+            Self::String(s) => InterpolateItem::String(s),
+            Self::Expr { expr, format } => InterpolateItem::Expr {
+                expr: Box::new(f(*expr)?),
+                format,
+            },
+        })
+    }
 }
 
 #[derive(Debug, PartialEq, Eq, Clone, Serialize, Deserialize)]
 pub struct SwitchCase<T> {
     pub condition: T,
     pub value: T,
 }
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ident.rs` & `prql_python-0.9.3/local_dependencies/prql-ast/src/expr/ident.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/literal.rs` & `prql_python-0.9.3/local_dependencies/prql-ast/src/expr/literal.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ops.rs` & `prql_python-0.9.3/local_dependencies/prql-ast/src/expr/ops.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-ast/src/expr.rs` & `prql_python-0.9.3/local_dependencies/prql-ast/src/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-ast/src/span.rs` & `prql_python-0.9.3/local_dependencies/prql-ast/src/span.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-ast/src/stmt.rs` & `prql_python-0.9.3/local_dependencies/prql-ast/src/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/Cargo.toml` & `prql_python-0.9.3/local_dependencies/prql-parser/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 description = "A parser for the PRQL query language."
 name = "prql-parser"
 
 edition= "2021"
 license= "Apache-2.0"
 repository= "https://github.com/PRQL/prql"
 rust-version= "1.65.0"
-version= "0.9.2"
+version= "0.9.3"
+
+[lib]
+doctest = false
 
 [dependencies]
 itertools = "0.11.0"
-prql-ast = {path = "../prql-ast", version = "0.9.2" }
+prql-ast = {path = "../prql-ast", version = "0.9.3" }
 semver = {version = "1.0.14"}
 
 # Chumsky's default features have issues when running in wasm (though we only
 # see it when compiling on MacOS), so we only include features when running
 # outside wasm.
 [target.'cfg(not(target_family="wasm"))'.dependencies]
 chumsky = "0.9.2"
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/src/expr.rs` & `prql_python-0.9.3/local_dependencies/prql-parser/src/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/src/interpolation.rs` & `prql_python-0.9.3/local_dependencies/prql-parser/src/interpolation.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/src/lexer.rs` & `prql_python-0.9.3/local_dependencies/prql-parser/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/src/lib.rs` & `prql_python-0.9.3/local_dependencies/prql-parser/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap` & `prql_python-0.9.3/local_dependencies/prql-parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/src/span.rs` & `prql_python-0.9.3/local_dependencies/prql-parser/src/span.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-parser/src/stmt.rs` & `prql_python-0.9.3/local_dependencies/prql-parser/src/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/Cargo.toml` & `prql_python-0.9.3/local_dependencies/prql-compiler/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 description = "PRQL is a modern language for transforming data — a simple, powerful, pipelined SQL replacement."
 name = "prql-compiler"
 
 edition= "2021"
 license= "Apache-2.0"
 repository= "https://github.com/PRQL/prql"
 rust-version= "1.65.0"
-version= "0.9.2"
+version= "0.9.3"
 
 metadata.msrv = "1.65.0"
 
 [features]
 default = []
 # Technically tokio could be limited to external tests, but its types are in
 # signatures which would require lots of conditional compilation.
 test-dbs = ["duckdb", "rusqlite", "tokio"]
 test-dbs-external = ["chrono", "duckdb", "mysql", "pg_bigdecimal", "postgres", "rusqlite", "tiberius", "tokio", "tokio-util"]
 
 [dependencies]
-prql-ast = {path = "../prql-ast", version = "0.9.2" }
-prql-parser = {path = "../prql-parser", version = "0.9.2" }
+prql-ast = {path = "../prql-ast", version = "0.9.3" }
+prql-parser = {path = "../prql-parser", version = "0.9.3" }
 
 anstream = {version = "0.3.2", features = ["auto"]}
 anyhow = {version = "1.0.57", features = ["backtrace"]}
 ariadne = "0.3.0"
 csv = "1.2.0"
 enum-as-inner = "0.6.0"
 itertools = "0.11.0"
 log = "0.4.17"
 once_cell = "1.18.0"
 regex = "1.9.0"
 semver = {version = "1.0.14", features = ["serde"]}
 # We could put `serde` behind a feature if needed.
 serde = {version = "1.0.137", features = ["derive"]}
 serde_json = "1.0.81"
-sqlformat = "0.2.0"
+sqlformat = "0.2.1"
 sqlparser = {version = "0.36.0", features = ["serde"]}
 strum = {version = "0.25.0", features = ["std", "derive"]}
 strum_macros = "0.25.0"
 
 serde_yaml = {version = "0.9", optional = true}
 
 [target.'cfg(not(target_family="wasm"))'.dependencies]
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/ARCHITECTURE.md` & `prql_python-0.9.3/local_dependencies/prql-compiler/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/README.md` & `prql_python-0.9.3/local_dependencies/prql-compiler/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/benches/bench.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/ast.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/ast.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/literal.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/literal.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/pl.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/codegen/pl.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/error.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/error.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/generic.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/generic.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/expr.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/expr.rs`

 * *Files 12% similar despite different names*

```diff
@@ -64,21 +64,18 @@
 pub enum ExprKind {
     Ident(Ident),
     All {
         within: Ident,
         except: Vec<Expr>,
     },
     Literal(Literal),
-    Pipeline(Pipeline),
 
     Tuple(Vec<Expr>),
     Array(Vec<Expr>),
     Range(Range),
-    Binary(BinaryExpr),
-    Unary(UnaryExpr),
     FuncCall(FuncCall),
     Func(Box<Func>),
     TransformCall(TransformCall),
     SString(Vec<InterpolateItem>),
     FString(Vec<InterpolateItem>),
     Case(Vec<SwitchCase>),
     RqOperator {
@@ -92,27 +89,14 @@
     Param(String),
 
     /// When used instead of function body, the function will be translated to a RQ operator.
     /// Contains ident of the RQ operator.
     Internal(String),
 }
 
-#[derive(Debug, PartialEq, Clone, Serialize, Deserialize)]
-pub struct BinaryExpr {
-    pub left: Box<Expr>,
-    pub op: BinOp,
-    pub right: Box<Expr>,
-}
-
-#[derive(Debug, PartialEq, Clone, Serialize, Deserialize)]
-pub struct UnaryExpr {
-    pub op: UnOp,
-    pub expr: Box<Expr>,
-}
-
 /// Function call.
 #[derive(Debug, PartialEq, Clone, Serialize, Deserialize)]
 pub struct FuncCall {
     pub name: Box<Expr>,
     pub args: Vec<Expr>,
     #[serde(default, skip_serializing_if = "HashMap::is_empty")]
     pub named_args: HashMap<String, Expr>,
@@ -151,22 +135,10 @@
 
     #[serde(skip_serializing_if = "Option::is_none")]
     pub ty: Option<TyOrExpr>,
 
     pub default_value: Option<Box<Expr>>,
 }
 
-/// A value and a series of functions that are to be applied to that value one after another.
-#[derive(Debug, PartialEq, Clone, Serialize, Deserialize)]
-pub struct Pipeline {
-    pub exprs: Vec<Expr>,
-}
-
 pub type Range = generic::Range<Box<Expr>>;
 pub type InterpolateItem = generic::InterpolateItem<Expr>;
 pub type SwitchCase = generic::SwitchCase<Box<Expr>>;
-
-impl From<Vec<Expr>> for Pipeline {
-    fn from(nodes: Vec<Expr>) -> Self {
-        Pipeline { exprs: nodes }
-    }
-}
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/fold.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/fold.rs`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,14 @@
             name: ty_def.name,
             value: fold_optional_box(self, ty_def.value)?,
         })
     }
     fn fold_module_def(&mut self, module_def: ModuleDef) -> Result<ModuleDef> {
         fold_module_def(self, module_def)
     }
-    fn fold_pipeline(&mut self, pipeline: Pipeline) -> Result<Pipeline> {
-        fold_pipeline(self, pipeline)
-    }
     fn fold_func_call(&mut self, func_call: FuncCall) -> Result<FuncCall> {
         fold_func_call(self, func_call)
     }
     fn fold_transform_call(&mut self, transform_call: TransformCall) -> Result<TransformCall> {
         fold_transform_call(self, transform_call)
     }
     fn fold_func(&mut self, func: Func) -> Result<Func> {
@@ -75,27 +72,17 @@
     use ExprKind::*;
     Ok(match expr_kind {
         Ident(ident) => Ident(ident),
         All { within, except } => All {
             within,
             except: fold.fold_exprs(except)?,
         },
-        Binary(BinaryExpr { op, left, right }) => Binary(BinaryExpr {
-            op,
-            left: Box::new(fold.fold_expr(*left)?),
-            right: Box::new(fold.fold_expr(*right)?),
-        }),
-        Unary(UnaryExpr { op, expr }) => Unary(UnaryExpr {
-            op,
-            expr: Box::new(fold.fold_expr(*expr)?),
-        }),
         Tuple(items) => Tuple(fold.fold_exprs(items)?),
         Array(items) => Array(fold.fold_exprs(items)?),
         Range(range) => Range(fold_range(fold, range)?),
-        Pipeline(p) => Pipeline(fold.fold_pipeline(p)?),
         SString(items) => SString(
             items
                 .into_iter()
                 .map(|x| fold.fold_interpolate_item(x))
                 .try_collect()?,
         ),
         FString(items) => FString(
@@ -157,20 +144,14 @@
 pub fn fold_range<F: ?Sized + PlFold>(fold: &mut F, Range { start, end }: Range) -> Result<Range> {
     Ok(Range {
         start: fold_optional_box(fold, start)?,
         end: fold_optional_box(fold, end)?,
     })
 }
 
-pub fn fold_pipeline<T: ?Sized + PlFold>(fold: &mut T, pipeline: Pipeline) -> Result<Pipeline> {
-    Ok(Pipeline {
-        exprs: fold.fold_exprs(pipeline.exprs)?,
-    })
-}
-
 // This aren't strictly in the hierarchy, so we don't need to
 // have an assoc. function for `fold_optional_box` — we just
 // call out to the function in this module
 pub fn fold_optional_box<F: ?Sized + PlFold>(
     fold: &mut F,
     opt: Option<Box<Expr>>,
 ) -> Result<Option<Box<Expr>>> {
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/lineage.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/lineage.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 mod stmt;
 mod types;
 mod utils;
 
 use crate::generic::{SortDirection, WindowKind};
 use crate::ir::rq::TableRef;
 use crate::*;
-use crate::{ir::rq::Query, sql::internal::SqlTransform, SourceTree, Span};
+use crate::{ir::rq::RelationalQuery, sql::internal::SqlTransform, SourceTree, Span};
 
 pub use self::expr::*;
 pub use self::extra::expr::*;
 pub use self::fold::*;
 pub use self::lineage::*;
 pub use self::stmt::*;
 pub use self::types::*;
 pub use self::utils::*;
-pub use prql_ast::expr::{BinOp, Ident, Literal, UnOp, ValueAndUnit};
+pub use prql_ast::expr::{BinOp, BinaryExpr, Ident, Literal, UnOp, UnaryExpr, ValueAndUnit};
 
 pub fn print_mem_sizes() {
     use std::mem::size_of;
 
     println!("{:16}= {}", "Annotation", size_of::<Annotation>());
     println!("{:16}= {}", "BinaryExpr", size_of::<BinaryExpr>());
     println!("{:16}= {}", "BinOp", size_of::<BinOp>());
@@ -47,19 +47,18 @@
     println!("{:16}= {}", "FuncParam", size_of::<FuncParam>());
     println!("{:16}= {}", "InterpolateItem", size_of::<InterpolateItem>());
     println!("{:16}= {}", "JoinSide", size_of::<JoinSide>());
     println!("{:16}= {}", "Lineage", size_of::<Lineage>());
     println!("{:16}= {}", "LineageColumn", size_of::<LineageColumn>());
     println!("{:16}= {}", "LineageInput", size_of::<LineageInput>());
     println!("{:16}= {}", "ModuleDef", size_of::<ModuleDef>());
-    println!("{:16}= {}", "Pipeline", size_of::<Pipeline>());
     println!("{:16}= {}", "PrimitiveSet", size_of::<PrimitiveSet>());
-    println!("{:16}= {}", "Query", size_of::<Query>());
     println!("{:16}= {}", "QueryDef", size_of::<QueryDef>());
     println!("{:16}= {}", "Range", size_of::<Range>());
+    println!("{:16}= {}", "RelationalQuery", size_of::<RelationalQuery>());
     println!("{:16}= {}", "SortDirection", size_of::<SortDirection>());
     println!("{:16}= {}", "SourceTree", size_of::<SourceTree>());
     println!("{:16}= {}", "Span", size_of::<Span>());
     println!("{:16}= {}", "SqlTransform", size_of::<SqlTransform>());
     println!("{:16}= {}", "Stmt", size_of::<Stmt>());
     println!("{:16}= {}", "StmtKind", size_of::<StmtKind>());
     println!("{:16}= {}", "SwitchCase", size_of::<SwitchCase>());
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/stmt.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/types.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/pl/types.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/expr.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/fold.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/fold.rs`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     }
     fn fold_relation_kind(&mut self, rel_kind: RelationKind) -> Result<RelationKind> {
         fold_relation_kind(self, rel_kind)
     }
     fn fold_table_ref(&mut self, table_ref: TableRef) -> Result<TableRef> {
         fold_table_ref(self, table_ref)
     }
-    fn fold_query(&mut self, query: Query) -> Result<Query> {
+    fn fold_query(&mut self, query: RelationalQuery) -> Result<RelationalQuery> {
         fold_query(self, query)
     }
     fn fold_expr(&mut self, mut expr: Expr) -> Result<Expr> {
         expr.kind = self.fold_expr_kind(expr.kind)?;
         Ok(expr)
     }
     fn fold_expr_kind(&mut self, kind: ExprKind) -> Result<ExprKind> {
@@ -135,16 +135,19 @@
             .map(|(col, cid)| -> Result<_> {
                 Ok((fold.fold_relation_column(col)?, fold.fold_cid(cid)?))
             })
             .try_collect()?,
     })
 }
 
-pub fn fold_query<F: ?Sized + RqFold>(fold: &mut F, query: Query) -> Result<Query> {
-    Ok(Query {
+pub fn fold_query<F: ?Sized + RqFold>(
+    fold: &mut F,
+    query: RelationalQuery,
+) -> Result<RelationalQuery> {
+    Ok(RelationalQuery {
         def: query.def,
         relation: fold.fold_relation(query.relation)?,
         tables: query
             .tables
             .into_iter()
             .map(|t| fold.fold_table(t))
             .try_collect()?,
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/ids.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/ids.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 use expr::{InterpolateItem, Range, SwitchCase};
 use serde::{Deserialize, Serialize};
 
 use super::pl::Ident;
 use super::pl::{Literal, QueryDef};
 
 #[derive(Debug, PartialEq, Clone, Serialize, Deserialize)]
-pub struct Query {
+pub struct RelationalQuery {
     pub def: QueryDef,
 
     pub tables: Vec<TableDecl>,
     pub relation: Relation,
 }
 
 #[derive(Debug, PartialEq, Clone, Serialize, Deserialize)]
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/transform.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/transform.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/utils.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/ir/rq/utils.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/lib.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -224,27 +224,30 @@
             signature_comment: true,
             color: false,
         }
     }
 }
 
 impl Options {
-    pub fn no_format(mut self) -> Self {
-        self.format = false;
+    pub fn with_format(mut self, format: bool) -> Self {
+        self.format = format;
         self
     }
 
+    pub fn no_format(self) -> Self {
+        self.with_format(false)
+    }
+
     pub fn with_signature_comment(mut self, signature_comment: bool) -> Self {
         self.signature_comment = signature_comment;
         self
     }
 
-    pub fn no_signature(mut self) -> Self {
-        self.signature_comment = false;
-        self
+    pub fn no_signature(self) -> Self {
+        self.with_signature_comment(false)
     }
 
     pub fn with_target(mut self, target: Target) -> Self {
         self.target = target;
         self
     }
 
@@ -275,29 +278,29 @@
 ) -> Result<SourceTree<Vec<prql_ast::stmt::Stmt>>, ErrorMessages> {
     parser::parse(prql)
         .map_err(error::downcast)
         .map_err(|e| e.composed(prql))
 }
 
 /// Perform semantic analysis and convert PL to RQ.
-pub fn pl_to_rq(pl: Vec<prql_ast::stmt::Stmt>) -> Result<ir::rq::Query, ErrorMessages> {
+pub fn pl_to_rq(pl: Vec<prql_ast::stmt::Stmt>) -> Result<ir::rq::RelationalQuery, ErrorMessages> {
     let source_tree = SourceTree::single(PathBuf::new(), pl);
     semantic::resolve_and_lower(source_tree, &[]).map_err(error::downcast)
 }
 
 /// Perform semantic analysis and convert PL to RQ.
 pub fn pl_to_rq_tree(
     pl: SourceTree<Vec<prql_ast::stmt::Stmt>>,
     main_path: &[String],
-) -> Result<ir::rq::Query, ErrorMessages> {
+) -> Result<ir::rq::RelationalQuery, ErrorMessages> {
     semantic::resolve_and_lower(pl, main_path).map_err(error::downcast)
 }
 
 /// Generate SQL from RQ.
-pub fn rq_to_sql(rq: ir::rq::Query, options: &Options) -> Result<String, ErrorMessages> {
+pub fn rq_to_sql(rq: ir::rq::RelationalQuery, options: &Options) -> Result<String, ErrorMessages> {
     sql::compile(rq, options).map_err(error::downcast)
 }
 
 /// Generate PRQL code from PL AST
 pub fn pl_to_prql(pl: Vec<prql_ast::stmt::Stmt>) -> Result<String, ErrorMessages> {
     Ok(codegen::write_stmts(&pl))
 }
@@ -313,20 +316,20 @@
 
     /// JSON deserialization
     pub fn to_pl(json: &str) -> Result<Vec<prql_ast::stmt::Stmt>, ErrorMessages> {
         serde_json::from_str(json).map_err(|e| anyhow::anyhow!(e).into())
     }
 
     /// JSON serialization
-    pub fn from_rq(rq: ir::rq::Query) -> Result<String, ErrorMessages> {
+    pub fn from_rq(rq: ir::rq::RelationalQuery) -> Result<String, ErrorMessages> {
         serde_json::to_string(&rq).map_err(|e| anyhow::anyhow!(e).into())
     }
 
     /// JSON deserialization
-    pub fn to_rq(json: &str) -> Result<ir::rq::Query, ErrorMessages> {
+    pub fn to_rq(json: &str) -> Result<ir::rq::RelationalQuery, ErrorMessages> {
         serde_json::from_str(json).map_err(|e| anyhow::anyhow!(e).into())
     }
 }
 
 /// All paths are relative to the project root.
 #[derive(Debug, Clone, Default, Serialize)]
 pub struct SourceTree<T: Sized + Serialize = String> {
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/parser.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/parser.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/eval/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/eval/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 use std::iter::zip;
 
 use anyhow::Result;
 use itertools::Itertools;
 
 use crate::error::{Error, Span, WithErrorInfo};
-use crate::ir::pl::{Expr, ExprKind, Func, FuncCall, FuncParam, Ident, Literal, PlFold};
+use crate::ir::pl::{Expr, ExprKind, Func, FuncParam, Ident, Literal, PlFold};
 
 use super::ast_expand;
-use super::resolver::{binary_to_func_call, unary_to_func_call};
 
 pub fn eval(expr: prql_ast::expr::Expr) -> Result<Expr> {
-    let expr = ast_expand::expand_expr(expr);
+    let expr = ast_expand::expand_expr(expr)?;
 
     Evaluator::new().fold_expr(expr)
 }
 
 /// Converts an expression to a value
 ///
 /// Serves as a working draft of PRQL semantics definition.
@@ -40,24 +39,14 @@
             ExprKind::Array(_) | ExprKind::Tuple(_) | ExprKind::Range(_) => {
                 self.fold_expr_kind(expr.kind)?
             }
 
             // functions are values
             ExprKind::Func(f) => ExprKind::Func(f),
 
-            // convert to function calls and then evaluate to a value
-            ExprKind::Binary(binary) => {
-                let func_call = binary_to_func_call(binary, expr.span);
-                self.fold_expr(func_call)?.kind
-            }
-            ExprKind::Unary(unary) => {
-                let func_call = unary_to_func_call(unary, expr.span);
-                self.fold_expr(func_call)?.kind
-            }
-
             // ident are not values
             ExprKind::Ident(ident) => {
                 // here we'd have to implement the whole name resolution, but for now,
                 // let's do something simple
 
                 // this is very crude, but for simple cases, it's enough
                 let mut ident = ident;
@@ -84,25 +73,14 @@
 
                 if func.args.len() < func.params.len() {
                     ExprKind::Func(func)
                 } else {
                     self.eval_function(*func, expr.span)?
                 }
             }
-            ExprKind::Pipeline(mut pipeline) => {
-                let mut res = self.fold_expr(pipeline.exprs.remove(0))?;
-                for expr in pipeline.exprs {
-                    let func_call =
-                        Expr::new(ExprKind::FuncCall(FuncCall::new_simple(expr, vec![res])));
-
-                    res = self.fold_expr(func_call)?;
-                }
-
-                return Ok(res);
-            }
 
             ExprKind::All { .. }
             | ExprKind::TransformCall(_)
             | ExprKind::SString(_)
             | ExprKind::FString(_)
             | ExprKind::Case(_)
             | ExprKind::RqOperator { .. }
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/lowering.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/lowering.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 use anyhow::Result;
 use enum_as_inner::EnumAsInner;
 use itertools::Itertools;
 
 use crate::error::{Error, Reason, Span, WithErrorInfo};
 use crate::generic::{ColumnSort, WindowFrame};
 use crate::ir::generic::{InterpolateItem, Range, SwitchCase};
-use crate::ir::pl::{
-    self, BinaryExpr, Ident, Lineage, LineageColumn, PlFold, QueryDef, TupleField, UnaryExpr,
+use crate::ir::pl::{self, Ident, Lineage, LineageColumn, PlFold, QueryDef, TupleField};
+use crate::ir::rq::{
+    self, CId, RelationColumn, RelationLiteral, RelationalQuery, TId, TableDecl, Transform,
 };
-use crate::ir::rq::{self, CId, Query, RelationColumn, RelationLiteral, TId, TableDecl, Transform};
-use crate::semantic::context::TableExpr;
+use crate::semantic::decl::TableExpr;
 use crate::semantic::module::Module;
 use crate::semantic::write_pl;
 use crate::utils::{toposort, IdGenerator};
 use crate::COMPILER_VERSION;
 
-use super::context::{self, Context, DeclKind};
-use super::NS_DEFAULT_DB;
+use super::decl::{self, DeclKind};
+use super::{RootModule, NS_DEFAULT_DB};
 
 /// Convert AST into IR and make sure that:
 /// - transforms are not nested,
 /// - transforms have correct partition, window and sort set,
 /// - make sure there are no unresolved expressions.
-pub fn lower_to_ir(context: Context, main_path: &[String]) -> Result<(Query, Context)> {
+pub fn lower_to_ir(
+    context: RootModule,
+    main_path: &[String],
+) -> Result<(RelationalQuery, RootModule)> {
     // find main
     log::debug!("lookup for main pipeline in {main_path:?}");
     let (_, main_ident) = context.find_main_rel(main_path).map_err(|hint| {
         Error::new_simple("Missing main pipeline")
             .with_code("E0001")
             .with_hints(hint)
     })?;
@@ -56,15 +59,15 @@
 
         if is_main {
             let main_table = l.table_buffer.pop().unwrap();
             main_relation = Some(main_table.relation);
         }
     }
 
-    let query = Query {
+    let query = RelationalQuery {
         def,
         tables: l.table_buffer,
         relation: main_relation.unwrap(),
     };
     Ok((query, l.context))
 }
 
@@ -110,15 +113,15 @@
 }
 
 #[derive(Debug)]
 struct Lowerer {
     cid: IdGenerator<CId>,
     tid: IdGenerator<TId>,
 
-    context: Context,
+    context: RootModule,
 
     /// describes what has certain id has been lowered to
     node_mapping: HashMap<usize, LoweredTarget>,
 
     /// mapping from [Ident] of [crate::ast::TableDef] into [TId]s
     table_mapping: HashMap<Ident, TId>,
 
@@ -139,15 +142,15 @@
 
     /// Lowered node was a pipeline input.
     /// Contains mapping from column names to CIds, along with order in frame.
     Input(HashMap<RelationColumn, (CId, usize)>),
 }
 
 impl Lowerer {
-    fn new(context: Context) -> Self {
+    fn new(context: RootModule) -> Self {
         Lowerer {
             context,
 
             cid: IdGenerator::new(),
             tid: IdGenerator::new(),
 
             node_mapping: HashMap::new(),
@@ -155,16 +158,16 @@
 
             window: None,
             pipeline: Vec::new(),
             table_buffer: Vec::new(),
         }
     }
 
-    fn lower_table_decl(&mut self, table: context::TableDecl, fq_ident: Ident) -> Result<()> {
-        let context::TableDecl { ty, expr } = table;
+    fn lower_table_decl(&mut self, table: decl::TableDecl, fq_ident: Ident) -> Result<()> {
+        let decl::TableDecl { ty, expr } = table;
 
         // TODO: can this panic?
         let columns = ty.unwrap().into_relation().unwrap();
 
         let (relation, name) = match expr {
             TableExpr::RelationVar(expr) => {
                 // a CTE
@@ -819,29 +822,26 @@
             pl::ExprKind::Param(id) => rq::ExprKind::Param(id),
 
             pl::ExprKind::FuncCall(_)
             | pl::ExprKind::Range(_)
             | pl::ExprKind::Tuple(_)
             | pl::ExprKind::Array(_)
             | pl::ExprKind::Func(_)
-            | pl::ExprKind::Pipeline(_)
             | pl::ExprKind::Type(_)
             | pl::ExprKind::TransformCall(_) => {
                 log::debug!("cannot lower {expr:?}");
                 return Err(Error::new(Reason::Unexpected {
                     found: format!("`{}`", write_pl(expr.clone())),
                 })
                 .push_hint("this is probably a 'bad type' error (we are working on that)")
                 .with_span(expr.span)
                 .into());
             }
 
-            pl::ExprKind::Unary(UnaryExpr { .. })
-            | pl::ExprKind::Binary(BinaryExpr { .. })
-            | pl::ExprKind::Internal(_) => {
+            pl::ExprKind::Internal(_) => {
                 panic!("Unresolved lowering: {}", write_pl(expr))
             }
         };
 
         Ok(rq::Expr {
             kind,
             span: expr.span,
@@ -943,20 +943,20 @@
     }
 }
 
 #[derive(Default)]
 struct TableExtractor {
     path: Vec<String>,
 
-    tables: Vec<(Ident, context::TableDecl)>,
+    tables: Vec<(Ident, decl::TableDecl)>,
 }
 
 impl TableExtractor {
     /// Finds table declarations in a module, recursively.
-    fn extract(root_module: &Module) -> Vec<(Ident, context::TableDecl)> {
+    fn extract(root_module: &Module) -> Vec<(Ident, decl::TableDecl)> {
         let mut te = TableExtractor::default();
         te.extract_from_module(root_module);
         te.tables
     }
 
     /// Finds table declarations in a module, recursively.
     fn extract_from_module(&mut self, namespace: &Module) {
@@ -978,17 +978,17 @@
     }
 }
 
 /// Does a topological sort of the pipeline definitions and prunes all definitions that
 /// are not needed for the main pipeline. To do this, it needs to collect references
 /// between pipelines.
 fn toposort_tables(
-    tables: Vec<(Ident, context::TableDecl)>,
+    tables: Vec<(Ident, decl::TableDecl)>,
     main_table: &Ident,
-) -> Vec<(Ident, context::TableDecl)> {
+) -> Vec<(Ident, decl::TableDecl)> {
     let tables: HashMap<_, _, RandomState> = HashMap::from_iter(tables);
 
     let mut dependencies: Vec<(Ident, Vec<Ident>)> = Vec::new();
     for (ident, table) in &tables {
         let deps = if let TableExpr::RelationVar(e) = &table.expr {
             TableDepsCollector::collect(*e.clone())
         } else {
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 //! Semantic resolver (name resolution, type checking and lowering to RQ)
 
 mod ast_expand;
-mod context;
+mod decl;
 mod eval;
 mod lowering;
 mod module;
 pub mod reporting;
 mod resolver;
+mod root_module;
 mod static_analysis;
 
 use anyhow::Result;
 use itertools::Itertools;
 use std::path::PathBuf;
 
-pub use self::context::Context;
 pub use self::module::Module;
 use self::resolver::Resolver;
 pub use self::resolver::ResolverOptions;
+pub use self::root_module::RootModule;
 pub use eval::eval;
 pub use lowering::lower_to_ir;
 
 use crate::error::WithErrorInfo;
 use crate::ir::pl::{self, Lineage, LineageColumn, ModuleDef, Stmt, StmtKind, TypeDef, VarDef};
-use crate::ir::rq::Query;
+use crate::ir::rq::RelationalQuery;
 use crate::{Error, Reason, SourceTree};
 
 /// Runs semantic analysis on the query and lowers PL to RQ.
 pub fn resolve_and_lower(
     file_tree: SourceTree<Vec<prql_ast::stmt::Stmt>>,
     main_path: &[String],
-) -> Result<Query> {
+) -> Result<RelationalQuery> {
     let context = resolve(file_tree, Default::default())?;
 
     let (query, _) = lowering::lower_to_ir(context, main_path)?;
     Ok(query)
 }
 
 /// Runs semantic analysis on the query.
 pub fn resolve(
     mut file_tree: SourceTree<Vec<prql_ast::stmt::Stmt>>,
     options: ResolverOptions,
-) -> Result<Context> {
+) -> Result<RootModule> {
     // inject std module if it does not exist
     if !file_tree.sources.contains_key(&PathBuf::from("std.prql")) {
         let mut source_tree = SourceTree {
             sources: Default::default(),
             source_ids: file_tree.source_ids.clone(),
         };
         load_std_lib(&mut source_tree);
         let ast = crate::parser::parse(&source_tree).unwrap();
         let (path, content) = ast.sources.into_iter().next().unwrap();
         file_tree.insert(path, content);
     }
 
     // init empty context
-    let context = Context {
+    let context = RootModule {
         root_mod: Module::new_root(),
-        ..Context::default()
+        ..RootModule::default()
     };
     let mut resolver = Resolver::new(context, options);
 
     // resolve sources one by one
     // TODO: recursive references
     for (path, stmts) in normalize(file_tree)? {
-        let stmts = ast_expand::expand_stmts(stmts);
+        let stmts = ast_expand::expand_stmts(stmts)?;
 
         resolver.current_module_path = path;
         resolver.fold_statements(stmts)?;
     }
 
     Ok(resolver.context)
 }
@@ -206,27 +207,27 @@
     crate::codegen::write_expr(&expr)
 }
 #[cfg(test)]
 pub mod test {
     use anyhow::Result;
     use insta::assert_yaml_snapshot;
 
-    use crate::ir::rq::Query;
+    use crate::ir::rq::RelationalQuery;
     use crate::parser::parse;
 
-    use super::{resolve, resolve_and_lower, Context};
+    use super::{resolve, resolve_and_lower, RootModule};
 
-    pub fn parse_resolve_and_lower(query: &str) -> Result<Query> {
+    pub fn parse_resolve_and_lower(query: &str) -> Result<RelationalQuery> {
         let mut source_tree = query.into();
         super::load_std_lib(&mut source_tree);
 
         resolve_and_lower(parse(&source_tree)?, &[])
     }
 
-    pub fn parse_and_resolve(query: &str) -> Result<Context> {
+    pub fn parse_and_resolve(query: &str) -> Result<RootModule> {
         let mut source_tree = query.into();
         super::load_std_lib(&mut source_tree);
 
         resolve(parse(&source_tree)?, Default::default())
     }
 
     #[test]
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/module.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/module.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use anyhow::Result;
 use itertools::Itertools;
 use serde::{Deserialize, Serialize};
 
 use crate::ir::pl::{Expr, Ident, TupleField, Ty};
 use crate::Error;
 
-use super::context::{Decl, DeclKind, TableDecl, TableExpr};
+use super::decl::{Decl, DeclKind, TableDecl, TableExpr};
 use super::{Lineage, LineageColumn, NS_PARAM, NS_STD};
 use super::{NS_INFER, NS_INFER_MODULE, NS_SELF, NS_THAT, NS_THIS};
 
 #[derive(Default, PartialEq, Serialize, Deserialize, Clone)]
 pub struct Module {
     /// Names declared in this module. This is the important thing.
     pub(super) names: HashMap<String, Decl>,
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/reporting.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/reporting.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 use std::fmt::Write;
 use std::ops::Range;
 
 use anyhow::{Ok, Result};
 use ariadne::{Color, Label, Report, ReportBuilder, ReportKind, Source};
 
-use super::context::{DeclKind, TableDecl, TableExpr};
+use super::decl::{DeclKind, TableDecl, TableExpr};
 use super::NS_DEFAULT_DB;
-use super::{Context, Lineage};
+use super::{Lineage, RootModule};
 use crate::error::Span;
 use crate::ir::pl::*;
 
-pub fn label_references(context: &Context, source_id: String, source: String) -> Vec<u8> {
+pub fn label_references(context: &RootModule, source_id: String, source: String) -> Vec<u8> {
     let mut report = Report::build(ReportKind::Custom("Info", Color::Blue), &source_id, 0);
 
     let source = Source::from(source);
 
     // label all idents and function calls
     let mut labeler = Labeler {
         context,
@@ -30,15 +30,15 @@
         .write((source_id, source), &mut out)
         .unwrap();
     out
 }
 
 /// Traverses AST and add labels for each of the idents and function calls
 struct Labeler<'a> {
-    context: &'a Context,
+    context: &'a RootModule,
     source: &'a Source,
     source_id: &'a str,
     report: &'a mut ReportBuilder<'static, (String, Range<usize>)>,
 }
 
 impl<'a> Labeler<'a> {
     fn fold_table_exprs(&mut self) {
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/root_module_impl.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 use anyhow::Result;
 use itertools::Itertools;
 
 use prql_ast::expr::Ident;
 
 use crate::error::WithErrorInfo;
 use crate::ir::pl::{Annotation, Expr, ExprKind, LineageColumn, TupleField, Ty};
-use crate::semantic::context::{Decl, DeclKind, TableDecl, TableExpr};
-use crate::semantic::{Context, Module, NS_INFER, NS_INFER_MODULE, NS_SELF, NS_THAT, NS_THIS};
+use crate::semantic::decl::{Decl, DeclKind, TableDecl, TableExpr};
+use crate::semantic::{Module, RootModule, NS_INFER, NS_INFER_MODULE, NS_SELF, NS_THAT, NS_THIS};
 use crate::Error;
 
-impl Context {
+impl RootModule {
     pub(super) fn declare(
         &mut self,
         ident: Ident,
         decl: DeclKind,
         id: Option<usize>,
         annotations: Vec<Annotation>,
     ) -> Result<()> {
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 use std::collections::HashMap;
 use std::iter::zip;
 
-use anyhow::{anyhow, bail, Result};
+use anyhow::Result;
 use itertools::{Itertools, Position};
 
 use crate::error::{Error, Reason, Span, WithErrorInfo};
 use crate::ir::pl::*;
-use crate::semantic::context::TableDecl;
+use crate::semantic::decl::TableDecl;
 use crate::semantic::{static_analysis, NS_PARAM};
 use crate::utils::IdGenerator;
 
-use super::context::{Context, Decl, DeclKind, TableExpr};
+use super::decl::{Decl, DeclKind, TableExpr};
 use super::module::Module;
-use super::reporting::debug_call_tree;
-use super::{write_pl, NS_DEFAULT_DB, NS_INFER, NS_STD, NS_THAT, NS_THIS};
+use super::{write_pl, RootModule, NS_DEFAULT_DB, NS_INFER, NS_STD, NS_THAT, NS_THIS};
 use flatten::Flattener;
 use transforms::coerce_into_tuple_and_flatten;
 use type_resolver::infer_type;
 
-mod context_impl;
 mod flatten;
+mod root_module_impl;
 mod transforms;
 mod type_resolver;
 
 /// Can fold (walk) over AST and for each function call or variable find what they are referencing.
 pub struct Resolver {
-    pub context: Context,
+    pub context: RootModule,
 
     pub current_module_path: Vec<String>,
 
     default_namespace: Option<String>,
 
     /// Sometimes ident closures must be resolved and sometimes not. See [test::test_func_call_resolve].
     in_func_call_name: bool,
@@ -43,15 +42,15 @@
 
 #[derive(Default, Clone)]
 pub struct ResolverOptions {
     pub allow_module_decls: bool,
 }
 
 impl Resolver {
-    pub fn new(context: Context, options: ResolverOptions) -> Self {
+    pub fn new(context: RootModule, options: ResolverOptions) -> Self {
         Resolver {
             context,
             options,
             current_module_path: Vec::new(),
             default_namespace: None,
             in_func_call_name: false,
             disable_type_checking: false,
@@ -347,14 +346,22 @@
                     _ => Expr {
                         kind: ExprKind::Ident(fq_ident),
                         ..node
                     },
                 }
             }
 
+            ExprKind::FuncCall(FuncCall { name, args, .. })
+                if (name.kind.as_ident()).map_or(false, |i| i.to_string() == "std.not")
+                    && matches!(args[0].kind, ExprKind::Tuple(_)) =>
+            {
+                let arg = args.into_iter().exactly_one().unwrap();
+                self.resolve_column_exclusion(arg)?
+            }
+
             ExprKind::FuncCall(FuncCall {
                 name,
                 args,
                 named_args,
             }) => {
                 // fold function name
                 self.default_namespace = None;
@@ -366,45 +373,16 @@
                 let func = *name.try_cast(|n| n.into_func(), None, "a function")?;
 
                 // fold function
                 let func = self.apply_args_to_closure(func, args, named_args)?;
                 self.fold_function(func, span)?
             }
 
-            ExprKind::Pipeline(pipeline) => {
-                self.default_namespace = None;
-                self.resolve_pipeline(pipeline)?
-            }
-
             ExprKind::Func(closure) => self.fold_function(*closure, span)?,
 
-            ExprKind::Unary(UnaryExpr {
-                op: UnOp::EqSelf,
-                expr,
-            }) => {
-                let kind = self.resolve_eq_self(*expr, span)?;
-                Expr { kind, ..node }
-            }
-
-            ExprKind::Unary(UnaryExpr {
-                op: UnOp::Add,
-                expr,
-            }) => self.fold_expr(*expr)?,
-
-            ExprKind::Unary(UnaryExpr {
-                op: UnOp::Not,
-                expr,
-            }) if matches!(expr.kind, ExprKind::Tuple(_)) => {
-                self.resolve_column_exclusion(*expr)?
-            }
-
-            ExprKind::Unary(unary) => self.fold_expr(unary_to_func_call(unary, span))?,
-
-            ExprKind::Binary(binary) => self.fold_expr(binary_to_func_call(binary, span))?,
-
             ExprKind::All { within, except } => {
                 let decl = self.context.root_mod.get(&within);
 
                 // lookup ids of matched inputs
                 let target_ids = decl
                     .and_then(|d| d.kind.as_module())
                     .iter()
@@ -501,115 +479,15 @@
                 }
             }
         }
         Ok(r)
     }
 }
 
-pub fn unary_to_func_call(UnaryExpr { op, expr }: UnaryExpr, span: Option<Span>) -> Expr {
-    let func_name = match op {
-        UnOp::Neg => ["std", "neg"],
-        UnOp::Not => ["std", "not"],
-        UnOp::Add | UnOp::EqSelf => unreachable!(),
-    };
-    let mut func_call = Expr::new(ExprKind::FuncCall(FuncCall::new_simple(
-        Expr::new(ExprKind::Ident(Ident::from_path(func_name.to_vec()))),
-        vec![*expr],
-    )));
-    func_call.span = span;
-    func_call
-}
-
-pub fn binary_to_func_call(BinaryExpr { op, left, right }: BinaryExpr, span: Option<Span>) -> Expr {
-    let func_name = match op {
-        BinOp::Mul => ["std", "mul"],
-        BinOp::DivInt => ["std", "div_i"],
-        BinOp::DivFloat => ["std", "div_f"],
-        BinOp::Mod => ["std", "mod"],
-        BinOp::Add => ["std", "add"],
-        BinOp::Sub => ["std", "sub"],
-        BinOp::Eq => ["std", "eq"],
-        BinOp::Ne => ["std", "ne"],
-        BinOp::Gt => ["std", "gt"],
-        BinOp::Lt => ["std", "lt"],
-        BinOp::Gte => ["std", "gte"],
-        BinOp::Lte => ["std", "lte"],
-        BinOp::RegexSearch => ["std", "regex_search"],
-        BinOp::And => ["std", "and"],
-        BinOp::Or => ["std", "or"],
-        BinOp::Coalesce => ["std", "coalesce"],
-    };
-    let mut func_call = Expr::new(ExprKind::FuncCall(FuncCall::new_simple(
-        Expr::new(ExprKind::Ident(Ident::from_path(func_name.to_vec()))),
-        vec![*left, *right],
-    )));
-    func_call.span = span;
-    func_call
-}
-
 impl Resolver {
-    fn resolve_pipeline(&mut self, Pipeline { mut exprs }: Pipeline) -> Result<Expr> {
-        let mut value = exprs.remove(0);
-        value = self.fold_expr(value)?;
-
-        // This is a workaround for pipelines that start with a transform.
-        // It checks if first value has resolved to a closure, and if it has,
-        // constructs an adhoc closure around the pipeline.
-        // Maybe this should not even be supported, or maybe we should have
-        // some kind of indication that first element of a pipeline is not a
-        // plain value.
-        let closure_param = if let ExprKind::Func(closure) = &mut value.kind {
-            // only apply this workaround if closure expects a single arg
-            if (closure.params.len() - closure.args.len()) == 1 {
-                let param = "_pip_val";
-                let value = Expr::new(ExprKind::Ident(Ident::from_name(param)));
-                closure.args.push(value);
-                Some(param)
-            } else {
-                None
-            }
-        } else {
-            None
-        };
-
-        // the beef of this function: wrapping into func calls
-        for expr in exprs {
-            let span = expr.span;
-
-            value = Expr::new(ExprKind::FuncCall(FuncCall::new_simple(expr, vec![value])));
-            value.span = span;
-        }
-
-        // second part of the workaround
-        if let Some(closure_param) = closure_param {
-            value = Expr::new(ExprKind::Func(Box::new(Func {
-                name_hint: None,
-                body: Box::new(value),
-                return_ty: None,
-
-                args: vec![],
-                params: vec![FuncParam {
-                    name: closure_param.to_string(),
-                    default_value: None,
-                    ty: None,
-                }],
-                named_params: vec![],
-                env: HashMap::new(),
-            })));
-        }
-
-        if log::log_enabled!(log::Level::Debug) {
-            let (v, tree) = debug_call_tree(value);
-            value = v;
-            log::debug!("unpacked pipeline to following call tree: \n{tree}");
-        }
-
-        self.fold_expr(value)
-    }
-
     pub fn resolve_ident(&mut self, ident: &Ident) -> Result<Ident, Error> {
         if let Some(default_namespace) = &self.default_namespace {
             self.context.resolve_ident(ident, Some(default_namespace))
         } else {
             let mut ident = ident.clone().prepend(self.current_module_path.clone());
 
             let mut res = self.context.resolve_ident(&ident, None);
@@ -646,17 +524,15 @@
             ))
             .with_span(span)
             .into());
         }
 
         let enough_args = closure.args.len() == closure.params.len();
         if !enough_args {
-            // not enough arguments: don't fold
-            log::debug!("returning as closure");
-            return Ok(expr_of_func(closure));
+            return Ok(expr_of_func(closure, span));
         }
 
         // make sure named args are pushed into params
         let closure = if !closure.named_params.is_empty() {
             self.apply_args_to_closure(closure, [].into(), [].into())?
         } else {
             closure
@@ -673,15 +549,22 @@
         if log::log_enabled!(log::Level::Debug) {
             let name = closure
                 .name_hint
                 .clone()
                 .unwrap_or_else(|| Ident::from_name("<unnamed>"));
             log::debug!("resolving args of function {}", name);
         }
-        let closure = self.resolve_function_args(closure)?;
+        let res = self.resolve_function_args(closure)?;
+
+        let closure = match res {
+            Ok(func) => func,
+            Err(func) => {
+                return Ok(expr_of_func(func, span));
+            }
+        };
 
         let needs_window = (closure.params.last())
             .and_then(|p| p.ty.as_ref())
             .map(|t| t.as_ty().unwrap().is_sub_type_of_array())
             .unwrap_or_default();
 
         // evaluate
@@ -739,15 +622,15 @@
                 body
             }
         };
 
         // pop the env
         self.context.root_mod.stack_pop(NS_PARAM).unwrap();
 
-        Ok(res)
+        Ok(Expr { span, ..res })
     }
 
     fn fold_function_types(&mut self, mut closure: Func) -> Result<Func> {
         closure.params = closure
             .params
             .into_iter()
             .map(|p| -> Result<_> {
@@ -788,19 +671,21 @@
         }
 
         // positional
         closure.args.extend(args);
         Ok(closure)
     }
 
-    fn resolve_function_args(&mut self, to_resolve: Func) -> Result<Func> {
+    /// Resolves function arguments. Will return `Err(func)` is partial application is required.
+    fn resolve_function_args(&mut self, to_resolve: Func) -> Result<Result<Func, Func>> {
         let mut closure = Func {
             args: vec![Expr::new(Literal::Null); to_resolve.args.len()],
             ..to_resolve
         };
+        let mut partial_application_position = None;
 
         let func_name = &closure.name_hint;
 
         let (relations, other): (Vec<_>, Vec<_>) = zip(&closure.params, to_resolve.args)
             .enumerate()
             .partition(|(_, (param, _))| {
                 let is_relation = param
@@ -816,92 +701,126 @@
         let has_relations = !relations.is_empty();
 
         // resolve relational args
         if has_relations {
             self.context.root_mod.shadow(NS_THIS);
             self.context.root_mod.shadow(NS_THAT);
 
-            for (pos, (index, (param, arg))) in relations.into_iter().with_position() {
+            for (pos, (index, (param, mut arg))) in relations.into_iter().with_position() {
                 let is_last = matches!(pos, Position::Last | Position::Only);
 
                 // just fold the argument alone
-                let arg = self.fold_and_type_check(arg, param, func_name)?;
+                if partial_application_position.is_none() {
+                    arg = self
+                        .fold_and_type_check(arg, param, func_name)?
+                        .unwrap_or_else(|a| {
+                            partial_application_position = Some(index);
+                            a
+                        });
+                }
                 log::debug!("resolved arg to {}", arg.kind.as_ref());
 
                 // add relation frame into scope
-                let frame = arg.lineage.as_ref().unwrap();
-                if is_last {
-                    self.context.root_mod.insert_frame(frame, NS_THIS);
-                } else {
-                    self.context.root_mod.insert_frame(frame, NS_THAT);
+                if partial_application_position.is_none() {
+                    let frame = arg.lineage.as_ref().unwrap();
+                    if is_last {
+                        self.context.root_mod.insert_frame(frame, NS_THIS);
+                    } else {
+                        self.context.root_mod.insert_frame(frame, NS_THAT);
+                    }
                 }
 
                 closure.args[index] = arg;
             }
         }
 
         // resolve other positional
         for (index, (param, mut arg)) in other {
-            if let ExprKind::Tuple(fields) = arg.kind {
-                // if this is a tuple, resolve elements separately,
-                // so they can be added to scope, before resolving subsequent elements.
-
-                let mut fields_new = Vec::with_capacity(fields.len());
-                for field in fields {
-                    let field = self.fold_within_namespace(field, &param.name)?;
-
-                    // add aliased columns into scope
-                    if let Some(alias) = field.alias.clone() {
-                        let id = field.id.unwrap();
-                        self.context.root_mod.insert_frame_col(NS_THIS, alias, id);
+            if partial_application_position.is_none() {
+                if let ExprKind::Tuple(fields) = arg.kind {
+                    // if this is a tuple, resolve elements separately,
+                    // so they can be added to scope, before resolving subsequent elements.
+
+                    let mut fields_new = Vec::with_capacity(fields.len());
+                    for field in fields {
+                        let field = self.fold_within_namespace(field, &param.name)?;
+
+                        // add aliased columns into scope
+                        if let Some(alias) = field.alias.clone() {
+                            let id = field.id.unwrap();
+                            self.context.root_mod.insert_frame_col(NS_THIS, alias, id);
+                        }
+                        fields_new.push(field);
                     }
-                    fields_new.push(field);
+
+                    // note that this tuple node has to be resolved itself
+                    // (it's elements are already resolved and so their resolving
+                    // should be skipped)
+                    arg.kind = ExprKind::Tuple(fields_new);
                 }
 
-                // note that this tuple node has to be resolved itself
-                // (it's elements are already resolved and so their resolving
-                // should be skipped)
-                arg.kind = ExprKind::Tuple(fields_new);
+                arg = self
+                    .fold_and_type_check(arg, param, func_name)?
+                    .unwrap_or_else(|a| {
+                        partial_application_position = Some(index);
+                        a
+                    });
             }
 
-            let arg = self.fold_and_type_check(arg, param, func_name)?;
-
             closure.args[index] = arg;
         }
 
         if has_relations {
             self.context.root_mod.unshadow(NS_THIS);
             self.context.root_mod.unshadow(NS_THAT);
         }
 
-        Ok(closure)
+        Ok(if let Some(position) = partial_application_position {
+            log::debug!(
+                "partial application of {} at arg {position}",
+                closure.as_debug_name()
+            );
+
+            Err(extract_partial_application(closure, position))
+        } else {
+            Ok(closure)
+        })
     }
 
     fn fold_and_type_check(
         &mut self,
         arg: Expr,
         param: &FuncParam,
         func_name: &Option<Ident>,
-    ) -> Result<Expr> {
+    ) -> Result<Result<Expr, Expr>> {
         let mut arg = self.fold_within_namespace(arg, &param.name)?;
 
         // don't validate types of unresolved exprs
         if arg.id.is_some() && !self.disable_type_checking {
             // validate type
 
+            let expects_func = param
+                .ty
+                .as_ref()
+                .map(|t| t.as_ty().unwrap().is_function())
+                .unwrap_or_default();
+            if !expects_func && arg.kind.is_func() {
+                return Ok(Err(arg));
+            }
+
             let who = || {
                 func_name
                     .as_ref()
                     .map(|n| format!("function {n}, param `{}`", param.name))
             };
             let ty = param.ty.as_ref().map(|t| t.as_ty().unwrap());
             self.validate_type(&mut arg, ty, &who)?;
         }
 
-        Ok(arg)
+        Ok(Ok(arg))
     }
 
     fn fold_within_namespace(&mut self, expr: Expr, param_name: &str) -> Result<Expr> {
         let prev_namespace = self.default_namespace.take();
 
         if param_name.starts_with("noresolve.") {
             return Ok(expr);
@@ -912,40 +831,14 @@
         };
 
         let res = self.fold_expr(expr);
         self.default_namespace = prev_namespace;
         res
     }
 
-    fn resolve_eq_self(&mut self, expr: Expr, span: Option<Span>) -> Result<ExprKind> {
-        let ident = expr
-            .kind
-            .into_ident()
-            .map_err(|_| anyhow!("you can only use column names with self-equality operator."))?;
-        if !ident.path.is_empty() {
-            bail!("you cannot use namespace prefix with self-equality operator.");
-        }
-        let mut left = Expr::new(ExprKind::Ident(Ident {
-            path: vec![NS_THIS.to_string()],
-            name: ident.name.clone(),
-        }));
-        left.span = span;
-        let mut right = Expr::new(ExprKind::Ident(Ident {
-            path: vec![NS_THAT.to_string()],
-            name: ident.name,
-        }));
-        right.span = span;
-        let kind = ExprKind::RqOperator {
-            name: "std.eq".to_string(),
-            args: vec![left, right],
-        };
-        let kind = fold_expr_kind(self, kind)?;
-        Ok(kind)
-    }
-
     fn resolve_column_exclusion(&mut self, expr: Expr) -> Result<Expr> {
         let expr = self.fold_expr(expr)?;
         let tuple = coerce_into_tuple_and_flatten(expr)?;
         let except: Vec<Expr> = tuple
             .into_iter()
             .map(|e| match e.kind {
                 ExprKind::Ident(_) | ExprKind::All { .. } => Ok(e),
@@ -978,24 +871,97 @@
                 Some(set_expr)
             }
             None => None,
         })
     }
 
     fn fold_ty_or_expr(&mut self, ty_or_expr: Option<TyOrExpr>) -> Result<Option<TyOrExpr>> {
-        Ok(match ty_or_expr {
+        self.context.root_mod.shadow(NS_THIS);
+        self.context.root_mod.shadow(NS_THAT);
+
+        let res = match ty_or_expr {
             Some(TyOrExpr::Expr(ty_expr)) => {
                 Some(TyOrExpr::Ty(self.fold_type_expr(Some(ty_expr))?.unwrap()))
             }
             _ => ty_or_expr,
-        })
+        };
+
+        self.context.root_mod.unshadow(NS_THIS);
+        self.context.root_mod.unshadow(NS_THAT);
+        Ok(res)
+    }
+}
+
+fn extract_partial_application(mut func: Func, position: usize) -> Func {
+    // Input:
+    // Func {
+    //     params: [x, y, z],
+    //     args: [
+    //         x,
+    //         Func {
+    //             params: [a, b],
+    //             args: [a],
+    //             body: arg_body
+    //         },
+    //         z
+    //     ],
+    //     body: parent_body
+    // }
+
+    // Output:
+    // Func {
+    //     params: [b],
+    //     args: [],
+    //     body: Func {
+    //         params: [x, y, z],
+    //         args: [
+    //             x,
+    //             Func {
+    //                 params: [a, b],
+    //                 args: [a, b],
+    //                 body: arg_body
+    //             },
+    //             z
+    //         ],
+    //         body: parent_body
+    //     }
+    // }
+
+    // This is quite in-efficient, especially for long pipelines.
+    // Maybe it could be special-cased, for when the arg func has a single param.
+    // In that case, it may be possible to pull the arg func up and basically swap
+    // it with the parent func.
+
+    let arg = func.args.get_mut(position).unwrap();
+    let arg_func = arg.kind.as_func_mut().unwrap();
+
+    let param_name = format!("_partial_{}", arg.id.unwrap());
+    let substitute_arg = Expr::new(Ident::from_path(vec![
+        NS_PARAM.to_string(),
+        param_name.clone(),
+    ]));
+    arg_func.args.push(substitute_arg);
+
+    // set the arg func body to the parent func
+    Func {
+        name_hint: None,
+        return_ty: None,
+        body: Box::new(Expr::new(func)),
+        params: vec![FuncParam {
+            name: param_name,
+            ty: None,
+            default_value: None,
+        }],
+        named_params: Default::default(),
+        args: Default::default(),
+        env: Default::default(),
     }
 }
 
-fn expr_of_func(func: Func) -> Expr {
+fn expr_of_func(func: Func, span: Option<Span>) -> Expr {
     let ty = TyFunc {
         args: func
             .params
             .iter()
             .skip(func.args.len())
             .map(|a| a.ty.as_ref().map(|x| x.as_ty().cloned().unwrap()))
             .collect(),
@@ -1003,14 +969,15 @@
     };
 
     Expr {
         ty: Some(Ty {
             kind: TyKind::Function(Some(ty)),
             name: None,
         }),
+        span,
         ..Expr::new(ExprKind::Func(Box::new(func)))
     }
 }
 
 fn ty_of_lineage(lineage: &Lineage) -> Ty {
     Ty::relation(
         lineage
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap`

 * *Files 15% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 expression: "resolve_lineage(r#\"\n            from e = employees\n            join salaries (==emp_no)\n            group {e.emp_no, e.gender} (\n                aggregate {\n                    emp_salary = average salaries.salary\n                }\n            )\n            \"#).unwrap()"
 ---
 columns:
   - Single:
       name:
         - e
         - emp_no
-      target_id: 221
+      target_id: 214
       target_name: ~
   - Single:
       name:
         - e
         - gender
-      target_id: 222
+      target_id: 215
       target_name: ~
   - Single:
       name:
         - emp_salary
-      target_id: 247
+      target_id: 239
       target_name: ~
 inputs:
-  - id: 182
+  - id: 206
     name: e
     table:
       - default_db
       - employees
-  - id: 216
+  - id: 199
     name: salaries
     table:
       - default_db
       - salaries
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 expression: "resolve_lineage(r#\"\n            from orders\n            select {customer_no, gross, tax, gross - tax}\n            take 20\n            \"#).unwrap()"
 ---
 columns:
   - Single:
       name:
         - orders
         - customer_no
-      target_id: 212
+      target_id: 202
       target_name: ~
   - Single:
       name:
         - orders
         - gross
-      target_id: 213
+      target_id: 203
       target_name: ~
   - Single:
       name:
         - orders
         - tax
-      target_id: 214
+      target_id: 204
       target_name: ~
   - Single:
       name: ~
-      target_id: 216
+      target_id: 205
       target_name: ~
 inputs:
-  - id: 182
+  - id: 201
     name: orders
     table:
       - default_db
       - orders
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       name: ~
     lineage:
       columns:
         - All:
             input_name: c_invoice
             except: []
       inputs:
-        - id: 182
+        - id: 194
           name: c_invoice
           table:
             - default_db
             - c_invoice
   kind:
     Aggregate:
       assigns:
@@ -181,20 +181,20 @@
   name: relation
 lineage:
   columns:
     - Single:
         name:
           - c_invoice
           - issued_at
-        target_id: 205
+        target_id: 195
         target_name: ~
     - Single:
         name: ~
-        target_id: 229
+        target_id: 218
         target_name: ~
   inputs:
-    - id: 182
+    - id: 194
       name: c_invoice
       table:
         - default_db
         - c_invoice
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 use anyhow::{anyhow, bail, Result};
 use itertools::Itertools;
 use serde::Deserialize;
 use std::iter::zip;
 
 use crate::error::{Error, Reason, WithErrorInfo};
 use crate::generic::{SortDirection, WindowKind};
-use crate::ir::pl::BinaryExpr;
 use crate::ir::pl::PlFold;
 use crate::ir::pl::*;
 use crate::semantic::write_pl;
 
-use super::super::context::{Decl, DeclKind};
+use super::super::decl::{Decl, DeclKind};
 use super::super::module::Module;
 use super::Resolver;
-use super::{Context, Lineage};
+use super::{Lineage, RootModule};
 use super::{NS_PARAM, NS_THIS};
 
 /// try to convert function call with enough args into transform
 pub fn cast_transform(resolver: &mut Resolver, closure: Func) -> Result<Expr> {
     let internal_name = closure.body.kind.as_internal().unwrap();
 
     let (kind, input) = match internal_name.as_str() {
@@ -204,30 +203,18 @@
         "in" => {
             // yes, this is not a transform, but this is the most appropriate place for it
 
             let [pattern, value] = unpack::<2>(closure);
 
             match pattern.kind {
                 ExprKind::Range(Range { start, end }) => {
-                    let start = start.map(|start| {
-                        Expr::new(ExprKind::Binary(BinaryExpr {
-                            left: Box::new(value.clone()),
-                            op: BinOp::Gte,
-                            right: start,
-                        }))
-                    });
-                    let end = end.map(|end| {
-                        Expr::new(ExprKind::Binary(BinaryExpr {
-                            left: Box::new(value),
-                            op: BinOp::Lte,
-                            right: end,
-                        }))
-                    });
+                    let start = start.map(|s| new_binop(value.clone(), &["std", "gte"], *s));
+                    let end = end.map(|end| new_binop(value, &["std", "lte"], *end));
 
-                    let res = new_binop(start, BinOp::And, end);
+                    let res = maybe_binop(start, &["std", "and"], end);
                     let res =
                         res.unwrap_or_else(|| Expr::new(ExprKind::Literal(Literal::Boolean(true))));
                     return Ok(res);
                 }
                 ExprKind::Tuple(_) => {
                     // TODO: should translate into `value IN (...)`
                     //   but RQ currently does not support sub queries or
@@ -248,15 +235,15 @@
             // yes, this is not a transform, but this is the most appropriate place for it
 
             let [list] = unpack::<1>(closure);
             let list = list.kind.into_tuple().unwrap();
 
             let mut res = None;
             for item in list {
-                res = new_binop(res, BinOp::And, Some(item));
+                res = maybe_binop(res, &["std", "and"], Some(item));
             }
             let res = res.unwrap_or_else(|| Expr::new(ExprKind::Literal(Literal::Boolean(true))));
 
             return Ok(res);
         }
 
         "tuple_map" => {
@@ -299,15 +286,15 @@
         "_eq" => {
             // yes, this is not a transform, but this is the most appropriate place for it
 
             let [list] = unpack::<1>(closure);
             let list = list.kind.into_tuple().unwrap();
             let [a, b]: [Expr; 2] = list.try_into().unwrap();
 
-            let res = new_binop(Some(a), BinOp::Eq, Some(b)).unwrap();
+            let res = maybe_binop(Some(a), &["std", "eq"], Some(b)).unwrap();
             return Ok(res);
         }
 
         "from_text" => {
             // yes, this is not a transform, but this is the most appropriate place for it
 
             let [format, text_expr] = unpack::<2>(closure);
@@ -507,15 +494,15 @@
 
         env: Default::default(),
     })));
     Ok(pipeline)
 }
 
 impl TransformCall {
-    pub fn infer_type(&self, context: &Context) -> Result<Lineage> {
+    pub fn infer_type(&self, context: &RootModule) -> Result<Lineage> {
         use TransformKind::*;
 
         fn ty_frame_or_default(expr: &Expr) -> Result<Lineage> {
             expr.lineage
                 .clone()
                 .ok_or_else(|| anyhow!("expected {expr:?} to have table type"))
         }
@@ -656,15 +643,15 @@
 
 impl Lineage {
     pub fn clear(&mut self) {
         self.prev_columns.clear();
         self.prev_columns.append(&mut self.columns);
     }
 
-    pub fn apply_assign(&mut self, expr: &Expr, context: &Context) {
+    pub fn apply_assign(&mut self, expr: &Expr, context: &RootModule) {
         // spacial case: all except
         if let ExprKind::All { except, .. } = &expr.kind {
             let except_exprs: HashSet<&usize> =
                 except.iter().flat_map(|e| e.target_id.iter()).collect();
             let except_inputs: HashSet<&usize> =
                 except.iter().flat_map(|e| e.target_ids.iter()).collect();
 
@@ -718,15 +705,15 @@
         self.columns.push(LineageColumn::Single {
             name,
             target_id: id,
             target_name: None,
         });
     }
 
-    pub fn apply_assigns(&mut self, assigns: &[Expr], context: &Context) {
+    pub fn apply_assigns(&mut self, assigns: &[Expr], context: &RootModule) {
         for expr in assigns {
             self.apply_assign(expr, context);
         }
     }
 
     pub fn find_input(&self, input_name: &str) -> Option<&LineageInput> {
         self.inputs.iter().find(|i| i.name == input_name)
@@ -747,15 +734,15 @@
                 _ => {}
             }
         }
     }
 }
 
 impl LineageInput {
-    fn get_all_columns(&self, except: &[Expr], context: &Context) -> Vec<LineageColumn> {
+    fn get_all_columns(&self, except: &[Expr], context: &RootModule) -> Vec<LineageColumn> {
         let rel_def = context.root_mod.get(&self.table).unwrap();
         let rel_def = rel_def.kind.as_table_decl().unwrap();
 
         // TODO: can this panic?
         let columns = rel_def.ty.as_ref().unwrap().as_relation().unwrap();
 
         // special case: wildcard
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             Literal::String(_) => TyKind::Primitive(PrimitiveSet::Text),
             Literal::Date(_) => TyKind::Primitive(PrimitiveSet::Date),
             Literal::Time(_) => TyKind::Primitive(PrimitiveSet::Time),
             Literal::Timestamp(_) => TyKind::Primitive(PrimitiveSet::Timestamp),
             Literal::ValueAndUnit(_) => return Ok(None), // TODO
         },
 
-        ExprKind::Ident(_) | ExprKind::Pipeline(_) | ExprKind::FuncCall(_) => return Ok(None),
+        ExprKind::Ident(_) | ExprKind::FuncCall(_) => return Ok(None),
 
         ExprKind::SString(_) => return Ok(None),
         ExprKind::FString(_) => TyKind::Primitive(PrimitiveSet::Text),
         ExprKind::Range(_) => return Ok(None), // TODO
 
         ExprKind::TransformCall(_) => return Ok(None), // TODO
         ExprKind::Tuple(fields) => TyKind::Tuple(
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/static_analysis.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/static_analysis.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/std.prql` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/semantic/std.prql`

 * *Files 1% similar despite different names*

```diff
@@ -116,25 +116,23 @@
   range:0..0
   expanding <bool>:false
   rolling <int>:0
   pipeline <transform>
   tbl <relation>
   -> <relation> internal window
 
-let noop = x -> x
-
 let append = `default_db.bottom`<relation> top<relation> -> <relation> internal append
 let intersect = `default_db.bottom`<relation> top<relation> -> <relation> (
-  noop t = top
-  join (noop b = bottom) (tuple_every (tuple_map _eq (tuple_zip t.* b.*)))
+  t = top
+  join (b = bottom) (tuple_every (tuple_map _eq (tuple_zip t.* b.*)))
   select t.*
 )
 let remove = `default_db.bottom`<relation> top<relation> -> <relation> (
-  noop t = top
-  join side:left (noop b = bottom) (tuple_every (tuple_map _eq (tuple_zip t.* b.*)))
+  t = top
+  join side:left (b = bottom) (tuple_every (tuple_map _eq (tuple_zip t.* b.*)))
   filter (tuple_every (tuple_map _is_null b.*))
   select t.*
 )
 let loop = func
   pipeline <transform>
   top <relation>
   -> <relation> internal loop
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/dialect.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/dialect.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_expr.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/gen_expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_projection.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/gen_projection.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_query.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/gen_query.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
     self as sql_ast, Join, JoinConstraint, JoinOperator, Select, SelectItem, SetExpr, TableAlias,
     TableFactor, TableWithJoins,
 };
 
 use crate::error::WithErrorInfo;
 use crate::ir::generic::InterpolateItem;
 use crate::ir::pl::{JoinSide, Literal};
-use crate::ir::rq::{CId, Expr, ExprKind, Query, RelationLiteral};
+use crate::ir::rq::{CId, Expr, ExprKind, RelationLiteral, RelationalQuery};
 use crate::utils::{BreakUp, Pluck};
 use crate::Error;
 
 use super::gen_expr::*;
 use super::gen_projection::*;
 use super::srq::ast::{Cte, CteKind, RelationExpr, RelationExprKind, SqlRelation, SqlTransform};
 
 use super::operators::translate_operator;
 use super::{Context, Dialect};
 
 type Transform = SqlTransform<RelationExpr, ()>;
 
-pub fn translate_query(query: Query, dialect: Option<Dialect>) -> Result<sql_ast::Query> {
+pub fn translate_query(query: RelationalQuery, dialect: Option<Dialect>) -> Result<sql_ast::Query> {
     // compile from RQ to SRQ
     let (srq_query, mut ctx) = super::srq::compile_query(query, dialect)?;
 
     let mut query = translate_relation(srq_query.main_relation, &mut ctx)?;
 
     if !srq_query.ctes.is_empty() {
         // attach CTEs
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/keywords.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/keywords.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 mod operators;
 mod srq;
 
 pub use dialect::{Dialect, SupportLevel};
 
 use anyhow::Result;
 
-use crate::{ir::rq::Query, Options, COMPILER_VERSION};
+use crate::{ir::rq::RelationalQuery, Options, COMPILER_VERSION};
 
 use self::dialect::DialectHandler;
 use self::srq::ast::Cte;
 use self::srq::context::AnchorContext;
 
 /// Translate a PRQL AST into a SQL string.
-pub fn compile(query: Query, options: &Options) -> Result<String> {
+pub fn compile(query: RelationalQuery, options: &Options) -> Result<String> {
     let crate::Target::Sql(dialect) = options.target;
     let sql_ast = gen_query::translate_query(query, dialect)?;
 
     let sql = sql_ast.to_string();
 
     // formatting
     let sql = if options.format {
@@ -56,36 +56,36 @@
 
     Ok(sql)
 }
 
 /// This module gives access to internal machinery that gives no stability guarantees.
 pub mod internal {
     use super::*;
-    use crate::ir::rq::{Query, Transform};
+    use crate::ir::rq::{RelationalQuery, Transform};
 
     pub use super::srq::ast::SqlTransform;
 
-    fn init(query: Query) -> Result<(Vec<Transform>, Context)> {
+    fn init(query: RelationalQuery) -> Result<(Vec<Transform>, Context)> {
         let (ctx, relation) = AnchorContext::of(query);
         let ctx = Context::new(dialect::Dialect::Generic, ctx);
 
         let pipeline = (relation.kind.into_pipeline())
             .map_err(|_| anyhow::anyhow!("Main RQ relation is not a pipeline."))?;
         Ok((pipeline, ctx))
     }
 
     /// Applies preprocessing to the main relation in RQ. Meant for debugging purposes.
-    pub fn preprocess(query: Query) -> Result<Vec<SqlTransform>> {
+    pub fn preprocess(query: RelationalQuery) -> Result<Vec<SqlTransform>> {
         let (pipeline, mut ctx) = init(query)?;
 
         srq::preprocess::preprocess(pipeline, &mut ctx)
     }
 
     /// Applies preprocessing and anchoring to the main relation in RQ. Meant for debugging purposes.
-    pub fn anchor(query: Query) -> Result<srq::ast::SqlQuery> {
+    pub fn anchor(query: RelationalQuery) -> Result<srq::ast::SqlQuery> {
         let (query, _ctx) = srq::compile_query(query, Some(dialect::Dialect::Generic))?;
         Ok(query)
     }
 }
 
 #[derive(Debug)]
 struct Context {
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/operators.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/operators.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/anchor.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/anchor.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/ast.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/ast.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/context.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/context.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 use anyhow::Result;
 use enum_as_inner::EnumAsInner;
 use serde::Serialize;
 
 use crate::ir::pl::Ident;
 use crate::ir::rq::{
-    fold_table, CId, Compute, Query, Relation, RelationColumn, RelationKind, RqFold, TId,
+    fold_table, CId, Compute, Relation, RelationColumn, RelationKind, RelationalQuery, RqFold, TId,
     TableDecl, TableRef, Transform,
 };
 
 use crate::utils::{IdGenerator, NameGenerator};
 
 use super::ast::{SqlRelation, SqlTransform};
 
@@ -118,15 +118,15 @@
     RelationColumn(RIId, CId, RelationColumn),
     Compute(Box<Compute>),
 }
 
 impl AnchorContext {
     /// Returns a new AnchorContext object based on a Query object. This method
     /// generates new IDs and names for tables and columns as needed.
-    pub fn of(query: Query) -> (Self, Relation) {
+    pub fn of(query: RelationalQuery) -> (Self, Relation) {
         let (cid, tid, query) = IdGenerator::load(query);
 
         let context = AnchorContext {
             cid,
             tid,
             riid: IdGenerator::new(),
             col_name: NameGenerator::new("_expr_"),
@@ -273,15 +273,15 @@
 
 /// Loads info about [Query] into [AnchorContext]
 struct QueryLoader {
     context: AnchorContext,
 }
 
 impl QueryLoader {
-    fn load(context: AnchorContext, query: Query) -> (AnchorContext, Relation) {
+    fn load(context: AnchorContext, query: RelationalQuery) -> (AnchorContext, Relation) {
         let mut loader = QueryLoader { context };
 
         for t in query.tables {
             loader.load_table(t).unwrap();
         }
         let relation = loader.fold_relation(query.relation).unwrap();
         (loader.context, relation)
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 use std::collections::HashSet;
 use std::str::FromStr;
 
 use anyhow::Result;
 use itertools::Itertools;
 
 use crate::ir::pl::Ident;
-use crate::ir::rq::{Query, RelationKind, RqFold, Transform};
+use crate::ir::rq::{RelationKind, RelationalQuery, RqFold, Transform};
 use crate::utils::BreakUp;
 use crate::Target;
 
 use super::anchor::{self, anchor_split};
 use super::ast::{
     fold_sql_transform, Cte, CteKind, RelationExpr, RelationExprKind, SqlQuery, SqlRelation,
     SqlTransform, SrqMapper,
 };
 use super::context::{AnchorContext, RIId, RelationAdapter, RelationStatus};
 
 use super::super::{Context, Dialect};
 use super::{postprocess, preprocess};
 
 pub(in super::super) fn compile_query(
-    query: Query,
+    query: RelationalQuery,
     dialect: Option<Dialect>,
 ) -> Result<(SqlQuery, Context)> {
     let dialect = if let Some(dialect) = dialect {
         dialect
     } else {
         let target = query.def.other.get("target");
         let Target::Sql(maybe_dialect) = target
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/std.sql.prql` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/sql/std.sql.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/tests/test.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs`

 * *Files 14% similar despite different names*

```diff
@@ -55,39 +55,29 @@
 
     // Really complicated error message for something so fundamental
     assert_display_snapshot!(compile(r###"
     select tracks
     from artists
     "###).unwrap_err(), @r###"
     Error:
-       ╭─[:2:5]
+       ╭─[:3:5]
        │
-     2 │ ╭─▶     select tracks
-     3 │ ├─▶     from artists
-       │ │
-       │ ╰────────────────────── main expected type `relation`, but found type `infer -> infer`
-       │
-       │     Help: Have you forgotten an argument to function main?
-       │
-       │     Note: Type `relation` expands to `[tuple_of_scalars]`
+     3 │     from artists
+       │     ──────┬─────
+       │           ╰─────── expected a function, but found `default_db.artists`
     ───╯
     "###);
 
     // It's better if we can tell them to put in {} braces
     assert_display_snapshot!(compile(r###"
     from artists
     sort -name
     "###).unwrap_err(), @r###"
-    Error:
-       ╭─[:3:11]
-       │
-     3 │     sort -name
-       │           ──┬─
-       │             ╰─── Unknown name
-    ───╯
+    Error: expected a pipeline that resolves to a table, but found `internal std.sub`
+    ↳ Hint: are you missing `from` statement?
     "###);
 }
 
 #[test]
 fn array_instead_of_tuple() {
     // Particularly given this used to be our syntax, this could be clearer
     // (though we do say so in the message, which is friendly!)
@@ -118,7 +108,46 @@
        │
      3 │     select f"{}"
        │              ┬
        │              ╰── unexpected end of input while parsing interpolated string
     ───╯
     "###);
 }
+
+#[test]
+fn select_with_extra_fstr() {
+    // Should complain in the same way as `select lower "mooo"`
+    assert_display_snapshot!(compile(r###"
+    from foo
+    select lower f"{x}/{y}"
+    "###).unwrap_err(), @r###"
+    Error:
+       ╭─[:3:20]
+       │
+     3 │     select lower f"{x}/{y}"
+       │                    ─┬─
+       │                     ╰─── Unknown name
+    ───╯
+    "###);
+}
+
+// See also test_error_messages::test_type_error_placement
+#[test]
+fn misplaced_type_error() {
+    // This one should point at `foo` in `select (... foo)`
+    // (preferably in addition to the error that is currently generated)
+    assert_display_snapshot!(compile(r###"
+    let foo = 123
+    from t
+    select (true && foo)
+    "###).unwrap_err(), @r###"
+    Error:
+       ╭─[:2:15]
+       │
+     2 │     let foo = 123
+       │               ─┬─
+       │                ╰─── function std.and, param `right` expected type `bool`, but found type `int`
+       │
+       │ Help: Type `bool` expands to `bool`
+    ───╯
+    "###);
+}
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_error_messages.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/tests/test_error_messages.rs`

 * *Files 9% similar despite different names*

```diff
@@ -185,14 +185,35 @@
      3 │     select (a && b) + c
        │             ───┬──
        │                ╰──── function std.add, param `left` expected type `int || float || timestamp || date`, but found type `bool`
     ───╯
     "###);
 }
 
+// See also test_bad_error_messages::misplaced_type_error
+// Note that the ``` Help: Type `bool` expands to `bool` ``` is not that useful
+#[test]
+fn test_type_error_placement() {
+    assert_display_snapshot!(compile(r###"
+    let foo = x -> (x | as integer)
+    from t
+    select (true && (foo y))
+    "###).unwrap_err(), @r###"
+    Error:
+       ╭─[:4:22]
+       │
+     4 │     select (true && (foo y))
+       │                      ──┬──
+       │                        ╰──── function std.and, param `right` expected type `bool`, but found type `scalar`
+       │
+       │ Help: Type `bool` expands to `bool`
+    ───╯
+    "###);
+}
+
 #[test]
 fn test_ambiguous() {
     assert_display_snapshot!(compile(r#"
     from a
     derive date = x
     select date
     "#)
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/id_gen.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/utils/id_gen.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::marker::PhantomData;
 
 use anyhow::Result;
 
-use crate::ir::rq::{fold_table, CId, Query, RqFold, TId, TableDecl};
+use crate::ir::rq::{fold_table, CId, RelationalQuery, RqFold, TId, TableDecl};
 
 #[derive(Debug, Clone)]
 pub struct IdGenerator<T: From<usize>> {
     next_id: usize,
     phantom: PhantomData<T>,
 }
 
@@ -33,15 +33,15 @@
             phantom: PhantomData,
         }
     }
 }
 
 impl IdGenerator<usize> {
     /// Returns a new id generators capable of generating new ids for given query.
-    pub fn load(query: Query) -> (IdGenerator<CId>, IdGenerator<TId>, Query) {
+    pub fn load(query: RelationalQuery) -> (IdGenerator<CId>, IdGenerator<TId>, RelationalQuery) {
         let mut loader = IdLoader {
             cid: IdGenerator::<CId>::default(),
             tid: IdGenerator::<TId>::default(),
         };
         let query = loader.fold_query(query).unwrap();
         (loader.cid, loader.tid, query)
     }
```

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/mod.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/toposort.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/src/utils/toposort.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/README.md` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/connection.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/connection.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/docker-compose.yml` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/main.rs` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/main.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap` & `prql_python-0.9.3/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/Cargo.toml` & `prql_python-0.9.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 name = "prql-python"
 publish = false
 
 edition= "2021"
 license= "Apache-2.0"
 repository= "https://github.com/PRQL/prql"
 rust-version= "1.65.0"
-version= "0.9.2"
+version= "0.9.3"
 
 [lib]
 crate-type = ["cdylib"]
 name = "prql_python"
 
 [target.'cfg(not(target_family="wasm"))'.dependencies]
 pyo3 = {version = "0.19.0", features = ["abi3-py37"]}
```

### Comparing `prql_python-0.9.2/.gitignore` & `prql_python-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/README.md` & `prql_python-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/noxfile.py` & `prql_python-0.9.3/noxfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     _install_prql_python(session)
     session.install("-v", "-r", "requirements.txt")
     session.run("pytest", str(Path("python", "tests")))
 
 
 @nox.session(python=VERSIONS)  # type: ignore[misc]
 def typing(session: Session) -> None:
-    """Run the test suite with pytest."""
+    """Check types with mypy"""
     _install_prql_python(session)
     session.install("mypy==1.4.0")
     session.run("mypy")
```

### Comparing `prql_python-0.9.2/pyproject.toml` & `prql_python-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/python/tests/test_all.py` & `prql_python-0.9.3/python/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/src/lib.rs` & `prql_python-0.9.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.2/PKG-INFO` & `prql_python-0.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prql-python
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/PRQL/prql
```

