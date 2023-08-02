# Comparing `tmp/sdmxthon-2.1.tar.gz` & `tmp/sdmxthon-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmxthon-2.1.tar", last modified: Tue Mar 14 10:18:26 2023, max compression
+gzip compressed data, was "sdmxthon-2.2.tar", last modified: Wed Aug  2 08:45:50 2023, max compression
```

## Comparing `sdmxthon-2.1.tar` & `sdmxthon-2.2.tar`

### file list

```diff
@@ -1,106 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.527347 sdmxthon-2.1/
--rw-rw-rw-   0        0        0      143 2021-05-28 09:14:58.000000 sdmxthon-2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2477 2023-03-14 10:18:26.528747 sdmxthon-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2021-11-10 17:15:12.000000 sdmxthon-2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.447620 sdmxthon-2.1/SDMXthon.egg-info/
--rw-rw-rw-   0        0        0     2477 2023-03-14 10:18:25.000000 sdmxthon-2.1/SDMXthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3636 2023-03-14 10:18:26.000000 sdmxthon-2.1/SDMXthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 10:18:25.000000 sdmxthon-2.1/SDMXthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-14 10:18:26.000000 sdmxthon-2.1/SDMXthon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-14 10:18:26.000000 sdmxthon-2.1/SDMXthon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.449132 sdmxthon-2.1/sdmxthon/
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.453299 sdmxthon-2.1/sdmxthon/WebServices/
--rw-rw-rw-   0        0        0        0 2021-03-22 11:19:40.000000 sdmxthon-2.1/sdmxthon/WebServices/__init__.py
--rw-rw-rw-   0        0        0     3352 2023-03-14 10:16:48.000000 sdmxthon-2.1/sdmxthon/WebServices/app.py
--rw-rw-rw-   0        0        0    10675 2023-03-03 11:30:01.000000 sdmxthon-2.1/sdmxthon/WebServices/sdmx_requests.py
--rw-rw-rw-   0        0        0     6821 2023-03-14 10:17:34.000000 sdmxthon-2.1/sdmxthon/WebServices/test.py
--rw-rw-rw-   0        0        0      155 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.453299 sdmxthon-2.1/sdmxthon/api/
--rw-rw-rw-   0        0        0     4865 2022-12-22 16:42:27.000000 sdmxthon-2.1/sdmxthon/api/api.py
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.465015 sdmxthon-2.1/sdmxthon/model/
--rw-rw-rw-   0        0        0        0 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/model/__init__.py
--rw-rw-rw-   0        0        0    21407 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/base.py
--rw-rw-rw-   0        0        0    15792 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/component.py
--rw-rw-rw-   0        0        0    16059 2022-12-22 16:42:27.000000 sdmxthon-2.1/sdmxthon/model/dataset.py
--rw-rw-rw-   0        0        0    28924 2023-03-14 10:17:06.000000 sdmxthon-2.1/sdmxthon/model/definitions.py
--rw-rw-rw-   0        0        0     6854 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/descriptors.py
--rw-rw-rw-   0        0        0     2118 2021-11-10 17:15:12.000000 sdmxthon-2.1/sdmxthon/model/extras.py
--rw-rw-rw-   0        0        0    15559 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/header.py
--rw-rw-rw-   0        0        0    22740 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/itemScheme.py
--rw-rw-rw-   0        0        0     7469 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/message.py
--rw-rw-rw-   0        0        0     4230 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/representation.py
--rw-rw-rw-   0        0        0     6478 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/model/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.469374 sdmxthon-2.1/sdmxthon/parsers/
--rw-rw-rw-   0        0        0       36 2021-03-22 11:19:58.000000 sdmxthon-2.1/sdmxthon/parsers/__init__.py
--rw-rw-rw-   0        0        0     5474 2022-12-22 16:42:27.000000 sdmxthon-2.1/sdmxthon/parsers/data_read.py
--rw-rw-rw-   0        0        0    25740 2021-12-01 17:37:22.000000 sdmxthon-2.1/sdmxthon/parsers/data_validations.py
--rw-rw-rw-   0        0        0    25564 2023-03-14 09:54:53.000000 sdmxthon-2.1/sdmxthon/parsers/metadata_read.py
--rw-rw-rw-   0        0        0     5455 2022-12-22 16:42:27.000000 sdmxthon-2.1/sdmxthon/parsers/read.py
--rw-rw-rw-   0        0        0    24588 2021-12-01 12:46:51.000000 sdmxthon-2.1/sdmxthon/parsers/write.py
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.521112 sdmxthon-2.1/sdmxthon/schemas/
--rw-rw-rw-   0        0        0   113624 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXCommon.xsd
--rw-rw-rw-   0        0        0   278665 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXCommonReferences.xsd
--rw-rw-rw-   0        0        0      805 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXDataGeneric.xsd
--rw-rw-rw-   0        0        0    24835 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXDataGenericBase.xsd
--rw-rw-rw-   0        0        0     9579 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd
--rw-rw-rw-   0        0        0     1156 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXDataStructureSpecific.xsd
--rw-rw-rw-   0        0        0    41262 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd
--rw-rw-rw-   0        0        0     8408 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd
--rw-rw-rw-   0        0        0    81157 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXMessage.xsd
--rw-rw-rw-   0        0        0     3624 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXMessageFooter.xsd
--rw-rw-rw-   0        0        0    16072 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXMetadataGeneric.xsd
--rw-rw-rw-   0        0        0    30613 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd
--rw-rw-rw-   0        0        0     2172 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQuery.xsd
--rw-rw-rw-   0        0        0    46248 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryBase.xsd
--rw-rw-rw-   0        0        0     6558 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryCategorisation.xsd
--rw-rw-rw-   0        0        0     5726 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryCategory.xsd
--rw-rw-rw-   0        0        0     5284 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryCodelist.xsd
--rw-rw-rw-   0        0        0     6473 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryConcept.xsd
--rw-rw-rw-   0        0        0    11540 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryConstraint.xsd
--rw-rw-rw-   0        0        0    34427 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryData.xsd
--rw-rw-rw-   0        0        0    19416 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryDataStructure.xsd
--rw-rw-rw-   0        0        0     4184 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryDataflow.xsd
--rw-rw-rw-   0        0        0     5308 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd
--rw-rw-rw-   0        0        0    25651 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryMetadata.xsd
--rw-rw-rw-   0        0        0    14717 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd
--rw-rw-rw-   0        0        0     4352 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryMetadataflow.xsd
--rw-rw-rw-   0        0        0     7463 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryOrganisation.xsd
--rw-rw-rw-   0        0        0     9459 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryProcess.xsd
--rw-rw-rw-   0        0        0     5669 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd
--rw-rw-rw-   0        0        0     7677 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd
--rw-rw-rw-   0        0        0     5305 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQuerySchema.xsd
--rw-rw-rw-   0        0        0    10154 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryStructureSet.xsd
--rw-rw-rw-   0        0        0     3709 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXQueryStructures.xsd
--rw-rw-rw-   0        0        0     1009 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXRegistry.xsd
--rw-rw-rw-   0        0        0    14238 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXRegistryBase.xsd
--rw-rw-rw-   0        0        0    19745 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXRegistryRegistration.xsd
--rw-rw-rw-   0        0        0    10271 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXRegistryStructure.xsd
--rw-rw-rw-   0        0        0    63155 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXRegistrySubscription.xsd
--rw-rw-rw-   0        0        0    41096 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructure.xsd
--rw-rw-rw-   0        0        0    39172 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureBase.xsd
--rw-rw-rw-   0        0        0     2069 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureCategorisation.xsd
--rw-rw-rw-   0        0        0     4767 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureCategory.xsd
--rw-rw-rw-   0        0        0     4930 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureCodelist.xsd
--rw-rw-rw-   0        0        0     7866 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureConcept.xsd
--rw-rw-rw-   0        0        0    28760 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureConstraint.xsd
--rw-rw-rw-   0        0        0    52702 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureDataStructure.xsd
--rw-rw-rw-   0        0        0     2167 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureDataflow.xsd
--rw-rw-rw-   0        0        0    23519 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd
--rw-rw-rw-   0        0        0    37058 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd
--rw-rw-rw-   0        0        0     2265 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureMetadataflow.xsd
--rw-rw-rw-   0        0        0    19113 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureOrganisation.xsd
--rw-rw-rw-   0        0        0    14460 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureProcess.xsd
--rw-rw-rw-   0        0        0     2597 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd
--rw-rw-rw-   0        0        0     6218 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd
--rw-rw-rw-   0        0        0    34361 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/SDMXStructureStructureSet.xsd
--rw-rw-rw-   0        0        0     3363 2021-05-28 09:14:58.000000 sdmxthon-2.1/sdmxthon/schemas/xml.xsd
-drwxrwxrwx   0        0        0        0 2023-03-14 10:18:26.527347 sdmxthon-2.1/sdmxthon/utils/
--rw-rw-rw-   0        0        0        0 2021-03-22 11:19:40.000000 sdmxthon-2.1/sdmxthon/utils/__init__.py
--rw-rw-rw-   0        0        0      290 2021-11-10 17:15:12.000000 sdmxthon-2.1/sdmxthon/utils/enums.py
--rw-rw-rw-   0        0        0     2753 2022-12-22 16:42:27.000000 sdmxthon-2.1/sdmxthon/utils/handlers.py
--rw-rw-rw-   0        0        0     6291 2022-12-22 16:42:27.000000 sdmxthon-2.1/sdmxthon/utils/mappings.py
--rw-rw-rw-   0        0        0     3716 2021-12-01 16:51:53.000000 sdmxthon-2.1/sdmxthon/utils/parsing_words.py
--rw-rw-rw-   0        0        0      125 2023-03-14 10:10:33.000000 sdmxthon-2.1/sdmxthon/utils/xml_allowed_errors.py
--rw-rw-rw-   0        0        0     3626 2023-03-14 10:03:32.000000 sdmxthon-2.1/sdmxthon/utils/xml_base.py
--rw-rw-rw-   0        0        0       42 2023-03-14 10:18:26.528747 sdmxthon-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1598 2023-03-14 10:05:49.000000 sdmxthon-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.504953 sdmxthon-2.2/
+-rw-rw-rw-   0        0        0      143 2021-05-28 09:14:58.000000 sdmxthon-2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2477 2023-08-02 08:45:50.504953 sdmxthon-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2021-11-10 17:15:12.000000 sdmxthon-2.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.393909 sdmxthon-2.2/sdmxthon/
+-rw-rw-rw-   0        0        0      155 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.399913 sdmxthon-2.2/sdmxthon/api/
+-rw-rw-rw-   0        0        0     4865 2022-12-22 16:42:27.000000 sdmxthon-2.2/sdmxthon/api/api.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.411908 sdmxthon-2.2/sdmxthon/model/
+-rw-rw-rw-   0        0        0        0 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/model/__init__.py
+-rw-rw-rw-   0        0        0    21944 2023-08-02 08:45:03.000000 sdmxthon-2.2/sdmxthon/model/base.py
+-rw-rw-rw-   0        0        0    15792 2021-12-01 12:46:51.000000 sdmxthon-2.2/sdmxthon/model/component.py
+-rw-rw-rw-   0        0        0    16528 2023-08-02 08:45:03.000000 sdmxthon-2.2/sdmxthon/model/dataset.py
+-rw-rw-rw-   0        0        0    28924 2023-03-14 10:20:20.000000 sdmxthon-2.2/sdmxthon/model/definitions.py
+-rw-rw-rw-   0        0        0     6854 2021-12-01 12:46:51.000000 sdmxthon-2.2/sdmxthon/model/descriptors.py
+-rw-rw-rw-   0        0        0     2118 2021-11-10 17:15:12.000000 sdmxthon-2.2/sdmxthon/model/extras.py
+-rw-rw-rw-   0        0        0    15559 2021-12-01 12:46:51.000000 sdmxthon-2.2/sdmxthon/model/header.py
+-rw-rw-rw-   0        0        0    22740 2021-12-01 12:46:51.000000 sdmxthon-2.2/sdmxthon/model/itemScheme.py
+-rw-rw-rw-   0        0        0     7469 2023-06-14 09:27:10.000000 sdmxthon-2.2/sdmxthon/model/message.py
+-rw-rw-rw-   0        0        0     4230 2021-12-01 12:46:51.000000 sdmxthon-2.2/sdmxthon/model/representation.py
+-rw-rw-rw-   0        0        0     6478 2021-12-01 12:46:51.000000 sdmxthon-2.2/sdmxthon/model/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.418907 sdmxthon-2.2/sdmxthon/parsers/
+-rw-rw-rw-   0        0        0       36 2021-03-22 11:19:58.000000 sdmxthon-2.2/sdmxthon/parsers/__init__.py
+-rw-rw-rw-   0        0        0     5474 2022-12-22 16:42:27.000000 sdmxthon-2.2/sdmxthon/parsers/data_read.py
+-rw-rw-rw-   0        0        0    25740 2021-12-01 17:37:22.000000 sdmxthon-2.2/sdmxthon/parsers/data_validations.py
+-rw-rw-rw-   0        0        0    25564 2023-03-14 10:20:20.000000 sdmxthon-2.2/sdmxthon/parsers/metadata_read.py
+-rw-rw-rw-   0        0        0     5455 2022-12-22 16:42:27.000000 sdmxthon-2.2/sdmxthon/parsers/read.py
+-rw-rw-rw-   0        0        0    24519 2023-08-02 08:45:03.000000 sdmxthon-2.2/sdmxthon/parsers/write.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.496953 sdmxthon-2.2/sdmxthon/schemas/
+-rw-rw-rw-   0        0        0   113624 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXCommon.xsd
+-rw-rw-rw-   0        0        0   278665 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXCommonReferences.xsd
+-rw-rw-rw-   0        0        0      805 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXDataGeneric.xsd
+-rw-rw-rw-   0        0        0    24835 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXDataGenericBase.xsd
+-rw-rw-rw-   0        0        0     9579 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd
+-rw-rw-rw-   0        0        0     1156 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXDataStructureSpecific.xsd
+-rw-rw-rw-   0        0        0    41262 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd
+-rw-rw-rw-   0        0        0     8408 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd
+-rw-rw-rw-   0        0        0    81157 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXMessage.xsd
+-rw-rw-rw-   0        0        0     3624 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXMessageFooter.xsd
+-rw-rw-rw-   0        0        0    16072 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXMetadataGeneric.xsd
+-rw-rw-rw-   0        0        0    30613 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd
+-rw-rw-rw-   0        0        0     2172 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQuery.xsd
+-rw-rw-rw-   0        0        0    46248 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryBase.xsd
+-rw-rw-rw-   0        0        0     6558 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryCategorisation.xsd
+-rw-rw-rw-   0        0        0     5726 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryCategory.xsd
+-rw-rw-rw-   0        0        0     5284 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryCodelist.xsd
+-rw-rw-rw-   0        0        0     6473 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryConcept.xsd
+-rw-rw-rw-   0        0        0    11540 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryConstraint.xsd
+-rw-rw-rw-   0        0        0    34427 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryData.xsd
+-rw-rw-rw-   0        0        0    19416 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryDataStructure.xsd
+-rw-rw-rw-   0        0        0     4184 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryDataflow.xsd
+-rw-rw-rw-   0        0        0     5308 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd
+-rw-rw-rw-   0        0        0    25651 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryMetadata.xsd
+-rw-rw-rw-   0        0        0    14717 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd
+-rw-rw-rw-   0        0        0     4352 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryMetadataflow.xsd
+-rw-rw-rw-   0        0        0     7463 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryOrganisation.xsd
+-rw-rw-rw-   0        0        0     9459 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryProcess.xsd
+-rw-rw-rw-   0        0        0     5669 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd
+-rw-rw-rw-   0        0        0     7677 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd
+-rw-rw-rw-   0        0        0     5305 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQuerySchema.xsd
+-rw-rw-rw-   0        0        0    10154 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryStructureSet.xsd
+-rw-rw-rw-   0        0        0     3709 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXQueryStructures.xsd
+-rw-rw-rw-   0        0        0     1009 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXRegistry.xsd
+-rw-rw-rw-   0        0        0    14238 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXRegistryBase.xsd
+-rw-rw-rw-   0        0        0    19745 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXRegistryRegistration.xsd
+-rw-rw-rw-   0        0        0    10271 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXRegistryStructure.xsd
+-rw-rw-rw-   0        0        0    63155 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXRegistrySubscription.xsd
+-rw-rw-rw-   0        0        0    41096 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructure.xsd
+-rw-rw-rw-   0        0        0    39172 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureBase.xsd
+-rw-rw-rw-   0        0        0     2069 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureCategorisation.xsd
+-rw-rw-rw-   0        0        0     4767 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureCategory.xsd
+-rw-rw-rw-   0        0        0     4930 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureCodelist.xsd
+-rw-rw-rw-   0        0        0     7866 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureConcept.xsd
+-rw-rw-rw-   0        0        0    28760 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureConstraint.xsd
+-rw-rw-rw-   0        0        0    52702 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureDataStructure.xsd
+-rw-rw-rw-   0        0        0     2167 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureDataflow.xsd
+-rw-rw-rw-   0        0        0    23519 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd
+-rw-rw-rw-   0        0        0    37058 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd
+-rw-rw-rw-   0        0        0     2265 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureMetadataflow.xsd
+-rw-rw-rw-   0        0        0    19113 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureOrganisation.xsd
+-rw-rw-rw-   0        0        0    14460 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureProcess.xsd
+-rw-rw-rw-   0        0        0     2597 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd
+-rw-rw-rw-   0        0        0     6218 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd
+-rw-rw-rw-   0        0        0    34361 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/SDMXStructureStructureSet.xsd
+-rw-rw-rw-   0        0        0     3363 2021-05-28 09:14:58.000000 sdmxthon-2.2/sdmxthon/schemas/xml.xsd
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.503953 sdmxthon-2.2/sdmxthon/utils/
+-rw-rw-rw-   0        0        0        0 2021-03-22 11:19:40.000000 sdmxthon-2.2/sdmxthon/utils/__init__.py
+-rw-rw-rw-   0        0        0      290 2021-11-10 17:15:12.000000 sdmxthon-2.2/sdmxthon/utils/enums.py
+-rw-rw-rw-   0        0        0     2753 2022-12-22 16:42:27.000000 sdmxthon-2.2/sdmxthon/utils/handlers.py
+-rw-rw-rw-   0        0        0     6291 2022-12-22 16:42:27.000000 sdmxthon-2.2/sdmxthon/utils/mappings.py
+-rw-rw-rw-   0        0        0     3716 2021-12-01 16:51:53.000000 sdmxthon-2.2/sdmxthon/utils/parsing_words.py
+-rw-rw-rw-   0        0        0      125 2023-03-14 10:20:20.000000 sdmxthon-2.2/sdmxthon/utils/xml_allowed_errors.py
+-rw-rw-rw-   0        0        0     3626 2023-03-14 10:20:20.000000 sdmxthon-2.2/sdmxthon/utils/xml_base.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:45:50.398907 sdmxthon-2.2/sdmxthon.egg-info/
+-rw-rw-rw-   0        0        0     2477 2023-08-02 08:45:49.000000 sdmxthon-2.2/sdmxthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3347 2023-08-02 08:45:50.000000 sdmxthon-2.2/sdmxthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:45:49.000000 sdmxthon-2.2/sdmxthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-08-02 08:45:50.000000 sdmxthon-2.2/sdmxthon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 08:45:50.000000 sdmxthon-2.2/sdmxthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:45:50.505954 sdmxthon-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1598 2023-08-02 08:45:03.000000 sdmxthon-2.2/setup.py
```

### Comparing `sdmxthon-2.1/PKG-INFO` & `sdmxthon-2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmxthon
-Version: 2.1
+Version: 2.2
 Summary: Library with SDMX to Pandas, Pandas to SDMX, SDMX validation and SDMX metadata validation
 Author: MeaningfulData
 Author-email: javier.hernandez@meaningfuldata.eu
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Meaningful-Data/sdmxthon/issues
 Project-URL: Documentation, https://docs.sdmxthon.meaningfuldata.eu
 Project-URL: Source Code, https://github.com/Meaningful-Data/sdmxthon
