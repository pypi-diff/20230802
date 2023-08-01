# Comparing `tmp/labxpipe-0.7.0.tar.gz` & `tmp/labxpipe-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labxpipe-0.7.0.tar", last modified: Wed May 17 02:14:01 2023, max compression
+gzip compressed data, was "labxpipe-0.7.1.tar", last modified: Tue Aug  1 22:43:31 2023, max compression
```

## Comparing `labxpipe-0.7.0.tar` & `labxpipe-0.7.1.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.047361 labxpipe-0.7.0/
--rw-r--r--   0 build     (1000) build     (1001)       17 2023-05-17 02:13:32.000000 labxpipe-0.7.0/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/.sourcehut/
--rw-r--r--   0 build     (1000) build     (1001)     1272 2023-05-17 02:13:32.000000 labxpipe-0.7.0/.sourcehut/arch.yml
--rw-r--r--   0 build     (1000) build     (1001)    16726 2023-05-17 02:13:32.000000 labxpipe-0.7.0/LICENSE
--rw-r--r--   0 build     (1000) build     (1001)    12773 2023-05-17 02:14:01.047361 labxpipe-0.7.0/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)    12477 2023-05-17 02:13:32.000000 labxpipe-0.7.0/README.md
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/config/
--rw-r--r--   0 build     (1000) build     (1001)     1065 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/labxpipe.json
--rw-r--r--   0 build     (1000) build     (1001)     1123 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/labxpipe_trackhub.json
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/config/pipelines/
--rw-r--r--   0 build     (1000) build     (1001)     2189 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/chip_seq.json
--rw-r--r--   0 build     (1000) build     (1001)     2440 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq.json
--rw-r--r--   0 build     (1000) build     (1001)     2226 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq_cufflinks.json
--rw-r--r--   0 build     (1000) build     (1001)     2898 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq_no_db.json
--rw-r--r--   0 build     (1000) build     (1001)     2802 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq_with_plotting.json
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.040745 labxpipe-0.7.0/img/
--rw-r--r--   0 build     (1000) build     (1001)     5728 2023-05-17 02:13:32.000000 labxpipe-0.7.0/img/logo.svg
--rw-r--r--   0 build     (1000) build     (1001)      581 2023-05-17 02:13:32.000000 labxpipe-0.7.0/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1001)       38 2023-05-17 02:14:01.047361 labxpipe-0.7.0/setup.cfg
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/src/
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.040745 labxpipe-0.7.0/src/labxpipe/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.044053 labxpipe-0.7.0/src/labxpipe/interfaces/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     1547 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bg2bw.py
--rw-r--r--   0 build     (1000) build     (1001)     5817 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bowtie2.py
--rw-r--r--   0 build     (1000) build     (1001)     4700 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bwa_mem2.py
--rw-r--r--   0 build     (1000) build     (1001)     2336 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_cufflinks.py
--rw-r--r--   0 build     (1000) build     (1001)     8069 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_geneabacus.py
--rw-r--r--   0 build     (1000) build     (1001)     4642 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_minimap2.py
--rw-r--r--   0 build     (1000) build     (1001)     4564 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_readknead.py
--rw-r--r--   0 build     (1000) build     (1001)     2733 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_samtools.py
--rw-r--r--   0 build     (1000) build     (1001)     6569 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_star.py
--rw-r--r--   0 build     (1000) build     (1001)     2876 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/parallel_helpers.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.044053 labxpipe-0.7.0/src/labxpipe/steps/
--rw-r--r--   0 build     (1000) build     (1001)      423 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     4181 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/bowtie2.py
--rw-r--r--   0 build     (1000) build     (1001)     4152 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/bwa_mem2.py
--rw-r--r--   0 build     (1000) build     (1001)     1431 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/cleaning.py
--rw-r--r--   0 build     (1000) build     (1001)     2413 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/cufflinks.py
--rw-r--r--   0 build     (1000) build     (1001)     6565 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/geneabacus.py
--rw-r--r--   0 build     (1000) build     (1001)     4238 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/minimap2.py
--rw-r--r--   0 build     (1000) build     (1001)     5492 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/readknead.py
--rw-r--r--   0 build     (1000) build     (1001)     2950 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/samtools_sort.py
--rw-r--r--   0 build     (1000) build     (1001)     3625 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/samtools_uniquify.py
--rw-r--r--   0 build     (1000) build     (1001)     3235 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/star.py
--rw-r--r--   0 build     (1000) build     (1001)     8654 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/trackhub.py
--rw-r--r--   0 build     (1000) build     (1001)     1739 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/utils.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.040745 labxpipe-0.7.0/src/labxpipe.egg-info/
--rw-r--r--   0 build     (1000) build     (1001)    12773 2023-05-17 02:14:00.000000 labxpipe-0.7.0/src/labxpipe.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)     1789 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1001)        1 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1001)       56 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1001)       44 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1001)       26 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/top_level.txt
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.047361 labxpipe-0.7.0/src/labxpipe_scripts/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/__init__.py
--rwxr-xr-x   0 build     (1000) build     (1001)     2440 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe.py
--rwxr-xr-x   0 build     (1000) build     (1001)    15493 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_demultiplex.py
--rwxr-xr-x   0 build     (1000) build     (1001)     7803 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_extract.py
--rwxr-xr-x   0 build     (1000) build     (1001)     7704 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_generate.py
--rwxr-xr-x   0 build     (1000) build     (1001)    17284 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_merge_count.py
--rwxr-xr-x   0 build     (1000) build     (1001)     4243 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_profile.py
--rwxr-xr-x   0 build     (1000) build     (1001)    13924 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_report.py
--rwxr-xr-x   0 build     (1000) build     (1001)    16815 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_run.py
--rwxr-xr-x   0 build     (1000) build     (1001)    21424 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_trackhub.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:31.005391 labxpipe-0.7.1/
+-rw-r--r--   0 build     (1000) build     (1001)       17 2023-08-01 22:42:38.000000 labxpipe-0.7.1/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.995391 labxpipe-0.7.1/.sourcehut/
+-rw-r--r--   0 build     (1000) build     (1001)     1272 2023-08-01 22:42:38.000000 labxpipe-0.7.1/.sourcehut/arch.yml
+-rw-r--r--   0 build     (1000) build     (1001)    16726 2023-08-01 22:42:38.000000 labxpipe-0.7.1/LICENSE
+-rw-r--r--   0 build     (1000) build     (1001)    17025 2023-08-01 22:43:31.005391 labxpipe-0.7.1/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)    16729 2023-08-01 22:42:38.000000 labxpipe-0.7.1/README.md
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.995391 labxpipe-0.7.1/config/
+-rw-r--r--   0 build     (1000) build     (1001)     1065 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/labxpipe.json
+-rw-r--r--   0 build     (1000) build     (1001)     1123 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/labxpipe_trackhub.json
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.998725 labxpipe-0.7.1/config/pipelines/
+-rw-r--r--   0 build     (1000) build     (1001)     2561 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/pipelines/chip_seq.json
+-rw-r--r--   0 build     (1000) build     (1001)     3127 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/pipelines/chip_seq_user_function.json
+-rw-r--r--   0 build     (1000) build     (1001)     2922 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/pipelines/mrna_seq.json
+-rw-r--r--   0 build     (1000) build     (1001)     2655 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/pipelines/mrna_seq_cufflinks.json
+-rw-r--r--   0 build     (1000) build     (1001)     3380 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/pipelines/mrna_seq_no_db.json
+-rw-r--r--   0 build     (1000) build     (1001)     4830 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/pipelines/mrna_seq_profiling_bam.json
+-rw-r--r--   0 build     (1000) build     (1001)     3300 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/pipelines/mrna_seq_with_plotting.json
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.998725 labxpipe-0.7.1/config/user_steps/
+-rw-r--r--   0 build     (1000) build     (1001)     2031 2023-08-01 22:42:38.000000 labxpipe-0.7.1/config/user_steps/macs3.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.998725 labxpipe-0.7.1/img/
+-rw-r--r--   0 build     (1000) build     (1001)     5728 2023-08-01 22:42:38.000000 labxpipe-0.7.1/img/logo.svg
+-rw-r--r--   0 build     (1000) build     (1001)      581 2023-08-01 22:42:38.000000 labxpipe-0.7.1/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1001)       38 2023-08-01 22:43:31.005391 labxpipe-0.7.1/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.995391 labxpipe-0.7.1/src/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.998725 labxpipe-0.7.1/src/labxpipe/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:31.002058 labxpipe-0.7.1/src/labxpipe/interfaces/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     1547 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_bg2bw.py
+-rw-r--r--   0 build     (1000) build     (1001)     5817 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_bowtie2.py
+-rw-r--r--   0 build     (1000) build     (1001)     4700 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_bwa_mem2.py
+-rw-r--r--   0 build     (1000) build     (1001)     2336 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_cufflinks.py
+-rw-r--r--   0 build     (1000) build     (1001)     8069 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_geneabacus.py
+-rw-r--r--   0 build     (1000) build     (1001)     4642 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_minimap2.py
+-rw-r--r--   0 build     (1000) build     (1001)     4564 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_readknead.py
+-rw-r--r--   0 build     (1000) build     (1001)     2733 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_samtools.py
+-rw-r--r--   0 build     (1000) build     (1001)     6569 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_star.py
+-rw-r--r--   0 build     (1000) build     (1001)     2876 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/parallel_helpers.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:31.005391 labxpipe-0.7.1/src/labxpipe/steps/
+-rw-r--r--   0 build     (1000) build     (1001)      423 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     4181 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/bowtie2.py
+-rw-r--r--   0 build     (1000) build     (1001)     4152 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/bwa_mem2.py
+-rw-r--r--   0 build     (1000) build     (1001)     1431 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/cleaning.py
+-rw-r--r--   0 build     (1000) build     (1001)     2413 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/cufflinks.py
+-rw-r--r--   0 build     (1000) build     (1001)     6565 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/geneabacus.py
+-rw-r--r--   0 build     (1000) build     (1001)     4238 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/minimap2.py
+-rw-r--r--   0 build     (1000) build     (1001)     5492 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/readknead.py
+-rw-r--r--   0 build     (1000) build     (1001)     2950 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/samtools_sort.py
+-rw-r--r--   0 build     (1000) build     (1001)     3625 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/samtools_uniquify.py
+-rw-r--r--   0 build     (1000) build     (1001)     3235 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/steps/star.py
+-rw-r--r--   0 build     (1000) build     (1001)     8654 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/trackhub.py
+-rw-r--r--   0 build     (1000) build     (1001)     1739 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe/utils.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:30.998725 labxpipe-0.7.1/src/labxpipe.egg-info/
+-rw-r--r--   0 build     (1000) build     (1001)    17025 2023-08-01 22:43:30.000000 labxpipe-0.7.1/src/labxpipe.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)     1906 2023-08-01 22:43:30.000000 labxpipe-0.7.1/src/labxpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1001)        1 2023-08-01 22:43:30.000000 labxpipe-0.7.1/src/labxpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1001)       56 2023-08-01 22:43:30.000000 labxpipe-0.7.1/src/labxpipe.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1001)       44 2023-08-01 22:43:30.000000 labxpipe-0.7.1/src/labxpipe.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1001)       26 2023-08-01 22:43:30.000000 labxpipe-0.7.1/src/labxpipe.egg-info/top_level.txt
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-01 22:43:31.005391 labxpipe-0.7.1/src/labxpipe_scripts/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/__init__.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     2440 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    15493 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_demultiplex.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     7819 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_extract.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     7704 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_generate.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    17821 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_merge_count.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     4243 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_profile.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    13924 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_report.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    17321 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_run.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    21424 2023-08-01 22:42:38.000000 labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_trackhub.py
```

### Comparing `labxpipe-0.7.0/.sourcehut/arch.yml` & `labxpipe-0.7.1/.sourcehut/arch.yml`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/LICENSE` & `labxpipe-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/PKG-INFO` & `labxpipe-0.7.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labxpipe
-Version: 0.7.0
+Version: 0.7.1
 Summary: Genomics pipelines
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: homepage, https://git.sr.ht/~vejnar/LabxPipe
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,19 +24,21 @@
 
 ## Examples
 
 See JSON files in `config/pipelines` of this repository.
 
 | Pipeline JSON file            |                                                                                                                           |
 | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
-| `mrna_seq.json`               | mRNA-seq                                                                                                                  |
-| `mrna_seq_no_db.json`         | mRNA-seq. No [LabxDB](https://labxdb.vejnar.org)                                                                          |
-| `mrna_seq_with_plotting.json` | mRNA-seq. Plotting non-mapped reads. Demonstrate `step_input`                                                             |
-| `mrna_seq_cufflinks.json`     | mRNA-seq. Replaces GeneAbacus by Cufflinks                                                                                |
-| `chip_seq.json`               | ChIP-seq using [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads. |
+| `mrna_seq.json`               | mRNA-seq.                                                                                                                 |
+| `mrna_seq_profiling_bam.json` | mRNA-seq. Genomic coverage profiles using [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus). BAM and SAM outputs.            |
+| `mrna_seq_no_db.json`         | mRNA-seq. No [LabxDB](https://labxdb.vejnar.org).                                                                         |
+| `mrna_seq_with_plotting.json` | mRNA-seq. Plotting non-mapped reads. Demonstrate `step_input`.                                                            |
+| `mrna_seq_cufflinks.json`     | mRNA-seq. Replaces GeneAbacus by Cufflinks.                                                                               |
+| `chip_seq.json`               | ChIP-seq. [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads.      |
+| `chip_seq_user_function.json` | ChIP-seq. [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads. Genomic coverage profiles using [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus). Peak-calling using [MACS3](https://github.com/macs3-project/MACS) employing a *user-defined step/function*. |
 
 Following demonstrates how to apply `mrna_seq.json` pipeline. It requires:
 * [LabxDB](https://labxdb.vejnar.org)
 * FASTQ files for sample named `AGR000850` and `AGR000912`
     ```
     /plus/data/seq/by_run/AGR000850
     ├── 23_009_R1.fastq.zst
