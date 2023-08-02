# Comparing `tmp/autocorrect_py-2.8.0.tar.gz` & `tmp/autocorrect_py-2.8.3.tar.gz`

## Comparing `autocorrect_py-2.8.0.tar` & `autocorrect_py-2.8.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/Cargo.toml
--rw-r--r--   0      501       20     2482 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/.autocorrectrc.default
--rw-r--r--   0      501       20     1066 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/LICENSE
--rw-r--r--   0      501       20     5214 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/README.md
--rw-r--r--   0      501       20     6828 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/example.rs
--rw-r--r--   0      501       20     1906 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.html
--rw-r--r--   0      501       20      893 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.js
--rw-r--r--   0      501       20      279 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.json
--rw-r--r--   0      501       20     5194 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.md
--rw-r--r--   0      501       20     3094 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.yml
--rw-r--r--   0      501       20    97501 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/large.json
--rw-r--r--   0      501       20     1892 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/asciidoc.pest
--rw-r--r--   0      501       20      502 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/c.pest
--rw-r--r--   0      501       20      295 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/conf.pest
--rw-r--r--   0      501       20      603 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/csharp.pest
--rw-r--r--   0      501       20      342 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/css.pest
--rw-r--r--   0      501       20      618 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/dart.pest
--rw-r--r--   0      501       20      768 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/elixir.pest
--rw-r--r--   0      501       20      798 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/gettext.pest
--rw-r--r--   0      501       20      793 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/go.pest
--rw-r--r--   0      501       20     5199 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/html.pest
--rw-r--r--   0      501       20      600 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/java.pest
--rw-r--r--   0      501       20     1286 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/javascript.pest
--rw-r--r--   0      501       20     1326 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/json.pest
--rw-r--r--   0      501       20     1193 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/jupyter.pest
--rw-r--r--   0      501       20      611 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/kotlin.pest
--rw-r--r--   0      501       20      600 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/latex.pest
--rw-r--r--   0      501       20     4224 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/markdown.pest
--rw-r--r--   0      501       20      670 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/objective_c.pest
--rw-r--r--   0      501       20      763 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/php.pest
--rw-r--r--   0      501       20      721 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/python.pest
--rw-r--r--   0      501       20      647 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/ruby.pest
--rw-r--r--   0      501       20      579 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/rust.pest
--rw-r--r--   0      501       20      664 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/scala.pest
--rw-r--r--   0      501       20      420 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/sql.pest
--rw-r--r--   0      501       20      594 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/strings.pest
--rw-r--r--   0      501       20      794 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/swift.pest
--rw-r--r--   0      501       20      589 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/xml.pest
--rw-r--r--   0      501       20      696 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/yaml.pest
--rw-r--r--   0      501       20       89 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/release.toml
--rw-r--r--   0      501       20     3533 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/asciidoc.rs
--rw-r--r--   0      501       20     1482 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/c.rs
--rw-r--r--   0      501       20    12808 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/code.rs
--rw-r--r--   0      501       20      987 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/conf.rs
--rw-r--r--   0      501       20     1563 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/csharp.rs
--rw-r--r--   0      501       20     1315 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/css.rs
--rw-r--r--   0      501       20     1639 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/dart.rs
--rw-r--r--   0      501       20     1717 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/elixir.rs
--rw-r--r--   0      501       20     1528 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/gettext.rs
--rw-r--r--   0      501       20     1716 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/go.rs
--rw-r--r--   0      501       20     9557 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/html.rs
--rw-r--r--   0      501       20     1628 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/java.rs
--rw-r--r--   0      501       20     7364 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/javascript.rs
--rw-r--r--   0      501       20     1649 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/json.rs
--rw-r--r--   0      501       20    11585 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/jupyter.rs
--rw-r--r--   0      501       20     1446 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/kotlin.rs
--rw-r--r--   0      501       20     4600 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/latex.rs
--rw-r--r--   0      501       20    12553 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/markdown.rs
--rw-r--r--   0      501       20     4458 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/mod.rs
--rw-r--r--   0      501       20     1453 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/objective_c.rs
--rw-r--r--   0      501       20     1723 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/php.rs
--rw-r--r--   0      501       20     1598 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/python.rs
--rw-r--r--   0      501       20     1174 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/ruby.rs
--rw-r--r--   0      501       20     2502 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/rust.rs
--rw-r--r--   0      501       20     1627 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/scala.rs
--rw-r--r--   0      501       20     1294 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/sql.rs
--rw-r--r--   0      501       20     1318 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/strings.rs
--rw-r--r--   0      501       20     1796 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/swift.rs
--rw-r--r--   0      501       20     4816 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/types.rs
--rw-r--r--   0      501       20     1253 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/xml.rs
--rw-r--r--   0      501       20     1077 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/yaml.rs
--rw-r--r--   0      501       20    13723 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/mod.rs
--rw-r--r--   0      501       20     3000 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/severity.rs
--rw-r--r--   0      501       20     2136 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/spellcheck.rs
--rw-r--r--   0      501       20      407 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/toggle.pest
--rw-r--r--   0      501       20     8865 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/toggle.rs
--rw-r--r--   0      501       20     6309 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/diff.rs
--rw-r--r--   0      501       20    19238 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/format.rs
--rw-r--r--   0      501       20     1592 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/ignorer.rs
--rw-r--r--   0      501       20     4682 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/lib.rs
--rw-r--r--   0      501       20     1609 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/json.rs
--rw-r--r--   0      501       20     8773 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/mod.rs
--rw-r--r--   0      501       20     4670 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/rdjson.rs
--rw-r--r--   0      501       20     4766 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/fullwidth.rs
--rw-r--r--   0      501       20    13453 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/halfwidth.rs
--rw-r--r--   0      501       20    10177 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/mod.rs
--rw-r--r--   0      501       20     2733 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/rule.rs
--rw-r--r--   0      501       20     3967 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/spellcheck.rs
--rw-r--r--   0      501       20     2192 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/strategery.rs
--rw-r--r--   0      501       20     2968 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/word.rs
--rw-r--r--   0      501       20     1563 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/de.rs
--rw-r--r--   0      501       20      713 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/error.rs
--rw-r--r--   0      501       20       52 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/mod.rs
--rw-r--r--   0      501       20      453 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/.autocorrectrc.test
--rw-r--r--   0      501       20     7914 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json
--rw-r--r--   0      501       20    16656 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt
--rw-r--r--   0      501       20    16591 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb
--rw-r--r--   0      501       20      849 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb
--rw-r--r--   0      501       20      644 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/format.rs
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect-derive/Cargo.toml
--rw-r--r--   0      501       20     1153 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect-derive/src/lib.rs
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/Cargo.toml
--rw-r--r--   0      501       20     3078 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/.gitignore
--rw-r--r--   0      501       20     1603 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/README.md
--rw-r--r--   0      501       20      601 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/autocorrect_py.pyi
--rw-r--r--   0      501       20       76 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/pyproject.toml
--rw-r--r--   0      501       20     3660 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/src/lib.rs
--rw-r--r--   0      501       20     1461 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/test_autocorrect_py.py
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect-derive/Cargo.toml
+-rw-r--r--   0      501       20     1153 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect-derive/src/lib.rs
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/Cargo.toml
+-rw-r--r--   0      501       20     2482 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/.autocorrectrc.default
+-rw-r--r--   0      501       20     1066 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/LICENSE
+-rw-r--r--   0      501       20     5214 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/README.md
+-rw-r--r--   0      501       20     6828 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/example.rs
+-rw-r--r--   0      501       20     1906 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.html
+-rw-r--r--   0      501       20      893 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.js
+-rw-r--r--   0      501       20      279 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.json
+-rw-r--r--   0      501       20     5194 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.md
+-rw-r--r--   0      501       20     3094 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.yml
+-rw-r--r--   0      501       20    97501 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/large.json
+-rw-r--r--   0      501       20     1892 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/asciidoc.pest
+-rw-r--r--   0      501       20      502 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/c.pest
+-rw-r--r--   0      501       20      295 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/conf.pest
+-rw-r--r--   0      501       20      603 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/csharp.pest
+-rw-r--r--   0      501       20      342 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/css.pest
+-rw-r--r--   0      501       20      618 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/dart.pest
+-rw-r--r--   0      501       20      768 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/elixir.pest
+-rw-r--r--   0      501       20      798 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/gettext.pest
+-rw-r--r--   0      501       20      793 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/go.pest
+-rw-r--r--   0      501       20     5199 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/html.pest
+-rw-r--r--   0      501       20      600 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/java.pest
+-rw-r--r--   0      501       20     1286 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/javascript.pest
+-rw-r--r--   0      501       20     1326 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/json.pest
+-rw-r--r--   0      501       20     1193 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/jupyter.pest
+-rw-r--r--   0      501       20      611 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/kotlin.pest
+-rw-r--r--   0      501       20      600 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/latex.pest
+-rw-r--r--   0      501       20     4224 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/markdown.pest
+-rw-r--r--   0      501       20      670 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/objective_c.pest
+-rw-r--r--   0      501       20      763 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/php.pest
+-rw-r--r--   0      501       20      721 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/python.pest
+-rw-r--r--   0      501       20      647 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/ruby.pest
+-rw-r--r--   0      501       20      579 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/rust.pest
+-rw-r--r--   0      501       20      664 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/scala.pest
+-rw-r--r--   0      501       20      420 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/sql.pest
+-rw-r--r--   0      501       20      594 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/strings.pest
+-rw-r--r--   0      501       20      794 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/swift.pest
+-rw-r--r--   0      501       20      589 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/xml.pest
+-rw-r--r--   0      501       20      696 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/yaml.pest
+-rw-r--r--   0      501       20       89 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/release.toml
+-rw-r--r--   0      501       20     3533 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/asciidoc.rs
+-rw-r--r--   0      501       20     1482 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/c.rs
+-rw-r--r--   0      501       20    12808 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/code.rs
+-rw-r--r--   0      501       20      987 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/conf.rs
+-rw-r--r--   0      501       20     1563 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/csharp.rs
+-rw-r--r--   0      501       20     1315 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/css.rs
+-rw-r--r--   0      501       20     1639 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/dart.rs
+-rw-r--r--   0      501       20     1717 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/elixir.rs
+-rw-r--r--   0      501       20     1528 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/gettext.rs
+-rw-r--r--   0      501       20     1716 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/go.rs
+-rw-r--r--   0      501       20     9557 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/html.rs
+-rw-r--r--   0      501       20     1628 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/java.rs
+-rw-r--r--   0      501       20     7364 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/javascript.rs
+-rw-r--r--   0      501       20     1649 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/json.rs
+-rw-r--r--   0      501       20    11585 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/jupyter.rs
+-rw-r--r--   0      501       20     1446 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/kotlin.rs
+-rw-r--r--   0      501       20     4600 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/latex.rs
+-rw-r--r--   0      501       20    12553 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/markdown.rs
+-rw-r--r--   0      501       20     4458 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/mod.rs
+-rw-r--r--   0      501       20     1453 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/objective_c.rs
+-rw-r--r--   0      501       20     1723 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/php.rs
+-rw-r--r--   0      501       20     1598 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/python.rs
+-rw-r--r--   0      501       20     1174 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/ruby.rs
+-rw-r--r--   0      501       20     2502 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/rust.rs
+-rw-r--r--   0      501       20     1627 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/scala.rs
+-rw-r--r--   0      501       20     1294 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/sql.rs
+-rw-r--r--   0      501       20     1318 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/strings.rs
+-rw-r--r--   0      501       20     1796 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/swift.rs
+-rw-r--r--   0      501       20     4816 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/types.rs
+-rw-r--r--   0      501       20     1253 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/xml.rs
+-rw-r--r--   0      501       20     1077 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/yaml.rs
+-rw-r--r--   0      501       20    13723 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/mod.rs
+-rw-r--r--   0      501       20     3000 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/severity.rs
+-rw-r--r--   0      501       20     2136 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/spellcheck.rs
+-rw-r--r--   0      501       20      407 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/toggle.pest
+-rw-r--r--   0      501       20     8865 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/toggle.rs
+-rw-r--r--   0      501       20     6309 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/diff.rs
+-rw-r--r--   0      501       20    19238 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/format.rs
+-rw-r--r--   0      501       20     1592 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/ignorer.rs
+-rw-r--r--   0      501       20     4682 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/lib.rs
+-rw-r--r--   0      501       20     1666 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/result/json.rs
+-rw-r--r--   0      501       20     8773 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/result/mod.rs
+-rw-r--r--   0      501       20     4809 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/result/rdjson.rs
+-rw-r--r--   0      501       20     4766 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/fullwidth.rs
+-rw-r--r--   0      501       20    13453 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/halfwidth.rs
+-rw-r--r--   0      501       20    10177 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/mod.rs
+-rw-r--r--   0      501       20     2733 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/rule.rs
+-rw-r--r--   0      501       20     3967 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/spellcheck.rs
+-rw-r--r--   0      501       20     2192 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/strategery.rs
+-rw-r--r--   0      501       20     2968 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/word.rs
+-rw-r--r--   0      501       20     1563 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/serde_any/de.rs
+-rw-r--r--   0      501       20      713 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/serde_any/error.rs
+-rw-r--r--   0      501       20       52 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/src/serde_any/mod.rs
+-rw-r--r--   0      501       20      453 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/.autocorrectrc.test
+-rw-r--r--   0      501       20     7914 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json
+-rw-r--r--   0      501       20    16656 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt
+-rw-r--r--   0      501       20    16591 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb
+-rw-r--r--   0      501       20      849 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb
+-rw-r--r--   0      501       20      644 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/format.rs
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 autocorrect_py-2.8.3/Cargo.toml
+-rw-r--r--   0      501       20     3078 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/.gitignore
+-rw-r--r--   0      501       20     1603 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/README.md
+-rw-r--r--   0      501       20      601 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/autocorrect_py.pyi
+-rw-r--r--   0      501       20       76 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/pyproject.toml
+-rw-r--r--   0      501       20     3660 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/src/lib.rs
+-rw-r--r--   0      501       20     1461 2023-08-02 00:32:13.000000 autocorrect_py-2.8.3/test_autocorrect_py.py
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 autocorrect_py-2.8.3/PKG-INFO
```

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/Cargo.toml` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 edition = "2021"
 homepage = "https://github.com/huacnlee/autocorrect"
 keywords = ["autocorrect", "lint", "format"]
 license = "MIT"
 name = "autocorrect"
 readme = "../README.md"
 repository = "https://github.com/huacnlee/autocorrect"
