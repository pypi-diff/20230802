# Comparing `tmp/pjplan-0.0.8.tar.gz` & `tmp/pjplan-0.0.9.tar.gz`

## Comparing `pjplan-0.0.8.tar` & `pjplan-0.0.9.tar`

### file list

```diff
@@ -1,109 +1,131 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pjplan-0.0.8/.env
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pjplan-0.0.8/install.bat
--rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.8/publish.bat
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pjplan-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/Makefile
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/conf.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/make.bat
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/modules.rst
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.io.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.rst
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.viz.dhtmlx.rst
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.viz.mermaid.rst
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.viz.rst
--rw-r--r--   0        0        0   446858 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0   196365 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.doctree
--rw-r--r--   0        0        0    33626 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.io.doctree
--rw-r--r--   0        0        0    22463 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.dhtmlx.doctree
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.doctree
--rw-r--r--   0        0        0    18945 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.mermaid.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    20224 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/index.html
--rw-r--r--   0        0        0    19015 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/modules.html
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/objects.inv
--rw-r--r--   0        0        0    75565 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.html
--rw-r--r--   0        0        0    14983 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.io.html
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.viz.dhtmlx.html
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.viz.html
--rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.viz.mermaid.html
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/search.html
--rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.io.rst.txt
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.rst.txt
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.viz.dhtmlx.rst.txt
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.viz.mermaid.rst.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.viz.rst.txt
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_static/img/readme/mermaid_gantt.png
--rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_static/img/readme/mermaid_network.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/README.md
--rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/calendar/calendar.ipynb
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb
--rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/critical-path/critical-path.ipynb
--rw-r--r--   0        0        0    93575 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb
--rw-r--r--   0        0        0    80191 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/forward-scheduler/forward-scheduler.ipynb
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/getting-started/getting-started.ipynb
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/getting-started/gs.html
--rw-r--r--   0        0        0    10375 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/mermaid-network/mermaid-network.ipynb
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/pandas/pandas.ipynb
--rw-r--r--   0        0        0    23893 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/print/print.ipynb
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/dhtmlx-gantt/main.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/dhtmlx-gantt/.streamlit/config.toml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-gantt/main.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-gantt/.streamlit/config.toml
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-network/main.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-network/.streamlit/config.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/__init__.py
--rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/calendar.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/resource.py
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/schedule.py
--rw-r--r--   0        0        0    31938 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/task.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/utils.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/wbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/alg/__init__.py
--rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/alg/critical_path.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/io/__init__.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/io/csv_io.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/io/raw.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/dhtmlx/__init__.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/dhtmlx/gantt.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/dhtmlx/templates/gantt.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/__init__.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/gantt.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/network.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/templates/gantt.html
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/templates/network.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/__init__.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_calendar.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_schedule.py
--rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_task.py
--rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_wbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_io/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_io/test_csv_io.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pjplan-0.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pjplan-0.0.8/LICENSE
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pjplan-0.0.8/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pjplan-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 pjplan-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pjplan-0.0.9/.env
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pjplan-0.0.9/.readthedocs.yml
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pjplan-0.0.9/install.bat
+-rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.9/publish.bat
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pjplan-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/requirements.in
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0   106081 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0    10251 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/en/index.doctree
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/en/installation.doctree
+-rw-r--r--   0        0        0    16101 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/en/getting-started/getting-started.doctree
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/nbsphinx/en/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/nbsphinx/ru/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0    14700 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/ru/index.doctree
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/ru/installation.doctree
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/ru/toc.doctree
+-rw-r--r--   0        0        0    16465 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/ru/getting-started/getting-started.doctree
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/doctrees/ttt/index.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/index.html
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/search.html
+-rw-r--r--   0        0        0    15902 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/en/index.md.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/en/installation.md.txt
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/en/getting-started/getting-started.ipynb.txt
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/ru/index.md.txt
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/ru/index.rst.txt
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/ru/installation.md.txt
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/ru/toc.md.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/ru/toc.rst.txt
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/ru/getting-started/getting-started.ipynb.txt
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_sources/ttt/index.rst.txt
+-rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15716 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/img/readme/mermaid_gantt.png
+-rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/_static/img/readme/mermaid_network.png
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/en/index.html
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/en/installation.html
+-rw-r--r--   0        0        0    14671 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/en/getting-started/getting-started.html
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/en/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/ru/index.html
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/ru/installation.html
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/ru/toc.html
+-rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/ru/getting-started/getting-started.html
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/ru/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_build/html/ttt/index.html
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_static/img/readme/mermaid_gantt.png
+-rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/_static/img/readme/mermaid_network.png
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/en/index.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/en/installation.md
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/en/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/ru/index.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/ru/installation.md
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 pjplan-0.0.9/docs/ru/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/README.md
+-rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/calendar/calendar.ipynb
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb
+-rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/critical-path/critical-path.ipynb
+-rw-r--r--   0        0        0    93575 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb
+-rw-r--r--   0        0        0    80191 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/forward-scheduler/forward-scheduler.ipynb
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/getting-started/gs.html
+-rw-r--r--   0        0        0    10375 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/mermaid-network/mermaid-network.ipynb
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/pandas/pandas.ipynb
+-rw-r--r--   0        0        0    23893 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/jupyter/print/print.ipynb
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/streamlit/dhtmlx-gantt/g.html
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/streamlit/dhtmlx-gantt/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/streamlit/dhtmlx-gantt/.streamlit/config.toml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/streamlit/mermaid-gantt/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/streamlit/mermaid-gantt/.streamlit/config.toml
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/streamlit/mermaid-network/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.9/examples/streamlit/mermaid-network/.streamlit/config.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/__init__.py
+-rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/calendar.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/resource.py
+-rw-r--r--   0        0        0    17623 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/schedule.py
+-rw-r--r--   0        0        0    32827 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/task.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/utils.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/wbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/alg/__init__.py
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/alg/critical_path.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/io/__init__.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/io/csv_io.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/io/raw.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/dhtmlx/__init__.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/dhtmlx/gantt.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/dhtmlx/templates/gantt.html
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/dhtmlx/templates/resource_usage.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/mermaid/__init__.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/mermaid/gantt.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/mermaid/network.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/mermaid/templates/gantt.html
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pjplan-0.0.9/src/pjplan/viz/mermaid/templates/network.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.9/tests/test_pjplan/__init__.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pjplan-0.0.9/tests/test_pjplan/test_calendar.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 pjplan-0.0.9/tests/test_pjplan/test_schedule.py
+-rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 pjplan-0.0.9/tests/test_pjplan/test_task.py
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 pjplan-0.0.9/tests/test_pjplan/test_wbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.9/tests/test_pjplan/test_io/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pjplan-0.0.9/tests/test_pjplan/test_io/test_csv_io.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pjplan-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pjplan-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 pjplan-0.0.9/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pjplan-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 pjplan-0.0.9/PKG-INFO
```

### Comparing `pjplan-0.0.8/docs/Makefile` & `pjplan-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/make.bat` & `pjplan-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/_build/doctrees/index.doctree` & `pjplan-0.0.9/docs/_build/doctrees/ttt/index.doctree`

 * *Files 9% similar despite different names*

