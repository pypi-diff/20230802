# Comparing `tmp/bowtie_json_schema-2023.7.9.tar.gz` & `tmp/bowtie_json_schema-2023.8.1.tar.gz`

## Comparing `bowtie_json_schema-2023.7.9.tar` & `bowtie_json_schema-2023.8.1.tar`

### file list

```diff
@@ -1,84 +1,83 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.flake8
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.readthedocs.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/test-requirements.in
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/SECURITY.md
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/release.yml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/build-frontend.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/deploy-frontend.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/documentation-links.yml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/images.yml
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/__main__.py
--rw-r--r--   0        0        0    31626 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/cli.rst
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/conf.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/requirements.in
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/requirements.txt
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/_static/dreamed.png
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/.eslintrc.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/index.html
--rw-r--r--   0        0        0   165159 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/package-lock.json
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/package.json
--rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/tsconfig.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/vite.config.js
--rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/public/favicon.ico
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/MainContainer.jsx
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/ReportDataHandler.jsx
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/ReportView.jsx
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/index.jsx
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/CopyToClipboard.jsx
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/LoadingAnimation.jsx
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/NavBar.jsx
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionItem.jsx
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionSvg.jsx
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/CasesSection.jsx
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/SchemaDisplay.jsx
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/DragAndDrop/DragAndDrop.jsx
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Modals/DetailsButtonModal.jsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Modals/RunTimeInfoModal.jsx
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/RunInfo/RunInfoSection.jsx
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.jsx
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummarySection.jsx
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummaryTable.jsx
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/context/BowtieVersionContext.jsx
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/context/ThemeContext.jsx
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/LICENSE
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/README.rst
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/pyproject.toml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/PKG-INFO
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/test-requirements.in
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/SECURITY.md
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/release.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/build-frontend.yml
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/deploy-frontend.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/documentation-links.yml
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/images.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/__main__.py
+-rw-r--r--   0        0        0    32694 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/cli.rst
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/conf.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/contributing.rst
+-rw-r--r--   0        0        0    34142 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/requirements.in
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/requirements.txt
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/_static/dreamed.png
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/.eslintrc.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/index.html
+-rw-r--r--   0        0        0   165159 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/package-lock.json
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/package.json
+-rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/tsconfig.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/vite.config.js
+-rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/public/favicon.ico
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/MainContainer.jsx
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/ReportDataHandler.jsx
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/ReportView.jsx
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/index.jsx
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/CopyToClipboard.jsx
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/LoadingAnimation.jsx
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/NavBar.jsx
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionItem.jsx
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionSvg.jsx
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/CasesSection.jsx
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/SchemaDisplay.jsx
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/DragAndDrop/DragAndDrop.jsx
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Modals/DetailsButtonModal.jsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Modals/RunTimeInfoModal.jsx
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/RunInfo/RunInfoSection.jsx
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.jsx
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummarySection.jsx
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummaryTable.jsx
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/context/BowtieVersionContext.jsx
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/context/ThemeContext.jsx
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/README.rst
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.7.9/.pre-commit-config.yaml` & `bowtie_json_schema-2023.8.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.9.0
+    rev: v3.10.1
     hooks:
       - id: pyupgrade
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.278"
+    rev: "v0.0.281"
     hooks:
       - id: ruff
   - repo: https://github.com/Riverside-Healthcare/djLint
-    rev: v1.31.1
+    rev: v1.32.1
     hooks:
       - id: djlint-jinja
   - repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
       - name: black (python implementations & bowtie internals)
         id: black
@@ -78,15 +78,15 @@
   - repo: https://github.com/pre-commit/mirrors-clang-format
     rev: v16.0.6
     hooks:
       - name: clang-format (c/c++/c#/java implementations)
         id: clang-format
         types_or: [c++, c, c#, java, objective-c]
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.45.0
+    rev: v8.46.0
     hooks:
       - name: eslint
         id: eslint
         files: ^frontend/src/.*\.jsx?$
         types: [file]
         additional_dependencies:
           - eslint@8.43.0
```

