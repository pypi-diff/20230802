# Comparing `tmp/caluma_alexandria-1.2.0.tar.gz` & `tmp/caluma_alexandria-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma_alexandria-1.2.0.tar", max compression
+gzip compressed data, was "caluma_alexandria-2.0.0.tar", max compression
```

## Comparing `caluma_alexandria-1.2.0.tar` & `caluma_alexandria-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     9458 2023-06-09 09:29:53.238949 caluma_alexandria-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    35148 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/LICENSE
--rw-r--r--   0        0        0     4650 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/README.md
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/__init__.py
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/__init__.py
--rw-r--r--   0        0        0      863 2023-05-04 13:55:17.660574 caluma_alexandria-1.2.0/alexandria/core/apps.py
--rw-r--r--   0        0        0      195 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/collections.py
--rw-r--r--   0        0        0     1922 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/factories.py
--rw-r--r--   0        0        0     5022 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/filters.py
--rw-r--r--   0        0        0    13121 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      490 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/migrations/0002_tags_monolingual.py
--rw-r--r--   0        0        0      644 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/migrations/0003_file_upload_status.py
--rw-r--r--   0        0        0     2982 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/migrations/0004_tag_synonym_group.py
--rw-r--r--   0        0        0     1065 2023-04-27 09:52:20.806733 caluma_alexandria-1.2.0/alexandria/core/migrations/0005_rename_type_and_meta.py
--rw-r--r--   0        0        0     1146 2023-05-11 11:29:27.228878 caluma_alexandria-1.2.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/migrations/__init__.py
--rw-r--r--   0        0        0     6353 2023-05-11 09:24:07.841154 caluma_alexandria-1.2.0/alexandria/core/models.py
--rw-r--r--   0        0        0     4623 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/core/permissions.py
--rw-r--r--   0        0        0     6967 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/core/serializers.py
--rw-r--r--   0        0        0     2770 2023-06-01 09:09:52.734835 caluma_alexandria-1.2.0/alexandria/core/storage_clients.py
--rw-r--r--   0        0        0     1544 2023-04-27 09:52:20.810733 caluma_alexandria-1.2.0/alexandria/core/thumbs.py
--rw-r--r--   0        0        0      462 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/urls.py
--rw-r--r--   0        0        0     1754 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/core/validation.py
--rw-r--r--   0        0        0     6025 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/views.py
--rw-r--r--   0        0        0     5021 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/core/visibilities.py
--rw-r--r--   0        0        0        0 2022-12-16 12:36:48.076001 caluma_alexandria-1.2.0/alexandria/oidc_auth/__init__.py
--rw-r--r--   0        0        0     4224 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2022-12-16 12:36:48.080001 caluma_alexandria-1.2.0/alexandria/oidc_auth/models.py
--rw-r--r--   0        0        0       30 2023-04-19 12:35:40.637143 caluma_alexandria-1.2.0/alexandria/settings/__init__.py
--rw-r--r--   0        0        0     5008 2023-06-09 09:10:05.343196 caluma_alexandria-1.2.0/alexandria/settings/alexandria.py
--rw-r--r--   0        0        0     4778 2023-05-04 12:51:21.034379 caluma_alexandria-1.2.0/alexandria/settings/django.py
--rw-r--r--   0        0        0      162 2023-04-27 09:52:20.810733 caluma_alexandria-1.2.0/alexandria/urls.py
--rw-r--r--   0        0        0      407 2023-04-19 08:37:34.482085 caluma_alexandria-1.2.0/alexandria/wsgi.py
--rw-r--r--   0        0        0     3021 2023-06-09 09:29:26.542772 caluma_alexandria-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 caluma_alexandria-1.2.0/setup.py
--rw-r--r--   0        0        0     6034 1970-01-01 00:00:00.000000 caluma_alexandria-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11730 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35148 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4660 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/__init__.py
+-rw-r--r--   0        0        0      863 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/apps.py
+-rw-r--r--   0        0        0      195 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/collections.py
+-rw-r--r--   0        0        0     1966 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/factories.py
+-rw-r--r--   0        0        0     5022 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/filters.py
+-rw-r--r--   0        0        0    13121 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      490 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0002_tags_monolingual.py
+-rw-r--r--   0        0        0      644 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0003_file_upload_status.py
+-rw-r--r--   0        0        0     2982 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0004_tag_synonym_group.py
+-rw-r--r--   0        0        0     1065 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py
+-rw-r--r--   0        0        0     1146 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
+-rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/__init__.py
+-rw-r--r--   0        0        0     6353 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/models.py
+-rw-r--r--   0        0        0     4645 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/permissions.py
+-rw-r--r--   0        0        0     6967 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/serializers.py
+-rw-r--r--   0        0        0     2902 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/storage_clients.py
+-rw-r--r--   0        0        0     1588 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/thumbs.py
+-rw-r--r--   0        0        0      462 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/urls.py
+-rw-r--r--   0        0        0     1754 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/validation.py
+-rw-r--r--   0        0        0     6069 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/views.py
+-rw-r--r--   0        0        0     5021 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/visibilities.py
+-rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     4224 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/oidc_auth/models.py
+-rw-r--r--   0        0        0       30 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/settings/__init__.py
+-rw-r--r--   0        0        0     3816 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/settings/alexandria.py
+-rw-r--r--   0        0        0     4817 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/settings/django.py
+-rw-r--r--   0        0        0      162 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/urls.py
+-rw-r--r--   0        0        0      407 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/wsgi.py
+-rw-r--r--   0        0        0     2901 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 caluma_alexandria-2.0.0/PKG-INFO
```

### Comparing `caluma_alexandria-1.2.0/LICENSE` & `caluma_alexandria-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/README.md` & `caluma_alexandria-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,72 +15,74 @@
 [Original RFC that led to alexandria](docs/original_alexandria_rfc.md)
 
 ## Getting started
 
 ### Installation
 
 **Requirements**
