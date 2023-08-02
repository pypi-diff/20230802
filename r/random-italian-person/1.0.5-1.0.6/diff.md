# Comparing `tmp/random_italian_person-1.0.5.tar.gz` & `tmp/random_italian_person-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/random_italian_person-1.0.5.tar", last modified: Sun Apr  2 10:10:37 2023, max compression
+gzip compressed data, was "dist/random_italian_person-1.0.6.tar", last modified: Wed Aug  2 18:01:04 2023, max compression
```

## Comparing `random_italian_person-1.0.5.tar` & `random_italian_person-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       44 2022-11-10 12:20:47.000000 random_italian_person-1.0.5/MANIFEST.in
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5618 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5152 2023-04-02 10:09:58.000000 random_italian_person-1.0.5/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       95 2022-11-10 12:20:47.000000 random_italian_person-1.0.5/random_italian_person/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       76 2023-04-02 10:10:23.000000 random_italian_person-1.0.5/random_italian_person/__version__.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person/datasets/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)  2179738 2022-11-23 13:14:22.000000 random_italian_person-1.0.5/random_italian_person/datasets/addresses.csv
--rw-r--r--   0 lucacappelletti   (501) staff       (20)   315281 2022-11-10 12:20:47.000000 random_italian_person-1.0.5/random_italian_person/datasets/municipalities.csv
--rw-r--r--   0 lucacappelletti   (501) staff       (20)   238124 2022-11-10 12:20:47.000000 random_italian_person-1.0.5/random_italian_person/datasets/names.csv
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    26632 2022-11-10 12:20:47.000000 random_italian_person-1.0.5/random_italian_person/datasets/surnames.csv
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4182 2023-04-02 09:36:24.000000 random_italian_person-1.0.5/random_italian_person/random_italian_person.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person/utils/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       81 2022-11-10 12:20:47.000000 random_italian_person-1.0.5/random_italian_person/utils/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      572 2022-11-10 12:20:47.000000 random_italian_person-1.0.5/random_italian_person/utils/random_birthday.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5618 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      640 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      120 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       22 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/random_italian_person.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2023-04-02 10:10:37.000000 random_italian_person-1.0.5/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1813 2023-04-02 09:53:03.000000 random_italian_person-1.0.5/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       44 2022-11-10 12:20:47.000000 random_italian_person-1.0.6/MANIFEST.in
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     6455 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     5385 2023-08-02 17:56:59.000000 random_italian_person-1.0.6/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       95 2022-11-10 12:20:47.000000 random_italian_person-1.0.6/random_italian_person/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       77 2023-08-02 18:00:28.000000 random_italian_person-1.0.6/random_italian_person/__version__.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person/datasets/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)  2179738 2022-11-23 13:14:22.000000 random_italian_person-1.0.6/random_italian_person/datasets/addresses.csv
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)   315281 2022-11-10 12:20:47.000000 random_italian_person-1.0.6/random_italian_person/datasets/municipalities.csv
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)   238124 2022-11-10 12:20:47.000000 random_italian_person-1.0.6/random_italian_person/datasets/names.csv
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    26632 2022-11-10 12:20:47.000000 random_italian_person-1.0.6/random_italian_person/datasets/surnames.csv
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4630 2023-08-02 17:51:06.000000 random_italian_person-1.0.6/random_italian_person/random_italian_person.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person/utils/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       81 2022-11-10 12:20:47.000000 random_italian_person-1.0.6/random_italian_person/utils/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      572 2022-11-10 12:20:47.000000 random_italian_person-1.0.6/random_italian_person/utils/random_birthday.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     6455 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      640 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      120 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       22 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/random_italian_person.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2023-08-02 18:01:04.000000 random_italian_person-1.0.6/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1844 2023-08-02 17:53:38.000000 random_italian_person-1.0.6/setup.py
```

### Comparing `random_italian_person-1.0.5/PKG-INFO` & `random_italian_person-1.0.6/random_italian_person.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,86 @@
 Metadata-Version: 2.1