```

### Comparing `sdmxthon-2.1/README.rst` & `sdmxthon-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/SDMXthon.egg-info/PKG-INFO` & `sdmxthon-2.2/sdmxthon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmxthon
-Version: 2.1
+Version: 2.2
 Summary: Library with SDMX to Pandas, Pandas to SDMX, SDMX validation and SDMX metadata validation
 Author: MeaningfulData
 Author-email: javier.hernandez@meaningfuldata.eu
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Meaningful-Data/sdmxthon/issues
 Project-URL: Documentation, https://docs.sdmxthon.meaningfuldata.eu
 Project-URL: Source Code, https://github.com/Meaningful-Data/sdmxthon
```

### Comparing `sdmxthon-2.1/SDMXthon.egg-info/SOURCES.txt` & `sdmxthon-2.2/sdmxthon.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-.
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-SDMXthon.egg-info/PKG-INFO
-SDMXthon.egg-info/SOURCES.txt
-SDMXthon.egg-info/dependency_links.txt
-SDMXthon.egg-info/requires.txt
-SDMXthon.egg-info/top_level.txt
 sdmxthon/__init__.py
 sdmxthon.egg-info/PKG-INFO
 sdmxthon.egg-info/SOURCES.txt
 sdmxthon.egg-info/dependency_links.txt
 sdmxthon.egg-info/requires.txt
 sdmxthon.egg-info/top_level.txt