-* docker
-* docker-compose
+
+- docker
+- docker-compose
 
 After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/projectcaluma/alexandria/master/docker-compose.yml) and run the following commands:
 
 ```bash
 # only needs to be run once
 echo UID=$UID > .env
 
-docker-compose up -d
+docker compose up -d
 ```
 
 You can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/).
 
 ### Example data
 
 To load a set of categories run the following command:
+
 ```bash
 make load_example_data
 ```
 
 ### Configuration
 
 Document Merge Service is a [12factor app](https://12factor.net/) which means that configuration is stored in environment variables.
 Different environment variable types are explained at [django-environ](https://github.com/joke2k/django-environ#supported-types).
 
 #### Common
 
 A list of configuration options which you need
 
-* Django configuration
-  * `SECRET_KEY`: A secret key used for cryptography. This needs to be a random string of a certain length. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-SECRET_KEY).
-  * `ALLOWED_HOSTS`: A list of hosts/domains your service will be served from. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#allowed-hosts).
-  * `DATABASE_ENGINE`: Database backend to use. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-DATABASE-ENGINE). (default: django.db.backends.postgresql)
-  * `DATABASE_HOST`: Host to use when connecting to database (default: localhost)
-  * `DATABASE_PORT`: Port to use when connecting to database (default: 5432)
-  * `DATABASE_NAME`: Name of database to use (default: alexandria)
-  * `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)
-  * `DATABASE_PASSWORD`: Password to use when connecting to database
-* Authentication configuration
-  * `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC
-  * `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development
-  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own
-  * `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
-  * `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
-  * `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
-* Authorization configurations
-  * `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models
-  * `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models
-* Data validation configuration
-  * `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)
+- Django configuration
+  - `SECRET_KEY`: A secret key used for cryptography. This needs to be a random string of a certain length. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-SECRET_KEY).
+  - `ALLOWED_HOSTS`: A list of hosts/domains your service will be served from. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#allowed-hosts).
+  - `DATABASE_ENGINE`: Database backend to use. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-DATABASE-ENGINE). (default: django.db.backends.postgresql)
+  - `DATABASE_HOST`: Host to use when connecting to database (default: localhost)
+  - `DATABASE_PORT`: Port to use when connecting to database (default: 5432)
+  - `DATABASE_NAME`: Name of database to use (default: alexandria)
+  - `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)
+  - `DATABASE_PASSWORD`: Password to use when connecting to database
+- Authentication configuration
+  - `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC
+  - `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development
+  - `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own
+  - `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
+  - `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
+  - `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
+- Authorization configurations
+  - `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models
+  - `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models
+- Data validation configuration
+  - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)
 
 For development, you can also set the following environemnt variables to help
 you:
 