-Name: random_italian_person
-Version: 1.0.5
+Name: random-italian-person
+Version: 1.0.6
 Summary: Python package to generate an Italian person randomly.
 Home-page: https://github.com/LucaCappelletti94/random_italian_person
 Author: LucaCappelletti94
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
+Description: random_italian_person
+        =========================================================================================
+        |pip| |downloads| |github|
+        
+        Python package to generate an Italian person randomly.
+        
+        How do I install this package?
+        ----------------------------------------------
+        As usual, just download it using pip:
+        
+        .. code:: shell
+        
+            pip install random_italian_person
+        
+        
+        Usage examples
+        -----------------------------------------------
+        
+        .. code:: python
+        
+            from random_italian_person import RandomItalianPerson
+        
+            person = RandomItalianPerson()
+        
+            print(person.describe())
+            # 'Rodrigo Benedetti è nata/o a Molazzana (LU) il 1972-12-18. Ora vive a Cagliari (CA) in Via Giuseppe Garibaldi 109.'
+        
+        Generate a CSV of random italian persons
+        -----------------------------------------------
+        One of the most common usages for this library is to render
+        fake datasets for testing porposes. For instance,
+        to generate a CSV with 5 random person you can use:
+        
+        .. code:: python
+        
+            import pandas as pd
+            from random_italian_person import RandomItalianPerson
+        
+            df = pd.DataFrame([
+                RandomItalianPerson().data
+                for _ in range(5)
+            ])
+        
+        The obtained dataframe will look like:
+        
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | region                | province   | surname   | name      | sex   | birth_municipality   | birth_province   | birth_region   |   birth_cap | birth_province_code   | birthdate   | address           | house_number   |   cap | municipality   | province_code   | codice_fiscale   |
+        +=======================+============+===========+===========+=======+======================+==================+================+=============+=======================+=============+===================+================+=======+================+=================+==================+
+        | Marche                | Macerata   | Di Felice | Giacomina | F     | Mosciano Sant'angelo | Teramo           | Abruzzo        |       64023 | TE                    | 1945-09-18  | Viale De Amicis   | 76             | 62020 | Colmurano      | MC              | DFLGMN45P58F764B |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Friuli Venezia Giulia | Udine      | Galli     | Imen      | F     | Isola Dovarese       | Cremona          | Lombardia      |       26031 | CR                    | 1942-03-10  | Via Udine         | 2              | 33020 | Verzegnis      | UD              | GLLMNI42C50E356T |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Abruzzo               | Pescara    | Rosso     | Eva       | F     | Cellarengo           | Asti             | Piemonte       |       14010 | AT                    | 2001-12-31  | Via G. Fonzi      | 58             | 65010 | Spoltore       | PE              | RSSVEA01T71C438U |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Emilia Romagna        | Bologna    | Grasso    | Emanuele  | M     | Caposele             | Avellino         | Campania       |       83040 | AV                    | 1942-08-27  | Via G. Massarenti | 223/5          | 40138 | Bologna        | BO              | GRSMNL42M27B674L |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Sicilia               | Palermo    | Pastorino | Lenuta    | F     | Borzonasca           | Genova           | Liguria        |       16041 | GE                    | 1972-09-05  | Via Montalbo      | 124            | 90142 | Palermo        | PA              | PSTLNT72P45B067T |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        
+        
+        .. |pip| image:: https://badge.fury.io/py/random-italian-person.svg
+            :target: https://badge.fury.io/py/random-italian-person
+            :alt: Pypi project
+        
+        .. |downloads| image:: https://pepy.tech/badge/random-italian-person
+            :target: https://pepy.tech/badge/random-italian-person
+            :alt: Pypi total project downloads
+        
+        .. |github| image:: https://github.com/lucacappelletti94/random_italian_person/actions/workflows/python.yml/badge.svg
+            :target: https://github.com/lucacappelletti94/random_italian_person/actions
+            :alt: Github Actions
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.0
 Provides-Extra: test
