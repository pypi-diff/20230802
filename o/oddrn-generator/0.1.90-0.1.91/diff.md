# Comparing `tmp/oddrn_generator-0.1.90.tar.gz` & `tmp/oddrn_generator-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oddrn_generator-0.1.90.tar", max compression
+gzip compressed data, was "oddrn_generator-0.1.91.tar", max compression
```

## Comparing `oddrn_generator-0.1.90.tar` & `oddrn_generator-0.1.91.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11356 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/LICENSE
--rw-r--r--   0        0        0     6337 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/README.md
--rw-r--r--   0        0        0     2722 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/__init__.py
--rw-r--r--   0        0        0      158 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/exceptions.py
--rw-r--r--   0        0        0    12718 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/generators.py
--rw-r--r--   0        0        0    24577 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/path_models.py
--rw-r--r--   0        0        0     3652 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/server_models.py
--rw-r--r--   0        0        0      287 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/utils/__init__.py
--rw-r--r--   0        0        0     7327 2023-07-28 12:41:12.000000 oddrn_generator-0.1.90/oddrn_generator/utils/external_generators.py
--rw-r--r--   0        0        0      734 2023-07-28 12:41:43.000000 oddrn_generator-0.1.90/pyproject.toml
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 oddrn_generator-0.1.90/setup.py
--rw-r--r--   0        0        0     7089 1970-01-01 00:00:00.000000 oddrn_generator-0.1.90/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/LICENSE
+-rw-r--r--   0        0        0     6337 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/README.md
+-rw-r--r--   0        0        0     2786 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/oddrn_generator/__init__.py
+-rw-r--r--   0        0        0      158 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/oddrn_generator/exceptions.py
+-rw-r--r--   0        0        0    12925 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/oddrn_generator/generators.py
+-rw-r--r--   0        0        0    24803 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/oddrn_generator/path_models.py
+-rw-r--r--   0        0        0     4381 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/oddrn_generator/server_models.py
+-rw-r--r--   0        0        0      287 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/oddrn_generator/utils/__init__.py
+-rw-r--r--   0        0        0     7327 2023-08-02 08:24:24.000000 oddrn_generator-0.1.91/oddrn_generator/utils/external_generators.py
+-rw-r--r--   0        0        0      734 2023-08-02 08:25:02.000000 oddrn_generator-0.1.91/pyproject.toml
+-rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 oddrn_generator-0.1.91/setup.py
+-rw-r--r--   0        0        0     7089 1970-01-01 00:00:00.000000 oddrn_generator-0.1.91/PKG-INFO
```

### Comparing `oddrn_generator-0.1.90/LICENSE` & `oddrn_generator-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.90/README.md` & `oddrn_generator-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.90/oddrn_generator/__init__.py` & `oddrn_generator-0.1.91/oddrn_generator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     TarantoolGenerator,
     TrinoGenerator,
     VerticaGenerator,
     BigTableGenerator,
     DuckDBGenerator,
     ScyllaDBGenerator,
     GCSGenerator,
+    AzureBlobStorageGenerator,
 )
 
 __all__ = [
     "AirbyteGenerator",
     "AirflowGenerator",
     "AthenaGenerator",
     "AzureSQLGenerator",
@@ -110,8 +111,9 @@
     "VerticaGenerator",
     "SQLiteGenerator",
     "S3CustomGenerator",
     "BigTableGenerator",
     "DuckDBGenerator",
     "ScyllaDBGenerator",
     "GCSGenerator",
+    "AzureBlobStorageGenerator",
 ]
```

### Comparing `oddrn_generator-0.1.90/oddrn_generator/generators.py` & `oddrn_generator-0.1.91/oddrn_generator/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,19 +52,21 @@
     SingleStorePathsModel,
     SnowflakePathsModel,
     SQLitePathsModel,
     SupersetPathsModel,
     TableauPathsModel,
     TarantoolPathsModel,
     VerticaPathsModel,
