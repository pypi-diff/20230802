# Comparing `tmp/data_inclusion_schema-0.9.0.tar.gz` & `tmp/data_inclusion_schema-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_inclusion_schema-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "data_inclusion_schema-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `data_inclusion_schema-0.9.0.tar` & `data_inclusion_schema-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2422 2023-06-30 08:51:01.949597 data_inclusion_schema-0.9.0/README.md
--rw-r--r--   0        0        0     1276 2023-06-30 08:51:01.949597 data_inclusion_schema-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/__init__.py
--rw-r--r--   0        0        0     1526 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/__main__.py
--rw-r--r--   0        0        0     1217 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/base.py
--rw-r--r--   0        0        0      466 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/code_officiel_geographique.py
--rw-r--r--   0        0        0      912 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/frais.py
--rw-r--r--   0        0        0     7575 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/labels_nationaux.py
--rw-r--r--   0        0        0     5153 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/models.py
--rw-r--r--   0        0        0      264 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/modes_accueil.py
--rw-r--r--   0        0        0     1446 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/modes_orientation.py
--rw-r--r--   0        0        0     1687 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/profils.py
--rw-r--r--   0        0        0    25488 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/thematiques.py
--rw-r--r--   0        0        0     1955 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_services.py
--rw-r--r--   0        0        0     7581 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_structures.py
--rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 data_inclusion_schema-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2422 2023-08-02 09:57:41.802390 data_inclusion_schema-0.9.1/README.md
+-rw-r--r--   0        0        0     1276 2023-08-02 09:57:41.802390 data_inclusion_schema-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/__init__.py
+-rw-r--r--   0        0        0     1526 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/__main__.py
+-rw-r--r--   0        0        0     1217 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/base.py
+-rw-r--r--   0        0        0      466 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/code_officiel_geographique.py
+-rw-r--r--   0        0        0      912 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/frais.py
+-rw-r--r--   0        0        0     7575 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/labels_nationaux.py
+-rw-r--r--   0        0        0     5601 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/models.py
+-rw-r--r--   0        0        0      264 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/modes_accueil.py
+-rw-r--r--   0        0        0     1446 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/modes_orientation.py
+-rw-r--r--   0        0        0     1687 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/profils.py
+-rw-r--r--   0        0        0    25487 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/thematiques.py
+-rw-r--r--   0        0        0     1955 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/typologies_de_services.py
+-rw-r--r--   0        0        0     7581 2023-08-02 09:57:41.806390 data_inclusion_schema-0.9.1/src/data_inclusion/schema/typologies_de_structures.py
+-rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 data_inclusion_schema-0.9.1/PKG-INFO
```

### Comparing `data_inclusion_schema-0.9.0/README.md` & `data_inclusion_schema-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/pyproject.toml` & `data_inclusion_schema-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "data-inclusion-schema"
-version = "0.9.0"
+version = "0.9.1"
 description = "Schéma de l'offre d'insertion"
 authors = [{ name = "data.inclusion", email = "data.inclusion@beta.gouv.fr" }]
 readme = "README.md"
 dynamic = []
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-dependencies = ["pydantic[email]>=1.9.1,<2.0.0"]
+dependencies = ["pydantic[email]>=2.1.1,<3.0.0"]
 
 
 [project.urls]
 Home = "https://www.data.inclusion.beta.gouv.fr"
 Documentation = "https://www.data.inclusion.beta.gouv.fr/schemas-de-donnees-de-loffre/schema-des-structures-et-services-dinsertion"
 Source = "https://github.com/betagouv/data-inclusion-schema"