-
-random_italian_person
-=========================================================================================
-|pip| |downloads|
-
-Python package to generate an Italian person randomly.
-
-How do I install this package?
-----------------------------------------------
-As usual, just download it using pip:
-
-.. code:: shell
-
-    pip install random_italian_person
-
-
-Usage examples
------------------------------------------------
-
-.. code:: python
-
-    from random_italian_person import RandomItalianPerson
-
-    person = RandomItalianPerson()
-
-    print(person.describe())
-    # 'Rodrigo Benedetti è nata/o a Molazzana (LU) il 1972-12-18. Ora vive a Cagliari (CA) in Via Giuseppe Garibaldi 109.'
-
-Generate a CSV of random italian persons
------------------------------------------------
-One of the most common usages for this library is to render
-fake datasets for testing porposes. For instance,
-to generate a CSV with 5 random person you can use:
-
-.. code:: python
-
-    import pandas as pd
-    from random_italian_person import RandomItalianPerson
-
-    df = pd.DataFrame([
-        RandomItalianPerson().data
-        for _ in range(5)
-    ])
-
-The obtained dataframe will look like:
-
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| region                | province   | surname   | name      | sex   | birth_municipality   | birth_province   | birth_region   |   birth_cap | birth_province_code   | birthdate   | address           | house_number   |   cap | municipality   | province_code   | codice_fiscale   |
-+=======================+============+===========+===========+=======+======================+==================+================+=============+=======================+=============+===================+================+=======+================+=================+==================+
-| Marche                | Macerata   | Di Felice | Giacomina | F     | Mosciano Sant'angelo | Teramo           | Abruzzo        |       64023 | TE                    | 1945-09-18  | Viale De Amicis   | 76             | 62020 | Colmurano      | MC              | DFLGMN45P58F764B |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Friuli Venezia Giulia | Udine      | Galli     | Imen      | F     | Isola Dovarese       | Cremona          | Lombardia      |       26031 | CR                    | 1942-03-10  | Via Udine         | 2              | 33020 | Verzegnis      | UD              | GLLMNI42C50E356T |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Abruzzo               | Pescara    | Rosso     | Eva       | F     | Cellarengo           | Asti             | Piemonte       |       14010 | AT                    | 2001-12-31  | Via G. Fonzi      | 58             | 65010 | Spoltore       | PE              | RSSVEA01T71C438U |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Emilia Romagna        | Bologna    | Grasso    | Emanuele  | M     | Caposele             | Avellino         | Campania       |       83040 | AV                    | 1942-08-27  | Via G. Massarenti | 223/5          | 40138 | Bologna        | BO              | GRSMNL42M27B674L |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Sicilia               | Palermo    | Pastorino | Lenuta    | F     | Borzonasca           | Genova           | Liguria        |       16041 | GE                    | 1972-09-05  | Via Montalbo      | 124            | 90142 | Palermo        | PA              | PSTLNT72P45B067T |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-
-
-.. |pip| image:: https://badge.fury.io/py/random-italian-person.svg
-    :target: https://badge.fury.io/py/random-italian-person
-    :alt: Pypi project
-
-.. |downloads| image:: https://pepy.tech/badge/random-italian-person
-    :target: https://pepy.tech/badge/random-italian-person
-    :alt: Pypi total project downloads
-
-
```

### Comparing `random_italian_person-1.0.5/README.rst` & `random_italian_person-1.0.6/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 random_italian_person
 =========================================================================================
-|pip| |downloads|
+|pip| |downloads| |github|
 
 Python package to generate an Italian person randomly.
 
 How do I install this package?
 ----------------------------------------------
 As usual, just download it using pip:
 
@@ -61,7 +61,11 @@
 .. |pip| image:: https://badge.fury.io/py/random-italian-person.svg
     :target: https://badge.fury.io/py/random-italian-person
     :alt: Pypi project
 
 .. |downloads| image:: https://pepy.tech/badge/random-italian-person
     :target: https://pepy.tech/badge/random-italian-person
     :alt: Pypi total project downloads
+
+.. |github| image:: https://github.com/lucacappelletti94/random_italian_person/actions/workflows/python.yml/badge.svg
+    :target: https://github.com/lucacappelletti94/random_italian_person/actions
+    :alt: Github Actions
```

### Comparing `random_italian_person-1.0.5/random_italian_person/datasets/addresses.csv` & `random_italian_person-1.0.6/random_italian_person/datasets/addresses.csv`

 * *Files identical despite different names*

### Comparing `random_italian_person-1.0.5/random_italian_person/datasets/municipalities.csv` & `random_italian_person-1.0.6/random_italian_person/datasets/municipalities.csv`

 * *Files identical despite different names*

### Comparing `random_italian_person-1.0.5/random_italian_person/datasets/names.csv` & `random_italian_person-1.0.6/random_italian_person/datasets/names.csv`

 * *Files identical despite different names*

### Comparing `random_italian_person-1.0.5/random_italian_person/datasets/surnames.csv` & `random_italian_person-1.0.6/random_italian_person/datasets/surnames.csv`

 * *Files identical despite different names*

### Comparing `random_italian_person-1.0.5/random_italian_person/random_italian_person.py` & `random_italian_person-1.0.6/random_italian_person/random_italian_person.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import os
-import pandas as pd
-import numpy as np
+"""Random Italian person generator."""
 import json