### Comparing `bowtie_json_schema-2023.7.9/noxfile.py` & `bowtie_json_schema-2023.8.1/noxfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
 @session(python=["3.10", "3.11"])
 def tests(session):
+    """
+    Run Bowtie's test suite.
+    """
     session.install("-r", ROOT / "test-requirements.txt")
 
     if session.posargs and session.posargs[0] == "coverage":
         if len(session.posargs) > 1 and session.posargs[1] == "github":
             github = os.environ["GITHUB_STEP_SUMMARY"]
         else:
             github = None
@@ -53,22 +56,28 @@
                 )
     else:
         session.run("pytest", *session.posargs, TESTS)
 
 
 @session(tags=["build"])
 def build(session):
+    """
+    Build Bowtie (via a PEP517 builder), and check the built artifact is valid.
+    """
     session.install("build", "twine")
     with TemporaryDirectory() as tmpdir:
         session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
         session.run("twine", "check", "--strict", tmpdir + "/*")
 
 
 @session(tags=["build"])
 def shiv(session):
+    """
+    Build a shiv which will run Bowtie.
+    """
     session.install("shiv")
 
     with ExitStack() as stack:
         if session.posargs:
             out = session.posargs[0]
         else:
             tmpdir = Path(stack.enter_context(TemporaryDirectory()))
@@ -85,20 +94,26 @@
             out,
         )
         print(f"Outputted a shiv to {out}.")
 
 
 @session(tags=["style"])
 def style(session):
+    """
+    Lint for style on Bowtie's Python codebase.
+    """
     session.install("ruff")
     session.run("ruff", "check", BOWTIE, TESTS, __file__)
 
 
 @session()
 def typing(session):