```diff
@@ -1,349 +1,306 @@
-00000000: 8005 95c1 1500 0000 0000 008c 0f73 7068  .............sph
+00000000: 8005 9507 1300 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
-00000070: 6805 8ccb 706a 706c 616e 2064 6f63 756d  h...pjplan docum
-00000080: 656e 7461 7469 6f6e 206d 6173 7465 7220  entation master 
-00000090: 6669 6c65 2c20 6372 6561 7465 6420 6279  file, created by
-000000a0: 0a73 7068 696e 782d 7175 6963 6b73 7461  .sphinx-quicksta
-000000b0: 7274 206f 6e20 5475 6520 4d61 7220 3238  rt on Tue Mar 28
-000000c0: 2032 333a 3235 3a33 3320 3230 3233 2e0a   23:25:33 2023..
-000000d0: 596f 7520 6361 6e20 6164 6170 7420 7468  You can adapt th
-000000e0: 6973 2066 696c 6520 636f 6d70 6c65 7465  is file complete
-000000f0: 6c79 2074 6f20 796f 7572 206c 696b 696e  ly to your likin
-00000100: 672c 2062 7574 2069 7420 7368 6f75 6c64  g, but it should
-00000110: 2061 7420 6c65 6173 740a 636f 6e74 6169   at least.contai
-00000120: 6e20 7468 6520 726f 6f74 2060 746f 6374  n the root `toct
-00000130: 7265 6560 2064 6972 6563 7469 7665 2e94  ree` directive..
-00000140: 6807 5d94 6809 8c04 5465 7874 9493 948c  h.].h...Text....
-00000150: cb70 6a70 6c61 6e20 646f 6375 6d65 6e74  .pjplan document
-00000160: 6174 696f 6e20 6d61 7374 6572 2066 696c  ation master fil
-00000170: 652c 2063 7265 6174 6564 2062 790a 7370  e, created by.sp
-00000180: 6869 6e78 2d71 7569 636b 7374 6172 7420  hinx-quickstart 
-00000190: 6f6e 2054 7565 204d 6172 2032 3820 3233  on Tue Mar 28 23
-000001a0: 3a32 353a 3333 2032 3032 332e 0a59 6f75  :25:33 2023..You
-000001b0: 2063 616e 2061 6461 7074 2074 6869 7320   can adapt this 
-000001c0: 6669 6c65 2063 6f6d 706c 6574 656c 7920  file completely 
-000001d0: 746f 2079 6f75 7220 6c69 6b69 6e67 2c20  to your liking, 
-000001e0: 6275 7420 6974 2073 686f 756c 6420 6174  but it should at
-000001f0: 206c 6561 7374 0a63 6f6e 7461 696e 2074   least.contain t
-00000200: 6865 2072 6f6f 7420 6074 6f63 7472 6565  he root `toctree
-00000210: 6020 6469 7265 6374 6976 652e 9485 9481  ` directive.....
-00000220: 947d 948c 0670 6172 656e 7494 680c 7362  .}...parent.h.sb
-00000230: 618c 0a61 7474 7269 6275 7465 7394 7d94  a..attributes.}.
-00000240: 288c 0369 6473 945d 948c 0763 6c61 7373  (..ids.]...class
-00000250: 6573 945d 948c 056e 616d 6573 945d 948c  es.]...names.]..
-00000260: 0864 7570 6e61 6d65 7394 5d94 8c08 6261  .dupnames.]...ba
-00000270: 636b 7265 6673 945d 948c 0978 6d6c 3a73  ckrefs.]...xml:s
-00000280: 7061 6365 948c 0870 7265 7365 7276 6594  pace...preserve.
-00000290: 758c 0774 6167 6e61 6d65 9468 0a68 1668  u..tagname.h.h.h
-000002a0: 038c 095f 646f 6375 6d65 6e74 9468 038c  ..._document.h..
-000002b0: 0673 6f75 7263 6594 8c28 443a 5c68 6f6d  .source..(D:\hom
-000002c0: 655c 7079 7072 6f6a 6563 7473 5c70 6a70  e\pyprojects\pjp
-000002d0: 6c61 6e5c 646f 6373 5c69 6e64 6578 2e72  lan\docs\index.r
-000002e0: 7374 948c 046c 696e 6594 4b05 7562 6809  st...line.K.ubh.
-000002f0: 8c07 7365 6374 696f 6e94 9394 2981 947d  ..section...)..}
-00000300: 9428 6805 6806 6807 5d94 2868 098c 0574  .(h.h.h.].(h...t
-00000310: 6974 6c65 9493 9429 8194 7d94 2868 058c  itle...)..}.(h..
-00000320: 2257 656c 636f 6d65 2074 6f20 706a 706c  "Welcome to pjpl
-00000330: 616e 2773 2064 6f63 756d 656e 7461 7469  an's documentati
-00000340: 6f6e 2194 6807 5d94 6811 8c24 5765 6c63  on!.h.].h..$Welc
-00000350: 6f6d 6520 746f 2070 6a70 6c61 6ee2 8099  ome to pjplan...
-00000360: 7320 646f 6375 6d65 6e74 6174 696f 6e21  s documentation!
-00000370: 9485 9481 947d 9428 6816 6831 6826 6803  .....}.(h.h1h&h.
-00000380: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
-00000390: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-000003a0: 5d94 7568 2568 2f68 1668 2c68 2668 0368  ].uh%h/h.h,h&h.h
-000003b0: 2768 2868 294b 0775 6268 098c 0863 6f6d  'h(h)K.ubh...com
-000003c0: 706f 756e 6494 9394 2981 947d 9428 6805  pound...)..}.(h.
-000003d0: 6806 6807 5d94 6800 8c07 746f 6374 7265  h.h.].h...toctre
-000003e0: 6594 9394 2981 947d 9428 6805 6806 6807  e...)..}.(h.h.h.
-000003f0: 5d94 6817 7d94 2868 195d 9468 1b5d 9468  ].h.}.(h.].h.].h
-00000400: 1d5d 9468 1f5d 9468 215d 9468 168c 0569  .].h.].h!].h...i
-00000410: 6e64 6578 948c 0765 6e74 7269 6573 945d  ndex...entries.]
-00000420: 944e 8c07 6d6f 6475 6c65 7394 8694 618c  .N..modules...a.
-00000430: 0c69 6e63 6c75 6465 6669 6c65 7394 5d94  .includefiles.].
-00000440: 6852 618c 086d 6178 6465 7074 6894 4b02  hRa..maxdepth.K.
-00000450: 8c07 6361 7074 696f 6e94 8c09 436f 6e74  ..caption...Cont
-00000460: 656e 7473 3a94 8c04 676c 6f62 9489 8c06  ents:...glob....
-00000470: 6869 6464 656e 9489 8c0d 696e 636c 7564  hidden....includ
-00000480: 6568 6964 6465 6e94 898c 086e 756d 6265  ehidden....numbe
-00000490: 7265 6494 4b00 8c0a 7469 746c 6573 6f6e  red.K...titleson
-000004a0: 6c79 9489 8c0a 7261 7765 6e74 7269 6573  ly....rawentries
-000004b0: 945d 948c 0a72 6177 6361 7074 696f 6e94  .]...rawcaption.
-000004c0: 6858 7568 2568 4468 2768 2868 294b 0968  hXuh%hDh'h(h)K.h
-000004d0: 1668 4175 6261 6817 7d94 2868 195d 9468  .hAubah.}.(h.].h
-000004e0: 1b5d 948c 0f74 6f63 7472 6565 2d77 7261  .]...toctree-wra
-000004f0: 7070 6572 9461 681d 5d94 681f 5d94 6821  pper.ah.].h.].h!
-00000500: 5d94 7568 2568 3f68 1668 2c68 2668 0368  ].uh%h?h.h,h&h.h
-00000510: 2768 2868 294e 7562 6568 177d 9428 6819  'h(h)Nubeh.}.(h.
-00000520: 5d94 8c21 7765 6c63 6f6d 652d 746f 2d70  ]..!welcome-to-p
-00000530: 6a70 6c61 6e2d 732d 646f 6375 6d65 6e74  jplan-s-document
-00000540: 6174 696f 6e94 6168 1b5d 9468 1d5d 948c  ation.ah.].h.]..
-00000550: 2277 656c 636f 6d65 2074 6f20 706a 706c  "welcome to pjpl
-00000560: 616e 2773 2064 6f63 756d 656e 7461 7469  an's documentati
-00000570: 6f6e 2194 6168 1f5d 9468 215d 9475 6825  on!.ah.].h!].uh%
-00000580: 682a 6816 6803 6826 6803 6827 6828 6829  h*h.h.h&h.h'h(h)
-00000590: 4b07 7562 682b 2981 947d 9428 6805 6806  K.ubh+)..}.(h.h.
-000005a0: 6807 5d94 2868 3029 8194 7d94 2868 058c  h.].(h0)..}.(h..
-000005b0: 1249 6e64 6963 6573 2061 6e64 2074 6162  .Indices and tab
-000005c0: 6c65 7394 6807 5d94 6811 8c12 496e 6469  les.h.].h...Indi
-000005d0: 6365 7320 616e 6420 7461 626c 6573 9485  ces and tables..
-000005e0: 9481 947d 9428 6816 6873 6826 6803 6827  ...}.(h.hsh&h.h'
-000005f0: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00000600: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00000610: 7568 2568 2f68 1668 7068 2668 0368 2768  uh%h/h.hph&h.h'h
-00000620: 2868 294b 1275 6268 098c 0b62 756c 6c65  (h)K.ubh...bulle
-00000630: 745f 6c69 7374 9493 9429 8194 7d94 2868  t_list...)..}.(h
-00000640: 0568 0668 075d 9428 6809 8c09 6c69 7374  .h.h.].(h...list
-00000650: 5f69 7465 6d94 9394 2981 947d 9428 6805  _item...)..}.(h.
-00000660: 8c0f 3a72 6566 3a60 6765 6e69 6e64 6578  ..:ref:`genindex
-00000670: 6094 6807 5d94 6809 8c09 7061 7261 6772  `.h.].h...paragr
-00000680: 6170 6894 9394 2981 947d 9428 6805 688a  aph...)..}.(h.h.
-00000690: 6807 5d94 6800 8c0c 7065 6e64 696e 675f  h.].h...pending_
-000006a0: 7872 6566 9493 9429 8194 7d94 2868 0568  xref...)..}.(h.h
-000006b0: 8a68 075d 9468 098c 0669 6e6c 696e 6594  .h.].h...inline.
-000006c0: 9394 2981 947d 9428 6805 688a 6807 5d94  ..)..}.(h.h.h.].
-000006d0: 6811 8c08 6765 6e69 6e64 6578 9485 9481  h...genindex....
-000006e0: 947d 9428 6816 6898 6826 6803 6827 4e68  .}.(h.h.h&h.h'Nh
-000006f0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00000700: 5d94 288c 0478 7265 6694 8c03 7374 6494  ].(..xref...std.
-00000710: 8c07 7374 642d 7265 6694 6568 1d5d 9468  ..std-ref.eh.].h
-00000720: 1f5d 9468 215d 9475 6825 6896 6816 6893  .].h!].uh%h.h.h.
-00000730: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00000740: 681d 5d94 681f 5d94 6821 5d94 8c06 7265  h.].h.].h!]...re
-00000750: 6664 6f63 9468 4f8c 0972 6566 646f 6d61  fdoc.hO..refdoma
-00000760: 696e 9468 a38c 0772 6566 7479 7065 948c  in.h...reftype..
-00000770: 0372 6566 948c 0b72 6566 6578 706c 6963  .ref...refexplic
-00000780: 6974 9489 8c07 7265 6677 6172 6e94 888c  it....refwarn...
-00000790: 0972 6566 7461 7267 6574 948c 0867 656e  .reftarget...gen
-000007a0: 696e 6465 7894 7568 2568 9168 2768 2868  index.uh%h.h'h(h
-000007b0: 294b 1468 1668 8e75 6261 6817 7d94 2868  )K.h.h.ubah.}.(h
-000007c0: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-000007d0: 215d 9475 6825 688c 6827 6828 6829 4b14  !].uh%h.h'h(h)K.
-000007e0: 6816 6888 7562 6168 177d 9428 6819 5d94  h.h.ubah.}.(h.].
-000007f0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00000800: 7568 2568 8668 1668 8368 2668 0368 2768  uh%h.h.h.h&h.h'h
-00000810: 2868 294e 7562 6887 2981 947d 9428 6805  (h)Nubh.)..}.(h.
-00000820: 8c0f 3a72 6566 3a60 6d6f 6469 6e64 6578  ..:ref:`modindex
-00000830: 6094 6807 5d94 688d 2981 947d 9428 6805  `.h.].h.)..}.(h.
-00000840: 68c4 6807 5d94 6892 2981 947d 9428 6805  h.h.].h.)..}.(h.
-00000850: 68c4 6807 5d94 6897 2981 947d 9428 6805  h.h.].h.)..}.(h.
-00000860: 68c4 6807 5d94 6811 8c08 6d6f 6469 6e64  h.h.].h...modind
-00000870: 6578 9485 9481 947d 9428 6816 68cc 6826  ex.....}.(h.h.h&
-00000880: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
-00000890: 6819 5d94 681b 5d94 2868 a28c 0373 7464  h.].h.].(h...std
-000008a0: 948c 0773 7464 2d72 6566 9465 681d 5d94  ...std-ref.eh.].
-000008b0: 681f 5d94 6821 5d94 7568 2568 9668 1668  h.].h!].uh%h.h.h
-000008c0: c975 6261 6817 7d94 2868 195d 9468 1b5d  .ubah.}.(h.].h.]
-000008d0: 9468 1d5d 9468 1f5d 9468 215d 948c 0672  .h.].h.].h!]...r
-000008e0: 6566 646f 6394 684f 8c09 7265 6664 6f6d  efdoc.hO..refdom
-000008f0: 6169 6e94 68d6 8c07 7265 6674 7970 6594  ain.h...reftype.
-00000900: 8c03 7265 6694 8c0b 7265 6665 7870 6c69  ..ref...refexpli
-00000910: 6369 7494 898c 0772 6566 7761 726e 9488  cit....refwarn..
-00000920: 68b4 8c08 6d6f 6469 6e64 6578 9475 6825  h...modindex.uh%
-00000930: 6891 6827 6828 6829 4b15 6816 68c6 7562  h.h'h(h)K.h.h.ub
-00000940: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-00000950: 5d94 681f 5d94 6821 5d94 7568 2568 8c68  ].h.].h!].uh%h.h
-00000960: 2768 2868 294b 1568 1668 c275 6261 6817  'h(h)K.h.h.ubah.
-00000970: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000980: 1f5d 9468 215d 9475 6825 6886 6816 6883  .].h!].uh%h.h.h.
-00000990: 6826 6803 6827 6828 6829 4e75 6268 8729  h&h.h'h(h)Nubh.)
-000009a0: 8194 7d94 2868 058c 0e3a 7265 663a 6073  ..}.(h...:ref:`s
-000009b0: 6561 7263 6860 0a94 6807 5d94 688d 2981  earch`..h.].h.).
-000009c0: 947d 9428 6805 8c0d 3a72 6566 3a60 7365  .}.(h...:ref:`se
-000009d0: 6172 6368 6094 6807 5d94 6892 2981 947d  arch`.h.].h.)..}
-000009e0: 9428 6805 68fa 6807 5d94 6897 2981 947d  .(h.h.h.].h.)..}
-000009f0: 9428 6805 68fa 6807 5d94 6811 8c06 7365  .(h.h.h.].h...se
-00000a00: 6172 6368 9485 9481 947d 9428 6816 68ff  arch.....}.(h.h.
-00000a10: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
-00000a20: 9428 6819 5d94 681b 5d94 2868 a28c 0373  .(h.].h.].(h...s
-00000a30: 7464 948c 0773 7464 2d72 6566 9465 681d  td...std-ref.eh.
-00000a40: 5d94 681f 5d94 6821 5d94 7568 2568 9668  ].h.].h!].uh%h.h
-00000a50: 1668 fc75 6261 6817 7d94 2868 195d 9468  .h.ubah.}.(h.].h
-00000a60: 1b5d 9468 1d5d 9468 1f5d 9468 215d 948c  .].h.].h.].h!]..
-00000a70: 0672 6566 646f 6394 684f 8c09 7265 6664  .refdoc.hO..refd
-00000a80: 6f6d 6169 6e94 6a09 0100 008c 0772 6566  omain.j......ref
-00000a90: 7479 7065 948c 0372 6566 948c 0b72 6566  type...ref...ref
-00000aa0: 6578 706c 6963 6974 9489 8c07 7265 6677  explicit....refw
-00000ab0: 6172 6e94 8868 b48c 0673 6561 7263 6894  arn..h...search.
-00000ac0: 7568 2568 9168 2768 2868 294b 1668 1668  uh%h.h'h(h)K.h.h
-00000ad0: f875 6261 6817 7d94 2868 195d 9468 1b5d  .ubah.}.(h.].h.]
-00000ae0: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
-00000af0: 688c 6827 6828 6829 4b16 6816 68f4 7562  h.h'h(h)K.h.h.ub
-00000b00: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-00000b10: 5d94 681f 5d94 6821 5d94 7568 2568 8668  ].h.].h!].uh%h.h
-00000b20: 1668 8368 2668 0368 2768 2868 294e 7562  .h.h&h.h'h(h)Nub
-00000b30: 6568 177d 9428 6819 5d94 681b 5d94 681d  eh.}.(h.].h.].h.
-00000b40: 5d94 681f 5d94 6821 5d94 8c06 6275 6c6c  ].h.].h!]...bull
-00000b50: 6574 948c 012a 9475 6825 6881 6827 6828  et...*.uh%h.h'h(
-00000b60: 6829 4b14 6816 6870 6826 6803 7562 6800  h)K.h.hph&h.ubh.
-00000b70: 8c10 7461 6275 6c61 725f 636f 6c5f 7370  ..tabular_col_sp
-00000b80: 6563 9493 9429 8194 7d94 2868 0568 0668  ec...)..}.(h.h.h
-00000b90: 075d 9468 177d 9428 6819 5d94 681b 5d94  .].h.}.(h.].h.].
-00000ba0: 681d 5d94 681f 5d94 6821 5d94 8c04 7370  h.].h.].h!]...sp
-00000bb0: 6563 948c 105c 587b 317d 7b32 7d5c 587b  ec...\X{1}{2}\X{
-00000bc0: 317d 7b32 7d94 7568 256a 2f01 0000 6816  1}{2}.uh%j/...h.
-00000bd0: 6870 6826 6803 6827 6828 6829 4b18 7562  hph&h.h'h(h)K.ub
-00000be0: 8c16 7370 6869 6e78 2e65 7874 2e61 7574  ..sphinx.ext.aut
-00000bf0: 6f73 756d 6d61 7279 948c 1161 7574 6f73  osummary...autos
-00000c00: 756d 6d61 7279 5f74 6162 6c65 9493 9429  ummary_table...)
-00000c10: 8194 7d94 2868 058c 040a 0a0a 0a94 6807  ..}.(h........h.
-00000c20: 5d94 6809 8c05 7461 626c 6594 9394 2981  ].h...table...).
-00000c30: 947d 9428 6805 6806 6807 5d94 6809 8c06  .}.(h.h.h.].h...
-00000c40: 7467 726f 7570 9493 9429 8194 7d94 2868  tgroup...)..}.(h
-00000c50: 0568 0668 075d 9428 6809 8c07 636f 6c73  .h.h.].(h...cols
-00000c60: 7065 6394 9394 2981 947d 9428 6805 6806  pec...)..}.(h.h.
-00000c70: 6807 5d94 6817 7d94 2868 195d 9468 1b5d  h.].h.}.(h.].h.]
-00000c80: 9468 1d5d 9468 1f5d 9468 215d 948c 0863  .h.].h.].h!]...c
-00000c90: 6f6c 7769 6474 6894 4b0a 7568 256a 4d01  olwidth.K.uh%jM.
-00000ca0: 0000 6816 6a4a 0100 0075 626a 4e01 0000  ..h.jJ...ubjN...
-00000cb0: 2981 947d 9428 6805 6806 6807 5d94 6817  )..}.(h.h.h.].h.
-00000cc0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000cd0: 1f5d 9468 215d 948c 0863 6f6c 7769 6474  .].h!]...colwidt
-00000ce0: 6894 4b5a 7568 256a 4d01 0000 6816 6a4a  h.KZuh%jM...h.jJ
-00000cf0: 0100 0075 6268 098c 0574 626f 6479 9493  ...ubh...tbody..
-00000d00: 9429 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
-00000d10: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-00000d20: 681f 5d94 6821 5d94 7568 256a 6301 0000  h.].h!].uh%jc...
-00000d30: 6816 6a4a 0100 0075 6265 6817 7d94 2868  h.jJ...ubeh.}.(h
-00000d40: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-00000d50: 215d 948c 0463 6f6c 7394 4b02 7568 256a  !]...cols.K.uh%j
-00000d60: 4801 0000 6816 6a45 0100 0075 6261 6817  H...h.jE...ubah.
-00000d70: 7d94 2868 195d 9468 1b5d 948c 1561 7574  }.(h.].h.]...aut
-00000d80: 6f73 756d 6d61 7279 206c 6f6e 6774 6162  osummary longtab
-00000d90: 6c65 9461 681d 5d94 681f 5d94 6821 5d94  le.ah.].h.].h!].
-00000da0: 7568 256a 4301 0000 6816 6a3f 0100 0075  uh%jC...h.j?...u
-00000db0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
-00000dc0: 1d5d 9468 1f5d 9468 215d 9468 2368 2475  .].h.].h!].h#h$u
-00000dd0: 6825 6a3d 0100 0068 1668 7068 2668 0368  h%j=...h.hph&h.h
-00000de0: 2768 2868 294b 1875 6265 6817 7d94 2868  'h(h)K.ubeh.}.(h
-00000df0: 195d 948c 1269 6e64 6963 6573 2d61 6e64  .]...indices-and
-00000e00: 2d74 6162 6c65 7394 6168 1b5d 9468 1d5d  -tables.ah.].h.]
-00000e10: 948c 1269 6e64 6963 6573 2061 6e64 2074  ...indices and t
-00000e20: 6162 6c65 7394 6168 1f5d 9468 215d 9475  ables.ah.].h!].u
-00000e30: 6825 682a 6816 6803 6826 6803 6827 6828  h%h*h.h.h&h.h'h(
-00000e40: 6829 4b12 7562 6568 177d 9428 6819 5d94  h)K.ubeh.}.(h.].
-00000e50: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00000e60: 8c06 736f 7572 6365 9468 2875 6825 6801  ..source.h(uh%h.
-00000e70: 8c0e 6375 7272 656e 745f 736f 7572 6365  ..current_source
-00000e80: 944e 8c0c 6375 7272 656e 745f 6c69 6e65  .N..current_line
-00000e90: 944e 8c08 7365 7474 696e 6773 948c 1164  .N..settings...d
-00000ea0: 6f63 7574 696c 732e 6672 6f6e 7465 6e64  ocutils.frontend
-00000eb0: 948c 0656 616c 7565 7394 9394 2981 947d  ...Values...)..}
-00000ec0: 9428 682f 4e8c 0967 656e 6572 6174 6f72  .(h/N..generator
-00000ed0: 944e 8c09 6461 7465 7374 616d 7094 4e8c  .N..datestamp.N.
-00000ee0: 0b73 6f75 7263 655f 6c69 6e6b 944e 8c0a  .source_link.N..
-00000ef0: 736f 7572 6365 5f75 726c 944e 8c0d 746f  source_url.N..to
-00000f00: 635f 6261 636b 6c69 6e6b 7394 8c05 656e  c_backlinks...en
-00000f10: 7472 7994 8c12 666f 6f74 6e6f 7465 5f62  try...footnote_b
-00000f20: 6163 6b6c 696e 6b73 944b 018c 0d73 6563  acklinks.K...sec
-00000f30: 746e 756d 5f78 666f 726d 944b 018c 0e73  tnum_xform.K...s
-00000f40: 7472 6970 5f63 6f6d 6d65 6e74 7394 4e8c  trip_comments.N.
-00000f50: 1b73 7472 6970 5f65 6c65 6d65 6e74 735f  .strip_elements_
-00000f60: 7769 7468 5f63 6c61 7373 6573 944e 8c0d  with_classes.N..
-00000f70: 7374 7269 705f 636c 6173 7365 7394 4e8c  strip_classes.N.
-00000f80: 0c72 6570 6f72 745f 6c65 7665 6c94 4b02  .report_level.K.
-00000f90: 8c0a 6861 6c74 5f6c 6576 656c 944b 058c  ..halt_level.K..
-00000fa0: 1165 7869 745f 7374 6174 7573 5f6c 6576  .exit_status_lev
-00000fb0: 656c 944b 058c 0564 6562 7567 944e 8c0e  el.K...debug.N..
-00000fc0: 7761 726e 696e 675f 7374 7265 616d 944e  warning_stream.N
-00000fd0: 8c09 7472 6163 6562 6163 6b94 888c 0e69  ..traceback....i
-00000fe0: 6e70 7574 5f65 6e63 6f64 696e 6794 8c09  nput_encoding...
-00000ff0: 7574 662d 382d 7369 6794 8c1c 696e 7075  utf-8-sig...inpu
-00001000: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
-00001010: 5f68 616e 646c 6572 948c 0673 7472 6963  _handler...stric
-00001020: 7494 8c0f 6f75 7470 7574 5f65 6e63 6f64  t...output_encod
-00001030: 696e 6794 8c05 7574 662d 3894 8c1d 6f75  ing...utf-8...ou
-00001040: 7470 7574 5f65 6e63 6f64 696e 675f 6572  tput_encoding_er
-00001050: 726f 725f 6861 6e64 6c65 7294 6aad 0100  ror_handler.j...
-00001060: 008c 0e65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
-00001070: 6794 8c05 7574 662d 3894 8c1c 6572 726f  g...utf-8...erro
-00001080: 725f 656e 636f 6469 6e67 5f65 7272 6f72  r_encoding_error
-00001090: 5f68 616e 646c 6572 948c 1062 6163 6b73  _handler...backs
-000010a0: 6c61 7368 7265 706c 6163 6594 8c0d 6c61  lashreplace...la
-000010b0: 6e67 7561 6765 5f63 6f64 6594 8c02 656e  nguage_code...en
-000010c0: 948c 1372 6563 6f72 645f 6465 7065 6e64  ...record_depend
-000010d0: 656e 6369 6573 944e 8c06 636f 6e66 6967  encies.N..config
-000010e0: 944e 8c09 6964 5f70 7265 6669 7894 6806  .N..id_prefix.h.
-000010f0: 8c0e 6175 746f 5f69 645f 7072 6566 6978  ..auto_id_prefix
-00001100: 948c 0269 6494 8c0d 6475 6d70 5f73 6574  ...id...dump_set
-00001110: 7469 6e67 7394 4e8c 0e64 756d 705f 696e  tings.N..dump_in
-00001120: 7465 726e 616c 7394 4e8c 0f64 756d 705f  ternals.N..dump_
-00001130: 7472 616e 7366 6f72 6d73 944e 8c0f 6475  transforms.N..du
-00001140: 6d70 5f70 7365 7564 6f5f 786d 6c94 4e8c  mp_pseudo_xml.N.
-00001150: 1065 7870 6f73 655f 696e 7465 726e 616c  .expose_internal
-00001160: 7394 4e8c 0e73 7472 6963 745f 7669 7369  s.N..strict_visi
-00001170: 746f 7294 4e8c 0f5f 6469 7361 626c 655f  tor.N.._disable_
-00001180: 636f 6e66 6967 944e 8c07 5f73 6f75 7263  config.N.._sourc
-00001190: 6594 6828 8c0c 5f64 6573 7469 6e61 7469  e.h(.._destinati
-000011a0: 6f6e 944e 8c0d 5f63 6f6e 6669 675f 6669  on.N.._config_fi
-000011b0: 6c65 7394 5d94 8c16 6669 6c65 5f69 6e73  les.]...file_ins
-000011c0: 6572 7469 6f6e 5f65 6e61 626c 6564 9488  ertion_enabled..
-000011d0: 8c0b 7261 775f 656e 6162 6c65 6494 4b01  ..raw_enabled.K.
-000011e0: 8c11 6c69 6e65 5f6c 656e 6774 685f 6c69  ..line_length_li
-000011f0: 6d69 7494 4d10 278c 0e70 6570 5f72 6566  mit.M.'..pep_ref
-00001200: 6572 656e 6365 7394 4e8c 0c70 6570 5f62  erences.N..pep_b
-00001210: 6173 655f 7572 6c94 8c18 6874 7470 733a  ase_url...https:
-00001220: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
-00001230: 672f 948c 1570 6570 5f66 696c 655f 7572  g/...pep_file_ur
-00001240: 6c5f 7465 6d70 6c61 7465 948c 0870 6570  l_template...pep
-00001250: 2d25 3034 6494 8c0e 7266 635f 7265 6665  -%04d...rfc_refe
-00001260: 7265 6e63 6573 944e 8c0c 7266 635f 6261  rences.N..rfc_ba
-00001270: 7365 5f75 726c 948c 2668 7474 7073 3a2f  se_url..&https:/
-00001280: 2f64 6174 6174 7261 636b 6572 2e69 6574  /datatracker.iet
-00001290: 662e 6f72 672f 646f 632f 6874 6d6c 2f94  f.org/doc/html/.
-000012a0: 8c09 7461 625f 7769 6474 6894 4b08 8c1d  ..tab_width.K...
-000012b0: 7472 696d 5f66 6f6f 746e 6f74 655f 7265  trim_footnote_re
-000012c0: 6665 7265 6e63 655f 7370 6163 6594 898c  ference_space...
-000012d0: 1073 796e 7461 785f 6869 6768 6c69 6768  .syntax_highligh
-000012e0: 7494 8c04 6c6f 6e67 948c 0c73 6d61 7274  t...long...smart
-000012f0: 5f71 756f 7465 7394 888c 1373 6d61 7274  _quotes....smart
-00001300: 7175 6f74 6573 5f6c 6f63 616c 6573 945d  quotes_locales.]
-00001310: 948c 1d63 6861 7261 6374 6572 5f6c 6576  ...character_lev
-00001320: 656c 5f69 6e6c 696e 655f 6d61 726b 7570  el_inline_markup
-00001330: 9489 8c0e 646f 6374 6974 6c65 5f78 666f  ....doctitle_xfo
-00001340: 726d 9489 8c0d 646f 6369 6e66 6f5f 7866  rm....docinfo_xf
-00001350: 6f72 6d94 4b01 8c12 7365 6374 7375 6274  orm.K...sectsubt
-00001360: 6974 6c65 5f78 666f 726d 9489 8c0d 696d  itle_xform....im
-00001370: 6167 655f 6c6f 6164 696e 6794 8c04 6c69  age_loading...li
-00001380: 6e6b 948c 1065 6d62 6564 5f73 7479 6c65  nk...embed_style
-00001390: 7368 6565 7494 898c 1563 6c6f 616b 5f65  sheet....cloak_e
-000013a0: 6d61 696c 5f61 6464 7265 7373 6573 9488  mail_addresses..
-000013b0: 8c11 7365 6374 696f 6e5f 7365 6c66 5f6c  ..section_self_l
-000013c0: 696e 6b94 898c 0365 6e76 944e 7562 8c08  ink....env.Nub..
-000013d0: 7265 706f 7274 6572 944e 8c10 696e 6469  reporter.N..indi
-000013e0: 7265 6374 5f74 6172 6765 7473 945d 948c  rect_targets.]..
-000013f0: 1173 7562 7374 6974 7574 696f 6e5f 6465  .substitution_de
-00001400: 6673 947d 948c 1273 7562 7374 6974 7574  fs.}...substitut
-00001410: 696f 6e5f 6e61 6d65 7394 7d94 8c08 7265  ion_names.}...re
-00001420: 666e 616d 6573 947d 948c 0672 6566 6964  fnames.}...refid
-00001430: 7394 7d94 8c07 6e61 6d65 6964 7394 7d94  s.}...nameids.}.
-00001440: 2868 6d68 6a6a 8701 0000 6a84 0100 0075  (hmhjj....j....u
-00001450: 8c09 6e61 6d65 7479 7065 7394 7d94 2868  ..nametypes.}.(h
-00001460: 6d89 6a87 0100 0089 7568 197d 9428 686a  m.j.....uh.}.(hj
-00001470: 682c 6a84 0100 0068 7075 8c0d 666f 6f74  h,j....hpu..foot
-00001480: 6e6f 7465 5f72 6566 7394 7d94 8c0d 6369  note_refs.}...ci
-00001490: 7461 7469 6f6e 5f72 6566 7394 7d94 8c0d  tation_refs.}...
-000014a0: 6175 746f 666f 6f74 6e6f 7465 7394 5d94  autofootnotes.].
-000014b0: 8c11 6175 746f 666f 6f74 6e6f 7465 5f72  ..autofootnote_r
-000014c0: 6566 7394 5d94 8c10 7379 6d62 6f6c 5f66  efs.]...symbol_f
-000014d0: 6f6f 746e 6f74 6573 945d 948c 1473 796d  ootnotes.]...sym
-000014e0: 626f 6c5f 666f 6f74 6e6f 7465 5f72 6566  bol_footnote_ref
-000014f0: 7394 5d94 8c09 666f 6f74 6e6f 7465 7394  s.]...footnotes.
-00001500: 5d94 8c09 6369 7461 7469 6f6e 7394 5d94  ]...citations.].
-00001510: 8c12 6175 746f 666f 6f74 6e6f 7465 5f73  ..autofootnote_s
-00001520: 7461 7274 944b 018c 1573 796d 626f 6c5f  tart.K...symbol_
-00001530: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
-00001540: 008c 0a69 645f 636f 756e 7465 7294 8c0b  ...id_counter...
-00001550: 636f 6c6c 6563 7469 6f6e 7394 8c07 436f  collections...Co
-00001560: 756e 7465 7294 9394 7d94 8594 5294 8c0e  unter...}...R...
-00001570: 7061 7273 655f 6d65 7373 6167 6573 945d  parse_messages.]
-00001580: 948c 1274 7261 6e73 666f 726d 5f6d 6573  ...transform_mes
-00001590: 7361 6765 7394 5d94 8c0b 7472 616e 7366  sages.]...transf
-000015a0: 6f72 6d65 7294 4e8c 0b69 6e63 6c75 6465  ormer.N..include
-000015b0: 5f6c 6f67 945d 948c 0a64 6563 6f72 6174  _log.]...decorat
-000015c0: 696f 6e94 4e68 2668 0375 622e            ion.Nh&h.ub.
+00000070: 6805 8cc8 7474 7420 646f 6375 6d65 6e74  h...ttt document
+00000080: 6174 696f 6e20 6d61 7374 6572 2066 696c  ation master fil
+00000090: 652c 2063 7265 6174 6564 2062 790a 7370  e, created by.sp
+000000a0: 6869 6e78 2d71 7569 636b 7374 6172 7420  hinx-quickstart 
+000000b0: 6f6e 2053 6174 2041 7072 2031 3520 3137  on Sat Apr 15 17
+000000c0: 3a35 353a 3232 2032 3032 332e 0a59 6f75  :55:22 2023..You
+000000d0: 2063 616e 2061 6461 7074 2074 6869 7320   can adapt this 
+000000e0: 6669 6c65 2063 6f6d 706c 6574 656c 7920  file completely 
+000000f0: 746f 2079 6f75 7220 6c69 6b69 6e67 2c20  to your liking, 
+00000100: 6275 7420 6974 2073 686f 756c 6420 6174  but it should at
+00000110: 206c 6561 7374 0a63 6f6e 7461 696e 2074   least.contain t
+00000120: 6865 2072 6f6f 7420 6074 6f63 7472 6565  he root `toctree
+00000130: 6020 6469 7265 6374 6976 652e 9468 075d  ` directive..h.]
+00000140: 9468 098c 0454 6578 7494 9394 8cc8 7474  .h...Text.....tt
+00000150: 7420 646f 6375 6d65 6e74 6174 696f 6e20  t documentation 
+00000160: 6d61 7374 6572 2066 696c 652c 2063 7265  master file, cre
+00000170: 6174 6564 2062 790a 7370 6869 6e78 2d71  ated by.sphinx-q
+00000180: 7569 636b 7374 6172 7420 6f6e 2053 6174  uickstart on Sat
+00000190: 2041 7072 2031 3520 3137 3a35 353a 3232   Apr 15 17:55:22
+000001a0: 2032 3032 332e 0a59 6f75 2063 616e 2061   2023..You can a
+000001b0: 6461 7074 2074 6869 7320 6669 6c65 2063  dapt this file c
+000001c0: 6f6d 706c 6574 656c 7920 746f 2079 6f75  ompletely to you
+000001d0: 7220 6c69 6b69 6e67 2c20 6275 7420 6974  r liking, but it
+000001e0: 2073 686f 756c 6420 6174 206c 6561 7374   should at least
+000001f0: 0a63 6f6e 7461 696e 2074 6865 2072 6f6f  .contain the roo
+00000200: 7420 6074 6f63 7472 6565 6020 6469 7265  t `toctree` dire
+00000210: 6374 6976 652e 9485 9481 947d 948c 0670  ctive......}...p
+00000220: 6172 656e 7494 680c 7362 618c 0a61 7474  arent.h.sba..att
+00000230: 7269 6275 7465 7394 7d94 288c 0369 6473  ributes.}.(..ids
+00000240: 945d 948c 0763 6c61 7373 6573 945d 948c  .]...classes.]..
+00000250: 056e 616d 6573 945d 948c 0864 7570 6e61  .names.]...dupna
+00000260: 6d65 7394 5d94 8c08 6261 636b 7265 6673  mes.]...backrefs
+00000270: 945d 948c 0978 6d6c 3a73 7061 6365 948c  .]...xml:space..
+00000280: 0870 7265 7365 7276 6594 758c 0774 6167  .preserve.u..tag
+00000290: 6e61 6d65 9468 0a68 1668 038c 095f 646f  name.h.h.h..._do
+000002a0: 6375 6d65 6e74 9468 038c 0673 6f75 7263  cument.h...sourc
+000002b0: 6594 8c2c 443a 5c68 6f6d 655c 7079 7072  e..,D:\home\pypr
+000002c0: 6f6a 6563 7473 5c70 6a70 6c61 6e5c 646f  ojects\pjplan\do
+000002d0: 6373 5c74 7474 5c69 6e64 6578 2e72 7374  cs\ttt\index.rst
+000002e0: 948c 046c 696e 6594 4b05 7562 6809 8c07  ...line.K.ubh...
+000002f0: 7365 6374 696f 6e94 9394 2981 947d 9428  section...)..}.(
+00000300: 6805 6806 6807 5d94 2868 098c 0574 6974  h.h.h.].(h...tit
+00000310: 6c65 9493 9429 8194 7d94 2868 058c 1f57  le...)..}.(h...W
+00000320: 656c 636f 6d65 2074 6f20 7474 7427 7320  elcome to ttt's 
+00000330: 646f 6375 6d65 6e74 6174 696f 6e21 9468  documentation!.h
+00000340: 075d 9468 118c 2157 656c 636f 6d65 2074  .].h..!Welcome t
+00000350: 6f20 7474 74e2 8099 7320 646f 6375 6d65  o ttt...s docume
+00000360: 6e74 6174 696f 6e21 9485 9481 947d 9428  ntation!.....}.(
+00000370: 6816 6831 6826 6803 6827 4e68 294e 7562  h.h1h&h.h'Nh)Nub
+00000380: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+00000390: 5d94 681f 5d94 6821 5d94 7568 2568 2f68  ].h.].h!].uh%h/h
+000003a0: 1668 2c68 2668 0368 2768 2868 294b 0775  .h,h&h.h'h(h)K.u
+000003b0: 6268 098c 0863 6f6d 706f 756e 6494 9394  bh...compound...
+000003c0: 2981 947d 9428 6805 6806 6807 5d94 6800  )..}.(h.h.h.].h.
+000003d0: 8c07 746f 6374 7265 6594 9394 2981 947d  ..toctree...)..}
+000003e0: 9428 6805 6806 6807 5d94 6817 7d94 2868  .(h.h.h.].h.}.(h
+000003f0: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00000400: 215d 9468 168c 0974 7474 2f69 6e64 6578  !].h...ttt/index
+00000410: 948c 0765 6e74 7269 6573 945d 948c 0c69  ...entries.]...i
+00000420: 6e63 6c75 6465 6669 6c65 7394 5d94 8c08  ncludefiles.]...
+00000430: 6d61 7864 6570 7468 944a ffff ffff 8c07  maxdepth.J......
+00000440: 6361 7074 696f 6e94 4e8c 0467 6c6f 6294  caption.N..glob.
+00000450: 888c 0668 6964 6465 6e94 888c 0d69 6e63  ...hidden....inc
+00000460: 6c75 6465 6869 6464 656e 9489 8c08 6e75  ludehidden....nu
+00000470: 6d62 6572 6564 944b 008c 0a74 6974 6c65  mbered.K...title
+00000480: 736f 6e6c 7994 898c 0a72 6177 656e 7472  sonly....rawentr
+00000490: 6965 7394 5d94 7568 2568 4468 2768 2868  ies.].uh%hDh'h(h
+000004a0: 294b 0968 1668 4175 6261 6817 7d94 2868  )K.h.hAubah.}.(h
+000004b0: 195d 9468 1b5d 948c 0f74 6f63 7472 6565  .].h.]...toctree
+000004c0: 2d77 7261 7070 6572 9461 681d 5d94 681f  -wrapper.ah.].h.
+000004d0: 5d94 6821 5d94 7568 2568 3f68 1668 2c68  ].h!].uh%h?h.h,h
+000004e0: 2668 0368 2768 2868 294e 7562 6568 177d  &h.h'h(h)Nubeh.}
+000004f0: 9428 6819 5d94 8c1e 7765 6c63 6f6d 652d  .(h.]...welcome-
+00000500: 746f 2d74 7474 2d73 2d64 6f63 756d 656e  to-ttt-s-documen
+00000510: 7461 7469 6f6e 9461 681b 5d94 681d 5d94  tation.ah.].h.].
+00000520: 8c1f 7765 6c63 6f6d 6520 746f 2074 7474  ..welcome to ttt
+00000530: 2773 2064 6f63 756d 656e 7461 7469 6f6e  's documentation
+00000540: 2194 6168 1f5d 9468 215d 9475 6825 682a  !.ah.].h!].uh%h*
+00000550: 6816 6803 6826 6803 6827 6828 6829 4b07  h.h.h&h.h'h(h)K.
+00000560: 7562 682b 2981 947d 9428 6805 6806 6807  ubh+)..}.(h.h.h.
+00000570: 5d94 2868 3029 8194 7d94 2868 058c 1249  ].(h0)..}.(h...I
+00000580: 6e64 6963 6573 2061 6e64 2074 6162 6c65  ndices and table
+00000590: 7394 6807 5d94 6811 8c12 496e 6469 6365  s.h.].h...Indice
+000005a0: 7320 616e 6420 7461 626c 6573 9485 9481  s and tables....
+000005b0: 947d 9428 6816 686f 6826 6803 6827 4e68  .}.(h.hoh&h.h'Nh
+000005c0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+000005d0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+000005e0: 2568 2f68 1668 6c68 2668 0368 2768 2868  %h/h.hlh&h.h'h(h
+000005f0: 294b 1275 6268 098c 0b62 756c 6c65 745f  )K.ubh...bullet_
+00000600: 6c69 7374 9493 9429 8194 7d94 2868 0568  list...)..}.(h.h
+00000610: 0668 075d 9428 6809 8c09 6c69 7374 5f69  .h.].(h...list_i
+00000620: 7465 6d94 9394 2981 947d 9428 6805 8c0f  tem...)..}.(h...
+00000630: 3a72 6566 3a60 6765 6e69 6e64 6578 6094  :ref:`genindex`.
+00000640: 6807 5d94 6809 8c09 7061 7261 6772 6170  h.].h...paragrap
+00000650: 6894 9394 2981 947d 9428 6805 6886 6807  h...)..}.(h.h.h.
+00000660: 5d94 6800 8c0c 7065 6e64 696e 675f 7872  ].h...pending_xr
+00000670: 6566 9493 9429 8194 7d94 2868 0568 8668  ef...)..}.(h.h.h
+00000680: 075d 9468 098c 0669 6e6c 696e 6594 9394  .].h...inline...
+00000690: 2981 947d 9428 6805 6886 6807 5d94 6811  )..}.(h.h.h.].h.
+000006a0: 8c08 6765 6e69 6e64 6578 9485 9481 947d  ..genindex.....}
+000006b0: 9428 6816 6894 6826 6803 6827 4e68 294e  .(h.h.h&h.h'Nh)N
+000006c0: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+000006d0: 288c 0478 7265 6694 8c03 7374 6494 8c07  (..xref...std...
+000006e0: 7374 642d 7265 6694 6568 1d5d 9468 1f5d  std-ref.eh.].h.]
+000006f0: 9468 215d 9475 6825 6892 6816 688f 7562  .h!].uh%h.h.h.ub
+00000700: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+00000710: 5d94 681f 5d94 6821 5d94 8c06 7265 6664  ].h.].h!]...refd
+00000720: 6f63 9468 4f8c 0972 6566 646f 6d61 696e  oc.hO..refdomain
+00000730: 9468 9f8c 0772 6566 7479 7065 948c 0372  .h...reftype...r
+00000740: 6566 948c 0b72 6566 6578 706c 6963 6974  ef...refexplicit
+00000750: 9489 8c07 7265 6677 6172 6e94 888c 0972  ....refwarn....r
+00000760: 6566 7461 7267 6574 948c 0867 656e 696e  eftarget...genin
+00000770: 6465 7894 7568 2568 8d68 2768 2868 294b  dex.uh%h.h'h(h)K
+00000780: 1468 1668 8a75 6261 6817 7d94 2868 195d  .h.h.ubah.}.(h.]
+00000790: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+000007a0: 9475 6825 6888 6827 6828 6829 4b14 6816  .uh%h.h'h(h)K.h.
+000007b0: 6884 7562 6168 177d 9428 6819 5d94 681b  h.ubah.}.(h.].h.
+000007c0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+000007d0: 2568 8268 1668 7f68 2668 0368 2768 2868  %h.h.h.h&h.h'h(h
+000007e0: 294e 7562 6883 2981 947d 9428 6805 8c0f  )Nubh.)..}.(h...
+000007f0: 3a72 6566 3a60 6d6f 6469 6e64 6578 6094  :ref:`modindex`.
+00000800: 6807 5d94 6889 2981 947d 9428 6805 68c0  h.].h.)..}.(h.h.
+00000810: 6807 5d94 688e 2981 947d 9428 6805 68c0  h.].h.)..}.(h.h.
+00000820: 6807 5d94 6893 2981 947d 9428 6805 68c0  h.].h.)..}.(h.h.
+00000830: 6807 5d94 6811 8c08 6d6f 6469 6e64 6578  h.].h...modindex
+00000840: 9485 9481 947d 9428 6816 68c8 6826 6803  .....}.(h.h.h&h.
+00000850: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+00000860: 5d94 681b 5d94 2868 9e8c 0373 7464 948c  ].h.].(h...std..
+00000870: 0773 7464 2d72 6566 9465 681d 5d94 681f  .std-ref.eh.].h.
+00000880: 5d94 6821 5d94 7568 2568 9268 1668 c575  ].h!].uh%h.h.h.u
+00000890: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+000008a0: 1d5d 9468 1f5d 9468 215d 948c 0672 6566  .].h.].h!]...ref
+000008b0: 646f 6394 684f 8c09 7265 6664 6f6d 6169  doc.hO..refdomai
+000008c0: 6e94 68d2 8c07 7265 6674 7970 6594 8c03  n.h...reftype...
+000008d0: 7265 6694 8c0b 7265 6665 7870 6c69 6369  ref...refexplici
+000008e0: 7494 898c 0772 6566 7761 726e 9488 68b0  t....refwarn..h.
+000008f0: 8c08 6d6f 6469 6e64 6578 9475 6825 688d  ..modindex.uh%h.
+00000900: 6827 6828 6829 4b15 6816 68c2 7562 6168  h'h(h)K.h.h.ubah
+00000910: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000920: 681f 5d94 6821 5d94 7568 2568 8868 2768  h.].h!].uh%h.h'h
+00000930: 2868 294b 1568 1668 be75 6261 6817 7d94  (h)K.h.h.ubah.}.
+00000940: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00000950: 9468 215d 9475 6825 6882 6816 687f 6826  .h!].uh%h.h.h.h&
+00000960: 6803 6827 6828 6829 4e75 6268 8329 8194  h.h'h(h)Nubh.)..
+00000970: 7d94 2868 058c 0d3a 7265 663a 6073 6561  }.(h...:ref:`sea
+00000980: 7263 6860 9468 075d 9468 8929 8194 7d94  rch`.h.].h.)..}.
+00000990: 2868 0568 f268 075d 9468 8e29 8194 7d94  (h.h.h.].h.)..}.
+000009a0: 2868 0568 f268 075d 9468 9329 8194 7d94  (h.h.h.].h.)..}.
+000009b0: 2868 0568 f268 075d 9468 118c 0673 6561  (h.h.h.].h...sea
+000009c0: 7263 6894 8594 8194 7d94 2868 1668 fa68  rch.....}.(h.h.h
+000009d0: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
+000009e0: 2868 195d 9468 1b5d 9428 689e 8c03 7374  (h.].h.].(h...st
+000009f0: 6494 8c07 7374 642d 7265 6694 6568 1d5d  d...std-ref.eh.]
+00000a00: 9468 1f5d 9468 215d 9475 6825 6892 6816  .h.].h!].uh%h.h.
+00000a10: 68f7 7562 6168 177d 9428 6819 5d94 681b  h.ubah.}.(h.].h.
+00000a20: 5d94 681d 5d94 681f 5d94 6821 5d94 8c06  ].h.].h.].h!]...
+00000a30: 7265 6664 6f63 9468 4f8c 0972 6566 646f  refdoc.hO..refdo
+00000a40: 6d61 696e 946a 0401 0000 8c07 7265 6674  main.j......reft
+00000a50: 7970 6594 8c03 7265 6694 8c0b 7265 6665  ype...ref...refe
+00000a60: 7870 6c69 6369 7494 898c 0772 6566 7761  xplicit....refwa
+00000a70: 726e 9488 68b0 8c06 7365 6172 6368 9475  rn..h...search.u
+00000a80: 6825 688d 6827 6828 6829 4b16 6816 68f4  h%h.h'h(h)K.h.h.
+00000a90: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+00000aa0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+00000ab0: 8868 2768 2868 294b 1668 1668 f075 6261  .h'h(h)K.h.h.uba
+00000ac0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00000ad0: 9468 1f5d 9468 215d 9475 6825 6882 6816  .h.].h!].uh%h.h.
+00000ae0: 687f 6826 6803 6827 6828 6829 4e75 6265  h.h&h.h'h(h)Nube
+00000af0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00000b00: 9468 1f5d 9468 215d 948c 0662 756c 6c65  .h.].h!]...bulle
+00000b10: 7494 8c01 2a94 7568 2568 7d68 2768 2868  t...*.uh%h}h'h(h
+00000b20: 294b 1468 1668 6c68 2668 0375 6265 6817  )K.h.hlh&h.ubeh.
+00000b30: 7d94 2868 195d 948c 1269 6e64 6963 6573  }.(h.]...indices
+00000b40: 2d61 6e64 2d74 6162 6c65 7394 6168 1b5d  -and-tables.ah.]
+00000b50: 9468 1d5d 948c 1269 6e64 6963 6573 2061  .h.]...indices a
+00000b60: 6e64 2074 6162 6c65 7394 6168 1f5d 9468  nd tables.ah.].h
+00000b70: 215d 9475 6825 682a 6816 6803 6826 6803  !].uh%h*h.h.h&h.
+00000b80: 6827 6828 6829 4b12 7562 6568 177d 9428  h'h(h)K.ubeh.}.(
+00000b90: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00000ba0: 6821 5d94 8c06 736f 7572 6365 9468 2875  h!]...source.h(u
+00000bb0: 6825 6801 8c0e 6375 7272 656e 745f 736f  h%h...current_so
+00000bc0: 7572 6365 944e 8c0c 6375 7272 656e 745f  urce.N..current_
+00000bd0: 6c69 6e65 944e 8c08 7365 7474 696e 6773  line.N..settings
+00000be0: 948c 1164 6f63 7574 696c 732e 6672 6f6e  ...docutils.fron
+00000bf0: 7465 6e64 948c 0656 616c 7565 7394 9394  tend...Values...
+00000c00: 2981 947d 9428 682f 4e8c 0967 656e 6572  )..}.(h/N..gener
+00000c10: 6174 6f72 944e 8c09 6461 7465 7374 616d  ator.N..datestam
+00000c20: 7094 4e8c 0b73 6f75 7263 655f 6c69 6e6b  p.N..source_link
+00000c30: 944e 8c0a 736f 7572 6365 5f75 726c 944e  .N..source_url.N
+00000c40: 8c0d 746f 635f 6261 636b 6c69 6e6b 7394  ..toc_backlinks.
+00000c50: 8c05 656e 7472 7994 8c12 666f 6f74 6e6f  ..entry...footno
+00000c60: 7465 5f62 6163 6b6c 696e 6b73 944b 018c  te_backlinks.K..
+00000c70: 0d73 6563 746e 756d 5f78 666f 726d 944b  .sectnum_xform.K
+00000c80: 018c 0e73 7472 6970 5f63 6f6d 6d65 6e74  ...strip_comment
+00000c90: 7394 4e8c 1b73 7472 6970 5f65 6c65 6d65  s.N..strip_eleme
+00000ca0: 6e74 735f 7769 7468 5f63 6c61 7373 6573  nts_with_classes
+00000cb0: 944e 8c0d 7374 7269 705f 636c 6173 7365  .N..strip_classe
+00000cc0: 7394 4e8c 0c72 6570 6f72 745f 6c65 7665  s.N..report_leve
+00000cd0: 6c94 4b02 8c0a 6861 6c74 5f6c 6576 656c  l.K...halt_level
+00000ce0: 944b 058c 1165 7869 745f 7374 6174 7573  .K...exit_status
+00000cf0: 5f6c 6576 656c 944b 058c 0564 6562 7567  _level.K...debug
+00000d00: 944e 8c0e 7761 726e 696e 675f 7374 7265  .N..warning_stre
+00000d10: 616d 944e 8c09 7472 6163 6562 6163 6b94  am.N..traceback.
+00000d20: 888c 0e69 6e70 7574 5f65 6e63 6f64 696e  ...input_encodin
+00000d30: 6794 8c09 7574 662d 382d 7369 6794 8c1c  g...utf-8-sig...
+00000d40: 696e 7075 745f 656e 636f 6469 6e67 5f65  input_encoding_e
+00000d50: 7272 6f72 5f68 616e 646c 6572 948c 0673  rror_handler...s
+00000d60: 7472 6963 7494 8c0f 6f75 7470 7574 5f65  trict...output_e
+00000d70: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
+00000d80: 8c1d 6f75 7470 7574 5f65 6e63 6f64 696e  ..output_encodin
+00000d90: 675f 6572 726f 725f 6861 6e64 6c65 7294  g_error_handler.
+00000da0: 6a55 0100 008c 0e65 7272 6f72 5f65 6e63  jU.....error_enc
+00000db0: 6f64 696e 6794 8c05 7574 662d 3894 8c1c  oding...utf-8...
+00000dc0: 6572 726f 725f 656e 636f 6469 6e67 5f65  error_encoding_e
+00000dd0: 7272 6f72 5f68 616e 646c 6572 948c 1062  rror_handler...b
+00000de0: 6163 6b73 6c61 7368 7265 706c 6163 6594  ackslashreplace.
+00000df0: 8c0d 6c61 6e67 7561 6765 5f63 6f64 6594  ..language_code.
+00000e00: 8c02 656e 948c 1372 6563 6f72 645f 6465  ..en...record_de
+00000e10: 7065 6e64 656e 6369 6573 944e 8c06 636f  pendencies.N..co
+00000e20: 6e66 6967 944e 8c09 6964 5f70 7265 6669  nfig.N..id_prefi
+00000e30: 7894 6806 8c0e 6175 746f 5f69 645f 7072  x.h...auto_id_pr
+00000e40: 6566 6978 948c 0269 6494 8c0d 6475 6d70  efix...id...dump
+00000e50: 5f73 6574 7469 6e67 7394 4e8c 0e64 756d  _settings.N..dum
+00000e60: 705f 696e 7465 726e 616c 7394 4e8c 0f64  p_internals.N..d
+00000e70: 756d 705f 7472 616e 7366 6f72 6d73 944e  ump_transforms.N
+00000e80: 8c0f 6475 6d70 5f70 7365 7564 6f5f 786d  ..dump_pseudo_xm
+00000e90: 6c94 4e8c 1065 7870 6f73 655f 696e 7465  l.N..expose_inte
+00000ea0: 726e 616c 7394 4e8c 0e73 7472 6963 745f  rnals.N..strict_
+00000eb0: 7669 7369 746f 7294 4e8c 0f5f 6469 7361  visitor.N.._disa
+00000ec0: 626c 655f 636f 6e66 6967 944e 8c07 5f73  ble_config.N.._s
+00000ed0: 6f75 7263 6594 6828 8c0c 5f64 6573 7469  ource.h(.._desti
+00000ee0: 6e61 7469 6f6e 944e 8c0d 5f63 6f6e 6669  nation.N.._confi
+00000ef0: 675f 6669 6c65 7394 5d94 8c16 6669 6c65  g_files.]...file
+00000f00: 5f69 6e73 6572 7469 6f6e 5f65 6e61 626c  _insertion_enabl
+00000f10: 6564 9488 8c0b 7261 775f 656e 6162 6c65  ed....raw_enable
+00000f20: 6494 4b01 8c11 6c69 6e65 5f6c 656e 6774  d.K...line_lengt
+00000f30: 685f 6c69 6d69 7494 4a00 e1f5 058c 0e70  h_limit.J......p
+00000f40: 6570 5f72 6566 6572 656e 6365 7394 4e8c  ep_references.N.
+00000f50: 0c70 6570 5f62 6173 655f 7572 6c94 8c18  .pep_base_url...
+00000f60: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
+00000f70: 686f 6e2e 6f72 672f 948c 1570 6570 5f66  hon.org/...pep_f
+00000f80: 696c 655f 7572 6c5f 7465 6d70 6c61 7465  ile_url_template
+00000f90: 948c 0870 6570 2d25 3034 6494 8c0e 7266  ...pep-%04d...rf
+00000fa0: 635f 7265 6665 7265 6e63 6573 944e 8c0c  c_references.N..
+00000fb0: 7266 635f 6261 7365 5f75 726c 948c 2668  rfc_base_url..&h
+00000fc0: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+00000fd0: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+00000fe0: 6874 6d6c 2f94 8c09 7461 625f 7769 6474  html/...tab_widt
+00000ff0: 6894 4b08 8c1d 7472 696d 5f66 6f6f 746e  h.K...trim_footn
+00001000: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
+00001010: 6163 6594 898c 1073 796e 7461 785f 6869  ace....syntax_hi
+00001020: 6768 6c69 6768 7494 8c04 6c6f 6e67 948c  ghlight...long..
+00001030: 0c73 6d61 7274 5f71 756f 7465 7394 888c  .smart_quotes...
+00001040: 1373 6d61 7274 7175 6f74 6573 5f6c 6f63  .smartquotes_loc
+00001050: 616c 6573 945d 948c 1d63 6861 7261 6374  ales.]...charact
+00001060: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
+00001070: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
+00001080: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
+00001090: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
+000010a0: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
+000010b0: 9489 8c0d 696d 6167 655f 6c6f 6164 696e  ....image_loadin
+000010c0: 6794 8c04 6c69 6e6b 948c 1065 6d62 6564  g...link...embed
+000010d0: 5f73 7479 6c65 7368 6565 7494 898c 1563  _stylesheet....c
+000010e0: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
+000010f0: 7373 6573 9488 8c11 7365 6374 696f 6e5f  sses....section_
+00001100: 7365 6c66 5f6c 696e 6b94 898c 0365 6e76  self_link....env
+00001110: 944e 7562 8c08 7265 706f 7274 6572 944e  .Nub..reporter.N
+00001120: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
+00001130: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
+00001140: 696f 6e5f 6465 6673 947d 948c 1273 7562  ion_defs.}...sub
+00001150: 7374 6974 7574 696f 6e5f 6e61 6d65 7394  stitution_names.
+00001160: 7d94 8c08 7265 666e 616d 6573 947d 948c  }...refnames.}..
+00001170: 0672 6566 6964 7394 7d94 8c07 6e61 6d65  .refids.}...name
+00001180: 6964 7394 7d94 2868 6968 666a 2f01 0000  ids.}.(hihfj/...
+00001190: 6a2c 0100 0075 8c09 6e61 6d65 7479 7065  j,...u..nametype
+000011a0: 7394 7d94 2868 6989 6a2f 0100 0089 7568  s.}.(hi.j/....uh
+000011b0: 197d 9428 6866 682c 6a2c 0100 0068 6c75  .}.(hfh,j,...hlu
+000011c0: 8c0d 666f 6f74 6e6f 7465 5f72 6566 7394  ..footnote_refs.
+000011d0: 7d94 8c0d 6369 7461 7469 6f6e 5f72 6566  }...citation_ref
+000011e0: 7394 7d94 8c0d 6175 746f 666f 6f74 6e6f  s.}...autofootno
+000011f0: 7465 7394 5d94 8c11 6175 746f 666f 6f74  tes.]...autofoot
+00001200: 6e6f 7465 5f72 6566 7394 5d94 8c10 7379  note_refs.]...sy
+00001210: 6d62 6f6c 5f66 6f6f 746e 6f74 6573 945d  mbol_footnotes.]
+00001220: 948c 1473 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
+00001230: 7465 5f72 6566 7394 5d94 8c09 666f 6f74  te_refs.]...foot
+00001240: 6e6f 7465 7394 5d94 8c09 6369 7461 7469  notes.]...citati
+00001250: 6f6e 7394 5d94 8c12 6175 746f 666f 6f74  ons.]...autofoot
+00001260: 6e6f 7465 5f73 7461 7274 944b 018c 1573  note_start.K...s
+00001270: 796d 626f 6c5f 666f 6f74 6e6f 7465 5f73  ymbol_footnote_s
+00001280: 7461 7274 944b 008c 0a69 645f 636f 756e  tart.K...id_coun
+00001290: 7465 7294 8c0b 636f 6c6c 6563 7469 6f6e  ter...collection
+000012a0: 7394 8c07 436f 756e 7465 7294 9394 7d94  s...Counter...}.
+000012b0: 8594 5294 8c0e 7061 7273 655f 6d65 7373  ..R...parse_mess
+000012c0: 6167 6573 945d 948c 1274 7261 6e73 666f  ages.]...transfo
+000012d0: 726d 5f6d 6573 7361 6765 7394 5d94 8c0b  rm_messages.]...
+000012e0: 7472 616e 7366 6f72 6d65 7294 4e8c 0b69  transformer.N..i
+000012f0: 6e63 6c75 6465 5f6c 6f67 945d 948c 0a64  nclude_log.]...d
+00001300: 6563 6f72 6174 696f 6e94 4e68 2668 0375  ecoration.Nh&h.u
+00001310: 622e                                     b.
```