```

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/__main__.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/__main__.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/base.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/base.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/frais.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/frais.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/labels_nationaux.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/labels_nationaux.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/models.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import date, datetime
 from typing import Optional
 
 import pydantic
-from pydantic import BaseModel, EmailStr, Extra, HttpUrl, constr
+from pydantic import BaseModel, ConfigDict, EmailStr, HttpUrl, StringConstraints
+from typing_extensions import Annotated
 
 from data_inclusion.schema.code_officiel_geographique import TypeCOG
 from data_inclusion.schema.frais import Frais
 from data_inclusion.schema.labels_nationaux import LabelNational
 from data_inclusion.schema.modes_accueil import ModeAccueil
 from data_inclusion.schema.modes_orientation import (
     ModeOrientationAccompagnateur,
@@ -15,129 +16,145 @@
 from data_inclusion.schema.profils import Profil
 from data_inclusion.schema.thematiques import Thematique
 from data_inclusion.schema.typologies_de_services import TypologieService
 from data_inclusion.schema.typologies_de_structures import Typologie
 
 
 class Service(BaseModel):
+    model_config = ConfigDict(extra="forbid")
+
+    # fields
     id: str
-    structure_id: Optional[str]
+    structure_id: Optional[str] = None
     source: str
     nom: str
-    presentation_resume: Optional[constr(max_length=280)]
-    presentation_detail: Optional[str]
-    types: Optional[list[TypologieService]]
-    thematiques: Optional[list[Thematique]]
-    prise_rdv: Optional[HttpUrl]
-    frais: Optional[list[Frais]]
-    frais_autres: Optional[str]
-    profils: Optional[list[Profil]]
-    pre_requis: Optional[str]
-    cumulable: Optional[bool]
-    justificatifs: Optional[str]
-    formulaire_en_ligne: Optional[HttpUrl]
-    commune: Optional[str]
-    code_postal: Optional[constr(min_length=5, max_length=5, regex=r"^\d{5}$")]
-    code_insee: Optional[constr(min_length=5, max_length=5)]
-    adresse: Optional[str]
-    complement_adresse: Optional[str]
-    longitude: Optional[float]
-    latitude: Optional[float]
-    recurrence: Optional[str]
-    date_creation: Optional[date]
-    date_suspension: Optional[date]
-    lien_source: Optional[HttpUrl]
-    telephone: Optional[str]
-    courriel: Optional[EmailStr]
-    contact_public: Optional[bool]
-    date_maj: Optional[date | datetime]
-    modes_accueil: Optional[list[ModeAccueil]]
-    zone_diffusion_type: Optional[TypeCOG]
+    presentation_resume: Optional[
+        Annotated[str, StringConstraints(max_length=280)]
+    ] = None
+    presentation_detail: Optional[str] = None
+    types: Optional[list[TypologieService]] = None
+    thematiques: Optional[list[Thematique]] = None
+    prise_rdv: Optional[HttpUrl] = None
+    frais: Optional[list[Frais]] = None
+    frais_autres: Optional[str] = None
+    profils: Optional[list[Profil]] = None
+    pre_requis: Optional[str] = None
+    cumulable: Optional[bool] = None
+    justificatifs: Optional[str] = None
+    formulaire_en_ligne: Optional[HttpUrl] = None
+    commune: Optional[str] = None
+    code_postal: Optional[
+        Annotated[
+            str, StringConstraints(min_length=5, max_length=5, pattern=r"^\d{5}$")
+        ]
+    ] = None
+    code_insee: Optional[
+        Annotated[str, StringConstraints(min_length=5, max_length=5)]
+    ] = None
+    adresse: Optional[str] = None
+    complement_adresse: Optional[str] = None
+    longitude: Optional[float] = None
+    latitude: Optional[float] = None
+    recurrence: Optional[str] = None
+    date_creation: Optional[date] = None
+    date_suspension: Optional[date] = None
+    lien_source: Optional[HttpUrl] = None
+    telephone: Optional[str] = None
+    courriel: Optional[EmailStr] = None
+    contact_public: Optional[bool] = None
+    date_maj: Optional[date | datetime] = None
+    modes_accueil: Optional[list[ModeAccueil]] = None
+    zone_diffusion_type: Optional[TypeCOG] = None
     zone_diffusion_code: Optional[
-        constr(regex=r"^\w{5}$")  # code commune
-        | constr(regex=r"^\d{9}$")  # code epci
-        | constr(regex=r"^\w{2,3}$")  # code departement
-        | constr(regex=r"^\d{2}$")  # code region
-    ]
-    zone_diffusion_nom: Optional[str]
-    contact_nom_prenom: Optional[str]
-    modes_orientation_beneficiaire: Optional[list[ModeOrientationBeneficiaire]]
-    modes_orientation_accompagnateur: Optional[list[ModeOrientationAccompagnateur]]
-
-    class Config:
-        extra = Extra.forbid
+        Annotated[str, StringConstraints(pattern=r"^\w{5}$")]  # code commune
+        | Annotated[str, StringConstraints(pattern=r"^\d{9}$")]  # code epci
+        | Annotated[str, StringConstraints(pattern=r"^\w{2,3}$")]  # code departement
+        | Annotated[str, StringConstraints(pattern=r"^\d{2}$")]  # code region
+    ] = None
+    zone_diffusion_nom: Optional[str] = None
+    contact_nom_prenom: Optional[str] = None
+    modes_orientation_beneficiaire: Optional[list[ModeOrientationBeneficiaire]] = None
+    modes_orientation_accompagnateur: Optional[
+        list[ModeOrientationAccompagnateur]
+    ] = None
 
 
 class Structure(BaseModel):
+    model_config = ConfigDict(extra="forbid")
+
+    # fields
     id: str
-    siret: Optional[constr(min_length=14, max_length=14, regex=r"^\d{14}$")]
-    rna: Optional[constr(min_length=10, max_length=10, regex=r"^W\d{9}$")]
+    siret: Optional[
+        Annotated[
+            str, StringConstraints(min_length=14, max_length=14, pattern=r"^\d{14}$")
+        ]
+    ] = None
+    rna: Optional[
+        Annotated[
+            str, StringConstraints(min_length=10, max_length=10, pattern=r"^W\d{9}$")
+        ]
+    ] = None
     nom: str
     commune: str
-    code_postal: constr(min_length=5, max_length=5, regex=r"^\d{5}$")
-    code_insee: Optional[constr(min_length=5, max_length=5)]
+    code_postal: Annotated[
+        str, StringConstraints(min_length=5, max_length=5, pattern=r"^\d{5}$")
+    ]
+    code_insee: Optional[
+        Annotated[str, StringConstraints(min_length=5, max_length=5)]
+    ] = None
     adresse: str
-    complement_adresse: Optional[str]
-    longitude: Optional[float]
-    latitude: Optional[float]
-    typologie: Optional[Typologie]
-    telephone: Optional[str]
-    courriel: Optional[EmailStr]
-    site_web: Optional[HttpUrl]
-    presentation_resume: Optional[constr(max_length=280)]
-    presentation_detail: Optional[str]
-    source: Optional[str]
+    complement_adresse: Optional[str] = None
+    longitude: Optional[float] = None
+    latitude: Optional[float] = None
+    typologie: Optional[Typologie] = None
+    telephone: Optional[str] = None
+    courriel: Optional[EmailStr] = None
+    site_web: Optional[HttpUrl] = None
+    presentation_resume: Optional[
+        Annotated[str, StringConstraints(max_length=280)]
+    ] = None
+    presentation_detail: Optional[str] = None
+    source: Optional[str] = None
     date_maj: date | datetime
     antenne: bool = False
-    lien_source: Optional[HttpUrl]
-    horaires_ouverture: Optional[str]
-    accessibilite: Optional[HttpUrl]
-    labels_nationaux: Optional[list[LabelNational]]
-    labels_autres: Optional[list[str]]
-    thematiques: Optional[list[Thematique]]
-
-    class Config:
-        extra = Extra.forbid
+    lien_source: Optional[HttpUrl] = None
+    horaires_ouverture: Optional[str] = None
+    accessibilite: Optional[HttpUrl] = None
+    labels_nationaux: Optional[list[LabelNational]] = None
+    labels_autres: Optional[list[str]] = None
+    thematiques: Optional[list[Thematique]] = None
 
 
 def generate_structures_json_schema():
     """Generate the structures file json schema from the `Structure` model."""
 
-    # json schema for a file containing a **list** of structures
+    adapter = pydantic.TypeAdapter(list[Structure])
+    schema = adapter.json_schema()
+
     return {
         "title": "Structures de l'insertion",
         "$schema": "http://json-schema.org/draft-07/schema",
         "$id": (
             "https://raw.githubusercontent.com/betagouv/data-inclusion-schema"
             "/main/structures.json"
         ),
         "description": "",
-        "type": "array",
-        "items": {
-            "$ref": "#/definitions/Structure",
-        },
-        # Pydantic generates the json schema of a **single** structure from the
-        # `Structure` model. Only the definitions are extracted.
-        "definitions": pydantic.schema_of(Structure)["definitions"],
+        **schema,
     }
 
 
 def generate_services_json_schema():
     """Generate the services file json schema from the `Service` model."""
 
-    # json schema for a file containing a **list** of services
+    adapter = pydantic.TypeAdapter(list[Service])
+    schema = adapter.json_schema()
+
     return {
         "title": "Services de l'insertion",
         "$schema": "http://json-schema.org/draft-07/schema",
         "$id": (
             "https://raw.githubusercontent.com/betagouv/data-inclusion-schema"
             "/main/services.json"
         ),
         "description": "",
-        "type": "array",
-        "items": {
-            "$ref": "#/definitions/Service",
-        },
-        # Pydantic generates the json schema of a **single** service from the
-        # `Service` model. Only the definitions are extracted.
-        "definitions": pydantic.schema_of(Service)["definitions"],
+        **schema,
     }
```

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/modes_orientation.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/modes_orientation.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/profils.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/profils.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/thematiques.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/thematiques.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,15 +675,15 @@
     SANTE__ACCES_AUX_SOINS = (
         "sante--acces-aux-soins",
         "Accès aux soins",
         None,
     )
     SANTE__DIAGNOSTIC_ET_ACCOMPAGNEMENT_A_LEMPLOYABILITE = (
         "sante--diagnostic-et-accompagnement-a-lemployabilite",
-        "Diagnostic et accompagnement à l’employabailité",
+        "Diagnostic et accompagnement à l’employabilité",
         None,
     )
 
     SE_FORMER = (
         "se-former",
         "Se former",
         None,
```

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_services.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/typologies_de_services.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_structures.py` & `data_inclusion_schema-0.9.1/src/data_inclusion/schema/typologies_de_structures.py`

 * *Files identical despite different names*

### Comparing `data_inclusion_schema-0.9.0/PKG-INFO` & `data_inclusion_schema-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: data-inclusion-schema
-Version: 0.9.0
+Version: 0.9.1
 Summary: Schéma de l'offre d'insertion
 Author-email: "data.inclusion" <data.inclusion@beta.gouv.fr>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: pydantic[email]>=1.9.1,<2.0.0
+Requires-Dist: pydantic[email]>=2.1.1,<3.0.0
 Requires-Dist: black==22.10.0 ; extra == "dev"
 Requires-Dist: pre-commit==2.20.0 ; extra == "dev"
 Project-URL: Documentation, https://www.data.inclusion.beta.gouv.fr/schemas-de-donnees-de-loffre/schema-des-structures-et-services-dinsertion
 Project-URL: Home, https://www.data.inclusion.beta.gouv.fr
 Project-URL: Source, https://github.com/betagouv/data-inclusion-schema
 Provides-Extra: dev
```