+    """
+    Check Bowtie's codebase using pyright.
+    """
     session.install("pyright", ROOT)
     session.run("pyright", BOWTIE)
 
 
 @session(tags=["docs"])
 @nox.parametrize(
     "builder",
@@ -110,14 +125,17 @@
             "linkcheck",
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
+    """
+    Build Bowtie's documentation.
+    """
     session.install("-r", DOCS / "requirements.txt")
     with TemporaryDirectory() as tmpdir_str:
         tmpdir = Path(tmpdir_str)
         argv = ["-n", "-T", "-W"]
         if builder != "spelling":
             argv += ["-q"]
         session.run(
@@ -130,14 +148,17 @@
             tmpdir / builder,
             *argv,
         )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
+    """
+    Check Bowtie's documentation style.
+    """
     session.install(
         "doc8",
         "pygments",
         "pygments-github-lexers",
     )
     session.run("python", "-m", "doc8", "--config", PYPROJECT, DOCS)
 
@@ -218,15 +239,41 @@
         command = f"{bowtie} suite -i {{implementation}} {posargs}"
     else:
         args, command = [], f"{bowtie} suite {posargs}"
     return args, command
 
 
 @session(default=False)
+def develop_harness(session):
+    """
+    Build a local version of an implementation harness.
+
+    This is used / useful during development of a new harness.
+
+    For "real" versions of harnesses, rely on the built version from GitHub
+    packages.
+    """
+    for each in session.posargs:
+        name = Path(each).name
+        session.run(
+            "podman",
+            "build",
+            "-f",
+            IMPLEMENTATIONS / name / "Dockerfile",
+            "-t",
+            f"ghcr.io/bowtie-jsonschema/{name}",
+            external=True,
+        )
+
+
+@session(default=False)
 def requirements(session):
+    """
+    Update bowtie's requirements.txt files.
+    """
     session.install("pip-tools")
     for each in [DOCS / "requirements.in", ROOT / "test-requirements.in"]:
         session.run(
             "pip-compile",
             "--resolver",
             "backtracking",
             "-U",
```

### Comparing `bowtie_json_schema-2023.7.9/test-requirements.txt` & `bowtie_json_schema-2023.8.1/test-requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile test-requirements.in
 #
 aiodocker==0.21.0
     # via bowtie-json-schema
-aiohttp==3.8.4
+aiohttp==3.8.5
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 async-timeout==4.0.2
     # via aiohttp
 attrs==23.1.0
     # via
     #   aiohttp
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 file:.#egg=bowtie-json-schema
     # via -r test-requirements.in
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
 cffi==1.15.1
     # via cryptography
 charset-normalizer==3.2.0
     # via
     #   aiohttp
     #   requests
-click==8.1.5
+click==8.1.6
     # via
     #   bowtie-json-schema
     #   trogon
 cryptography==41.0.2
     # via pyjwt
 frozenlist==1.4.0
     # via
@@ -48,17 +48,17 @@
     #   yarl
 importlib-metadata==6.8.0
     # via textual
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via bowtie-json-schema
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via bowtie-json-schema
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 linkify-it-py==2.0.2
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
@@ -79,56 +79,56 @@
     # via pytest
 pprintpp==0.4.0
     # via pytest-icdiff
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via rich
-pyjwt[crypto]==2.7.0
+pyjwt[crypto]==2.8.0
     # via github3-py
 pytest==7.4.0
     # via
     #   -r test-requirements.in
     #   pytest-asyncio
     #   pytest-icdiff
 pytest-asyncio==0.21.1
     # via -r test-requirements.in
 pytest-icdiff==0.6
     # via -r test-requirements.in
 python-dateutil==2.8.2
     # via github3-py
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via github3-py
 rich==13.4.2
     # via
     #   bowtie-json-schema
     #   textual
-rpds-py==0.8.11
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.29.0
+textual==0.30.0
     # via trogon
 trogon==0.5.0
     # via bowtie-json-schema
 typing-extensions==4.7.1
     # via
     #   aiodocker
     #   textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 yarl==1.9.2
     # via aiohttp
 zipp==3.16.2
     # via importlib-metadata
```

### Comparing `bowtie_json_schema-2023.7.9/.github/SECURITY.md` & `bowtie_json_schema-2023.8.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/.github/dependabot.yml` & `bowtie_json_schema-2023.8.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/.github/workflows/build-frontend.yml` & `bowtie_json_schema-2023.8.1/.github/workflows/build-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/.github/workflows/ci.yml` & `bowtie_json_schema-2023.8.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,15 @@
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
-            nox --list-sessions |
-            grep '^* ' |
-            cut -d ' ' -f 2- |
-            jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
+            nox --list-sessions --json | jq '[.[].session]'
           )
 
   ci:
     needs: list
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
```

### Comparing `bowtie_json_schema-2023.7.9/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.8.1/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/.github/workflows/deploy-frontend.yml` & `bowtie_json_schema-2023.8.1/.github/workflows/deploy-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/.github/workflows/images.yml` & `bowtie_json_schema-2023.8.1/.github/workflows/images.yml`

 * *Files 0% similar despite different names*

```diff
@@ -83,13 +83,13 @@
           tags: ${{ steps.build_image.outputs.tags }}
           registry: ghcr.io/${{ github.repository_owner }}
           username: ${{ github.actor }}
           password: ${{ github.token }}
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
 
       - name: Install Bowtie
-        uses: bowtie-json-schema/bowtie@v2023.07.7
+        uses: bowtie-json-schema/bowtie@v2023.07.10
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
 
       - name: Smoke Test
         run: bowtie smoke -i "${{ steps.build_image.outputs.image-with-tag }}"
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
```

### Comparing `bowtie_json_schema-2023.7.9/.github/workflows/report.yml` & `bowtie_json_schema-2023.8.1/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/bowtie/_cli.py` & `bowtie_json_schema-2023.8.1/bowtie/_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,22 @@
     "6": DRAFT6,
     "draft6": DRAFT6,
     "4": DRAFT4,
     "draft4": DRAFT4,
     "3": DRAFT3,
     "draft3": DRAFT3,
 }