### Comparing `pjplan-0.0.8/docs/_build/doctrees/modules.doctree` & `pjplan-0.0.9/docs/_build/doctrees/ru/toc.doctree`

 * *Files 13% similar despite different names*

```diff
@@ -1,166 +1,154 @@
-00000000: 8005 9551 0a00 0000 0000 008c 0f73 7068  ...Q.........sph
+00000000: 8005 9594 0900 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
-00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
-00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
-00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
-00000080: 6594 9394 2981 947d 9428 6805 8c03 7372  e...)..}.(h...sr
-00000090: 6394 6807 5d94 6809 8c04 5465 7874 9493  c.h.].h...Text..
-000000a0: 948c 0373 7263 9485 9481 947d 9428 8c06  ...src.....}.(..
-000000b0: 7061 7265 6e74 9468 118c 095f 646f 6375  parent.h..._docu
-000000c0: 6d65 6e74 9468 038c 0673 6f75 7263 6594  ment.h...source.
-000000d0: 4e8c 046c 696e 6594 4e75 6261 8c0a 6174  N..line.Nuba..at
-000000e0: 7472 6962 7574 6573 947d 9428 8c03 6964  tributes.}.(..id
-000000f0: 7394 5d94 8c07 636c 6173 7365 7394 5d94  s.]...classes.].
-00000100: 8c05 6e61 6d65 7394 5d94 8c08 6475 706e  ..names.]...dupn
-00000110: 616d 6573 945d 948c 0862 6163 6b72 6566  ames.]...backref
-00000120: 7394 5d94 758c 0774 6167 6e61 6d65 9468  s.].u..tagname.h
-00000130: 0f68 1b68 0c68 1c68 0368 1d8c 2a44 3a5c  .h.h.h.h.h..*D:\
-00000140: 686f 6d65 5c70 7970 726f 6a65 6374 735c  home\pyprojects\
-00000150: 706a 706c 616e 5c64 6f63 735c 6d6f 6475  pjplan\docs\modu
-00000160: 6c65 732e 7273 7494 681e 4b02 7562 6809  les.rst.h.K.ubh.
-00000170: 8c08 636f 6d70 6f75 6e64 9493 9429 8194  ..compound...)..
-00000180: 7d94 2868 0568 0668 075d 9468 008c 0774  }.(h.h.h.].h...t
-00000190: 6f63 7472 6565 9493 9429 8194 7d94 2868  octree...)..}.(h
-000001a0: 0568 0668 075d 9468 1f7d 9428 6821 5d94  .h.h.].h.}.(h!].
-000001b0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000001c0: 681b 8c07 6d6f 6475 6c65 7394 8c07 656e  h...modules...en
-000001d0: 7472 6965 7394 5d94 4e8c 0670 6a70 6c61  tries.].N..pjpla
-000001e0: 6e94 8694 618c 0c69 6e63 6c75 6465 6669  n...a..includefi
-000001f0: 6c65 7394 5d94 6840 618c 086d 6178 6465  les.].h@a..maxde
-00000200: 7074 6894 4b04 8c07 6361 7074 696f 6e94  pth.K...caption.
-00000210: 4e8c 0467 6c6f 6294 898c 0668 6964 6465  N..glob....hidde
-00000220: 6e94 898c 0d69 6e63 6c75 6465 6869 6464  n....includehidd
-00000230: 656e 9489 8c08 6e75 6d62 6572 6564 944b  en....numbered.K
-00000240: 008c 0a74 6974 6c65 736f 6e6c 7994 898c  ...titlesonly...
-00000250: 0a72 6177 656e 7472 6965 7394 5d94 7568  .rawentries.].uh
-00000260: 2b68 3268 1d68 2c68 1e4b 0468 1b68 2f75  +h2h.h,h.K.h.h/u
-00000270: 6261 681f 7d94 2868 215d 9468 235d 948c  bah.}.(h!].h#]..
-00000280: 0f74 6f63 7472 6565 2d77 7261 7070 6572  .toctree-wrapper
-00000290: 9461 6825 5d94 6827 5d94 6829 5d94 7568  .ah%].h'].h)].uh
-000002a0: 2b68 2d68 1b68 0c68 1c68 0368 1d68 2c68  +h-h.h.h.h.h.h,h
-000002b0: 1e4e 7562 6568 1f7d 9428 6821 5d94 8c03  .Nubeh.}.(h!]...
-000002c0: 7372 6394 6168 235d 9468 255d 948c 0373  src.ah#].h%]...s
-000002d0: 7263 9461 6827 5d94 6829 5d94 7568 2b68  rc.ah'].h)].uh+h
-000002e0: 0a68 1b68 0368 1c68 0368 1d68 2c68 1e4b  .h.h.h.h.h.h,h.K
-000002f0: 0275 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-00000300: 9468 255d 9468 275d 9468 295d 948c 0673  .h%].h'].h)]...s
-00000310: 6f75 7263 6594 682c 7568 2b68 018c 0e63  ource.h,uh+h...c
-00000320: 7572 7265 6e74 5f73 6f75 7263 6594 4e8c  urrent_source.N.
-00000330: 0c63 7572 7265 6e74 5f6c 696e 6594 4e8c  .current_line.N.
-00000340: 0873 6574 7469 6e67 7394 8c11 646f 6375  .settings...docu
-00000350: 7469 6c73 2e66 726f 6e74 656e 6494 8c06  tils.frontend...
-00000360: 5661 6c75 6573 9493 9429 8194 7d94 2868  Values...)..}.(h
-00000370: 0f4e 8c09 6765 6e65 7261 746f 7294 4e8c  .N..generator.N.
-00000380: 0964 6174 6573 7461 6d70 944e 8c0b 736f  .datestamp.N..so
-00000390: 7572 6365 5f6c 696e 6b94 4e8c 0a73 6f75  urce_link.N..sou
-000003a0: 7263 655f 7572 6c94 4e8c 0d74 6f63 5f62  rce_url.N..toc_b
-000003b0: 6163 6b6c 696e 6b73 948c 0565 6e74 7279  acklinks...entry
-000003c0: 948c 1266 6f6f 746e 6f74 655f 6261 636b  ...footnote_back
-000003d0: 6c69 6e6b 7394 4b01 8c0d 7365 6374 6e75  links.K...sectnu
-000003e0: 6d5f 7866 6f72 6d94 4b01 8c0e 7374 7269  m_xform.K...stri
-000003f0: 705f 636f 6d6d 656e 7473 944e 8c1b 7374  p_comments.N..st
-00000400: 7269 705f 656c 656d 656e 7473 5f77 6974  rip_elements_wit
-00000410: 685f 636c 6173 7365 7394 4e8c 0d73 7472  h_classes.N..str
-00000420: 6970 5f63 6c61 7373 6573 944e 8c0c 7265  ip_classes.N..re
-00000430: 706f 7274 5f6c 6576 656c 944b 028c 0a68  port_level.K...h
-00000440: 616c 745f 6c65 7665 6c94 4b05 8c11 6578  alt_level.K...ex
-00000450: 6974 5f73 7461 7475 735f 6c65 7665 6c94  it_status_level.
-00000460: 4b05 8c05 6465 6275 6794 4e8c 0e77 6172  K...debug.N..war
-00000470: 6e69 6e67 5f73 7472 6561 6d94 4e8c 0974  ning_stream.N..t
-00000480: 7261 6365 6261 636b 9488 8c0e 696e 7075  raceback....inpu
-00000490: 745f 656e 636f 6469 6e67 948c 0975 7466  t_encoding...utf
-000004a0: 2d38 2d73 6967 948c 1c69 6e70 7574 5f65  -8-sig...input_e
-000004b0: 6e63 6f64 696e 675f 6572 726f 725f 6861  ncoding_error_ha
-000004c0: 6e64 6c65 7294 8c06 7374 7269 6374 948c  ndler...strict..
-000004d0: 0f6f 7574 7075 745f 656e 636f 6469 6e67  .output_encoding
-000004e0: 948c 0575 7466 2d38 948c 1d6f 7574 7075  ...utf-8...outpu
-000004f0: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
-00000500: 5f68 616e 646c 6572 9468 7f8c 0e65 7272  _handler.h...err
-00000510: 6f72 5f65 6e63 6f64 696e 6794 8c05 7574  or_encoding...ut
-00000520: 662d 3894 8c1c 6572 726f 725f 656e 636f  f-8...error_enco
-00000530: 6469 6e67 5f65 7272 6f72 5f68 616e 646c  ding_error_handl
-00000540: 6572 948c 1062 6163 6b73 6c61 7368 7265  er...backslashre
-00000550: 706c 6163 6594 8c0d 6c61 6e67 7561 6765  place...language
-00000560: 5f63 6f64 6594 8c02 656e 948c 1372 6563  _code...en...rec
-00000570: 6f72 645f 6465 7065 6e64 656e 6369 6573  ord_dependencies
-00000580: 944e 8c06 636f 6e66 6967 944e 8c09 6964  .N..config.N..id
-00000590: 5f70 7265 6669 7894 6806 8c0e 6175 746f  _prefix.h...auto
-000005a0: 5f69 645f 7072 6566 6978 948c 0269 6494  _id_prefix...id.
-000005b0: 8c0d 6475 6d70 5f73 6574 7469 6e67 7394  ..dump_settings.
-000005c0: 4e8c 0e64 756d 705f 696e 7465 726e 616c  N..dump_internal
-000005d0: 7394 4e8c 0f64 756d 705f 7472 616e 7366  s.N..dump_transf
-000005e0: 6f72 6d73 944e 8c0f 6475 6d70 5f70 7365  orms.N..dump_pse
-000005f0: 7564 6f5f 786d 6c94 4e8c 1065 7870 6f73  udo_xml.N..expos
-00000600: 655f 696e 7465 726e 616c 7394 4e8c 0e73  e_internals.N..s
-00000610: 7472 6963 745f 7669 7369 746f 7294 4e8c  trict_visitor.N.
-00000620: 0f5f 6469 7361 626c 655f 636f 6e66 6967  ._disable_config
-00000630: 944e 8c07 5f73 6f75 7263 6594 682c 8c0c  .N.._source.h,..
-00000640: 5f64 6573 7469 6e61 7469 6f6e 944e 8c0d  _destination.N..
-00000650: 5f63 6f6e 6669 675f 6669 6c65 7394 5d94  _config_files.].
-00000660: 8c16 6669 6c65 5f69 6e73 6572 7469 6f6e  ..file_insertion
-00000670: 5f65 6e61 626c 6564 9488 8c0b 7261 775f  _enabled....raw_
-00000680: 656e 6162 6c65 6494 4b01 8c11 6c69 6e65  enabled.K...line
-00000690: 5f6c 656e 6774 685f 6c69 6d69 7494 4d10  _length_limit.M.
-000006a0: 278c 0e70 6570 5f72 6566 6572 656e 6365  '..pep_reference
-000006b0: 7394 4e8c 0c70 6570 5f62 6173 655f 7572  s.N..pep_base_ur
-000006c0: 6c94 8c18 6874 7470 733a 2f2f 7065 7073  l...https://peps
-000006d0: 2e70 7974 686f 6e2e 6f72 672f 948c 1570  .python.org/...p
-000006e0: 6570 5f66 696c 655f 7572 6c5f 7465 6d70  ep_file_url_temp
-000006f0: 6c61 7465 948c 0870 6570 2d25 3034 6494  late...pep-%04d.
-00000700: 8c0e 7266 635f 7265 6665 7265 6e63 6573  ..rfc_references
-00000710: 944e 8c0c 7266 635f 6261 7365 5f75 726c  .N..rfc_base_url
-00000720: 948c 2668 7474 7073 3a2f 2f64 6174 6174  ..&https://datat
-00000730: 7261 636b 6572 2e69 6574 662e 6f72 672f  racker.ietf.org/
-00000740: 646f 632f 6874 6d6c 2f94 8c09 7461 625f  doc/html/...tab_
-00000750: 7769 6474 6894 4b08 8c1d 7472 696d 5f66  width.K...trim_f
-00000760: 6f6f 746e 6f74 655f 7265 6665 7265 6e63  ootnote_referenc
-00000770: 655f 7370 6163 6594 898c 1073 796e 7461  e_space....synta
-00000780: 785f 6869 6768 6c69 6768 7494 8c04 6c6f  x_highlight...lo
-00000790: 6e67 948c 0c73 6d61 7274 5f71 756f 7465  ng...smart_quote
-000007a0: 7394 888c 1373 6d61 7274 7175 6f74 6573  s....smartquotes
-000007b0: 5f6c 6f63 616c 6573 945d 948c 1d63 6861  _locales.]...cha
-000007c0: 7261 6374 6572 5f6c 6576 656c 5f69 6e6c  racter_level_inl
-000007d0: 696e 655f 6d61 726b 7570 9489 8c0e 646f  ine_markup....do
-000007e0: 6374 6974 6c65 5f78 666f 726d 9489 8c0d  ctitle_xform....
-000007f0: 646f 6369 6e66 6f5f 7866 6f72 6d94 4b01  docinfo_xform.K.
-00000800: 8c12 7365 6374 7375 6274 6974 6c65 5f78  ..sectsubtitle_x
-00000810: 666f 726d 9489 8c0d 696d 6167 655f 6c6f  form....image_lo
-00000820: 6164 696e 6794 8c04 6c69 6e6b 948c 1065  ading...link...e
-00000830: 6d62 6564 5f73 7479 6c65 7368 6565 7494  mbed_stylesheet.
-00000840: 898c 1563 6c6f 616b 5f65 6d61 696c 5f61  ...cloak_email_a
-00000850: 6464 7265 7373 6573 9488 8c11 7365 6374  ddresses....sect
-00000860: 696f 6e5f 7365 6c66 5f6c 696e 6b94 898c  ion_self_link...
-00000870: 0365 6e76 944e 7562 8c08 7265 706f 7274  .env.Nub..report
-00000880: 6572 944e 8c10 696e 6469 7265 6374 5f74  er.N..indirect_t
-00000890: 6172 6765 7473 945d 948c 1173 7562 7374  argets.]...subst
-000008a0: 6974 7574 696f 6e5f 6465 6673 947d 948c  itution_defs.}..
-000008b0: 1273 7562 7374 6974 7574 696f 6e5f 6e61  .substitution_na
-000008c0: 6d65 7394 7d94 8c08 7265 666e 616d 6573  mes.}...refnames
-000008d0: 947d 948c 0672 6566 6964 7394 7d94 8c07  .}...refids.}...
-000008e0: 6e61 6d65 6964 7394 7d94 6859 6856 738c  nameids.}.hYhVs.
-000008f0: 096e 616d 6574 7970 6573 947d 9468 5989  .nametypes.}.hY.
-00000900: 7368 217d 9468 5668 0c73 8c0d 666f 6f74  sh!}.hVh.s..foot
-00000910: 6e6f 7465 5f72 6566 7394 7d94 8c0d 6369  note_refs.}...ci
-00000920: 7461 7469 6f6e 5f72 6566 7394 7d94 8c0d  tation_refs.}...
-00000930: 6175 746f 666f 6f74 6e6f 7465 7394 5d94  autofootnotes.].
-00000940: 8c11 6175 746f 666f 6f74 6e6f 7465 5f72  ..autofootnote_r
-00000950: 6566 7394 5d94 8c10 7379 6d62 6f6c 5f66  efs.]...symbol_f
-00000960: 6f6f 746e 6f74 6573 945d 948c 1473 796d  ootnotes.]...sym
-00000970: 626f 6c5f 666f 6f74 6e6f 7465 5f72 6566  bol_footnote_ref
-00000980: 7394 5d94 8c09 666f 6f74 6e6f 7465 7394  s.]...footnotes.
-00000990: 5d94 8c09 6369 7461 7469 6f6e 7394 5d94  ]...citations.].
-000009a0: 8c12 6175 746f 666f 6f74 6e6f 7465 5f73  ..autofootnote_s
-000009b0: 7461 7274 944b 018c 1573 796d 626f 6c5f  tart.K...symbol_
-000009c0: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
-000009d0: 008c 0a69 645f 636f 756e 7465 7294 8c0b  ...id_counter...
-000009e0: 636f 6c6c 6563 7469 6f6e 7394 8c07 436f  collections...Co
-000009f0: 756e 7465 7294 9394 7d94 8594 5294 8c0e  unter...}...R...
-00000a00: 7061 7273 655f 6d65 7373 6167 6573 945d  parse_messages.]
-00000a10: 948c 1274 7261 6e73 666f 726d 5f6d 6573  ...transform_mes
-00000a20: 7361 6765 7394 5d94 8c0b 7472 616e 7366  sages.]...transf
-00000a30: 6f72 6d65 7294 4e8c 0b69 6e63 6c75 6465  ormer.N..include
-00000a40: 5f6c 6f67 945d 948c 0a64 6563 6f72 6174  _log.]...decorat
-00000a50: 696f 6e94 4e68 1c68 0375 622e            ion.Nh.h.ub.
+00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0863  cutils.nodes...c
+00000060: 6f6d 706f 756e 6494 9394 2981 947d 9428  ompound...)..}.(
+00000070: 6805 6806 6807 5d94 6800 8c07 746f 6374  h.h.h.].h...toct
+00000080: 7265 6594 9394 2981 947d 9428 6805 6806  ree...)..}.(h.h.
+00000090: 6807 5d94 8c0a 6174 7472 6962 7574 6573  h.]...attributes
+000000a0: 947d 9428 8c03 6964 7394 5d94 8c07 636c  .}.(..ids.]...cl
+000000b0: 6173 7365 7394 5d94 8c05 6e61 6d65 7394  asses.]...names.
+000000c0: 5d94 8c08 6475 706e 616d 6573 945d 948c  ]...dupnames.]..
+000000d0: 0862 6163 6b72 6566 7394 5d94 8c06 7061  .backrefs.]...pa
+000000e0: 7265 6e74 948c 0672 752f 746f 6394 8c07  rent...ru/toc...
+000000f0: 656e 7472 6965 7394 5d94 284e 8c08 7275  entries.].(N..ru
+00000100: 2f69 6e64 6578 9486 944e 8c0f 7275 2f69  /index...N..ru/i
+00000110: 6e73 7461 6c6c 6174 696f 6e94 8694 658c  nstallation...e.
+00000120: 0c69 6e63 6c75 6465 6669 6c65 7394 5d94  .includefiles.].
+00000130: 2868 2468 2665 8c08 6d61 7864 6570 7468  (h$h&e..maxdepth
+00000140: 944a ffff ffff 8c07 6361 7074 696f 6e94  .J......caption.
+00000150: 4e8c 0467 6c6f 6294 888c 0668 6964 6465  N..glob....hidde
+00000160: 6e94 888c 0d69 6e63 6c75 6465 6869 6464  n....includehidd
+00000170: 656e 9489 8c08 6e75 6d62 6572 6564 944b  en....numbered.K
+00000180: 008c 0a74 6974 6c65 736f 6e6c 7994 898c  ...titlesonly...
+00000190: 0a72 6177 656e 7472 6965 7394 5d94 758c  .rawentries.].u.
+000001a0: 0774 6167 6e61 6d65 9468 0f8c 0673 6f75  .tagname.h...sou
+000001b0: 7263 6594 8c29 443a 5c68 6f6d 655c 7079  rce..)D:\home\py
+000001c0: 7072 6f6a 6563 7473 5c70 6a70 6c61 6e5c  projects\pjplan\
+000001d0: 646f 6373 5c72 755c 746f 632e 7273 7494  docs\ru\toc.rst.
+000001e0: 8c04 6c69 6e65 944b 0168 2068 0c75 6261  ..line.K.h h.uba
+000001f0: 6814 7d94 2868 165d 9468 185d 948c 0f74  h.}.(h.].h.]...t
+00000200: 6f63 7472 6565 2d77 7261 7070 6572 9461  octree-wrapper.a
+00000210: 681a 5d94 681c 5d94 681e 5d94 7568 3368  h.].h.].h.].uh3h
+00000220: 0a68 2068 038c 095f 646f 6375 6d65 6e74  .h h..._document
+00000230: 9468 0368 3468 3568 364e 7562 6168 147d  .h.h4h5h6Nubah.}
+00000240: 9428 6816 5d94 6818 5d94 681a 5d94 681c  .(h.].h.].h.].h.
+00000250: 5d94 681e 5d94 8c06 736f 7572 6365 9468  ].h.]...source.h
+00000260: 3575 6833 6801 8c0e 6375 7272 656e 745f  5uh3h...current_
+00000270: 736f 7572 6365 944e 8c0c 6375 7272 656e  source.N..curren
+00000280: 745f 6c69 6e65 944e 8c08 7365 7474 696e  t_line.N..settin
+00000290: 6773 948c 1164 6f63 7574 696c 732e 6672  gs...docutils.fr
+000002a0: 6f6e 7465 6e64 948c 0656 616c 7565 7394  ontend...Values.
+000002b0: 9394 2981 947d 9428 8c05 7469 746c 6594  ..)..}.(..title.
+000002c0: 4e8c 0967 656e 6572 6174 6f72 944e 8c09  N..generator.N..
+000002d0: 6461 7465 7374 616d 7094 4e8c 0b73 6f75  datestamp.N..sou
+000002e0: 7263 655f 6c69 6e6b 944e 8c0a 736f 7572  rce_link.N..sour
+000002f0: 6365 5f75 726c 944e 8c0d 746f 635f 6261  ce_url.N..toc_ba
+00000300: 636b 6c69 6e6b 7394 8c05 656e 7472 7994  cklinks...entry.
+00000310: 8c12 666f 6f74 6e6f 7465 5f62 6163 6b6c  ..footnote_backl
+00000320: 696e 6b73 944b 018c 0d73 6563 746e 756d  inks.K...sectnum
+00000330: 5f78 666f 726d 944b 018c 0e73 7472 6970  _xform.K...strip
+00000340: 5f63 6f6d 6d65 6e74 7394 4e8c 1b73 7472  _comments.N..str
+00000350: 6970 5f65 6c65 6d65 6e74 735f 7769 7468  ip_elements_with
+00000360: 5f63 6c61 7373 6573 944e 8c0d 7374 7269  _classes.N..stri
+00000370: 705f 636c 6173 7365 7394 4e8c 0c72 6570  p_classes.N..rep
+00000380: 6f72 745f 6c65 7665 6c94 4b02 8c0a 6861  ort_level.K...ha
+00000390: 6c74 5f6c 6576 656c 944b 058c 1165 7869  lt_level.K...exi
+000003a0: 745f 7374 6174 7573 5f6c 6576 656c 944b  t_status_level.K
+000003b0: 058c 0564 6562 7567 944e 8c0e 7761 726e  ...debug.N..warn
+000003c0: 696e 675f 7374 7265 616d 944e 8c09 7472  ing_stream.N..tr
+000003d0: 6163 6562 6163 6b94 888c 0e69 6e70 7574  aceback....input
+000003e0: 5f65 6e63 6f64 696e 6794 8c09 7574 662d  _encoding...utf-
+000003f0: 382d 7369 6794 8c1c 696e 7075 745f 656e  8-sig...input_en
+00000400: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
+00000410: 646c 6572 948c 0673 7472 6963 7494 8c0f  dler...strict...
+00000420: 6f75 7470 7574 5f65 6e63 6f64 696e 6794  output_encoding.
+00000430: 8c05 7574 662d 3894 8c1d 6f75 7470 7574  ..utf-8...output
+00000440: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
+00000450: 6861 6e64 6c65 7294 6863 8c0e 6572 726f  handler.hc..erro
+00000460: 725f 656e 636f 6469 6e67 948c 0575 7466  r_encoding...utf
+00000470: 2d38 948c 1c65 7272 6f72 5f65 6e63 6f64  -8...error_encod
+00000480: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+00000490: 7294 8c10 6261 636b 736c 6173 6872 6570  r...backslashrep
+000004a0: 6c61 6365 948c 0d6c 616e 6775 6167 655f  lace...language_
+000004b0: 636f 6465 948c 0265 6e94 8c13 7265 636f  code...en...reco
+000004c0: 7264 5f64 6570 656e 6465 6e63 6965 7394  rd_dependencies.
+000004d0: 4e8c 0663 6f6e 6669 6794 4e8c 0969 645f  N..config.N..id_
+000004e0: 7072 6566 6978 9468 068c 0e61 7574 6f5f  prefix.h...auto_
+000004f0: 6964 5f70 7265 6669 7894 8c02 6964 948c  id_prefix...id..
+00000500: 0d64 756d 705f 7365 7474 696e 6773 944e  .dump_settings.N
+00000510: 8c0e 6475 6d70 5f69 6e74 6572 6e61 6c73  ..dump_internals
+00000520: 944e 8c0f 6475 6d70 5f74 7261 6e73 666f  .N..dump_transfo
+00000530: 726d 7394 4e8c 0f64 756d 705f 7073 6575  rms.N..dump_pseu
+00000540: 646f 5f78 6d6c 944e 8c10 6578 706f 7365  do_xml.N..expose
+00000550: 5f69 6e74 6572 6e61 6c73 944e 8c0e 7374  _internals.N..st
+00000560: 7269 6374 5f76 6973 6974 6f72 944e 8c0f  rict_visitor.N..
+00000570: 5f64 6973 6162 6c65 5f63 6f6e 6669 6794  _disable_config.
+00000580: 4e8c 075f 736f 7572 6365 9468 358c 0c5f  N.._source.h5.._
+00000590: 6465 7374 696e 6174 696f 6e94 4e8c 0d5f  destination.N.._
+000005a0: 636f 6e66 6967 5f66 696c 6573 945d 948c  config_files.]..
+000005b0: 1666 696c 655f 696e 7365 7274 696f 6e5f  .file_insertion_
+000005c0: 656e 6162 6c65 6494 888c 0b72 6177 5f65  enabled....raw_e
+000005d0: 6e61 626c 6564 944b 018c 116c 696e 655f  nabled.K...line_
+000005e0: 6c65 6e67 7468 5f6c 696d 6974 944a 00e1  length_limit.J..
+000005f0: f505 8c0e 7065 705f 7265 6665 7265 6e63  ....pep_referenc
+00000600: 6573 944e 8c0c 7065 705f 6261 7365 5f75  es.N..pep_base_u
+00000610: 726c 948c 1868 7474 7073 3a2f 2f70 6570  rl...https://pep
+00000620: 732e 7079 7468 6f6e 2e6f 7267 2f94 8c15  s.python.org/...
+00000630: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
+00000640: 706c 6174 6594 8c08 7065 702d 2530 3464  plate...pep-%04d
+00000650: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
+00000660: 7394 4e8c 0c72 6663 5f62 6173 655f 7572  s.N..rfc_base_ur
+00000670: 6c94 8c26 6874 7470 733a 2f2f 6461 7461  l..&https://data
+00000680: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
+00000690: 2f64 6f63 2f68 746d 6c2f 948c 0974 6162  /doc/html/...tab
+000006a0: 5f77 6964 7468 944b 088c 1d74 7269 6d5f  _width.K...trim_
+000006b0: 666f 6f74 6e6f 7465 5f72 6566 6572 656e  footnote_referen
+000006c0: 6365 5f73 7061 6365 9489 8c10 7379 6e74  ce_space....synt
+000006d0: 6178 5f68 6967 686c 6967 6874 948c 046c  ax_highlight...l
+000006e0: 6f6e 6794 8c0c 736d 6172 745f 7175 6f74  ong...smart_quot
+000006f0: 6573 9488 8c13 736d 6172 7471 756f 7465  es....smartquote
+00000700: 735f 6c6f 6361 6c65 7394 5d94 8c1d 6368  s_locales.]...ch
+00000710: 6172 6163 7465 725f 6c65 7665 6c5f 696e  aracter_level_in
+00000720: 6c69 6e65 5f6d 6172 6b75 7094 898c 0e64  line_markup....d
+00000730: 6f63 7469 746c 655f 7866 6f72 6d94 898c  octitle_xform...
+00000740: 0d64 6f63 696e 666f 5f78 666f 726d 944b  .docinfo_xform.K
+00000750: 018c 1273 6563 7473 7562 7469 746c 655f  ...sectsubtitle_
+00000760: 7866 6f72 6d94 898c 0d69 6d61 6765 5f6c  xform....image_l
+00000770: 6f61 6469 6e67 948c 046c 696e 6b94 8c10  oading...link...
+00000780: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
+00000790: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
+000007a0: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
+000007b0: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
+000007c0: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
+000007d0: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
+000007e0: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
+000007f0: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
+00000800: 8c12 7375 6273 7469 7475 7469 6f6e 5f6e  ..substitution_n
+00000810: 616d 6573 947d 948c 0872 6566 6e61 6d65  ames.}...refname
+00000820: 7394 7d94 8c06 7265 6669 6473 947d 948c  s.}...refids.}..
+00000830: 076e 616d 6569 6473 947d 948c 096e 616d  .nameids.}...nam
+00000840: 6574 7970 6573 947d 9468 167d 948c 0d66  etypes.}.h.}...f
+00000850: 6f6f 746e 6f74 655f 7265 6673 947d 948c  ootnote_refs.}..
+00000860: 0d63 6974 6174 696f 6e5f 7265 6673 947d  .citation_refs.}
+00000870: 948c 0d61 7574 6f66 6f6f 746e 6f74 6573  ...autofootnotes
+00000880: 945d 948c 1161 7574 6f66 6f6f 746e 6f74  .]...autofootnot
+00000890: 655f 7265 6673 945d 948c 1073 796d 626f  e_refs.]...symbo
+000008a0: 6c5f 666f 6f74 6e6f 7465 7394 5d94 8c14  l_footnotes.]...
+000008b0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
+000008c0: 7265 6673 945d 948c 0966 6f6f 746e 6f74  refs.]...footnot
+000008d0: 6573 945d 948c 0963 6974 6174 696f 6e73  es.]...citations
+000008e0: 945d 948c 1261 7574 6f66 6f6f 746e 6f74  .]...autofootnot
+000008f0: 655f 7374 6172 7494 4b01 8c15 7379 6d62  e_start.K...symb
+00000900: 6f6c 5f66 6f6f 746e 6f74 655f 7374 6172  ol_footnote_star
+00000910: 7494 4b00 8c0a 6964 5f63 6f75 6e74 6572  t.K...id_counter
+00000920: 948c 0b63 6f6c 6c65 6374 696f 6e73 948c  ...collections..
+00000930: 0743 6f75 6e74 6572 9493 947d 9485 9452  .Counter...}...R
+00000940: 948c 0e70 6172 7365 5f6d 6573 7361 6765  ...parse_message
+00000950: 7394 5d94 8c12 7472 616e 7366 6f72 6d5f  s.]...transform_
+00000960: 6d65 7373 6167 6573 945d 948c 0b74 7261  messages.]...tra
+00000970: 6e73 666f 726d 6572 944e 8c0b 696e 636c  nsformer.N..incl
+00000980: 7564 655f 6c6f 6794 5d94 8c0a 6465 636f  ude_log.]...deco
+00000990: 7261 7469 6f6e 944e 683e 6803 7562 2e    ration.Nh>h.ub.
```