+    BlobPathsModel,
 )
 from oddrn_generator.server_models import (
     AbstractServerModel,
     AWSCloudModel,
-    AzureCloudModel,
+    BlobStorageCloudModel,
+    AzureDomainCloudModel,
     AzureCloudSettings,
     CloudSettings,
     GCPCloudModel,
     GoogleCloudSettings,
     HostnameModel,
     HostSettings,
     S3CloudModel,
@@ -409,15 +411,15 @@
     paths_model = DmsPathsModel
     server_model = AWSCloudModel
 
 
 class PowerBiGenerator(Generator):
     source = "powerbi"
     paths_model = PowerBiPathModel
-    server_model = AzureCloudModel
+    server_model = AzureDomainCloudModel
 
 
 class RedashGenerator(Generator):
     source = "redash"
     paths_model = RedashPathsModel
     server_model = HostnameModel
 
@@ -514,7 +516,13 @@
     server_model = HostnameModel
 
 
 class GCSGenerator(Generator):
     source = "gcs"
     paths_model = GCSPathsModel
     server_model = GCPCloudModel
+
+
+class AzureBlobStorageGenerator(Generator):
+    source = "blob_storage"
+    paths_model = BlobPathsModel
+    server_model = BlobStorageCloudModel
```

### Comparing `oddrn_generator-0.1.90/oddrn_generator/path_models.py` & `oddrn_generator-0.1.91/oddrn_generator/path_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,7 +824,18 @@
 
     class Config:
         dependencies_map = {
             "buckets": ("buckets",),
             "keys": ("buckets", "keys"),
             "columns": ("buckets", "keys", "columns"),
         }
+
+
+class BlobPathsModel(BasePathsModel):
+    keys: Optional[str]
+    columns: Optional[str]
+
+    class Config:
+        dependencies_map = {
+            "keys": ("keys", ),
+            "columns": ("keys", "columns", )
+        }
```

### Comparing `oddrn_generator-0.1.90/oddrn_generator/server_models.py` & `oddrn_generator-0.1.91/oddrn_generator/server_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from abc import ABC, abstractmethod
 from urllib.parse import urlparse
-
+from typing import Optional
 from pydantic import BaseModel, validator
 
 
 class HostSettings(BaseModel):
     host: str
 
 
 class CloudSettings(BaseModel):
     account: str
     region: str
 
 
 class AzureCloudSettings(BaseModel):
-    domain: str
+    domain: Optional[str]
+    account: Optional[str]
+    container: Optional[str]
 
 
 class GoogleCloudSettings(BaseModel):
     project: str
 
 
 class S3CustomSettings(BaseModel):
@@ -81,15 +83,15 @@
 
         if cloud_settings:
             return cls(account=cloud_settings.account, region=cloud_settings.region)
         else:
             raise ValueError("You must specify cloud settings")
 
 
-class AzureCloudModel(AbstractServerModel, BaseModel):
+class AzureDomainCloudModel(AbstractServerModel, BaseModel):
     domain: str
 
     def __str__(self) -> str:
         return (
             f"cloud/azure/{'/'.join('{}/{}'.format(*p) for p in self.dict().items())}"
         )
 
@@ -99,14 +101,36 @@
 
         if azure_cloud_settings:
             return cls(domain=azure_cloud_settings.domain)
         else:
             raise ValueError("You must specify cloud settings")
 
 
+class BlobStorageCloudModel(AbstractServerModel, BaseModel):
+    account: str
+    container: str
+
+    def __str__(self) -> str:
+        return (
+            f"cloud/azure/{'/'.join('{}/{}'.format(*p) for p in self.dict().items())}"
+        )
+
+    @classmethod
+    def create(cls, config: ServerModelConfig):
+        azure_cloud_settings = config.azure_cloud_settings
+
+        if azure_cloud_settings:
+            return cls(
+                account=azure_cloud_settings.account,
+                container=azure_cloud_settings.container
+            )
+        else:
+            raise ValueError("You must specify cloud settings")
+
+
 class S3CustomModel(AbstractServerModel, BaseModel):
     endpoint: str
 
     def __str__(self) -> str:
         return f"{'/'.join('{}/{}'.format(*p) for p in self.dict().items())}"
 
     @classmethod
```

### Comparing `oddrn_generator-0.1.90/oddrn_generator/utils/external_generators.py` & `oddrn_generator-0.1.91/oddrn_generator/utils/external_generators.py`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.90/pyproject.toml` & `oddrn_generator-0.1.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oddrn-generator"
-version = "0.1.90"
+version = "0.1.91"
 description = "Open Data Discovery Resource Name Generator"
 authors = ["Open Data Discovery <pypi@opendatadiscovery.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/opendatadiscovery/oddrn-generator"
 repository = "https://github.com/opendatadiscovery/oddrn-generator"
 keywords = ["oddrn", "opendatadiscovery"]
```

### Comparing `oddrn_generator-0.1.90/setup.py` & `oddrn_generator-0.1.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'oddrn-generator',
-    'version': '0.1.90',
+    'version': '0.1.91',
     'description': 'Open Data Discovery Resource Name Generator',
     'long_description': '[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)\n\n# Open Data Discovery Resource Name Generator\n\nHelps generate oddrn for data sources.\n\n* [Requirements](#requirements)\n* [Installation](#installation)\n* [Available generators](#available-generators)\n* [Generator properties](#generator-properties)\n* [Generator methods](#generator-methods)\n* [Generator properties](#generator-properties)\n* [Example usage](#example-usage)\n* [Exceptions](#example-usage)\n* [Development](#development)\n\n## Requirements\n\n* __Python >= 3.7__\n\n## Installation\n\n```bash\npoetry add oddrn-generator\n# or\npip install oddrn-generator\n```\n\n## Usage and configuration\n\n### Available generators\n| DataSource   | Generator class name  |\n|--------------|-----------------------|\n| cassandra    | CassandraGenerator    |\n| postgresql   | PostgresqlGenerator   |\n| mysql        | MysqlGenerator        |\n| glue         | GlueGenerator         |\n| s3           | S3Generator           |\n| kafka        | KafkaGenerator        |\n| kafkaconnect | KafkaConnectGenerator |\n| snowflake    | SnowflakeGenerator    |\n| airflow      | AirflowGenerator      |\n| hive         | HiveGenerator         |\n| dynamodb     | DynamodbGenerator     |\n| odbc         | OdbcGenerator         |\n| mssql        | MssqlGenerator        |\n| oracle       | OracleGenerator       |\n| redshift     | RedshiftGenerator     |\n| clickhouse   | ClickHouseGenerator   |\n| athena       | AthenaGenerator       |\n| quicksight   | QuicksightGenerator   |\n| dbt          | DbtGenerator          |\n| prefect      | PrefectGenerator      |\n| tableau      | TableauGenerator      |\n| neo4j        | Neo4jGenerator        |\n| mongodb      | MongoGenerator        |\n| vertica      | VerticaGenerator      |\n| CubeJs       | CubeJsGenerator       |\n| superset     | SupersetGenerator     |\n| Presto       | PrestoGenerator       |\n| Trino        | TrinoGenerator        |\n| dms          | DmsGenerator          |\n| powerbi      | PowerBiGenerator      |\n\n### Generator properties\n\n* base_oddrn - Get base oddrn (without path)\n* available_paths - Get all available path of generator\n\n### Generator methods\n\n* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using \'\n  new_value\' param\n* set_oddrn_paths(**kwargs) - Set or update values of oddrn path\n* get_data_source_oddrn() - Get data source oddrn\n\n### Generator parameters:\n\n* host_settings: str - optional. Hostname configuration\n* cloud_settings: dict - optional. Cloud configuration\n* **kwargs - path\'s name and values\n\n### Example usage\n\n```python\n# postgresql\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\', tables=\'table_name\'\n)\n\noddrn_gen.base_oddrn\n# //postgresql/host/my.host.com:5432\noddrn_gen.available_paths\n# (\'schemas\', \'databases\', \'tables\', \'columns\')\n\noddrn_gen.get_data_source_oddrn()\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("schemas")\n# //postgresql/host/my.host.com:5432/schemas/schema_name\n\noddrn_gen.get_oddrn_by_path("databases")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/table_name\n\n# you can set or change path:\noddrn_gen.set_oddrn_paths(tables=\'another_table_name\', columns=\'new_column_name\')\noddrn_gen.get_oddrn_by_path("columns")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/new_column_name\n\n# you can get path wih new values:\noddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name\n\n\n# glue\nfrom oddrn_generator import GlueGenerator\n\noddrn_gen = GlueGenerator(\n    cloud_settings={\'account\': \'acc_id\', \'region\': \'reg_id\'},\n    databases=\'database_name\', tables=\'table_name\', columns=\'column_name\',\n    jobs=\'job_name\', runs=\'run_name\', owners=\'owner_name\'\n)\n\noddrn_gen.available_paths\n# (\'databases\', \'tables\', \'columns\', \'owners\', \'jobs\', \'runs\')\n\noddrn_gen.get_oddrn_by_path("databases")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name\'\n\noddrn_gen.get_oddrn_by_path("columns")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name/columns/column_name\n\noddrn_gen.get_oddrn_by_path("jobs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name\n\noddrn_gen.get_oddrn_by_path("runs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name/runs/run_name\n\noddrn_gen.get_oddrn_by_path("owners")\n# //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name\n\n```\n\n### Exceptions\n\n* WrongPathOrderException - raises when trying set path that depends on another path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\',\n    columns=\'column_without_table\'\n)\n# WrongPathOrderException: \'columns\' can not be without \'tables\' attribute\n```\n\n* EmptyPathValueException - raises when trying to get a path that is not set up\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("tables")\n\n# EmptyPathValueException: Path \'tables\' is not set up\n```\n\n* PathDoestExistException - raises when trying to get not existing oddrn path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("jobs")\n\n# PathDoestExistException: Path \'jobs\' doesn\'t exist in generator\n```\n\n## Development\n\n```bash\n#Install dependencies\npoetry install\n\n#Activate shell\npoetry shell\n\n# Run tests\npython run pytest\n```\n',
     'author': 'Open Data Discovery',
     'author_email': 'pypi@opendatadiscovery.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/opendatadiscovery/oddrn-generator',
```

### Comparing `oddrn_generator-0.1.90/PKG-INFO` & `oddrn_generator-0.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oddrn-generator
-Version: 0.1.90
+Version: 0.1.91
 Summary: Open Data Discovery Resource Name Generator
 Home-page: https://github.com/opendatadiscovery/oddrn-generator
 License: Apache-2.0
 Keywords: oddrn,opendatadiscovery
 Author: Open Data Discovery
 Author-email: pypi@opendatadiscovery.org
 Requires-Python: >=3.9,<4.0
```