+TEST_SUITE_DIALECT_URLS = {
+    DRAFT2020: f"{TEST_SUITE_URL}/tree/main/tests/draft2020-12",
+    DRAFT2019: f"{TEST_SUITE_URL}/tree/main/tests/draft2019-09",
+    DRAFT7: f"{TEST_SUITE_URL}/tree/main/tests/draft7",
+    DRAFT6: f"{TEST_SUITE_URL}/tree/main/tests/draft6",
+    DRAFT4: f"{TEST_SUITE_URL}/tree/main/tests/draft4",
+    DRAFT3: f"{TEST_SUITE_URL}/tree/main/tests/draft3",
+}
 LATEST_DIALECT_NAME = "draft2020-12"
 
 #: Should match the magic value used to validate `schema`s in `io-schema.json`
 CURRENT_DIALECT_URI = "urn:current-dialect"
 
 FORMAT = click.option(
     "--format",
@@ -620,14 +628,18 @@
         value: Any,
         param: click.Parameter | None,
         ctx: click.Context | None,
     ) -> tuple[Iterable[TestCase], str, dict[str, Any]]:
         if not isinstance(value, str):
             return value
 
+        # Convert dialect URIs or shortnames to test suite URIs
+        value = DIALECT_SHORTNAMES.get(value, value)
+        value = TEST_SUITE_DIALECT_URLS.get(value, value)
+
         is_local_path = not value.casefold().startswith(TEST_SUITE_URL)
         if is_local_path:
             cases, dialect = self._cases_and_dialect(path=Path(value))
             run_metadata = {}
         else:
             # Sigh. PyCQA/isort#1839
             # isort: off
@@ -700,25 +712,36 @@
     input: tuple[Iterable[TestCase], str, dict[str, Any]],
     filter: str,
     **kwargs: Any,
 ):
     """
     Run test cases from the official JSON Schema test suite.
 
-    Supports file or URL inputs like:
+    Supports a number of possible inputs:
+
+        * file paths found on the local file system containing tests, e.g.:
+
+            - ``{PATH}/tests/draft7`` to run the draft 7 version's tests out of a local checkout of the test suite
+
+            - ``{PATH}/tests/draft7/foo.json`` to run just one file from a checkout
+
+        * URLs to the test suite repository hosted on GitHub, e.g.:
+
+            - ``https://github.com/json-schema-org/JSON-Schema-Test-Suite/blob/main/tests/draft7/``
+              to run a version directly from any branch which exists in GitHub
 
-        * ``{ROOT}/tests/draft7`` to run a version's tests
+            - ``https://github.com/json-schema-org/JSON-Schema-Test-Suite/blob/main/tests/draft7/foo.json``
+              to run a single file directly from a branch which exists in GitHub
 
-        * ``{ROOT}/tests/draft7/foo.json`` to run just one file
+        * short name versions of the previous URLs (similar to those providable
+          to ``bowtie validate`` via its ``--dialect`` option), e.g.:
 
-        * ``https://github.com/json-schema-org/JSON-Schema-Test-Suite/blob/main/tests/draft7/``
-          to run a version directly from a branch which exists in GitHub
+            - ``7``, to run the draft 7 tests directly from GitHub (as in the
+              URL example above)
 
-        * ``https://github.com/json-schema-org/JSON-Schema-Test-Suite/blob/main/tests/draft7/foo.json``
-          to run a single file directly from a branch which exists in GitHub
     """  # noqa: E501
     cases, dialect, metadata = input
     if filter:
         cases = (case for case in cases if fnmatch(case.description, filter))
 
     task = _run(**kwargs, dialect=dialect, cases=cases, run_metadata=metadata)
     exit_code = asyncio.run(task)