@@ -62,20 +64,36 @@
     ```
     Output is written in `path_output` directory.
 2. Create report:
     ```bash
     lxpipe report --pipeline mrna_seq.json
     ```
     Report file `mrna_seq.xlsx` should be created in same directory as `mrna_seq.json`.
-3. Merge gene/mRNA counts generated by [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus) in `counting` directory:
+3. Extract output file(s) to use them directly, for instance to load them in IGV. For example:
+    * To extract BAM files and rename them using the sample label:
+        ```bash
+        lxpipe extract --pipeline mrna_seq.json \
+                       --files aligning,accepted_hits.sam.zst \
+                       --label
+        ```
+    * To extract BigWig profile files and rename them using the sample label and reference in addition to the original filename used as filename suffix:
+        ```bash
+        lxpipe extract --pipeline mrna_seq.json \
+                       --files profiling,genome_plus.bw \
+                       --label \
+                       --reference \
+                       --suffix
+        ```
+    Use `-d`/`--dry_run` to test the extract command before applying it.
+4. Merge gene/mRNA counts generated by [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus) in `counting` directory:
     ```bash
     lxpipe merge-count --pipeline mrna_seq.json \
                        --step counting
     ```
-4. Trackhub. Requirements:
+5. Create a trackhub. Requirements:
     * [ChromosomeMappings](https://github.com/dpryan79/ChromosomeMappings) file (to map chromosome names from Ensembl/NCBI to UCSC)
     * Tabulated file (with chromosome name and length)
 
     Execute in a separate directory:
     ```bash
     lxpipe trackhub --runs AGR000850,AGR000912 \
                     --species_ucsc danRer11 \
@@ -96,126 +114,184 @@
 
 ## Writing pipelines
 
 Parameters are defined first globally (see above), then per pipeline, then per replicate/run, and then per step/function. The latest definition takes precedence: `path_seq_run` defined in `/etc/hts/labxpipe.json` is used by default, but if `path_seq_run` is defined in the pipeline file, it will be used instead.
 
 Main parameters
 
-| Parameter          | Type          |
-| ------------------ | ------------- |
-| name               | string        |
-| path_output        | string        |
-| path_seq_run       | string        |
-| path_annots        | string        |
-| path_bowtie2_index | string        |
-| path_star_index    | string        |
-| fastq_exts         | []strings     |
-| adaptors           | {}            |
-| logging_level      | string        |
-| run_refs           | []strings     |
-| replicate_refs     | []strings     |
-| ref_info_source    | []strings     |
-| ref_infos          | {}            |
-| analysis           | [{}, {}, ...] |
+| Parameter           | Type          |
+| ------------------- | ------------- |
+| name                | string        |
+| path_output         | string        |
+| path_seq_run        | string        |
+| path_local_steps    | string        |
+| path_annots         | string        |
+| path_bowtie2_index  | string        |
+| path_bwa-mem2_index | string        |
+| path_minimap2_index | string        |
+| path_star_index     | string        |
+| fastq_exts          | []strings     |
+| adaptors            | {}            |
+| logging_level       | string        |
+| run_refs            | []strings     |
+| replicate_refs      | []strings     |
+| ref_info_source     | []strings     |
+| ref_infos           | {}            |
+| analysis            | [{}, {}, ...] |
 
-Parameters for all functions
+Parameters for all steps
 
 | Parameter     | Type    |
 | ------------- | ------- |
 | step_name     | string  |
 | step_function | string  |
 | step_desc     | string  |
 | force         | boolean |
 
-Function-specific parameters
+Step-specific parameters
 
-| Function           | Synonym          | Parameter             | Type          |
+| Step               | Synonym          | Parameter             | Type          |
 | ------------------ | ---------------- | --------------------- | ------------- |
 | readknead          | preparing        | options               | []strings     |
 |                    |                  | ops_r1                | [{}, {}, ...] |
 |                    |                  | ops_r2                | [{}, {}, ...] |
 |                    |                  | plot_fastq_in         | boolean       |
 |                    |                  | plot_fastq            | boolean       |
 |                    |                  | fastq_out             | boolean       |
 |                    |                  | zip_fastq_out         | string        |
 | bowtie2            | genomic_aligning | options               | []strings     |
 |                    |                  | index                 | string        |
 |                    |                  | output                | string        |
 |                    |                  | output_unfiltered     | string        |
 |                    |                  | compress_sam          | boolean       |
 |                    |                  | compress_sam_cmd      | string        |
