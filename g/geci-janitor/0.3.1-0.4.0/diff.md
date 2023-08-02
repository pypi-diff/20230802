# Comparing `tmp/geci_janitor-0.3.1.tar.gz` & `tmp/geci_janitor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geci_janitor-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geci_janitor-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geci_janitor-0.3.1.tar` & `geci_janitor-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1037 2023-07-24 19:01:40.960477 geci_janitor-0.3.1/README.md
--rw-r--r--   0        0        0       81 2023-07-24 19:01:40.960477 geci_janitor-0.3.1/geci_janitor/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-24 19:01:40.960477 geci_janitor-0.3.1/geci_janitor/cli.py
--rw-r--r--   0        0        0      451 2023-07-24 19:01:40.960477 geci_janitor-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 geci_janitor-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-08-02 17:52:39.009592 geci_janitor-0.4.0/README.md
+-rw-r--r--   0        0        0       81 2023-08-02 17:52:39.009592 geci_janitor-0.4.0/geci_janitor/__init__.py
+-rw-r--r--   0        0        0     1750 2023-08-02 17:52:39.009592 geci_janitor-0.4.0/geci_janitor/cli.py
+-rw-r--r--   0        0        0      519 2023-08-02 17:52:39.009592 geci_janitor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 geci_janitor-0.4.0/PKG-INFO
```

### Comparing `geci_janitor-0.3.1/geci_janitor/cli.py` & `geci_janitor-0.4.0/geci_janitor/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,23 @@
 
 @janitor.command(help="Clean and check IG_POSICION_TRAMPAS and IG_MORFOMETRIA")
 def transform_cat_data():
     command = "docker run --rm --volume $PWD:/data islasgeci/diferencias_morfometria_posicion_trampas:latest ./src/verify_data.sh /data"
     os.system(command)
 
 
+@janitor.command()
+def weekly_effort_summary(file: str):
+    """
+    Calculate summary from IG_POSICION_TRAMPAS_{date}_clean.csv \n
+    """
+    command = f"docker run --rm --volume $PWD:/workdir/datos islasgeci/datatools:latest ./src/get_weekly_summary.sh datos/{file}"
+    os.system(command)
+
+
 @janitor.command(help="Generate tidy and weekly effort tables for socorro monthly cat data")
 def clean_socorro_week_data(week: int, data_file: str):
     command = f"docker run -v $PWD/results:/workdir/results -v $PWD:/workdir/data islasgeci/datatools bash -c 'python src/get_weekly_summary_socorro_from_excell.py {week} data/{data_file} && cambia_formato_fecha results/week_{week}.csv > results/week_{week}_iso.csv'"
     os.system(command)
     command = f"docker run -v $PWD/results:/workdir/results -v $PWD:/workdir/data islasgeci/diferencias_morfometria_posicion_trampas src/make_table_tidy.R --data results/socorro_cleaned_format.csv --salida results/tidy_{week}.csv"
     os.system(command)
```

