# Comparing `tmp/cybergis_compute_client-0.2.4.tar.gz` & `tmp/cybergis_compute_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybergis_compute_client-0.2.4.tar", last modified: Thu Mar  2 15:15:00 2023, max compression
+gzip compressed data, was "cybergis_compute_client-0.2.5.tar", last modified: Wed Aug  2 17:15:23 2023, max compression
```

## Comparing `cybergis_compute_client-0.2.4.tar` & `cybergis_compute_client-0.2.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.477858 cybergis_compute_client-0.2.4/
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.465858 cybergis_compute_client-0.2.4/.github/
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.465858 cybergis_compute_client-0.2.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      404 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      747 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      821 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       41 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.465858 cybergis_compute_client-0.2.4/.github/workflows/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      553 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.github/workflows/PythonCodeTestCases.yml
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      549 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.github/workflows/PythonQualityCheck.yml
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      588 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.github/workflows/SphinxBuild.yml
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1986 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/.gitignore
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    11386 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/LICENSE
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     5620 2023-03-02 15:15:00.477858 cybergis_compute_client-0.2.4/PKG-INFO
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     4841 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/README.md
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.469858 cybergis_compute_client-0.2.4/cybergis_compute_client/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2180 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/cybergis_compute_client/Client.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    21106 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/cybergis_compute_client/CyberGISCompute.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    13819 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/cybergis_compute_client/Job.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      537 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/cybergis_compute_client/MarkdownTable.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    44048 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/cybergis_compute_client/UI.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2654 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/cybergis_compute_client/Zip.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      700 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/cybergis_compute_client/__init__.py
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.469858 cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     5620 2023-03-02 15:15:00.000000 cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/PKG-INFO
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1868 2023-03-02 15:15:00.000000 cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/SOURCES.txt
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)        1 2023-03-02 15:15:00.000000 cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/dependency_links.txt
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       56 2023-03-02 15:15:00.000000 cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/requires.txt
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       29 2023-03-02 15:15:00.000000 cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/top_level.txt
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.469858 cybergis_compute_client-0.2.4/docs/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      634 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/Makefile
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.473858 cybergis_compute_client-0.2.4/docs/_static/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    22382 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/favico.ico
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.473858 cybergis_compute_client-0.2.4/docs/_static/gif/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   906811 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/gif/CyberGIS-ComputeHello.gif
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)  1009434 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/gif/CyberGIS-HelloWorld.gif
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.473858 cybergis_compute_client-0.2.4/docs/_static/img/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    17723 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/Compute.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    14626 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/DownloadJobOutput.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    97257 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/JupyterExportAs.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    25843 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/ListGit.png
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.477858 cybergis_compute_client-0.2.4/docs/_static/img/models/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   682708 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/models/AccessChicago.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   344691 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/models/IllinoisAccess.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)  1071330 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/models/RemoteSensingDataFusion.png
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.477858 cybergis_compute_client-0.2.4/docs/_static/img/user-guide/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   113343 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/user-guide/CompletedJob.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    21172 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/user-guide/DownloadSuccess.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    71065 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/user-guide/JobSubmitted.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    47606 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/user-guide/NewNotebook.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    63253 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/user-guide/SDKUI.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    98773 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/_static/img/user-guide/YourJobs.png
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     4152 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/about.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     3826 2023-03-02 15:11:00.000000 cybergis_compute_client-0.2.4/docs/conf.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2586 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/contributing.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      679 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/external.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     3428 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/help.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2754 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/index.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      800 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/make.bat
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.477858 cybergis_compute_client-0.2.4/docs/model_contribution/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    21782 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/model_contribution/develop_model.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1874 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/model_contribution/faq.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      770 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/model_contribution/index.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     5013 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/models.rst
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.477858 cybergis_compute_client-0.2.4/docs/notebooks/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       41 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/notebooks/hello_world.nblink
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1374 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/reference.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     3604 2023-03-02 15:11:49.000000 cybergis_compute_client-0.2.4/docs/release-notes.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      136 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/requirements.txt
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     9765 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/docs/usage.rst
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    68246 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/hello_world.ipynb
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      103 2023-03-02 15:15:00.481858 cybergis_compute_client-0.2.4/setup.cfg
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     4073 2023-03-02 15:10:56.000000 cybergis_compute_client-0.2.4/setup.py
-drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:15:00.477858 cybergis_compute_client-0.2.4/test/
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1829 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/test/UI_test_cases.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)        0 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/test/__init__.py
--rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2093 2023-03-02 15:08:52.000000 cybergis_compute_client-0.2.4/test/test_cases.py
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.267524 cybergis_compute_client-0.2.5/
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.235522 cybergis_compute_client-0.2.5/.github/
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.239522 cybergis_compute_client-0.2.5/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      404 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      747 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      821 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       41 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.239522 cybergis_compute_client-0.2.5/.github/workflows/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      553 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.github/workflows/PythonCodeTestCases.yml
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      549 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.github/workflows/PythonQualityCheck.yml
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      588 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.github/workflows/SphinxBuild.yml
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1986 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/.gitignore
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    11386 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/LICENSE
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     5620 2023-08-02 17:15:23.267524 cybergis_compute_client-0.2.5/PKG-INFO
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     4841 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/README.md
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.239522 cybergis_compute_client-0.2.5/cybergis_compute_client/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2180 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/cybergis_compute_client/Client.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    21106 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/cybergis_compute_client/CyberGISCompute.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    13819 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/cybergis_compute_client/Job.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      537 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/cybergis_compute_client/MarkdownTable.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    45932 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/cybergis_compute_client/UI.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2654 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/cybergis_compute_client/Zip.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      700 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/cybergis_compute_client/__init__.py
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.239522 cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     5620 2023-08-02 17:15:22.000000 cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/PKG-INFO
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1868 2023-08-02 17:15:23.000000 cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)        1 2023-08-02 17:15:22.000000 cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       56 2023-08-02 17:15:22.000000 cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/requires.txt
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       29 2023-08-02 17:15:22.000000 cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/top_level.txt
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.247522 cybergis_compute_client-0.2.5/docs/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      634 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/Makefile
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.247522 cybergis_compute_client-0.2.5/docs/_static/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    22382 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/favico.ico
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.251523 cybergis_compute_client-0.2.5/docs/_static/gif/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   906811 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/gif/CyberGIS-ComputeHello.gif
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)  1009434 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/gif/CyberGIS-HelloWorld.gif
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.255523 cybergis_compute_client-0.2.5/docs/_static/img/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    17723 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/Compute.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    14626 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/DownloadJobOutput.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    97257 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/JupyterExportAs.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    25843 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/ListGit.png
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.255523 cybergis_compute_client-0.2.5/docs/_static/img/models/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   682708 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/models/AccessChicago.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   344691 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/models/IllinoisAccess.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)  1071330 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/models/RemoteSensingDataFusion.png
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.263523 cybergis_compute_client-0.2.5/docs/_static/img/user-guide/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)   113343 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/user-guide/CompletedJob.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    21172 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/user-guide/DownloadSuccess.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    71065 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/user-guide/JobSubmitted.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    47606 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/user-guide/NewNotebook.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    63253 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/user-guide/SDKUI.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    98773 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/_static/img/user-guide/YourJobs.png
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     4152 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/about.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     3826 2023-08-02 17:07:59.000000 cybergis_compute_client-0.2.5/docs/conf.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2586 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/contributing.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      679 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/external.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     3428 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/help.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2754 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/index.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      800 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/make.bat
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.267524 cybergis_compute_client-0.2.5/docs/model_contribution/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    21782 2023-08-02 17:12:49.000000 cybergis_compute_client-0.2.5/docs/model_contribution/develop_model.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1874 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/model_contribution/faq.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      770 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/model_contribution/index.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     5013 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/models.rst
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.267524 cybergis_compute_client-0.2.5/docs/notebooks/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)       41 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/notebooks/hello_world.nblink
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1374 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/reference.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     4022 2023-08-02 17:13:42.000000 cybergis_compute_client-0.2.5/docs/release-notes.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      136 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/requirements.txt
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     9765 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/docs/usage.rst
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)    68246 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/hello_world.ipynb
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)      103 2023-08-02 17:15:23.271524 cybergis_compute_client-0.2.5/setup.cfg
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     4073 2023-08-02 17:07:54.000000 cybergis_compute_client-0.2.5/setup.py
+drwxrwxr-x   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:15:23.267524 cybergis_compute_client-0.2.5/test/
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     1829 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/test/UI_test_cases.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)        0 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/test/__init__.py
+-rw-rw-r--   0 dijkstra  (1000) dijkstra  (1000)     2093 2023-08-02 17:07:33.000000 cybergis_compute_client-0.2.5/test/test_cases.py
```

### Comparing `cybergis_compute_client-0.2.4/.github/ISSUE_TEMPLATE/config.yml` & `cybergis_compute_client-0.2.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `cybergis_compute_client-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/.github/workflows/PythonCodeTestCases.yml` & `cybergis_compute_client-0.2.5/.github/workflows/PythonCodeTestCases.yml`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/.github/workflows/PythonQualityCheck.yml` & `cybergis_compute_client-0.2.5/.github/workflows/PythonQualityCheck.yml`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/.github/workflows/SphinxBuild.yml` & `cybergis_compute_client-0.2.5/.github/workflows/SphinxBuild.yml`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/.gitignore` & `cybergis_compute_client-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/LICENSE` & `cybergis_compute_client-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/PKG-INFO` & `cybergis_compute_client-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybergis_compute_client
-Version: 0.2.4
+Version: 0.2.5
 Summary: CyberGISX compatable HPC job submission client
 Home-page: https://github.com/cybergis/cybergis-compute-python-sdk
 Author: CyberGIS Center
 Author-email: help@cybergis.org
 License: Apache License 2.0
 Keywords: HPC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cybergis_compute_client-0.2.4/README.md` & `cybergis_compute_client-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client/Client.py` & `cybergis_compute_client-0.2.5/cybergis_compute_client/Client.py`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client/CyberGISCompute.py` & `cybergis_compute_client-0.2.5/cybergis_compute_client/CyberGISCompute.py`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client/Job.py` & `cybergis_compute_client-0.2.5/cybergis_compute_client/Job.py`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client/MarkdownTable.py` & `cybergis_compute_client-0.2.5/cybergis_compute_client/MarkdownTable.py`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client/UI.py` & `cybergis_compute_client-0.2.5/cybergis_compute_client/UI.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,16 +78,18 @@
         self.renderComponents()
         divider = Markdown('***')
         # render main UI
         # 1. job template
         job_config = widgets.Output()
         with job_config:
             display(Markdown('# Welcome to CyberGIS-Compute'))
