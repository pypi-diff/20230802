# Comparing `tmp/french_cities-0.1.0a9.tar.gz` & `tmp/french_cities-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.0a9.tar", max compression
+gzip compressed data, was "french_cities-0.1.1a1.tar", max compression
```

## Comparing `french_cities-0.1.0a9.tar` & `french_cities-0.1.1a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      349 2023-07-25 14:34:53.551368 french_cities-0.1.0a9/french_cities/__init__.py
--rw-r--r--   0        0        0    19611 2023-07-25 12:18:31.033911 french_cities-0.1.0a9/french_cities/city_finder.py
--rw-r--r--   0        0        0     7464 2023-07-25 14:33:59.441164 french_cities-0.1.0a9/french_cities/departement_finder.py
--rw-r--r--   0        0        0      535 2023-07-25 08:14:16.766868 french_cities-0.1.0a9/french_cities/utils.py
--rw-r--r--   0        0        0     7844 2023-07-23 11:38:50.970042 french_cities-0.1.0a9/french_cities/vintage.py
--rw-r--r--   0        0        0     1235 2023-07-25 14:35:07.329769 french_cities-0.1.0a9/pyproject.toml
--rw-r--r--   0        0        0     9426 2023-07-25 14:15:49.284414 french_cities-0.1.0a9/README.fr.md
--rw-r--r--   0        0        0     7918 2023-07-25 14:15:36.692406 french_cities-0.1.0a9/README.md
--rw-r--r--   0        0        0    18350 1970-01-01 00:00:00.000000 french_cities-0.1.0a9/PKG-INFO
+-rw-r--r--   0        0        0    10111 2023-08-02 16:22:01.998280 french_cities-0.1.1a1/README.fr.md
+-rw-r--r--   0        0        0     8545 2023-08-02 16:22:01.998280 french_cities-0.1.1a1/README.md
+-rw-r--r--   0        0        0      394 2023-08-02 16:22:02.002280 french_cities-0.1.1a1/french_cities/__init__.py
+-rw-r--r--   0        0        0    22856 2023-08-02 16:22:02.002280 french_cities-0.1.1a1/french_cities/city_finder.py
+-rw-r--r--   0        0        0     9317 2023-08-02 16:22:02.002280 french_cities-0.1.1a1/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      519 2023-08-02 16:22:02.002280 french_cities-0.1.1a1/french_cities/utils.py
+-rw-r--r--   0        0        0     7956 2023-08-02 16:22:02.002280 french_cities-0.1.1a1/french_cities/vintage.py
+-rw-r--r--   0        0        0     1279 2023-08-02 16:22:02.002280 french_cities-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0    20203 1970-01-01 00:00:00.000000 french_cities-0.1.1a1/PKG-INFO
```

### Comparing `french_cities-0.1.0a9/french_cities/departement_finder.py` & `french_cities-0.1.1a1/french_cities/departement_finder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,226 +1,283 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Jul  6 11:38:34 2023
-"""
-import pandas as pd
-import io
-from requests_cache import CachedSession
-from requests import Session
-from datetime import timedelta
-import logging
-import time
-from tqdm import tqdm
-from pebble import ThreadPool
-
-from french_cities.utils import init_pynsee
-
-
-logger = logging.getLogger(__name__)
-
-
-def _process_departements_from_postal(
-    df: pd.DataFrame, source: str, alias: str, session: Session = None
-) -> pd.DataFrame:
-    """
-    Retrieve departement's code from postoffice code. Adds the result as a new
-    column to dataframe under the label 'alias'. Uses the BAN (Base Adresse
-    Nationale under the hood) and OpenDataSoft's freemium API in backoffice (
-    mostly in case of "Cedex" codes)
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        DataFrame containing postal codes
-    source : str
-        Field containing the postal codes
-    alias : str
-        Column to store the departements' codes unto
-    session : Session, optional
-        Web session. The default is None (and will use a CachedSession with
-        30 days expiration)
-
-    Returns
-    -------
-    df : pd.DataFrame
-        Updated DataFrame with departement's codes
-
-    """
-
-    if not session:
-        session = CachedSession(
-            allowable_methods=("GET", "POST"), expire_after=timedelta(days=30)
-        )
-
-    postal_codes = df[[source]].drop_duplicates(keep="first")
-
-    r = session.post(
-        # recherche grâce à l'API de la BAN
-        "https://api-adresse.data.gouv.fr/search/csv/",
-        files=[
-            ("data", postal_codes.to_csv(index=False)),
-            ("postcode", (None, source)),
-            ("result_columns", (None, source)),
-            ("result_columns", (None, "result_context")),
-        ],
-    )
-    result = pd.read_csv(io.BytesIO(r.content), dtype=str)
-    result[alias] = (
-        result["result_context"].str.split(",", expand=True)[0].str.strip(" ")
-    )
-    result = result.drop("result_context", axis=1)
-
-    # where code is unknown, use Christian Quest Dataset with Cedex codes and
-    # OpenDataSoft API (v2.1 contrairement à la doc disponible) en Freemium
-    # https://www.data.gouv.fr/fr/datasets/liste-des-cedex/#_
-    # https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr
-    def get(x):
-        while True:
-            r = session.get(
-                # recherche "en masse" grâce à l'API de la BAN
-                "https://public.opendatasoft.com/api/explore/v2.1/catalog/datasets/correspondance-code-cedex-code-insee/records",
-                params={
-                    "select": "insee,nom_dep",
-                    "where": f"code={x}",
-                    "limit": "10",
-                    "offset": "0",
-                    "timezone": "UTC",
-                    "include_links": "false",
-                    "include_app_metas": "false",
-                },
-            )
-            if r.ok:
-                break
-            elif r.status_code == 429:
-                time.sleep(1)
-            else:
-                logger.warning(
-                    f"Error occured on code {x} on OpenDataSoft's API"
-                )
-                return None
-        results = r.json()["results"]
-        for dict_ in results:
-            dict_.update({source: x})
-        return results
-
-    ix = result[result[alias].isnull()].index
-    if len(ix) > 0:
-        logger.info("postal codes unrecognized - maybe Cedex codes")
-        args = result.loc[ix, source].tolist()
-        results_cedex = []
-        with tqdm(
-            total=len(args), desc="Querying OpenDataSoft API", leave=False
-        ) as pbar:
-            with ThreadPool(10) as pool:
-                future = pool.map(get, args)
-                results_iterator = future.result()
-                while True:
-                    try:
-                        this_result = next(results_iterator)
-                        if this_result:
-                            results_cedex += this_result
-                    except StopIteration:
-                        break
-                    finally:
-                        pbar.update(1)
-        results_cedex = pd.DataFrame(results_cedex)
-        results_cedex = _process_departements_from_insee_code(
-            results_cedex, source="insee", alias="dep_cedex", session=session
-        )
-        result = result.merge(results_cedex, on=source, how="left")
-        result.loc[ix, alias] = result.loc[ix, "dep_cedex"]
-        result = result.drop(list(set(results_cedex.columns) - {source,}), axis=1)
-
-    logger.info("résultat obtenu")
-
-    df = df.merge(result, on=source, how="left")
-
-    return df
-
-
-def _process_departements_from_insee_code(
-    df: pd.DataFrame, source: str, alias: str, session: Session = None
-) -> pd.DataFrame:
-    """
-    Compute departement's codes from official french cities codes (COG INSEE).
-    Adds the result as a new column to dataframe under the label 'alias'.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        DataFrame containing official cities codes
-    source : str
-        Field containing the official codes (INSEE COG)
-    alias : str
-        Column to store the departements' codes unto
-    session : Session, optional
-        Web session. The default is None (and will use a CachedSession with
-        30 days expiration)
-        **ignored argument, set only for coherence with
-        _process_departements_from_postal**
-
-    Returns
-    -------
-    df : pd.DataFrame
-        Updated DataFrame with departement's codes
-
-    """
-    df[alias] = df[source].str[:2]
-
-    ix = df[df[alias] == "97"].index
-    df.loc[ix, alias] = df.loc[ix, source].str[:3]
-
-    return df
-
-
-def find_departements(
-    df: pd.DataFrame,
-    source: str,
-    alias: str,
-    type_code: str,
-    session: Session = None,
-) -> pd.DataFrame:
-    """
-    Compute departement's codes from postal or official codes (ie. INSEE COG)'
-    Adds the result as a new column to dataframe under the label 'alias'.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        DataFrame containing official cities codes
-    source : str
-        Field containing the post or official codes
-    alias : str
-        Column to store the departements' codes unto
-    type_code : str
-        Type of codes passed under `alias` label. Should be either 'insee' for
-        official codes or 'postcode' for postal codes.
-    session : Session, optional
-        Web session. The default is None (and will use a CachedSession with
-        30 days expiration)
-
-    Raises
-    ------
-    ValueError
-        If type_code not among "postcode", "insee".
-
-    Returns
-    -------
-    df : pd.DataFrame
-        Updated DataFrame with departement's codes
-
-    """
-    if type_code not in {"postcode", "insee"}:
-        msg = (
-            "type_code must be among ('postcode', 'insee') - "
-            f"found {type_code} instead"
-        )
-        raise ValueError(msg)
-
-    init_pynsee()
-
-    df = df.copy()
-    if type_code == "postcode":
-        func = _process_departements_from_postal
-    elif type_code == "insee":
-        func = _process_departements_from_insee_code
-    return func(df, source, alias, session)
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Jul  6 11:38:34 2023
+"""
+import pandas as pd
+import io
+from requests_cache import CachedSession
+from requests import Session
+from datetime import timedelta
+import logging
+import time
+from tqdm import tqdm
+from pebble import ThreadPool
+from rapidfuzz import fuzz
+from unidecode import unidecode
+
+from french_cities.utils import init_pynsee
+
+
+logger = logging.getLogger(__name__)
+
+
+def _process_departements_from_postal(
+    df: pd.DataFrame, source: str, alias: str, session: Session = None
+) -> pd.DataFrame:
+    """
+    Retrieve departement's code from postoffice code. Adds the result as a new
+    column to dataframe under the label 'alias'. Uses the BAN (Base Adresse
+    Nationale under the hood) and OpenDataSoft's freemium API in backoffice (
+    mostly in case of "Cedex" codes)
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame containing postal codes
+    source : str
+        Field containing the postal codes
+    alias : str
+        Column to store the departements' codes unto
+    session : Session, optional
+        Web session. The default is None (and will use a CachedSession with
+        30 days expiration)
+
+    Returns
+    -------
+    df : pd.DataFrame
+        Updated DataFrame with departement's codes
+
+    """
+
+    if not session:
+        session = CachedSession(
+            allowable_methods=("GET", "POST"), expire_after=timedelta(days=30)
+        )
+
+    postal_codes = df[[source]].drop_duplicates(keep="first")
+    r = session.post(
+        # recherche grâce à l'API de la BAN
+        "https://api-adresse.data.gouv.fr/search/csv/",
+        files=[
+            ("data", postal_codes.to_csv(index=False)),
+            ("postcode", (None, source)),
+            ("result_columns", (None, source)),
+            ("result_columns", (None, "result_context")),
+        ],
+    )
+    result = pd.read_csv(io.BytesIO(r.content), dtype=str)
+    result[alias] = (
+        result["result_context"].str.split(",", expand=True)[0].str.strip(" ")
+    )
+    result = result.drop("result_context", axis=1)
+
+    # where code is unknown, use Christian Quest Dataset with Cedex codes and
+    # OpenDataSoft API (v2.1 contrairement à la doc disponible) en Freemium
+    # https://www.data.gouv.fr/fr/datasets/liste-des-cedex/#_
+    # https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr
+    def get(x):
+        while True:
+            r = session.get(
+                # recherche "en masse" grâce à l'API de la BAN
+                "https://public.opendatasoft.com/api/explore/v2.1/catalog/datasets/correspondance-code-cedex-code-insee/records",
+                params={
+                    "select": "insee,libelle,nom_com",
+                    "where": f"code={x}",
+                    "limit": "10",
+                    "offset": "0",
+                    "timezone": "UTC",
+                    "include_links": "false",
+                    "include_app_metas": "false",
+                },
+            )
+            if r.ok:
+                break
+            elif r.status_code == 429:
+                time.sleep(1)
+            else:
+                logger.warning(
+                    f"Error occured on code {x} on OpenDataSoft's API"
+                )
+                return None
+        results = r.json()["results"]
+
+        for dict_ in results:
+            dict_.update({source: x})
+        return results
+
+    ix = result[result[alias].isnull()].index
+    if len(ix) > 0:
+        logger.info("postal codes unrecognized - maybe Cedex codes")
+        args = result.loc[ix, source].dropna().tolist()
+        results_cedex = []
+        with tqdm(
+            total=len(args), desc="Querying OpenDataSoft API", leave=False
+        ) as pbar:
+            with ThreadPool(10) as pool:
+                future = pool.map(get, args)
+                results_iterator = future.result()
+                while True:
+                    try:
+                        this_result = next(results_iterator)
+                        if this_result:
+                            results_cedex += this_result
+                    except StopIteration:
+                        break
+                    finally:
+                        pbar.update(1)
+        results_cedex = pd.DataFrame(results_cedex)
+
+        # Select main city in case of discordant results. For instance, with
+        # postcode=74105, you'll get:
+        #    insee       nom_dep          libelle          nom_com
+        # 0  74145  HAUTE-SAVOIE  ANNEMASSE CEDEX          Juvigny
+        # 1  74012  HAUTE-SAVOIE  ANNEMASSE CEDEX        Annemasse
+        # 2  74305  HAUTE-SAVOIE  ANNEMASSE CEDEX   Ville-la-Grand
+        # 3  74298  HAUTE-SAVOIE  ANNEMASSE CEDEX  Vétraz-Monthoux
+
+        if not results_cedex.empty:
+            for f in ["libelle", "nom_com"]:
+                results_cedex[f] = (
+                    results_cedex[f]
+                    .str.upper()
+                    .apply(unidecode)
+                    .str.split(r"\W+")
+                    .str.join(" ")
+                    .str.strip(" ")
+                )
+            results_cedex["libelle"] = results_cedex["libelle"].str.replace(
+                r" CEDEX", ""
+            )
+            results_cedex["score"] = results_cedex[
+                ["libelle", "nom_com"]
+            ].apply(lambda xy: fuzz.token_set_ratio(*xy), axis=1)
+
+            results_cedex = results_cedex.sort_values([source, "score"])
+            results_cedex = results_cedex.drop_duplicates(source, keep="last")
+            results_cedex = results_cedex.drop(
+                ["nom_com", "score", "libelle"], axis=1
+            )
+            results_cedex = results_cedex.drop_duplicates()
+
+            results_cedex = _process_departements_from_insee_code(
+                results_cedex,
+                source="insee",
+                alias="dep_cedex",
+                session=session,
+            )
+            result = result.merge(results_cedex, on=source, how="left")
+            result.loc[ix, alias] = result.loc[ix, "dep_cedex"]
+            result = result.drop(
+                list(
+                    set(results_cedex.columns)
+                    - {
+                        source,
+                    }
+                ),
+                axis=1,
+            )
+
+    ix = result[result[alias].isnull()].index
+    if len(ix) > 0:
+        # Still no results -> assume we can use the first characters of
+        # postcode anyway
+        result.loc[ix, alias] = _process_departements_from_insee_code(
+            result.loc[ix],
+            source=source,
+            alias="dep",
+            session=session,
+        )[alias]
+
+    logger.info("résultat obtenu")
+
+    df = df.merge(result, on=source, how="left")
+
+    return df
+
+
+def _process_departements_from_insee_code(
+    df: pd.DataFrame, source: str, alias: str, session: Session = None
+) -> pd.DataFrame:
+    """
+    Compute departement's codes from official french cities codes (COG INSEE).
+    Adds the result as a new column to dataframe under the label 'alias'.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame containing official cities codes
+    source : str
+        Field containing the official codes (INSEE COG)
+    alias : str
+        Column to store the departements' codes unto
+    session : Session, optional
+        Web session. The default is None (and will use a CachedSession with
+        30 days expiration)
+        **ignored argument, set only for coherence with
+        _process_departements_from_postal**
+
+    Returns
+    -------
+    df : pd.DataFrame
+        Updated DataFrame with departement's codes
+
+    """
+    df[alias] = df[source].str[:2]
+
+    ix = df[df[alias] == "97"].index
+    df.loc[ix, alias] = df.loc[ix, source].str[:3]
+
+    return df
+
+
+def find_departements(
+    df: pd.DataFrame,
+    source: str,
+    alias: str,
+    type_code: str,
+    session: Session = None,
+) -> pd.DataFrame:
+    """
+    Compute departement's codes from postal or official codes (ie. INSEE COG)'
+    Adds the result as a new column to dataframe under the label 'alias'.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame containing official cities codes
+    source : str
+        Field containing the post or official codes
+    alias : str
+        Column to store the departements' codes unto
+    type_code : str
+        Type of codes passed under `alias` label. Should be either 'insee' for
+        official codes or 'postcode' for postal codes.
+    session : Session, optional
+        Web session. The default is None (and will use a CachedSession with
+        30 days expiration)
+
+    Raises
+    ------
+    ValueError
+        If type_code not among "postcode", "insee".
+
+    Returns
+    -------
+    df : pd.DataFrame
+        Updated DataFrame with departement's codes
+
+    """
+    if type_code not in {"postcode", "insee"}:
+        msg = (
+            "type_code must be among ('postcode', 'insee') - "
+            f"found {type_code} instead"
+        )
+        raise ValueError(msg)
+
+    init_pynsee()
+
+    df = df.copy()
+    if type_code == "postcode":
+        func = _process_departements_from_postal
+    elif type_code == "insee":
+        func = _process_departements_from_insee_code
+    return func(df, source, alias, session)
```

### Comparing `french_cities-0.1.0a9/README.fr.md` & `french_cities-0.1.1a1/README.fr.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,238 +1,253 @@
-# french-cities
-Boîte à outils sur les communes françaises : millésimage, reconnaissance de 
-départements ou de communes...
-
-
-# Installation
-
-`pip install french-cities`
-
-Notez qu'à cette heure, `pynsee` ne supporte pas les projections de codes commune. 
-Dans l'immédiat, après avoir installé `french-cities` depuis pypi, il faut donc
-désinstaller `pynsee` puis réinstaller la version master courante depuis son repo 
-github :
-```
-pip uninstall pynsee
-pip install git+https://github.com/InseeFrLab/pynsee
-```
-
-# Configuration
-
-## Ajout des clefs API INSEE
-`french-cities` utilise `pynsee`, qui nécessite des cles API INSEE pour être 
-fonctionnel. Jusqu'à quatre clefs peuvent être spécifiées à l'aide de variables
-d'environnement :
-* insee_key
-* insee_secret, 
-* http_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
-* https_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
-
-Merci de se référer à [la documentation de `pynsee`](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
-pour plus d'information sur les clefs API et la configuration.
-
-## Gestion des sessions web
-`pynsee` utilise son propre gestionnaire de session web. 
-Ainsi, les objets Session passés en argument à `french-cities` ne seront
-**PAS** partagés avec `pynsee`. Cela explique la possibilité de passer une 
-session en argument alors même que des proxy professionnels peuvent être 
-spécifiés par variables d'environnement (pour `pynsee`).
-
-## Utilisation
-
-### Pourquoi french-cities ?
-Des packages et des API sont déjà disponibles pour des recherches usuelles. Par
-exemple, `pynsee` utilise les API de l'INSEE pour retrouver de multiples données
-(comme les départements, les régions, etc.) ; `geopy` peut également retrouver
-des communes à partir de leurs noms en s'appuyant sur la BAN (Base Adresse 
-Nationale) ou sur le service de géocodage Nominatim.
-
-La différence est que `french-cities` est optimisé pour travailler avec des données
-fournies sous la forme de Series ou DataFrames pandas. Ce package gérera mieux
-de gros volumes de données que ne le feraient des appels multiples à des API.
-
-### Trouver les départements
-`french-cities` peut retrouver un code département à partir de codes postaux ou 
-de codes communes officiels (COG/INSEE).
-
-Travailler à partir de codes postaux entraînera l'utilisation de la BAN (Base
-Adresse Nationale) et devrait fournir des résultats corrects. Le cas des codes
-Cedex n'étant que partiellement géré par la BAN, un appel est fait dans un
-second temps à l'[API d'OpenDataSoft](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr)
-construite sur la base des [travaux de Christian Quest](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
-Cette utilisation s'appuie sur un accès freemium non authentifié; l'utilisateur 
-du package est invité à contrôler les conditions générales d'utilisation de l'API auprès du
-fournisseur.
-
-Travailler à partir de codes communes officiels peut entraîner des résultats
-erronés pour des données anciennes, dans le cas de communes ayant changé de
-département (ce qui est relativement rare).
-Ce choix est délibéré : seuls les premiers caractères des codes commune sont
-utilisés pour la reconnaissance du département (algorithme rapide et qui donne
-des résultats corrects pour 99% des cas), par opposition à un requêtage
-systématique aux API (processus sans erreur mais long).
-
-```
-from french_cities import find_departements
-import pandas as pd
-
-df = pd.DataFrame(
-    {
-        "code_postal": ["59800", "97133", "20000"],
-        "code_commune": ["59350", "97701", "2A004"],
-        "communes": ["Lille", "Saint-Barthélémy", "Ajaccio"],
-        "deps": ["59", "977", "2A"],
-    }
-)
-df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
-df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
-
-print(df)
-```
-
-Pour une documentation complète sur la fonction `find_departements`, merci 
-d'utiliser la commande suivante :
-`help(find_departements)`.
-
-### Trouver les codes communes
-`french-cities` peut retrouver le code commune à partir de champs multiples.
-Il est capable de détecter certaines erreurs simples dans les champs (jusqu'à 
-une certaine limite).
-
-Les colonnes utilisées par l'algorithme pour cette détection sont (par ordre
-de priorité) :
-* 'x' et 'y' (dans ce cas, un code EPSG doit être explicitement donné);
-* 'postcode' et 'city'
-* 'address', 'postcode' et 'city'
-* 'department' et 'city'
-
-Il est à noter que l'algorithme peu faire être source d'erreur dès lors que
-la jointure spatiale (coordonnées x & y) sera sollicitée sur un millésime ancien.
-Les communes impactées sont les communes restaurées ("scission"), le flux de données
-spatialisées du COG servi par pynsee n'étant pas millésimé à ce jour.
-
-La reconnaissance syntaxique (champs postcode, city, address, departement) est
-basée sur la BAN (base adresse nationale). L'algorithme ne conservera pas de
-résultats insuffisamment fiables, mais des erreurs peuvent subsister (elles 
-seront dans ce cas cohérentes avec les résultats de la BAN).
-
-```
-from french_cities import find_city
-import pandas as pd
-
-df = pd.DataFrame(
-    [
-        {
-            "x": 2.294694,
-            "y": 48.858093,
-            "location": "Tour Eiffel",
-            "dep": "75",
-            "city": "Paris",
-            "address": "5 Avenue Anatole France",
-            "postcode": "75007",
-            "target": "75056",
-        },
-        {
-            "x": 8.738962,
-            "y": 41.919216,
-            "location": "mairie",
-            "dep": "2A",
-            "city": "Ajaccio",
-            "address": "Antoine Sérafini",
-            "postcode": "20000",
-            "target": "2A004",
-        },
-        {
-            "x": -52.334990,
-            "y": 4.938194,
-            "location": "mairie",
-            "dep": "973",
-            "city": "Cayenne",
-            "address": "1 rue de Rémire",
-            "postcode": "97300",
-            "target": "97302",
-        },
-        {
-            "x": np.nan,
-            "y": np.nan,
-            "location": "Erreur code postal Lille/Lyon",
-            "dep": "59",
-            "city": "Lille",
-            "address": "1 rue Faidherbe",
-            "postcode": "69000",
-            "target": "59350",
-        },
-    ]
-)
-df = find_city(df, epsg=4326)
-
-print(df)
-```
-
-Pour une documentation complète sur la fonction `find_city`, merci 
-d'utiliser la commande suivante :
-`help(find_city)`.
-
-### Projection de codes communes dans un millésime donné
-`french-cities` peut tenter de "projeter" un dataframe dans un millésime donné,
-la date initiale demeurant inconnue (voire inexistante, les cas de fichiers
-"multi-millésimés" étant fréquents dans la vie réelle).
-
-Des erreurs peuvent survenir, notamment pour les communes restaurées (dans la 
-mesure où la date initiale de la donnée est inconnue ou inexistante).
-
-Dans le cas où la date des données est connue, il peut être pertinent d'utiliser
-l'API de projection mise à disposition par l'INSEE et accessible au travers de 
-`pynsee`. Il convient de noter que cette utilisation peut être lente, dans la 
-mesure ou chaque commune devra être testée via l'API (qui n'autorise que 
-30 requêtes par minute).
-
-En substance, l'algorithme de `french-cities` contrôle si le code commune existe
-dans le millésime souhaité :
-* s'il existe il sera conservé (à l'approximation précédente près qui peut donc
-impacter les communes restaurées) ;
-* s'il n'existe pas, le code est recherché dans des millésimes antérieurs (et
-l'API de projection de l'INSEE sera mobilisée de manière ciblée).
-
-Cet algorithme va également :
-* convertir les codes des éventuels arrondissements municipaux en celui de leur
-commune de rattachement;
-* convertir les codes des communes associées et déléguées en celui de leur 
-commune de rattachement.
-
-```
-from french_cities import set_vintage
-import pandas as pd
-
-df = pd.DataFrame(
-    [
-        ["07180", "Fusion"],
-        ["02077", "Commune déléguée"],
-        ["02564", "Commune nouvelle"],
-        ["75101", "Arrondissement municipal"],
-        ["59298", "Commune associée"],
-        ["99999", "Code erroné"],
-        ["14472", "Oudon"],
-    ],
-    columns=["A", "Test"],
-    index=["A", "B", "C", "D", 1, 2, 3],
-)
-df = set_vintage(df, 2023, field="A")
-print(df)
-```
-
-Pour une documentation complète sur la fonction `set_vintage`, merci 
-d'utiliser la commande suivante :
-`help(set_vintage)`.
-
-
-## Support
-En cas de bugues, merci d'ouvrir un ticket [sur le repo](https://github.com/tgrandje/french-cities/issues).
-
-## Auteur
-Thomas GRANDJEAN (DREAL Hauts-de-France, service Information, Développement Durable et Évaluation Environnementale, pôle Promotion de la Connaissance).
-
-## Licence
-Licence Ouverte version 2.0 [etalab-2.0](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf)
-
-## État du projet
+# french-cities
+Boîte à outils sur les communes françaises : millésimage, reconnaissance de 
+départements ou de communes...
+
+
+# Installation
+
+`pip install french-cities[full]`
+
+Notez qu'à cette heure, `pynsee` ne supporte pas les projections de codes commune. 
+Dans l'immédiat, après avoir installé `french-cities` depuis pypi, il faut donc
+désinstaller `pynsee` puis réinstaller la version master courante depuis son repo 
+github :
+```
+pip uninstall pynsee
+pip install git+https://github.com/InseeFrLab/pynsee
+```
+
+L'installation "full" permet d'installer geopy qui est une dépendance 
+optionnelle utilisable en dernier ressort.
+
+# Configuration
+
+## Ajout des clefs API INSEE
+`french-cities` utilise `pynsee`, qui nécessite des cles API INSEE pour être 
+fonctionnel. Jusqu'à quatre clefs peuvent être spécifiées à l'aide de variables
+d'environnement :
+* insee_key
+* insee_secret, 
+* http_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
+* https_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
+
+Merci de se référer à [la documentation de `pynsee`](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
+pour plus d'information sur les clefs API et la configuration.
+
+A noter que la configuration des proxy par variable d'environnement sera 
+fonctionnelle pour à la fois `pynsee` et `geopy`.
+
+## Gestion des sessions web
+`pynsee` et `geopy` utilisent leur propres gestionnaires de session web. 
+Ainsi, les objets Session passés en argument à `french-cities` ne seront
+**PAS** partagés avec `pynsee` ou `geopy`. Cela explique la possibilité de 
+passer une session en argument alors même que des proxy professionnels peuvent 
+être spécifiés par variables d'environnement (pour `pynsee` et `geopy`).
+
+## Utilisation
+
+### Pourquoi french-cities ?
+Des packages et des API sont déjà disponibles pour des recherches usuelles. Par
+exemple, `pynsee` utilise les API de l'INSEE pour retrouver de multiples données
+(comme les départements, les régions, etc.) ; `geopy` peut également retrouver
+des communes à partir de leurs noms en s'appuyant sur la BAN (Base Adresse 
+Nationale) ou sur le service de géocodage Nominatim.
+
+La différence est que `french-cities` est optimisé pour travailler avec des données
+fournies sous la forme de Series ou DataFrames pandas. Ce package gérera mieux
+de gros volumes de données que ne le feraient des appels multiples à des API.
+
+### Trouver les départements
+`french-cities` peut retrouver un code département à partir de codes postaux ou 
+de codes communes officiels (COG/INSEE).
+
+Travailler à partir de codes postaux entraînera l'utilisation de la BAN (Base
+Adresse Nationale) et devrait fournir des résultats corrects. Le cas des codes
+Cedex n'étant que partiellement géré par la BAN, un appel est fait dans un
+second temps à l'[API d'OpenDataSoft](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr)
+construite sur la base des [travaux de Christian Quest](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
+Cette utilisation s'appuie sur un accès freemium non authentifié; l'utilisateur 
+du package est invité à contrôler les conditions générales d'utilisation de l'API auprès du
+fournisseur.
+
+Travailler à partir de codes communes officiels peut entraîner des résultats
+erronés pour des données anciennes, dans le cas de communes ayant changé de
+département (ce qui est relativement rare).
+Ce choix est délibéré : seuls les premiers caractères des codes commune sont
+utilisés pour la reconnaissance du département (algorithme rapide et qui donne
+des résultats corrects pour 99% des cas), par opposition à un requêtage
+systématique aux API (processus sans erreur mais long).
+
+```
+from french_cities import find_departements
+import pandas as pd
+
+df = pd.DataFrame(
+    {
+        "code_postal": ["59800", "97133", "20000"],
+        "code_commune": ["59350", "97701", "2A004"],
+        "communes": ["Lille", "Saint-Barthélémy", "Ajaccio"],
+        "deps": ["59", "977", "2A"],
+    }
+)
+df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
+df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
+
+print(df)
+```
+
+Pour une documentation complète sur la fonction `find_departements`, merci 
+d'utiliser la commande suivante :
+`help(find_departements)`.
+
+### Trouver les codes communes
+`french-cities` peut retrouver le code commune à partir de champs multiples.
+Il est capable de détecter certaines erreurs simples dans les champs (jusqu'à 
+une certaine limite).
+
+Les colonnes utilisées par l'algorithme pour cette détection sont (par ordre
+de priorité) :
+* 'x' et 'y' (dans ce cas, un code EPSG doit être explicitement donné);
+* 'postcode' et 'city'
+* 'address', 'postcode' et 'city'
+* 'department' et 'city'
+
+Il est à noter que l'algorithme peu faire être source d'erreur dès lors que
+la jointure spatiale (coordonnées x & y) sera sollicitée sur un millésime ancien.
+Les communes impactées sont les communes restaurées ("scission"), le flux de données
+spatialisées du COG servi par pynsee n'étant pas millésimé à ce jour.
+
+La reconnaissance syntaxique (champs postcode, city, address, departement) est
+basée sur la BAN (base adresse nationale). L'algorithme ne conservera pas de
+résultats insuffisamment fiables, mais des erreurs peuvent subsister (elles 
+seront dans ce cas cohérentes avec les résultats de la BAN).
+
+```
+from french_cities import find_city
+import pandas as pd
+
+df = pd.DataFrame(
+    [
+        {
+            "x": 2.294694,
+            "y": 48.858093,
+            "location": "Tour Eiffel",
+            "dep": "75",
+            "city": "Paris",
+            "address": "5 Avenue Anatole France",
+            "postcode": "75007",
+            "target": "75056",
+        },
+        {
+            "x": 8.738962,
+            "y": 41.919216,
+            "location": "mairie",
+            "dep": "2A",
+            "city": "Ajaccio",
+            "address": "Antoine Sérafini",
+            "postcode": "20000",
+            "target": "2A004",
+        },
+        {
+            "x": -52.334990,
+            "y": 4.938194,
+            "location": "mairie",
+            "dep": "973",
+            "city": "Cayenne",
+            "address": "1 rue de Rémire",
+            "postcode": "97300",
+            "target": "97302",
+        },
+        {
+            "x": np.nan,
+            "y": np.nan,
+            "location": "Erreur code postal Lille/Lyon",
+            "dep": "59",
+            "city": "Lille",
+            "address": "1 rue Faidherbe",
+            "postcode": "69000",
+            "target": "59350",
+        },
+    ]
+)
+df = find_city(df, epsg=4326)
+
+print(df)
+```
+
+Pour une documentation complète sur la fonction `find_city`, merci 
+d'utiliser la commande suivante :
+`help(find_city)`.
+
+**Nota** : pour activer l'utilisation de `geopy` (API Nominatim d'OpenStreeMap) 
+en dernier ressort, il convient d'utiliser l'argument `use_nominatim_backend=True`.
+
+### Projection de codes communes dans un millésime donné
+`french-cities` peut tenter de "projeter" un dataframe dans un millésime donné,
+la date initiale demeurant inconnue (voire inexistante, les cas de fichiers
+"multi-millésimés" étant fréquents dans la vie réelle).
+
+Des erreurs peuvent survenir, notamment pour les communes restaurées (dans la 
+mesure où la date initiale de la donnée est inconnue ou inexistante).
+
+Dans le cas où la date des données est connue, il peut être pertinent d'utiliser
+l'API de projection mise à disposition par l'INSEE et accessible au travers de 
+`pynsee`. Il convient de noter que cette utilisation peut être lente, dans la 
+mesure ou chaque commune devra être testée via l'API (qui n'autorise que 
+30 requêtes par minute).
+
+En substance, l'algorithme de `french-cities` contrôle si le code commune existe
+dans le millésime souhaité :
+* s'il existe il sera conservé (à l'approximation précédente près qui peut donc
+impacter les communes restaurées) ;
+* s'il n'existe pas, le code est recherché dans des millésimes antérieurs (et
+l'API de projection de l'INSEE sera mobilisée de manière ciblée).
+
+Cet algorithme va également :
+* convertir les codes des éventuels arrondissements municipaux en celui de leur
+commune de rattachement;
+* convertir les codes des communes associées et déléguées en celui de leur 
+commune de rattachement.
+
+```
+from french_cities import set_vintage
+import pandas as pd
+
+df = pd.DataFrame(
+    [
+        ["07180", "Fusion"],
+        ["02077", "Commune déléguée"],
+        ["02564", "Commune nouvelle"],
+        ["75101", "Arrondissement municipal"],
+        ["59298", "Commune associée"],
+        ["99999", "Code erroné"],
+        ["14472", "Oudon"],
+    ],
+    columns=["A", "Test"],
+    index=["A", "B", "C", "D", 1, 2, 3],
+)
+df = set_vintage(df, 2023, field="A")
+print(df)
+```
+
+Pour une documentation complète sur la fonction `set_vintage`, merci 
+d'utiliser la commande suivante :
+`help(set_vintage)`.
+
+## Documentation externe
+
+`french-cities` utilise plusieurs API externes. N'hésitez pas à consulter :
+* [documentation](https://adresse.data.gouv.fr/api-doc/adresse) (en Français) de l'API Adresse
+* [documentation](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr) (en Français) de l'API OpenDataSoft.
+* [Politique d'usage de Nominatim](https://operations.osmfoundation.org/policies/nominatim/)
+
+## Support
+En cas de bugues, merci d'ouvrir un ticket [sur le repo](https://github.com/tgrandje/french-cities/issues).
+
+## Auteur
+Thomas GRANDJEAN (DREAL Hauts-de-France, service Information, Développement Durable et Évaluation Environnementale, pôle Promotion de la Connaissance).
+
+## Licence
+Licence Ouverte version 2.0 [etalab-2.0](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf)
+
+## État du projet
 Phase de test.
```

### Comparing `french_cities-0.1.0a9/README.md` & `french_cities-0.1.1a1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,225 +1,239 @@
-# french-cities
-Toolbox on french cities: set vintage, find departments, find cities...
-
-
-# Installation
-
-`pip install french-cities`
-
-Note that at this instant, `pynsee` doesn't support communal projection.
-After installing `french-cities` from pypi, please uninstall pynsee and replace
-it with the current master:
-```
-pip uninstall pynsee
-pip install git+https://github.com/InseeFrLab/pynsee
-```
-
-
-
-# Configuration
-
-## Setting INSEE's API keys
-`french-cities` uses `pynsee` under the hood. For it to work, you need to set
-the credentials up. You can set up to four environment variables:
-* insee_key
-* insee_secret, 
-* http_proxy (if accessing web behind a corporate proxy)
-* https_proxy (if accessing web behind a corporate proxy)
-
-Please refer to [`pynsee`'s documentation](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
-to help configure the API's access.
-
-## Session management
-Note that `pynsee` uses it's own web session. Every Session object you will pass
-to `french-cities` will **NOT** be shared with `pynsee`. This explains the
-possibility to pass a session as an argument to `french-cities` functions,
-even if you had to configure the corporate proxy through environment variables
-for `pynsee`.
-
-## Basic usage
-
-### Why french-cities?
-There are already available packages and APIs meant to be used for basic french
-cities management. For instance, `pynsee` uses the INSEE's API to retrieve
-multiple data (including departement, region, ...). `geopy` can also retrieve
-cities from their names using the BAN (Base Adresse Nationale) API or the 
-Nominatim geocoding service.
-
-The difference is that `french-cities` is primarly meant to perform against whole
-pandas series/dataframes. It should handle better performance than multiple API 
-calls and will optimize the call to each endpoints.
-
-### Retrieve departements' codes
-`french-cities` can retrieve departement's codes from postal codes or official
-(COG/INSEE) codes. 
-
-Working from postal codes will make use of the BAN (Base Adresse Nationale)
-and should return correct results. The case of "Cedex" codes is only partially
-covered by the BAN, so [OpenDataSoft's API](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr),
-constructed upon [Christian Quest works](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
-This consumes the freemium API and no authentication is included:
-the user of the present package should check the current API's legal terms
-directly on OpenDataSoft's website.
-
-Working from official codes may give wrong results when working on an old
-dataset and with cities which have changed of departments (which is rarely seen). 
-This is deliberate: it will use the first characters of the cities' codes 
-(which is a fast process and 99% accurate) instead of using an API (which is
-lengthy though foolproof).
-
-```
-from french_cities import find_departements
-import pandas as pd
-
-df = pd.DataFrame(
-    {
-        "code_postal": ["59800", "97133", "20000"],
-        "code_commune": ["59350", "97701", "2A004"],
-        "communes": ["Lille", "Saint-Barthélémy", "Ajaccio"],
-        "deps": ["59", "977", "2A"],
-    }
-)
-df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
-df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
-
-print(df)
-```
-
-For a complete documentation on `find_departements`, please type 
-`help(find_departements)`.
-
-### Retrieve cities' codes
-`french-cities` can retrieve cities' codes from multiple fields. It will work
-out basic mistakes (up to a certain limit).
-
-The columns used by the algorithm can be (in the order of precedence used by
-the algorithm):
-* 'x' and 'y' (in that case, epsg must be explicitly given);
-* 'postcode' and 'city'
-* 'address', 'postcode' and 'city'
-* 'department' and 'city'
-
-Note that the algorithm can (and will) make errors using xy coordinates on a 
-older vintage (ie different from the current one) in the case of historic 
-splitting of cities (the geographic files are not vintaged yet).
-
-The lexical (postcode, city, address, departement) recognition is based on the
-BAN (base adresse nationale). The algorithm won't collect underscored
-results, but failures may still occure (and will be in accordance with the 
-BAN's failures).
-
-```
-from french_cities import find_city
-import pandas as pd
-
-df = pd.DataFrame(
-    [
-        {
-            "x": 2.294694,
-            "y": 48.858093,
-            "location": "Tour Eiffel",
-            "dep": "75",
-            "city": "Paris",
-            "address": "5 Avenue Anatole France",
-            "postcode": "75007",
-            "target": "75056",
-        },
-        {
-            "x": 8.738962,
-            "y": 41.919216,
-            "location": "mairie",
-            "dep": "2A",
-            "city": "Ajaccio",
-            "address": "Antoine Sérafini",
-            "postcode": "20000",
-            "target": "2A004",
-        },
-        {
-            "x": -52.334990,
-            "y": 4.938194,
-            "location": "mairie",
-            "dep": "973",
-            "city": "Cayenne",
-            "address": "1 rue de Rémire",
-            "postcode": "97300",
-            "target": "97302",
-        },
-        {
-            "x": np.nan,
-            "y": np.nan,
-            "location": "Erreur code postal Lille/Lyon",
-            "dep": "59",
-            "city": "Lille",
-            "address": "1 rue Faidherbe",
-            "postcode": "69000",
-            "target": "59350",
-        },
-    ]
-)
-df = find_city(df, epsg=4326)
-
-print(df)
-```
-
-For a complete documentation on `find_city`, please type 
-`help(find_city)`.
-
-### Set vintage to cities' codes
-`french-cities` can try to project a given dataframe into a set vintage,
-starting from an unknown vintage (or even a non-vintaged dataset, which is 
-often the case).
-
-Error may occur for splitted cities as the starting vintage is unknown
-(or inexistant).
-
-In case of a known starting vintage, you can make use of
-INSEE's projection API (with `pynsee`). Note that this might prove slower as
-each row will have to induce a request to the API (which allows up to 
-30 requests/minute).
-
-Basically, the algorithm of `french-cities` will try to see if a given city
-code exists in the desired vintage:
-* if yes, it will be kept (we the aforementionned approximation regarding
-restored cities);
-* if not, it will look in older vintages and make use of INSEE's projection API.
-
-This algorithm will also:
-* convert communal districts' into cities' codes;
-* convert delegated or associated cities' codes into it's parent's.
-
-```
-from french_cities import set_vintage
-import pandas as pd
-
-df = pd.DataFrame(
-    [
-        ["07180", "Fusion"],
-        ["02077", "Commune déléguée"],
-        ["02564", "Commune nouvelle"],
-        ["75101", "Arrondissement municipal"],
-        ["59298", "Commune associée"],
-        ["99999", "Code erroné"],
-        ["14472", "Oudon"],
-    ],
-    columns=["A", "Test"],
-    index=["A", "B", "C", "D", 1, 2, 3],
-)
-df = set_vintage(df, 2023, field="A")
-print(df)
-```
-
-For a complete documentation on `set_vintage`, please type 
-`help(set_vintage)`.
-
-
-## Support
-In case of bugs, please open an issue [on the repo](https://github.com/tgrandje/french-cities/issues).
-
-## Author
-Thomas GRANDJEAN (DREAL Hauts-de-France, service Information, Développement Durable et Évaluation Environnementale, pôle Promotion de la Connaissance).
-
-## Licence
-Licence Ouverte version 2.0 [etalab-2.0](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf)
-
-## Project Status
+# french-cities
+Toolbox on french cities: set vintage, find departments, find cities...
+
+
+# Installation
+
+`pip install french-cities[full]`
+
+Note that at this instant, `pynsee` doesn't support communal projection.
+After installing `french-cities` from pypi, please uninstall pynsee and replace
+it with the current master:
+```
+pip uninstall pynsee
+pip install git+https://github.com/InseeFrLab/pynsee
+```
+
+Note that the "full" installation will also install geopy, which might use
+Nominatim API for city recognition as a last resort.
+
+
+# Configuration
+
+## Setting INSEE's API keys
+`french-cities` uses `pynsee` under the hood. For it to work, you need to set
+the credentials up. You can set up to four environment variables:
+* insee_key
+* insee_secret, 
+* http_proxy (if accessing web behind a corporate proxy)
+* https_proxy (if accessing web behind a corporate proxy)
+
+Please refer to [`pynsee`'s documentation](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
+to help configure the API's access.
+
+Note that setting environment variable for proxy will set it for both `pynsee`
+and `geopy`.
+
+## Session management
+Note that `pynsee` and `geopy` use their own web session. Every Session object 
+you will pass to `french-cities` will **NOT** be shared with `pynsee` or `geopy`. 
+This explains the possibility to pass a session as an argument to `french-cities` 
+functions, even if you had to configure the corporate proxy through environment 
+variables for `pynsee` and `geopy`.
+
+## Basic usage
+
+### Why french-cities?
+There are already available packages and APIs meant to be used for basic french
+cities management. For instance, `pynsee` uses the INSEE's API to retrieve
+multiple data (including departement, region, ...). `geopy` can also retrieve
+cities from their names using the BAN (Base Adresse Nationale) API or the 
+Nominatim geocoding service.
+
+The difference is that `french-cities` is primarly meant to perform against whole
+pandas series/dataframes. It should handle better performance than multiple API 
+calls and will optimize the call to each endpoints.
+
+### Retrieve departements' codes
+`french-cities` can retrieve departement's codes from postal codes or official
+(COG/INSEE) codes. 
+
+Working from postal codes will make use of the BAN (Base Adresse Nationale)
+and should return correct results. The case of "Cedex" codes is only partially
+covered by the BAN, so [OpenDataSoft's API](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr),
+constructed upon [Christian Quest works](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
+This consumes the freemium API and no authentication is included:
+the user of the present package should check the current API's legal terms
+directly on OpenDataSoft's website.
+
+Working from official codes may give wrong results when working on an old
+dataset and with cities which have changed of departments (which is rarely seen). 
+This is deliberate: it will use the first characters of the cities' codes 
+(which is a fast process and 99% accurate) instead of using an API (which is
+lengthy though foolproof).
+
+```
+from french_cities import find_departements
+import pandas as pd
+
+df = pd.DataFrame(
+    {
+        "code_postal": ["59800", "97133", "20000"],
+        "code_commune": ["59350", "97701", "2A004"],
+        "communes": ["Lille", "Saint-Barthélémy", "Ajaccio"],
+        "deps": ["59", "977", "2A"],
+    }
+)
+df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
+df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
+
+print(df)
+```
+
+For a complete documentation on `find_departements`, please type 
+`help(find_departements)`.
+
+### Retrieve cities' codes
+`french-cities` can retrieve cities' codes from multiple fields. It will work
+out basic mistakes (up to a certain limit).
+
+The columns used by the algorithm can be (in the order of precedence used by
+the algorithm):
+* 'x' and 'y' (in that case, epsg must be explicitly given);
+* 'postcode' and 'city'
+* 'address', 'postcode' and 'city'
+* 'department' and 'city'
+
+Note that the algorithm can (and will) make errors using xy coordinates on a 
+older vintage (ie different from the current one) in the case of historic 
+splitting of cities (the geographic files are not vintaged yet).
+
+The lexical (postcode, city, address, departement) recognition is based on the
+BAN (base adresse nationale). The algorithm won't collect underscored
+results, but failures may still occure (and will be in accordance with the 
+BAN's failures).
+
+```
+from french_cities import find_city
+import pandas as pd
+
+df = pd.DataFrame(
+    [
+        {
+            "x": 2.294694,
+            "y": 48.858093,
+            "location": "Tour Eiffel",
+            "dep": "75",
+            "city": "Paris",
+            "address": "5 Avenue Anatole France",
+            "postcode": "75007",
+            "target": "75056",
+        },
+        {
+            "x": 8.738962,
+            "y": 41.919216,
+            "location": "mairie",
+            "dep": "2A",
+            "city": "Ajaccio",
+            "address": "Antoine Sérafini",
+            "postcode": "20000",
+            "target": "2A004",
+        },
+        {
+            "x": -52.334990,
+            "y": 4.938194,
+            "location": "mairie",
+            "dep": "973",
+            "city": "Cayenne",
+            "address": "1 rue de Rémire",
+            "postcode": "97300",
+            "target": "97302",
+        },
+        {
+            "x": np.nan,
+            "y": np.nan,
+            "location": "Erreur code postal Lille/Lyon",
+            "dep": "59",
+            "city": "Lille",
+            "address": "1 rue Faidherbe",
+            "postcode": "69000",
+            "target": "59350",
+        },
+    ]
+)
+df = find_city(df, epsg=4326)
+
+print(df)
+```
+
+For a complete documentation on `find_city`, please type 
+`help(find_city)`.
+
+**Note** : to activate `geopy` (Nominatim API from OpenStreeMap) usage in last 
+resort, you will need to use the argument `use_nominatim_backend=True`.
+
+### Set vintage to cities' codes
+`french-cities` can try to project a given dataframe into a set vintage,
+starting from an unknown vintage (or even a non-vintaged dataset, which is 
+often the case).
+
+Error may occur for splitted cities as the starting vintage is unknown
+(or inexistant).
+
+In case of a known starting vintage, you can make use of
+INSEE's projection API (with `pynsee`). Note that this might prove slower as
+each row will have to induce a request to the API (which allows up to 
+30 requests/minute).
+
+Basically, the algorithm of `french-cities` will try to see if a given city
+code exists in the desired vintage:
+* if yes, it will be kept (we the aforementionned approximation regarding
+restored cities);
+* if not, it will look in older vintages and make use of INSEE's projection API.
+
+This algorithm will also:
+* convert communal districts' into cities' codes;
+* convert delegated or associated cities' codes into it's parent's.
+
+```
+from french_cities import set_vintage
+import pandas as pd
+
+df = pd.DataFrame(
+    [
+        ["07180", "Fusion"],
+        ["02077", "Commune déléguée"],
+        ["02564", "Commune nouvelle"],
+        ["75101", "Arrondissement municipal"],
+        ["59298", "Commune associée"],
+        ["99999", "Code erroné"],
+        ["14472", "Oudon"],
+    ],
+    columns=["A", "Test"],
+    index=["A", "B", "C", "D", 1, 2, 3],
+)
+df = set_vintage(df, 2023, field="A")
+print(df)
+```
+
+For a complete documentation on `set_vintage`, please type 
+`help(set_vintage)`.
+
+## External documentation
+
+`french-cities` makes use of multiple APIs. Please read :
+* [documentation](https://adresse.data.gouv.fr/api-doc/adresse) (in french) on API Adresse
+* [documentation](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr) (in french) on OpenDataSoft API
+* [Nominatim Usage Policy](https://operations.osmfoundation.org/policies/nominatim/)
+
+## Support
+In case of bugs, please open an issue [on the repo](https://github.com/tgrandje/french-cities/issues).
+
+## Author
+Thomas GRANDJEAN (DREAL Hauts-de-France, service Information, Développement Durable et Évaluation Environnementale, pôle Promotion de la Connaissance).
+
+## Licence
+Licence Ouverte version 2.0 [etalab-2.0](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf)
+
+## Project Status
 Test phase.
```

### Comparing `french_cities-0.1.0a9/PKG-INFO` & `french_cities-0.1.1a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.0a9
+Version: 0.1.1a1
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
@@ -12,17 +12,19 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
+Provides-Extra: full
 Requires-Dist: geopandas (>=0.13.2,<0.14.0)
+Requires-Dist: geopy (>=2.3.0,<3.0.0) ; extra == "full"
+Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pebble (>=5.0.3,<6.0.0)
 Requires-Dist: pynsee (>=0.1.4,<0.2.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
@@ -34,24 +36,26 @@
 
 # french-cities
 Toolbox on french cities: set vintage, find departments, find cities...
 
 
 # Installation
 
-`pip install french-cities`
+`pip install french-cities[full]`
 
 Note that at this instant, `pynsee` doesn't support communal projection.
 After installing `french-cities` from pypi, please uninstall pynsee and replace
 it with the current master:
 ```
 pip uninstall pynsee
 pip install git+https://github.com/InseeFrLab/pynsee
 ```
 
+Note that the "full" installation will also install geopy, which might use
+Nominatim API for city recognition as a last resort.
 
 
 # Configuration
 
 ## Setting INSEE's API keys
 `french-cities` uses `pynsee` under the hood. For it to work, you need to set
 the credentials up. You can set up to four environment variables:
@@ -59,20 +63,23 @@
 * insee_secret, 
 * http_proxy (if accessing web behind a corporate proxy)
 * https_proxy (if accessing web behind a corporate proxy)
 
 Please refer to [`pynsee`'s documentation](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
 to help configure the API's access.
 
+Note that setting environment variable for proxy will set it for both `pynsee`
+and `geopy`.
+
 ## Session management
-Note that `pynsee` uses it's own web session. Every Session object you will pass
-to `french-cities` will **NOT** be shared with `pynsee`. This explains the
-possibility to pass a session as an argument to `french-cities` functions,
-even if you had to configure the corporate proxy through environment variables
-for `pynsee`.
+Note that `pynsee` and `geopy` use their own web session. Every Session object 
+you will pass to `french-cities` will **NOT** be shared with `pynsee` or `geopy`. 
+This explains the possibility to pass a session as an argument to `french-cities` 
+functions, even if you had to configure the corporate proxy through environment 
+variables for `pynsee` and `geopy`.
 
 ## Basic usage
 
 ### Why french-cities?
 There are already available packages and APIs meant to be used for basic french
 cities management. For instance, `pynsee` uses the INSEE's API to retrieve
 multiple data (including departement, region, ...). `geopy` can also retrieve
@@ -194,14 +201,17 @@
 
 print(df)
 ```
 
 For a complete documentation on `find_city`, please type 
 `help(find_city)`.
 
+**Note** : to activate `geopy` (Nominatim API from OpenStreeMap) usage in last 
+resort, you will need to use the argument `use_nominatim_backend=True`.
+
 ### Set vintage to cities' codes
 `french-cities` can try to project a given dataframe into a set vintage,
 starting from an unknown vintage (or even a non-vintaged dataset, which is 
 often the case).
 
 Error may occur for splitted cities as the starting vintage is unknown
 (or inexistant).
@@ -241,14 +251,20 @@
 df = set_vintage(df, 2023, field="A")
 print(df)
 ```
 
 For a complete documentation on `set_vintage`, please type 
 `help(set_vintage)`.
 
+## External documentation
+
+`french-cities` makes use of multiple APIs. Please read :
+* [documentation](https://adresse.data.gouv.fr/api-doc/adresse) (in french) on API Adresse
+* [documentation](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr) (in french) on OpenDataSoft API
+* [Nominatim Usage Policy](https://operations.osmfoundation.org/policies/nominatim/)
 
 ## Support
 In case of bugs, please open an issue [on the repo](https://github.com/tgrandje/french-cities/issues).
 
 ## Author
 Thomas GRANDJEAN (DREAL Hauts-de-France, service Information, Développement Durable et Évaluation Environnementale, pôle Promotion de la Connaissance).
 
@@ -260,45 +276,51 @@
 # french-cities
 Boîte à outils sur les communes françaises : millésimage, reconnaissance de 
 départements ou de communes...
 
 
 # Installation
 
-`pip install french-cities`
+`pip install french-cities[full]`
 
 Notez qu'à cette heure, `pynsee` ne supporte pas les projections de codes commune. 
 Dans l'immédiat, après avoir installé `french-cities` depuis pypi, il faut donc
 désinstaller `pynsee` puis réinstaller la version master courante depuis son repo 
 github :
 ```
 pip uninstall pynsee
 pip install git+https://github.com/InseeFrLab/pynsee
 ```
 
+L'installation "full" permet d'installer geopy qui est une dépendance 
+optionnelle utilisable en dernier ressort.
+
 # Configuration
 
 ## Ajout des clefs API INSEE
 `french-cities` utilise `pynsee`, qui nécessite des cles API INSEE pour être 
 fonctionnel. Jusqu'à quatre clefs peuvent être spécifiées à l'aide de variables
 d'environnement :
 * insee_key
 * insee_secret, 
 * http_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
 * https_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
 
 Merci de se référer à [la documentation de `pynsee`](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
 pour plus d'information sur les clefs API et la configuration.
 
+A noter que la configuration des proxy par variable d'environnement sera 
+fonctionnelle pour à la fois `pynsee` et `geopy`.
+
 ## Gestion des sessions web
-`pynsee` utilise son propre gestionnaire de session web. 
+`pynsee` et `geopy` utilisent leur propres gestionnaires de session web. 
 Ainsi, les objets Session passés en argument à `french-cities` ne seront
-**PAS** partagés avec `pynsee`. Cela explique la possibilité de passer une 
-session en argument alors même que des proxy professionnels peuvent être 
-spécifiés par variables d'environnement (pour `pynsee`).
+**PAS** partagés avec `pynsee` ou `geopy`. Cela explique la possibilité de 
+passer une session en argument alors même que des proxy professionnels peuvent 
+être spécifiés par variables d'environnement (pour `pynsee` et `geopy`).
 
 ## Utilisation
 
 ### Pourquoi french-cities ?
 Des packages et des API sont déjà disponibles pour des recherches usuelles. Par
 exemple, `pynsee` utilise les API de l'INSEE pour retrouver de multiples données
 (comme les départements, les régions, etc.) ; `geopy` peut également retrouver
@@ -427,14 +449,17 @@
 print(df)
 ```
 
 Pour une documentation complète sur la fonction `find_city`, merci 
 d'utiliser la commande suivante :
 `help(find_city)`.
 
+**Nota** : pour activer l'utilisation de `geopy` (API Nominatim d'OpenStreeMap) 
+en dernier ressort, il convient d'utiliser l'argument `use_nominatim_backend=True`.
+
 ### Projection de codes communes dans un millésime donné
 `french-cities` peut tenter de "projeter" un dataframe dans un millésime donné,
 la date initiale demeurant inconnue (voire inexistante, les cas de fichiers
 "multi-millésimés" étant fréquents dans la vie réelle).
 
 Des erreurs peuvent survenir, notamment pour les communes restaurées (dans la 
 mesure où la date initiale de la donnée est inconnue ou inexistante).
@@ -479,14 +504,20 @@
 print(df)
 ```
 
 Pour une documentation complète sur la fonction `set_vintage`, merci 
 d'utiliser la commande suivante :
 `help(set_vintage)`.
 
+## Documentation externe
+
+`french-cities` utilise plusieurs API externes. N'hésitez pas à consulter :
+* [documentation](https://adresse.data.gouv.fr/api-doc/adresse) (en Français) de l'API Adresse
+* [documentation](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr) (en Français) de l'API OpenDataSoft.
+* [Politique d'usage de Nominatim](https://operations.osmfoundation.org/policies/nominatim/)
 
 ## Support
 En cas de bugues, merci d'ouvrir un ticket [sur le repo](https://github.com/tgrandje/french-cities/issues).
 
 ## Auteur
 Thomas GRANDJEAN (DREAL Hauts-de-France, service Information, Développement Durable et Évaluation Environnementale, pôle Promotion de la Connaissance).
```