### Comparing `pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.doctree` & `pjplan-0.0.9/docs/_build/doctrees/en/installation.doctree`

 * *Files 19% similar despite different names*

```diff
@@ -1,222 +1,210 @@
-00000000: 8005 95d3 0d00 0000 0000 008c 0f73 7068  .............sph
+00000000: 8005 9510 0d00 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
-00000080: 6594 9394 2981 947d 9428 6805 8c12 706a  e...)..}.(h...pj
-00000090: 706c 616e 2e76 697a 2070 6163 6b61 6765  plan.viz package
-000000a0: 9468 075d 9468 098c 0454 6578 7494 9394  .h.].h...Text...
-000000b0: 8c12 706a 706c 616e 2e76 697a 2070 6163  ..pjplan.viz pac
-000000c0: 6b61 6765 9485 9481 947d 9428 8c06 7061  kage.....}.(..pa
-000000d0: 7265 6e74 9468 118c 095f 646f 6375 6d65  rent.h..._docume
-000000e0: 6e74 9468 038c 0673 6f75 7263 6594 4e8c  nt.h...source.N.
-000000f0: 046c 696e 6594 4e75 6261 8c0a 6174 7472  .line.Nuba..attr
-00000100: 6962 7574 6573 947d 9428 8c03 6964 7394  ibutes.}.(..ids.
-00000110: 5d94 8c07 636c 6173 7365 7394 5d94 8c05  ]...classes.]...
-00000120: 6e61 6d65 7394 5d94 8c08 6475 706e 616d  names.]...dupnam
-00000130: 6573 945d 948c 0862 6163 6b72 6566 7394  es.]...backrefs.
-00000140: 5d94 758c 0774 6167 6e61 6d65 9468 0f68  ].u..tagname.h.h
-00000150: 1b68 0c68 1c68 0368 1d8c 2d44 3a5c 686f  .h.h.h.h..-D:\ho
-00000160: 6d65 5c70 7970 726f 6a65 6374 735c 706a  me\pyprojects\pj
-00000170: 706c 616e 5c64 6f63 735c 706a 706c 616e  plan\docs\pjplan
-00000180: 2e76 697a 2e72 7374 9468 1e4b 0275 6268  .viz.rst.h.K.ubh
-00000190: 0b29 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-000001a0: 6810 2981 947d 9428 6805 8c0b 5375 6270  h.)..}.(h...Subp
-000001b0: 6163 6b61 6765 7394 6807 5d94 6816 8c0b  ackages.h.].h...
-000001c0: 5375 6270 6163 6b61 6765 7394 8594 8194  Subpackages.....
-000001d0: 7d94 2868 1b68 3068 1c68 0368 1d4e 681e  }.(h.h0h.h.h.Nh.
-000001e0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-000001f0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00000200: 680f 681b 682d 681c 6803 681d 682c 681e  h.h.h-h.h.h.h,h.
-00000210: 4b05 7562 6809 8c08 636f 6d70 6f75 6e64  K.ubh...compound
-00000220: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-00000230: 9468 008c 0774 6f63 7472 6565 9493 9429  .h...toctree...)
-00000240: 8194 7d94 2868 0568 0668 075d 9468 1f7d  ..}.(h.h.h.].h.}
-00000250: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00000260: 5d94 6829 5d94 681b 8c0a 706a 706c 616e  ].h)].h...pjplan
-00000270: 2e76 697a 948c 0765 6e74 7269 6573 945d  .viz...entries.]
-00000280: 9428 4e8c 1170 6a70 6c61 6e2e 7669 7a2e  .(N..pjplan.viz.
-00000290: 6468 746d 6c78 9486 944e 8c12 706a 706c  dhtmlx...N..pjpl
-000002a0: 616e 2e76 697a 2e6d 6572 6d61 6964 9486  an.viz.mermaid..
-000002b0: 9465 8c0c 696e 636c 7564 6566 696c 6573  .e..includefiles
-000002c0: 945d 9428 6851 6853 658c 086d 6178 6465  .].(hQhSe..maxde
-000002d0: 7074 6894 4b04 8c07 6361 7074 696f 6e94  pth.K...caption.
-000002e0: 4e8c 0467 6c6f 6294 898c 0668 6964 6465  N..glob....hidde
-000002f0: 6e94 898c 0d69 6e63 6c75 6465 6869 6464  n....includehidd
-00000300: 656e 9489 8c08 6e75 6d62 6572 6564 944b  en....numbered.K
-00000310: 008c 0a74 6974 6c65 736f 6e6c 7994 898c  ...titlesonly...
-00000320: 0a72 6177 656e 7472 6965 7394 5d94 7568  .rawentries.].uh
-00000330: 2b68 4368 1d68 2c68 1e4b 0768 1b68 4075  +hCh.h,h.K.h.h@u
-00000340: 6261 681f 7d94 2868 215d 9468 235d 948c  bah.}.(h!].h#]..
-00000350: 0f74 6f63 7472 6565 2d77 7261 7070 6572  .toctree-wrapper
-00000360: 9461 6825 5d94 6827 5d94 6829 5d94 7568  .ah%].h'].h)].uh
-00000370: 2b68 3e68 1b68 2d68 1c68 0368 1d68 2c68  +h>h.h-h.h.h.h,h
-00000380: 1e4e 7562 6568 1f7d 9428 6821 5d94 8c0b  .Nubeh.}.(h!]...
-00000390: 7375 6270 6163 6b61 6765 7394 6168 235d  subpackages.ah#]
-000003a0: 9468 255d 948c 0b73 7562 7061 636b 6167  .h%]...subpackag
-000003b0: 6573 9461 6827 5d94 6829 5d94 7568 2b68  es.ah'].h)].uh+h
-000003c0: 0a68 1b68 0c68 1c68 0368 1d68 2c68 1e4b  .h.h.h.h.h.h,h.K
-000003d0: 0575 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
-000003e0: 075d 9428 6810 2981 947d 9428 6805 8c0f  .].(h.)..}.(h...
-000003f0: 4d6f 6475 6c65 2063 6f6e 7465 6e74 7394  Module contents.
-00000400: 6807 5d94 6816 8c0f 4d6f 6475 6c65 2063  h.].h...Module c
-00000410: 6f6e 7465 6e74 7394 8594 8194 7d94 2868  ontents.....}.(h
-00000420: 1b68 7268 1c68 0368 1d4e 681e 4e75 6261  .hrh.h.h.Nh.Nuba
-00000430: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00000440: 9468 275d 9468 295d 9475 682b 680f 681b  .h'].h)].uh+h.h.
-00000450: 686f 681c 6803 681d 682c 681e 4b0e 7562  hoh.h.h.h,h.K.ub
-00000460: 6800 8c05 696e 6465 7894 9394 2981 947d  h...index...)..}
-00000470: 9428 6805 6806 6807 5d94 681f 7d94 2868  .(h.h.h.].h.}.(h
-00000480: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00000490: 295d 948c 0765 6e74 7269 6573 945d 9428  )]...entries.].(
-000004a0: 8c04 7061 6972 948c 126d 6f64 756c 653b  ..pair...module;
-000004b0: 2070 6a70 6c61 6e2e 7669 7a94 8c11 6d6f   pjplan.viz...mo
-000004c0: 6475 6c65 2d70 6a70 6c61 6e2e 7669 7a94  dule-pjplan.viz.
-000004d0: 6806 4e74 9461 7568 2b68 8068 1b68 6f68  h.Nt.auh+h.h.hoh
-000004e0: 1c68 0368 1d4e 681e 4e75 6265 681f 7d94  .h.h.Nh.Nubeh.}.
-000004f0: 2868 215d 9428 688f 8c0f 6d6f 6475 6c65  (h!].(h...module
-00000500: 2d63 6f6e 7465 6e74 7394 6568 235d 9468  -contents.eh#].h
-00000510: 255d 948c 0f6d 6f64 756c 6520 636f 6e74  %]...module cont
-00000520: 656e 7473 9461 6827 5d94 6829 5d94 7568  ents.ah'].h)].uh
-00000530: 2b68 0a68 1b68 0c68 1c68 0368 1d68 2c68  +h.h.h.h.h.h.h,h
-00000540: 1e4b 0e75 6265 681f 7d94 2868 215d 948c  .K.ubeh.}.(h!]..
-00000550: 1270 6a70 6c61 6e2d 7669 7a2d 7061 636b  .pjplan-viz-pack
-00000560: 6167 6594 6168 235d 9468 255d 948c 1270  age.ah#].h%]...p
-00000570: 6a70 6c61 6e2e 7669 7a20 7061 636b 6167  jplan.viz packag
-00000580: 6594 6168 275d 9468 295d 9475 682b 680a  e.ah'].h)].uh+h.
-00000590: 681b 6803 681c 6803 681d 682c 681e 4b02  h.h.h.h.h.h,h.K.
-000005a0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-000005b0: 6825 5d94 6827 5d94 6829 5d94 8c06 736f  h%].h'].h)]...so
-000005c0: 7572 6365 9468 2c75 682b 6801 8c0e 6375  urce.h,uh+h...cu
-000005d0: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
-000005e0: 6375 7272 656e 745f 6c69 6e65 944e 8c08  current_line.N..
-000005f0: 7365 7474 696e 6773 948c 1164 6f63 7574  settings...docut
-00000600: 696c 732e 6672 6f6e 7465 6e64 948c 0656  ils.frontend...V
-00000610: 616c 7565 7394 9394 2981 947d 9428 680f  alues...)..}.(h.
-00000620: 4e8c 0967 656e 6572 6174 6f72 944e 8c09  N..generator.N..
-00000630: 6461 7465 7374 616d 7094 4e8c 0b73 6f75  datestamp.N..sou
-00000640: 7263 655f 6c69 6e6b 944e 8c0a 736f 7572  rce_link.N..sour
-00000650: 6365 5f75 726c 944e 8c0d 746f 635f 6261  ce_url.N..toc_ba
-00000660: 636b 6c69 6e6b 7394 8c05 656e 7472 7994  cklinks...entry.
-00000670: 8c12 666f 6f74 6e6f 7465 5f62 6163 6b6c  ..footnote_backl
-00000680: 696e 6b73 944b 018c 0d73 6563 746e 756d  inks.K...sectnum
-00000690: 5f78 666f 726d 944b 018c 0e73 7472 6970  _xform.K...strip
-000006a0: 5f63 6f6d 6d65 6e74 7394 4e8c 1b73 7472  _comments.N..str
-000006b0: 6970 5f65 6c65 6d65 6e74 735f 7769 7468  ip_elements_with
-000006c0: 5f63 6c61 7373 6573 944e 8c0d 7374 7269  _classes.N..stri
-000006d0: 705f 636c 6173 7365 7394 4e8c 0c72 6570  p_classes.N..rep
-000006e0: 6f72 745f 6c65 7665 6c94 4b02 8c0a 6861  ort_level.K...ha
-000006f0: 6c74 5f6c 6576 656c 944b 058c 1165 7869  lt_level.K...exi
-00000700: 745f 7374 6174 7573 5f6c 6576 656c 944b  t_status_level.K
-00000710: 058c 0564 6562 7567 944e 8c0e 7761 726e  ...debug.N..warn
-00000720: 696e 675f 7374 7265 616d 944e 8c09 7472  ing_stream.N..tr
-00000730: 6163 6562 6163 6b94 888c 0e69 6e70 7574  aceback....input
-00000740: 5f65 6e63 6f64 696e 6794 8c09 7574 662d  _encoding...utf-
-00000750: 382d 7369 6794 8c1c 696e 7075 745f 656e  8-sig...input_en
-00000760: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00000770: 646c 6572 948c 0673 7472 6963 7494 8c0f  dler...strict...
-00000780: 6f75 7470 7574 5f65 6e63 6f64 696e 6794  output_encoding.
-00000790: 8c05 7574 662d 3894 8c1d 6f75 7470 7574  ..utf-8...output
-000007a0: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
-000007b0: 6861 6e64 6c65 7294 68c4 8c0e 6572 726f  handler.h...erro
-000007c0: 725f 656e 636f 6469 6e67 948c 0575 7466  r_encoding...utf
-000007d0: 2d38 948c 1c65 7272 6f72 5f65 6e63 6f64  -8...error_encod
-000007e0: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-000007f0: 7294 8c10 6261 636b 736c 6173 6872 6570  r...backslashrep
-00000800: 6c61 6365 948c 0d6c 616e 6775 6167 655f  lace...language_
-00000810: 636f 6465 948c 0265 6e94 8c13 7265 636f  code...en...reco
-00000820: 7264 5f64 6570 656e 6465 6e63 6965 7394  rd_dependencies.
-00000830: 4e8c 0663 6f6e 6669 6794 4e8c 0969 645f  N..config.N..id_
-00000840: 7072 6566 6978 9468 068c 0e61 7574 6f5f  prefix.h...auto_
-00000850: 6964 5f70 7265 6669 7894 8c02 6964 948c  id_prefix...id..
-00000860: 0d64 756d 705f 7365 7474 696e 6773 944e  .dump_settings.N
-00000870: 8c0e 6475 6d70 5f69 6e74 6572 6e61 6c73  ..dump_internals
-00000880: 944e 8c0f 6475 6d70 5f74 7261 6e73 666f  .N..dump_transfo
-00000890: 726d 7394 4e8c 0f64 756d 705f 7073 6575  rms.N..dump_pseu
-000008a0: 646f 5f78 6d6c 944e 8c10 6578 706f 7365  do_xml.N..expose
-000008b0: 5f69 6e74 6572 6e61 6c73 944e 8c0e 7374  _internals.N..st
-000008c0: 7269 6374 5f76 6973 6974 6f72 944e 8c0f  rict_visitor.N..
-000008d0: 5f64 6973 6162 6c65 5f63 6f6e 6669 6794  _disable_config.
-000008e0: 4e8c 075f 736f 7572 6365 9468 2c8c 0c5f  N.._source.h,.._
-000008f0: 6465 7374 696e 6174 696f 6e94 4e8c 0d5f  destination.N.._
-00000900: 636f 6e66 6967 5f66 696c 6573 945d 948c  config_files.]..
-00000910: 1666 696c 655f 696e 7365 7274 696f 6e5f  .file_insertion_
-00000920: 656e 6162 6c65 6494 888c 0b72 6177 5f65  enabled....raw_e
-00000930: 6e61 626c 6564 944b 018c 116c 696e 655f  nabled.K...line_
-00000940: 6c65 6e67 7468 5f6c 696d 6974 944d 1027  length_limit.M.'
-00000950: 8c0e 7065 705f 7265 6665 7265 6e63 6573  ..pep_references
-00000960: 944e 8c0c 7065 705f 6261 7365 5f75 726c  .N..pep_base_url
-00000970: 948c 1868 7474 7073 3a2f 2f70 6570 732e  ...https://peps.
-00000980: 7079 7468 6f6e 2e6f 7267 2f94 8c15 7065  python.org/...pe
-00000990: 705f 6669 6c65 5f75 726c 5f74 656d 706c  p_file_url_templ
-000009a0: 6174 6594 8c08 7065 702d 2530 3464 948c  ate...pep-%04d..
-000009b0: 0e72 6663 5f72 6566 6572 656e 6365 7394  .rfc_references.
-000009c0: 4e8c 0c72 6663 5f62 6173 655f 7572 6c94  N..rfc_base_url.
-000009d0: 8c26 6874 7470 733a 2f2f 6461 7461 7472  .&https://datatr
-000009e0: 6163 6b65 722e 6965 7466 2e6f 7267 2f64  acker.ietf.org/d
-000009f0: 6f63 2f68 746d 6c2f 948c 0974 6162 5f77  oc/html/...tab_w
-00000a00: 6964 7468 944b 088c 1d74 7269 6d5f 666f  idth.K...trim_fo
-00000a10: 6f74 6e6f 7465 5f72 6566 6572 656e 6365  otnote_reference
-00000a20: 5f73 7061 6365 9489 8c10 7379 6e74 6178  _space....syntax
-00000a30: 5f68 6967 686c 6967 6874 948c 046c 6f6e  _highlight...lon
-00000a40: 6794 8c0c 736d 6172 745f 7175 6f74 6573  g...smart_quotes
-00000a50: 9488 8c13 736d 6172 7471 756f 7465 735f  ....smartquotes_
-00000a60: 6c6f 6361 6c65 7394 5d94 8c1d 6368 6172  locales.]...char
-00000a70: 6163 7465 725f 6c65 7665 6c5f 696e 6c69  acter_level_inli
-00000a80: 6e65 5f6d 6172 6b75 7094 898c 0e64 6f63  ne_markup....doc
-00000a90: 7469 746c 655f 7866 6f72 6d94 898c 0d64  title_xform....d
-00000aa0: 6f63 696e 666f 5f78 666f 726d 944b 018c  ocinfo_xform.K..
-00000ab0: 1273 6563 7473 7562 7469 746c 655f 7866  .sectsubtitle_xf
-00000ac0: 6f72 6d94 898c 0d69 6d61 6765 5f6c 6f61  orm....image_loa
-00000ad0: 6469 6e67 948c 046c 696e 6b94 8c10 656d  ding...link...em
-00000ae0: 6265 645f 7374 796c 6573 6865 6574 9489  bed_stylesheet..
-00000af0: 8c15 636c 6f61 6b5f 656d 6169 6c5f 6164  ..cloak_email_ad
-00000b00: 6472 6573 7365 7394 888c 1173 6563 7469  dresses....secti
-00000b10: 6f6e 5f73 656c 665f 6c69 6e6b 9489 8c03  on_self_link....
-00000b20: 656e 7694 4e75 628c 0872 6570 6f72 7465  env.Nub..reporte
-00000b30: 7294 4e8c 1069 6e64 6972 6563 745f 7461  r.N..indirect_ta
-00000b40: 7267 6574 7394 5d94 8c11 7375 6273 7469  rgets.]...substi
-00000b50: 7475 7469 6f6e 5f64 6566 7394 7d94 8c12  tution_defs.}...
-00000b60: 7375 6273 7469 7475 7469 6f6e 5f6e 616d  substitution_nam
-00000b70: 6573 947d 948c 0872 6566 6e61 6d65 7394  es.}...refnames.
-00000b80: 7d94 8c06 7265 6669 6473 947d 948c 076e  }...refids.}...n
-00000b90: 616d 6569 6473 947d 9428 689e 689b 686c  ameids.}.(h.h.hl
-00000ba0: 6869 6896 6893 758c 096e 616d 6574 7970  hih.h.u..nametyp
-00000bb0: 6573 947d 9428 689e 8968 6c89 6896 8975  es.}.(h..hl.h..u
-00000bc0: 6821 7d94 2868 9b68 0c68 6968 2d68 9368  h!}.(h.h.hih-h.h
-00000bd0: 6f68 8f68 098c 0674 6172 6765 7494 9394  oh.h...target...
-00000be0: 2981 947d 9428 6805 6806 6807 5d94 681f  )..}.(h.h.h.].h.
-00000bf0: 7d94 2868 215d 9468 8f61 6823 5d94 6825  }.(h!].h.ah#].h%
-00000c00: 5d94 6827 5d94 6829 5d94 8c05 6973 6d6f  ].h'].h)]...ismo
-00000c10: 6494 8875 682b 6a0a 0100 0068 1d8c 5d44  d..uh+j....h..]D
-00000c20: 3a5c 686f 6d65 5c64 6576 746f 6f6c 735c  :\home\devtools\
-00000c30: 7079 7468 6f6e 2d33 2e31 305c 6c69 625c  python-3.10\lib\
-00000c40: 7369 7465 2d70 6163 6b61 6765 735c 706a  site-packages\pj
-00000c50: 706c 616e 5c76 697a 5c5f 5f69 6e69 745f  plan\viz\__init_
-00000c60: 5f2e 7079 3a64 6f63 7374 7269 6e67 206f  _.py:docstring o
-00000c70: 6620 706a 706c 616e 2e76 697a 9468 1e4b  f pjplan.viz.h.K
-00000c80: 0168 1b68 6f68 1c68 0375 6275 8c0d 666f  .h.hoh.h.ubu..fo
-00000c90: 6f74 6e6f 7465 5f72 6566 7394 7d94 8c0d  otnote_refs.}...
-00000ca0: 6369 7461 7469 6f6e 5f72 6566 7394 7d94  citation_refs.}.
-00000cb0: 8c0d 6175 746f 666f 6f74 6e6f 7465 7394  ..autofootnotes.
-00000cc0: 5d94 8c11 6175 746f 666f 6f74 6e6f 7465  ]...autofootnote
-00000cd0: 5f72 6566 7394 5d94 8c10 7379 6d62 6f6c  _refs.]...symbol
-00000ce0: 5f66 6f6f 746e 6f74 6573 945d 948c 1473  _footnotes.]...s
-00000cf0: 796d 626f 6c5f 666f 6f74 6e6f 7465 5f72  ymbol_footnote_r
-00000d00: 6566 7394 5d94 8c09 666f 6f74 6e6f 7465  efs.]...footnote
-00000d10: 7394 5d94 8c09 6369 7461 7469 6f6e 7394  s.]...citations.
-00000d20: 5d94 8c12 6175 746f 666f 6f74 6e6f 7465  ]...autofootnote
-00000d30: 5f73 7461 7274 944b 018c 1573 796d 626f  _start.K...symbo
-00000d40: 6c5f 666f 6f74 6e6f 7465 5f73 7461 7274  l_footnote_start
-00000d50: 944b 008c 0a69 645f 636f 756e 7465 7294  .K...id_counter.
-00000d60: 8c0b 636f 6c6c 6563 7469 6f6e 7394 8c07  ..collections...
-00000d70: 436f 756e 7465 7294 9394 7d94 8594 5294  Counter...}...R.
-00000d80: 8c0e 7061 7273 655f 6d65 7373 6167 6573  ..parse_messages
-00000d90: 945d 948c 1274 7261 6e73 666f 726d 5f6d  .]...transform_m
-00000da0: 6573 7361 6765 7394 5d94 8c0b 7472 616e  essages.]...tran
-00000db0: 7366 6f72 6d65 7294 4e8c 0b69 6e63 6c75  sformer.N..inclu
-00000dc0: 6465 5f6c 6f67 945d 948c 0a64 6563 6f72  de_log.]...decor
-00000dd0: 6174 696f 6e94 4e68 1c68 0375 622e       ation.Nh.h.ub.
+00000080: 6594 9394 2981 947d 9428 6805 8c0c 496e  e...)..}.(h...In
+00000090: 7374 616c 6c61 7469 6f6e 9468 075d 9468  stallation.h.].h
+000000a0: 098c 0454 6578 7494 9394 8c0c 496e 7374  ...Text.....Inst
+000000b0: 616c 6c61 7469 6f6e 9485 9481 947d 9428  allation.....}.(
+000000c0: 8c06 7061 7265 6e74 9468 118c 095f 646f  ..parent.h..._do
+000000d0: 6375 6d65 6e74 9468 038c 0673 6f75 7263  cument.h...sourc
+000000e0: 6594 4e8c 046c 696e 6594 4e75 6261 8c0a  e.N..line.Nuba..
+000000f0: 6174 7472 6962 7574 6573 947d 9428 8c03  attributes.}.(..
+00000100: 6964 7394 5d94 8c07 636c 6173 7365 7394  ids.]...classes.
+00000110: 5d94 8c05 6e61 6d65 7394 5d94 8c08 6475  ]...names.]...du
+00000120: 706e 616d 6573 945d 948c 0862 6163 6b72  pnames.]...backr
+00000130: 6566 7394 5d94 758c 0774 6167 6e61 6d65  efs.].u..tagname
+00000140: 9468 0f68 1e4b 0168 1d8c 3144 3a5c 686f  .h.h.K.h..1D:\ho
+00000150: 6d65 5c70 7970 726f 6a65 6374 735c 706a  me\pyprojects\pj
+00000160: 706c 616e 5c64 6f63 735c 656e 5c69 6e73  plan\docs\en\ins
+00000170: 7461 6c6c 6174 696f 6e2e 6d64 9468 1b68  tallation.md.h.h
+00000180: 0c68 1c68 0375 6268 098c 0970 6172 6167  .h.h.ubh...parag
+00000190: 7261 7068 9493 9429 8194 7d94 2868 058c  raph...)..}.(h..
+000001a0: 2b2a 2a70 6a70 6c61 6e2a 2a20 6973 2063  +**pjplan** is c
+000001b0: 6f6d 7061 7274 6962 6c65 2077 6974 6820  ompartible with 
+000001c0: 5079 7468 6f6e 2033 2e37 2b2e 9468 075d  Python 3.7+..h.]
+000001d0: 9428 6816 6806 8594 8194 7d94 2868 1b68  .(h.h.....}.(h.h
+000001e0: 2f68 1c68 0368 1d4e 681e 4e75 6268 098c  /h.h.h.Nh.Nubh..
+000001f0: 0673 7472 6f6e 6794 9394 2981 947d 9428  .strong...)..}.(
+00000200: 6805 8c06 706a 706c 616e 9468 075d 9468  h...pjplan.h.].h
+00000210: 168c 0670 6a70 6c61 6e94 8594 8194 7d94  ...pjplan.....}.
+00000220: 2868 1b68 3868 1c68 0368 1d4e 681e 4e75  (h.h8h.h.h.Nh.Nu
+00000230: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00000240: 255d 9468 275d 9468 295d 9475 682b 6836  %].h'].h)].uh+h6
+00000250: 681e 4b03 681d 682c 681b 682f 681c 6803  h.K.h.h,h.h/h.h.
+00000260: 7562 6816 8c21 2069 7320 636f 6d70 6172  ubh..! is compar
+00000270: 7469 626c 6520 7769 7468 2050 7974 686f  tible with Pytho
+00000280: 6e20 332e 372b 2e94 8594 8194 7d94 2868  n 3.7+......}.(h
+00000290: 1b68 2f68 1c68 0368 1d4e 681e 4e75 6265  .h/h.h.h.Nh.Nube
+000002a0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000002b0: 9468 275d 9468 295d 9475 682b 682d 681e  .h'].h)].uh+h-h.
+000002c0: 4b03 681d 682c 681b 680c 681c 6803 7562  K.h.h,h.h.h.h.ub
+000002d0: 682e 2981 947d 9428 6805 8c21 596f 7520  h.)..}.(h..!You 
+000002e0: 6361 6e20 696e 7374 616c 6c20 706a 706c  can install pjpl
+000002f0: 616e 2075 7369 6e67 2070 6970 3a94 6807  an using pip:.h.
+00000300: 5d94 6816 8c21 596f 7520 6361 6e20 696e  ].h..!You can in
+00000310: 7374 616c 6c20 706a 706c 616e 2075 7369  stall pjplan usi
+00000320: 6e67 2070 6970 3a94 8594 8194 7d94 2868  ng pip:.....}.(h
+00000330: 1b68 5068 1c68 0368 1d4e 681e 4e75 6261  .hPh.h.h.Nh.Nuba
+00000340: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000350: 9468 275d 9468 295d 9475 682b 682d 681e  .h'].h)].uh+h-h.
+00000360: 4b05 681d 682c 681b 680c 681c 6803 7562  K.h.h,h.h.h.h.ub
+00000370: 6809 8c0d 6c69 7465 7261 6c5f 626c 6f63  h...literal_bloc
+00000380: 6b94 9394 2981 947d 9428 6805 8c13 7069  k...)..}.(h...pi
+00000390: 7020 696e 7374 616c 6c20 706a 706c 616e  p install pjplan
+000003a0: 0a94 6807 5d94 6816 8c13 7069 7020 696e  ..h.].h...pip in
+000003b0: 7374 616c 6c20 706a 706c 616e 0a94 8594  stall pjplan....
+000003c0: 8194 7d94 681b 6860 7362 6168 1f7d 9428  ..}.h.h`sbah.}.(
+000003d0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000003e0: 6829 5d94 8c08 6c61 6e67 7561 6765 948c  h)]...language..
+000003f0: 0442 6173 6894 8c09 786d 6c3a 7370 6163  .Bash...xml:spac
+00000400: 6594 8c08 7072 6573 6572 7665 9475 682b  e...preserve.uh+
+00000410: 685e 681d 682c 681e 4b06 681b 680c 681c  h^h.h,h.K.h.h.h.
+00000420: 6803 7562 6568 1f7d 9428 6821 5d94 8c0c  h.ubeh.}.(h!]...
+00000430: 696e 7374 616c 6c61 7469 6f6e 9461 6823  installation.ah#
+00000440: 5d94 6825 5d94 8c0c 696e 7374 616c 6c61  ].h%]...installa
+00000450: 7469 6f6e 9461 6827 5d94 6829 5d94 7568  tion.ah'].h)].uh
+00000460: 2b68 0a68 1e4b 0168 1d68 2c68 1b68 0368  +h.h.K.h.h,h.h.h
+00000470: 1c68 0375 6261 681f 7d94 2868 215d 9468  .h.ubah.}.(h!].h
+00000480: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00000490: 0673 6f75 7263 6594 682c 7568 2b68 018c  .source.h,uh+h..
+000004a0: 0e63 7572 7265 6e74 5f73 6f75 7263 6594  .current_source.
+000004b0: 4e8c 0c63 7572 7265 6e74 5f6c 696e 6594  N..current_line.
+000004c0: 4e8c 0873 6574 7469 6e67 7394 8c11 646f  N..settings...do
+000004d0: 6375 7469 6c73 2e66 726f 6e74 656e 6494  cutils.frontend.
+000004e0: 8c06 5661 6c75 6573 9493 9429 8194 7d94  ..Values...)..}.
+000004f0: 2868 0f4e 8c09 6765 6e65 7261 746f 7294  (h.N..generator.
+00000500: 4e8c 0964 6174 6573 7461 6d70 944e 8c0b  N..datestamp.N..
+00000510: 736f 7572 6365 5f6c 696e 6b94 4e8c 0a73  source_link.N..s
+00000520: 6f75 7263 655f 7572 6c94 4e8c 0d74 6f63  ource_url.N..toc
+00000530: 5f62 6163 6b6c 696e 6b73 948c 0565 6e74  _backlinks...ent
+00000540: 7279 948c 1266 6f6f 746e 6f74 655f 6261  ry...footnote_ba
+00000550: 636b 6c69 6e6b 7394 4b01 8c0d 7365 6374  cklinks.K...sect
+00000560: 6e75 6d5f 7866 6f72 6d94 4b01 8c0e 7374  num_xform.K...st
+00000570: 7269 705f 636f 6d6d 656e 7473 944e 8c1b  rip_comments.N..
+00000580: 7374 7269 705f 656c 656d 656e 7473 5f77  strip_elements_w
+00000590: 6974 685f 636c 6173 7365 7394 4e8c 0d73  ith_classes.N..s
+000005a0: 7472 6970 5f63 6c61 7373 6573 944e 8c0c  trip_classes.N..
+000005b0: 7265 706f 7274 5f6c 6576 656c 944b 028c  report_level.K..
+000005c0: 0a68 616c 745f 6c65 7665 6c94 4b05 8c11  .halt_level.K...
+000005d0: 6578 6974 5f73 7461 7475 735f 6c65 7665  exit_status_leve
+000005e0: 6c94 4b05 8c05 6465 6275 6794 4e8c 0e77  l.K...debug.N..w
+000005f0: 6172 6e69 6e67 5f73 7472 6561 6d94 4e8c  arning_stream.N.
+00000600: 0974 7261 6365 6261 636b 9488 8c0e 696e  .traceback....in
+00000610: 7075 745f 656e 636f 6469 6e67 948c 0975  put_encoding...u
+00000620: 7466 2d38 2d73 6967 948c 1c69 6e70 7574  tf-8-sig...input
+00000630: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
+00000640: 6861 6e64 6c65 7294 8c06 7374 7269 6374  handler...strict
+00000650: 948c 0f6f 7574 7075 745f 656e 636f 6469  ...output_encodi
+00000660: 6e67 948c 0575 7466 2d38 948c 1d6f 7574  ng...utf-8...out
+00000670: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
+00000680: 6f72 5f68 616e 646c 6572 9468 9d8c 0e65  or_handler.h...e
+00000690: 7272 6f72 5f65 6e63 6f64 696e 6794 8c05  rror_encoding...
+000006a0: 7574 662d 3894 8c1c 6572 726f 725f 656e  utf-8...error_en
+000006b0: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
+000006c0: 646c 6572 948c 1062 6163 6b73 6c61 7368  dler...backslash
+000006d0: 7265 706c 6163 6594 8c0d 6c61 6e67 7561  replace...langua
+000006e0: 6765 5f63 6f64 6594 8c02 656e 948c 1372  ge_code...en...r
+000006f0: 6563 6f72 645f 6465 7065 6e64 656e 6369  ecord_dependenci
+00000700: 6573 944e 8c06 636f 6e66 6967 944e 8c09  es.N..config.N..
+00000710: 6964 5f70 7265 6669 7894 6806 8c0e 6175  id_prefix.h...au
+00000720: 746f 5f69 645f 7072 6566 6978 948c 0269  to_id_prefix...i
+00000730: 6494 8c0d 6475 6d70 5f73 6574 7469 6e67  d...dump_setting
+00000740: 7394 4e8c 0e64 756d 705f 696e 7465 726e  s.N..dump_intern
+00000750: 616c 7394 4e8c 0f64 756d 705f 7472 616e  als.N..dump_tran
+00000760: 7366 6f72 6d73 944e 8c0f 6475 6d70 5f70  sforms.N..dump_p
+00000770: 7365 7564 6f5f 786d 6c94 4e8c 1065 7870  seudo_xml.N..exp
+00000780: 6f73 655f 696e 7465 726e 616c 7394 4e8c  ose_internals.N.
+00000790: 0e73 7472 6963 745f 7669 7369 746f 7294  .strict_visitor.
+000007a0: 4e8c 0f5f 6469 7361 626c 655f 636f 6e66  N.._disable_conf
+000007b0: 6967 944e 8c07 5f73 6f75 7263 6594 682c  ig.N.._source.h,
+000007c0: 8c0c 5f64 6573 7469 6e61 7469 6f6e 944e  .._destination.N
+000007d0: 8c0d 5f63 6f6e 6669 675f 6669 6c65 7394  .._config_files.
+000007e0: 5d94 8c16 6669 6c65 5f69 6e73 6572 7469  ]...file_inserti
+000007f0: 6f6e 5f65 6e61 626c 6564 9488 8c0b 7261  on_enabled....ra
+00000800: 775f 656e 6162 6c65 6494 4b01 8c11 6c69  w_enabled.K...li
+00000810: 6e65 5f6c 656e 6774 685f 6c69 6d69 7494  ne_length_limit.
+00000820: 4a00 e1f5 058c 0e70 6570 5f72 6566 6572  J......pep_refer
+00000830: 656e 6365 7394 4e8c 0c70 6570 5f62 6173  ences.N..pep_bas
+00000840: 655f 7572 6c94 8c18 6874 7470 733a 2f2f  e_url...https://
+00000850: 7065 7073 2e70 7974 686f 6e2e 6f72 672f  peps.python.org/
+00000860: 948c 1570 6570 5f66 696c 655f 7572 6c5f  ...pep_file_url_
+00000870: 7465 6d70 6c61 7465 948c 0870 6570 2d25  template...pep-%
+00000880: 3034 6494 8c0e 7266 635f 7265 6665 7265  04d...rfc_refere
+00000890: 6e63 6573 944e 8c0c 7266 635f 6261 7365  nces.N..rfc_base
+000008a0: 5f75 726c 948c 2668 7474 7073 3a2f 2f64  _url..&https://d
+000008b0: 6174 6174 7261 636b 6572 2e69 6574 662e  atatracker.ietf.
+000008c0: 6f72 672f 646f 632f 6874 6d6c 2f94 8c09  org/doc/html/...
+000008d0: 7461 625f 7769 6474 6894 4b08 8c1d 7472  tab_width.K...tr
+000008e0: 696d 5f66 6f6f 746e 6f74 655f 7265 6665  im_footnote_refe
+000008f0: 7265 6e63 655f 7370 6163 6594 898c 1073  rence_space....s
+00000900: 796e 7461 785f 6869 6768 6c69 6768 7494  yntax_highlight.
+00000910: 8c04 6c6f 6e67 948c 0c73 6d61 7274 5f71  ..long...smart_q
+00000920: 756f 7465 7394 888c 1373 6d61 7274 7175  uotes....smartqu
+00000930: 6f74 6573 5f6c 6f63 616c 6573 945d 948c  otes_locales.]..
+00000940: 1d63 6861 7261 6374 6572 5f6c 6576 656c  .character_level
+00000950: 5f69 6e6c 696e 655f 6d61 726b 7570 9489  _inline_markup..
+00000960: 8c0e 646f 6374 6974 6c65 5f78 666f 726d  ..doctitle_xform
+00000970: 9489 8c0d 646f 6369 6e66 6f5f 7866 6f72  ....docinfo_xfor
+00000980: 6d94 4b01 8c12 7365 6374 7375 6274 6974  m.K...sectsubtit
+00000990: 6c65 5f78 666f 726d 9489 8c0d 696d 6167  le_xform....imag
+000009a0: 655f 6c6f 6164 696e 6794 8c04 6c69 6e6b  e_loading...link
+000009b0: 948c 1065 6d62 6564 5f73 7479 6c65 7368  ...embed_stylesh
+000009c0: 6565 7494 898c 1563 6c6f 616b 5f65 6d61  eet....cloak_ema
+000009d0: 696c 5f61 6464 7265 7373 6573 9488 8c11  il_addresses....
+000009e0: 7365 6374 696f 6e5f 7365 6c66 5f6c 696e  section_self_lin
+000009f0: 6b94 898c 0365 6e76 944e 7562 8c08 7265  k....env.Nub..re
+00000a00: 706f 7274 6572 944e 8c10 696e 6469 7265  porter.N..indire
+00000a10: 6374 5f74 6172 6765 7473 945d 948c 1173  ct_targets.]...s
+00000a20: 7562 7374 6974 7574 696f 6e5f 6465 6673  ubstitution_defs
+00000a30: 947d 9428 8c0f 776f 7264 636f 756e 742d  .}.(..wordcount-
+00000a40: 776f 7264 7394 6809 8c17 7375 6273 7469  words.h...substi
+00000a50: 7475 7469 6f6e 5f64 6566 696e 6974 696f  tution_definitio
+00000a60: 6e94 9394 2981 947d 9428 6805 8c02 3132  n...)..}.(h...12
+00000a70: 9468 075d 9468 168c 0231 3294 8594 8194  .h.].h...12.....
+00000a80: 7d94 681b 68db 7362 6168 1f7d 9428 6821  }.h.h.sbah.}.(h!
+00000a90: 5d94 6823 5d94 6825 5d94 8c0f 776f 7264  ].h#].h%]...word
+00000aa0: 636f 756e 742d 776f 7264 7394 6168 275d  count-words.ah']
+00000ab0: 9468 295d 9475 682b 68d9 681d 682c 7562  .h)].uh+h.h.h,ub
+00000ac0: 8c11 776f 7264 636f 756e 742d 6d69 6e75  ..wordcount-minu
+00000ad0: 7465 7394 68da 2981 947d 9428 6805 8c01  tes.h.)..}.(h...
+00000ae0: 3094 6807 5d94 6816 8c01 3094 8594 8194  0.h.].h...0.....
+00000af0: 7d94 681b 68eb 7362 6168 1f7d 9428 6821  }.h.h.sbah.}.(h!
+00000b00: 5d94 6823 5d94 6825 5d94 8c11 776f 7264  ].h#].h%]...word
+00000b10: 636f 756e 742d 6d69 6e75 7465 7394 6168  count-minutes.ah
+00000b20: 275d 9468 295d 9475 682b 68d9 681d 682c  '].h)].uh+h.h.h,
+00000b30: 7562 758c 1273 7562 7374 6974 7574 696f  ubu..substitutio
+00000b40: 6e5f 6e61 6d65 7394 7d94 288c 0f77 6f72  n_names.}.(..wor
+00000b50: 6463 6f75 6e74 2d77 6f72 6473 9468 d88c  dcount-words.h..
+00000b60: 1177 6f72 6463 6f75 6e74 2d6d 696e 7574  .wordcount-minut
+00000b70: 6573 9468 ea75 8c08 7265 666e 616d 6573  es.h.u..refnames
+00000b80: 947d 948c 0672 6566 6964 7394 7d94 8c07  .}...refids.}...
+00000b90: 6e61 6d65 6964 7394 7d94 6877 6874 738c  nameids.}.hwhts.
+00000ba0: 096e 616d 6574 7970 6573 947d 9468 7789  .nametypes.}.hw.
+00000bb0: 7368 217d 9468 7468 0c73 8c0d 666f 6f74  sh!}.hth.s..foot
+00000bc0: 6e6f 7465 5f72 6566 7394 7d94 8c0d 6369  note_refs.}...ci
+00000bd0: 7461 7469 6f6e 5f72 6566 7394 7d94 8c0d  tation_refs.}...
+00000be0: 6175 746f 666f 6f74 6e6f 7465 7394 5d94  autofootnotes.].
+00000bf0: 8c11 6175 746f 666f 6f74 6e6f 7465 5f72  ..autofootnote_r
+00000c00: 6566 7394 5d94 8c10 7379 6d62 6f6c 5f66  efs.]...symbol_f
+00000c10: 6f6f 746e 6f74 6573 945d 948c 1473 796d  ootnotes.]...sym
+00000c20: 626f 6c5f 666f 6f74 6e6f 7465 5f72 6566  bol_footnote_ref
+00000c30: 7394 5d94 8c09 666f 6f74 6e6f 7465 7394  s.]...footnotes.
+00000c40: 5d94 8c09 6369 7461 7469 6f6e 7394 5d94  ]...citations.].
+00000c50: 8c12 6175 746f 666f 6f74 6e6f 7465 5f73  ..autofootnote_s
+00000c60: 7461 7274 944b 018c 1573 796d 626f 6c5f  tart.K...symbol_
+00000c70: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
+00000c80: 008c 0a69 645f 636f 756e 7465 7294 8c0b  ...id_counter...
+00000c90: 636f 6c6c 6563 7469 6f6e 7394 8c07 436f  collections...Co
+00000ca0: 756e 7465 7294 9394 7d94 8594 5294 8c0e  unter...}...R...
+00000cb0: 7061 7273 655f 6d65 7373 6167 6573 945d  parse_messages.]
+00000cc0: 948c 1274 7261 6e73 666f 726d 5f6d 6573  ...transform_mes
+00000cd0: 7361 6765 7394 5d94 8c0b 7472 616e 7366  sages.]...transf
+00000ce0: 6f72 6d65 7294 4e8c 0b69 6e63 6c75 6465  ormer.N..include
+00000cf0: 5f6c 6f67 945d 948c 0a64 6563 6f72 6174  _log.]...decorat
+00000d00: 696f 6e94 4e68 1c68 038c 0a6d 7973 745f  ion.Nh.h...myst_
+00000d10: 736c 7567 7394 7d94 7562 2e              slugs.}.ub.
```

### Comparing `pjplan-0.0.8/docs/_build/html/index.html` & `pjplan-0.0.9/docs/_build/html/ttt/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -2,98 +2,87 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Welcome to pjplan’s documentation! &#8212; pjplan 0.0.3 documentation</title>
-    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
-    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
-    <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="src" href="modules.html" />
+    <title>Welcome to ttt’s documentation! &#8212; pjplan 0.0.8 documentation</title>
+    <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="../_static/alabaster.css" />
+    <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
+    <script src="../_static/doctools.js"></script>
+    <script src="../_static/sphinx_highlight.js"></script>
+    <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
+    <link rel="index" title="Index" href="../genindex.html" />
+    <link rel="search" title="Search" href="../search.html" />
    
