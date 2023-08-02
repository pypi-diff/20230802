# Comparing `tmp/cjdb-1.2.0.tar.gz` & `tmp/cjdb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjdb-1.2.0.tar", max compression
+gzip compressed data, was "cjdb-2.0.0.tar", max compression
```

## Comparing `cjdb-1.2.0.tar` & `cjdb-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-03-24 08:47:24.943711 cjdb-1.2.0/LICENSE
--rw-r--r--   0        0        0    12711 2023-04-21 14:57:08.421775 cjdb-1.2.0/README.md
--rw-r--r--   0        0        0      167 2023-04-21 14:57:08.422846 cjdb-1.2.0/cjdb/__init__.py
--rw-r--r--   0        0        0      218 2023-04-21 14:57:08.423404 cjdb-1.2.0/cjdb/logger.py
--rw-r--r--   0        0        0      648 2023-04-21 14:57:08.423822 cjdb-1.2.0/cjdb/main.py
--rw-r--r--   0        0        0     4966 2023-04-21 14:57:08.424374 cjdb-1.2.0/cjdb/model/README.md
--rw-r--r--   0        0        0        0 2023-04-11 07:29:22.588412 cjdb-1.2.0/cjdb/model/__init__.py
--rw-r--r--   0        0        0     5239 2023-04-21 14:57:08.424706 cjdb-1.2.0/cjdb/model/sqlalchemy_models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 07:29:22.588804 cjdb-1.2.0/cjdb/modules/__init__.py
--rw-r--r--   0        0        0     3410 2023-04-21 14:57:08.425457 cjdb-1.2.0/cjdb/modules/arg_parser.py
--rw-r--r--   0        0        0     2180 2023-04-21 14:57:08.425797 cjdb-1.2.0/cjdb/modules/checks.py
--rw-r--r--   0        0        0      838 2023-04-21 14:57:08.426042 cjdb-1.2.0/cjdb/modules/exceptions.py
--rw-r--r--   0        0        0     2081 2023-04-21 14:57:08.426320 cjdb-1.2.0/cjdb/modules/extensions.py
--rw-r--r--   0        0        0     6847 2023-04-21 14:57:08.426679 cjdb-1.2.0/cjdb/modules/geometric.py
--rw-r--r--   0        0        0    16607 2023-04-21 14:57:08.426996 cjdb-1.2.0/cjdb/modules/importer.py
--rw-r--r--   0        0        0     1599 2023-04-21 14:57:08.427292 cjdb-1.2.0/cjdb/modules/utils.py
--rw-r--r--   0        0        0        0 2023-04-11 07:29:22.590399 cjdb-1.2.0/cjdb/resources/__init__.py
--rw-r--r--   0        0        0      875 2023-04-21 14:57:08.427663 cjdb-1.2.0/cjdb/resources/object_types.py
--rw-r--r--   0        0        0      802 2023-04-21 14:57:08.427887 cjdb-1.2.0/cjdb/resources/post_import.sql
--rw-r--r--   0        0        0     2107 2023-04-21 14:57:08.428211 cjdb-1.2.0/cjdb/resources/strings.py
--rw-r--r--   0        0        0      926 2023-04-21 14:57:08.429390 cjdb-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    14134 1970-01-01 00:00:00.000000 cjdb-1.2.0/setup.py
--rw-r--r--   0        0        0    13597 1970-01-01 00:00:00.000000 cjdb-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-24 08:47:24.943711 cjdb-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9098 2023-08-02 12:58:30.738475 cjdb-2.0.0/README.md
+-rw-r--r--   0        0        0      167 2023-04-26 14:13:59.366331 cjdb-2.0.0/cjdb/__init__.py
+-rw-r--r--   0        0        0     4553 2023-08-02 12:58:30.739343 cjdb-2.0.0/cjdb/cli.py
+-rw-r--r--   0        0        0      218 2023-04-21 14:57:08.423404 cjdb-2.0.0/cjdb/logger.py
+-rw-r--r--   0        0        0     1308 2023-08-02 12:58:30.739602 cjdb-2.0.0/cjdb/model/BASICQUERIES.md
+-rw-r--r--   0        0        0     4324 2023-08-02 12:58:30.740126 cjdb-2.0.0/cjdb/model/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 07:29:22.588412 cjdb-2.0.0/cjdb/model/__init__.py
+-rw-r--r--   0        0        0     4337 2023-08-02 12:58:30.740529 cjdb-2.0.0/cjdb/model/sqlalchemy_models/__init__.py
+-rw-r--r--   0        0        0    60850 2023-08-02 12:58:30.741174 cjdb-2.0.0/cjdb/model/uml.png
+-rw-r--r--   0        0        0        0 2023-04-11 07:29:22.588804 cjdb-2.0.0/cjdb/modules/__init__.py
+-rw-r--r--   0        0        0     2180 2023-06-30 07:28:22.952965 cjdb-2.0.0/cjdb/modules/checks.py
+-rw-r--r--   0        0        0     2964 2023-08-02 12:58:30.741593 cjdb-2.0.0/cjdb/modules/exceptions.py
+-rw-r--r--   0        0        0    13885 2023-08-02 12:58:30.741956 cjdb-2.0.0/cjdb/modules/exporter.py
+-rw-r--r--   0        0        0     2363 2023-08-02 12:58:30.742242 cjdb-2.0.0/cjdb/modules/extensions.py
+-rw-r--r--   0        0        0     8507 2023-08-02 12:58:30.742568 cjdb-2.0.0/cjdb/modules/geometric.py
+-rw-r--r--   0        0        0    20058 2023-08-02 12:58:30.743090 cjdb-2.0.0/cjdb/modules/importer.py
+-rw-r--r--   0        0        0     1887 2023-08-02 12:58:30.743387 cjdb-2.0.0/cjdb/modules/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:29:22.590399 cjdb-2.0.0/cjdb/resources/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-21 14:57:08.427663 cjdb-2.0.0/cjdb/resources/object_types.py
+-rw-r--r--   0        0        0      913 2023-08-02 12:58:30.743667 cjdb-2.0.0/cjdb/resources/post_import.sql
+-rw-r--r--   0        0        0     1859 2023-08-02 12:58:30.743947 cjdb-2.0.0/cjdb/resources/strings.py
+-rw-r--r--   0        0        0     1006 2023-08-02 12:58:30.754701 cjdb-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10339 1970-01-01 00:00:00.000000 cjdb-2.0.0/setup.py
+-rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 cjdb-2.0.0/PKG-INFO
```

### Comparing `cjdb-1.2.0/LICENSE` & `cjdb-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cjdb-1.2.0/README.md` & `cjdb-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,350 +1,44 @@
-# cjdb
-[![MIT badge](https://img.shields.io/pypi/l/cjdb)](LICENSE) &nbsp; [![PyPI](https://img.shields.io/pypi/v/cjdb)](https://pypi.org/project/cjdb)
-
-`cjdb` is a Python based importer of CityJSONL files to a PostgreSQL database. It requires the [PostGIS](https://postgis.net/) extension.
-
-Authors: Cynthia Cai, Lan Yan, Yitong Xia, Chris Poon, Siebren Meines, Leon Powalka
-
-Maintainer: Gina Stavropoulou
-
-## Table of Contents  
-### [1.Data model](#1-data-model)
-### [2.Installation](#2-installation)
-- [Using pip](#using-pip)
-- [Using Docker](#using-docker)
-### [3.Usage](#3-usage)
-- [CLI](#cli)
-- [Quickstart](#quickstart)
-- [Basic Queries](#basic-queries)
-### [4.Local development](#4-local-development)
-- [Install and Build](#install-and-build)
-- [Testing](#testing)
-### [5.Explanation](#5-explanation)
- - [Model assumptions](#model-assumptions)
- - [What is a City Model?](#what-is-a-city-model)
- - [Types of input](#types-of-input)
- - [Coordinate Reference Systems](#coordinate-reference-systems)
- - [3D reprojections](#3d-reprojections)
- - [CityJSON Extensions](#cityjson-extensions)
- - [CityJSON GeometryTemplate](#cityjson-geometrytemplate)
- - [Data validation](#data-validation)
- - [Repeated object IDs](#repeated-object-ids)
----
-## 1. Data model
-For the underlying data model see [cjdb/model/README.md](cjdb/model/README.md)
-
-
-## 2. Installation
-### Using pip
-```bash
-pip install cjdb
-```
-It is recommended to install it in an isolated environment, because of fragile external library dependencies for CQL filter parsing.
-
-### Using docker
-Build:
-```bash
-docker build -t cjdb:latest .
-```
-
-Run:
-```bash
-docker run --rm -it cjdb cjdb --help
-```
-
-To import some files, the `-v` option is needed to mount our local file directory in the container:
-```bash
-docker run -v {MYDIRECTORY}:/data --rm -it --network=host cjdb cjdb -H localhost -U postgres -d postgres -W postgres /data/5870_ext.jsonl 
-```
-## 3. Usage <a name="usage"></a>
-
-### CLI <a name="cli"></a>
-
-```bash
-cj2pgsql [-h] [-H DB_HOST] [-p DB_PORT] -U DB_USER [-W DB_PASSWORD] -d DB_NAME [-s DB_SCHEMA] [-I TARGET_SRID][-x INDEXED_ATTRIBUTES] [-px PARTIAL_INDEXED_ATTRIBUTES] [-g] [-a | -o] [-e | -u] [file_or_directory]
-```
-#### Positional Arguments
-file_or_directory
-Source CityJSONL file or a directory with CityJSONL files. STDIN if not specified. If specifying a directory, all the *.jsonl files inside of it will be imported.
-
-Default: “stdin”
-
-#### Named Arguments
-`-I, --srid`
-Target coordinate system SRID. All 3D and 2D geometries will be reprojected.
-
-`-x, --attr-index`
-CityObject attribute to be indexed using a btree index. Can be specified multiple times, for each attribute once.
-
-Default: []
-
-`-px, --partial-attr-index`
-CityObject attribute to be indexed using a btree partial index. Can be specified multiple times, for each attribute once. This index indexes on a condition ‘where {
-                {ATTR_NAME
-                }
-        } is not null’. This means that it saves space and improves query performance when the attribute is not present for all imported CityObjects.
-
-Default: []
-
-`-g, --ignore-repeated-file`
-Ignore repeated file names warning when importing. By default, the importer will send out warnings if a specific file has already been imported.
-
-Default: False
-
-`-a, --append`
-Run in append mode (as opposed to default create mode). This assumes the database structure exists already and new data is to be appended.
-
-Default: False
-
-`-o, --overwrite`
-Overwrite the data that is currently in the database schema. Warning: this causes the loss of what was imported before to the database schema.
-
-Default: False
-
-`-u, --update-existing`
-Check if the object with given ID exists before inserting, and update it if it does. The old object will be updated with the new object’s properties.
-
-Default: False
-
-#### Database connection arguments
-`-H, --host`
-PostgreSQL database host
-
-Default: “localhost”
-
-`-p, --port`
-PostgreSQL database port
-
-Default: 5432
-
-`-U, --user`
-PostgreSQL database user name
-
-`-W, --password`
-PostgreSQL database user password
-
-`-d, --database`
-PostgreSQL database name
-
-`-s, --schema`
-Target database schema
-
-Default: “public”
-
-### Quickstart
-
-Sample CityJSON data can be downloaded from [3DBAG download service](https://3dbag.nl/nl/download?tid=901). Then, having the CityJSON file, a combination of [cjio](https://github.com/cityjson/cjio) (external CityJSON processing library) and cjdb is needed to import it to a specified schema in a database. 
-
-1. Convert CityJSON to CityJSONL
-
-```bash
-cjio --suppress_msg tile_901.json export jsonl tile_901.jsonl 
-```
-
-2. Create a new database
-
-  - [how to create a new database](https://postgis.net/workshops/postgis-intro/creating_db.html)
-
-3. Import CityJSONL to the database
-```bash
-PGPASSWORD=postgres cjdb -H localhost -U postgres -d postgres -s cjdb -o tile_901.jsonl   
-```
-
-**Alternatively steps 1 and 2 in a single command:**
-
-```bash
-cjio --suppress_msg tile_901.json export jsonl stdout | cjdb -H localhost -U postgres -d postgres -s cjdb -o
-```
-
-The metadata and the objects can then be found in the tables in the specified schema (`cjdb` in this example).
-
-
-Password can be specified in the `PGPASSWORD` environment variable. If not specified, the app will prompt for the password.
-
-
-### Basic Queries
-
-- Query an object with a specific id:
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE object_id = 'NL.IMBAG.Pand.0503100000000334';
-```
-
-- Query a building with a specific child
-```SQL
-SELECT o.* FROM cjdb.family f
-INNER JOIN cjdb.cj_object o ON o.object_id = f.parent_id
-WHERE f.child_id = 'NL.IMBAG.Pand.0503100000000334-0'
-```
-
-- Query all buildings within a bounding box
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE type = 'Building'
-AND ST_Contains(ST_MakeEnvelope(81900.00, 446850.00, 81930.00, 446900.00, 7415), ground_geometry)
-ORDER BY id ASC;
-```
-
-- Query the building intersecting with a point
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE ground_geometry && ST_MakePoint(81915.00, 446850.00)
-AND type = 'Building'
-ORDER BY object_id ASC;
-```
-
-- Query all objects with a slanted roof
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE (attributes->'dak_type')::varchar = '"slanted"'
-ORDER BY id ASC;
-```
-
-- Query all the buildings made after 2000:
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE (attributes->'oorspronkelijkbouwjaar')::int > 2000
-AND type = 'Building'
-ORDER BY id ASC;
-```
-
-- Query all objects with LOD 1.2
-
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE geometry::jsonb @> '[{"lod": 1.2}]'::jsonb
-```
-
-## 4. Local development
-
-### Install and Build
-Make sure [poetry](https://python-poetry.org/docs/) is installed and the [creation of virtual environments within the project is allowed](
-https://python-poetry.org/docs/configuration/#virtualenvsin-project):
-
-```
-poetry config virtualenvs.in-project true
-```
-
-Then, to create a local environment with all the necessary dependencies, run from the repository root:
-```bash
-poetry install
-```
-
-To activate the env:
-```bash
-source .venv/bin/activate 
-```
-
-Then you can run the CLI command:
-```bash
-cjdb --help
-```
-
-Every time you make some changed to the package you can run `poetry install` to reinstall.
-
-
-### Testing
-In onder to run the tests you need to have [PostgreSQL](https://www.postgresql.org/download/) installed. Then you can run:
-
-```bash
-pytest -v
-```
-
-## 5. Explanation
----
-### Model assumptions
-The `cjdb` importer loads the data in accordance with a specific data model.
-
-Model documentation:
- [model/README](model/README.md)
-
-#### Indexes
-Some indexes are created by default (refer to [model/README](model/README.md)).
-
-Additionally, the user can specify which CityObject attributes are to be indexed with the `-x/--attr-index` or `-px/--partial-attr-index` flag, we recommend doing this if several queries are made on specific attributes. 
-The second option uses a partial index with a `not null` condition on the attribute. This saves disk space when indexing an attribute that is not present among all the imported CityObjects. 
-This is often the case with CityJSON, because in a single dataset there can be different object types, with different attributes.
-
-
-### Structuring the database and its schemas
-
-It is recommended to group together semantically coherent objects, by importing them to the same database schema.
-One database can have different schemas.
-
-While the current data model supports the import of any type of CityJSON objects together (`Building` and `SolitaryVegetationObject`), the data becomes harder to manage for the user. 
-Example of this would be having different attributes for the same CityObject type (which should be consistent for data coming from the same source).
-
-
-### Input == CityJSONFeature
-The importer works only on [*CityJSONL* files](https://www.cityjson.org/specs/#text-sequences-and-streaming-with-cityjsonfeature), that is where a CityJSON file is decomposed into its *features* (`CityJSONFeature`).
-
-The easiest way to create these from a CityJSON file is with [cjio](https://github.com/cityjson/cjio), and to follow [those instructions](https://github.com/cityjson/cjio#stdin-and-stdout).
-
-The importer supports 3 kinds of input:
-  1. a single CityJSONL file (only those as the output of cjio currently work)
-  1. a directory of CityJSONL files (all files with *jsonl* extensions are located and imported)
-  1. STDIN using the pipe operator: `cat file.jsonl | cjdb ...`
-
-
-
-### Coordinate Reference Systems
-The `cjdb` importer does not allow inconsistent CRSs (coordinate reference systems) within the same database schema. For storing data in separate CRSs, you have to use different schemas.
-
-The data needs to be either harmonized beforehand, or the `-I/--srid` flag can be used upon import, to reproject all the geometries to the one specified CRS. 
-Specifying a 2D CRS (instead of a 3D one) will cause the Z-coordinates to remain unchanged.
-
-**Note:** reprojections slow down the import significantly.
-
-**Note:** Source data with missing `"metadata"/"referenceSystem"` cannot be reprojected due to unknown source reference system.
-
-
-### 3D reprojections
-[`pyproj`](https://pyproj4.github.io/pyproj/stable/) is used for CRS reprojections. 
-While it supports 3D CRS transformations between different systems, sometimes downloading additional [grids](https://pyproj4.github.io/pyproj/stable/transformation_grids.html) is required. 
-The importer will attempt to download the grids needed for the reprojection, with the following message:
-
-```
-Attempting to download additional grids required for CRS transformation.
-This can also be done manually, and the files should be put in this folder:
-        {pyproj_directory}
-```
-
-If that fails, the user will have to download the required grids and put them in the printed `{pyproj_directory}` themselves. 
-
-
-### CityJSON Extensions
-If [CityJSON Extensions](https://www.cityjson.org/extensions/) are present in the imported files, they can be found listed in the `extensions` column in the `import_meta` table.
-
-The [CityJSON specifications](https://www.cityjson.org/specs/#extensions) mention 3 different extendable features, and the `cjdb` importer deals with them as follows:
-
-1. Complex attributes
-
-No action is taken. These attributes end up in the `attributes` JSONB column.
-
-2. Additional root properties
-
-Additional root properties are placed in the `extra properties` JSONB column in the `import_meta` table.
-
-3. Additional CityObject type
-
-Additional CityObject types are appended to the list of allowed CityJSON objects.
-
-### CityJSON GeometryTemplate
-[Geometry templates](https://www.cityjson.org/specs/1.1.2/#geometry-templates)
-are resolved for each object geometry, so that the object in the table ends up with its real-world coordinates (instead of vertex references or relative template coordinates).
-
-### Data validation
-The importer does not validate the structure of the file. It is assumed that the input file is schema-valid ([CityJSON validator](https://validator.cityjson.org/)).
-It sends out warnings when:
-- there appear CityObject types defined neither in the main CityJSON specification nor any of the supplied extensions. 
-- the specified target CRS does not have the Z-axis defined
-- the source dataset does not have a CRS defined at all
-
-### Repeated object IDs
-By default, the importer does not check if an object with a given ID exists already in the database. This is because such an operation for every inserted object results in a performance penalty.
-
-The user can choose to run the import with either the `-e/--skip-existing` option to skip existing objects or `-u, --update-existing` to update existing objects. This will slow down the import, but it will also ensure that repeated object cases are handled.
-
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
+packages = \
+['cjdb',
+ 'cjdb.model',
+ 'cjdb.model.sqlalchemy_models',
+ 'cjdb.modules',
+ 'cjdb.resources']
+
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['cjio>=0.8.1,<0.9.0',
+ 'geoalchemy2>=0.13.1,<0.14.0',
+ 'numpy>=1.24.2,<2.0.0',
+ 'psycopg2-binary>=2.9.6,<3.0.0',
+ 'pyproj>=3.5.0,<4.0.0',
+ 'requests>=2.28.2,<3.0.0',
+ 'shapely>=2.0.1,<3.0.0']
+
+entry_points = \
+{'console_scripts': ['cjdb = cjdb.cli:cjdb']}
+
+setup_kwargs = {
+    'name': 'cjdb',
+    'version': '2.0.0',
+    'description': 'CJDB is a tool that enables CityJSON integration with a PostgreSQL database',
+    'long_description': '# cjdb\n[![MIT badge](https://img.shields.io/pypi/l/cjdb)](LICENSE) &nbsp; [![PyPI](https://img.shields.io/pypi/v/cjdb)](https://pypi.org/project/cjdb)\n\n`cjdb` is a Python-based importer/exporter of [CityJSONL files (CityJSON Lines)](https://www.cityjson.org/cityjsonl/) to and from a PostgreSQL database. \nIt requires the [PostGIS](https://postgis.net/) extension.\n\n\n## Installation\n```bash\npip install cjdb\n```\nIt is recommended to install it in an isolated environment.\n\n\n## Usage\n\nCheck our [docs online](https://cityjson.github.io/cjdb/cjdb.html)  or\n\n```bash\ncjdb --help\n```\n\n## Quickstart\n\nSample CityJSON data can be downloaded from [the 3DBAG download service](https://3dbag.nl/). \nFor example, [download the tile "9-284-556"](https://data.3dbag.nl/cityjson/v20230622/tiles/9/284/556/9-284-556.city.json), within which part of TU Delft is located.\nThen, having downloaded the CityJSON file, you need a combination of [cjio](https://github.com/cityjson/cjio) (external CityJSON processing library) and cjdb to import it to a schema in a database.  Here is a step-by-step guide:\n\n1. Convert CityJSON to CityJSONL\n\n```bash\ncjio --suppress_msg 9-284-556.json export jsonl 9-284-556.jsonl \n```\n\n2. Create a new database called "testcjdb"\n\nIf you installed PostgreSQL you should have the program \'createdb\', so `createdb testcjdb`\n\nAlternatively, you can use PgAdmin, [see how](https://postgis.net/workshops/postgis-intro/creating_db.html).\n\n3. Import CityJSONL to the database in the schema "cjdb"\n```bash\ncjdb import -H localhost -U postgres -d testcjdb -s cjdb  -f 9-284-556.jsonl\n```\n\n**Alternatively steps 1 and 3 in a single command:**\n\n```bash\ncjio --suppress_msg 9-284-556.json export jsonl stdout | cjdb import -H localhost -U postgres -d postgres -s cjdb\n```\n\nThe metadata and the objects can then be found in the tables in the specified schema (`cjdb` in this example).\n\nThe password can be specified in the `PGPASSWORD` environment variable. If not specified, the app will prompt for the password.\n\n4. If you want to export from the database you have two options. You can export the whole database in a CityJSONL file with: \n```bash\ncjdb export -H localhost -U postgres -d testcjdb -s cjdb -o result.jsonl\n```\nor export only part of it, using a select query as input. The select query should return the ids of the objects to be exported:\n\n```bash\ncjdb export -H localhost -U postgres -d testcjdb -s cjdb -o result.jsonl -q "SELECT 1 as id"\n```\n\n## Using docker\nBuild:\n```bash\ndocker build -t cjdb:latest .\n```\n\nRun:\n```bash\ndocker run --rm -it cjdb cjdb --help\n```\n\nTo import some files, the `-v` option is needed to mount our local file directory in the container:\n```bash\ndocker run -v {MYDIRECTORY}:/data --rm -it --network=host cjdb cjdb import -H localhost -U postgres -d postgres -W postgres -f /data/5870_ext.jsonl \n```\n\n## Important Notes\n### Data model\n\nThe `cjdb` importer loads the data in accordance with a [specific data model](cjdb/model/README.md).\n\nFor example SQL queries on the tables see [here](cjdb/model/BASICQUERIES.md)\n\n\n### Indexes\nSome indexes are created when a new schema is created (refer to [Data Model](cjdb/model/README.md)).\n\nIn addition to these indexes, the user can add more indexes on certain  CityObject attributes with the `-x/--attr-index` or the `-px/--partial-attr-index` flags.\nWe recommend these additional indexes for attributes that are frequently queried.\nThe second option uses a partial index with a `not null` condition on the attribute.\nThis saves disk space when indexing an attribute that is not present among all the imported CityObjects.\nThis is often the case with CityJSON, because in a single dataset there can be different object types, with different attributes.\n\n\n### Structuring the database and its schemas\n\nIt is recommended to group together semantically coherent objects, by importing them to the same database schema.\nOne database can have different schemas.\n\nWhile the current data model supports the import of any type of CityJSON objects together (`Building` and `SolitaryVegetationObject`), the data becomes harder to manage for the user. \nExample of this would be having different attributes for the same CityObject type (which should be consistent for data coming from the same source).\n\n\n### Input == CityJSONFeature\nThe importer works only on with [*CityJSONL* files](https://www.cityjson.org/specs/#text-sequences-and-streaming-with-cityjsonfeature), which are CityJSON files decomposed into their *features* (`CityJSONFeature`).\n\nThe easiest way to create these from a CityJSON file is with [cjio](https://github.com/cityjson/cjio), by following [these instructions](https://github.com/cityjson/cjio#stdin-and-stdout).\n\nThe importer supports 3 kinds of input:\n  1. a single CityJSONL file (only those as the output of cjio currently work)\n  1. a directory of CityJSONL files (all files with *jsonl* extensions are located and imported)\n  1. STDIN using the pipe operator: `cat file.jsonl | cjdb ...`\n\n\n### Coordinate Reference Systems\nThe `cjdb` importer does not allow inconsistent CRSs (coordinate reference systems) within the same database schema. For storing data in different CRSs, you have to create different schemas.\n\nThe data needs to be either harmonized beforehand, or the `--transform` flag can be used upon import, to reproject all the geometries to the CRS of the existing schema. \nSpecifying a 2D CRS (instead of a 3D one) will cause the Z-coordinates to remain unchanged.\n\n**Note:** reprojections slow down the import significantly.\n\n**Note:** Source data with missing `"metadata"/"referenceSystem"` cannot be reprojected due to unknown source reference system. \nYou can use the `-I/--srid` flag to set the SRID of the input file. \n\n\n### 3D reprojections\n[`pyproj`](https://pyproj4.github.io/pyproj/stable/) is used for CRS reprojections. \nWhile it supports 3D CRS transformations between different systems, sometimes downloading additional [grids](https://pyproj4.github.io/pyproj/stable/transformation_grids.html) is required. \nThe importer will attempt to download the grids needed for the reprojection, with the following message:\n\n```\nAttempting to download additional grids required for CRS transformation.\nThis can also be done manually, and the files should be put in this folder:\n        {pyproj_directory}\n```\n\nIf that fails, the user will have to download the required grids and put them in the printed `{pyproj_directory}` themselves. \n\n\n### CityJSON Extensions\nIf [CityJSON Extensions](https://www.cityjson.org/extensions/) are present in the imported files, they can be found listed in the `extensions` column in the `cj_metadata` table.\n\nThe [CityJSON specifications](https://www.cityjson.org/specs/#extensions) mention 3 different extendable features, and the `cjdb` importer deals with them as follows:\n\n1. Complex attributes\n\nNo action is taken. These attributes end up in the `attributes` JSONB column.\n\n2. Additional root properties\n\nAdditional root properties are placed in the `extra properties` JSONB column in the `cj_metadata` table.\n\n3. Additional CityObject type\n\nAdditional CityObject types are appended to the list of allowed CityJSON objects.\n\n### CityJSON GeometryTemplate\n[Geometry templates](https://www.cityjson.org/specs/1.1.2/#geometry-templates)\nare resolved for each object geometry, so that the object in the table ends up with its real-world coordinates (instead of vertex references or relative template coordinates).\n\n### Data validation\nThe importer does not validate the structure of the file. It is assumed that the input file is schema-valid ([CityJSON validator](https://validator.cityjson.org/)).\nIt sends out warnings when:\n- CityObject types appear which are defined neither in the main CityJSON specification nor in any of the supplied extensions. \n- the specified target CRS does not have the Z-axis defined\n- the source dataset does not have a CRS defined at all\n\n### Repeated object IDs\nThe importer does not check if an object with a specific ID exists already in the database - every imported object gets and new id. However, at the time of import the importer will detect previously detected files with the same filename. The user can choose to run the import with either the `-g, --ignore-repeated-file` option to import files with the same filename under a different id or `--overwrite` to overwrite *all* previously imported objects with this filename.\n\n\n## Contributors\n\nThis project started as a group project in the [MSc Geomatics at TUDelft](https://geomatics.tudelft.nl/).\nThe original code for the project can be found [here](https://github.com/leoleonsio/cjdb), and the authors were:\n[@cynthiacai56](https://github.com/cynthiacai56), [@LanYan1110](https://github.com/LanYan1110), [@YitongXia](https://github.com/YitongXia), [@Topher2k](https://github.com/Topher2k), [@siebren014](https://github.com/siebren014), [@leoleonsio](https://github.com/leoleonsio)\n\nThis version has been improved and will be maintained by [@GinaStavropoulou](https://github.com/GinaStavropoulou), and [@hugoledoux](https://github.com/hugoledoux).\n\n',
+    'author': 'Cynthia Cai',
+    'author_email': 'None',
+    'maintainer': 'Gina Stavropoulou',
+    'maintainer_email': 'g.stavropoulou@tudelft.nl',
+    'url': 'https://github.com/tudelft3d/cjdb',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
+    'python_requires': '>=3.11,<4.0',
+}
 
 
+setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cjdb-1.2.0/cjdb/model/README.md` & `cjdb-2.0.0/cjdb/model/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-# cjdb data model
-cjdb data model is designed to store CityJSONL files in a Postgres database.
-
-## Table of Contents
-### [1. Overview](#overview)
-
-### [2. Table Structure](#table_structure)
- - [import_meta](#import_meta)
- - [cj_object](#cj_object)
- - [Family](#family)
 
-### [3. Indexing](#Indexing)
-
- 
-## 1. Overview <a name="overview"></a>
+# cjdb data model
+cjdb data model is designed to store 3D city models in CityJSON in a PostgreSQL/PostGIS database.
 
-After reading the readme, the user will:
 
-1) Understand the table structure of cjdb model.
+## The data model used 
 
-2) Understand the indexing possiblities within the database, and their effects on operations.
+The conceptual data model contains two main tables. The **cj_metadata** table for storing imported files' information, e.g. name or metadata of the source file. The **city_object** table for storing city objects. 
 
-## 2. Table Structure <a name="table_structure"></a>
+The physical data model adds one more table on the conceptual data model: the **city_object_relationships** table to store relations between city objects, e.g the parent-children relationship. This table is added to achieve higher querying speed when selecting objects by their parent/child relationship. Example of this would be: "give me all the objects which are children of X". 
 
-The conceptual data model contains two main tables. The **import_meta** table for storing imported files' information, e.g. name or metadata of the source file. The **cj_object** table for storing city objects. 
+![UML drawio](uml.png)
 
-![UML drawio](https://user-images.githubusercontent.com/92783160/200633172-e33fc6ae-26b4-4b16-a2a7-968cc9a34d5e.png)
 
+### cj_metadata 
 
-The physical data model adds one more table on the conceptual data model: the **family** table to store relations between city objects, e.g the parent-children relationship. This table is added to achieve higher querying speed when selecting objects by their parent/child relationship. Example of this would be: "give me all the objects which are children of X". 
+The `cj_metadata` table stores information from imported files, e.g. name or metadata of the source file. 
 
+ - **id**: cj_metadata record's index within the database.
+ - **version**: CityJSON version used.
+ - **source_file**: name of the source file.
+ - **metadata**: [CityJSON metadata object](https://www.cityjson.org/specs/#metadata), a JSON object describing the creator, dataset extent or coordinate reference system used, etc.
+ - **transform**: [CityJSON transform object](https://www.cityjson.org/specs/#transform-object), a JSON object describing how to decompress the integer coordinates of the geometries to obtain real-world coordinates.
+ - **srid**: Coordinate reference system (CRS) of the imported city objects in the database. If not specified when importing, the CRS will be the same with the source file's CRS. If specified when importing, the CRS will be the specified CRS.
+ - **extensions**: [CityJSON Extensions](https://www.cityjson.org/specs/#extensions), a JSON file that documents how the core data model of CityJSON is extended.
+ - **extra_properties**: [extraRootProperties](https://www.cityjson.org/specs/#case-2-adding-new-properties-at-the-root-of-a-document), a JSON object with added new properties at the root of the imported document.
+ - **geometry_templates**: [CityJSON geometry-templates object](https://www.cityjson.org/specs/#geometry-templates), a JSON object containing the templates that can be reused by different City Objects (usually for trees).
+ - **bbox**: bounding box is taken from the `geographicExtent` object from the `metadata` section
+ - **started_at**: importing start time.
+ - **finished_at**: importing finish time. `null` if not finished.
 
-![Physical Model drawio (3)](https://user-images.githubusercontent.com/92783160/200633220-92f95184-edce-44b9-bfa9-7db5fccbfc0e.png)
 
 
-### 1. import_meta <a name="import_meta"></a>
+### city_object 
 
-The import_meta table stores information from imported files, e.g. name or metadata of the source file. Belowing section describes its attributes.
+The `city_object` model stores individual city objects, for instance buildings, roads, or bridges. Its attributes are described below. 
+The **attributes** and **geometry** are seperated into two jsonb column for query optimization purpose.
 
-<**id**: import_meta record's index within the database.<br/>
-**source_file**: name of the source file.<br/>
-**version**: cityJSON version used.<br/>
-**metadata**: [cityJSON metadata object](https://www.cityjson.org/specs/#metadata), a JSON object describing the creator, dataset extent or coordinate reference system used, etc.<br/>
-**transform**:[cityJSON transform object](https://www.cityjson.org/specs/#transform-object), a JSON object describing how to decompress the integer coordinates of the geometries to obtain real-world coordinates.<br/>
-**geometry_templates**: [cityJSON geometry-templates object](https://www.cityjson.org/specs/#geometry-templates), a JSON object containing the templates that can be reused by different City Objects (usually for trees).<br/>
-**srid**: Coordinate reference system (CRS) of the imported city objects in the database. If not specified when importing, the CRS will be the same with the source file's CRS. If specified when importing, the CRS will be the specified CRS.<br/>
-**extensions**: [cityJSON Extensions](https://www.cityjson.org/specs/#extensions), a JSON file that documents how the core data model of CityJSON is extended.<br/>
-**extra_properties**: [extraRootProperties](https://www.cityjson.org/specs/#case-2-adding-new-properties-at-the-root-of-a-document), a JSON object with added new properties at the root of the imported document.<br/>
-**started_at**: importing start time.<br/>
-**finished_at**: importing finish time. `null` if not finished.<br/>
-**Bounding box**: bounding box is taken from the `geographicExtent` object from the `metadata` section
+  - **id**: city object's index within the database.
+  - **cj_metadata_id**: the source file id of the city object, foriegn key to the id column of metadata table.
+  - **type**: type of the city object (e.g. building, buildingparts, etc.).
+  - **object_id**: the identification string of the city object (e.g. NL.IMBAG.Pand.0503100000000033-0).
+  - **cj_metadata_id**: the source file id of the city object, foriegn key to the id column of metadata table.
+  - **attributes**: [cityJSON attributes](https://www.cityjson.org/specs/#attributes-for-all-city-objects), a JSON object that describes attributes of the city object (e.g. roof type, area, etc.).
+  - **geometry**: [cityJSON geometry](https://www.cityjson.org/specs/#geometry-objects), a JSON object that describes the geometry of the city object.
+  - **ground_geometry**: the 2D footprint of the city object, in PostGIS geometry type.
 
-### 2. cj_object <a name="cj_object"></a>
 
-The cj_object model stores individual city objects, for instance buildings, roads, or bridges. Its attributes are described below. The **attributes** and **geometry** are seperated into two jsonb column for query optimization purpose.
+### city_object_relationships
 
-**id**: city object's index within the database.<br/>
-**import_meta_id**: the source file id of the city object, foriegn key to the id column of import_meta table.<br/>
-**object_id**: the identification string of the city object (e.g. NL.IMBAG.Pand.0503100000000033-0).<br/>
-**type**: type of the city object (e.g. building, buildingparts, etc.).<br/>
-**attributes**:[cityJSON attributes](https://www.cityjson.org/specs/#attributes-for-all-city-objects), a JSON object that describes attributes of the city object (e.g. roof type, area, etc.).<br/>
-**geometry**: [cityJSON geometry](https://www.cityjson.org/specs/#geometry-objects), a JSON object that describes the geometry of the city object.<br/>
-**ground_geometry**: ground geometry of the city object, in geometry type.<br/>
+The `city_object_relationships` model stores the relations between city objects.
 
-### 3. Family <a name="family"></a>
-The family model stores the relations between city objects.
+  - **id**: city_object_relationships index within the database.
+  - **parent_id**: the id of the parent object.
+  - **child_id**: the id of the child object.
 
-**id**: family object's index within the database.<br/>
-**parent_id**: the identification id of the parent object.<br/>
-**child_id**: the identification id of the child object.<br/>
 
-## 3. Indexing
+## Indexing
 
 Indexing certain columns or [expressions](https://www.postgresql.org/docs/current/indexes-expressional.html) speeds up querying on them. 
 
 The users can use GIN index on lod, to speed up queries on geometries:
 
-CREATE INDEX lod ON cjdb.cj_object USING GIN (geometry jsonb_path_ops);
+```sql
+CREATE INDEX lod ON cjdb.city_object USING GIN (geometry jsonb_path_ops);
+```
 
-The users can use B-tree partial index on attributes. It will slightly increase the query speed.
+The users can use B-tree partial index on attributes, these will slightly increase the query speed.
```

### Comparing `cjdb-1.2.0/cjdb/model/sqlalchemy_models/__init__.py` & `cjdb-2.0.0/cjdb/model/sqlalchemy_models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,78 @@
-import sys
-
 from geoalchemy2 import Geometry
 from sqlalchemy import (Column, ForeignKey, Integer, String, UniqueConstraint,
                         func)
 from sqlalchemy.dialects.postgresql import JSONB, TIMESTAMP
 from sqlalchemy.orm import declarative_base, relationship
 
-from cjdb.logger import logger
 
 Base = declarative_base()
 
 
 class BaseModel(Base):
     __abstract__ = True
     id = Column(Integer, primary_key=True)
 
 
 def NullableJSONB():
     return JSONB(none_as_null=True)
 
 
-class ImportMetaModel(BaseModel):
-    __tablename__ = "import_meta"
+class CjMetadataModel(BaseModel):
+    __tablename__ = "cj_metadata"
     __table_args__ = {"schema": "cjdb"}
     source_file = Column(String)
     version = Column(String(10), nullable=False)
     meta = Column(JSONB, name="metadata")
     transform = Column(NullableJSONB())
     geometry_templates = Column(NullableJSONB())
     srid = Column(Integer)
     extensions = Column(NullableJSONB())
     extra_properties = Column(NullableJSONB())
     started_at = Column(TIMESTAMP, default=func.now())
     finished_at = Column(TIMESTAMP)
     bbox = Column(Geometry("Polygon"))
-
-    def compare_existing(self, session, ignore_repeated_file, update_existing):
-        result_ok = True
-
-        # check if the file was already imported
-        if self.source_file.lower() != "stdin" and \
-           not ignore_repeated_file and \
-           not update_existing:
+    objects = relationship("CjObjectModel",
+                           backref='cj_metadata',
+                           passive_deletes=True)
+
+    def get_already_imported_files(self, session):
+        # query already imported files,
+        # return false if stdin.
+        if self.source_file.lower() != "stdin":
             same_source_import = (
-                session.query(ImportMetaModel)
+                session.query(CjMetadataModel)
                 .filter_by(source_file=self.source_file)
-                .filter(ImportMetaModel.finished_at.isnot(None))
-                .order_by(ImportMetaModel.finished_at.desc())
-                .first()
+                .filter(CjMetadataModel.finished_at.isnot(None))
             )
-            if same_source_import:
-                logger.warning(
-                    "File %s was previously imported at %s. "
-                    "Use the -g flag to suppress this warning.",
-                    self.source_file,  same_source_import.finished_at
-                )
-
-                user_answer = input(
-                    "Should the import continue? "
-                    "Already imported City Objects will be skipped. "
-                    "If you want to update them instead "
-                    "use the flag --update-existing. \n"
-                    " [y / n]\n"
-                )
-                if user_answer.lower() != "y":
-                    logger.info("Import process terminated by user.")
-                    sys.exit(1)
-
-        # check if the CRS is consistent with other imports
-        different_srid_meta = (
-            session.query(ImportMetaModel)
-            .filter(ImportMetaModel.srid != self.srid)
-            .filter(ImportMetaModel.finished_at.isnot(None))
-            .order_by(ImportMetaModel.finished_at.desc())
-            .first()
-        )
 
-        if different_srid_meta:
-            logger.error("Inconsistent Coordinate Reference Systems detected."
-                         "\nCurrently imported SRID: %s \n"
-                         "Recently imported SRID: %s "
-                         "\nUse the '-I/--srid' flag to reproject everything "
-                         "to a single specified CRS or modify source data.",
-                         self.srid, different_srid_meta.srid
-                         )
-            return False
+            return same_source_import
+        return False
 
-        return result_ok
+    def different_srid_meta(self, session):
+        """Check if the CRS is consistent with previous imports."""
+        return (
+            session.query(CjMetadataModel)
+            .filter(CjMetadataModel.srid != self.srid)
+            .filter(CjMetadataModel.finished_at.isnot(None))
+            .order_by(CjMetadataModel.finished_at.desc())
+            .first()
+        )
 
 
 class CjObjectModel(BaseModel):
-    __tablename__ = "cj_object"
+    __tablename__ = "city_object"
     __table_args__ = {"schema": "cjdb"}
-    import_meta_id = Column(Integer, ForeignKey(ImportMetaModel.id))
-    object_id = Column(String, nullable=False, unique=True)
+    cj_metadata_id = Column(Integer, ForeignKey(CjMetadataModel.id, ondelete='CASCADE'))
+    object_id = Column(String, nullable=False)
     type = Column(String, nullable=False)
     attributes = Column(NullableJSONB())
     geometry = Column(NullableJSONB())
     ground_geometry = Column(Geometry("MultiPolygon"))
-    import_meta = relationship(ImportMetaModel)
+    metadata_id_object_id_unique = UniqueConstraint(cj_metadata_id, object_id)
 
     @classmethod
     def get_attributes_and_types(cls, session):
         # sample attributes for each object type
         # this is needed to create proper indexes and also
         # to use those indexes when querying
         sampled_objects = (
@@ -121,20 +91,30 @@
         if sampled_objects:
             for cj_obj in sampled_objects:
                 for attr_name, value in cj_obj.attributes.items():
                     type_mapping[attr_name] = type(value)
 
         return type_mapping
 
+    @classmethod
+    def get_max_id(cls, session) -> int:
+        max = session.query(func.max(cls.id)).scalar()
+        if max:
+            return max
+        else:
+            return 0
+
 
-class FamilyModel(BaseModel):
-    __tablename__ = "family"
+class CityObjectRelationshipModel(BaseModel):
+    __tablename__ = "city_object_relationships"
     __table_args__ = {"schema": "cjdb"}
-    parent_id = Column(String, ForeignKey(CjObjectModel.object_id))
-    child_id = Column(String, ForeignKey(CjObjectModel.object_id))
+    parent_id = Column(Integer, ForeignKey(CjObjectModel.id,
+                                           ondelete='CASCADE'))
+    child_id = Column(Integer, ForeignKey(CjObjectModel.id,
+                                          ondelete='CASCADE'))
 
     parent = relationship(CjObjectModel,
                           foreign_keys=[parent_id],
                           post_update=True)
     child = relationship(CjObjectModel,
                          foreign_keys=[child_id],
                          post_update=True)
```

### Comparing `cjdb-1.2.0/cjdb/modules/checks.py` & `cjdb-2.0.0/cjdb/modules/checks.py`

 * *Files identical despite different names*

### Comparing `cjdb-1.2.0/cjdb/modules/extensions.py` & `cjdb-2.0.0/cjdb/modules/extensions.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,39 +18,44 @@
     def get_extensions(self, extensions):
         for ext_name, content in extensions.items():
             url = content.get("url")
             if url:
                 try:
                     resp = requests.get(url, timeout=10)
                 except Exception as e:
+                    logger.error(e)
                     resp = None
 
                 if resp and resp.status_code == 200:
                     try:
                         ext_definition = json.loads(resp.text)
                         self.full_definitions[ext_name] = ext_definition
                     except ValueError as e:
                         logger.error(
                             "Extension url: %s did not provide a correct json"
-                            " schema", url
+                            " schema: %s", url, e
                         )
                         # raise
                         # throw this exception or ignore it?
                         return
-
-                    for prop_name in ext_definition["extraRootProperties"]:
-                        self.extra_root_properties.append(prop_name)
+                    if "extraRootProperties" not in ext_definition.keys():
+                        print(ext_definition.keys())
+                    else:
+                        for prop_name in ext_definition["extraRootProperties"]:
+                            self.extra_root_properties.append(prop_name)
 
                     for obj_type, extra_attributes in ext_definition[
                         "extraAttributes"
                     ].items():
                         if obj_type not in self.extra_attributes:
                             self.extra_attributes[obj_type] = []
                         for attr_name in extra_attributes:
                             self.extra_attributes[obj_type].append(attr_name)
 
                     for obj_type in ext_definition["extraCityObjects"]:
                         self.extra_city_objects.append(obj_type)
                 else:
-                    msg = f"Extension url: {url} did not return a correct response"
+                    msg = (f"""Extension url: {url} did not return a """
+                           """correct response""")
+                    logger.error(msg)
                     # raise Exception(msg)
                     return
```

### Comparing `cjdb-1.2.0/cjdb/modules/geometric.py` & `cjdb-2.0.0/cjdb/modules/geometric.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import copy
+from statistics import mean
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
+from cjio.geom_help import get_normal_newell
 from pyproj import CRS, Transformer
+from shapely import force_2d
 from shapely.geometry import MultiPolygon, Point, Polygon
-from shapely.validation import explain_validity
+from shapely.ops import unary_union
 
 from cjdb.logger import logger
+from cjdb.modules.exceptions import InvalidLodException
 
 
 # get srid from a CRS string definition
 def get_srid(crs):
     if crs:
         proj = CRS.from_string(crs)
         srid = proj.to_epsg()
@@ -123,85 +128,132 @@
         else:
             # resolve without geometry template
             resolve(lod_level, vertices)
 
     return geometry
 
 
-def get_ground_geometry(geometry, obj_id):
-    # returns a shapely multipolygon (see shapely.geometry.MultiPolygon)
-    # the MultiPolygon should be a 2D geometry (Z coordinate is omitted)
-    # this geometry should be obtained by parsing the "geometry" object
-    # from cityjson -> the argument of this function
-    # the geometry is a multipolygon of all the ground
-    # surfaces in the lowest available LOD
-
-    planes = dict()
-    z_min = 0
-    for boundary in geometry[0]["boundaries"]:
-        for i, shell in enumerate(boundary):
-            if type(shell[0]) is list:
-                if type(shell[0][0]) is list:
-                    for ring in shell:
-                        Point_list = []
-                        z_tot = 0
-                        z_count = 0
-                        for x, y, z in ring:
-                            z_tot = z + z_tot
-                            z_count = z_count + 1
-                            p = Point(x, y, z)
-                            Point_list.append(p)
-                        z_avg = round(z_tot / z_count, 6)
-                        z_min = z_avg
-                        planes[str(z_avg)] = Point_list
-                else:
-                    Point_list = []
-                    z_tot = 0
-                    z_count = 0
-                    for x, y, z in shell:
-                        z_tot = z + z_tot
-                        z_count = z_count + 1
-                        p = Point(x, y, z)
-                        Point_list.append(p)
-                    z_avg = round(z_tot / z_count, 6)
-                    z_min = z_avg
-                    planes[str(z_avg)] = Point_list
-
-    for key in planes:
-        z_num = float(key)
-        if z_num < z_min:
-            z_min = z_num
-
-    ground_points = []
-    ground_points_dic = {}
-
-    for key in planes:
-        if abs(float(key) - z_min) < 0.3:
-            for p in planes[key]:
-                str_p = str(p.x) + " " + str(p.y)
-                if (str_p in ground_points_dic.keys()) is False:
-                    ground_points_dic[str_p] = 0
-
-    for key in ground_points_dic:
-        p_x = key.split()[0]
-        p_y = key.split()[1]
-        p = Point(float(p_x), float(p_y))
-        ground_points.append(p)
+def get_geometry_with_minimum_lod(
+    geometries: List[Dict[str, Any]]
+) -> Optional[Dict[str, Any]]:
+    """Receives a list of Geometry objects and returns
+    the geometry with the minimum LoD."""
+    if len(geometries) == 0:
+        return None
+    elif len(geometries) == 1:
+        return geometries[0]
+    else:
+        try:
+            lods = [float(geom["lod"]) for geom in geometries]
+        except ValueError:
+            raise InvalidLodException()
+        index_of_min = lods.index(min(lods))
+        return geometries[index_of_min]
+
+
+def get_flattened_polygons_from_boundaries(
+    boundaries: List, polygons: Optional[List] = None
+) -> List[Union[Polygon, MultiPolygon]]:
+    if polygons is None:
+        polygons = []
+    if (
+        isinstance(boundaries[0], list)
+        and len(boundaries[0]) == 3
+        and all(isinstance(p, float) for p in boundaries[0])
+    ):
+        surface_points = []
+        for point in boundaries:
+            surface_points.append(Point(point[0], point[1], point[2]))
+        polygons.append(Polygon(surface_points))
+        return polygons
+    else:
+        for shell in boundaries:
+            polygons = get_flattened_polygons_from_boundaries(
+                shell,
+                polygons=polygons)
+        return polygons
+
+
+def is_surface_vertical(normal: np.ndarray) -> bool:
+    """
+    Given the surface normal as input, if it is (almost)
+    perpendicular to the "ground" (xy) normal (0,0,1) then
+    the surface can be considered vertical and the function
+    will return True, otherwise False.
+    We check if the vectors are perpendicular to each other
+    by calculating their dot product. If the dot product is
+    close to 0 then the vectors are perpendicular.
+    """
+    dot_prd = 0 * normal[0] \
+        + 0 * normal[1] \
+        + 1 * normal[2]
+
+    if abs(dot_prd) < 0.1:
+        return True
+    else:
+        return False
+
+
+def get_ground_surfaces(polygons: List[Polygon]) -> List[Polygon]:
+    ground_surfaces = {}
+    for polygon in polygons:
+        xyz = np.asarray(polygon.exterior.coords)[0:-1]
+        normal, is_coplanar = get_normal_newell(xyz)
+        if is_surface_vertical(normal):
+            continue
+        else:
+            z = mean([point[2] for point in polygon.exterior.coords])
+            ground_surfaces[z] = force_2d(polygon)
+    if len(ground_surfaces) == 0:
+        raise Exception(polygons)
+    z_mean = mean(ground_surfaces.keys())
+    return [v for k, v in ground_surfaces.items() if k < z_mean]
 
-    if len(ground_points) >= 3:
-        ground_polygon = Polygon([[p.x, p.y] for p in ground_points])
+
+def merge_into_a_multipolygon(ground_surfaces:
+                              List[Union[Polygon, MultiPolygon]]
+                              ) -> MultiPolygon:
+    polygon = unary_union(force_2d(ground_surfaces))
+    if isinstance(polygon, MultiPolygon):
+        return polygon
     else:
+        return MultiPolygon([polygon])
+
+
+def get_ground_geometry(
+    geometries: List[Dict[str, Any]], obj_id: str
+) -> MultiPolygon:
+    """ Receives a list of transformed boundary coordinates
+    of the city object
+    and extracts only the ground surface.
+    If there is an LoD 0, then all the available surfaces
+    are merged and returned.
+    If not, then only the non-vertical surfaces with the lowest
+    height are merged and returned.
+    """
+    geometry = get_geometry_with_minimum_lod(geometries)
+
+    if geometry is None:
+        logger.warning(f"No geometry for object ID=({obj_id}) ")
+        return None
+
+    if geometry["type"] == "MultiPoint" or\
+       geometry["type"] == "MultiLineString":
         logger.warning(
-            f"Ground geometry for object ID=({obj_id}) could not be"
-            " calculated."
+            f"""MultiPoint or MultiLineString type has no ground geometry,
+            object ID=({obj_id})"""
         )
+        # TODO return convex hull of the points as ground geometry.
         return None
 
-    if ground_polygon.is_valid is False:
-        ground_polygon = ground_polygon.buffer(0)
-        if ground_polygon.is_valid is False:
-            logger.info(explain_validity(ground_polygon))
-
-    if type(ground_polygon) is Polygon:
-        ground_polygon = MultiPolygon([ground_polygon])
-
-    return ground_polygon
+    if float(geometry["lod"]) < 1:
+        flattented_polygons = get_flattened_polygons_from_boundaries(
+            geometry["boundaries"]
+        )
+        return merge_into_a_multipolygon(flattented_polygons)
+    else:
+        # TODO: check if there are surface types available
+        # to choose the ground surfaces
+        surfaces = get_flattened_polygons_from_boundaries(
+            geometry["boundaries"])
+        ground_surfaces = get_ground_surfaces(surfaces)
+        return merge_into_a_multipolygon(ground_surfaces)
```

### Comparing `cjdb-1.2.0/cjdb/modules/importer.py` & `cjdb-2.0.0/cjdb/modules/importer.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,95 +5,99 @@
 from typing import Optional, Tuple
 
 from shapely.geometry.base import BaseGeometry
 from sqlalchemy import func, text
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.orm import Session
 
+import cjdb.modules.exceptions as exceptions
 from cjdb.logger import logger
-from cjdb.model.sqlalchemy_models import (BaseModel, CjObjectModel,
-                                          FamilyModel, ImportMetaModel)
-from cjdb.modules.checks import (check_object_type, check_reprojection,
+from cjdb.model.sqlalchemy_models import (BaseModel,
+                                          CityObjectRelationshipModel,
+                                          CjMetadataModel, CjObjectModel)
+from cjdb.modules.checks import (check_object_type,
                                  check_root_properties)
-from cjdb.modules.exceptions import (InvalidCityJSONObjectException,
-                                     InvalidMetadataException)
 from cjdb.modules.extensions import ExtensionHandler
 from cjdb.modules.geometric import (get_ground_geometry, get_srid,
                                     reproject_vertex_list,
                                     resolve_geometry_vertices,
                                     transform_vertex)
-from cjdb.modules.utils import (find_extra_properties, get_cj_object_types,
-                                is_cityjson_object, to_dict)
+from cjdb.modules.utils import (find_extra_properties, get_city_object_types,
+                                is_cityjson_object, is_valid_file, to_dict)
 
 
 # class to store variables per file import - for clarity
 class SingleFileImport:
     def __init__(self, file="stdin"):
         self.file = file
-        self.target_srid = None
-        self.import_meta = None  # meta read from the file
         self.source_srid = None
+        self.cj_metadata = None  # meta read from the file
+        self.target_srid = None
         self.extension_handler = (
             None  # data about extensions - extra properties, root attributes
         )
-        self.cj_objects = []
+        self.city_objects = []
         self.families = []
 
 
 # importer class called once per whole import
 class Importer:
-    def __init__(self, engine, args):
+    def __init__(self, engine, filepath, db_schema, input_srid,
+                 indexed_attributes, partial_indexed_attributes,
+                 ignore_repeated_file, overwrite, transform):
         self.engine = engine
-        self.args = args
+        self.filepath = filepath
+        self.db_schema = db_schema
+        self.input_srid = input_srid
+        self.indexed_attributes = indexed_attributes
+        self.partial_indexed_attributes = partial_indexed_attributes
+        self.ignore_repeated_file = ignore_repeated_file
+        self.overwrite = overwrite
+        self.max_id = 0
+        self.processed = dict()
+        self.transform = transform
+
         # get allowed types for validation
-        self.cj_object_types = get_cj_object_types()
+        self.city_object_types = get_city_object_types()
         self.current = SingleFileImport()
 
         for table in BaseModel.metadata.tables.values():
-            table.schema = self.args.db_schema
+            table.schema = self.db_schema
 
     def __enter__(self):
         self.session = Session(self.engine)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.session.close()
 
     def run_import(self) -> None:
-        # create model if in create mode, else append data
-        if not self.args.append_mode:
-            self.prepare_database()
+        self.prepare_database()
+        self.max_id = CjObjectModel.get_max_id(self.session)
         self.parse_cityjson()
         self.session.commit()
         # post import operations like clustering, indexing...
-        if not self.args.append_mode:
-            self.post_import()
-        self.current.import_meta.finished_at = func.now()
+        self.post_import()
         self.session.commit()
-        logger.info(f"Imported from {self.args.filepath} successfully")
 
     def prepare_database(self) -> None:
         """Adds the postgis extension and creates
         the schema and the tables."""
         with self.engine.connect() as conn:
             conn.execute(text("""CREATE EXTENSION IF NOT EXISTS postgis"""))
-            if self.args.overwrite:
-                conn.execute(text(f"""DROP SCHEMA
-                             IF EXISTS {self.args.db_schema}
-                             CASCADE"""))
             conn.execute(text(f"""CREATE SCHEMA IF NOT EXISTS
-                                  {self.args.db_schema}"""))
+                                  {self.db_schema}"""))
             conn.commit()
         # create all tables defined as SqlAlchemy models
         for table in BaseModel.metadata.tables.values():
             table.create(self.engine, checkfirst=True)
 
     def parse_cityjson(self) -> None:
         """Parses the input path."""
-        source_path = self.args.filepath
+        source_path = self.filepath
 
         if os.path.isfile(source_path) or source_path.lower() == "stdin":
             self.process_file(source_path)
 
         elif os.path.isdir(source_path):
             self.process_directory(source_path)
 
@@ -104,51 +108,92 @@
         """Perform post import operation on the schema,
            like clustering and indexing"""
 
         cur_path = Path(__file__).parent
         sql_path = os.path.join(cur_path.parent, "resources/post_import.sql")
 
         with open(sql_path) as f:
-            cmd = f.read().format(schema=self.args.db_schema)
+            cmd = f.read().format(schema=self.db_schema)
         with self.engine.connect() as conn:
             conn.execute(text(cmd))
         self.index_attributes()
 
-    def extract_import_metadata(self, line_json):
-        if "metadata" not in line_json:
-            raise InvalidMetadataException("The file should contain a member"
-                                           "'metadata', in the first object")
+    def set_target_srid(self) -> None:
+        """
+        This function sets the  target SRID for the file being imported,
+        i.e. the SRID for the geometries to be transformed to.
+        If the flag --transform is used then the geometries should
+        be transformed from the source SRID to the SRID of the existing
+        schema and the target SRID is set to the SRID of the schema.
+        If no --transform flag is used then the geometries do not need to
+        be transformed and the target SRID is set to the source SRID.
+        """
+        if not self.transform:
+            self.current.target_srid = self.current.source_srid
+        else:
+            schema_srid = (self.session.query(CjMetadataModel)
+                           .filter(CjMetadataModel.finished_at.isnot(None))
+                           .order_by(CjMetadataModel.finished_at.desc())
+                           .first()
+                           )
+            if schema_srid:
+                self.current.target_srid = schema_srid.srid
+            else:
+                raise exceptions.NoSchemaSridException()
+        logger.debug("Target SRID: %s", self.current.target_srid)
 
-        extra_root_properties = find_extra_properties(line_json)
+    def set_source_srid(self, line_json) -> None:
+        """
+        This function sets the SRID of the file being imported.
+        Usually the SRID of the file is defined in the "referenceSystem"
+        member of the json's metadata. If the file does have such member,
+        the user can use the flag -I/--srid to set the SRID of the file.
+        If both metadata-defined and user-defined SRIDs exist then the
+        user-defined SRID overwrites the metadata-SRID.
+        """
         self.current.source_srid = get_srid(
             line_json["metadata"].get("referenceSystem")
         )
-        if not self.current.source_srid:
-            logger.warning("No Coordinate Reference System"
-                           " specified for the dataset.")
-
-        # use specified target SRID for all the geometries
-        # If not specified use same as source.
-        if self.args.target_srid and self.current.source_srid:
-            self.current.target_srid = self.args.target_srid
-            check_reprojection(self.current.source_srid,
-                               self.current.target_srid)
-        elif self.args.target_srid:
-            self.current.target_srid = self.args.target_srid
+
+        if self.input_srid:
+            if self.current.source_srid:
+                logger.warning("""Input SRID is different than the SRID in the 
+                                file's metadata:
+                                Input SRID: %s
+                                Source SRID: %s
+                                Source SRID will be overwritten.""",
+                               self.input_srid,
+                               self.current.source_srid)
+
+            self.current.source_srid = self.input_srid
         else:
-            self.current.target_srid = self.current.source_srid
+            if not self.current.source_srid:
+                raise exceptions.MissingCRSException()
+
+        logger.debug("SRID of input file: %s", self.current.source_srid)
+
+    def extract_cj_metadatadata(self, line_json):
+        if "metadata" not in line_json:
+            raise exceptions.InvalidMetadataException(
+                "The file should contain a member"
+                "'metadata', in the first object")
+
+        extra_root_properties = find_extra_properties(line_json)
+
+        self.set_source_srid(line_json)
+        self.set_target_srid()
 
         # calculate dataset bbox based on geographicalExtent
         bbox = None
         if "geographicalExtent" in line_json["metadata"]:
             bbox_coords = line_json["metadata"]["geographicalExtent"]
             bbox_vertices = [bbox_coords[:3], bbox_coords[3:]]
 
             if (
-                self.current.source_srid
+                self.current.target_srid
                 and self.current.target_srid != self.current.source_srid
             ):
                 bbox_vertices = reproject_vertex_list(
                     bbox_vertices,
                     self.current.source_srid,
                     self.current.target_srid,
                 )
@@ -176,178 +221,206 @@
         # the extension defined extra properties
         check_root_properties(
             extra_root_properties,
             self.current.extension_handler.extra_root_properties,
         )
 
         # "or None" is added to change empty json "{}" to database null
-        import_meta = ImportMetaModel(
+        cj_metadata = CjMetadataModel(
             source_file=os.path.basename(self.current.file),
             version=line_json["version"],
             meta=line_json.get("metadata") or None,
             transform=line_json.get("transform") or None,
             geometry_templates=line_json.get("geometry-templates") or None,
             srid=self.current.target_srid,
             extensions=line_json.get("extensions") or None,
             extra_properties=extra_properties_obj or None,
             bbox=bbox,
         )
 
-        # compare to existing import metas
-        # for example to detect inconsistent CRS from different files
-        result_ok = import_meta.compare_existing(
-            self.session,
-            self.args.ignore_repeated_file,
-            self.args.update_existing
-        )
-        if not result_ok:
-            raise InvalidMetadataException()
+        if cj_metadata.source_file.lower() != "stdin":
+            # compare to existing import metas
+            imported_files = cj_metadata.get_already_imported_files(
+                self.session
+            )
+
+            if (
+                self.ignore_repeated_file and
+                    imported_files.first() and 
+                    not self.overwrite):
+                logger.warning("File already imported. Skipping...")
+                return False
+            elif imported_files.first() and not self.overwrite:
+                logger.warning(
+                    "A file with the same name (%s) was previously "
+                    "imported on %s. Use the --ignore-repeated-file "
+                    "to skip already imported files.",
+                    cj_metadata.source_file, imported_files.first().finished_at
+                )
+                user_answer = input(
+                    "Should the import continue? "
+                    "Already imported city objects will be skipped. "
+                    "If you want to overwrite them instead "
+                    "use the flag --overwrite. \n"
+                    " [y / n]\n"
+                )
+                if user_answer.lower() != "y":
+                    logger.warning(
+                        f"Import of file {cj_metadata.source_file}"
+                        "skipped by user.")
+                    return False
+            elif imported_files.first() and self.overwrite:
+                logger.warning(
+                    "File already imported. Overwriting all objects"
+                    f" from source file {cj_metadata.source_file}")
+                imported_files.delete()
+
+        different_srid = cj_metadata.different_srid_meta(self.session)
+        if different_srid:
+            logger.error("Not matching coordinate Reference Systems"
+                         "\nCurrently imported SRID: %s"
+                         "\nRecently imported SRID: %s",
+                         cj_metadata.srid, different_srid.srid)
+            raise exceptions.InconsistentCRSException()
 
         # add metadata to the database
-        import_meta.__table__.schema = self.args.db_schema
-        self.current.import_meta = import_meta
-        self.session.add(import_meta)
+        cj_metadata.__table__.schema = self.db_schema
+        self.current.cj_metadata = cj_metadata
+        self.session.add(cj_metadata)
         self.session.commit()
+        return True
 
     def process_line(self, line_json) -> None:
         # unpack vertices for the cityobjects based on
         # the CityJSON transform
         # this is done once for the CityJSONFeature
         vertices = [
-            transform_vertex(v, self.current.import_meta.transform)
+            transform_vertex(v, self.current.cj_metadata.transform)
             for v in line_json["vertices"]
         ]
 
         # reproject if needed
         source_target_srid = None
         if (
-            self.current.source_srid
-            and self.current.target_srid != self.current.source_srid
+            self.current.target_srid != self.current.source_srid
         ):
             source_target_srid = (
                 self.current.source_srid,
                 self.current.target_srid,
             )
             vertices = reproject_vertex_list(vertices, *source_target_srid)
 
         # list of relationships for the CityJSONFeature
-        family_ties = []
+        city_object_relationships_ties = []
         # objects for the CityJSONFeature
         cj_feature_objects = {}
 
         # create CityJSONObjects
         for obj_id, cityobj in line_json["CityObjects"].items():
-            obj_to_update = None
-
-            # optionally check if the object exists -
-            # to skip it or update it
-            if self.args.update_existing:
-                existing = (
-                    self.session.query(CjObjectModel)
-                    .filter_by(object_id=obj_id)
-                    .first()
-                )
-
-                if existing:
-                    logger.warning(f"CityObject (id:{obj_id}) already exists. Updating.")  # noqa
-                    obj_to_update = existing
 
             # get 3D geom, ground geom and bbox
             geometry, ground_geometry = self.get_geometries(
                 obj_id, cityobj, vertices, source_target_srid
             )
 
             # check if the object type is allowed by the official
             # spec or extension
             check_result, message = check_object_type(
                 cityobj.get("type"),
-                self.cj_object_types,
+                self.city_object_types,
                 self.current.extension_handler.extra_city_objects,
             )
             if not check_result:
                 logger.info(message)
 
             # update or insert the object
             # 'or None' is added to change empty json "{}" to database null
-            if obj_to_update:
-                cj_object = obj_to_update
-                cj_object.type = cityobj.get("type")
-                cj_object.attributes = cityobj.get("attributes") or None
-                cj_object.geometry = geometry
-                cj_object.ground_geometry = ground_geometry
-                cj_object.import_meta = self.current.import_meta
-            else:
-                cj_object = CjObjectModel(
-                    object_id=obj_id,
-                    type=cityobj.get("type"),
-                    attributes=cityobj.get("attributes") or None,
-                    geometry=geometry,
-                    ground_geometry=ground_geometry,
-                )
 
-                # add CityJson object to the database
-                cj_object.__table__.schema = self.args.db_schema
-                cj_object.import_meta_id = self.current.import_meta.id
-                self.current.cj_objects.append(to_dict(cj_object))
+            city_object_id = self.processed.get(obj_id, None)
+            if not city_object_id:
+                self.max_id = self.max_id + 1
+                self.processed[obj_id] = self.max_id
+                city_object_id = self.max_id
+            city_object = CjObjectModel(
+                id=city_object_id,
+                object_id=obj_id,
+                type=cityobj.get("type"),
+                attributes=cityobj.get("attributes") or None,
+                geometry=geometry,
+                ground_geometry=ground_geometry,
+            )
+
+            # add CityJson object to the database
+            city_object.__table__.schema = self.db_schema
+            city_object.cj_metadata_id = self.current.cj_metadata.id
+            self.current.city_objects.append(to_dict(city_object))
 
-            cj_feature_objects[obj_id] = cj_object
+            cj_feature_objects[obj_id] = city_object
 
             # save children-parent links
             for child_id in cityobj.get("children", []):
-                family_ties.append((obj_id, child_id))
-
-                # delete previous ties if updating object
-                if obj_to_update:
-                    children = self.session.query(FamilyModel).filter_by(
-                        child_id=child_id
-                    )
-                    children.delete()
+                child_unique_id = self.processed.get(child_id, None)
+                if child_unique_id:
+                    city_object_relationships_ties.append((city_object_id,
+                                                           child_unique_id))
+                else:
+                    self.max_id = self.max_id + 1
+                    self.processed[child_id] = self.max_id
+                    city_object_relationships_ties.append((city_object_id,
+                                                           self.max_id))
 
         # create children-parent links after all objects
         # from the CityJSONFeature already exist
-        for parent_id, child_id in family_ties:
+        for parent_id, child_id in city_object_relationships_ties:
             self.current.families.append({"parent_id": parent_id,
                                           "child_id": child_id})
 
-    def process_file(self, filepath) -> None:
+    def process_file(self, filepath) -> bool:
         """Process a single cityJSON file"""
         self.current = SingleFileImport(filepath)
         logger.info("Running import for file: %s", filepath)
 
         if filepath.lower() == "stdin":
             f = sys.stdin
         else:
+            if not is_valid_file(filepath):
+                raise exceptions.InvalidFileException()
             f = open(filepath, "rt")
 
         first_line = f.readline()
         first_line_json = json.loads(first_line.rstrip("\n"))
         if not is_cityjson_object(first_line_json):
-            raise InvalidCityJSONObjectException()
-        self.extract_import_metadata(first_line_json)
+            raise exceptions.InvalidCityJSONObjectException()
+        metadata_ok = self.extract_cj_metadatadata(first_line_json)
+        if not metadata_ok:
+            return False
         for line in f.readlines():
             line_json = json.loads(line.rstrip("\n"))
             self.process_line(line_json)
 
-        if self.current.cj_objects:
+        if self.current.city_objects:
             obj_insert = (
                 insert(CjObjectModel)
-                .values(self.current.cj_objects)
+                .values(self.current.city_objects)
                 .on_conflict_do_nothing()
             )
             self.session.execute(obj_insert)
+        self.session.commit()
 
         if self.current.families:
-            family_insert = (
-                insert(FamilyModel)
+            city_object_relationships_insert = (
+                insert(CityObjectRelationshipModel)
                 .values(self.current.families)
                 .on_conflict_do_nothing()
-            )  # noqa
-            self.session.execute(family_insert)
-        self.current.import_meta.finished_at = func.now()
+            )
+            self.session.execute(city_object_relationships_insert)
+        self.current.cj_metadata.finished_at = func.now()
         self.session.commit()
+        logger.info(f"File {filepath} imported successfully.")
+        return True
 
     def process_directory(self, dir_path) -> None:
         """Process all files in a directory."""
         logger.info("Running import for directory: %s", dir_path)
         ext = ".jsonl"
         for f in os.scandir(dir_path):
             if f.path.endswith(ext):
@@ -364,23 +437,23 @@
 
         # python type mapping for the attributes based on sampled values
         type_mapping = CjObjectModel.get_attributes_and_types(self.session)
 
         # sql index command
         cmd_base = (
             "create index if not exists {table}_{attr_name}_idx "
-            + "on {schema}.{table} using "
-            + "btree(((attributes->>'{attr_name}')::{attr_type}))"
+            "on {schema}.{table} using "
+            "btree(((attributes->>'{attr_name}')::{attr_type}))"
         )
 
         # prepare partial and non partial indexes in one list
         attributes = [
-            (a, True) for a in self.args.partial_indexed_attributes
+            (a, True) for a in self.partial_indexed_attributes
         ] + [  # noqa
-            (a, False) for a in self.args.indexed_attributes
+            (a, False) for a in self.indexed_attributes
         ]
 
         # for each attribute to be indexed
         for attr_name, is_partial in attributes:
             msg = f"Indexing CityObject attribute: '{attr_name}'"
             if is_partial:
                 msg += " with partial index"
@@ -417,21 +490,21 @@
         if "geometry" not in cityobj:
             return None, None
 
         # returned geometry is already in the required projection
         geometry = resolve_geometry_vertices(
             cityobj["geometry"],
             vertices,
-            self.current.import_meta.geometry_templates,
+            self.current.cj_metadata.geometry_templates,
             source_target_srid,
         )
 
         ground_geometry = get_ground_geometry(geometry, obj_id)
 
-        if (ground_geometry is None) is False:
+        if ground_geometry is not None:
             if not self.current.target_srid:
                 ground_geometry = func.st_geomfromtext(ground_geometry.wkt)
             else:
                 ground_geometry = func.st_geomfromtext(
                     ground_geometry.wkt, self.current.target_srid
                 )
```

### Comparing `cjdb-1.2.0/cjdb/modules/utils.py` & `cjdb-2.0.0/cjdb/modules/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from typing import Any, Dict
 
 import psycopg2
-from psycopg2.extras import RealDictCursor
 from sqlalchemy import create_engine
 
 from cjdb.resources import object_types
 
 
-def get_db_engine(args, echo=False):
+def is_valid_file(filepath: str) -> bool:
+    # TODO: this check sounds pretty easy to fulfil 
+    if filepath.endswith('.jsonl'):
+        return True
+    return False
+
+
+def get_db_engine(db_user, db_password, db_host, db_port, db_name, echo=False):
     conn_string = (
-        f"postgresql://{args.db_user}:{args.db_password}"
-        f"@{args.db_host}:{args.db_port}/{args.db_name}"
+        f"postgresql://{db_user}:{db_password}"
+        f"@{db_host}:{db_port}/{db_name}"
     )
-
     engine = create_engine(conn_string, echo=echo)
-
     return engine
 
-
-def open_connection(args):
-    conn = psycopg2.connect(
-        database=args.db_name,
-        host=args.db_host,
-        user=args.db_user,
-        port=args.db_port,
-        cursor_factory=RealDictCursor,
-    )
-
+def get_db_psycopg_conn(db_user, db_password, db_host, db_port, db_name):
+    # conn = psycopg2.connect("dbname=cj_denhaag user=hugo")
+    conn = psycopg2.connect(user=db_user, 
+                            password=db_password, 
+                            host=db_host, 
+                            port=db_port, 
+                            dbname=db_name)
     return conn
 
 
-# todo - this should take available object types from the official spec
-def get_cj_object_types():
+# TODO: this should take available object types from the official spec
+def get_city_object_types():
     types = object_types.types
 
     type_list = []
     for key, val in types.items():
         type_list.append(key)
         if val:
             for v in val:
```

### Comparing `cjdb-1.2.0/cjdb/resources/object_types.py` & `cjdb-2.0.0/cjdb/resources/object_types.py`

 * *Files identical despite different names*

### Comparing `cjdb-1.2.0/cjdb/resources/strings.py` & `cjdb-2.0.0/cjdb/resources/strings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-filepath_help = (
-    "Source a CityJSONL file or a directory with CityJSONL files. "
-    "If a path is not specified, STDIN will be used."
-)
-
 version_help = "Get the current version"
 
+filepath_help = ("Path to a CityJSONL file or a directory with "
+                 "CityJSONL files. If no path is specified, "
+                 "STDIN will be used."
+                 )
+
 host_help = "PostgreSQL database host"
 
 port_help = "PostgreSQL database port"
 
 user_help = "PostgreSQL database user name"
 
 password_help = "PostgreSQL database user password"
 
 database_help = "PostgreSQL database name"
 
-schema_help = "Target database schema"
+schema_help = "PostgreSQL database schema name"
 
 srid_help = (
-    "Target coordinate system SRID. "
-    "All 3D and 2D geometries will be reprojected."
+    "If no SRID is defined in the metadata of the file, "
+    "use this flag to define a SRID for the geometries. "
+    "If an SRID is defined in the metadata, this flag will "
+    "overwrite it."
 )
 
 index_help = (
     "CityObject attribute to be indexed using a btree index. "
     "Can be specified multiple times, for each attribute once."
 )
 
@@ -31,38 +33,29 @@
     "CityObject attribute to be indexed using a btree partial index. "
     "Can be specified multiple times, for each attribute once. "
     "This index indexes on a condition 'where {{ATTR_NAME}} is not null'. "
     "This means that it saves space and improves query performance when the "
     "attribute is not present for all imported CityObjects."
 )
 
-append_help = (
-    "Run in append mode (as opposed to default create mode). "
-    "This assumes the database structure exists already and "
-    "new data is to be appended."
-)
-
-overwrite_help = (
-    "Overwrite the data that is currently in the database schema. "
-    "Warning: this causes the loss of what was imported before "
-    "to the database schema."
-)
-
 ignore_file_help = (
     "Ignore repeated file names warning when importing. "
     "By default, the importer will send out warnings if a specific "
     "file has already been imported."
 )
 
-skip_existing = (
-    "Check if the object with given ID exists before inserting, and "
-    "skip it if it does. "
-    "By default, the importer does not check existence for "
-    "performance reasons, which means that importing the same object "
-    "twice will result in an error."
+overwrite_help = (
+    "If the file has been imported before, delete all "
+    "associated objects with this filename and reimport "
+    "all objects in the file."
+)
+
+transform_help = ("Transform input geometries to the CRS "
+                  "of the existing schema")
+
+output_help = (
+    "Name of the output file. Default name: 'cj_export.city.json' "
 )
 
-update_existing = (
-    "Check if the object with given ID exists before inserting, and "
-    "update it if it does. "
-    "The old object will be updated with the new object's properties."
+query_help = (
+    "SQL query with the ids of the objects to be exported."
 )
```

### Comparing `cjdb-1.2.0/setup.py` & `cjdb-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,210 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cjdb
+Version: 2.0.0
+Summary: CJDB is a tool that enables CityJSON integration with a PostgreSQL database
+Home-page: https://github.com/tudelft3d/cjdb
+License: MIT
+Keywords: CityJSON,PostgreSQL
+Author: Cynthia Cai
+Maintainer: Gina Stavropoulou
+Maintainer-email: g.stavropoulou@tudelft.nl
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cjio (>=0.8.1,<0.9.0)
+Requires-Dist: geoalchemy2 (>=0.13.1,<0.14.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: pyproj (>=3.5.0,<4.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: shapely (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://github.com/tudelft3d/cjdb
+Description-Content-Type: text/markdown
 
-packages = \
-['cjdb',
- 'cjdb.model',
- 'cjdb.model.sqlalchemy_models',
- 'cjdb.modules',
- 'cjdb.resources']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cjio>=0.8.1,<0.9.0',
- 'geoalchemy2>=0.13.1,<0.14.0',
- 'numpy>=1.24.2,<2.0.0',
- 'psycopg2-binary>=2.9.6,<3.0.0',
- 'pyproj>=3.5.0,<4.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'shapely>=2.0.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['cjdb = cjdb.main:main']}
-
-setup_kwargs = {
-    'name': 'cjdb',
-    'version': '1.2.0',
-    'description': 'CJDB is a tool that enables CityJSON integration with a PostgreSQL database',
-    'long_description': '# cjdb\n[![MIT badge](https://img.shields.io/pypi/l/cjdb)](LICENSE) &nbsp; [![PyPI](https://img.shields.io/pypi/v/cjdb)](https://pypi.org/project/cjdb)\n\n`cjdb` is a Python based importer of CityJSONL files to a PostgreSQL database. It requires the [PostGIS](https://postgis.net/) extension.\n\nAuthors: Cynthia Cai, Lan Yan, Yitong Xia, Chris Poon, Siebren Meines, Leon Powalka\n\nMaintainer: Gina Stavropoulou\n\n## Table of Contents  \n### [1.Data model](#1-data-model)\n### [2.Installation](#2-installation)\n- [Using pip](#using-pip)\n- [Using Docker](#using-docker)\n### [3.Usage](#3-usage)\n- [CLI](#cli)\n- [Quickstart](#quickstart)\n- [Basic Queries](#basic-queries)\n### [4.Local development](#4-local-development)\n- [Install and Build](#install-and-build)\n- [Testing](#testing)\n### [5.Explanation](#5-explanation)\n - [Model assumptions](#model-assumptions)\n - [What is a City Model?](#what-is-a-city-model)\n - [Types of input](#types-of-input)\n - [Coordinate Reference Systems](#coordinate-reference-systems)\n - [3D reprojections](#3d-reprojections)\n - [CityJSON Extensions](#cityjson-extensions)\n - [CityJSON GeometryTemplate](#cityjson-geometrytemplate)\n - [Data validation](#data-validation)\n - [Repeated object IDs](#repeated-object-ids)\n---\n## 1. Data model\nFor the underlying data model see [cjdb/model/README.md](cjdb/model/README.md)\n\n\n## 2. Installation\n### Using pip\n```bash\npip install cjdb\n```\nIt is recommended to install it in an isolated environment, because of fragile external library dependencies for CQL filter parsing.\n\n### Using docker\nBuild:\n```bash\ndocker build -t cjdb:latest .\n```\n\nRun:\n```bash\ndocker run --rm -it cjdb cjdb --help\n```\n\nTo import some files, the `-v` option is needed to mount our local file directory in the container:\n```bash\ndocker run -v {MYDIRECTORY}:/data --rm -it --network=host cjdb cjdb -H localhost -U postgres -d postgres -W postgres /data/5870_ext.jsonl \n```\n## 3. Usage <a name="usage"></a>\n\n### CLI <a name="cli"></a>\n\n```bash\ncj2pgsql [-h] [-H DB_HOST] [-p DB_PORT] -U DB_USER [-W DB_PASSWORD] -d DB_NAME [-s DB_SCHEMA] [-I TARGET_SRID][-x INDEXED_ATTRIBUTES] [-px PARTIAL_INDEXED_ATTRIBUTES] [-g] [-a | -o] [-e | -u] [file_or_directory]\n```\n#### Positional Arguments\nfile_or_directory\nSource CityJSONL file or a directory with CityJSONL files. STDIN if not specified. If specifying a directory, all the *.jsonl files inside of it will be imported.\n\nDefault: “stdin”\n\n#### Named Arguments\n`-I, --srid`\nTarget coordinate system SRID. All 3D and 2D geometries will be reprojected.\n\n`-x, --attr-index`\nCityObject attribute to be indexed using a btree index. Can be specified multiple times, for each attribute once.\n\nDefault: []\n\n`-px, --partial-attr-index`\nCityObject attribute to be indexed using a btree partial index. Can be specified multiple times, for each attribute once. This index indexes on a condition ‘where {\n                {ATTR_NAME\n                }\n        } is not null’. This means that it saves space and improves query performance when the attribute is not present for all imported CityObjects.\n\nDefault: []\n\n`-g, --ignore-repeated-file`\nIgnore repeated file names warning when importing. By default, the importer will send out warnings if a specific file has already been imported.\n\nDefault: False\n\n`-a, --append`\nRun in append mode (as opposed to default create mode). This assumes the database structure exists already and new data is to be appended.\n\nDefault: False\n\n`-o, --overwrite`\nOverwrite the data that is currently in the database schema. Warning: this causes the loss of what was imported before to the database schema.\n\nDefault: False\n\n`-u, --update-existing`\nCheck if the object with given ID exists before inserting, and update it if it does. The old object will be updated with the new object’s properties.\n\nDefault: False\n\n#### Database connection arguments\n`-H, --host`\nPostgreSQL database host\n\nDefault: “localhost”\n\n`-p, --port`\nPostgreSQL database port\n\nDefault: 5432\n\n`-U, --user`\nPostgreSQL database user name\n\n`-W, --password`\nPostgreSQL database user password\n\n`-d, --database`\nPostgreSQL database name\n\n`-s, --schema`\nTarget database schema\n\nDefault: “public”\n\n### Quickstart\n\nSample CityJSON data can be downloaded from [3DBAG download service](https://3dbag.nl/nl/download?tid=901). Then, having the CityJSON file, a combination of [cjio](https://github.com/cityjson/cjio) (external CityJSON processing library) and cjdb is needed to import it to a specified schema in a database. \n\n1. Convert CityJSON to CityJSONL\n\n```bash\ncjio --suppress_msg tile_901.json export jsonl tile_901.jsonl \n```\n\n2. Create a new database\n\n  - [how to create a new database](https://postgis.net/workshops/postgis-intro/creating_db.html)\n\n3. Import CityJSONL to the database\n```bash\nPGPASSWORD=postgres cjdb -H localhost -U postgres -d postgres -s cjdb -o tile_901.jsonl   \n```\n\n**Alternatively steps 1 and 2 in a single command:**\n\n```bash\ncjio --suppress_msg tile_901.json export jsonl stdout | cjdb -H localhost -U postgres -d postgres -s cjdb -o\n```\n\nThe metadata and the objects can then be found in the tables in the specified schema (`cjdb` in this example).\n\n\nPassword can be specified in the `PGPASSWORD` environment variable. If not specified, the app will prompt for the password.\n\n\n### Basic Queries\n\n- Query an object with a specific id:\n```SQL\nSELECT * FROM cjdb.cj_object\nWHERE object_id = \'NL.IMBAG.Pand.0503100000000334\';\n```\n\n- Query a building with a specific child\n```SQL\nSELECT o.* FROM cjdb.family f\nINNER JOIN cjdb.cj_object o ON o.object_id = f.parent_id\nWHERE f.child_id = \'NL.IMBAG.Pand.0503100000000334-0\'\n```\n\n- Query all buildings within a bounding box\n```SQL\nSELECT * FROM cjdb.cj_object\nWHERE type = \'Building\'\nAND ST_Contains(ST_MakeEnvelope(81900.00, 446850.00, 81930.00, 446900.00, 7415), ground_geometry)\nORDER BY id ASC;\n```\n\n- Query the building intersecting with a point\n```SQL\nSELECT * FROM cjdb.cj_object\nWHERE ground_geometry && ST_MakePoint(81915.00, 446850.00)\nAND type = \'Building\'\nORDER BY object_id ASC;\n```\n\n- Query all objects with a slanted roof\n```SQL\nSELECT * FROM cjdb.cj_object\nWHERE (attributes->\'dak_type\')::varchar = \'"slanted"\'\nORDER BY id ASC;\n```\n\n- Query all the buildings made after 2000:\n```SQL\nSELECT * FROM cjdb.cj_object\nWHERE (attributes->\'oorspronkelijkbouwjaar\')::int > 2000\nAND type = \'Building\'\nORDER BY id ASC;\n```\n\n- Query all objects with LOD 1.2\n\n```SQL\nSELECT * FROM cjdb.cj_object\nWHERE geometry::jsonb @> \'[{"lod": 1.2}]\'::jsonb\n```\n\n## 4. Local development\n\n### Install and Build\nMake sure [poetry](https://python-poetry.org/docs/) is installed and the [creation of virtual environments within the project is allowed](\nhttps://python-poetry.org/docs/configuration/#virtualenvsin-project):\n\n```\npoetry config virtualenvs.in-project true\n```\n\nThen, to create a local environment with all the necessary dependencies, run from the repository root:\n```bash\npoetry install\n```\n\nTo activate the env:\n```bash\nsource .venv/bin/activate \n```\n\nThen you can run the CLI command:\n```bash\ncjdb --help\n```\n\nEvery time you make some changed to the package you can run `poetry install` to reinstall.\n\n\n### Testing\nIn onder to run the tests you need to have [PostgreSQL](https://www.postgresql.org/download/) installed. Then you can run:\n\n```bash\npytest -v\n```\n\n## 5. Explanation\n---\n### Model assumptions\nThe `cjdb` importer loads the data in accordance with a specific data model.\n\nModel documentation:\n [model/README](model/README.md)\n\n#### Indexes\nSome indexes are created by default (refer to [model/README](model/README.md)).\n\nAdditionally, the user can specify which CityObject attributes are to be indexed with the `-x/--attr-index` or `-px/--partial-attr-index` flag, we recommend doing this if several queries are made on specific attributes. \nThe second option uses a partial index with a `not null` condition on the attribute. This saves disk space when indexing an attribute that is not present among all the imported CityObjects. \nThis is often the case with CityJSON, because in a single dataset there can be different object types, with different attributes.\n\n\n### Structuring the database and its schemas\n\nIt is recommended to group together semantically coherent objects, by importing them to the same database schema.\nOne database can have different schemas.\n\nWhile the current data model supports the import of any type of CityJSON objects together (`Building` and `SolitaryVegetationObject`), the data becomes harder to manage for the user. \nExample of this would be having different attributes for the same CityObject type (which should be consistent for data coming from the same source).\n\n\n### Input == CityJSONFeature\nThe importer works only on [*CityJSONL* files](https://www.cityjson.org/specs/#text-sequences-and-streaming-with-cityjsonfeature), that is where a CityJSON file is decomposed into its *features* (`CityJSONFeature`).\n\nThe easiest way to create these from a CityJSON file is with [cjio](https://github.com/cityjson/cjio), and to follow [those instructions](https://github.com/cityjson/cjio#stdin-and-stdout).\n\nThe importer supports 3 kinds of input:\n  1. a single CityJSONL file (only those as the output of cjio currently work)\n  1. a directory of CityJSONL files (all files with *jsonl* extensions are located and imported)\n  1. STDIN using the pipe operator: `cat file.jsonl | cjdb ...`\n\n\n\n### Coordinate Reference Systems\nThe `cjdb` importer does not allow inconsistent CRSs (coordinate reference systems) within the same database schema. For storing data in separate CRSs, you have to use different schemas.\n\nThe data needs to be either harmonized beforehand, or the `-I/--srid` flag can be used upon import, to reproject all the geometries to the one specified CRS. \nSpecifying a 2D CRS (instead of a 3D one) will cause the Z-coordinates to remain unchanged.\n\n**Note:** reprojections slow down the import significantly.\n\n**Note:** Source data with missing `"metadata"/"referenceSystem"` cannot be reprojected due to unknown source reference system.\n\n\n### 3D reprojections\n[`pyproj`](https://pyproj4.github.io/pyproj/stable/) is used for CRS reprojections. \nWhile it supports 3D CRS transformations between different systems, sometimes downloading additional [grids](https://pyproj4.github.io/pyproj/stable/transformation_grids.html) is required. \nThe importer will attempt to download the grids needed for the reprojection, with the following message:\n\n```\nAttempting to download additional grids required for CRS transformation.\nThis can also be done manually, and the files should be put in this folder:\n        {pyproj_directory}\n```\n\nIf that fails, the user will have to download the required grids and put them in the printed `{pyproj_directory}` themselves. \n\n\n### CityJSON Extensions\nIf [CityJSON Extensions](https://www.cityjson.org/extensions/) are present in the imported files, they can be found listed in the `extensions` column in the `import_meta` table.\n\nThe [CityJSON specifications](https://www.cityjson.org/specs/#extensions) mention 3 different extendable features, and the `cjdb` importer deals with them as follows:\n\n1. Complex attributes\n\nNo action is taken. These attributes end up in the `attributes` JSONB column.\n\n2. Additional root properties\n\nAdditional root properties are placed in the `extra properties` JSONB column in the `import_meta` table.\n\n3. Additional CityObject type\n\nAdditional CityObject types are appended to the list of allowed CityJSON objects.\n\n### CityJSON GeometryTemplate\n[Geometry templates](https://www.cityjson.org/specs/1.1.2/#geometry-templates)\nare resolved for each object geometry, so that the object in the table ends up with its real-world coordinates (instead of vertex references or relative template coordinates).\n\n### Data validation\nThe importer does not validate the structure of the file. It is assumed that the input file is schema-valid ([CityJSON validator](https://validator.cityjson.org/)).\nIt sends out warnings when:\n- there appear CityObject types defined neither in the main CityJSON specification nor any of the supplied extensions. \n- the specified target CRS does not have the Z-axis defined\n- the source dataset does not have a CRS defined at all\n\n### Repeated object IDs\nBy default, the importer does not check if an object with a given ID exists already in the database. This is because such an operation for every inserted object results in a performance penalty.\n\nThe user can choose to run the import with either the `-e/--skip-existing` option to skip existing objects or `-u, --update-existing` to update existing objects. This will slow down the import, but it will also ensure that repeated object cases are handled.\n\n\n\n\n',
-    'author': 'Cynthia Cai',
-    'author_email': 'None',
-    'maintainer': 'Gina Stavropoulou',
-    'maintainer_email': 'g.stavropoulou@tudelft.nl',
-    'url': 'https://github.com/tudelft3d/cjdb',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.11,<4.0',
-}
+# cjdb
+[![MIT badge](https://img.shields.io/pypi/l/cjdb)](LICENSE) &nbsp; [![PyPI](https://img.shields.io/pypi/v/cjdb)](https://pypi.org/project/cjdb)
+
+`cjdb` is a Python-based importer/exporter of [CityJSONL files (CityJSON Lines)](https://www.cityjson.org/cityjsonl/) to and from a PostgreSQL database. 
+It requires the [PostGIS](https://postgis.net/) extension.
+
+
+## Installation
+```bash
+pip install cjdb
+```
+It is recommended to install it in an isolated environment.
+
+
+## Usage
+
+Check our [docs online](https://cityjson.github.io/cjdb/cjdb.html)  or
+
+```bash
+cjdb --help
+```
+
+## Quickstart
+
+Sample CityJSON data can be downloaded from [the 3DBAG download service](https://3dbag.nl/). 
+For example, [download the tile "9-284-556"](https://data.3dbag.nl/cityjson/v20230622/tiles/9/284/556/9-284-556.city.json), within which part of TU Delft is located.
+Then, having downloaded the CityJSON file, you need a combination of [cjio](https://github.com/cityjson/cjio) (external CityJSON processing library) and cjdb to import it to a schema in a database.  Here is a step-by-step guide:
+
+1. Convert CityJSON to CityJSONL
+
+```bash
+cjio --suppress_msg 9-284-556.json export jsonl 9-284-556.jsonl 
+```
+
+2. Create a new database called "testcjdb"
+
+If you installed PostgreSQL you should have the program 'createdb', so `createdb testcjdb`
+
+Alternatively, you can use PgAdmin, [see how](https://postgis.net/workshops/postgis-intro/creating_db.html).
+
+3. Import CityJSONL to the database in the schema "cjdb"
+```bash
+cjdb import -H localhost -U postgres -d testcjdb -s cjdb  -f 9-284-556.jsonl
+```
+
+**Alternatively steps 1 and 3 in a single command:**
+
+```bash
+cjio --suppress_msg 9-284-556.json export jsonl stdout | cjdb import -H localhost -U postgres -d postgres -s cjdb
+```
+
+The metadata and the objects can then be found in the tables in the specified schema (`cjdb` in this example).
+
+The password can be specified in the `PGPASSWORD` environment variable. If not specified, the app will prompt for the password.
+
+4. If you want to export from the database you have two options. You can export the whole database in a CityJSONL file with: 
+```bash
+cjdb export -H localhost -U postgres -d testcjdb -s cjdb -o result.jsonl
+```
+or export only part of it, using a select query as input. The select query should return the ids of the objects to be exported:
+
+```bash
+cjdb export -H localhost -U postgres -d testcjdb -s cjdb -o result.jsonl -q "SELECT 1 as id"
+```
+
+## Using docker
+Build:
+```bash
+docker build -t cjdb:latest .
+```
+
+Run:
+```bash
+docker run --rm -it cjdb cjdb --help
+```
+
+To import some files, the `-v` option is needed to mount our local file directory in the container:
+```bash
+docker run -v {MYDIRECTORY}:/data --rm -it --network=host cjdb cjdb import -H localhost -U postgres -d postgres -W postgres -f /data/5870_ext.jsonl 
+```
+
+## Important Notes
+### Data model
+
+The `cjdb` importer loads the data in accordance with a [specific data model](cjdb/model/README.md).
+
+For example SQL queries on the tables see [here](cjdb/model/BASICQUERIES.md)
+
+
+### Indexes
+Some indexes are created when a new schema is created (refer to [Data Model](cjdb/model/README.md)).
+
+In addition to these indexes, the user can add more indexes on certain  CityObject attributes with the `-x/--attr-index` or the `-px/--partial-attr-index` flags.
+We recommend these additional indexes for attributes that are frequently queried.
+The second option uses a partial index with a `not null` condition on the attribute.
+This saves disk space when indexing an attribute that is not present among all the imported CityObjects.
+This is often the case with CityJSON, because in a single dataset there can be different object types, with different attributes.
+
+
+### Structuring the database and its schemas
+
+It is recommended to group together semantically coherent objects, by importing them to the same database schema.
+One database can have different schemas.
+
+While the current data model supports the import of any type of CityJSON objects together (`Building` and `SolitaryVegetationObject`), the data becomes harder to manage for the user. 
+Example of this would be having different attributes for the same CityObject type (which should be consistent for data coming from the same source).
+
+
+### Input == CityJSONFeature
+The importer works only on with [*CityJSONL* files](https://www.cityjson.org/specs/#text-sequences-and-streaming-with-cityjsonfeature), which are CityJSON files decomposed into their *features* (`CityJSONFeature`).
+
+The easiest way to create these from a CityJSON file is with [cjio](https://github.com/cityjson/cjio), by following [these instructions](https://github.com/cityjson/cjio#stdin-and-stdout).
+
+The importer supports 3 kinds of input:
+  1. a single CityJSONL file (only those as the output of cjio currently work)
+  1. a directory of CityJSONL files (all files with *jsonl* extensions are located and imported)
+  1. STDIN using the pipe operator: `cat file.jsonl | cjdb ...`
+
+
+### Coordinate Reference Systems
+The `cjdb` importer does not allow inconsistent CRSs (coordinate reference systems) within the same database schema. For storing data in different CRSs, you have to create different schemas.
+
+The data needs to be either harmonized beforehand, or the `--transform` flag can be used upon import, to reproject all the geometries to the CRS of the existing schema. 
+Specifying a 2D CRS (instead of a 3D one) will cause the Z-coordinates to remain unchanged.
+
+**Note:** reprojections slow down the import significantly.
+
+**Note:** Source data with missing `"metadata"/"referenceSystem"` cannot be reprojected due to unknown source reference system. 
+You can use the `-I/--srid` flag to set the SRID of the input file. 
+
+
+### 3D reprojections
+[`pyproj`](https://pyproj4.github.io/pyproj/stable/) is used for CRS reprojections. 
+While it supports 3D CRS transformations between different systems, sometimes downloading additional [grids](https://pyproj4.github.io/pyproj/stable/transformation_grids.html) is required. 
+The importer will attempt to download the grids needed for the reprojection, with the following message:
+
+```
+Attempting to download additional grids required for CRS transformation.
+This can also be done manually, and the files should be put in this folder:
+        {pyproj_directory}
+```
+
+If that fails, the user will have to download the required grids and put them in the printed `{pyproj_directory}` themselves. 
+
+
+### CityJSON Extensions
+If [CityJSON Extensions](https://www.cityjson.org/extensions/) are present in the imported files, they can be found listed in the `extensions` column in the `cj_metadata` table.
+
+The [CityJSON specifications](https://www.cityjson.org/specs/#extensions) mention 3 different extendable features, and the `cjdb` importer deals with them as follows:
+
+1. Complex attributes
+
+No action is taken. These attributes end up in the `attributes` JSONB column.
+
+2. Additional root properties
+
+Additional root properties are placed in the `extra properties` JSONB column in the `cj_metadata` table.
+
+3. Additional CityObject type
+
+Additional CityObject types are appended to the list of allowed CityJSON objects.
+
+### CityJSON GeometryTemplate
+[Geometry templates](https://www.cityjson.org/specs/1.1.2/#geometry-templates)
+are resolved for each object geometry, so that the object in the table ends up with its real-world coordinates (instead of vertex references or relative template coordinates).
+
+### Data validation
+The importer does not validate the structure of the file. It is assumed that the input file is schema-valid ([CityJSON validator](https://validator.cityjson.org/)).
+It sends out warnings when:
+- CityObject types appear which are defined neither in the main CityJSON specification nor in any of the supplied extensions. 
+- the specified target CRS does not have the Z-axis defined
+- the source dataset does not have a CRS defined at all
+
+### Repeated object IDs
+The importer does not check if an object with a specific ID exists already in the database - every imported object gets and new id. However, at the time of import the importer will detect previously detected files with the same filename. The user can choose to run the import with either the `-g, --ignore-repeated-file` option to import files with the same filename under a different id or `--overwrite` to overwrite *all* previously imported objects with this filename.
+
+
+## Contributors
+
+This project started as a group project in the [MSc Geomatics at TUDelft](https://geomatics.tudelft.nl/).
+The original code for the project can be found [here](https://github.com/leoleonsio/cjdb), and the authors were:
+[@cynthiacai56](https://github.com/cynthiacai56), [@LanYan1110](https://github.com/LanYan1110), [@YitongXia](https://github.com/YitongXia), [@Topher2k](https://github.com/Topher2k), [@siebren014](https://github.com/siebren014), [@leoleonsio](https://github.com/leoleonsio)
+
+This version has been improved and will be maintained by [@GinaStavropoulou](https://github.com/GinaStavropoulou), and [@hugoledoux](https://github.com/hugoledoux).
 
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cjdb-1.2.0/PKG-INFO` & `cjdb-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,329 +1,136 @@
-Metadata-Version: 2.1
-Name: cjdb
-Version: 1.2.0
-Summary: CJDB is a tool that enables CityJSON integration with a PostgreSQL database
-Home-page: https://github.com/tudelft3d/cjdb
-License: MIT
-Keywords: CityJSON,PostgreSQL
-Author: Cynthia Cai
-Maintainer: Gina Stavropoulou
-Maintainer-email: g.stavropoulou@tudelft.nl
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cjio (>=0.8.1,<0.9.0)
-Requires-Dist: geoalchemy2 (>=0.13.1,<0.14.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
-Requires-Dist: pyproj (>=3.5.0,<4.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: shapely (>=2.0.1,<3.0.0)
-Project-URL: Repository, https://github.com/tudelft3d/cjdb
-Description-Content-Type: text/markdown
-
 # cjdb
 [![MIT badge](https://img.shields.io/pypi/l/cjdb)](LICENSE) &nbsp; [![PyPI](https://img.shields.io/pypi/v/cjdb)](https://pypi.org/project/cjdb)
 
-`cjdb` is a Python based importer of CityJSONL files to a PostgreSQL database. It requires the [PostGIS](https://postgis.net/) extension.
-
-Authors: Cynthia Cai, Lan Yan, Yitong Xia, Chris Poon, Siebren Meines, Leon Powalka
-
-Maintainer: Gina Stavropoulou
+`cjdb` is a Python-based importer/exporter of [CityJSONL files (CityJSON Lines)](https://www.cityjson.org/cityjsonl/) to and from a PostgreSQL database. 
+It requires the [PostGIS](https://postgis.net/) extension.
 
-## Table of Contents  
-### [1.Data model](#1-data-model)
-### [2.Installation](#2-installation)
-- [Using pip](#using-pip)
-- [Using Docker](#using-docker)
-### [3.Usage](#3-usage)
-- [CLI](#cli)
-- [Quickstart](#quickstart)
-- [Basic Queries](#basic-queries)
-### [4.Local development](#4-local-development)
-- [Install and Build](#install-and-build)
-- [Testing](#testing)
-### [5.Explanation](#5-explanation)
- - [Model assumptions](#model-assumptions)
- - [What is a City Model?](#what-is-a-city-model)
- - [Types of input](#types-of-input)
- - [Coordinate Reference Systems](#coordinate-reference-systems)
- - [3D reprojections](#3d-reprojections)
- - [CityJSON Extensions](#cityjson-extensions)
- - [CityJSON GeometryTemplate](#cityjson-geometrytemplate)
- - [Data validation](#data-validation)
- - [Repeated object IDs](#repeated-object-ids)
----
-## 1. Data model
-For the underlying data model see [cjdb/model/README.md](cjdb/model/README.md)
 
-
-## 2. Installation
-### Using pip
+## Installation
 ```bash
 pip install cjdb
 ```
-It is recommended to install it in an isolated environment, because of fragile external library dependencies for CQL filter parsing.
+It is recommended to install it in an isolated environment.
 
-### Using docker
-Build:
-```bash
-docker build -t cjdb:latest .
-```
 
-Run:
-```bash
-docker run --rm -it cjdb cjdb --help
-```
+## Usage
 
-To import some files, the `-v` option is needed to mount our local file directory in the container:
-```bash
-docker run -v {MYDIRECTORY}:/data --rm -it --network=host cjdb cjdb -H localhost -U postgres -d postgres -W postgres /data/5870_ext.jsonl 
-```
-## 3. Usage <a name="usage"></a>
-
-### CLI <a name="cli"></a>
+Check our [docs online](https://cityjson.github.io/cjdb/cjdb.html)  or
 
 ```bash
-cj2pgsql [-h] [-H DB_HOST] [-p DB_PORT] -U DB_USER [-W DB_PASSWORD] -d DB_NAME [-s DB_SCHEMA] [-I TARGET_SRID][-x INDEXED_ATTRIBUTES] [-px PARTIAL_INDEXED_ATTRIBUTES] [-g] [-a | -o] [-e | -u] [file_or_directory]
+cjdb --help
 ```
-#### Positional Arguments
-file_or_directory
-Source CityJSONL file or a directory with CityJSONL files. STDIN if not specified. If specifying a directory, all the *.jsonl files inside of it will be imported.
-
-Default: “stdin”
-
-#### Named Arguments
-`-I, --srid`
-Target coordinate system SRID. All 3D and 2D geometries will be reprojected.
-
-`-x, --attr-index`
-CityObject attribute to be indexed using a btree index. Can be specified multiple times, for each attribute once.
-
-Default: []
-
-`-px, --partial-attr-index`
-CityObject attribute to be indexed using a btree partial index. Can be specified multiple times, for each attribute once. This index indexes on a condition ‘where {
-                {ATTR_NAME
-                }
-        } is not null’. This means that it saves space and improves query performance when the attribute is not present for all imported CityObjects.
-
-Default: []
-
-`-g, --ignore-repeated-file`
-Ignore repeated file names warning when importing. By default, the importer will send out warnings if a specific file has already been imported.
-
-Default: False
-
-`-a, --append`
-Run in append mode (as opposed to default create mode). This assumes the database structure exists already and new data is to be appended.
-
-Default: False
-
-`-o, --overwrite`
-Overwrite the data that is currently in the database schema. Warning: this causes the loss of what was imported before to the database schema.
-
-Default: False
-
-`-u, --update-existing`
-Check if the object with given ID exists before inserting, and update it if it does. The old object will be updated with the new object’s properties.
-
-Default: False
-
-#### Database connection arguments
-`-H, --host`
-PostgreSQL database host
-
-Default: “localhost”
-
-`-p, --port`
-PostgreSQL database port
-
-Default: 5432
-
-`-U, --user`
-PostgreSQL database user name
-
-`-W, --password`
-PostgreSQL database user password
 
-`-d, --database`
-PostgreSQL database name
+## Quickstart
 
-`-s, --schema`
-Target database schema
-
-Default: “public”
-
-### Quickstart
-
-Sample CityJSON data can be downloaded from [3DBAG download service](https://3dbag.nl/nl/download?tid=901). Then, having the CityJSON file, a combination of [cjio](https://github.com/cityjson/cjio) (external CityJSON processing library) and cjdb is needed to import it to a specified schema in a database. 
+Sample CityJSON data can be downloaded from [the 3DBAG download service](https://3dbag.nl/). 
+For example, [download the tile "9-284-556"](https://data.3dbag.nl/cityjson/v20230622/tiles/9/284/556/9-284-556.city.json), within which part of TU Delft is located.
+Then, having downloaded the CityJSON file, you need a combination of [cjio](https://github.com/cityjson/cjio) (external CityJSON processing library) and cjdb to import it to a schema in a database.  Here is a step-by-step guide:
 
 1. Convert CityJSON to CityJSONL
 
 ```bash
-cjio --suppress_msg tile_901.json export jsonl tile_901.jsonl 
+cjio --suppress_msg 9-284-556.json export jsonl 9-284-556.jsonl 
 ```
 
-2. Create a new database
+2. Create a new database called "testcjdb"
 
-  - [how to create a new database](https://postgis.net/workshops/postgis-intro/creating_db.html)
+If you installed PostgreSQL you should have the program 'createdb', so `createdb testcjdb`
 
-3. Import CityJSONL to the database
+Alternatively, you can use PgAdmin, [see how](https://postgis.net/workshops/postgis-intro/creating_db.html).
+
+3. Import CityJSONL to the database in the schema "cjdb"
 ```bash
-PGPASSWORD=postgres cjdb -H localhost -U postgres -d postgres -s cjdb -o tile_901.jsonl   
+cjdb import -H localhost -U postgres -d testcjdb -s cjdb  -f 9-284-556.jsonl
 ```
 
-**Alternatively steps 1 and 2 in a single command:**
+**Alternatively steps 1 and 3 in a single command:**
 
 ```bash
-cjio --suppress_msg tile_901.json export jsonl stdout | cjdb -H localhost -U postgres -d postgres -s cjdb -o
+cjio --suppress_msg 9-284-556.json export jsonl stdout | cjdb import -H localhost -U postgres -d postgres -s cjdb
 ```
 
 The metadata and the objects can then be found in the tables in the specified schema (`cjdb` in this example).
 
+The password can be specified in the `PGPASSWORD` environment variable. If not specified, the app will prompt for the password.
 
-Password can be specified in the `PGPASSWORD` environment variable. If not specified, the app will prompt for the password.
-
-
-### Basic Queries
-
-- Query an object with a specific id:
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE object_id = 'NL.IMBAG.Pand.0503100000000334';
-```
-
-- Query a building with a specific child
-```SQL
-SELECT o.* FROM cjdb.family f
-INNER JOIN cjdb.cj_object o ON o.object_id = f.parent_id
-WHERE f.child_id = 'NL.IMBAG.Pand.0503100000000334-0'
-```
-
-- Query all buildings within a bounding box
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE type = 'Building'
-AND ST_Contains(ST_MakeEnvelope(81900.00, 446850.00, 81930.00, 446900.00, 7415), ground_geometry)
-ORDER BY id ASC;
-```
-
-- Query the building intersecting with a point
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE ground_geometry && ST_MakePoint(81915.00, 446850.00)
-AND type = 'Building'
-ORDER BY object_id ASC;
-```
-
-- Query all objects with a slanted roof
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE (attributes->'dak_type')::varchar = '"slanted"'
-ORDER BY id ASC;
-```
-
-- Query all the buildings made after 2000:
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE (attributes->'oorspronkelijkbouwjaar')::int > 2000
-AND type = 'Building'
-ORDER BY id ASC;
-```
-
-- Query all objects with LOD 1.2
-
-```SQL
-SELECT * FROM cjdb.cj_object
-WHERE geometry::jsonb @> '[{"lod": 1.2}]'::jsonb
+4. If you want to export from the database you have two options. You can export the whole database in a CityJSONL file with: 
+```bash
+cjdb export -H localhost -U postgres -d testcjdb -s cjdb -o result.jsonl
 ```
+or export only part of it, using a select query as input. The select query should return the ids of the objects to be exported:
 
-## 4. Local development
-
-### Install and Build
-Make sure [poetry](https://python-poetry.org/docs/) is installed and the [creation of virtual environments within the project is allowed](
-https://python-poetry.org/docs/configuration/#virtualenvsin-project):
-
-```
-poetry config virtualenvs.in-project true
+```bash
+cjdb export -H localhost -U postgres -d testcjdb -s cjdb -o result.jsonl -q "SELECT 1 as id"
 ```
 
-Then, to create a local environment with all the necessary dependencies, run from the repository root:
+## Using docker
+Build:
 ```bash
-poetry install
+docker build -t cjdb:latest .
 ```
 
-To activate the env:
+Run:
 ```bash
-source .venv/bin/activate 
+docker run --rm -it cjdb cjdb --help
 ```
 
-Then you can run the CLI command:
+To import some files, the `-v` option is needed to mount our local file directory in the container:
 ```bash
-cjdb --help
+docker run -v {MYDIRECTORY}:/data --rm -it --network=host cjdb cjdb import -H localhost -U postgres -d postgres -W postgres -f /data/5870_ext.jsonl 
 ```
 
-Every time you make some changed to the package you can run `poetry install` to reinstall.
+## Important Notes
+### Data model
 
+The `cjdb` importer loads the data in accordance with a [specific data model](cjdb/model/README.md).
 
-### Testing
-In onder to run the tests you need to have [PostgreSQL](https://www.postgresql.org/download/) installed. Then you can run:
+For example SQL queries on the tables see [here](cjdb/model/BASICQUERIES.md)
 
-```bash
-pytest -v
-```
 
-## 5. Explanation
----
-### Model assumptions
-The `cjdb` importer loads the data in accordance with a specific data model.
+### Indexes
+Some indexes are created when a new schema is created (refer to [Data Model](cjdb/model/README.md)).
 
-Model documentation:
- [model/README](model/README.md)
-
-#### Indexes
-Some indexes are created by default (refer to [model/README](model/README.md)).
-
-Additionally, the user can specify which CityObject attributes are to be indexed with the `-x/--attr-index` or `-px/--partial-attr-index` flag, we recommend doing this if several queries are made on specific attributes. 
-The second option uses a partial index with a `not null` condition on the attribute. This saves disk space when indexing an attribute that is not present among all the imported CityObjects. 
+In addition to these indexes, the user can add more indexes on certain  CityObject attributes with the `-x/--attr-index` or the `-px/--partial-attr-index` flags.
+We recommend these additional indexes for attributes that are frequently queried.
+The second option uses a partial index with a `not null` condition on the attribute.
+This saves disk space when indexing an attribute that is not present among all the imported CityObjects.
 This is often the case with CityJSON, because in a single dataset there can be different object types, with different attributes.
 
 
 ### Structuring the database and its schemas
 
 It is recommended to group together semantically coherent objects, by importing them to the same database schema.
 One database can have different schemas.
 
 While the current data model supports the import of any type of CityJSON objects together (`Building` and `SolitaryVegetationObject`), the data becomes harder to manage for the user. 
 Example of this would be having different attributes for the same CityObject type (which should be consistent for data coming from the same source).
 
 
 ### Input == CityJSONFeature
-The importer works only on [*CityJSONL* files](https://www.cityjson.org/specs/#text-sequences-and-streaming-with-cityjsonfeature), that is where a CityJSON file is decomposed into its *features* (`CityJSONFeature`).
+The importer works only on with [*CityJSONL* files](https://www.cityjson.org/specs/#text-sequences-and-streaming-with-cityjsonfeature), which are CityJSON files decomposed into their *features* (`CityJSONFeature`).
 
-The easiest way to create these from a CityJSON file is with [cjio](https://github.com/cityjson/cjio), and to follow [those instructions](https://github.com/cityjson/cjio#stdin-and-stdout).
+The easiest way to create these from a CityJSON file is with [cjio](https://github.com/cityjson/cjio), by following [these instructions](https://github.com/cityjson/cjio#stdin-and-stdout).
 
 The importer supports 3 kinds of input:
   1. a single CityJSONL file (only those as the output of cjio currently work)
   1. a directory of CityJSONL files (all files with *jsonl* extensions are located and imported)
   1. STDIN using the pipe operator: `cat file.jsonl | cjdb ...`
 
 
-
 ### Coordinate Reference Systems
-The `cjdb` importer does not allow inconsistent CRSs (coordinate reference systems) within the same database schema. For storing data in separate CRSs, you have to use different schemas.
+The `cjdb` importer does not allow inconsistent CRSs (coordinate reference systems) within the same database schema. For storing data in different CRSs, you have to create different schemas.
 
-The data needs to be either harmonized beforehand, or the `-I/--srid` flag can be used upon import, to reproject all the geometries to the one specified CRS. 
+The data needs to be either harmonized beforehand, or the `--transform` flag can be used upon import, to reproject all the geometries to the CRS of the existing schema. 
 Specifying a 2D CRS (instead of a 3D one) will cause the Z-coordinates to remain unchanged.
 
 **Note:** reprojections slow down the import significantly.
 
-**Note:** Source data with missing `"metadata"/"referenceSystem"` cannot be reprojected due to unknown source reference system.
+**Note:** Source data with missing `"metadata"/"referenceSystem"` cannot be reprojected due to unknown source reference system. 
+You can use the `-I/--srid` flag to set the SRID of the input file. 
 
 
 ### 3D reprojections
 [`pyproj`](https://pyproj4.github.io/pyproj/stable/) is used for CRS reprojections. 
 While it supports 3D CRS transformations between different systems, sometimes downloading additional [grids](https://pyproj4.github.io/pyproj/stable/transformation_grids.html) is required. 
 The importer will attempt to download the grids needed for the reprojection, with the following message:
 
@@ -333,43 +140,46 @@
         {pyproj_directory}
 ```
 
 If that fails, the user will have to download the required grids and put them in the printed `{pyproj_directory}` themselves. 
 
 
 ### CityJSON Extensions
-If [CityJSON Extensions](https://www.cityjson.org/extensions/) are present in the imported files, they can be found listed in the `extensions` column in the `import_meta` table.
+If [CityJSON Extensions](https://www.cityjson.org/extensions/) are present in the imported files, they can be found listed in the `extensions` column in the `cj_metadata` table.
 
 The [CityJSON specifications](https://www.cityjson.org/specs/#extensions) mention 3 different extendable features, and the `cjdb` importer deals with them as follows:
 
 1. Complex attributes
 
 No action is taken. These attributes end up in the `attributes` JSONB column.
 
 2. Additional root properties
 
-Additional root properties are placed in the `extra properties` JSONB column in the `import_meta` table.
+Additional root properties are placed in the `extra properties` JSONB column in the `cj_metadata` table.
 
 3. Additional CityObject type
 
 Additional CityObject types are appended to the list of allowed CityJSON objects.
 
 ### CityJSON GeometryTemplate
 [Geometry templates](https://www.cityjson.org/specs/1.1.2/#geometry-templates)
 are resolved for each object geometry, so that the object in the table ends up with its real-world coordinates (instead of vertex references or relative template coordinates).
 
 ### Data validation
 The importer does not validate the structure of the file. It is assumed that the input file is schema-valid ([CityJSON validator](https://validator.cityjson.org/)).
 It sends out warnings when:
-- there appear CityObject types defined neither in the main CityJSON specification nor any of the supplied extensions. 
+- CityObject types appear which are defined neither in the main CityJSON specification nor in any of the supplied extensions. 
 - the specified target CRS does not have the Z-axis defined
 - the source dataset does not have a CRS defined at all
 
 ### Repeated object IDs
-By default, the importer does not check if an object with a given ID exists already in the database. This is because such an operation for every inserted object results in a performance penalty.
-
-The user can choose to run the import with either the `-e/--skip-existing` option to skip existing objects or `-u, --update-existing` to update existing objects. This will slow down the import, but it will also ensure that repeated object cases are handled.
+The importer does not check if an object with a specific ID exists already in the database - every imported object gets and new id. However, at the time of import the importer will detect previously detected files with the same filename. The user can choose to run the import with either the `-g, --ignore-repeated-file` option to import files with the same filename under a different id or `--overwrite` to overwrite *all* previously imported objects with this filename.
 
 
+## Contributors
 
+This project started as a group project in the [MSc Geomatics at TUDelft](https://geomatics.tudelft.nl/).
+The original code for the project can be found [here](https://github.com/leoleonsio/cjdb), and the authors were:
+[@cynthiacai56](https://github.com/cynthiacai56), [@LanYan1110](https://github.com/LanYan1110), [@YitongXia](https://github.com/YitongXia), [@Topher2k](https://github.com/Topher2k), [@siebren014](https://github.com/siebren014), [@leoleonsio](https://github.com/leoleonsio)
 
+This version has been improved and will be maintained by [@GinaStavropoulou](https://github.com/GinaStavropoulou), and [@hugoledoux](https://github.com/hugoledoux).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