-  * `DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.
-  * `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.
+- `ALEXANDRIA_DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.
+- `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.
 
 ## Contributing
 
 Look at our [contributing guidelines](CONTRIBUTING.md) to start with your first contribution.
 
 ## Maintainer's Handbook
 
-Some notes for maintaining this project can be found in [the maintainer's handbook](MAINTAINING.md).
+Some notes for maintaining this project can be found in [the maintainer's handbook](MAINTAINING.md).
```

### Comparing `caluma_alexandria-1.2.0/alexandria/core/apps.py` & `caluma_alexandria-2.0.0/alexandria/core/apps.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/factories.py` & `caluma_alexandria-2.0.0/alexandria/core/factories.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class TagSynonymGroupFactory(BaseFactory):
     class Meta:
         model = models.TagSynonymGroup
 
     @post_generation
     def tags(self, create, extracted, **kwargs):
-        if not create:
+        if not create:  # pragma: todo cover
             # Simple build, do nothing.
             return
 
         if extracted:
             # A list of tags were passed in, use them
             for tag in extracted:
                 self.tags.add(tag)
@@ -56,15 +56,15 @@
 
     title = Faker("name")
     description = Faker("text")
     category = SubFactory(CategoryFactory)
 
     @post_generation
     def tags(self, create, extracted, **kwargs):
-        if not create:
+        if not create:  # pragma: todo cover
             # Simple build, do nothing.
             return
 
         if extracted:
             # A list of tags were passed in, use them
             for tag in extracted:
                 self.tags.add(tag)
```

### Comparing `caluma_alexandria-1.2.0/alexandria/core/filters.py` & `caluma_alexandria-2.0.0/alexandria/core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/migrations/0001_initial.py` & `caluma_alexandria-2.0.0/alexandria/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/migrations/0003_file_upload_status.py` & `caluma_alexandria-2.0.0/alexandria/core/migrations/0003_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/migrations/0004_tag_synonym_group.py` & `caluma_alexandria-2.0.0/alexandria/core/migrations/0004_tag_synonym_group.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/migrations/0005_rename_type_and_meta.py` & `caluma_alexandria-2.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py` & `caluma_alexandria-2.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/models.py` & `caluma_alexandria-2.0.0/alexandria/core/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/permissions.py` & `caluma_alexandria-2.0.0/alexandria/core/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,10 +133,10 @@
     @object_permission_for(BaseModel)
     def base_object_permission(self, request, instance):
         return self.base_permission(request) and self.validate_group(
             request.user, instance.created_by_group
         )
 
     def validate_group(self, user, value):
-        if value and value not in user.groups:
+        if value and value not in user.groups:  # pragma: todo cover
             return False
         return True
```

### Comparing `caluma_alexandria-1.2.0/alexandria/core/serializers.py` & `caluma_alexandria-2.0.0/alexandria/core/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/storage_clients.py` & `caluma_alexandria-2.0.0/alexandria/core/storage_clients.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,51 +19,51 @@
     @wraps(fn)
     def wrapper(self, *args, **kwargs):
         try:
             return fn(self, *args, **kwargs)
         except minio.error.S3Error as exc:
             if (
                 exc.code == "NoSuchBucket"
-                and settings.MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET
+                and settings.ALEXANDRIA_MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET
             ):
                 log.warning(
                     f"Minio bucket '{self.bucket}' missing, trying to create it"
                 )
                 self.client.make_bucket(self.bucket)
                 return fn(self, *args, **kwargs)
-            raise
+            raise  # pragma: todo cover
 
     return wrapper
 
 
 class Minio:
     def __init__(self):
-        endpoint = settings.MINIO_STORAGE_ENDPOINT
-        access_key = settings.MINIO_STORAGE_ACCESS_KEY
-        secret_key = settings.MINIO_STORAGE_SECRET_KEY
-        secure = settings.MINIO_STORAGE_USE_HTTPS
+        endpoint = settings.ALEXANDRIA_MINIO_STORAGE_ENDPOINT
+        access_key = settings.ALEXANDRIA_MINIO_STORAGE_ACCESS_KEY
+        secret_key = settings.ALEXANDRIA_MINIO_STORAGE_SECRET_KEY
+        secure = settings.ALEXANDRIA_MINIO_STORAGE_USE_HTTPS
         self.client = minio.Minio(
             endpoint, access_key=access_key, secret_key=secret_key, secure=secure
         )
-        self.bucket = settings.MINIO_STORAGE_MEDIA_BUCKET_NAME
+        self.bucket = settings.ALEXANDRIA_MINIO_STORAGE_MEDIA_BUCKET_NAME
 
     @_retry_on_missing_bucket
     def download_url(self, object_name):
         return self.client.presigned_get_object(
             self.bucket,
             object_name,
-            timedelta(minutes=settings.MINIO_PRESIGNED_TTL_MINUTES),
+            timedelta(minutes=settings.ALEXANDRIA_MINIO_PRESIGNED_TTL_MINUTES),
         )
 
     @_retry_on_missing_bucket
     def upload_url(self, object_name):
         return self.client.presigned_put_object(
             self.bucket,
             object_name,
-            timedelta(minutes=settings.MINIO_PRESIGNED_TTL_MINUTES),
+            timedelta(minutes=settings.ALEXANDRIA_MINIO_PRESIGNED_TTL_MINUTES),
         )
 
     @_retry_on_missing_bucket
     def remove_object(self, object_name):
         self.client.remove_object(self.bucket, object_name)
 
     @_retry_on_missing_bucket
@@ -78,14 +78,14 @@
         with filepath.open("rb") as file_data:
             file_stat = filepath.stat()
             return self.client.put_object(
                 self.bucket, object_name, file_data, file_stat.st_size
             )
 
 
-if settings.MEDIA_STORAGE_SERVICE == "minio":
+if settings.ALEXANDRIA_MEDIA_STORAGE_SERVICE == "minio":
     client = Minio()
 else:  # pragma: no cover
     client = None
     raise NotImplementedError(
-        f"Storage service {settings.MEDIA_STORAGE_SERVICE} is not implemented!"
+        f"Storage service {settings.ALEXANDRIA_MEDIA_STORAGE_SERVICE} is not implemented!"
     )
```

### Comparing `caluma_alexandria-1.2.0/alexandria/core/thumbs.py` & `caluma_alexandria-2.0.0/alexandria/core/thumbs.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     with temp_filepath.open("wb") as f:
         for d in data.stream(32 * 1024):
             f.write(d)
 
     manager = PreviewManager(str(temp_dir.name))
 
     preview_kwargs = {}
-    if settings.THUMBNAIL_WIDTH:  # pragma: no cover
-        preview_kwargs["width"] = settings.THUMBNAIL_WIDTH
-    if settings.THUMBNAIL_HEIGHT:  # pragma: no cover
-        preview_kwargs["height"] = settings.THUMBNAIL_HEIGHT
+    if settings.ALEXANDRIA_THUMBNAIL_WIDTH:  # pragma: no cover
+        preview_kwargs["width"] = settings.ALEXANDRIA_THUMBNAIL_WIDTH
+    if settings.ALEXANDRIA_THUMBNAIL_HEIGHT:  # pragma: no cover
+        preview_kwargs["height"] = settings.ALEXANDRIA_THUMBNAIL_HEIGHT
 
     try:
         path_to_preview_image = manager.get_jpeg_preview(
             str(temp_filepath), **preview_kwargs
         )
     except UnsupportedMimeType:
         temp_filepath.unlink()
```

### Comparing `caluma_alexandria-1.2.0/alexandria/core/validation.py` & `caluma_alexandria-2.0.0/alexandria/core/validation.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/core/views.py` & `caluma_alexandria-2.0.0/alexandria/core/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             queryset = self.filter_queryset(self.get_queryset())
         except DjangoCoreValidationError as exp:
             raise ValidationError(*exp.messages)
 
         try:
             if not queryset:
                 raise NotFound()
-        except DjangoCoreValidationError:
+        except DjangoCoreValidationError:  # pragma: todo cover
             raise ValidationError(
                 _(
                     'The "files" filter must consist of a comma delimited list of '
                     "File PKs!"
                 )
             )
 
@@ -138,26 +138,26 @@
             )
 
             return response
 
 
 @require_http_methods(["HEAD", "POST"])
 def hook_view(request):
-    if not settings.ENABLE_THUMBNAIL_GENERATION:
+    if not settings.ALEXANDRIA_ENABLE_THUMBNAIL_GENERATION:
         return HttpResponse(status=HTTP_403_FORBIDDEN)
 
     if request.method == "HEAD":
         return HttpResponse(status=HTTP_200_OK)
 
     data = json.loads(request.body.decode("utf-8"))
 
     response_statuses = []
     for record in data["Records"]:
         bucket_name = record["s3"]["bucket"]["name"]
-        if not bucket_name == settings.MINIO_STORAGE_MEDIA_BUCKET_NAME:
+        if not bucket_name == settings.ALEXANDRIA_MINIO_STORAGE_MEDIA_BUCKET_NAME:
             response_statuses.append(HTTP_200_OK)
             continue
 
         file_pk = record["s3"]["object"]["key"].split("_")[0]
         try:
             file = models.File.objects.get(pk=file_pk)
         except models.File.DoesNotExist:
```

### Comparing `caluma_alexandria-1.2.0/alexandria/core/visibilities.py` & `caluma_alexandria-2.0.0/alexandria/core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/oidc_auth/authentication.py` & `caluma_alexandria-2.0.0/alexandria/oidc_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/oidc_auth/models.py` & `caluma_alexandria-2.0.0/alexandria/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-1.2.0/alexandria/settings/django.py` & `caluma_alexandria-2.0.0/alexandria/settings/django.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,17 +118,19 @@
 }
 
 JSON_API_FORMAT_FIELD_NAMES = "dasherize"
 JSON_API_FORMAT_TYPES = "dasherize"
 JSON_API_PLURALIZE_TYPES = True
 
 # Anonymous writing