-  <link rel="stylesheet" href="_static/custom.css" type="text/css" />
+  <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   
   
   <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
 
   </head><body>
   
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
-  <section id="welcome-to-pjplan-s-documentation">
-<h1>Welcome to pjplan’s documentation!<a class="headerlink" href="#welcome-to-pjplan-s-documentation" title="Permalink to this heading">¶</a></h1>
+  <section id="welcome-to-ttt-s-documentation">
+<h1>Welcome to ttt’s documentation!<a class="headerlink" href="#welcome-to-ttt-s-documentation" title="Permalink to this heading">¶</a></h1>
 <div class="toctree-wrapper compound">
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="modules.html">src</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="pjplan.html">pjplan package</a></li>
-</ul>
-</li>
-</ul>
 </div>
 </section>
 <section id="indices-and-tables">
 <h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading">¶</a></h1>
 <ul class="simple">
-<li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
-<li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
-<li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
+<li><p><a class="reference internal" href="../genindex.html"><span class="std std-ref">Index</span></a></p></li>
+<li><p><a class="reference internal" href="../py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
+<li><p><a class="reference internal" href="../search.html"><span class="std std-ref">Search Page</span></a></p></li>
 </ul>
-<table class="autosummary longtable docutils align-default">
-<tbody>
-</tbody>
-</table>
 </section>
 
 
           </div>
           
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="#">pjplan</a></h1>
+<h1 class="logo"><a href="../index.html">pjplan</a></h1>
 
 
 
 
 
 
 
 
 <h3>Navigation</h3>
 <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="modules.html">src</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../en/index.html">Englist</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../ru/index.html">Русский</a></li>
 </ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