```

### Comparing `bowtie_json_schema-2023.7.9/bowtie/_commands.py` & `bowtie_json_schema-2023.8.1/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/bowtie/_core.py` & `bowtie_json_schema-2023.8.1/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/bowtie/_report.py` & `bowtie_json_schema-2023.8.1/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/bowtie/exceptions.py` & `bowtie_json_schema-2023.8.1/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/docs/Makefile` & `bowtie_json_schema-2023.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/docs/cli.rst` & `bowtie_json_schema-2023.8.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/docs/conf.py` & `bowtie_json_schema-2023.8.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 pygments_dark_style = "one-dark"
 
 html_theme = "furo"
 html_logo = str(STATIC / "dreamed.png")
 html_static_path = [str(STATIC)]
 
 rst_prolog = """
-.. |site| replace:: https://bowtie-json-schema.github.io/bowtie/
+.. |site| replace:: https://bowtie.report/
 
 .. _official test suite: https://github.com/json-schema-org/JSON-Schema-Test-Suite
 """  # noqa: E501
 
 
 def entire_domain(host):
     return r"http.?://" + re.escape(host) + r"($|/.*)"
```

### Comparing `bowtie_json_schema-2023.7.9/docs/contributing.rst` & `bowtie_json_schema-2023.8.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/docs/implementers.rst` & `bowtie_json_schema-2023.8.1/docs/implementers.rst`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     print('Hello world')
 
 and build the image (below using ``podman`` but if you're using ``docker``, just substitute it for ``podman`` in all commands below):
 
 .. code:: sh
 
-    podman build --quiet -f Dockerfile -t bowtie-lua-jsonschema
+    podman build --quiet -f Dockerfile -t bowtie-lua-jsonschema .
 
 If everything went well, running:
 
 .. code:: sh
 
     podman run --rm bowtie-lua-jsonschema
 
@@ -137,15 +137,15 @@
 
 .. note::
 
     From here on out in this document it's assumed you rebuild your container image each time you modify the harness via
 
     .. code:: sh
 
-        podman build -f Dockerfile -t localhost/tutorial-lua-jsonschema
+        podman build -f Dockerfile -t localhost/tutorial-lua-jsonschema .
 
 Change your harness to contain:
 
 .. code:: lua
 
     local json = require 'json'
```

### Comparing `bowtie_json_schema-2023.7.9/docs/index.rst` & `bowtie_json_schema-2023.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/docs/requirements.txt` & `bowtie_json_schema-2023.8.1/docs/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --config=pyproject.toml docs/requirements.in
 #
 aiodocker==0.21.0
     # via bowtie-json-schema
-aiohttp==3.8.4
+aiohttp==3.8.5
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
     # via sphinx
 async-timeout==4.0.2
     # via aiohttp
@@ -22,44 +22,44 @@
     #   referencing
 babel==2.12.1
     # via sphinx
 beautifulsoup4==4.12.2
     # via furo
 file:.#egg=bowtie-json-schema
     # via -r docs/requirements.in
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
 cffi==1.15.1
     # via cryptography
 charset-normalizer==3.2.0
     # via
     #   aiohttp
     #   requests
-click==8.1.5
+click==8.1.6
     # via
     #   bowtie-json-schema
     #   sphinx-click
     #   trogon
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via pyjwt
 cycler==0.11.0
     # via matplotlib
 docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-click
-fonttools==4.41.0
+fonttools==4.41.1
     # via matplotlib
 frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
-furo==2023.5.20
+furo==2023.7.26
     # via -r docs/requirements.in
 github3-py==4.0.1
     # via bowtie-json-schema
 idna==3.4
     # via
     #   requests
     #   yarl
@@ -67,17 +67,17 @@
     # via sphinx
 importlib-metadata==6.8.0
     # via textual
 jinja2==3.1.2
     # via
     #   bowtie-json-schema
     #   sphinx
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via bowtie-json-schema
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 linkify-it-py==2.0.2
     # via markdown-it-py
 lxml==4.9.3
     # via sphinx-json-schema-spec
@@ -116,45 +116,45 @@
     # via
     #   furo
     #   pygments-github-lexers
     #   rich
     #   sphinx
 pygments-github-lexers==0.0.5
     # via -r docs/requirements.in