-sdmxthon/WebServices/__init__.py
-sdmxthon/WebServices/app.py
-sdmxthon/WebServices/sdmx_requests.py
-sdmxthon/WebServices/test.py
 sdmxthon/api/api.py
 sdmxthon/model/__init__.py
 sdmxthon/model/base.py
 sdmxthon/model/component.py
 sdmxthon/model/dataset.py
 sdmxthon/model/definitions.py
 sdmxthon/model/descriptors.py
```

### Comparing `sdmxthon-2.1/sdmxthon/api/api.py` & `sdmxthon-2.2/sdmxthon/api/api.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/base.py` & `sdmxthon-2.2/sdmxthon/model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         return self._content
 
     @content.setter
     def content(self, value):
         self._content = string_setter(value)
 
 
-class InternationalString(object):
+class InternationalString:
     """The International String is a collection of Localised
        Strings and supports the representation of text in
        multiple locales.
     """
 
     def __init__(self, localisedStrings: List[LocalisedString] = None):
         """Inits InternationalString with optional attributes."""
@@ -124,14 +124,24 @@
                     .replace("<", "&lt;").replace(">", "&gt;")
                 outfile.append(
                     f'{child1}<{name} xml:lang="{label}">'
                     f'{text}</{name}>')
 
         return outfile
 