-  <li><a href="#">Documentation overview</a><ul>
-      <li>Next: <a href="modules.html" title="next chapter">src</a></li>
+  <li><a href="../index.html">Documentation overview</a><ul>
   </ul></li>
 </ul>
 </div>
 <div id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
+    <form class="search" action="../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
@@ -112,15 +101,15 @@
       &copy;2023, Artem Snopkov.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
-      <a href="_sources/index.rst.txt"
+      <a href="../_sources/ttt/index.rst.txt"
           rel="nofollow">Page source</a>
     </div>
 
     
 
     
   </body>
```

#### html2text {}

```diff
@@ -1,28 +1,24 @@
 
 
 
 
 
 
 
-
-****** Welcome to pjplanâs documentation!Â¶ ******
-Contents:
-    * src
-          o pjplan_package
+****** Welcome to tttâs documentation!Â¶ ******
 
 ****** Indices and tablesÂ¶ ******
     * Index
     * Module_Index
     * Search_Page
 ****** pjplan ******
 **** Navigation ****
 Contents:
-    * src
+    * Englist
+    * Ð ÑÑÑÐºÐ¸Ð¹
 **** Related Topics ****
     * Documentation_overview
-          o Next: src
 **** Quick search ****
 [q                   ] [Go]
 ©2023, Artem Snopkov. | Powered by Sphinx_6.1.3 & Alabaster_0.7.13 | Page
 source