-pyjwt[crypto]==2.7.0
+pyjwt[crypto]==2.8.0
     # via github3-py
 pyparsing==3.0.9
     # via matplotlib
 python-dateutil==2.8.2
     # via
     #   github3-py
     #   matplotlib
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   github3-py
     #   sphinx
 rich==13.4.2
     # via
     #   bowtie-json-schema
     #   textual
-rpds-py==0.8.11
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==7.0.1
+sphinx==7.1.1
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
@@ -162,15 +162,15 @@
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-click==4.4.0
     # via -r docs/requirements.in
 sphinx-copybutton==0.5.2
     # via -r docs/requirements.in
-sphinx-json-schema-spec==2023.5.3
+sphinx-json-schema-spec==2023.7.2
     # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -182,27 +182,27 @@
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
 sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.29.0
+textual==0.30.0
     # via trogon
 trogon==0.5.0
     # via bowtie-json-schema
 typing-extensions==4.7.1
     # via
     #   aiodocker
     #   textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 yarl==1.9.2
     # via
     #   -r docs/requirements.in
     #   aiohttp
 zipp==3.16.2
     # via importlib-metadata
```

### Comparing `bowtie_json_schema-2023.7.9/docs/_static/dreamed.png` & `bowtie_json_schema-2023.8.1/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/package-lock.json` & `bowtie_json_schema-2023.8.1/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/package.json` & `bowtie_json_schema-2023.8.1/frontend/package.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2023.8.1/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/public/favicon.ico` & `bowtie_json_schema-2023.8.1/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/ReportDataHandler.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/ReportDataHandler.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/index.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/index.jsx`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 import { createHashRouter, RouterProvider } from "react-router-dom";
 import ThemeContextProvider from "./context/ThemeContext";
 import { MainContainer } from "./MainContainer";
 import { BowtieVersionContextProvider } from "./context/BowtieVersionContext";
 import { DragAndDrop } from "./components/DragAndDrop/DragAndDrop";
 import { parseReportData } from "./data/parseReportData";
 
-const reportUrl =
-  import.meta.env.MODE === "development"
-    ? "https://bowtie-json-schema.github.io/bowtie"
-    : import.meta.env.BASE_URL;
+const reportUrl = "https://bowtie.report";
 const titleTag = document.getElementsByTagName("title")[0];
 const dialectToName = {
   "draft2020-12": "Draft 2020-12",
   "draft2019-09": "Draft 2019-09",
   draft7: "Draft 7",
   draft6: "Draft 6",
   draft4: "Draft 4",
```

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/CopyToClipboard.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/CopyToClipboard.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/LoadingAnimation.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/LoadingAnimation.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/NavBar.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/NavBar.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionItem.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionItem.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionSvg.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionSvg.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/CasesSection.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/CasesSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/SchemaDisplay.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/SchemaDisplay.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/DragAndDrop/DragAndDrop.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/DragAndDrop/DragAndDrop.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Modals/DetailsButtonModal.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Modals/DetailsButtonModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Modals/RunTimeInfoModal.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Modals/RunTimeInfoModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/RunInfo/RunInfoSection.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/RunInfo/RunInfoSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummarySection.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummarySection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummaryTable.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummaryTable.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/context/ThemeContext.jsx` & `bowtie_json_schema-2023.8.1/frontend/src/context/ThemeContext.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2023.8.1/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/tests/test_integration.py` & `bowtie_json_schema-2023.8.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.8.1/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.8.1/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.8.1/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.8.1/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/.gitignore` & `bowtie_json_schema-2023.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/LICENSE` & `bowtie_json_schema-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/README.rst` & `bowtie_json_schema-2023.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/pyproject.toml` & `bowtie_json_schema-2023.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.9/PKG-INFO` & `bowtie_json_schema-2023.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.7.9
+Version: 2023.8.1
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