+import os
 from typing import Dict
+
+import numpy as np
+import pandas as pd
 from codicefiscale import codicefiscale
+
 from .utils import random_birthday
 
 
 class RandomItalianPerson:
 
     municipalities = None
     names = None
@@ -43,53 +46,58 @@
         if RandomItalianPerson.addresses is None:
             RandomItalianPerson.addresses = pd.read_csv(
                 "{}/datasets/addresses.csv".format(
                     os.path.dirname(os.path.abspath(__file__))),
                 dtype={"cap": str},
                 na_filter=False
             )
-
-        surname_data = RandomItalianPerson.surnames.sample(n=1)
-        name_data = RandomItalianPerson.names.iloc[np.random.choice(
-            RandomItalianPerson.names.index, p=RandomItalianPerson.frequencies)]
-        municipality_data = RandomItalianPerson.municipalities[
-            RandomItalianPerson.municipalities.province.isin(
-                surname_data.province)
-        ].sample(n=1)
-
-        address_data = RandomItalianPerson.addresses.sample(n=1)
-
-        self._data = {
-            **surname_data.reset_index(drop=True).iloc[0].to_dict(),
-            **name_data.to_dict(),
-            **{
-                "birth_{}".format(c): v
-                for c, v in municipality_data.reset_index(drop=True).iloc[0].to_dict().items()
-            },
-            "birthdate": random_birthday().isoformat(),
-            **address_data.reset_index(drop=True).iloc[0].to_dict()
-        }
-
-        try:
-            self._data["codice_fiscale"] = codicefiscale.encode(
-                lastname=self.surname,
-                firstname=self.name,
-                gender=self.sex,
-                birthdate=self.birthdate,
-                birthplace=self.birthplace
-            )
-        except TypeError:
-            self._data["codice_fiscale"] = codicefiscale.encode(
-                surname=self.surname,
-                name=self.name,
-                sex=self.sex,
-                birthdate=self.birthdate,
-                birthplace=self.birthplace
-            )
-
+        
+        while True:
+            try:
+                surname_data = RandomItalianPerson.surnames.sample(n=1)
+                name_data = RandomItalianPerson.names.iloc[np.random.choice(
+                    RandomItalianPerson.names.index, p=RandomItalianPerson.frequencies)]
+                municipality_data = RandomItalianPerson.municipalities[
+                    RandomItalianPerson.municipalities.province.isin(
+                        surname_data.province
+                    )
+                ].sample(n=1)
+
+                address_data = RandomItalianPerson.addresses.sample(n=1)
+
+                self._data = {
+                    **surname_data.reset_index(drop=True).iloc[0].to_dict(),
+                    **name_data.to_dict(),
+                    **{
+                        f"birth_{c}": v
+                        for c, v in municipality_data.reset_index(drop=True).iloc[0].to_dict().items()
+                    },
+                    "birthdate": random_birthday().isoformat(),
+                    **address_data.reset_index(drop=True).iloc[0].to_dict()
+                }
+
+                try:
+                    self._data["codice_fiscale"] = codicefiscale.encode(
+                        lastname=self.surname,
+                        firstname=self.name,
+                        gender=self.sex,
+                        birthdate=self.birthdate,
+                        birthplace=self.birthplace
+                    )
+                except TypeError:
+                    self._data["codice_fiscale"] = codicefiscale.encode(
+                        surname=self.surname,
+                        name=self.name,
+                        sex=self.sex,
+                        birthdate=self.birthdate,
+                        birthplace=self.birthplace
+                    )
+                break
+            except ValueError:
+                continue
     @property
     def name(self) -> str:
         return self._data["name"]
 
     @property
     def surname(self) -> str:
         return self._data["surname"]