```

### Comparing `pjplan-0.0.8/docs/_build/html/search.html` & `pjplan-0.0.9/docs/_build/html/search.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; pjplan 0.0.3 documentation</title>
+    <title>Search &#8212; pjplan 0.0.8 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
   
    
@@ -68,44 +69,29 @@
 
           </div>
           
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="index.html">pjplan</a></h1>
-
-
-
-
-
-
-
-
-<h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+  <div>
+    <h3><a href="index.html">Table of Contents</a></h3>
+    <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="modules.html">src</a></li>
+<li class="toctree-l1"><a class="reference internal" href="en/index.html">Englist</a></li>
+<li class="toctree-l1"><a class="reference internal" href="ru/index.html">Русский</a></li>
 </ul>
 
-<div class="relations">
+  </div><div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
   </ul></li>
 </ul>
 </div>
-
-
-
-
-
-
-
-
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2023, Artem Snopkov.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -5,14 +5,14 @@
 
 
 
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
-****** pjplan ******
-**** Navigation ****
+**** Table_of_Contents ****
 Contents:
-    * src
+    * Englist
+    * Ð ÑÑÑÐºÐ¸Ð¹
 **** Related Topics ****
     * Documentation_overview
 ©2023, Artem Snopkov. | Powered by Sphinx_6.1.3 & Alabaster_0.7.13
```

### Comparing `pjplan-0.0.8/docs/_build/html/_static/alabaster.css` & `pjplan-0.0.9/docs/_build/html/_static/alabaster.css`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     color: #000;
     margin: 0;
     padding: 0;
 }
 
 
 div.document {
-    width: 940px;
+    width: 1200px;
     margin: 30px auto 0 auto;
 }
 
 div.documentwrapper {
     float: left;
     width: 100%;
 }
@@ -43,15 +43,15 @@
 }
 
 div.body > .section {
     text-align: left;
 }
 
 div.footer {
-    width: 940px;
+    width: 1200px;
     margin: 20px auto 30px auto;
     font-size: 14px;
     color: #888;
     text-align: right;
 }
 
 div.footer a {
```

### Comparing `pjplan-0.0.8/docs/_build/html/_static/basic.css` & `pjplan-0.0.9/docs/_build/html/_static/basic.css`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     padding: 2px;
     border-collapse: collapse;
 }
 
 /* -- general body styles --------------------------------------------------- */
 
 div.body {
-    min-width: 360px;
+    min-width: 1000px;
     max-width: 800px;
 }
 
 div.body p, div.body dd, div.body li, div.body blockquote {
     -moz-hyphens: auto;
     -ms-hyphens: auto;
     -webkit-hyphens: auto;
```

### Comparing `pjplan-0.0.8/docs/_build/html/_static/doctools.js` & `pjplan-0.0.9/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/_build/html/_static/language_data.js` & `pjplan-0.0.9/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/_build/html/_static/pygments.css` & `pjplan-0.0.9/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/_build/html/_static/searchtools.js` & `pjplan-0.0.9/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/_build/html/_static/sphinx_highlight.js` & `pjplan-0.0.9/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/_static/img/readme/mermaid_gantt.png` & `pjplan-0.0.9/docs/_build/html/_static/img/readme/mermaid_gantt.png`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/docs/_static/img/readme/mermaid_network.png` & `pjplan-0.0.9/docs/_build/html/_static/img/readme/mermaid_network.png`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/calendar/calendar.ipynb` & `pjplan-0.0.9/examples/jupyter/calendar/calendar.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb` & `pjplan-0.0.9/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/critical-path/critical-path.ipynb` & `pjplan-0.0.9/examples/jupyter/critical-path/critical-path.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb` & `pjplan-0.0.9/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb` & `pjplan-0.0.9/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/forward-scheduler/forward-scheduler.ipynb` & `pjplan-0.0.9/examples/jupyter/forward-scheduler/forward-scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/getting-started/getting-started.ipynb` & `pjplan-0.0.9/examples/jupyter/getting-started/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/getting-started/gs.html` & `pjplan-0.0.9/examples/jupyter/getting-started/gs.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb` & `pjplan-0.0.9/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb` & `pjplan-0.0.9/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/mermaid-network/mermaid-network.ipynb` & `pjplan-0.0.9/examples/jupyter/mermaid-network/mermaid-network.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/pandas/pandas.ipynb` & `pjplan-0.0.9/examples/jupyter/pandas/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/jupyter/print/print.ipynb` & `pjplan-0.0.9/examples/jupyter/print/print.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/streamlit/dhtmlx-gantt/main.py` & `pjplan-0.0.9/examples/streamlit/dhtmlx-gantt/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 
 import streamlit as st
 import streamlit.components.v1 as components
 
 sys.path.append('../../src')
 
-from pjplan import Task, DefaultScheduler, WBS, DhtmlxGantt, DhtmlxGanttColumn
+from pjplan import Task, ForwardScheduler, WBS, DhtmlxGantt, DhtmlxGanttColumn
 
 
 def page(project: WBS):
     st.set_page_config(
         layout="wide",
         page_title='Диаграмма Ганта',
     )
@@ -39,24 +39,27 @@
             DhtmlxGanttColumn('name', 200),
             DhtmlxGanttColumn('start', 100),
             DhtmlxGanttColumn('end', 100, label='End date'),
             DhtmlxGanttColumn('progress', 100),
         ]
     )
 