-ALLOW_ANONYMOUS_WRITE = env.bool("ALLOW_ANONYMOUS_WRITE", default=False)
+ALEXANDRIA_ALLOW_ANONYMOUS_WRITE = env.bool(
+    "ALEXANDRIA_ALLOW_ANONYMOUS_WRITE", default=False
+)
 
-if ALLOW_ANONYMOUS_WRITE:
+if ALEXANDRIA_ALLOW_ANONYMOUS_WRITE:
     REST_FRAMEWORK["DEFAULT_PERMISSION_CLASSES"] = [
         "rest_framework.permissions.AllowAny",
     ]
 
 
 def parse_admins(admins):
     """
```

### Comparing `caluma_alexandria-1.2.0/pyproject.toml` & `caluma_alexandria-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma-alexandria"
-version = "1.2.0"
+version = "2.0.0"
 description = "Document management service"
 repository = "https://github.com/projectcaluma/alexandria"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -29,45 +29,44 @@
 django-localized-fields = "^6.6"
 djangorestframework = "^3.13.0"
 djangorestframework-jsonapi = ">=5.0.0,<7.0.0"
 minio = "^7.1.14"
 mozilla-django-oidc = "^2.0.0"
 preview-generator = "^0.29"
 psycopg2-binary = "~2.9"
-requests = "^2.28.0"
+requests = "^2.31.0"
 uwsgi = "^2.0.20"
-vtk = "^9.2.6"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3.0"
-django_extensions = "^3.2.1"
-factory-boy = "^3.2.1"
-flake8 = "^6.0.0"
-flake8-blind-except = "^0.2.1"
-flake8-debugger = "^4.1.2"
-flake8-docstrings = "^1.7.0"
-flake8-isort = "^6.0.0"
-flake8-string-format = "^0.3.0"
-flake8-tuple = "^0.4.1"
-gitlint = "^0.19.1"
-isort = "^5.12.0"
-pdbpp = "^0.10.3"
-pre_commit = "^3.2.2"
-pytest-cov = "^4.0.0"
-pytest-django = "^4.5.2"
-pytest-env = "^0.8.1"
-pytest-factoryboy = "^2.5.1"
-pytest-freezegun = "^0.4.2"
-pytest-mock = "^3.10.0"
-pytest-randomly = "^3.12.0"
-requests-mock = "^1.10.0"
-snapshottest = "^0.6.0"
-werkzeug = "^2.3.0"
-python-semantic-release = "^7.33.3"
-pytest = "^7.3.1"
+black = "23.7.0"
+django-extensions = "3.2.3"
+factory-boy = "3.3.0"
+flake8 = "6.1.0"
+flake8-blind-except = "0.2.1"
+flake8-debugger = "4.1.2"
+flake8-docstrings = "1.7.0"
+flake8-isort = "6.0.0"
+flake8-string-format = "0.3.0"
+flake8-tuple = "0.4.1"
+gitlint = "0.19.1"
+isort = "5.12.0"
+pdbpp = "0.10.3"
+pre-commit = "3.3.3"
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
+pytest-django = "4.5.2"
+pytest-env = "0.8.2"
+pytest-factoryboy = "2.5.1"
+pytest-freezegun = "0.4.2"
+pytest-mock = "3.11.1"
+pytest-randomly = "3.13.0"
+python-semantic-release = "7.33.3"
+requests-mock = "1.11.0"
+snapshottest = "0.6.0"
+werkzeug = "2.3.6"
 
 
 [tool.isort]
 skip = [
     "migrations",
     "snapshots",
 ]
@@ -93,33 +92,30 @@
     "OIDC_OP_INTROSPECT_ENDPOINT=mock://alexandria.github.com/openid/introspect",
     "OIDC_BEARER_TOKEN_REVALIDATION_TIME=60",
 ]
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 
-[coverage.run]
+[tool.coverage.run]
 source = ["."]
 
-[coverage.report]
+[tool.coverage.report]
 fail_under = 100
 exclude_lines = [
     "pragma: no cover",
     "pragma: todo cover",
     "def __str__",
     "def __unicode__",
     "def __repr__",
 ]
 omit = [
     "*/migrations/*",
     "*/apps.py",
     "manage.py",
-    "setup.py",
-    "alexandria/settings_*.py",
     "alexandria/wsgi.py",
-    "alexandria/alexandria_metadata.py",
 ]
 show_missing = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `caluma_alexandria-1.2.0/setup.py` & `caluma_alexandria-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: caluma-alexandria
+Version: 2.0.0
+Summary: Document management service
+Home-page: https://github.com/projectcaluma/alexandria
+License: GPL-3.0-or-later
+Author: Caluma
+Author-email: info@caluma.io
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: django (>=3.2,<3.3)
+Requires-Dist: django-environ (>=0.9.0,<0.11.0)
+Requires-Dist: django-filter (>=22.1,<24.0)
+Requires-Dist: django-localized-fields (>=6.6,<7.0)
+Requires-Dist: djangorestframework (>=3.13.0,<4.0.0)
+Requires-Dist: djangorestframework-jsonapi (>=5.0.0,<7.0.0)
+Requires-Dist: minio (>=7.1.14,<8.0.0)
+Requires-Dist: mozilla-django-oidc (>=2.0.0,<3.0.0)
+Requires-Dist: preview-generator (>=0.29,<0.30)
+Requires-Dist: psycopg2-binary (>=2.9,<2.10)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: uwsgi (>=2.0.20,<3.0.0)
+Project-URL: Repository, https://github.com/projectcaluma/alexandria
+Description-Content-Type: text/markdown
+
+# alexandria
+
+[![Build Status](https://github.com/projectcaluma/emeis/workflows/Tests/badge.svg)](https://github.com/projectcaluma/emeis/actions?query=workflow%3ATests)
+[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/projectcaluma/emeis/blob/master/setup.cfg#L50)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/projectcaluma/alexandria)
+[![License: GPL-3.0-or-later](https://img.shields.io/github/license/projectcaluma/emeis)](https://spdx.org/licenses/GPL-3.0-or-later.html)
+
+Our goal is to implement an external document management service to hold and provide uploaded documents.
+Documents can be uploaded and, depending on user access, managed by internal as well as external users.
+
+The goal is NOT to re implement a complex [DMS](https://en.wikipedia.org/wiki/Document_management_system) but rather to have a simple and user-friendly way of managing documents with different permissions.
+
+All User Interface interactions should be as simple as possible and easily understandable.
+
+[Original RFC that led to alexandria](docs/original_alexandria_rfc.md)
+
+## Getting started
+
+### Installation
+
+**Requirements**
+
+- docker
+- docker-compose
+
+After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/projectcaluma/alexandria/master/docker-compose.yml) and run the following commands:
+
+```bash
+# only needs to be run once
+echo UID=$UID > .env
+
+docker compose up -d
+```
+
+You can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/).
+
+### Example data
+
+To load a set of categories run the following command:
+
+```bash
+make load_example_data
+```
+
+### Configuration
+
+Document Merge Service is a [12factor app](https://12factor.net/) which means that configuration is stored in environment variables.
+Different environment variable types are explained at [django-environ](https://github.com/joke2k/django-environ#supported-types).
+
+#### Common
+
+A list of configuration options which you need
+
+- Django configuration
+  - `SECRET_KEY`: A secret key used for cryptography. This needs to be a random string of a certain length. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-SECRET_KEY).
+  - `ALLOWED_HOSTS`: A list of hosts/domains your service will be served from. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#allowed-hosts).
+  - `DATABASE_ENGINE`: Database backend to use. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-DATABASE-ENGINE). (default: django.db.backends.postgresql)
+  - `DATABASE_HOST`: Host to use when connecting to database (default: localhost)
+  - `DATABASE_PORT`: Port to use when connecting to database (default: 5432)
+  - `DATABASE_NAME`: Name of database to use (default: alexandria)
+  - `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)
+  - `DATABASE_PASSWORD`: Password to use when connecting to database
+- Authentication configuration
+  - `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC
+  - `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development
+  - `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own
+  - `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
+  - `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
+  - `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
+- Authorization configurations
+  - `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models
+  - `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models
+- Data validation configuration
+  - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)
+
+For development, you can also set the following environemnt variables to help
+you:
+
+- `ALEXANDRIA_DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.
+- `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.
 
-packages = \
-['alexandria',
- 'alexandria.core',
- 'alexandria.core.migrations',
- 'alexandria.oidc_auth',
- 'alexandria.settings']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['django-environ>=0.9.0,<0.11.0',
- 'django-filter>=22.1,<24.0',
- 'django-localized-fields>=6.6,<7.0',
- 'django>=3.2,<3.3',
- 'djangorestframework-jsonapi>=5.0.0,<7.0.0',
- 'djangorestframework>=3.13.0,<4.0.0',
- 'minio>=7.1.14,<8.0.0',
- 'mozilla-django-oidc>=2.0.0,<3.0.0',
- 'preview-generator>=0.29,<0.30',
- 'psycopg2-binary>=2.9,<2.10',
- 'requests>=2.28.0,<3.0.0',
- 'uwsgi>=2.0.20,<3.0.0',
- 'vtk>=9.2.6,<10.0.0']
-
-setup_kwargs = {
-    'name': 'caluma-alexandria',
-    'version': '1.2.0',
-    'description': 'Document management service',
-    'long_description': '# alexandria\n\n[![Build Status](https://github.com/projectcaluma/emeis/workflows/Tests/badge.svg)](https://github.com/projectcaluma/emeis/actions?query=workflow%3ATests)\n[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/projectcaluma/emeis/blob/master/setup.cfg#L50)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/projectcaluma/alexandria)\n[![License: GPL-3.0-or-later](https://img.shields.io/github/license/projectcaluma/emeis)](https://spdx.org/licenses/GPL-3.0-or-later.html)\n\nOur goal is to implement an external document management service to hold and provide uploaded documents.\nDocuments can be uploaded and, depending on user access, managed by internal as well as external users.\n\nThe goal is NOT to re implement a complex [DMS](https://en.wikipedia.org/wiki/Document_management_system) but rather to have a simple and user-friendly way of managing documents with different permissions.\n\nAll User Interface interactions should be as simple as possible and easily understandable.\n\n[Original RFC that led to alexandria](docs/original_alexandria_rfc.md)\n\n## Getting started\n\n### Installation\n\n**Requirements**\n* docker\n* docker-compose\n\nAfter installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/projectcaluma/alexandria/master/docker-compose.yml) and run the following commands:\n\n```bash\n# only needs to be run once\necho UID=$UID > .env\n\ndocker-compose up -d\n```\n\nYou can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/).\n\n### Example data\n\nTo load a set of categories run the following command:\n```bash\nmake load_example_data\n```\n\n### Configuration\n\nDocument Merge Service is a [12factor app](https://12factor.net/) which means that configuration is stored in environment variables.\nDifferent environment variable types are explained at [django-environ](https://github.com/joke2k/django-environ#supported-types).\n\n#### Common\n\nA list of configuration options which you need\n\n* Django configuration\n  * `SECRET_KEY`: A secret key used for cryptography. This needs to be a random string of a certain length. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-SECRET_KEY).\n  * `ALLOWED_HOSTS`: A list of hosts/domains your service will be served from. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#allowed-hosts).\n  * `DATABASE_ENGINE`: Database backend to use. See [more](https://docs.djangoproject.com/en/2.1/ref/settings/#std:setting-DATABASE-ENGINE). (default: django.db.backends.postgresql)\n  * `DATABASE_HOST`: Host to use when connecting to database (default: localhost)\n  * `DATABASE_PORT`: Port to use when connecting to database (default: 5432)\n  * `DATABASE_NAME`: Name of database to use (default: alexandria)\n  * `DATABASE_USER`: Username to use when connecting to the database (default: alexandria)\n  * `DATABASE_PASSWORD`: Password to use when connecting to database\n* Authentication configuration\n  * `OIDC_OP_USER_ENDPOINT`: Userinfo endpoint for OIDC\n  * `OIDC_VERIFY_SSL`: Set to `false` if you want to disable verifying SSL certs. Useful for development\n  * `OIDC_DRF_AUTH_BACKEND`: Overwrite the default authentication backend with your own\n  * `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own\n  * `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)\n  * `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)\n* Authorization configurations\n  * `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of classes that define visibility for all models\n  * `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of classes that define permissions for all models\n* Data validation configuration\n  * `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of classes that define [custom validations](docs/validation.md)\n\nFor development, you can also set the following environemnt variables to help\nyou:\n\n  * `DEV_AUTH_BACKEND`: Set this to "true" to enable a fake auth backend that simulates an authenticated user. Requires `DEBUG` to be set to `True` as well.\n  * `DEBUG`: Set this to true for debugging during development. Never enable this in production, as it **will** leak information to the public if you do.\n\n## Contributing\n\nLook at our [contributing guidelines](CONTRIBUTING.md) to start with your first contribution.\n\n## Maintainer\'s Handbook\n\nSome notes for maintaining this project can be found in [the maintainer\'s handbook](MAINTAINING.md).',
-    'author': 'Caluma',
-    'author_email': 'info@caluma.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/projectcaluma/alexandria',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+## Contributing
 
+Look at our [contributing guidelines](CONTRIBUTING.md) to start with your first contribution.
+
+## Maintainer's Handbook
+
+Some notes for maintaining this project can be found in [the maintainer's handbook](MAINTAINING.md).
 
-setup(**setup_kwargs)
```