-version = "2.8.0"
+version = "2.8.3"
 
 [lib]
 name = "autocorrect"
 path = "src/lib.rs"
 
 [dependencies]
 autocorrect-derive = {version = "0.3.0", path = "../autocorrect-derive" }
```

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/.autocorrectrc.default` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/.autocorrectrc.default`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/LICENSE` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/LICENSE`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/README.md` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/README.md`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/example.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/example.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.html` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.html`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.js` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.js`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.md` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.md`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.yml` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/example.yml`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/large.json` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/benches/fixtures/large.json`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/asciidoc.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/asciidoc.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/csharp.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/csharp.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/dart.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/dart.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/elixir.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/elixir.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/gettext.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/gettext.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/go.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/go.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/html.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/html.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/java.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/java.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/javascript.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/javascript.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/json.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/json.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/jupyter.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/jupyter.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/kotlin.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/kotlin.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/latex.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/latex.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/markdown.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/markdown.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/objective_c.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/objective_c.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/php.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/php.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/python.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/python.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/ruby.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/ruby.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/rust.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/rust.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/scala.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/scala.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/strings.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/strings.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/swift.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/swift.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/xml.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/xml.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/yaml.pest` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/grammar/yaml.pest`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/asciidoc.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/asciidoc.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/c.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/c.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/code.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/code.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/conf.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/conf.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/csharp.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/csharp.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/css.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/css.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/dart.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/dart.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/elixir.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/elixir.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/gettext.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/gettext.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/go.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/go.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/html.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/html.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/java.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/java.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/javascript.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/javascript.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/json.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/json.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/jupyter.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/jupyter.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/kotlin.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/kotlin.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/latex.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/latex.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/markdown.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/markdown.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/mod.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/mod.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/objective_c.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/objective_c.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/php.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/php.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/python.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/python.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/ruby.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/ruby.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/rust.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/rust.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/scala.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/scala.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/sql.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/sql.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/strings.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/strings.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/swift.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/swift.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/types.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/types.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/xml.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/xml.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/yaml.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/code/yaml.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/mod.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/mod.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/severity.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/severity.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/spellcheck.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/spellcheck.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/toggle.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/config/toggle.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/diff.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/diff.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/format.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/format.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/ignorer.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/ignorer.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/lib.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/lib.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/json.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/result/json.rs`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 }
 
 #[cfg(test)]
 pub(crate) fn crate_test_lint_results() -> Vec<LintResult> {
     use crate::result::{LineResult, Results, Severity};
 
     let mut lint_result = LintResult::new("hello你好.\n这是第2行");
-    lint_result.filepath = "test/foo/bar.rs".to_owned();
+    lint_result.line = 10;
+    lint_result.col = 12;
+    lint_result.filepath = "./test/foo/bar.rs".to_owned();
     lint_result.push(LineResult {
         line: 1,
         col: 1,
         new: "hello 你好。".to_owned(),
         old: "hello你好.".to_owned(),
         severity: Severity::Error,
     });
@@ -40,14 +42,14 @@
 
 #[cfg(test)]
 mod tests {
     #[test]
     fn test_to_lint_results_json() {
         let json = super::to_lint_results_json(crate::result::json::crate_test_lint_results());
 
-        let expected = r#"{"count": 1,"messages": [{"filepath":"test/foo/bar.rs","lines":[{"l":1,"c":1,"new":"hello 你好。","old":"hello你好.","severity":1},{"l":2,"c":1,"new":"这是第 2 行","old":"这是第2行","severity":1}],"error":""}]}"#;
+        let expected = r#"{"count": 1,"messages": [{"filepath":"./test/foo/bar.rs","lines":[{"l":1,"c":1,"new":"hello 你好。","old":"hello你好.","severity":1},{"l":2,"c":1,"new":"这是第 2 行","old":"这是第2行","severity":1}],"error":""}]}"#;
         if expected != json {
             println!("--------------- json:\n{}", json);
         }
         assert_json_eq!(expected, json);
     }
 }
```

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/mod.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/result/mod.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/rdjson.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/result/rdjson.rs`

 * *Files 11% similar despite different names*

```diff
@@ -63,40 +63,41 @@
     }
 }
 
 /// RDF JSONSchema
 /// https://github.com/reviewdog/reviewdog/blob/master/proto/rdf/jsonschema/Diagnostic.jsonschema
 #[doc(hidden)]
 pub(crate) fn to_rdjson_diagnostic(lint_result: &LintResult, pretty: bool) -> String {
-    let range = RdfRange {
-        start: Some(RdfLineColumn {
-            line: lint_result.line,
-            column: lint_result.col,
-        }),
-        end: None,
-    };
-
     let mut rdf_diagnostic: RdfDiagnostic = RdfDiagnostic {
         message: "".to_owned(),
         location: RdfLocation {
-            path: lint_result.filepath.clone(),
-            range: range.clone(),
+            path: lint_result.filepath.replace("./", ""),
+            range: RdfRange {
+                start: None,
+                end: None,
+            },
         },
         severity: "UNKNOWN_SEVERITY".to_owned(),
         code: RdfCode {
             value: Some("AutoCorrect".to_owned()),
             url: "https://github.com/huacnlee/autocorrect".to_owned(),
         },
         suggestions: vec![],
     };
 
     lint_result.lines.iter().for_each(|line_result| {
         if rdf_diagnostic.severity == "UNKNOWN_SEVERITY" {
             rdf_diagnostic.severity = to_severity_str(line_result.severity);
         }
+        if rdf_diagnostic.location.range.start.is_none() {
+            rdf_diagnostic.location.range.start = Some(RdfLineColumn {
+                line: line_result.line,
+                column: line_result.col,
+            });
+        }
 
         let suggestion = RdfSuggetion {
             text: line_result.new.clone(),
             range: RdfRange {
                 start: Some(RdfLineColumn {
                     line: line_result.line,
                     column: line_result.col,
```

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/fullwidth.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/fullwidth.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/halfwidth.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/halfwidth.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/mod.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/rule.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/rule.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/spellcheck.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/spellcheck.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/strategery.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/strategery.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/word.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/rule/word.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/de.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/serde_any/de.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/error.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/src/serde_any/error.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/format.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect/tests/format.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/local_dependencies/autocorrect-derive/src/lib.rs` & `autocorrect_py-2.8.3/local_dependencies/autocorrect-derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/Cargo.toml` & `autocorrect_py-2.8.3/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 description = "A linter and formatter for help you improve copywriting, to correct spaces, words, punctuations between CJK (Chinese, Japanese, Korean)."
 edition = "2018"
 homepage = "https://github.com/huacnlee/autocorrect"
 license = "MIT"
 name = "autocorrect-py"
 readme = "README.md"
 repository = "https://github.com/huacnlee/autocorrect"
-version = "2.8.0"
+version = "2.8.3"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 name = "autocorrect_py"
 
 [dependencies]
```

### Comparing `autocorrect_py-2.8.0/.gitignore` & `autocorrect_py-2.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/README.md` & `autocorrect_py-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/autocorrect_py.pyi` & `autocorrect_py-2.8.3/autocorrect_py.pyi`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/src/lib.rs` & `autocorrect_py-2.8.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/test_autocorrect_py.py` & `autocorrect_py-2.8.3/test_autocorrect_py.py`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.8.0/PKG-INFO` & `autocorrect_py-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocorrect-py
-Version: 2.8.0
+Version: 2.8.3
 Summary: A linter and formatter for help you improve copywriting, to correct spaces, words, punctuations between CJK (Chinese, Japanese, Korean).
 Home-Page: https://github.com/huacnlee/autocorrect
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/huacnlee/autocorrect
 
 # AutoCorrect for Python
```