-            display(Markdown('A scalable middleware framework for enabling high-performance and data-intensive geospatial research and education on CyberGIS-Jupyter'))
+            display(Markdown('A scalable middleware framework for enabling high-performance and data-intensive geospatial research and education on CyberGIS-Jupyter. [Click here for documentation.](https://cybergis.github.io/cybergis-compute-python-sdk/index.html)'))
             display(divider)
+            display(Markdown('**Your CyberGIS-Compute Username:** ' + str(self.compute.username)))
+            self.renderAnnouncements()
             display(self.jobTemplate['output'])
             display(self.description['output'])
             display(self.computingResource['output'])
             display(self.slurm['output'])
             display(self.param['output'])
             display(self.uploadData['output'])
             display(self.email['output'])
@@ -156,14 +158,30 @@
         self.renderDownload()
         self.renderRecentlySubmittedJobs()
         self.renderLoadMore()
         self.renderSubmitNew()
         self.renderFolders()
 
     # components
+    def renderAnnouncements(self):
+        """
+        Displays announcements if the announcement route exists and there are any
+        """
+        try:
+            announcement = self.compute.client.request('GET', '/announcement')["announcements"]
+            if (len(announcement) > 0):
+                display(Markdown('## Announcements'))
+                for i in range(len(announcement)):
+                    display(Markdown('### Message ' + str(i + 1) + ':'))
+                    display(Markdown('Message: ' + announcement[i]["message"]))
+                    display(Markdown('Posted by: ' + announcement[i]["poster"] + " at " + announcement[i]["time_stamp"]))
+                display(Markdown("***"))
+        except:
+            pass
+
     def renderJobTemplate(self):
         """
         Display a dropdown of jobs to run.
         Update jobTemplate when the dropdown changes.
         """
         if self.jobTemplate['output'] is None:
 