-|                    |                  | create_bam            | boolean       |
-|                    |                  | index_bam             | boolean       |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
+| bwa-mem2           |                  | options               | []strings     |
+|                    |                  | index                 | string        |
+|                    |                  | output                | string        |
+|                    |                  | compress_output       | boolean       |
+|                    |                  | compress_output_cmd   | string        |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
+| minimap2           |                  | options               | []strings     |
+|                    |                  | index                 | string        |
+|                    |                  | output                | string        |
+|                    |                  | compress_output       | boolean       |
+|                    |                  | compress_output_cmd   | string        |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
 | star               | aligning         | options               | []strings     |
 |                    |                  | index                 | string        |
 |                    |                  | output_type           | []strings     |
 |                    |                  | compress_sam          | boolean       |
 |                    |                  | compress_sam_cmd      | string        |
 |                    |                  | compress_unmapped     | boolean       |
 |                    |                  | compress_unmapped_cmd | string        |
 | cufflinks          |                  | options               | []strings     |
 |                    |                  | inputs                | [{}, {}, ...] |
 |                    |                  | features              | [{}, {}, ...] |
 | geneabacus         | counting         | options               | []strings     |
 |                    |                  | inputs                | [{}, {}, ...] |
+|                    |                  | path_annots           | string        |
 |                    |                  | features              | [{}, {}, ...] |
-| uniquify           |                  | options               | []strings     |
+| samtools_sort      |                  | options               | []strings     |
+|                    |                  | sort_by_name_bam      | boolean       |
+| samtools_uniquify  |                  | options               | []strings     |
 |                    |                  | sort_by_name_bam      | boolean       |
 |                    |                  | index_bam             | boolean       |
 | cleaning           |                  | steps                 | [{}, {}, ...] |
 
-Sample-specific parameters. Automatically populated if using LabxDB or sourced from `ref_infos`. These parameters can be changed manually in any function (for example setting `paired` to `False` will ignore second reads in that step).
+◆ indicates exclusive options. For example, either `create_bam` or `index_bam` can be used, but not both.
+
+Sample-specific parameters. Automatically populated if using LabxDB or sourced from `ref_infos`. These parameters can be changed manually in any step (for example setting `paired` to `false` will ignore second reads in that step).
 
 | Parameter      | Type    |
 | -------------- | ------- |
 | label_short    | string  |
 | paired         | boolean |
 | directional    | boolean |
 | r1_strand      | string  |
 | quality_scores | string  |
 