```

### Comparing `random_italian_person-1.0.5/random_italian_person/utils/random_birthday.py` & `random_italian_person-1.0.6/random_italian_person/utils/random_birthday.py`

 * *Files identical despite different names*

### Comparing `random_italian_person-1.0.5/random_italian_person.egg-info/PKG-INFO` & `random_italian_person-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,86 @@
 Metadata-Version: 2.1
-Name: random-italian-person
-Version: 1.0.5
+Name: random_italian_person
+Version: 1.0.6
 Summary: Python package to generate an Italian person randomly.
 Home-page: https://github.com/LucaCappelletti94/random_italian_person
 Author: LucaCappelletti94
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
+Description: random_italian_person
+        =========================================================================================
+        |pip| |downloads| |github|
+        
+        Python package to generate an Italian person randomly.
+        
+        How do I install this package?
+        ----------------------------------------------
+        As usual, just download it using pip:
+        
+        .. code:: shell
+        
+            pip install random_italian_person
+        
+        
+        Usage examples
+        -----------------------------------------------
+        
+        .. code:: python
+        
+            from random_italian_person import RandomItalianPerson
+        
+            person = RandomItalianPerson()
+        
+            print(person.describe())
+            # 'Rodrigo Benedetti è nata/o a Molazzana (LU) il 1972-12-18. Ora vive a Cagliari (CA) in Via Giuseppe Garibaldi 109.'
+        
+        Generate a CSV of random italian persons
+        -----------------------------------------------
+        One of the most common usages for this library is to render
+        fake datasets for testing porposes. For instance,
+        to generate a CSV with 5 random person you can use:
+        
+        .. code:: python
+        
+            import pandas as pd
+            from random_italian_person import RandomItalianPerson
+        
+            df = pd.DataFrame([
+                RandomItalianPerson().data
+                for _ in range(5)
+            ])
+        
+        The obtained dataframe will look like:
+        
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | region                | province   | surname   | name      | sex   | birth_municipality   | birth_province   | birth_region   |   birth_cap | birth_province_code   | birthdate   | address           | house_number   |   cap | municipality   | province_code   | codice_fiscale   |
+        +=======================+============+===========+===========+=======+======================+==================+================+=============+=======================+=============+===================+================+=======+================+=================+==================+
+        | Marche                | Macerata   | Di Felice | Giacomina | F     | Mosciano Sant'angelo | Teramo           | Abruzzo        |       64023 | TE                    | 1945-09-18  | Viale De Amicis   | 76             | 62020 | Colmurano      | MC              | DFLGMN45P58F764B |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Friuli Venezia Giulia | Udine      | Galli     | Imen      | F     | Isola Dovarese       | Cremona          | Lombardia      |       26031 | CR                    | 1942-03-10  | Via Udine         | 2              | 33020 | Verzegnis      | UD              | GLLMNI42C50E356T |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Abruzzo               | Pescara    | Rosso     | Eva       | F     | Cellarengo           | Asti             | Piemonte       |       14010 | AT                    | 2001-12-31  | Via G. Fonzi      | 58             | 65010 | Spoltore       | PE              | RSSVEA01T71C438U |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Emilia Romagna        | Bologna    | Grasso    | Emanuele  | M     | Caposele             | Avellino         | Campania       |       83040 | AV                    | 1942-08-27  | Via G. Massarenti | 223/5          | 40138 | Bologna        | BO              | GRSMNL42M27B674L |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        | Sicilia               | Palermo    | Pastorino | Lenuta    | F     | Borzonasca           | Genova           | Liguria        |       16041 | GE                    | 1972-09-05  | Via Montalbo      | 124            | 90142 | Palermo        | PA              | PSTLNT72P45B067T |
+        +-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
+        
+        
+        .. |pip| image:: https://badge.fury.io/py/random-italian-person.svg
+            :target: https://badge.fury.io/py/random-italian-person
+            :alt: Pypi project
+        
+        .. |downloads| image:: https://pepy.tech/badge/random-italian-person
+            :target: https://pepy.tech/badge/random-italian-person
+            :alt: Pypi total project downloads
+        
+        .. |github| image:: https://github.com/lucacappelletti94/random_italian_person/actions/workflows/python.yml/badge.svg
+            :target: https://github.com/lucacappelletti94/random_italian_person/actions
+            :alt: Github Actions
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.0
 Provides-Extra: test