@@ -697,16 +715,25 @@
                     dataPath = dataPath.replace(self.jupyter_globus['container_home_path'].strip('/'), '')
                     dataPath = os.path.join(self.jupyter_globus['root_path'], dataPath.strip('/'))
                     localDataFolder = {
                         'type': 'globus',
                         'endpoint': self.jupyter_globus['endpoint'],
                         'path': dataPath
                     }
-
-            self.compute.job = self.compute.create_job(hpc=data['computing_resource'], verbose=False)
+            try:
+                self.compute.job = self.compute.create_job(hpc=data['computing_resource'], verbose=False)
+            except Exception as e:
+                print("There was an exception while submitting the job: " + str(e))
+                if "Not authorized for HPC" in str(e):  # TODO: we should create a specific exception rather than checking the message
+                    with self.submit['alert_output']:
+                        display(Markdown("<b><font color='red'>You are not authorized to submit jobs to this HPC (" + str(data['computing_resource']) + "). Please try another HPC or contact the CyberGIS-Compute team.</b>"""))
+                else:  # generic error
+                    with self.submit['alert_output']:
+                        display(Markdown("<b><font color='red'>There was an exception while submitting the job: " + str(e) + "</b>"))
+                return
             # slurm
             slurm = data['slurm']
             if data['email'] is not None:
                 slurm['mail_user'] = [data['email']]
                 slurm['mail_type'] = ['FAIL', 'END', 'BEGIN']
             # param
             param = data['param']