+## User-defined step
+
+In addition to the provided steps/functions, i.e. `bowtie2`, `star` or `geneabacus`, users can defined their own step, usable in the LabxPipe pipelines. LabxPipe will import user-defined steps:
+* Written in Python
+* One step per file with the `.py` extension located in the directory defined by `path_local_steps`
+* Each step defined in individual file requires:
+    1. A `functions` variable listing the step name(s)
+    2. A function named `run` with the 3 parameters `path_in`, `path_out` and `params`
+
+    For example:
+    ```python
+    functions = ['macs3']
+    def run(path_in, path_out, params):
+        ...
+    ```
+
+Example of a user-defined function providing peak-calling using [MACS3](https://github.com/macs3-project/MACS) is available in `config/user_steps/macs3.py` in this repository.
+
+Example of a pipeline using the [MACS3](https://github.com/macs3-project/MACS) step is available in `config/pipelines/chip_seq_user_function.json` in this repository.
+
 ## Demultiplexing sequencing reads: `lxpipe demultiplex`
 
 * Demultiplex reads based on barcode sequences from the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org)
 * Demultiplexing using [ReadKnead](https://sr.ht/~vejnar/ReadKnead). The most important for demultiplexing is the ReadKnead pipeline. Pipelines are identified using the `Adapter 3'` field in LabxDB.
 
 * Example for simple demultiplexing. The first nucleotides at the 5' end of read 1 are used as barcodes (the `Adapter 3'` field is set to `sRNA 1.5` in LabxDB for these samples) with the following pipeline:
     ```json
     {
         "sRNA 1.5": {
-            "R1": [{"name": "demultiplex",
+            "R1": [
+                {
+                    "name": "demultiplex",
                     "end": 5,
-                    "max_mismatch": 1}],
+                    "max_mismatch": 1
+                }
+            ],
             "R2": null
         }
     }
     ```
     The barcode sequences are added by LabxPipe using the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org).
 
 * Example for iCLIP demultiplexing. In [Vejnar et al.](https://pubmed.ncbi.nlm.nih.gov/31227602), iCLIP is demultiplexed (the `Adapter 3'` field is set to `TruSeq-DMS+A Index` in LabxDB for these samples) using the following pipeline:
     ```json
     {
         "TruSeq-DMS+A Index": {
-            "R1": [{"name": "clip",
+            "R1": [
+                {
+                    "name": "clip",
                     "end": 5,
                     "length": 4,
-                    "add_clipped": true},
-                {"name": "trim",
-                 "end": 3,
-                 "algo": "bktrim",
-                 "min_sequence": 5,
-                 "keep": ["trim_exact", "trim_align"]},
-                {"name": "length",
-                 "min_length": 6},
-                {"name": "demultiplex",
-                 "end": 3,
-                 "max_mismatch": 1,
-                 "length_ligand": 2},
-                {"name": "length",
-                 "min_length": 15}],
+                    "add_clipped": true
+                },
+                {
+                    "name": "trim",
+                    "end": 3,
+                    "algo": "bktrim",
+                    "min_sequence": 5,
+                    "keep": ["trim_exact", "trim_align"]
+                },
+                {
+                    "name": "length",
+                    "min_length": 6
+                },
+                {
+                    "name": "demultiplex",
+                    "end": 3,
+                    "max_mismatch": 1,
+                    "length_ligand": 2
+                },
+                {
+                    "name": "length",
+                    "min_length": 15
+                }
+            ],
             "R2": null
         }
     }
     ```
     Pipeline is stored in `demux_truseq_dms_a.json`. The barcode sequences are added by LabxPipe using the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org). (NB: published demultiplexed data were generated using `"algo": "align"` with a minimum score of 80 instead of `"algo": "bktrim"`)
 
     Then pipeline was tested running:
```

### Comparing `labxpipe-0.7.0/README.md` & `labxpipe-0.7.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 
 ## Examples
 
 See JSON files in `config/pipelines` of this repository.
 
 | Pipeline JSON file            |                                                                                                                           |
 | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
-| `mrna_seq.json`               | mRNA-seq                                                                                                                  |
-| `mrna_seq_no_db.json`         | mRNA-seq. No [LabxDB](https://labxdb.vejnar.org)                                                                          |
-| `mrna_seq_with_plotting.json` | mRNA-seq. Plotting non-mapped reads. Demonstrate `step_input`                                                             |
-| `mrna_seq_cufflinks.json`     | mRNA-seq. Replaces GeneAbacus by Cufflinks                                                                                |
-| `chip_seq.json`               | ChIP-seq using [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads. |
+| `mrna_seq.json`               | mRNA-seq.                                                                                                                 |
+| `mrna_seq_profiling_bam.json` | mRNA-seq. Genomic coverage profiles using [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus). BAM and SAM outputs.            |
+| `mrna_seq_no_db.json`         | mRNA-seq. No [LabxDB](https://labxdb.vejnar.org).                                                                         |
+| `mrna_seq_with_plotting.json` | mRNA-seq. Plotting non-mapped reads. Demonstrate `step_input`.                                                            |
+| `mrna_seq_cufflinks.json`     | mRNA-seq. Replaces GeneAbacus by Cufflinks.                                                                               |
+| `chip_seq.json`               | ChIP-seq. [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads.      |
+| `chip_seq_user_function.json` | ChIP-seq. [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads. Genomic coverage profiles using [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus). Peak-calling using [MACS3](https://github.com/macs3-project/MACS) employing a *user-defined step/function*. |
 
 Following demonstrates how to apply `mrna_seq.json` pipeline. It requires:
 * [LabxDB](https://labxdb.vejnar.org)
 * FASTQ files for sample named `AGR000850` and `AGR000912`
     ```
     /plus/data/seq/by_run/AGR000850
     ├── 23_009_R1.fastq.zst
@@ -51,20 +53,36 @@
     ```
     Output is written in `path_output` directory.
 2. Create report:
     ```bash
     lxpipe report --pipeline mrna_seq.json
     ```
     Report file `mrna_seq.xlsx` should be created in same directory as `mrna_seq.json`.
-3. Merge gene/mRNA counts generated by [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus) in `counting` directory:
+3. Extract output file(s) to use them directly, for instance to load them in IGV. For example:
+    * To extract BAM files and rename them using the sample label:
+        ```bash
+        lxpipe extract --pipeline mrna_seq.json \
+                       --files aligning,accepted_hits.sam.zst \
+                       --label
+        ```
+    * To extract BigWig profile files and rename them using the sample label and reference in addition to the original filename used as filename suffix:
+        ```bash
+        lxpipe extract --pipeline mrna_seq.json \
+                       --files profiling,genome_plus.bw \
+                       --label \
+                       --reference \
+                       --suffix
+        ```
+    Use `-d`/`--dry_run` to test the extract command before applying it.
+4. Merge gene/mRNA counts generated by [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus) in `counting` directory:
     ```bash
     lxpipe merge-count --pipeline mrna_seq.json \
                        --step counting
     ```
-4. Trackhub. Requirements:
+5. Create a trackhub. Requirements:
     * [ChromosomeMappings](https://github.com/dpryan79/ChromosomeMappings) file (to map chromosome names from Ensembl/NCBI to UCSC)
     * Tabulated file (with chromosome name and length)
 
     Execute in a separate directory:
     ```bash
     lxpipe trackhub --runs AGR000850,AGR000912 \
                     --species_ucsc danRer11 \
@@ -85,126 +103,184 @@
 
 ## Writing pipelines
 
 Parameters are defined first globally (see above), then per pipeline, then per replicate/run, and then per step/function. The latest definition takes precedence: `path_seq_run` defined in `/etc/hts/labxpipe.json` is used by default, but if `path_seq_run` is defined in the pipeline file, it will be used instead.
 
 Main parameters
 
-| Parameter          | Type          |
-| ------------------ | ------------- |
-| name               | string        |
-| path_output        | string        |
-| path_seq_run       | string        |
-| path_annots        | string        |
-| path_bowtie2_index | string        |
-| path_star_index    | string        |
-| fastq_exts         | []strings     |
-| adaptors           | {}            |
-| logging_level      | string        |
-| run_refs           | []strings     |
-| replicate_refs     | []strings     |
-| ref_info_source    | []strings     |
-| ref_infos          | {}            |
-| analysis           | [{}, {}, ...] |
+| Parameter           | Type          |
+| ------------------- | ------------- |
+| name                | string        |
+| path_output         | string        |
+| path_seq_run        | string        |
+| path_local_steps    | string        |
+| path_annots         | string        |
+| path_bowtie2_index  | string        |
+| path_bwa-mem2_index | string        |
+| path_minimap2_index | string        |
+| path_star_index     | string        |
+| fastq_exts          | []strings     |
+| adaptors            | {}            |
+| logging_level       | string        |
+| run_refs            | []strings     |
+| replicate_refs      | []strings     |
+| ref_info_source     | []strings     |
+| ref_infos           | {}            |
+| analysis            | [{}, {}, ...] |
 
-Parameters for all functions
+Parameters for all steps
 
 | Parameter     | Type    |
 | ------------- | ------- |
 | step_name     | string  |
 | step_function | string  |
 | step_desc     | string  |
 | force         | boolean |
 
-Function-specific parameters
+Step-specific parameters
 
-| Function           | Synonym          | Parameter             | Type          |
+| Step               | Synonym          | Parameter             | Type          |
 | ------------------ | ---------------- | --------------------- | ------------- |
 | readknead          | preparing        | options               | []strings     |
 |                    |                  | ops_r1                | [{}, {}, ...] |
 |                    |                  | ops_r2                | [{}, {}, ...] |
 |                    |                  | plot_fastq_in         | boolean       |
 |                    |                  | plot_fastq            | boolean       |
 |                    |                  | fastq_out             | boolean       |
 |                    |                  | zip_fastq_out         | string        |
 | bowtie2            | genomic_aligning | options               | []strings     |
 |                    |                  | index                 | string        |
 |                    |                  | output                | string        |
 |                    |                  | output_unfiltered     | string        |
 |                    |                  | compress_sam          | boolean       |
 |                    |                  | compress_sam_cmd      | string        |
-|                    |                  | create_bam            | boolean       |
-|                    |                  | index_bam             | boolean       |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
+| bwa-mem2           |                  | options               | []strings     |
+|                    |                  | index                 | string        |
+|                    |                  | output                | string        |
+|                    |                  | compress_output       | boolean       |
+|                    |                  | compress_output_cmd   | string        |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
+| minimap2           |                  | options               | []strings     |
+|                    |                  | index                 | string        |
+|                    |                  | output                | string        |
+|                    |                  | compress_output       | boolean       |
+|                    |                  | compress_output_cmd   | string        |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
 | star               | aligning         | options               | []strings     |
 |                    |                  | index                 | string        |
 |                    |                  | output_type           | []strings     |
 |                    |                  | compress_sam          | boolean       |
 |                    |                  | compress_sam_cmd      | string        |
 |                    |                  | compress_unmapped     | boolean       |
 |                    |                  | compress_unmapped_cmd | string        |
 | cufflinks          |                  | options               | []strings     |
 |                    |                  | inputs                | [{}, {}, ...] |
 |                    |                  | features              | [{}, {}, ...] |
 | geneabacus         | counting         | options               | []strings     |
 |                    |                  | inputs                | [{}, {}, ...] |
+|                    |                  | path_annots           | string        |
 |                    |                  | features              | [{}, {}, ...] |
-| uniquify           |                  | options               | []strings     |
+| samtools_sort      |                  | options               | []strings     |
+|                    |                  | sort_by_name_bam      | boolean       |
+| samtools_uniquify  |                  | options               | []strings     |
 |                    |                  | sort_by_name_bam      | boolean       |
 |                    |                  | index_bam             | boolean       |
 | cleaning           |                  | steps                 | [{}, {}, ...] |
 
-Sample-specific parameters. Automatically populated if using LabxDB or sourced from `ref_infos`. These parameters can be changed manually in any function (for example setting `paired` to `False` will ignore second reads in that step).
+◆ indicates exclusive options. For example, either `create_bam` or `index_bam` can be used, but not both.
+
+Sample-specific parameters. Automatically populated if using LabxDB or sourced from `ref_infos`. These parameters can be changed manually in any step (for example setting `paired` to `false` will ignore second reads in that step).
 
 | Parameter      | Type    |
 | -------------- | ------- |
 | label_short    | string  |
 | paired         | boolean |
 | directional    | boolean |
 | r1_strand      | string  |
 | quality_scores | string  |
 
+## User-defined step
+
+In addition to the provided steps/functions, i.e. `bowtie2`, `star` or `geneabacus`, users can defined their own step, usable in the LabxPipe pipelines. LabxPipe will import user-defined steps:
+* Written in Python
+* One step per file with the `.py` extension located in the directory defined by `path_local_steps`
+* Each step defined in individual file requires:
+    1. A `functions` variable listing the step name(s)
+    2. A function named `run` with the 3 parameters `path_in`, `path_out` and `params`
+
+    For example:
+    ```python
+    functions = ['macs3']
+    def run(path_in, path_out, params):
+        ...
+    ```
+
+Example of a user-defined function providing peak-calling using [MACS3](https://github.com/macs3-project/MACS) is available in `config/user_steps/macs3.py` in this repository.
+
+Example of a pipeline using the [MACS3](https://github.com/macs3-project/MACS) step is available in `config/pipelines/chip_seq_user_function.json` in this repository.
+
 ## Demultiplexing sequencing reads: `lxpipe demultiplex`
 
 * Demultiplex reads based on barcode sequences from the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org)
 * Demultiplexing using [ReadKnead](https://sr.ht/~vejnar/ReadKnead). The most important for demultiplexing is the ReadKnead pipeline. Pipelines are identified using the `Adapter 3'` field in LabxDB.
 
 * Example for simple demultiplexing. The first nucleotides at the 5' end of read 1 are used as barcodes (the `Adapter 3'` field is set to `sRNA 1.5` in LabxDB for these samples) with the following pipeline:
     ```json
     {
         "sRNA 1.5": {
-            "R1": [{"name": "demultiplex",
+            "R1": [
+                {
+                    "name": "demultiplex",
                     "end": 5,
-                    "max_mismatch": 1}],
+                    "max_mismatch": 1
+                }
+            ],
             "R2": null
         }
     }
     ```
     The barcode sequences are added by LabxPipe using the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org).
 
 * Example for iCLIP demultiplexing. In [Vejnar et al.](https://pubmed.ncbi.nlm.nih.gov/31227602), iCLIP is demultiplexed (the `Adapter 3'` field is set to `TruSeq-DMS+A Index` in LabxDB for these samples) using the following pipeline:
     ```json
     {
         "TruSeq-DMS+A Index": {
-            "R1": [{"name": "clip",
+            "R1": [
+                {
+                    "name": "clip",
                     "end": 5,
                     "length": 4,
-                    "add_clipped": true},
-                {"name": "trim",
-                 "end": 3,
-                 "algo": "bktrim",
-                 "min_sequence": 5,
-                 "keep": ["trim_exact", "trim_align"]},
-                {"name": "length",
-                 "min_length": 6},
-                {"name": "demultiplex",
-                 "end": 3,
-                 "max_mismatch": 1,
-                 "length_ligand": 2},
-                {"name": "length",
-                 "min_length": 15}],
+                    "add_clipped": true
+                },
+                {
+                    "name": "trim",
+                    "end": 3,
+                    "algo": "bktrim",
+                    "min_sequence": 5,
+                    "keep": ["trim_exact", "trim_align"]
+                },
+                {
+                    "name": "length",
+                    "min_length": 6
+                },
+                {
+                    "name": "demultiplex",
+                    "end": 3,
+                    "max_mismatch": 1,
+                    "length_ligand": 2
+                },
+                {
+                    "name": "length",
+                    "min_length": 15
+                }
+            ],
             "R2": null
         }
     }
     ```
     Pipeline is stored in `demux_truseq_dms_a.json`. The barcode sequences are added by LabxPipe using the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org). (NB: published demultiplexed data were generated using `"algo": "align"` with a minimum score of 80 instead of `"algo": "bktrim"`)
 
     Then pipeline was tested running:
```

### Comparing `labxpipe-0.7.0/config/labxpipe.json` & `labxpipe-0.7.1/config/labxpipe.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/config/labxpipe_trackhub.json` & `labxpipe-0.7.1/config/labxpipe_trackhub.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/config/pipelines/chip_seq.json` & `labxpipe-0.7.1/config/pipelines/chip_seq.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999311067019401%*

 * *Differences: {"'analysis'": "{0: {'ops_r1': {1: {'keep': {insert: [(2, 'no_trim')], delete: [0]}, delete: "*

 * *               "['end']}}}}"}*

```diff
@@ -5,21 +5,20 @@
             "ops_r1": [
                 {
                     "base36": true,
                     "name": "rename"
                 },
                 {
                     "algo": "bktrim_paired",
-                    "end": 3,
                     "epsilon": 0.15,
                     "epsilon_indel": 0.1,
                     "keep": [
-                        "no_trim",
                         "trim_exact",
-                        "trim_align"
+                        "trim_align",
+                        "no_trim"
                     ],
                     "min_overlap": 2,
                     "name": "trim",
                     "sequence": "AGATCGGAAGAGCACACGTCTGAACTCCAGTCA",
                     "sequence_paired": "AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGT"
                 },
                 {
```

### Comparing `labxpipe-0.7.0/config/pipelines/mrna_seq.json` & `labxpipe-0.7.1/config/pipelines/mrna_seq_with_plotting.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8403167517006802%*

 * *Differences: {"'analysis'": "{0: {'ops_r1': {1: {'keep': {insert: [(2, 'no_trim')], delete: [0]}}}}, 1: "*

 * *               "{'options': {insert: [(10, '--outReadsUnmapped'), (11, 'Fastx')]}}, 3: "*

 * *               "{'step_input': 'aligning'}, insert: [(2, OrderedDict([('step_name', 'plotting'), "*

 * *               "('step_function', 'readknead'), ('step_desc', 'Plotting.'), ('force', False), "*

 * *               "('fastq_out', False), ('plot_fastq_in', True), ('plot_fastq', False)]))]}",*

 * * "'name'": "'mrna_seq_with_plotting'",*

 * * "'p […]*

```diff
@@ -8,17 +8,17 @@
                     "name": "rename"
                 },
                 {
                     "algo": "bktrim_paired",
                     "epsilon": 0.15,
                     "epsilon_indel": 0.1,
                     "keep": [
-                        "no_trim",
                         "trim_exact",
-                        "trim_align"
+                        "trim_align",
+                        "no_trim"
                     ],
                     "name": "trim",
                     "sequence": "AGATCGGAAGAGCACACGTCTGAACTCCAGTCAC",
                     "sequence_paired": "AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGTA"
                 },
                 {
                     "min_length": 20,
@@ -42,24 +42,35 @@
                 "--alignEndsType",
                 "Local",
                 "--sjdbScore",
                 "2",
                 "--outFilterMultimapNmax",
                 "1000",
                 "--outMultimapperOrder",
-                "Random"
+                "Random",
+                "--outReadsUnmapped",
+                "Fastx"
             ],
             "output_type": [
                 "SAM"
             ],
             "step_desc": "Aligning reads to mRNAs.",
             "step_function": "star",
             "step_name": "aligning"
         },
         {
+            "fastq_out": false,
+            "force": false,
+            "plot_fastq": false,
+            "plot_fastq_in": true,
+            "step_desc": "Plotting.",
+            "step_function": "readknead",
+            "step_name": "plotting"
+        },
+        {
             "features": [
                 {
                     "fon_name": "transcript_stable_id",
                     "name": "transcript_all",
                     "path_json": "danrer_cdna_all_ensembl104.fon1.json",
                     "read_min_overlap": 10
                 },
@@ -75,14 +86,15 @@
                 {
                     "fname": "accepted_hits.sam.zst",
                     "step": "aligning",
                     "type": "sam"
                 }
             ],
             "step_desc": "Counts for genes and transcripts.",
+            "step_input": "aligning",
             "step_name": "counting"
         },
         {
             "force": false,
             "step_desc": "Remove intermediate files",
             "step_name": "cleaning",
             "steps": [
@@ -90,16 +102,16 @@
                     "pattern": "*.fastq.lz4",
                     "step_name": "preparing"
                 }
             ]
         }
     ],
     "logging_level": "info",
-    "name": "mrna_seq",
+    "name": "mrna_seq_with_plotting",
     "path_bowtie2_index": "/plus/scratch/sai/bowtie2_indices",
-    "path_output": "/plus/scratch/users/charles/labxpipe/mrna_seq",
+    "path_output": "/plus/scratch/users/charles/labxpipe/mrna_seq_with_plotting",
     "path_star_index": "/plus/scratch/sai/star_indices",
     "run_refs": [
         "AGR000850",
         "AGR000912"
     ]
 }
```

### Comparing `labxpipe-0.7.0/config/pipelines/mrna_seq_cufflinks.json` & `labxpipe-0.7.1/config/pipelines/mrna_seq_cufflinks.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984986181972789%*

 * *Differences: {"'analysis'": "{0: {'ops_r1': {1: {'keep': {insert: [(2, 'no_trim')], delete: [0]}}}}, 1: "*

 * *               "{'index': 'danrer_genome_all_cdna_all_ensembl108_grcz11_sjdboverhang75'}, 2: "*

 * *               "{'features': {0: {'path_gff3': 'danrer_cdna_all_ensembl108.gff3'}}}}"}*

```diff
@@ -8,17 +8,17 @@
                     "name": "rename"
                 },
                 {
                     "algo": "bktrim_paired",
                     "epsilon": 0.15,
                     "epsilon_indel": 0.1,
                     "keep": [
-                        "no_trim",
                         "trim_exact",
-                        "trim_align"
+                        "trim_align",
+                        "no_trim"
                     ],
                     "name": "trim",
                     "sequence": "AGATCGGAAGAGCACACGTCTGAACTCCAGTCAC",
                     "sequence_paired": "AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGTA"
                 },
                 {
                     "min_length": 20,
@@ -31,15 +31,15 @@
             "step_function": "readknead",
             "step_name": "preparing",
             "zip_fastq_out": "lz4"
         },
         {
             "compress_sam": false,
             "force": false,
-            "index": "danrer_genome_all_cdna_all_ensembl104_grcz11_sjdboverhang75",
+            "index": "danrer_genome_all_cdna_all_ensembl108_grcz11_sjdboverhang75",
             "options": [
                 "--readMapNumber",
                 "1000000",
                 "--alignEndsType",
                 "Local",
                 "--sjdbScore",
                 "2",
@@ -56,15 +56,15 @@
             "step_function": "star",
             "step_name": "aligning"
         },
         {
             "features": [
                 {
                     "name": "transcript_all",
-                    "path_gff3": "danrer_cdna_all_ensembl106.gff3"
+                    "path_gff3": "danrer_cdna_all_ensembl108.gff3"
                 }
             ],
             "force": false,
             "inputs": [
                 {
                     "fname": "accepted_hits.bam",
                     "step": "aligning",
```

### Comparing `labxpipe-0.7.0/config/pipelines/mrna_seq_no_db.json` & `labxpipe-0.7.1/config/pipelines/mrna_seq_no_db.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999915449134199%*

 * *Differences: {"'analysis'": "{0: {'ops_r1': {1: {'keep': {insert: [(2, 'no_trim')], delete: [0]}}}}}"}*

```diff
@@ -8,17 +8,17 @@
                     "name": "rename"
                 },
                 {
                     "algo": "bktrim_paired",
                     "epsilon": 0.15,
                     "epsilon_indel": 0.1,
                     "keep": [
-                        "no_trim",
                         "trim_exact",
-                        "trim_align"
+                        "trim_align",
+                        "no_trim"
                     ],
                     "name": "trim",
                     "sequence": "AGATCGGAAGAGCACACGTCTGAACTCCAGTCAC",
                     "sequence_paired": "AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGTA"
                 },
                 {
                     "min_length": 20,
```

### Comparing `labxpipe-0.7.0/config/pipelines/mrna_seq_with_plotting.json` & `labxpipe-0.7.1/config/pipelines/mrna_seq.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8388924319727892%*

 * *Differences: {"'analysis'": "{0: {'ops_r1': {1: {'keep': {insert: [(2, 'no_trim')], delete: [0]}}}}, 1: "*

 * *               "{'index': 'danrer_genome_all_cdna_all_ensembl108_grcz11_sjdboverhang75', "*

 * *               "'options': {insert: [(2, '--readMapNumber'), (3, '1000000')], delete: [11, 10, 1, "*

 * *               "0]}}, 2: {'features': {0: {'name': 'transcript', 'path_json': "*

 * *               "'danrer_cdna_all_ensembl108.fon1.json.zst'}, 1: {'name': 'gene', 'path_json': "*

 * *               "'danrer_cdna_union2gene_all_ensembl1 […]*

```diff
@@ -8,17 +8,17 @@
                     "name": "rename"
                 },
                 {
                     "algo": "bktrim_paired",
                     "epsilon": 0.15,
                     "epsilon_indel": 0.1,
                     "keep": [
-                        "no_trim",
                         "trim_exact",
-                        "trim_align"
+                        "trim_align",
+                        "no_trim"
                     ],
                     "name": "trim",
                     "sequence": "AGATCGGAAGAGCACACGTCTGAACTCCAGTCAC",
                     "sequence_paired": "AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGTA"
                 },
                 {
                     "min_length": 20,
@@ -31,70 +31,58 @@
             "step_function": "readknead",
             "step_name": "preparing",
             "zip_fastq_out": "lz4"
         },
         {
             "compress_sam": true,
             "force": false,
-            "index": "danrer_genome_all_cdna_all_ensembl104_grcz11_sjdboverhang75",
+            "index": "danrer_genome_all_cdna_all_ensembl108_grcz11_sjdboverhang75",
             "options": [
-                "--readMapNumber",
-                "1000000",
                 "--alignEndsType",
                 "Local",
+                "--readMapNumber",
+                "1000000",
                 "--sjdbScore",
                 "2",
                 "--outFilterMultimapNmax",
                 "1000",
                 "--outMultimapperOrder",
-                "Random",
-                "--outReadsUnmapped",
-                "Fastx"
+                "Random"
             ],
             "output_type": [
                 "SAM"
             ],
             "step_desc": "Aligning reads to mRNAs.",
             "step_function": "star",
             "step_name": "aligning"
         },
         {
-            "fastq_out": false,
-            "force": false,
-            "plot_fastq": false,
-            "plot_fastq_in": true,
-            "step_desc": "Plotting.",
-            "step_function": "readknead",
-            "step_name": "plotting"
-        },
-        {
             "features": [
                 {
                     "fon_name": "transcript_stable_id",
-                    "name": "transcript_all",
-                    "path_json": "danrer_cdna_all_ensembl104.fon1.json",
+                    "name": "transcript",
+                    "path_json": "danrer_cdna_all_ensembl108.fon1.json.zst",
                     "read_min_overlap": 10
                 },
                 {
                     "fon_name": "gene_stable_id",
-                    "name": "gene_all",
-                    "path_json": "danrer_cdna_union2gene_all_ensembl104.fon1.json",
+                    "name": "gene",
+                    "path_json": "danrer_cdna_union2gene_all_ensembl108.fon1.json.zst",
                     "read_min_overlap": 10
                 }
             ],
             "force": false,
             "inputs": [
                 {
                     "fname": "accepted_hits.sam.zst",
                     "step": "aligning",
                     "type": "sam"
                 }
             ],
             "step_desc": "Counts for genes and transcripts.",
-            "step_input": "aligning",
             "step_name": "counting"
         },
         {
             "force": false,
             "step_desc": "Remove intermediate files",
             "step_name": "cleaning",
             "steps": [
@@ -102,16 +90,16 @@
                     "pattern": "*.fastq.lz4",
                     "step_name": "preparing"
                 }
             ]
         }
     ],
     "logging_level": "info",
-    "name": "mrna_seq_with_plotting",
+    "name": "mrna_seq",
     "path_bowtie2_index": "/plus/scratch/sai/bowtie2_indices",
-    "path_output": "/plus/scratch/users/charles/labxpipe/mrna_seq_with_plotting",
+    "path_output": "/plus/scratch/users/charles/labxpipe/mrna_seq",
     "path_star_index": "/plus/scratch/sai/star_indices",
     "run_refs": [
         "AGR000850",
         "AGR000912"
     ]
 }
```

### Comparing `labxpipe-0.7.0/img/logo.svg` & `labxpipe-0.7.1/img/logo.svg`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/pyproject.toml` & `labxpipe-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bg2bw.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_bg2bw.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bowtie2.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_bowtie2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bwa_mem2.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_bwa_mem2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_cufflinks.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_cufflinks.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_geneabacus.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_geneabacus.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_minimap2.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_minimap2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_readknead.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_readknead.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_samtools.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_samtools.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_star.py` & `labxpipe-0.7.1/src/labxpipe/interfaces/if_exe_star.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/parallel_helpers.py` & `labxpipe-0.7.1/src/labxpipe/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/bowtie2.py` & `labxpipe-0.7.1/src/labxpipe/steps/bowtie2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/bwa_mem2.py` & `labxpipe-0.7.1/src/labxpipe/steps/bwa_mem2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/cleaning.py` & `labxpipe-0.7.1/src/labxpipe/steps/cleaning.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/cufflinks.py` & `labxpipe-0.7.1/src/labxpipe/steps/cufflinks.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/geneabacus.py` & `labxpipe-0.7.1/src/labxpipe/steps/geneabacus.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/minimap2.py` & `labxpipe-0.7.1/src/labxpipe/steps/minimap2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/readknead.py` & `labxpipe-0.7.1/src/labxpipe/steps/readknead.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/samtools_sort.py` & `labxpipe-0.7.1/src/labxpipe/steps/samtools_sort.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/samtools_uniquify.py` & `labxpipe-0.7.1/src/labxpipe/steps/samtools_uniquify.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/steps/star.py` & `labxpipe-0.7.1/src/labxpipe/steps/star.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/trackhub.py` & `labxpipe-0.7.1/src/labxpipe/trackhub.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe/utils.py` & `labxpipe-0.7.1/src/labxpipe/utils.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe.egg-info/PKG-INFO` & `labxpipe-0.7.1/src/labxpipe.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labxpipe
-Version: 0.7.0
+Version: 0.7.1
 Summary: Genomics pipelines
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: homepage, https://git.sr.ht/~vejnar/LabxPipe
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,19 +24,21 @@
 
 ## Examples
 
 See JSON files in `config/pipelines` of this repository.
 
 | Pipeline JSON file            |                                                                                                                           |
 | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
-| `mrna_seq.json`               | mRNA-seq                                                                                                                  |
-| `mrna_seq_no_db.json`         | mRNA-seq. No [LabxDB](https://labxdb.vejnar.org)                                                                          |
-| `mrna_seq_with_plotting.json` | mRNA-seq. Plotting non-mapped reads. Demonstrate `step_input`                                                             |
-| `mrna_seq_cufflinks.json`     | mRNA-seq. Replaces GeneAbacus by Cufflinks                                                                                |
-| `chip_seq.json`               | ChIP-seq using [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads. |
+| `mrna_seq.json`               | mRNA-seq.                                                                                                                 |
+| `mrna_seq_profiling_bam.json` | mRNA-seq. Genomic coverage profiles using [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus). BAM and SAM outputs.            |
+| `mrna_seq_no_db.json`         | mRNA-seq. No [LabxDB](https://labxdb.vejnar.org).                                                                         |
+| `mrna_seq_with_plotting.json` | mRNA-seq. Plotting non-mapped reads. Demonstrate `step_input`.                                                            |
+| `mrna_seq_cufflinks.json`     | mRNA-seq. Replaces GeneAbacus by Cufflinks.                                                                               |
+| `chip_seq.json`               | ChIP-seq. [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads.      |
+| `chip_seq_user_function.json` | ChIP-seq. [Bowtie2](https://github.com/BenLangmead/bowtie2) and [Samtools](http://www.htslib.org) to uniquify reads. Genomic coverage profiles using [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus). Peak-calling using [MACS3](https://github.com/macs3-project/MACS) employing a *user-defined step/function*. |
 
 Following demonstrates how to apply `mrna_seq.json` pipeline. It requires:
 * [LabxDB](https://labxdb.vejnar.org)
 * FASTQ files for sample named `AGR000850` and `AGR000912`
     ```
     /plus/data/seq/by_run/AGR000850
     ├── 23_009_R1.fastq.zst
@@ -62,20 +64,36 @@
     ```
     Output is written in `path_output` directory.
 2. Create report:
     ```bash
     lxpipe report --pipeline mrna_seq.json
     ```
     Report file `mrna_seq.xlsx` should be created in same directory as `mrna_seq.json`.
-3. Merge gene/mRNA counts generated by [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus) in `counting` directory:
+3. Extract output file(s) to use them directly, for instance to load them in IGV. For example:
+    * To extract BAM files and rename them using the sample label:
+        ```bash
+        lxpipe extract --pipeline mrna_seq.json \
+                       --files aligning,accepted_hits.sam.zst \
+                       --label
+        ```
+    * To extract BigWig profile files and rename them using the sample label and reference in addition to the original filename used as filename suffix:
+        ```bash
+        lxpipe extract --pipeline mrna_seq.json \
+                       --files profiling,genome_plus.bw \
+                       --label \
+                       --reference \
+                       --suffix
+        ```
+    Use `-d`/`--dry_run` to test the extract command before applying it.
+4. Merge gene/mRNA counts generated by [GeneAbacus](https://sr.ht/~vejnar/GeneAbacus) in `counting` directory:
     ```bash
     lxpipe merge-count --pipeline mrna_seq.json \
                        --step counting
     ```
-4. Trackhub. Requirements:
+5. Create a trackhub. Requirements:
     * [ChromosomeMappings](https://github.com/dpryan79/ChromosomeMappings) file (to map chromosome names from Ensembl/NCBI to UCSC)
     * Tabulated file (with chromosome name and length)
 
     Execute in a separate directory:
     ```bash
     lxpipe trackhub --runs AGR000850,AGR000912 \
                     --species_ucsc danRer11 \
@@ -96,126 +114,184 @@
 
 ## Writing pipelines
 
 Parameters are defined first globally (see above), then per pipeline, then per replicate/run, and then per step/function. The latest definition takes precedence: `path_seq_run` defined in `/etc/hts/labxpipe.json` is used by default, but if `path_seq_run` is defined in the pipeline file, it will be used instead.
 
 Main parameters
 
-| Parameter          | Type          |
-| ------------------ | ------------- |
-| name               | string        |
-| path_output        | string        |
-| path_seq_run       | string        |
-| path_annots        | string        |
-| path_bowtie2_index | string        |
-| path_star_index    | string        |
-| fastq_exts         | []strings     |
-| adaptors           | {}            |
-| logging_level      | string        |
-| run_refs           | []strings     |
-| replicate_refs     | []strings     |
-| ref_info_source    | []strings     |
-| ref_infos          | {}            |
-| analysis           | [{}, {}, ...] |
+| Parameter           | Type          |
+| ------------------- | ------------- |
+| name                | string        |
+| path_output         | string        |
+| path_seq_run        | string        |
+| path_local_steps    | string        |
+| path_annots         | string        |
+| path_bowtie2_index  | string        |
+| path_bwa-mem2_index | string        |
+| path_minimap2_index | string        |
+| path_star_index     | string        |
+| fastq_exts          | []strings     |
+| adaptors            | {}            |
+| logging_level       | string        |
+| run_refs            | []strings     |
+| replicate_refs      | []strings     |
+| ref_info_source     | []strings     |
+| ref_infos           | {}            |
+| analysis            | [{}, {}, ...] |
 
-Parameters for all functions
+Parameters for all steps
 
 | Parameter     | Type    |
 | ------------- | ------- |
 | step_name     | string  |
 | step_function | string  |
 | step_desc     | string  |
 | force         | boolean |
 
-Function-specific parameters
+Step-specific parameters
 
-| Function           | Synonym          | Parameter             | Type          |
+| Step               | Synonym          | Parameter             | Type          |
 | ------------------ | ---------------- | --------------------- | ------------- |
 | readknead          | preparing        | options               | []strings     |
 |                    |                  | ops_r1                | [{}, {}, ...] |
 |                    |                  | ops_r2                | [{}, {}, ...] |
 |                    |                  | plot_fastq_in         | boolean       |
 |                    |                  | plot_fastq            | boolean       |
 |                    |                  | fastq_out             | boolean       |
 |                    |                  | zip_fastq_out         | string        |
 | bowtie2            | genomic_aligning | options               | []strings     |
 |                    |                  | index                 | string        |
 |                    |                  | output                | string        |
 |                    |                  | output_unfiltered     | string        |
 |                    |                  | compress_sam          | boolean       |
 |                    |                  | compress_sam_cmd      | string        |
-|                    |                  | create_bam            | boolean       |
-|                    |                  | index_bam             | boolean       |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
+| bwa-mem2           |                  | options               | []strings     |
+|                    |                  | index                 | string        |
+|                    |                  | output                | string        |
+|                    |                  | compress_output       | boolean       |
+|                    |                  | compress_output_cmd   | string        |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
+| minimap2           |                  | options               | []strings     |
+|                    |                  | index                 | string        |
+|                    |                  | output                | string        |
+|                    |                  | compress_output       | boolean       |
+|                    |                  | compress_output_cmd   | string        |
+|                    |                  | create_bam◆           | boolean       |
+|                    |                  | index_bam◆            | boolean       |
 | star               | aligning         | options               | []strings     |
 |                    |                  | index                 | string        |
 |                    |                  | output_type           | []strings     |
 |                    |                  | compress_sam          | boolean       |
 |                    |                  | compress_sam_cmd      | string        |
 |                    |                  | compress_unmapped     | boolean       |
 |                    |                  | compress_unmapped_cmd | string        |
 | cufflinks          |                  | options               | []strings     |
 |                    |                  | inputs                | [{}, {}, ...] |
 |                    |                  | features              | [{}, {}, ...] |
 | geneabacus         | counting         | options               | []strings     |
 |                    |                  | inputs                | [{}, {}, ...] |
+|                    |                  | path_annots           | string        |
 |                    |                  | features              | [{}, {}, ...] |
-| uniquify           |                  | options               | []strings     |
+| samtools_sort      |                  | options               | []strings     |
+|                    |                  | sort_by_name_bam      | boolean       |
+| samtools_uniquify  |                  | options               | []strings     |
 |                    |                  | sort_by_name_bam      | boolean       |
 |                    |                  | index_bam             | boolean       |
 | cleaning           |                  | steps                 | [{}, {}, ...] |
 
-Sample-specific parameters. Automatically populated if using LabxDB or sourced from `ref_infos`. These parameters can be changed manually in any function (for example setting `paired` to `False` will ignore second reads in that step).
+◆ indicates exclusive options. For example, either `create_bam` or `index_bam` can be used, but not both.
+
+Sample-specific parameters. Automatically populated if using LabxDB or sourced from `ref_infos`. These parameters can be changed manually in any step (for example setting `paired` to `false` will ignore second reads in that step).
 
 | Parameter      | Type    |
 | -------------- | ------- |
 | label_short    | string  |
 | paired         | boolean |
 | directional    | boolean |
 | r1_strand      | string  |
 | quality_scores | string  |
 
+## User-defined step
+
+In addition to the provided steps/functions, i.e. `bowtie2`, `star` or `geneabacus`, users can defined their own step, usable in the LabxPipe pipelines. LabxPipe will import user-defined steps:
+* Written in Python
+* One step per file with the `.py` extension located in the directory defined by `path_local_steps`
+* Each step defined in individual file requires:
+    1. A `functions` variable listing the step name(s)
+    2. A function named `run` with the 3 parameters `path_in`, `path_out` and `params`
+
+    For example:
+    ```python
+    functions = ['macs3']
+    def run(path_in, path_out, params):
+        ...
+    ```
+
+Example of a user-defined function providing peak-calling using [MACS3](https://github.com/macs3-project/MACS) is available in `config/user_steps/macs3.py` in this repository.
+
+Example of a pipeline using the [MACS3](https://github.com/macs3-project/MACS) step is available in `config/pipelines/chip_seq_user_function.json` in this repository.
+
 ## Demultiplexing sequencing reads: `lxpipe demultiplex`
 
 * Demultiplex reads based on barcode sequences from the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org)
 * Demultiplexing using [ReadKnead](https://sr.ht/~vejnar/ReadKnead). The most important for demultiplexing is the ReadKnead pipeline. Pipelines are identified using the `Adapter 3'` field in LabxDB.
 
 * Example for simple demultiplexing. The first nucleotides at the 5' end of read 1 are used as barcodes (the `Adapter 3'` field is set to `sRNA 1.5` in LabxDB for these samples) with the following pipeline:
     ```json
     {
         "sRNA 1.5": {
-            "R1": [{"name": "demultiplex",
+            "R1": [
+                {
+                    "name": "demultiplex",
                     "end": 5,
-                    "max_mismatch": 1}],
+                    "max_mismatch": 1
+                }
+            ],
             "R2": null
         }
     }
     ```
     The barcode sequences are added by LabxPipe using the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org).
 
 * Example for iCLIP demultiplexing. In [Vejnar et al.](https://pubmed.ncbi.nlm.nih.gov/31227602), iCLIP is demultiplexed (the `Adapter 3'` field is set to `TruSeq-DMS+A Index` in LabxDB for these samples) using the following pipeline:
     ```json
     {
         "TruSeq-DMS+A Index": {
-            "R1": [{"name": "clip",
+            "R1": [
+                {
+                    "name": "clip",
                     "end": 5,
                     "length": 4,
-                    "add_clipped": true},
-                {"name": "trim",
-                 "end": 3,
-                 "algo": "bktrim",
-                 "min_sequence": 5,
-                 "keep": ["trim_exact", "trim_align"]},
-                {"name": "length",
-                 "min_length": 6},
-                {"name": "demultiplex",
-                 "end": 3,
-                 "max_mismatch": 1,
-                 "length_ligand": 2},
-                {"name": "length",
-                 "min_length": 15}],
+                    "add_clipped": true
+                },
+                {
+                    "name": "trim",
+                    "end": 3,
+                    "algo": "bktrim",
+                    "min_sequence": 5,
+                    "keep": ["trim_exact", "trim_align"]
+                },
+                {
+                    "name": "length",
+                    "min_length": 6
+                },
+                {
+                    "name": "demultiplex",
+                    "end": 3,
+                    "max_mismatch": 1,
+                    "length_ligand": 2
+                },
+                {
+                    "name": "length",
+                    "min_length": 15
+                }
+            ],
             "R2": null
         }
     }
     ```
     Pipeline is stored in `demux_truseq_dms_a.json`. The barcode sequences are added by LabxPipe using the `Second barcode` field in [LabxDB](https://labxdb.vejnar.org). (NB: published demultiplexed data were generated using `"algo": "align"` with a minimum score of 80 instead of `"algo": "bktrim"`)
 
     Then pipeline was tested running:
```

### Comparing `labxpipe-0.7.0/src/labxpipe.egg-info/SOURCES.txt` & `labxpipe-0.7.1/src/labxpipe.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 LICENSE
 README.md
 pyproject.toml
 .sourcehut/arch.yml
 config/labxpipe.json
 config/labxpipe_trackhub.json
 config/pipelines/chip_seq.json
+config/pipelines/chip_seq_user_function.json
 config/pipelines/mrna_seq.json
 config/pipelines/mrna_seq_cufflinks.json
 config/pipelines/mrna_seq_no_db.json
+config/pipelines/mrna_seq_profiling_bam.json
 config/pipelines/mrna_seq_with_plotting.json
+config/user_steps/macs3.py
 img/logo.svg
 src/labxpipe/__init__.py
 src/labxpipe/parallel_helpers.py
 src/labxpipe/trackhub.py
 src/labxpipe/utils.py
 src/labxpipe.egg-info/PKG-INFO
 src/labxpipe.egg-info/SOURCES.txt
```

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_demultiplex.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_demultiplex.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_extract.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 
 """Extract & rename project output files"""
 
 import argparse
 import json
 import os
+import shutil
 import sys
 
 import labxdb
 import labxpipe.utils
 
 def main(argv=None):
     if argv is None:
@@ -164,12 +165,12 @@
             tmp.add(path_out)
 
     # Move
     for path_in, path_out in moves:
         if config['dry_run']:
             print(f'Move {path_in} -> {path_out}')
         else:
-            os.rename(path_in, path_out)
+            shutil.move(path_in, path_out)
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_generate.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_generate.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_merge_count.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_merge_count.py`

 * *Files 3% similar despite different names*

```diff
@@ -281,16 +281,29 @@
                         series.append(m.loc[:,main_column])
                     else:
                         logger.warning(f'Format of {sample_ref} incorrect')
                         continue
                 count_labels.append(merge['label_short'])
                 count_sums.append(np.sum(series, axis=0))
 
+            # Uniquify labels
+            count_uniq_labels = []
+            label_counter = {}
+            for cl in count_labels:
+                if cl in label_counter:
+                    label_counter[cl] += 1
+                    new_label = f'{cl}_{label_counter[cl]}'
+                    logger.warning(f'Column {cl} not unique: renaming to {new_label}')
+                    count_uniq_labels.append(new_label)
+                else:
+                    count_uniq_labels.append(cl)
+                    label_counter[cl] = 1
+
             # Export
-            main = pd.concat([main, pd.DataFrame(np.vstack(count_sums).T, columns=count_labels)], axis=1)
+            main = pd.concat([main, pd.DataFrame(np.vstack(count_sums).T, columns=count_uniq_labels)], axis=1)
             main.to_csv(f"{run_name}_{main_column}_{feature_name}{config['suffix']}.csv", index=False)
 
             # Normalization
             if config['step_name'] == 'counting':
                 if config['spike_in_main_prefix'] != '':
                     spike_in_names = config['spike_in_names']
                     # Normalize by *Spike-in Total*
```

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_profile.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_profile.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_report.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_report.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_run.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,24 @@
 import labxdb
 
 import pyfnutils as pfu
 import pyfnutils.log
 
 import labxpipe.steps
 
-def start_pipeline(run_cmd, path_pipeline, num_processor, run_ref, replicate_ref, http_url, http_login, http_password, http_path, http_db, failing):
+def start_pipeline(run_cmd, path_pipeline, num_processor, run_ref, replicate_ref, keep_failed_runs, http_url, http_login, http_password, http_path, http_db, failing):
     if failing.is_set() == False:
         try:
             cmd = run_cmd + ['--pipeline', path_pipeline, '--processor', str(num_processor)]
             if run_ref is not None:
                 cmd.extend(['--run', run_ref])
             if replicate_ref is not None:
                 cmd.extend(['--replicate', replicate_ref])
+            if keep_failed_runs == True:
+                cmd.extend(['--keep_failed_runs'])
             if http_url is not None:
                 cmd.extend(['--http_url', http_url])
             if http_login is not None:
                 cmd.extend(['--http_login', http_login])
             if http_password is not None:
                 cmd.extend(['--http_password', http_password])
             if http_path is not None:
@@ -75,14 +77,15 @@
     # Parse arguments
     parser = argparse.ArgumentParser(prog=prog, description='Analyze sequencing expt.')
     parser.add_argument('-c', '--pipeline', dest='path_pipeline', action='store', required=True, help='Path to pipeline')
     parser.add_argument('-r', '--run', dest='run_ref', action='store', help='Run')
     parser.add_argument('-n', '--replicate', dest='replicate_ref', action='store', help='Replicate')
     parser.add_argument('-w', '--worker', dest='num_worker', action='store', type=int, default=1, help='Number of run in parallel')
     parser.add_argument('-p', '--processor', dest='num_processor', action='store', type=int, default=2, help='Number of processor per run')
+    parser.add_argument('--keep_failed_runs', dest='keep_failed_runs', action='store_true', help='Don\'t skip the failed run(s)')
     parser.add_argument('--path_config', dest='path_config', action='store', help='Path to config')
     parser.add_argument('--http_url', '--labxdb_http_url', dest='labxdb_http_url', action='store', help='Database HTTP URL')
     parser.add_argument('--http_login', '--labxdb_http_login', dest='labxdb_http_login', action='store', help='Database HTTP login')
     parser.add_argument('--http_password', '--labxdb_http_password', dest='labxdb_http_password', action='store', help='Database HTTP password')
     parser.add_argument('--http_path', '--labxdb_http_path', dest='labxdb_http_path', action='store', help='Database HTTP path')
     parser.add_argument('--http_db', '--labxdb_http_db', dest='labxdb_http_db', action='store', help='Database HTTP DB')
     args = parser.parse_args(argv_parser)
@@ -152,19 +155,19 @@
                 if 'run_refs' in config:
                     refs.extend([(i, None, i) for i in config['run_refs']])
                 if 'replicate_refs' in config:
                     refs.extend([(None, i, i) for i in config['replicate_refs']])
                 for run_ref, replicate_ref, seq_ref in refs:
                     path_json_compl = os.path.join(config['path_output'], seq_ref, 'log', config['name']+'_compl.json')
                     if is_force or not os.path.exists(path_json_compl):
-                        jobs.append([job_cmd, config['path_pipeline'], config['num_processor'], run_ref, replicate_ref, config.get('labxdb_http_url'), config.get('labxdb_http_login'), config.get('labxdb_http_password'), config.get('labxdb_http_path'), config.get('labxdb_http_db'), failing])
+                        jobs.append([job_cmd, config['path_pipeline'], config['num_processor'], run_ref, replicate_ref, config.get('keep_failed_runs'), config.get('labxdb_http_url'), config.get('labxdb_http_login'), config.get('labxdb_http_password'), config.get('labxdb_http_path'), config.get('labxdb_http_db'), failing])
                     elif os.path.exists(path_json_compl):
                         ncompl = len([s for s in json.load(open(path_json_compl)) if s['status'] == 'done'])
                         if len(config['analysis']) > ncompl:
-                            jobs.append([job_cmd, config['path_pipeline'], config['num_processor'], run_ref, replicate_ref, config.get('labxdb_http_url'), config.get('labxdb_http_login'), config.get('labxdb_http_password'), config.get('labxdb_http_path'), config.get('labxdb_http_db'), failing])
+                            jobs.append([job_cmd, config['path_pipeline'], config['num_processor'], run_ref, replicate_ref, config.get('keep_failed_runs'), config.get('labxdb_http_url'), config.get('labxdb_http_login'), config.get('labxdb_http_password'), config.get('labxdb_http_path'), config.get('labxdb_http_db'), failing])
                 # Add jobs to queue
                 fs = []
                 if len(jobs) == 0:
                     logger.info('All done')
                 else:
                     logger.info(f'Queuing {len(jobs)} job(s)')
                     for job in jobs:
@@ -252,14 +255,17 @@
             dbl = labxdb.DBLink(config.get('labxdb_http_url'), config.get('labxdb_http_login'), config.get('labxdb_http_password'), config.get('labxdb_http_path'), config.get('labxdb_http_db'))
             if 'run_ref' in config:
                 # Query: Run
                 run = dbl.get('run/get-ref/'+config['run_ref'])[0][0]
             elif 'replicate_ref' in config:
                 # Query: Get all run(s)
                 runs = dbl.post('run', {'search_criterion':['3 replicate_ref EQUAL '+config['replicate_ref']], 'sort_criterion':['3 run_order ASC'], 'limit':'ALL'})
+                # Filter failed run(s)
+                if not config['keep_failed_runs']:
+                    runs = [r for r in runs if ('failed' not in r) or ('failed' in r and r['failed'] == False)]
                 # First run as reference run
                 run = runs[0]
             # Copy-paste info to config
             for field in ['quality_scores', 'directional', 'paired', 'r1_strand', 'max_read_length']:
                 config[field] = run[field]
             # Query: Replicate
             replicate = dbl.get('replicate/get-ref/'+run['replicate_ref'])[0][0]
```

### Comparing `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_trackhub.py` & `labxpipe-0.7.1/src/labxpipe_scripts/lxpipe_trackhub.py`

 * *Files identical despite different names*