-    components.html(gantt.to_html(), height=500)
+    with open("g.html", 'w') as f:
+        f.write(gantt.to_html())
+
+    components.html(gantt.to_html(), height=900)
 
 
 if __name__ == '__main__':
     with WBS() as prj:
         prj // Task(2, 'Задача 1', estimate=40, spent=20, resource='Tester')
         prj // Task(3, 'Задача 2', predecessors=[prj[2]], estimate=20, resource='Tester')
         with prj // Task(4, 'Задача 4') as t:
             t // Task(5, 'Задача 5', predecessors=[prj[3]], estimate=100)
             t // Task(6, 'Задача 6', predecessors=[prj[3]], estimate=50)
         with prj // Task(7, 'Задача 7') as t:
             t // Task(8, 'Задача 8', predecessors=[prj[6]], estimate=16)
             t // Task(9, 'Задача 9', predecessors=[prj[6]], estimate=16)
 
-    plan, usage = DefaultScheduler(datetime.now()).calc(prj)
+    plan = ForwardScheduler(datetime.now()).calc(prj)
 
-    page(plan)
+    page(plan.schedule)
```

### Comparing `pjplan-0.0.8/examples/streamlit/mermaid-gantt/main.py` & `pjplan-0.0.9/examples/streamlit/mermaid-gantt/main.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/examples/streamlit/mermaid-network/main.py` & `pjplan-0.0.9/examples/streamlit/mermaid-network/main.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/__init__.py` & `pjplan-0.0.9/src/pjplan/__init__.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/calendar.py` & `pjplan-0.0.9/src/pjplan/calendar.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/resource.py` & `pjplan-0.0.9/src/pjplan/resource.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/schedule.py` & `pjplan-0.0.9/src/pjplan/schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import dataclasses
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from typing import List, Set
+from typing import List, Set, Callable
 
 from pjplan import Task, WBS, IResource, Resource
 from pjplan.utils import TextTable, GREEN, YELLOW, GREY, RED
 
 
 def _validate_graph_isolation(project: WBS):
     all_tasks = {task.id: task for task in project.tasks}
@@ -52,57 +53,48 @@
     """Date"""
     task: Task
     """Task"""
     units: float
     """Units of resource reserved for this resource, task and date"""
 
 
-class ResourceUsage:
+class ResourceUsageReport:
     """Resource usage report"""
 
-    def __init__(self):
-        self.__items: List[ResourceUsageRow] = []
+    def __init__(self, rows: List[ResourceUsageRow]):
+        self.__rows = rows
 
-    @staticmethod
-    def __get_key(date: datetime):
-        return datetime(date.year, date.month, date.day, 0, 0, 0, 0)
+    def rows(self, _filter: Callable[[ResourceUsageRow], bool] = None) -> List[ResourceUsageRow]:
+        return [dataclasses.replace(r)
+                for r in self.__rows
+                if _filter is None or _filter(r)]
+
+    def reserved(self, resource: IResource, date: datetime) -> float:
+        units = [item.units
+                 for item in self.__rows
+                 if item.resource == resource and item.date == date]
 
-    def reserve(self, resource: IResource, date: datetime, task: Task, units: float) -> float:
-        self.__items.append(ResourceUsageRow(resource, self.__get_key(date), task, units))
-        return units
-
-    def reserved(self, resource: IResource, date: datetime, task: Task = None) -> float:
-        if task is None:
-            rows = [item.units for item in self.__items if
-                    item.resource == resource and item.date == self.__get_key(date)]
-        else:
-            rows = [item.units for item in self.__items if
-                    item.resource == resource and item.date == self.__get_key(date) and item.task == task]
-        if len(rows) == 0:
-            return 0
-        return sum(rows)
-
-    def rows(self) -> List[ResourceUsageRow]:
-        return self.__items
+        return sum(units, 0)
 
     def __repr__(self):
-        if len(self.__items) == 0:
+        if len(self.__rows) == 0:
             return "Empty"
 
-        dates = [item.date for item in self.__items]
+        dates = [item.date for item in self.__rows]
         min_date = min(dates)
         max_date = max(dates)
 
-        resources = set([item.resource for item in self.__items])
+        resources = set([item.resource for item in self.__rows])
 
         table = TextTable()
         table.new_row()
         table.new_cell('DATE', RED)
         for k in resources:
-            table.new_cell(k.name.upper(), RED)
+            name = k.name if k.name is not None else 'none'
+            table.new_cell(name.upper(), RED)
 
         d = min_date
         while d <= max_date:
             table.new_row()
             table.new_cell(d.strftime('%y-%m-%d'))
             for k in resources:
                 val = self.reserved(k, d)
@@ -114,20 +106,48 @@
                     color = YELLOW
                 table.new_cell(f"{val:.1f}", color)
             d += timedelta(days=1)
 
         return table.text_repr(True)
 
 
+class _ResourceUsage:
+
+    def __init__(self):
+        self.rows: List[ResourceUsageRow] = []
+
+    @staticmethod
+    def __get_key(date: datetime):
+        return datetime(date.year, date.month, date.day, 0, 0, 0, 0)
+
+    def reserve(self, resource: IResource, date: datetime, task: Task, units: float) -> float:
+        self.rows.append(ResourceUsageRow(resource, self.__get_key(date), task, units))
+        return units
+
+    def reserved(self, resource: IResource, date: datetime, task: Task = None) -> float:
+        if task is None:
+            units = [item.units
+                     for item in self.rows
+                     if item.resource == resource and item.date == self.__get_key(date)]
+        else:
+            units = [item.units
+                     for item in self.rows
+                     if item.resource == resource and item.date == self.__get_key(date) and item.task == task]
+
+        return sum(units, 0)
+
+
 @dataclass(frozen=True)
 class Schedule:
     """WBS schedule result"""
     schedule: WBS
     """Clone of original WBS with calculated start and end dates on each task"""
-    resource_usage: ResourceUsage
+    resources: List[IResource]
+    """List of resources"""
+    resource_usage: ResourceUsageReport
     """Resource usage report"""
 
 
 class IScheduler(ABC):
     """WBS schedule calculator"""
 
     @abstractmethod
@@ -154,15 +174,15 @@
         self.__resources = {} if resources is None else {r.name: r for r in resources}
         self.__balance_resources = balance_resources
         self.__default_estimate = default_estimate
 
     def __get_resource_nearest_available_date(
             self,
             resource: IResource,
-            resource_usage: ResourceUsage,
+            resource_usage: _ResourceUsage,
             start_date: datetime,
             task: Task,
             max_steps: int = 1000
     ) -> datetime:
         d = resource.get_nearest_availability_date(start_date, 1)
 
         for i in range(0, max_steps):
@@ -180,15 +200,15 @@
             "Can't find nearest availability time for resource", resource.name,
             "after", start_date.strftime('%Y-%m-%d')
         )
 
     def __shift_by_resource_usage_and_calendar(
             self,
             resource: IResource,
-            resource_usage: ResourceUsage,
+            resource_usage: _ResourceUsage,
             start_date: datetime,
             task: Task,
             left_hours: float,
             max_steps: int = 1000
     ) -> datetime:
         if left_hours == 0:
             return start_date
@@ -213,15 +233,15 @@
         percent = reserved / resource.get_available_units(date)
         return date + timedelta(hours=24 * percent)
 
     def __forward_pass(
             self,
             _task: Task,
             min_date: datetime,
-            resource_usage: ResourceUsage,
+            resource_usage: _ResourceUsage,
             calculated: List[int]
     ):
         if _task.id in calculated:
             return
 
         for pred in _task.predecessors:
             self.__forward_pass(pred, min_date, resource_usage, calculated)
@@ -283,20 +303,24 @@
         _validate_graph_isolation(wbs)
         _check_loops(wbs)
         self.__check_no_end_dates_in_future(wbs)
 
         forward = wbs.clone()
         self.__prepare_tasks(forward)
 
-        forward_resource_usage = ResourceUsage()
+        forward_resource_usage = _ResourceUsage()
         calculated = []
         for t in forward.roots:
             self.__forward_pass(t, self.__start, forward_resource_usage, calculated)
 
-        return Schedule(forward, forward_resource_usage)
+        return Schedule(
+            forward,
+            list(self.__resources.values()),
+            ResourceUsageReport(forward_resource_usage.rows)
+        )
 
     @staticmethod
     def __check_no_end_dates_in_future(project: WBS):
         now = datetime.now()
         for t in project.tasks:
             if t.end is not None and t.end > now:
                 raise RuntimeError(f"Task {t.id} has end date in future. Can't schedule this task.")
@@ -320,15 +344,15 @@
         self.__resources = {} if resources is None else {r.name: r for r in resources}
         self.__balance_resources = balance_resources
         self.__default_estimate = default_estimate
 
     def __get_resource_nearest_available_date(
             self,
             resource: IResource,
-            resource_usage: ResourceUsage,
+            resource_usage: _ResourceUsage,
             start_date: datetime,
             task: Task,
             max_steps: int = 1000
     ) -> datetime:
         d = resource.get_nearest_availability_date(start_date, -1) - timedelta(days=1)
 
         for i in range(0, max_steps):
@@ -346,15 +370,15 @@
             "Can't find nearest availability time for resource", resource.name,
             "after", start_date.strftime('%Y-%m-%d')
         )
 
     def __shift_by_resource_usage_and_calendar(
             self,
             resource: IResource,
-            resource_usage: ResourceUsage,
+            resource_usage: _ResourceUsage,
             start_date: datetime,
             task: Task,
             left_hours: float,
             max_steps: int = 1000
     ) -> datetime:
         if left_hours == 0:
             return start_date
@@ -380,15 +404,15 @@
 
         return date + timedelta(days=1) - timedelta(hours=24 * percent)
 
     def __backward_pass(
             self,
             _task: Task,
             min_date: datetime,
-            resource_usage: ResourceUsage,
+            resource_usage: _ResourceUsage,
             calculated: List[int]
     ):
         if _task.id in calculated:
             return
 
         for pred in _task.successors:
             self.__backward_pass(pred, min_date, resource_usage, calculated)
@@ -454,15 +478,19 @@
     def calc(self, project: WBS) -> Schedule:
         _validate_graph_isolation(project)
         _check_loops(project)
 
         backward = project.clone()
         self.__prepare_tasks(backward)
 
-        backward_resource_usage = ResourceUsage()
+        backward_resource_usage = _ResourceUsage()
         backward_roots = backward.roots
 
         calculated = []
         for i in range(len(backward_roots) - 1, -1, -1):
             self.__backward_pass(backward_roots[i], self.__end, backward_resource_usage, calculated)
 
-        return Schedule(backward, backward_resource_usage)
+        return Schedule(
+            backward,
+            list(self.__resources.values()),
+            ResourceUsageReport(backward_resource_usage.rows)
+        )
```

### Comparing `pjplan-0.0.8/src/pjplan/task.py` & `pjplan-0.0.9/src/pjplan/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,41 +231,61 @@
         def search(t, **kw):
             for k, v in kw.items():
                 if k.endswith("_like_"):
                     k = k[0:-6]
                     val = self.__get_task_attribute(t, k)
                     if val is None or not re.search(v, val):
                         return False
+                elif k.endswith("_not_like_"):
+                    k = k[0:-10]
+                    val = self.__get_task_attribute(t, k)
+                    if val is None or re.search(v, val):
+                        return False
                 elif k.endswith("_not_in_"):
                     k = k[0:-8]
                     if self.__get_task_attribute(t, k) in v:
                         return False
+                elif k.endswith("_is_none_"):
+                    k = k[0:-9]
+                    val = self.__get_task_attribute(t, k)
+                    if val is not None:
+                        return False
+                elif k.endswith("_is_not_none_"):
+                    k = k[0:-13]
+                    val = self.__get_task_attribute(t, k)
+                    if val is None:
+                        return False
                 elif k.endswith("_in_"):
                     k = k[0:-4]
                     if not self.__get_task_attribute(t, k) in v:
                         return False
                 elif k.endswith("_ne_"):
                     k = k[0:-4]
-                    if not self.__get_task_attribute(t, k) != v:
+                    val = self.__get_task_attribute(t, k)
+                    if val is None or not val != v:
                         return False
                 elif k.endswith("_le_"):
                     k = k[0:-4]
-                    if not self.__get_task_attribute(t, k) <= v:
+                    val = self.__get_task_attribute(t, k)
+                    if val is None or not val <= v:
                         return False
                 elif k.endswith("_lt_"):
                     k = k[0:-4]
-                    if not self.__get_task_attribute(t, k) < v:
+                    val = self.__get_task_attribute(t, k)
+                    if val is None or not val < v:
                         return False
                 elif k.endswith("_ge_"):
                     k = k[0:-4]
-                    if not self.__get_task_attribute(t, k) >= v:
+                    val = self.__get_task_attribute(t, k)
+                    if val is None or not val >= v:
                         return False
                 elif k.endswith("_gt_"):
                     k = k[0:-4]
-                    if not self.__get_task_attribute(t, k) > v:
+                    val = self.__get_task_attribute(t, k)
+                    if val is None or not val > v:
                         return False
                 elif self.__get_task_attribute(t, k) != v:
                     return False
             return True
 
         return _ImmutableTaskList([t for t in self if search(t, **kwargs)])
 
@@ -588,20 +608,20 @@
             predecessors: List['Task'] = None,
             successors: List['Task'] = None,
             **kwargs
     ):
         """
         :param id: task id, unique in task graph
         :param name: task name
-        :param resource: resource name (person, machine, etc.), necessary to perform task
+        :param resource: name of resource (person, machine, etc.), necessary to perform task
         :param start: task start date
         :param end: task end date
         :param milestone: is task milestone or not
-        :param estimate: task estimation in hours
-        :param spent: task completed work in hours
+        :param estimate: task estimation
+        :param spent: task completed work
         :param predecessors: predecessor tasks
         :param successors: successor tasks
         :param kwargs: additional task attributes
         """
         self.__id = id
         self.name = name
         self.resource = resource
```

### Comparing `pjplan-0.0.8/src/pjplan/utils.py` & `pjplan-0.0.9/src/pjplan/utils.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/wbs.py` & `pjplan-0.0.9/src/pjplan/wbs.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/alg/critical_path.py` & `pjplan-0.0.9/src/pjplan/alg/critical_path.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/io/csv_io.py` & `pjplan-0.0.9/src/pjplan/io/csv_io.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/io/raw.py` & `pjplan-0.0.9/src/pjplan/io/raw.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/viz/dhtmlx/gantt.py` & `pjplan-0.0.9/src/pjplan/viz/dhtmlx/gantt.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,21 +106,28 @@
 
                 res += '.' + css_class_name + ' .gantt_task_progress' + progress_css
 
             idx += 1
 
         return res, task_classes
 
-    def __data(self, task_classes: dict[int, str]):
+    def __resource_data(self):
+        resources = []
+        resources.append({"id": "Tester", "text": "QA"})
+        resources.append({"id": "Dev", "text": "Dev"})
+
+        return json.dumps(resources, ensure_ascii=False, indent=2)
+
+    def __gantt_data(self, task_classes: dict[int, str]):
 
         data = []
         links = []
 
         link_id = 0
-        for _root in self.wbs.tasks:
+        for _root in self.wbs.roots:
             for t in _root.all_children + [_root]:
 
                 progress = 0
                 if t.end < datetime.now():
                     progress = 1
                 elif t.estimate > 0:
                     progress = 1 - (max(t.estimate - t.spent, 0))/t.estimate
@@ -180,15 +187,16 @@
         return Template(template).substitute(
             readonly='true',
             row_height=self.__js(self.row_height),
             today_marker=self.__js(self.today_marker),
             columns=self.__columns(),
             scale=scale,
             task_classes_def=task_classes_def,
-            gantt_data=self.__data(task_classes)
+            gantt_data=self.__gantt_data(task_classes),
+            resource_data=self.__resource_data()
         )
 
     def _repr_html_(self):
         return ('<iframe srcdoc="{html}" width="100%" height="{height}" '
                 'style="border:none !important;" '
                 'allowfullscreen webkitallowfullscreen mozallowfullscreen>'
                 '</iframe>').format(html=escape(self.to_html()), height=self.height)
```

### Comparing `pjplan-0.0.8/src/pjplan/viz/dhtmlx/templates/gantt.html` & `pjplan-0.0.9/src/pjplan/viz/dhtmlx/templates/resource_usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             ],
             [
                 {unit: "month", format: "%M %Y", step: 1},
                 {
                     unit: "week", step: 1, format: function (date) {
                         var dateToStr = gantt.date.date_to_str("%d.%m");
                         var endDate = gantt.date.add(date, -6, "day");
-                        return dateToStr(date) + " - " + dateToStr(endDate);
+                        return dateToStr(endDate) + " - " + dateToStr(date);
                     }
                 }
             ],
             [
                 {unit: "month", format: "%M %y", step: 1},
                 {unit: "day", format: "%d", step: 1}
             ]
```

### Comparing `pjplan-0.0.8/src/pjplan/viz/mermaid/gantt.py` & `pjplan-0.0.9/src/pjplan/viz/mermaid/gantt.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/src/pjplan/viz/mermaid/network.py` & `pjplan-0.0.9/src/pjplan/viz/mermaid/network.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/tests/test_pjplan/test_calendar.py` & `pjplan-0.0.9/tests/test_pjplan/test_calendar.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/tests/test_pjplan/test_schedule.py` & `pjplan-0.0.9/tests/test_pjplan/test_schedule.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/tests/test_pjplan/test_task.py` & `pjplan-0.0.9/tests/test_pjplan/test_task.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/tests/test_pjplan/test_wbs.py` & `pjplan-0.0.9/tests/test_pjplan/test_wbs.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/tests/test_pjplan/test_io/test_csv_io.py` & `pjplan-0.0.9/tests/test_pjplan/test_io/test_csv_io.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/LICENSE` & `pjplan-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.8/README.md` & `pjplan-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pjplan: Python library for project schedule and analysis
+# pjplan: Python library for project planning and analysis
 
 ## What is it?
 
 **pjplan** turns your [Jupyter Notebook](https://jupyter.org/) into project management software. 
 This Python package gives you a simple API with following features:
 - Describe Work Burn-down Structure (WBS) of your project in code or load it from external source.
 - Manipulate tasks: link them as successors/predecessors, find, delete, reorder, etc. A lot of batch operations are supported via simple commands.
@@ -34,23 +34,24 @@
 ```bash
 pip install pjplan
 ```
 
 ## Getting started
 
 Let's define simple project WBS:
+
 ```python
 from pjplan import WBS, Task
 
 with WBS() as prj:
-  prj // Task(1, 'Task 1', estimate=40, resource='Developer')
-  prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource='Developer')
-  with prj // Task(3, 'Task 3') as t3:
-    t3 // Task(4, 'Task 4', predecessors=[prj[2]], estimate=100, resource='Tester')
-    t3 // Task(5, 'Task 5', predecessors=[prj[2]], estimate=50, resource='Tester')
+    prj // Task(1, 'Task 1', estimate=40, resource_name='Developer')
+    prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource_name='Developer')
+    with prj // Task(3, 'Task 3') as t3:
+        t3 // Task(4, 'Task 4', predecessors=[prj[2]], estimate=100, resource_name='Tester')
+        t3 // Task(5, 'Task 5', predecessors=[prj[2]], estimate=50, resource_name='Tester')
 ```
 
 Let's define resources:
 ```python
 from pjplan import Resource, WeeklyCalendar
 
 work_calendar = WeeklyCalendar(days=[0,1,2,3,4], units_per_day=8)
```

### Comparing `pjplan-0.0.8/pyproject.toml` & `pjplan-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pjplan"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Artem Snopkov", email="artem.snopkov@gmail.com" },
 ]
 description = "Python library for plan projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pjplan-0.0.8/PKG-INFO` & `pjplan-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pjplan
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for plan projects
 Project-URL: Homepage, https://github.com/artem-snopkov/pjplan
 Project-URL: Bug Tracker, https://github.com/artem-snopkov/pjplan/issues
 Author-email: Artem Snopkov <artem.snopkov@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# pjplan: Python library for project schedule and analysis
+# pjplan: Python library for project planning and analysis
 
 ## What is it?
 
 **pjplan** turns your [Jupyter Notebook](https://jupyter.org/) into project management software. 
 This Python package gives you a simple API with following features:
 - Describe Work Burn-down Structure (WBS) of your project in code or load it from external source.
 - Manipulate tasks: link them as successors/predecessors, find, delete, reorder, etc. A lot of batch operations are supported via simple commands.
@@ -48,23 +48,24 @@
 ```bash
 pip install pjplan
 ```
 
 ## Getting started
 
 Let's define simple project WBS:
+
 ```python
 from pjplan import WBS, Task
 
 with WBS() as prj:
-  prj // Task(1, 'Task 1', estimate=40, resource='Developer')
-  prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource='Developer')
-  with prj // Task(3, 'Task 3') as t3:
-    t3 // Task(4, 'Task 4', predecessors=[prj[2]], estimate=100, resource='Tester')
-    t3 // Task(5, 'Task 5', predecessors=[prj[2]], estimate=50, resource='Tester')
+    prj // Task(1, 'Task 1', estimate=40, resource_name='Developer')
+    prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource_name='Developer')
+    with prj // Task(3, 'Task 3') as t3:
+        t3 // Task(4, 'Task 4', predecessors=[prj[2]], estimate=100, resource_name='Tester')
+        t3 // Task(5, 'Task 5', predecessors=[prj[2]], estimate=50, resource_name='Tester')
 ```
 
 Let's define resources:
 ```python
 from pjplan import Resource, WeeklyCalendar
 
 work_calendar = WeeklyCalendar(days=[0,1,2,3,4], units_per_day=8)
```