@@ -772,14 +799,15 @@
             """
             if change['type'] == 'change':
                 if self.submitted:
                     return
                 self.hpcName = self.computingResource['dropdown'].value
                 self.hpc = self.hpcs[self.hpcName]
                 self.rerender(['description', 'slurm', 'param', 'uploadData'])
+                self.submit['alert_output'].clear_output()  # clear any errors from previous job
         return on_change
 
     def onLoadMoreClick(self):
         def on_click(change):
             """
             Increase the number of recently submitted jobs being displayed by five and rerender teh recently subsmitted and load more attributes.
             """
```

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client/Zip.py` & `cybergis_compute_client-0.2.5/cybergis_compute_client/Zip.py`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client/__init__.py` & `cybergis_compute_client-0.2.5/cybergis_compute_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/PKG-INFO` & `cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybergis-compute-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: CyberGISX compatable HPC job submission client
 Home-page: https://github.com/cybergis/cybergis-compute-python-sdk
 Author: CyberGIS Center
 Author-email: help@cybergis.org
 License: Apache License 2.0
 Keywords: HPC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cybergis_compute_client-0.2.4/cybergis_compute_client.egg-info/SOURCES.txt` & `cybergis_compute_client-0.2.5/cybergis_compute_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/Makefile` & `cybergis_compute_client-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/favico.ico` & `cybergis_compute_client-0.2.5/docs/_static/favico.ico`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/gif/CyberGIS-ComputeHello.gif` & `cybergis_compute_client-0.2.5/docs/_static/gif/CyberGIS-ComputeHello.gif`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/gif/CyberGIS-HelloWorld.gif` & `cybergis_compute_client-0.2.5/docs/_static/gif/CyberGIS-HelloWorld.gif`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/Compute.png` & `cybergis_compute_client-0.2.5/docs/_static/img/Compute.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/DownloadJobOutput.png` & `cybergis_compute_client-0.2.5/docs/_static/img/DownloadJobOutput.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/JupyterExportAs.png` & `cybergis_compute_client-0.2.5/docs/_static/img/JupyterExportAs.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/ListGit.png` & `cybergis_compute_client-0.2.5/docs/_static/img/ListGit.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/models/AccessChicago.png` & `cybergis_compute_client-0.2.5/docs/_static/img/models/AccessChicago.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/models/IllinoisAccess.png` & `cybergis_compute_client-0.2.5/docs/_static/img/models/IllinoisAccess.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/models/RemoteSensingDataFusion.png` & `cybergis_compute_client-0.2.5/docs/_static/img/models/RemoteSensingDataFusion.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/user-guide/CompletedJob.png` & `cybergis_compute_client-0.2.5/docs/_static/img/user-guide/CompletedJob.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/user-guide/DownloadSuccess.png` & `cybergis_compute_client-0.2.5/docs/_static/img/user-guide/DownloadSuccess.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/user-guide/JobSubmitted.png` & `cybergis_compute_client-0.2.5/docs/_static/img/user-guide/JobSubmitted.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/user-guide/NewNotebook.png` & `cybergis_compute_client-0.2.5/docs/_static/img/user-guide/NewNotebook.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/user-guide/SDKUI.png` & `cybergis_compute_client-0.2.5/docs/_static/img/user-guide/SDKUI.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/_static/img/user-guide/YourJobs.png` & `cybergis_compute_client-0.2.5/docs/_static/img/user-guide/YourJobs.png`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/about.rst` & `cybergis_compute_client-0.2.5/docs/about.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/conf.py` & `cybergis_compute_client-0.2.5/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # -- Project information -----------------------------------------------------
 project = 'CyberGIS-Compute Python SDK'
 copyright = '2022, CyberGIS Center'
 author = 'CyberGIS Center'
 
 # The full version, including alpha/beta/rc tags
-release = 'v0.2.4'
+release = 'v0.2.5'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `cybergis_compute_client-0.2.4/docs/contributing.rst` & `cybergis_compute_client-0.2.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/external.rst` & `cybergis_compute_client-0.2.5/docs/external.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/help.rst` & `cybergis_compute_client-0.2.5/docs/help.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/index.rst` & `cybergis_compute_client-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/make.bat` & `cybergis_compute_client-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/model_contribution/develop_model.rst` & `cybergis_compute_client-0.2.5/docs/model_contribution/develop_model.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/model_contribution/faq.rst` & `cybergis_compute_client-0.2.5/docs/model_contribution/faq.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/model_contribution/index.rst` & `cybergis_compute_client-0.2.5/docs/model_contribution/index.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/models.rst` & `cybergis_compute_client-0.2.5/docs/models.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/reference.rst` & `cybergis_compute_client-0.2.5/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/docs/release-notes.rst` & `cybergis_compute_client-0.2.5/docs/release-notes.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 Release Notes
 =============
 
 Release notes for the CyberGISX platform can be found here: `https://cybergisxhub.cigi.illinois.edu/release-notes/ <https://cybergisxhub.cigi.illinois.edu/release-notes/>`_
 
 For details and full changelogs, check out the releases on Github: `https://github.com/cybergis/cybergis-compute-python-sdk/releases <https://github.com/cybergis/cybergis-compute-python-sdk/releases>`_
 
+[v0.2.5] - 2023-08-02
+---------------------
+
+Added
+^^^^^
+
+* Added an announcements section to the GUI in `#65 <https://github.com/cybergis/cybergis-compute-python-sdk/pull/65>`_
+* Catching the Core's new HPC access denied exception in `#68 <https://github.com/cybergis/cybergis-compute-python-sdk/pull/68>`_
+* Added the username to the GUI in `#70 <https://github.com/cybergis/cybergis-compute-python-sdk/pull/70>`_
+
+
 [v0.2.4] - 2023-03-02
 ---------------------
 
 Added
 ^^^^^
 
 * Allow users to name folders in the UI in `#62 <https://github.com/cybergis/cybergis-compute-python-sdk/pull/62>`_
```

### Comparing `cybergis_compute_client-0.2.4/docs/usage.rst` & `cybergis_compute_client-0.2.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/hello_world.ipynb` & `cybergis_compute_client-0.2.5/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/setup.py` & `cybergis_compute_client-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='cybergis_compute_client',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.2.4',
+    version='0.2.5',
 
     description='CyberGISX compatable HPC job submission client',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/cybergis/cybergis-compute-python-sdk',
```

### Comparing `cybergis_compute_client-0.2.4/test/UI_test_cases.py` & `cybergis_compute_client-0.2.5/test/UI_test_cases.py`

 * *Files identical despite different names*

### Comparing `cybergis_compute_client-0.2.4/test/test_cases.py` & `cybergis_compute_client-0.2.5/test/test_cases.py`

 * *Files identical despite different names*

