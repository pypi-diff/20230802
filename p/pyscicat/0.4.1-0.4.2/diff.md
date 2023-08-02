# Comparing `tmp/pyscicat-0.4.1.tar.gz` & `tmp/pyscicat-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscicat-0.4.1.tar", last modified: Tue Jun 27 16:12:28 2023, max compression
+gzip compressed data, was "pyscicat-0.4.2.tar", last modified: Wed Aug  2 18:31:56 2023, max compression
```

## Comparing `pyscicat-0.4.1.tar` & `pyscicat-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524962 pyscicat-0.4.1/
--rw-r--r--   0 dylan      (501) staff       (20)      171 2023-06-23 22:30:03.000000 pyscicat-0.4.1/AUTHORS.rst
--rw-r--r--   0 dylan      (501) staff       (20)     2463 2023-06-23 22:30:03.000000 pyscicat-0.4.1/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      361 2023-06-23 22:30:03.000000 pyscicat-0.4.1/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)      888 2023-06-27 16:12:28.525047 pyscicat-0.4.1/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      337 2023-06-23 22:34:01.000000 pyscicat-0.4.1/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.522247 pyscicat-0.4.1/docs/
--rw-r--r--   0 dylan      (501) staff       (20)      673 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/Makefile
--rw-r--r--   0 dylan      (501) staff       (20)      797 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/make.bat
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.522397 pyscicat-0.4.1/docs/source/
--rw-r--r--   0 dylan      (501) staff       (20)     6442 2023-06-23 22:34:01.000000 pyscicat-0.4.1/docs/source/conf.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.520395 pyscicat-0.4.1/docs/source/reference/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.522813 pyscicat-0.4.1/docs/source/reference/generated/
--rw-r--r--   0 dylan      (501) staff       (20)      375 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/source/reference/generated/pyscicat.client.ScicatClient.rst
--rw-r--r--   0 dylan      (501) staff       (20)      287 2023-06-23 22:30:03.000000 pyscicat-0.4.1/docs/source/reference/generated/pyscicat.model.rst
--rw-r--r--   0 dylan      (501) staff       (20)      258 2023-06-23 22:30:03.000000 pyscicat-0.4.1/pyproject.toml
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.525591 pyscicat-0.4.1/pyscicat/
--rw-r--r--   0 dylan      (501) staff       (20)       93 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)      497 2023-06-27 16:12:28.525621 pyscicat-0.4.1/pyscicat/_version.py
--rw-r--r--   0 dylan      (501) staff       (20)    26331 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/client.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524740 pyscicat-0.4.1/pyscicat/hdf5/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/hdf5/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     3472 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/hdf5/h5tools.py
--rw-r--r--   0 dylan      (501) staff       (20)     4690 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/hdf5/scientific_metadata.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524853 pyscicat-0.4.1/pyscicat/ingest/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2023-06-23 22:30:03.000000 pyscicat-0.4.1/pyscicat/ingest/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     6108 2023-06-23 22:34:01.000000 pyscicat-0.4.1/pyscicat/model.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-27 16:12:28.524410 pyscicat-0.4.1/pyscicat.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)      888 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      607 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)      245 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)        9 2023-06-27 16:12:28.000000 pyscicat-0.4.1/pyscicat.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)     1123 2023-06-27 16:12:28.525450 pyscicat-0.4.1/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)      134 2023-06-23 22:34:01.000000 pyscicat-0.4.1/setup.py
--rw-r--r--   0 dylan      (501) staff       (20)    68751 2023-06-23 22:34:01.000000 pyscicat-0.4.1/versioneer.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.632481 pyscicat-0.4.2/
+-rw-r--r--   0 dylan      (501) staff       (20)      171 2023-06-23 22:30:03.000000 pyscicat-0.4.2/AUTHORS.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     2463 2023-06-23 22:30:03.000000 pyscicat-0.4.2/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)      361 2023-06-23 22:30:03.000000 pyscicat-0.4.2/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)      868 2023-08-02 18:31:56.632565 pyscicat-0.4.2/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      337 2023-06-23 22:34:01.000000 pyscicat-0.4.2/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.629650 pyscicat-0.4.2/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)      673 2023-06-23 22:30:03.000000 pyscicat-0.4.2/docs/Makefile
+-rw-r--r--   0 dylan      (501) staff       (20)      797 2023-06-23 22:30:03.000000 pyscicat-0.4.2/docs/make.bat
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.629777 pyscicat-0.4.2/docs/source/
+-rw-r--r--   0 dylan      (501) staff       (20)     6442 2023-06-23 22:34:01.000000 pyscicat-0.4.2/docs/source/conf.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.628301 pyscicat-0.4.2/docs/source/reference/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.630031 pyscicat-0.4.2/docs/source/reference/generated/
+-rw-r--r--   0 dylan      (501) staff       (20)      375 2023-06-23 22:30:03.000000 pyscicat-0.4.2/docs/source/reference/generated/pyscicat.client.ScicatClient.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      287 2023-06-23 22:30:03.000000 pyscicat-0.4.2/docs/source/reference/generated/pyscicat.model.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      258 2023-06-23 22:30:03.000000 pyscicat-0.4.2/pyproject.toml
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.633135 pyscicat-0.4.2/pyscicat/
+-rw-r--r--   0 dylan      (501) staff       (20)       93 2023-06-23 22:34:01.000000 pyscicat-0.4.2/pyscicat/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)      497 2023-08-02 18:31:56.633165 pyscicat-0.4.2/pyscicat/_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)    26331 2023-06-23 22:34:01.000000 pyscicat-0.4.2/pyscicat/client.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.632132 pyscicat-0.4.2/pyscicat/hdf5/
+-rw-------   0 dylan      (501) staff       (20)        0 2023-06-23 22:34:01.000000 pyscicat-0.4.2/pyscicat/hdf5/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3472 2023-06-23 22:34:01.000000 pyscicat-0.4.2/pyscicat/hdf5/h5tools.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4690 2023-06-23 22:34:01.000000 pyscicat-0.4.2/pyscicat/hdf5/scientific_metadata.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.632374 pyscicat-0.4.2/pyscicat/ingest/
+-rw-------   0 dylan      (501) staff       (20)        0 2023-06-23 22:30:03.000000 pyscicat-0.4.2/pyscicat/ingest/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     6605 2023-08-02 18:25:22.000000 pyscicat-0.4.2/pyscicat/model.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-08-02 18:31:56.631831 pyscicat-0.4.2/pyscicat.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)      868 2023-08-02 18:31:56.000000 pyscicat-0.4.2/pyscicat.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      607 2023-08-02 18:31:56.000000 pyscicat-0.4.2/pyscicat.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-08-02 18:31:56.000000 pyscicat-0.4.2/pyscicat.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      245 2023-08-02 18:31:56.000000 pyscicat-0.4.2/pyscicat.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        9 2023-08-02 18:31:56.000000 pyscicat-0.4.2/pyscicat.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     1123 2023-08-02 18:31:56.632977 pyscicat-0.4.2/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)      134 2023-06-23 22:34:01.000000 pyscicat-0.4.2/setup.py
+-rw-r--r--   0 dylan      (501) staff       (20)    68751 2023-06-23 22:34:01.000000 pyscicat-0.4.2/versioneer.py
```

### Comparing `pyscicat-0.4.1/LICENSE` & `pyscicat-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/PKG-INFO` & `pyscicat-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: pyscicat
-Version: 0.4.1
+Version: 0.4.2
 Summary: a python API to communicate with the Scicat API
 Home-page: https://github.com/scicatproject/pyscicat
 Author: Dylan McReynolds
 Author-email: dmcreynolds@lbl.gov
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: hdf5
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # Pyscicat
 Pyscicat is a python client library for interacting with the [SciCat backend](https://scicatproject.github.io/). It sends messages to the SciCat backend over HTTP. It currently does not contain any command line interface.
 
 Documentation for Pyscicat can be found is [available here](https://scicatproject.github.io/pyscicat/)
-
-
```

### Comparing `pyscicat-0.4.1/docs/Makefile` & `pyscicat-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/docs/make.bat` & `pyscicat-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/docs/source/conf.py` & `pyscicat-0.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/pyscicat/client.py` & `pyscicat-0.4.2/pyscicat/client.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/pyscicat/hdf5/h5tools.py` & `pyscicat-0.4.2/pyscicat/hdf5/h5tools.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/pyscicat/hdf5/scientific_metadata.py` & `pyscicat-0.4.2/pyscicat/hdf5/scientific_metadata.py`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/pyscicat/model.py` & `pyscicat-0.4.2/pyscicat/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     raw = "raw"
     derived = "derived"
 
 
 class MongoQueryable(BaseModel):
     """Many objects in SciCat are mongo queryable"""
 
-    createdBy: Optional[str]
-    updatedBy: Optional[str]
-    updatedAt: Optional[str]
-    createdAt: Optional[str]
+    createdBy: Optional[str] = None
+    updatedBy: Optional[str] = None
+    updatedAt: Optional[str] = None
+    createdAt: Optional[str] = None
 
 
 class Ownable(MongoQueryable):
     """Many objects in SciCat are ownable"""
 
     ownerGroup: str
-    accessGroups: Optional[List[str]]
-    instrumentGroup: Optional[str]
+    accessGroups: Optional[List[str]] = None
+    instrumentGroup: Optional[str] = None
 
 
 class User(BaseModel):
     """Base user."""
 
     # TODO: find out which of these are not optional and update
     realm: str
@@ -43,206 +43,206 @@
 
 class Proposal(Ownable):
     """
     Defines the purpose of an experiment and links an experiment to principal investigator and main proposer
     """
 
     proposalId: str
-    pi_email: Optional[str]
-    pi_firstname: Optional[str]
-    pi_lastname: Optional[str]
+    pi_email: Optional[str] = None
+    pi_firstname: Optional[str] = None
+    pi_lastname: Optional[str] = None
     email: str
-    firstname: Optional[str]
-    lastname: Optional[str]
-    title: Optional[str]  # required in next backend version
-    abstract: Optional[str]
-    startTime: Optional[str]
-    endTime: Optional[str]
+    firstname: Optional[str] = None
+    lastname: Optional[str] = None
+    title: Optional[str] = None  # required in next backend version
+    abstract: Optional[str] = None
+    startTime: Optional[str] = None
+    endTime: Optional[str] = None
     MeasurementPeriodList: Optional[
         List[dict]
-    ]  # may need updating with the measurement period model
+    ] = None  # may need updating with the measurement period model
 
 
 class Sample(Ownable):
     """
     Models describing the characteristics of the samples to be investigated.
     Raw datasets should be linked to such sample definitions.
     """
 
-    sampleId: Optional[str]
-    owner: Optional[str]
-    description: Optional[str]
-    sampleCharacteristics: Optional[dict]
+    sampleId: Optional[str] = None
+    owner: Optional[str] = None
+    description: Optional[str] = None
+    sampleCharacteristics: Optional[dict] = None
     isPublished: bool = False
 
 
 class Job(MongoQueryable):
     """
     This collection keeps information about jobs to be excuted in external systems.
     In particular it keeps information about the jobs submitted for archiving or
     retrieving datasets stored inside an archive system. It can also be used to keep
     track of analysis jobs e.g. for automated analysis workflows
     """
 
-    id: Optional[str]
+    id: Optional[str] = None
     emailJobInitiator: str
     type: str
-    creationTime: Optional[str]  # not sure yet which ones are optional or not.
-    executionTime: Optional[str]
-    jobParams: Optional[dict]
-    jobStatusMessage: Optional[str]
-    datasetList: Optional[dict]  # documentation says dict, but should maybe be list?
-    jobResultObject: Optional[dict]  # ibid.
+    creationTime: Optional[str] = None  # not sure yet which ones are optional or not.
+    executionTime: Optional[str] = None
+    jobParams: Optional[dict] = None
+    jobStatusMessage: Optional[str] = None
+    datasetList: Optional[dict] = None  # documentation says dict, but should maybe be list?
+    jobResultObject: Optional[dict] = None  # ibid.
 
 
 class Instrument(MongoQueryable):
     """
     Instrument class, most of this is flexibly definable in customMetadata
     """
 
-    pid: Optional[str]
+    pid: Optional[str] = None
     name: str
-    customMetadata: Optional[dict]
+    customMetadata: Optional[dict] = None
 
 
 class Dataset(Ownable):
     """
     A dataset in SciCat, base class for derived and raw datasets
     """
 
-    pid: Optional[str]
-    classification: Optional[str]
+    pid: Optional[str] = None
+    classification: Optional[str] = None
     contactEmail: str
     creationTime: str  # datetime
-    datasetName: Optional[str]
-    description: Optional[str]
-    history: Optional[List[dict]]  # list of foreigh key ids to the Messages table
-    instrumentId: Optional[str]
+    datasetName: Optional[str] = None
+    description: Optional[str] = None
+    history: Optional[List[dict]] = None  # list of foreigh key ids to the Messages table
+    instrumentId: Optional[str] = None
     isPublished: Optional[bool] = False
-    keywords: Optional[List[str]]
-    license: Optional[str]
-    numberOfFiles: Optional[int]
-    numberOfFilesArchived: Optional[int]
-    orcidOfOwner: Optional[str]
-    packedSize: Optional[int]
+    keywords: Optional[List[str]] = None
+    license: Optional[str] = None
+    numberOfFiles: Optional[int] = None
+    numberOfFilesArchived: Optional[int] = None
+    orcidOfOwner: Optional[str] = None
+    packedSize: Optional[int] = None
     owner: str
-    ownerEmail: Optional[str]
-    sharedWith: Optional[List[str]]
-    size: Optional[int]
+    ownerEmail: Optional[str] = None
+    sharedWith: Optional[List[str]] = None
+    size: Optional[int] = None
     sourceFolder: str
-    sourceFolderHost: Optional[str]
-    techniques: Optional[List[dict]]  # with {'pid':pid, 'name': name} as entries
+    sourceFolderHost: Optional[str] = None
+    techniques: Optional[List[dict]] = None  # with {'pid':pid, 'name': name} as entries
     type: DatasetType
-    validationStatus: Optional[str]
-    version: Optional[str]
-    scientificMetadata: Optional[Dict]
+    validationStatus: Optional[str] = None
+    version: Optional[str] = None
+    scientificMetadata: Optional[Dict] = None
 
 
 class RawDataset(Dataset):
     """
     Raw datasets from which derived datasets are... derived.
     """
 
-    principalInvestigator: Optional[str]
-    creationLocation: Optional[str]
+    principalInvestigator: Optional[str] = None
+    creationLocation: Optional[str] = None
     type: DatasetType = DatasetType.raw
-    dataFormat: Optional[str]
-    endTime: Optional[str]  # datetime
-    sampleId: Optional[str]
-    proposalId: Optional[str]
+    dataFormat: Optional[str] = None
+    endTime: Optional[str] = None  # datetime
+    sampleId: Optional[str] = None
+    proposalId: Optional[str] = None
 
 
 class DerivedDataset(Dataset):
     """
     Derived datasets which have been generated based on one or more raw datasets
     """
 
     investigator: str
     inputDatasets: List[str]
     usedSoftware: List[str]
-    jobParameters: Optional[dict]
-    jobLogData: Optional[str]
+    jobParameters: Optional[dict] = None
+    jobLogData: Optional[str] = None
     type: DatasetType = DatasetType.derived
 
 
 class DataFile(MongoQueryable):
     """
     A reference to a file in SciCat. Path is relative
     to the Dataset's sourceFolder parameter
 
     """
 
     path: str
     size: int
-    time: Optional[str]
-    chk: Optional[str]
+    time: Optional[str] = None
+    chk: Optional[str] = None
     uid: Optional[str] = None
     gid: Optional[str] = None
     perm: Optional[str] = None
 
 
 class Datablock(Ownable):
     """
     A Datablock maps between a Dataset and contains DataFiles
     """
 
-    id: Optional[str]
+    id: Optional[str] = None
     # archiveId: str = None  listed in catamel model, but comes back invalid?
     size: int
-    packedSize: Optional[int]
-    chkAlg: Optional[int]
+    packedSize: Optional[int] = None
+    chkAlg: Optional[int] = None
     version: str = None
-    instrumentGroup: Optional[str]
+    instrumentGroup: Optional[str] = None
     dataFileList: List[DataFile]
     datasetId: str
 
 
 class OrigDatablock(Ownable):
     """
     An Original Datablock maps between a Dataset and contains DataFiles
     """
 
-    id: Optional[str]
+    id: Optional[str] = None
     # archiveId: str = None  listed in catamel model, but comes back invalid?
     size: int
-    instrumentGroup: Optional[str]
+    instrumentGroup: Optional[str] = None
     dataFileList: List[DataFile]
     datasetId: str
 
 
 class Attachment(Ownable):
     """
     Attachments can be any base64 encoded string...thumbnails are attachments
     """
 
-    id: Optional[str]
+    id: Optional[str] = None
     thumbnail: str
-    caption: Optional[str]
+    caption: Optional[str] = None
     datasetId: str
 
 
 class PublishedData:
     """
     Published Data with registered DOI
     """
 
     doi: str
     affiliation: str
     creator: List[str]
     publisher: str
     publicationYear: int
     title: str
-    url: Optional[str]
+    url: Optional[str] = None
     abstract: str
     dataDescription: str
     resourceType: str
-    numberOfFiles: Optional[int]
-    sizeOfArchive: Optional[int]
+    numberOfFiles: Optional[int] = None
+    sizeOfArchive: Optional[int] = None
     pidArray: List[str]
     authors: List[str]
     registeredTime: str
     status: str
-    thumbnail: Optional[str]
+    thumbnail: Optional[str] = None
     createdBy: str
     updatedBy: str
     createdAt: str
     updatedAt: str
```

### Comparing `pyscicat-0.4.1/pyscicat.egg-info/PKG-INFO` & `pyscicat-0.4.2/pyscicat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: pyscicat
-Version: 0.4.1
+Version: 0.4.2
 Summary: a python API to communicate with the Scicat API
 Home-page: https://github.com/scicatproject/pyscicat
 Author: Dylan McReynolds
 Author-email: dmcreynolds@lbl.gov
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: hdf5
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # Pyscicat
 Pyscicat is a python client library for interacting with the [SciCat backend](https://scicatproject.github.io/). It sends messages to the SciCat backend over HTTP. It currently does not contain any command line interface.
 
 Documentation for Pyscicat can be found is [available here](https://scicatproject.github.io/pyscicat/)
-
-
```

### Comparing `pyscicat-0.4.1/pyscicat.egg-info/SOURCES.txt` & `pyscicat-0.4.2/pyscicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/setup.cfg` & `pyscicat-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyscicat-0.4.1/versioneer.py` & `pyscicat-0.4.2/versioneer.py`

 * *Files identical despite different names*