+    @classmethod
+    def from_str(cls, value):
+        """
+        Generates InternationalString from a str
+        :param value: Content of the String
+        :return: A InternationalString instance
+        """
+        return cls([LocalisedString(locale='English', label='en',
+                                    content=value)])
+
 
 class Annotation(object):
     """Additional descriptive information attached to an object"""
 
     def __init__(self, id_: str = None, title: str = None, type_: str = None,
                  url: str = None, text: InternationalString = None):
         self.id = id_
@@ -353,14 +363,19 @@
     def __init__(self, id_: str = None, uri: str = None, urn=None,
                  annotations: List[Annotation] = None,
                  name: InternationalString = None,
                  description: InternationalString = None):
         super(NameableArtefact, self).__init__(id_=id_, uri=uri, urn=urn,
                                                annotations=annotations)
 
+        if isinstance(name, str):
+            name = InternationalString.from_str(name)
+        if isinstance(description, str):
+            description = InternationalString.from_str(description)
+
         self._name = name
         self._description = description
 
     def __eq__(self, other):
         if isinstance(other, NameableArtefact):
             return (super(NameableArtefact, self).__eq__(other) and
                     self._name == other._name and
```

### Comparing `sdmxthon-2.1/sdmxthon/model/component.py` & `sdmxthon-2.2/sdmxthon/model/component.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/dataset.py` & `sdmxthon-2.2/sdmxthon/model/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,25 +303,34 @@
 
         :param pathToFeather: Path to Feather file
         :type pathToFeather: str
 
         """
         self.data.to_feather(pathToFeather, **kwargs)
 
-    def semantic_validation(self):
-        """Performs a Semantic Validation on the Data.
+    def structural_validation(self):
+        """Performs a Structural Validation on the Data.
 
         :returns:
             A list of errors as defined in the Validation Page.
 
         """
-        if isinstance(self.data, DataFrame):
-            return validate_data(self.data, self.structure)
-        raise ValueError(f'Data for dataset {self.structure.id} '
+        if self.data is None:
+            raise ValueError('The dataset should contain data to perform a structural validation')
+        elif self.structure is None:
+            raise ValueError('The dataset should contain a structure to perform a structural validation')
+        
+        if not isinstance(self.data, DataFrame):
+            raise ValueError(f'Data for dataset {self.structure.id} '
                          f'is not well formed')
+        elif not isinstance(self.structure, DataStructureDefinition):
+            raise TypeError('structure must be a DataStructureDefinition')
+            
+            
+        return validate_data(self.data, self.structure)
 
     def set_dimension_at_observation(self, dimAtObs):
         """Sets the dimensionAtObservation
             :param dimAtObs: Dimension At Observation
             :type dimAtObs: str
         """
         if (dimAtObs in self.structure.dimension_codes or
```

### Comparing `sdmxthon-2.1/sdmxthon/model/definitions.py` & `sdmxthon-2.2/sdmxthon/model/definitions.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/descriptors.py` & `sdmxthon-2.2/sdmxthon/model/descriptors.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/extras.py` & `sdmxthon-2.2/sdmxthon/model/extras.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/header.py` & `sdmxthon-2.2/sdmxthon/model/header.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/itemScheme.py` & `sdmxthon-2.2/sdmxthon/model/itemScheme.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/message.py` & `sdmxthon-2.2/sdmxthon/model/message.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/representation.py` & `sdmxthon-2.2/sdmxthon/model/representation.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/model/utils.py` & `sdmxthon-2.2/sdmxthon/model/utils.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/parsers/data_read.py` & `sdmxthon-2.2/sdmxthon/parsers/data_read.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/parsers/data_validations.py` & `sdmxthon-2.2/sdmxthon/parsers/data_validations.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/parsers/metadata_read.py` & `sdmxthon-2.2/sdmxthon/parsers/metadata_read.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/parsers/read.py` & `sdmxthon-2.2/sdmxthon/parsers/read.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/parsers/write.py` & `sdmxthon-2.2/sdmxthon/parsers/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from datetime import datetime
-from io import StringIO
 
 import pandas as pd
 
 from sdmxthon.model.component import PrimaryMeasure
 from sdmxthon.model.header import Header, Sender, Party
 from sdmxthon.parsers.data_validations import get_mandatory_attributes
 from sdmxthon.utils.enums import MessageTypeEnum
@@ -267,17 +266,15 @@
             outfile += parse_metadata(payload, prettyprint)
     outfile += f'</{messageAbbr}:{data_type_string}>'
 
     if path != '':
         with open(path, "w", encoding="UTF-8", errors='replace') as f:
             f.write(outfile)
     else:
-        f = StringIO()
-        f.write(outfile)
-        return f
+        return outfile
 
 
 def format_dict_ser(out, parser, data_dict, obs):
     data_dict['Series'][0]['Obs'] = obs.to_dict(orient="records")
     out.append(parser(data_dict['Series'][0]))
     del data_dict['Series'][0]
```

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXCommon.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXCommon.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXCommonReferences.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXCommonReferences.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXDataGeneric.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXDataGeneric.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXDataGenericBase.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXDataGenericBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXDataStructureSpecific.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXDataStructureSpecific.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXMessage.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXMessage.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXMessageFooter.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXMessageFooter.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXMetadataGeneric.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXMetadataGeneric.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQuery.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQuery.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryBase.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryCategorisation.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryCategorisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryCategory.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryCategory.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryCodelist.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryConcept.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryConcept.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryConstraint.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryConstraint.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryData.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryDataStructure.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryDataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryDataflow.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryDataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryMetadata.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryMetadata.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryMetadataflow.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryMetadataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryOrganisation.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryOrganisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryProcess.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryProcess.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQuerySchema.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQuerySchema.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryStructureSet.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryStructureSet.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXQueryStructures.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXQueryStructures.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXRegistry.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXRegistry.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXRegistryBase.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXRegistryBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXRegistryRegistration.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXRegistryRegistration.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXRegistryStructure.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXRegistryStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXRegistrySubscription.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXRegistrySubscription.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructure.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureBase.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureCategorisation.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureCategorisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureCategory.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureCategory.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureCodelist.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureConcept.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureConcept.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureConstraint.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureConstraint.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureDataStructure.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureDataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureDataflow.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureDataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureMetadataflow.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureMetadataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureOrganisation.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureOrganisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureProcess.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureProcess.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/SDMXStructureStructureSet.xsd` & `sdmxthon-2.2/sdmxthon/schemas/SDMXStructureStructureSet.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/schemas/xml.xsd` & `sdmxthon-2.2/sdmxthon/schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/utils/handlers.py` & `sdmxthon-2.2/sdmxthon/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/utils/mappings.py` & `sdmxthon-2.2/sdmxthon/utils/mappings.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/utils/parsing_words.py` & `sdmxthon-2.2/sdmxthon/utils/parsing_words.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/sdmxthon/utils/xml_base.py` & `sdmxthon-2.2/sdmxthon/utils/xml_base.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.1/setup.py` & `sdmxthon-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     name='sdmxthon',
     description='Library with SDMX to Pandas, Pandas to SDMX, '
                 'SDMX validation and SDMX metadata validation',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     packages=setuptools.find_packages(exclude=["testSuite"]),
     include_package_data=True,
-    version='2.1',
+    version='2.2',
     license='Apache 2.0',
     license_files='license.txt',
     author='MeaningfulData',
     author_email='javier.hernandez@meaningfuldata.eu',
     project_urls={
         'Bug Tracker': 'https://github.com/Meaningful-Data/sdmxthon/issues',
         'Documentation': 'https://docs.sdmxthon.meaningfuldata.eu',
```