-
-random_italian_person
-=========================================================================================
-|pip| |downloads|
-
-Python package to generate an Italian person randomly.
-
-How do I install this package?
-----------------------------------------------
-As usual, just download it using pip:
-
-.. code:: shell
-
-    pip install random_italian_person
-
-
-Usage examples
------------------------------------------------
-
-.. code:: python
-
-    from random_italian_person import RandomItalianPerson
-
-    person = RandomItalianPerson()
-
-    print(person.describe())
-    # 'Rodrigo Benedetti è nata/o a Molazzana (LU) il 1972-12-18. Ora vive a Cagliari (CA) in Via Giuseppe Garibaldi 109.'
-
-Generate a CSV of random italian persons
------------------------------------------------
-One of the most common usages for this library is to render
-fake datasets for testing porposes. For instance,
-to generate a CSV with 5 random person you can use:
-
-.. code:: python
-
-    import pandas as pd
-    from random_italian_person import RandomItalianPerson
-
-    df = pd.DataFrame([
-        RandomItalianPerson().data
-        for _ in range(5)
-    ])
-
-The obtained dataframe will look like:
-
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| region                | province   | surname   | name      | sex   | birth_municipality   | birth_province   | birth_region   |   birth_cap | birth_province_code   | birthdate   | address           | house_number   |   cap | municipality   | province_code   | codice_fiscale   |
-+=======================+============+===========+===========+=======+======================+==================+================+=============+=======================+=============+===================+================+=======+================+=================+==================+
-| Marche                | Macerata   | Di Felice | Giacomina | F     | Mosciano Sant'angelo | Teramo           | Abruzzo        |       64023 | TE                    | 1945-09-18  | Viale De Amicis   | 76             | 62020 | Colmurano      | MC              | DFLGMN45P58F764B |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Friuli Venezia Giulia | Udine      | Galli     | Imen      | F     | Isola Dovarese       | Cremona          | Lombardia      |       26031 | CR                    | 1942-03-10  | Via Udine         | 2              | 33020 | Verzegnis      | UD              | GLLMNI42C50E356T |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Abruzzo               | Pescara    | Rosso     | Eva       | F     | Cellarengo           | Asti             | Piemonte       |       14010 | AT                    | 2001-12-31  | Via G. Fonzi      | 58             | 65010 | Spoltore       | PE              | RSSVEA01T71C438U |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Emilia Romagna        | Bologna    | Grasso    | Emanuele  | M     | Caposele             | Avellino         | Campania       |       83040 | AV                    | 1942-08-27  | Via G. Massarenti | 223/5          | 40138 | Bologna        | BO              | GRSMNL42M27B674L |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-| Sicilia               | Palermo    | Pastorino | Lenuta    | F     | Borzonasca           | Genova           | Liguria        |       16041 | GE                    | 1972-09-05  | Via Montalbo      | 124            | 90142 | Palermo        | PA              | PSTLNT72P45B067T |
-+-----------------------+------------+-----------+-----------+-------+----------------------+------------------+----------------+-------------+-----------------------+-------------+-------------------+----------------+-------+----------------+-----------------+------------------+
-
-
-.. |pip| image:: https://badge.fury.io/py/random-italian-person.svg
-    :target: https://badge.fury.io/py/random-italian-person
-    :alt: Pypi project
-
-.. |downloads| image:: https://pepy.tech/badge/random-italian-person
-    :target: https://pepy.tech/badge/random-italian-person
-    :alt: Pypi total project downloads
-
-
```

### Comparing `random_italian_person-1.0.5/random_italian_person.egg-info/SOURCES.txt` & `random_italian_person-1.0.6/random_italian_person.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `random_italian_person-1.0.5/setup.py` & `random_italian_person-1.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     long_description=long_description,
     url="https://github.com/LucaCappelletti94/random_italian_person",
     author="LucaCappelletti94",
     author_email="cappelletti.luca94@gmail.com",
     # Choose your license
     license='MIT',
     include_package_data=True,
+    python_requires='>=3.8.0',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
     ],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     tests_require=test_deps,
```

