# Comparing `tmp/fastapi_user_auth-0.4.3.tar.gz` & `tmp/fastapi_user_auth-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_auth-0.4.3.tar", last modified: Mon Feb 13 08:53:06 2023, max compression
+gzip compressed data, was "fastapi_user_auth-0.5.0.tar", last modified: Sat Mar  4 15:50:02 2023, max compression
```

## Comparing `fastapi_user_auth-0.4.3.tar` & `fastapi_user_auth-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,35 @@
--rw-r--r--   0        0        0    11512 2022-10-18 06:03:57.961995 fastapi_user_auth-0.4.3/README.md
--rw-r--r--   0        0        0      358 2023-02-13 08:51:29.983202 fastapi_user_auth-0.4.3/fastapi_user_auth/__init__.py
--rw-r--r--   0        0        0    11705 2023-02-13 08:22:41.955097 fastapi_user_auth-0.4.3/fastapi_user_auth/admin.py
--rw-r--r--   0        0        0     3388 2023-02-13 08:41:13.510777 fastapi_user_auth-0.4.3/fastapi_user_auth/app.py
--rw-r--r--   0        0        0      119 2022-03-06 13:25:37.443534 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/__init__.py
--rw-r--r--   0        0        0    13440 2022-12-13 07:23:25.965695 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/auth.py
--rw-r--r--   0        0        0        0 2022-02-12 07:35:52.020000 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/__init__.py
--rw-r--r--   0        0        0      859 2022-09-23 13:13:16.799514 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/base.py
--rw-r--r--   0        0        0     2027 2022-11-01 03:13:24.339154 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/db.py
--rw-r--r--   0        0        0     1355 2022-11-01 03:13:24.341156 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/jwt.py
--rw-r--r--   0        0        0     1181 2022-09-23 13:13:16.810508 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/redis.py
--rw-r--r--   0        0        0     9332 2022-11-02 04:19:50.146932 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/models.py
--rw-r--r--   0        0        0      835 2022-09-23 13:13:16.814506 fastapi_user_auth-0.4.3/fastapi_user_auth/auth/schemas.py
--rw-r--r--   0        0        0     2370 2022-09-29 08:02:18.025487 fastapi_user_auth-0.4.3/fastapi_user_auth/locale/base.pot
--rw-r--r--   0        0        0     1902 2022-10-01 13:19:38.916990 fastapi_user_auth-0.4.3/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3101 2022-10-01 13:19:38.917998 fastapi_user_auth-0.4.3/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     2727 2022-10-01 13:19:38.985019 fastapi_user_auth-0.4.3/fastapi_user_auth/site.py
--rw-r--r--   0        0        0     2478 2022-11-16 09:28:26.287076 fastapi_user_auth-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    13416 1970-01-01 00:00:00.000000 fastapi_user_auth-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       98 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.flake8
+-rw-r--r--   0        0        0     1662 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      977 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2070 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.gitignore
+-rw-r--r--   0        0        0      326 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11157 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/README.md
+-rw-r--r--   0        0        0    10288 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/README.zh.md
+-rw-r--r--   0        0        0      345 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/__init__.py
+-rw-r--r--   0        0        0    11465 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/admin.py
+-rw-r--r--   0        0        0     3390 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/app.py
+-rw-r--r--   0        0        0      119 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/__init__.py
+-rw-r--r--   0        0        0    12985 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/auth.py
+-rw-r--r--   0        0        0        0 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/__init__.py
+-rw-r--r--   0        0        0      837 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/base.py
+-rw-r--r--   0        0        0     1976 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/db.py
+-rw-r--r--   0        0        0     1319 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/jwt.py
+-rw-r--r--   0        0        0     1151 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/redis.py
+-rw-r--r--   0        0        0     9027 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/models.py
+-rw-r--r--   0        0        0      805 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/schemas.py
+-rw-r--r--   0        0        0     1902 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2949 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     2729 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/site.py
+-rw-r--r--   0        0        0   177210 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/pdm.lock
+-rw-r--r--   0        0        0     2380 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1137 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/__init__.py
+-rw-r--r--   0        0        0     4909 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/conftest.py
+-rw-r--r--   0        0        0      812 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth.py
+-rw-r--r--   0        0        0     1372 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_mount.py
+-rw-r--r--   0        0        0     6711 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_requires.py
+-rw-r--r--   0        0        0      945 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_router.py
+-rw-r--r--   0        0        0     1241 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_user_model.py
+-rw-r--r--   0        0        0     1102 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_backend.py
+-rw-r--r--   0        0        0    13416 1970-01-01 00:00:00.000000 fastapi_user_auth-0.5.0/PKG-INFO
```

### Comparing `fastapi_user_auth-0.4.3/README.md` & `fastapi_user_auth-0.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,355 +1,354 @@
-[简体中文](https://github.com/amisadmin/fastapi_user_auth/blob/master/README.zh.md)
-| [English](https://github.com/amisadmin/fastapi_user_auth)
-
-# Project Introduction
-
-<h2 align="center">
-  FastAPI-User-Auth
-</h2>
-<p align="center">
-    <em>FastAPI-User-Auth is a simple and powerful FastAPI user RBAC authentication and authorization library.</em><br/>
-    <em>It is based on FastAPI-Amis-Admin and provides a freely extensible visual management interface.</em>
-</p>
-<p align="center">
-    <a href="https://github.com/amisadmin/fastapi_amis_admin/actions/workflows/pytest.yml" target="_blank">
-        <img src="https://github.com/amisadmin/fastapi_amis_admin/actions/workflows/pytest.yml/badge.svg" alt="Pytest">
-    </a>
-    <a href="https://pypi.org/project/fastapi_user_auth" target="_blank">
-        <img src="https://badgen.net/pypi/v/fastapi-user-auth?color=blue" alt="Package version">
-    </a>
-    <a href="https://pepy.tech/project/fastapi-user-auth" target="_blank">
-        <img src="https://pepy.tech/badge/fastapi-user-auth" alt="Downloads">
-    </a>
-    <a href="https://gitter.im/amisadmin/fastapi-amis-admin">
-        <img src="https://badges.gitter.im/amisadmin/fastapi-amis-admin.svg" alt="Chat on Gitter"/>
-    </a>
-    <a href="https://jq.qq.com/?_wv=1027&k=U4Dv6x8W" target="_blank">
-        <img src="https://badgen.net/badge/qq%E7%BE%A4/229036692/orange" alt="229036692">
-    </a>
-</p>
-<p align="center">
-  <a href="https://github.com/amisadmin/fastapi_user_auth" target="_blank">SourceCode</a>
-  ·
-  <a href="http://user-auth.demo.amis.work/" target="_blank">OnlineDemo</a>
-  ·
-  <a href="http://docs.amis.work" target="_blank">Documentation</a>
-  ·
-  <a href="http://docs.gh.amis.work" target="_blank">Can't open the document？</a>
-</p>
-
-------
-
-`FastAPI-User-Auth` It is an application plug -in based on [FastAPI-Amis-Admin](https://github.com/amisadmin/fastapi_amis_admin)
-, which is deeply integrated to provide user authentication and authorization..
-
-## Install
-
-```bash
-pip install fastapi-user-auth
-```
-
-## Simple example
-
-```python
-from fastapi import FastAPI
-from fastapi_amis_admin.admin.settings import Settings
-from fastapi_user_auth.site import AuthAdminSite
-from starlette.requests import Request
-from sqlmodel import SQLModel
-
-# Create Fast API application
-app = FastAPI()
-
-# Create an Admin Site instance
-site = AuthAdminSite(settings=Settings(database_url_async='sqlite+aiosqlite:///amisadmin.db'))
-auth = site.auth
-# Mount the Site management system to the FastAPI instance
-site.mount_app(app)
-
-# Create initialization database table
-@app.on_event("startup")
-async def startup():
-    await site.db.async_run_sync(SQLModel.metadata.create_all, is_session=False)
-    # Create default test user, Please change your password in time!!!
-    await auth.create_role_user('admin')
-    await auth.create_role_user('vip')
-
-# Requirements: User must be logged in
-@app.get("/auth/get_user")
-@auth.requires()
-def get_user(request: Request):
-    return request.user
-
-if __name__ == '__main__':
-    import uvicorn
-
-    uvicorn.run(app, debug=True)
-
-```
-
-## Ways of identifying
-
-### Decorator
-
-- Recommended scenario: Single route. Supports synchronous and asynchronous routing.
-
-```python
-# Requirements: User must be logged in
-@app.get("/auth/user")
-@auth.requires()
-def user(request: Request):
-    return request.user  # current request user object.
-
-# Authentication route: user has admin role
-@app.get("/auth/admin_roles")
-@auth.requires('admin')
-def admin_roles(request: Request):
-    return request.user
-
-# Requirement: User has vip role
-# Support synchronous and asynchronous routing
-@app.get("/auth/vip_roles")
-@auth.requires(['vip'])
-async def vip_roles(request: Request):
-    return request.user
-
-# Requirements: User has admin role or vip role
-@app.get("/auth/admin_or_vip_roles")
-@auth.requires(roles=['admin', 'vip'])
-def admin_or_vip_roles(request: Request):
-    return request.user
-
-# Requirement: The user belongs to the admin user group
-@app.get("/auth/admin_groups")
-@auth.requires(groups=['admin'])
-def admin_groups(request: Request):
-    return request.user
-
-# Requirements: The user has the admin role and belongs to the admin user group
-@app.get("/auth/admin_roles_and_admin_groups")
-@auth.requires(roles=['admin'], groups=['admin'])
-def admin_roles_and_admin_groups(request: Request):
-    return request.user
-
-# Requirements: The user has the vip role and has the `article:update` permission
-@app.get("/auth/vip_roles_and_article_update")
-@auth.requires(roles=['vip'], permissions=['article:update'])
-def vip_roles_and_article_update(request: Request):
-    return request.user
-
-```
-
-### Dependencies (recommended)
-
-- Recommended scenarios: single route, route collection, FastAPI application.
-
-```python
-from fastapi import Depends
-from typing import Tuple
-from fastapi_user_auth.auth import Auth
-from fastapi_user_auth.auth.models import User
-
-# Route parameter dependencies, this method is recommended
-@app.get("/auth/admin_roles_depend_1")
-def admin_roles(user: User = Depends(auth.get_current_user)):
-    return user  # or request.user
-
-# Path manipulation decorator dependencies
-@app.get("/auth/admin_roles_depend_2", dependencies=[Depends(auth.requires('admin')())])
-def admin_roles(request: Request):
-    return request.user
-
-# Global dependencies
-# All requests under the app application require the admin role
-app = FastAPI(dependencies=[Depends(auth.requires('admin')())])
-
-@app.get("/auth/admin_roles_depend_3")
-def admin_roles(request: Request):
-    return request.user
-
-```
-
-### Middleware
-
-- Recommended Scenario: FastAPI Application
-
-```python
-app = FastAPI()
-# Append `request.auth` and `request.user` objects before each request processing under the app
-auth.backend.attach_middleware(app)
-
-```
-
-### Call directly
-
-- Recommended scenarios: non-routing methods
-
-```python
-from fastapi_user_auth.auth.models import User
-
-async def get_request_user(request: Request) -> Optional[User]:
-    # user= await auth.get_current_user(request)
-    if await auth.requires('admin', response=False)(request):
-        return request.user
-    else:
-        return None
-
-```
-
-## Token storage backend
-
-`fastapi-user-auth` Supports multiple token storage methods. The default is: `DbTokenStore`, It is recommended to customize the modification to: `JwtTokenStore`
-
-### JwtTokenStore
-
-```python
-from fastapi_user_auth.auth.backends.jwt import JwtTokenStore
-from sqlalchemy.ext.asyncio import create_async_engine
-from sqlalchemy_database import AsyncDatabase
-
-# Create an asynchronous database engine
-engine = create_async_engine(url='sqlite+aiosqlite:///amisadmin.db', future=True)
-# Create auth object using `Jwt Token Store`
-auth = Auth(
-    db=AsyncDatabase(engine),
-    token_store=JwtTokenStore(secret_key='09d25e094faa6ca2556c818166b7a9563b93f7099f6f0f4caa6cf63b88e8d3e7')
-)
-
-# Pass the auth object into the Admin Site
-site = AuthAdminSite(
-    settings=Settings(database_url_async='sqlite+aiosqlite:///amisadmin.db'),
-    auth=auth
-)
-
-```
-
-### DbTokenStore
-
-```python
-# Create auth object using `Db Token Store`
-from fastapi_user_auth.auth.backends.db import DbTokenStore
-
-auth = Auth(
-    db=AsyncDatabase(engine),
-    token_store=DbTokenStore(db=AsyncDatabase(engine))
-)
-```
-
-### RedisTokenStore
-
-```python
-# Create auth object using `Redis Token Store`
-from fastapi_user_auth.auth.backends.redis import RedisTokenStore
-from aioredis import Redis
-
-auth = Auth(
-    db=AsyncDatabase(engine),
-    token_store=RedisTokenStore(redis=Redis.from_url('redis://localhost?db=0'))
-)
-```
-
-## RBAC model
-
-The `RBAC` model adopted by this system is as follows, you can also expand it according to your own needs.
-
-- Reference: [Design of Permission System](https://blog.csdn.net/qq_25889465/article/details/98473611)
-
-```mermaid
-flowchart LR
-	 User -. m:n .-> Group 
-	 User -. m:n .-> Role 
-     Group -. m:n .-> Role 
-	 Role -. m:n .-> Perimission 
-```
-
-## Advanced Extension
-
-```bash
-### Extending the `User` model
-
-```python
-from datetime import date
-
-from fastapi_amis_admin.models.fields import Field
-from fastapi_user_auth.auth.models import User
-
-# Customize `User` model, inherit `User`
-class MyUser(User, table = True):
-    point: float = Field(default = 0, title = 'Source', description = 'User source')
-    phone: str = Field(None, title = 'Phone number', max_length = 15)
-    parent_id: int = Field(None, title = "Superior", foreign_key = "auth_user.id")
-    birthday: date = Field(None, title = "Date of birth")
-    location: str = Field(None, title = "Location")
-
-# Create an auth object using a custom `User` model
-auth = Auth(db = AsyncDatabase(engine), user_model = MyUser)
-```
-
-### Extend the `Role`, `Group`, `Permission` models
-
-```python
-from fastapi_amis_admin.models.fields import Field
-from fastapi_user_auth.auth.models import Group
-
-# Customize the `Group` model, inherit `Base RBAC`; override the `Role`, the `Permission` model is similar, 
-# the difference is the table name.
-class MyGroup(Group, table=True):
-    __tablename__ = 'auth_group'  # Database table name, must be this to override the default model
-    icon: str = Field(None, title='Icon')
-    is_active: bool = Field(default=True, title="Activate now")
-
-```
-
-### Custom `User Auth App` default management class
-
-Default management classes can be overridden and replaced by inheritance.
-For Example: `UserLoginFormAdmin`,`UserRegFormAdmin`,`UserInfoFormAdmin`,
-`UserAdmin`,`GroupAdmin`,`RoleAdmin`,`PermissionAdmin`
-
-```python
-# Customize the model management class, inherit and override the corresponding default management class
-class MyGroupAdmin(admin.ModelAdmin):
-    group_schema = None
-    page_schema = PageSchema(label='用户组管理', icon='fa fa-group')
-    model = MyGroup
-    link_model_fields = [Group.roles]
-    readonly_fields = ['key']
-
-# Customize the user authentication application, inherit and override the default user authentication application
-class MyUserAuthApp(UserAuthApp):
-    GroupAdmin = MyGroupAdmin
-
-# Customize the user management site, inherit and override the default user management site
-class MyAuthAdminSite(AuthAdminSite):
-    UserAuthApp = MyUserAuthApp
-
-# Create a site object using a custom `Auth Admin Site` class
-site = MyAuthAdminSite(settings, auth=auth)
-```
-
-## Interface/UI preview
-
-- Open `http://127.0.0.1:8000/admin/auth/form/login` in your browser:
-
-![Login](https://s2.loli.net/2022/03/20/SZy6sjaVlBT8gin.png)
-
-- Open `http://127.0.0.1:8000/admin/` in your browser:
-
-![ModelAdmin](https://s2.loli.net/2022/03/20/ItgFYGUONm1jCz5.png)
-
-- Open `http://127.0.0.1:8000/admin/docs` in your browser:
-
-![Docs](https://s2.loli.net/2022/03/20/1GcCiPdmXayxrbH.png)
-
-## License
-
-- `fastapi-amis-admin` is based on `Apache2.0` Open source is free to use and can be freely used for commercial purposes, but please clearly display the copyright information about Fast API-Amis-Admin in the display interface.
-
-## Thanks
-
-Thanks to the following developers for their contributions to FastAPI-User-Auth:
-
-<a href="https://github.com/amisadmin/fastapi_user_auth/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=amisadmin/fastapi_user_auth"  alt=""/>
-</a>
-
+[简体中文](https://github.com/amisadmin/fastapi_user_auth/blob/master/README.zh.md)
+| [English](https://github.com/amisadmin/fastapi_user_auth)
+
+# Project Introduction
+
+<h2 align="center">
+  FastAPI-User-Auth
+</h2>
+<p align="center">
+    <em>FastAPI-User-Auth is a simple and powerful FastAPI user RBAC authentication and authorization library.</em><br/>
+    <em>It is based on FastAPI-Amis-Admin and provides a freely extensible visual management interface.</em>
+</p>
+<p align="center">
+    <a href="https://github.com/amisadmin/fastapi_amis_admin/actions/workflows/pytest.yml" target="_blank">
+        <img src="https://github.com/amisadmin/fastapi_amis_admin/actions/workflows/pytest.yml/badge.svg" alt="Pytest">
+    </a>
+    <a href="https://pypi.org/project/fastapi_user_auth" target="_blank">
+        <img src="https://badgen.net/pypi/v/fastapi-user-auth?color=blue" alt="Package version">
+    </a>
+    <a href="https://pepy.tech/project/fastapi-user-auth" target="_blank">
+        <img src="https://pepy.tech/badge/fastapi-user-auth" alt="Downloads">
+    </a>
+    <a href="https://gitter.im/amisadmin/fastapi-amis-admin">
+        <img src="https://badges.gitter.im/amisadmin/fastapi-amis-admin.svg" alt="Chat on Gitter"/>
+    </a>
+    <a href="https://jq.qq.com/?_wv=1027&k=U4Dv6x8W" target="_blank">
+        <img src="https://badgen.net/badge/qq%E7%BE%A4/229036692/orange" alt="229036692">
+    </a>
+</p>
+<p align="center">
+  <a href="https://github.com/amisadmin/fastapi_user_auth" target="_blank">SourceCode</a>
+  ·
+  <a href="http://user-auth.demo.amis.work/" target="_blank">OnlineDemo</a>
+  ·
+  <a href="http://docs.amis.work" target="_blank">Documentation</a>
+  ·
+  <a href="http://docs.gh.amis.work" target="_blank">Can't open the document？</a>
+</p>
+
+------
+
+`FastAPI-User-Auth` It is an application plug -in based on [FastAPI-Amis-Admin](https://github.com/amisadmin/fastapi_amis_admin)
+, which is deeply integrated to provide user authentication and authorization..
+
+## Install
+
+```bash
+pip install fastapi-user-auth
+```
+
+## Simple example
+
+```python
+from fastapi import FastAPI
+from fastapi_amis_admin.admin.settings import Settings
+from fastapi_user_auth.site import AuthAdminSite
+from starlette.requests import Request
+from sqlmodel import SQLModel
+
+# Create Fast API application
+app = FastAPI()
+
+# Create an Admin Site instance
+site = AuthAdminSite(settings=Settings(database_url_async='sqlite+aiosqlite:///amisadmin.db'))
+auth = site.auth
+# Mount the Site management system to the FastAPI instance
+site.mount_app(app)
+
+# Create initialization database table
+@app.on_event("startup")
+async def startup():
+    await site.db.async_run_sync(SQLModel.metadata.create_all, is_session=False)
+    # Create default admin user,user name:admin,password:admin,please change it after login!!!
+    await auth.create_role_user('admin')
+    await auth.create_role_user('vip')
+
+# Requirements: User must be logged in
+@app.get("/auth/get_user")
+@auth.requires()
+def get_user(request: Request):
+    return request.user
+
+if __name__ == '__main__':
+    import uvicorn
+
+    uvicorn.run(app, debug=True)
+
+```
+
+## Ways of identifying
+
+### Decorator
+
+- Recommended scenario: Single route. Supports synchronous and asynchronous routing.
+
+```python
+# Requirements: User must be logged in
+@app.get("/auth/user")
+@auth.requires()
+def user(request: Request):
+    return request.user  # current request user object.
+
+# Authentication route: user has admin role
+@app.get("/auth/admin_roles")
+@auth.requires('admin')
+def admin_roles(request: Request):
+    return request.user
+
+# Requirement: User has vip role
+# Support synchronous and asynchronous routing
+@app.get("/auth/vip_roles")
+@auth.requires(['vip'])
+async def vip_roles(request: Request):
+    return request.user
+
+# Requirements: User has admin role or vip role
+@app.get("/auth/admin_or_vip_roles")
+@auth.requires(roles=['admin', 'vip'])
+def admin_or_vip_roles(request: Request):
+    return request.user
+
+# Requirement: The user belongs to the admin user group
+@app.get("/auth/admin_groups")
+@auth.requires(groups=['admin'])
+def admin_groups(request: Request):
+    return request.user
+
+# Requirements: The user has the admin role and belongs to the admin user group
+@app.get("/auth/admin_roles_and_admin_groups")
+@auth.requires(roles=['admin'], groups=['admin'])
+def admin_roles_and_admin_groups(request: Request):
+    return request.user
+
+# Requirements: The user has the vip role and has the `article:update` permission
+@app.get("/auth/vip_roles_and_article_update")
+@auth.requires(roles=['vip'], permissions=['article:update'])
+def vip_roles_and_article_update(request: Request):
+    return request.user
+
+```
+
+### Dependencies (recommended)
+
+- Recommended scenarios: single route, route collection, FastAPI application.
+
+```python
+from fastapi import Depends
+from typing import Tuple
+from fastapi_user_auth.auth import Auth
+from fastapi_user_auth.auth.models import User
+
+# Route parameter dependencies, this method is recommended
+@app.get("/auth/admin_roles_depend_1")
+def admin_roles(user: User = Depends(auth.get_current_user)):
+    return user  # or request.user
+
+# Path manipulation decorator dependencies
+@app.get("/auth/admin_roles_depend_2", dependencies=[Depends(auth.requires('admin')())])
+def admin_roles(request: Request):
+    return request.user
+
+# Global dependencies
+# All requests under the app application require the admin role
+app = FastAPI(dependencies=[Depends(auth.requires('admin')())])
+
+@app.get("/auth/admin_roles_depend_3")
+def admin_roles(request: Request):
+    return request.user
+
+```
+
+### Middleware
+
+- Recommended Scenario: FastAPI Application
+
+```python
+app = FastAPI()
+# Append `request.auth` and `request.user` objects before each request processing under the app
+auth.backend.attach_middleware(app)
+
+```
+
+### Call directly
+
+- Recommended scenarios: non-routing methods
+
+```python
+from fastapi_user_auth.auth.models import User
+
+async def get_request_user(request: Request) -> Optional[User]:
+    # user= await auth.get_current_user(request)
+    if await auth.requires('admin', response=False)(request):
+        return request.user
+    else:
+        return None
+
+```
+
+## Token storage backend
+
+`fastapi-user-auth` Supports multiple token storage methods. The default is: `DbTokenStore`, It is recommended to customize the modification to: `JwtTokenStore`
+
+### JwtTokenStore
+
+```python
+from fastapi_user_auth.auth.backends.jwt import JwtTokenStore
+from sqlalchemy.ext.asyncio import create_async_engine
+from sqlalchemy_database import AsyncDatabase
+
+# Create an asynchronous database engine
+engine = create_async_engine(url='sqlite+aiosqlite:///amisadmin.db', future=True)
+# Create auth object using `Jwt Token Store`
+auth = Auth(
+    db=AsyncDatabase(engine),
+    token_store=JwtTokenStore(secret_key='09d25e094faa6ca2556c818166b7a9563b93f7099f6f0f4caa6cf63b88e8d3e7')
+)
+
+# Pass the auth object into the Admin Site
+site = AuthAdminSite(
+    settings=Settings(database_url_async='sqlite+aiosqlite:///amisadmin.db'),
+    auth=auth
+)
+
+```
+
+### DbTokenStore
+
+```python
+# Create auth object using `Db Token Store`
+from fastapi_user_auth.auth.backends.db import DbTokenStore
+
+auth = Auth(
+    db=AsyncDatabase(engine),
+    token_store=DbTokenStore(db=AsyncDatabase(engine))
+)
+```
+
+### RedisTokenStore
+
+```python
+# Create auth object using `Redis Token Store`
+from fastapi_user_auth.auth.backends.redis import RedisTokenStore
+from aioredis import Redis
+
+auth = Auth(
+    db=AsyncDatabase(engine),
+    token_store=RedisTokenStore(redis=Redis.from_url('redis://localhost?db=0'))
+)
+```
+
+## RBAC model
+
+The `RBAC` model adopted by this system is as follows, you can also expand it according to your own needs.
+
+- Reference: [Design of Permission System](https://blog.csdn.net/qq_25889465/article/details/98473611)
+
+```mermaid
+flowchart LR
+	 User -. m:n .-> Group 
+	 User -. m:n .-> Role 
+     Group -. m:n .-> Role 
+	 Role -. m:n .-> Perimission 
+```
+
+## Advanced Extension
+
+```bash
+### Extending the `User` model
+
+```python
+from datetime import date
+
+from fastapi_amis_admin.models.fields import Field
+from fastapi_user_auth.auth.models import User
+
+# Customize `User` model, inherit `User`
+class MyUser(User, table = True):
+    point: float = Field(default = 0, title = 'Source', description = 'User source')
+    phone: str = Field(None, title = 'Phone number', max_length = 15)
+    parent_id: int = Field(None, title = "Superior", foreign_key = "auth_user.id")
+    birthday: date = Field(None, title = "Date of birth")
+    location: str = Field(None, title = "Location")
+
+# Create an auth object using a custom `User` model
+auth = Auth(db = AsyncDatabase(engine), user_model = MyUser)
+```
+
+### Extend the `Role`, `Group`, `Permission` models
+
+```python
+from fastapi_amis_admin.models.fields import Field
+from fastapi_user_auth.auth.models import Group
+
+# Customize the `Group` model, inherit `Base RBAC`; override the `Role`, the `Permission` model is similar, 
+# the difference is the table name.
+class MyGroup(Group, table=True):
+    __tablename__ = 'auth_group'  # Database table name, must be this to override the default model
+    icon: str = Field(None, title='Icon')
+    is_active: bool = Field(default=True, title="Activate now")
+
+```
+
+### Custom `User Auth App` default management class
+
+Default management classes can be overridden and replaced by inheritance.
+For Example: `UserLoginFormAdmin`,`UserRegFormAdmin`,`UserInfoFormAdmin`,
+`UserAdmin`,`GroupAdmin`,`RoleAdmin`,`PermissionAdmin`
+
+```python
+# Customize the model management class, inherit and override the corresponding default management class
+class MyGroupAdmin(admin.ModelAdmin):
+    page_schema = PageSchema(label='用户组管理', icon='fa fa-group')
+    model = MyGroup
+    link_model_fields = [Group.roles]
+    readonly_fields = ['key']
+
+# Customize the user authentication application, inherit and override the default user authentication application
+class MyUserAuthApp(UserAuthApp):
+    GroupAdmin = MyGroupAdmin
+
+# Customize the user management site, inherit and override the default user management site
+class MyAuthAdminSite(AuthAdminSite):
+    UserAuthApp = MyUserAuthApp
+
+# Create a site object using a custom `Auth Admin Site` class
+site = MyAuthAdminSite(settings, auth=auth)
+```
+
+## Interface/UI preview
+
+- Open `http://127.0.0.1:8000/admin/auth/form/login` in your browser:
+
+![Login](https://s2.loli.net/2022/03/20/SZy6sjaVlBT8gin.png)
+
+- Open `http://127.0.0.1:8000/admin/` in your browser:
+
+![ModelAdmin](https://s2.loli.net/2022/03/20/ItgFYGUONm1jCz5.png)
+
+- Open `http://127.0.0.1:8000/admin/docs` in your browser:
+
+![Docs](https://s2.loli.net/2022/03/20/1GcCiPdmXayxrbH.png)
+
+## License
+
+- `fastapi-amis-admin` is based on `Apache2.0` Open source is free to use and can be freely used for commercial purposes, but please clearly display the copyright information about Fast API-Amis-Admin in the display interface.
+
+## Thanks
+
+Thanks to the following developers for their contributions to FastAPI-User-Auth:
+
+<a href="https://github.com/amisadmin/fastapi_user_auth/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=amisadmin/fastapi_user_auth"  alt=""/>
+</a>
+
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/admin.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,284 +1,279 @@
-import contextlib
-from typing import Any, Callable, Dict, List, Type
-
-from fastapi import Depends, HTTPException
-from fastapi_amis_admin.admin import FormAdmin, ModelAdmin
-from fastapi_amis_admin.amis.components import (
-    Action,
-    ActionType,
-    ButtonToolbar,
-    Form,
-    Grid,
-    Horizontal,
-    Html,
-    Page,
-    PageSchema,
-)
-from fastapi_amis_admin.amis.constants import DisplayModeEnum, LevelEnum
-from fastapi_amis_admin.crud.base import SchemaUpdateT
-from fastapi_amis_admin.crud.schema import BaseApiOut
-from fastapi_amis_admin.utils.translation import i18n as _
-from pydantic import BaseModel
-from sqlalchemy import select
-from starlette import status
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.routing import NoMatchFound
-
-from fastapi_user_auth.auth import Auth
-from fastapi_user_auth.auth.models import BaseUser, Group, Permission, Role, User
-from fastapi_user_auth.auth.schemas import UserLoginOut
-
-
-def attach_page_head(page: Page) -> Page:
-    desc = _("Amis is a low-code front-end framework that reduces page development effort and greatly improves efficiency")
-    page.body = [
-        Html(
-            html=f'<div style="display: flex; justify-content: center; align-items: center; margin: 96px 0px 8px;">'
-            f'<img src="https://baidu.gitee.io/amis/static/favicon_b3b0647.png" alt="logo" style="margin-right: 8px; '
-            f'width: 48px;"><span style="font-size: 32px; font-weight: bold;">Amis Admin</span></div>'
-            f'<div style="width: 100%; text-align: center; color: rgba(0, 0, 0, 0.45); margin-bottom: 40px;">{desc}</div>'
-        ),
-        Grid(columns=[{"body": [page.body], "lg": 2, "md": 4, "valign": "middle"}], align="center", valign="middle"),
-    ]
-    return page
-
-
-class UserLoginFormAdmin(FormAdmin):
-    page = Page(title=_("User Login"))
-    page_path = "/login"
-    page_parser_mode = "html"
-    schema: Type[SchemaUpdateT] = None
-    schema_submit_out: Type[UserLoginOut] = None
-    page_schema = None
-    page_route_kwargs = {"name": "login"}
-
-    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[BaseModel]:  # self.schema_submit_out
-        if request.user:
-            return BaseApiOut(code=1, msg=_("User logged in!"), data=self.schema_submit_out.parse_obj(request.user))
-        user = await request.auth.authenticate_user(username=data.username, password=data.password)  # type:ignore
-        if not user:
-            return BaseApiOut(status=-1, msg=_("Incorrect username or password!"))
-        if not user.is_active:
-            return BaseApiOut(status=-2, msg=_("Inactive user status!"))
-
-        token_info = self.schema_submit_out.parse_obj(user)
-        auth: Auth = request.auth
-        token_info.access_token = await auth.backend.token_store.write_token(user.dict())
-        return BaseApiOut(code=0, data=token_info)
-
-    @property
-    def route_submit(self):
-        async def route(response: Response, result: BaseApiOut = Depends(super().route_submit)):
-            if result.status == 0 and result.code == 0:  # 登录成功,设置用户信息
-                response.set_cookie("Authorization", f"bearer {result.data.access_token}")
-            return result
-
-        return route
-
-    async def get_form(self, request: Request) -> Form:
-        form = await super().get_form(request)
-        buttons = []
-        with contextlib.suppress(NoMatchFound):
-            buttons.append(
-                ActionType.Link(
-                    actionType="link",
-                    link=f"{self.site.router_path}{self.app.router.url_path_for('reg')}",
-                    label=_("Sign up"),
-                )
-            )
-        buttons.append(Action(actionType="submit", label=_("Sign in"), level=LevelEnum.primary))
-        form.body.sort(key=lambda form_item: form_item.type, reverse=True)
-        form.update_from_kwargs(
-            title="",
-            mode=DisplayModeEnum.horizontal,
-            submitText=_("Sign in"),
-            actionsClassName="no-border m-none p-none",
-            panelClassName="",
-            wrapWithPanel=True,
-            horizontal=Horizontal(left=3, right=9),
-            actions=[ButtonToolbar(buttons=buttons)],
-        )
-        form.redirect = request.query_params.get("redirect") or "/"
-        return form
-
-    async def get_page(self, request: Request) -> Page:
-        page = await super().get_page(request)
-        return attach_page_head(page)
-
-    @property
-    def route_page(self) -> Callable:
-        async def route(request: Request, result=Depends(super().route_page)):
-            if request.user:
-                raise HTTPException(
-                    status_code=status.HTTP_307_TEMPORARY_REDIRECT,
-                    detail="already logged in",
-                    headers={"location": request.query_params.get("redirect") or "/"},
-                )
-            return result
-
-        return route
-
-    async def has_page_permission(self, request: Request) -> bool:
-        return True
-
-
-class UserRegFormAdmin(FormAdmin):
-    user_model: Type[BaseUser] = User
-    page = Page(title=_("User Register"))
-    page_path = "/reg"
-    page_parser_mode = "html"
-    schema: Type[SchemaUpdateT] = None
-    schema_submit_out: Type[UserLoginOut] = None
-    page_schema = None
-    page_route_kwargs = {"name": "reg"}
-
-    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[BaseModel]:  # self.schema_submit_out
-        auth: Auth = request.auth
-        user = await auth.db.async_scalar(select(self.user_model).where(self.user_model.username == data.username))
-        if user:
-            return BaseApiOut(status=-1, msg=_("Username has been registered!"), data=None)
-        user = await auth.db.async_scalar(select(self.user_model).where(self.user_model.email == data.email))
-        if user:
-            return BaseApiOut(status=-2, msg=_("Email has been registered!"), data=None)
-        values = data.dict(exclude={"id", "password"})
-        values["password"] = auth.pwd_context.hash(data.password.get_secret_value())  # 密码hash保存
-        user = self.user_model.parse_obj(values)
-        try:
-            auth.db.add(user)
-            await auth.db.async_flush()
-        except Exception as e:
-            raise HTTPException(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                detail=f"Error Execute SQL：{e}",
-            ) from e
-        # 注册成功,设置用户信息
-        token_info = self.schema_submit_out.parse_obj(user)
-        token_info.access_token = await auth.backend.token_store.write_token(user.dict())
-        return BaseApiOut(code=0, msg=_("Registered successfully!"), data=token_info)
-
-    @property
-    def route_submit(self):
-        async def route(response: Response, result: BaseApiOut = Depends(super().route_submit)):
-            if result.status == 0 and result.code == 0:  # 登录成功,设置用户信息
-                response.set_cookie("Authorization", f"bearer {result.data.access_token}")
-            return result
-
-        return route
-
-    async def get_form(self, request: Request) -> Form:
-        form = await super().get_form(request)
-        form.redirect = request.query_params.get("redirect") or "/"
-        form.update_from_kwargs(
-            title="",
-            mode=DisplayModeEnum.horizontal,
-            submitText=_("Sign up"),
-            actionsClassName="no-border m-none p-none",
-            panelClassName="",
-            wrapWithPanel=True,
-            horizontal=Horizontal(left=3, right=9),
-            actions=[
-                ButtonToolbar(
-                    buttons=[
-                        ActionType.Link(
-                            actionType="link",
-                            link=f"{self.router_path}/login",
-                            label=_("Sign in"),
-                        ),
-                        Action(actionType="submit", label=_("Sign up"), level=LevelEnum.primary),
-                    ]
-                )
-            ],
-        )
-
-        return form
-
-    async def get_page(self, request: Request) -> Page:
-        page = await super().get_page(request)
-        return attach_page_head(page)
-
-    async def has_page_permission(self, request: Request) -> bool:
-        return True
-
-
-class UserInfoFormAdmin(FormAdmin):
-    page_schema = None
-    group_schema = None
-    user_model: Type[BaseUser] = User
-    page = Page(title=_("User Profile"))
-    page_path = "/userinfo"
-    schema: Type[SchemaUpdateT] = None
-    schema_submit_out: Type[BaseUser] = None
-    form_init = True
-    form = Form(mode=DisplayModeEnum.horizontal)
-    page_route_kwargs = {"name": "userinfo"}
-
-    async def get_init_data(self, request: Request, **kwargs) -> BaseApiOut[Any]:
-        return BaseApiOut(data=request.user.dict(exclude={"password"}))
-
-    async def get_form(self, request: Request) -> Form:
-        form = await super().get_form(request)
-        formitems = [
-            await self.get_form_item(request, modelfield)
-            for k, modelfield in self.user_model.__fields__.items()
-            if k not in self.schema.__fields__
-        ]
-        form.body.extend(formitem.update_from_kwargs(disabled=True) for formitem in formitems if formitem)
-        return form
-
-    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[Any]:
-        for k, v in data.dict(exclude_none=True).items():
-            if k == "password":
-                if not v:
-                    continue
-                else:
-                    v = request.auth.pwd_context.hash(v)  # 密码hash保存
-            setattr(request.user, k, v)
-        return BaseApiOut(data=self.schema_submit_out.parse_obj(request.user))
-
-    async def has_page_permission(self, request: Request) -> bool:
-        return await self.site.auth.requires(response=False)(request)
-
-
-class UserAdmin(ModelAdmin):
-    group_schema = None
-    page_schema = PageSchema(label=_("User"), icon="fa fa-user")
-    model: Type[BaseUser] = None
-    exclude = ["password"]
-    link_model_fields = [User.roles, User.groups]
-    search_fields = [User.username]
-
-    async def on_create_pre(self, request: Request, obj, **kwargs) -> Dict[str, Any]:
-        data = await super(UserAdmin, self).on_create_pre(request, obj, **kwargs)
-        data["password"] = request.auth.pwd_context.hash(data["password"])  # 密码hash保存
-        return data
-
-    async def on_update_pre(self, request: Request, obj, item_id: List[int], **kwargs) -> Dict[str, Any]:
-        data = await super(UserAdmin, self).on_update_pre(request, obj, item_id, **kwargs)
-        password = data.get("password")
-        if password:
-            data["password"] = request.auth.pwd_context.hash(data["password"])  # 密码hash保存
-        return data
-
-
-class RoleAdmin(ModelAdmin):
-    group_schema = None
-    page_schema = PageSchema(label=_("Role"), icon="fa fa-group")
-    model = Role
-    link_model_fields = [Role.permissions]
-    readonly_fields = ["key"]
-
-
-class GroupAdmin(ModelAdmin):
-    group_schema = None
-    page_schema = PageSchema(label=_("Group"), icon="fa fa-group")
-    model = Group
-    link_model_fields = [Group.roles]
-    readonly_fields = ["key"]
-
-
-class PermissionAdmin(ModelAdmin):
-    group_schema = None
-    page_schema = PageSchema(label=_("Permission"), icon="fa fa-lock")
-    model = Permission
-    readonly_fields = ["key"]
+import contextlib
+from typing import Any, Callable, Dict, List, Type
+
+from fastapi import Depends, HTTPException
+from fastapi_amis_admin.admin import FormAdmin, ModelAdmin, PageSchemaAdmin
+from fastapi_amis_admin.amis.components import (
+    Action,
+    ActionType,
+    ButtonToolbar,
+    Form,
+    Grid,
+    Horizontal,
+    Html,
+    Page,
+    PageSchema,
+)
+from fastapi_amis_admin.amis.constants import DisplayModeEnum, LevelEnum
+from fastapi_amis_admin.crud.base import SchemaUpdateT
+from fastapi_amis_admin.crud.schema import BaseApiOut
+from fastapi_amis_admin.utils.translation import i18n as _
+from pydantic import BaseModel
+from sqlalchemy import select
+from starlette import status
+from starlette.requests import Request
+from starlette.responses import Response
+from starlette.routing import NoMatchFound
+
+from fastapi_user_auth.auth import Auth
+from fastapi_user_auth.auth.models import BaseUser, Group, Permission, Role, User
+from fastapi_user_auth.auth.schemas import UserLoginOut
+
+
+def attach_page_head(page: Page) -> Page:
+    desc = _("Amis is a low-code front-end framework that reduces page development effort and greatly improves efficiency")
+    page.body = [
+        Html(
+            html=f'<div style="display: flex; justify-content: center; align-items: center; margin: 96px 0px 8px;">'
+            f'<img src="https://baidu.gitee.io/amis/static/favicon_b3b0647.png" alt="logo" style="margin-right: 8px; '
+            f'width: 48px;"><span style="font-size: 32px; font-weight: bold;">Amis Admin</span></div>'
+            f'<div style="width: 100%; text-align: center; color: rgba(0, 0, 0, 0.45); margin-bottom: 40px;">{desc}</div>'
+        ),
+        Grid(columns=[{"body": [page.body], "lg": 2, "md": 4, "valign": "middle"}], align="center", valign="middle"),
+    ]
+    return page
+
+
+class UserLoginFormAdmin(FormAdmin):
+    page = Page(title=_("User Login"))
+    page_path = "/login"
+    page_parser_mode = "html"
+    schema: Type[SchemaUpdateT] = None
+    schema_submit_out: Type[UserLoginOut] = None
+    page_schema = None
+    page_route_kwargs = {"name": "login"}
+
+    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[BaseModel]:  # self.schema_submit_out
+        if request.user:
+            return BaseApiOut(code=1, msg=_("User logged in!"), data=self.schema_submit_out.parse_obj(request.user))
+        user = await request.auth.authenticate_user(username=data.username, password=data.password)  # type:ignore
+        if not user:
+            return BaseApiOut(status=-1, msg=_("Incorrect username or password!"))
+        if not user.is_active:
+            return BaseApiOut(status=-2, msg=_("Inactive user status!"))
+
+        token_info = self.schema_submit_out.parse_obj(user)
+        auth: Auth = request.auth
+        token_info.access_token = await auth.backend.token_store.write_token(user.dict())
+        return BaseApiOut(code=0, data=token_info)
+
+    @property
+    def route_submit(self):
+        async def route(response: Response, result: BaseApiOut = Depends(super().route_submit)):
+            if result.status == 0 and result.code == 0:  # 登录成功,设置用户信息
+                response.set_cookie("Authorization", f"bearer {result.data.access_token}")
+            return result
+
+        return route
+
+    async def get_form(self, request: Request) -> Form:
+        form = await super().get_form(request)
+        buttons = []
+        with contextlib.suppress(NoMatchFound):
+            buttons.append(
+                ActionType.Link(
+                    actionType="link",
+                    link=f"{self.site.router_path}{self.app.router.url_path_for('reg')}",
+                    label=_("Sign up"),
+                )
+            )
+        buttons.append(Action(actionType="submit", label=_("Sign in"), level=LevelEnum.primary))
+        form.body.sort(key=lambda form_item: form_item.type, reverse=True)
+        form.update_from_kwargs(
+            title="",
+            mode=DisplayModeEnum.horizontal,
+            submitText=_("Sign in"),
+            actionsClassName="no-border m-none p-none",
+            panelClassName="",
+            wrapWithPanel=True,
+            horizontal=Horizontal(left=3, right=9),
+            actions=[ButtonToolbar(buttons=buttons)],
+        )
+        form.redirect = request.query_params.get("redirect") or "/"
+        return form
+
+    async def get_page(self, request: Request) -> Page:
+        page = await super().get_page(request)
+        return attach_page_head(page)
+
+    @property
+    def route_page(self) -> Callable:
+        async def route(request: Request, result=Depends(super().route_page)):
+            if request.user:
+                raise HTTPException(
+                    status_code=status.HTTP_307_TEMPORARY_REDIRECT,
+                    detail="already logged in",
+                    headers={"location": request.query_params.get("redirect") or "/"},
+                )
+            return result
+
+        return route
+
+    async def has_page_permission(self, request: Request, obj: PageSchemaAdmin = None, action: str = None) -> bool:
+        return True
+
+
+class UserRegFormAdmin(FormAdmin):
+    user_model: Type[BaseUser] = User
+    page = Page(title=_("User Register"))
+    page_path = "/reg"
+    page_parser_mode = "html"
+    schema: Type[SchemaUpdateT] = None
+    schema_submit_out: Type[UserLoginOut] = None
+    page_schema = None
+    page_route_kwargs = {"name": "reg"}
+
+    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[BaseModel]:  # self.schema_submit_out
+        auth: Auth = request.auth
+        user = await auth.db.async_scalar(select(self.user_model).where(self.user_model.username == data.username))
+        if user:
+            return BaseApiOut(status=-1, msg=_("Username has been registered!"), data=None)
+        user = await auth.db.async_scalar(select(self.user_model).where(self.user_model.email == data.email))
+        if user:
+            return BaseApiOut(status=-2, msg=_("Email has been registered!"), data=None)
+        values = data.dict(exclude={"id", "password"})
+        values["password"] = auth.pwd_context.hash(data.password.get_secret_value())  # 密码hash保存
+        user = self.user_model.parse_obj(values)
+        try:
+            auth.db.add(user)
+            await auth.db.async_flush()
+        except Exception as e:
+            raise HTTPException(
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+                detail=f"Error Execute SQL：{e}",
+            ) from e
+        # 注册成功,设置用户信息
+        token_info = self.schema_submit_out.parse_obj(user)
+        token_info.access_token = await auth.backend.token_store.write_token(user.dict())
+        return BaseApiOut(code=0, msg=_("Registered successfully!"), data=token_info)
+
+    @property
+    def route_submit(self):
+        async def route(response: Response, result: BaseApiOut = Depends(super().route_submit)):
+            if result.status == 0 and result.code == 0:  # 登录成功,设置用户信息
+                response.set_cookie("Authorization", f"bearer {result.data.access_token}")
+            return result
+
+        return route
+
+    async def get_form(self, request: Request) -> Form:
+        form = await super().get_form(request)
+        form.redirect = request.query_params.get("redirect") or "/"
+        form.update_from_kwargs(
+            title="",
+            mode=DisplayModeEnum.horizontal,
+            submitText=_("Sign up"),
+            actionsClassName="no-border m-none p-none",
+            panelClassName="",
+            wrapWithPanel=True,
+            horizontal=Horizontal(left=3, right=9),
+            actions=[
+                ButtonToolbar(
+                    buttons=[
+                        ActionType.Link(
+                            actionType="link",
+                            link=f"{self.router_path}/login",
+                            label=_("Sign in"),
+                        ),
+                        Action(actionType="submit", label=_("Sign up"), level=LevelEnum.primary),
+                    ]
+                )
+            ],
+        )
+
+        return form
+
+    async def get_page(self, request: Request) -> Page:
+        page = await super().get_page(request)
+        return attach_page_head(page)
+
+    async def has_page_permission(self, request: Request, obj: PageSchemaAdmin = None, action: str = None) -> bool:
+        return True
+
+
+class UserInfoFormAdmin(FormAdmin):
+    page_schema = None
+    user_model: Type[BaseUser] = User
+    page = Page(title=_("User Profile"))
+    page_path = "/userinfo"
+    schema: Type[SchemaUpdateT] = None
+    schema_submit_out: Type[BaseUser] = None
+    form_init = True
+    form = Form(mode=DisplayModeEnum.horizontal)
+    page_route_kwargs = {"name": "userinfo"}
+
+    async def get_init_data(self, request: Request, **kwargs) -> BaseApiOut[Any]:
+        return BaseApiOut(data=request.user.dict(exclude={"password"}))
+
+    async def get_form(self, request: Request) -> Form:
+        form = await super().get_form(request)
+        formitems = [
+            await self.get_form_item(request, modelfield)
+            for k, modelfield in self.user_model.__fields__.items()
+            if k not in self.schema.__fields__
+        ]
+        form.body.extend(formitem.update_from_kwargs(disabled=True) for formitem in formitems if formitem)
+        return form
+
+    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[Any]:
+        for k, v in data.dict(exclude_none=True).items():
+            if k == "password":
+                if not v:
+                    continue
+                else:
+                    v = request.auth.pwd_context.hash(v)  # 密码hash保存
+            setattr(request.user, k, v)
+        return BaseApiOut(data=self.schema_submit_out.parse_obj(request.user))
+
+    async def has_page_permission(self, request: Request, obj: PageSchemaAdmin = None, action: str = None) -> bool:
+        return await self.site.auth.requires(response=False)(request)
+
+
+class UserAdmin(ModelAdmin):
+    page_schema = PageSchema(label=_("User"), icon="fa fa-user")
+    model: Type[BaseUser] = None
+    exclude = ["password"]
+    link_model_fields = [User.roles, User.groups]
+    search_fields = [User.username]
+
+    async def on_create_pre(self, request: Request, obj, **kwargs) -> Dict[str, Any]:
+        data = await super(UserAdmin, self).on_create_pre(request, obj, **kwargs)
+        data["password"] = request.auth.pwd_context.hash(data["password"])  # 密码hash保存
+        return data
+
+    async def on_update_pre(self, request: Request, obj, item_id: List[int], **kwargs) -> Dict[str, Any]:
+        data = await super(UserAdmin, self).on_update_pre(request, obj, item_id, **kwargs)
+        password = data.get("password")
+        if password:
+            data["password"] = request.auth.pwd_context.hash(data["password"])  # 密码hash保存
+        return data
+
+
+class RoleAdmin(ModelAdmin):
+    page_schema = PageSchema(label=_("Role"), icon="fa fa-group")
+    model = Role
+    link_model_fields = [Role.permissions]
+    readonly_fields = ["key"]
+
+
+class GroupAdmin(ModelAdmin):
+    page_schema = PageSchema(label=_("Group"), icon="fa fa-group")
+    model = Group
+    link_model_fields = [Group.roles]
+    readonly_fields = ["key"]
+
+
+class PermissionAdmin(ModelAdmin):
+    page_schema = PageSchema(label=_("Permission"), icon="fa fa-lock")
+    model = Permission
+    readonly_fields = ["key"]
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/app.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from typing import Type
-
-from fastapi_amis_admin.admin import AdminApp, ModelAdmin
-from fastapi_amis_admin.amis.components import PageSchema
-from fastapi_amis_admin.crud.utils import schema_create_by_schema
-from fastapi_amis_admin.utils.translation import i18n as _
-from starlette.requests import Request
-
-from fastapi_user_auth.admin import GroupAdmin as DefaultGroupAdmin
-from fastapi_user_auth.admin import PermissionAdmin as DefaultPermissionAdmin
-from fastapi_user_auth.admin import RoleAdmin as DefaultRoleAdmin
-from fastapi_user_auth.admin import UserAdmin as DefaultUserAdmin
-from fastapi_user_auth.admin import UserInfoFormAdmin as DefaultUserInfoFormAdmin
-from fastapi_user_auth.admin import UserLoginFormAdmin as DefaultUserLoginFormAdmin
-from fastapi_user_auth.admin import UserRegFormAdmin as DefaultUserRegFormAdmin
-from fastapi_user_auth.auth import AuthRouter
-
-
-class UserAuthApp(AdminApp, AuthRouter):
-    page_schema = PageSchema(label=_("User Authentication"), icon="fa fa-lock", sort=99)
-    router_prefix = "/auth"
-    # default admin
-    UserLoginFormAdmin: Type[DefaultUserLoginFormAdmin] = DefaultUserLoginFormAdmin
-    UserRegFormAdmin: Type[DefaultUserRegFormAdmin] = DefaultUserRegFormAdmin
-    UserInfoFormAdmin: Type[DefaultUserInfoFormAdmin] = DefaultUserInfoFormAdmin
-    UserAdmin: Type[DefaultUserAdmin] = DefaultUserAdmin
-    RoleAdmin: Type[ModelAdmin] = DefaultRoleAdmin
-    GroupAdmin: Type[ModelAdmin] = DefaultGroupAdmin
-    PermissionAdmin: Type[ModelAdmin] = DefaultPermissionAdmin
-
-    def __init__(self, app: "AdminApp"):
-        AdminApp.__init__(self, app)
-        self.auth = self.auth or self.site.auth
-        AuthRouter.__init__(self)
-        self.UserAdmin.model = self.UserAdmin.model or self.auth.user_model
-        self.UserLoginFormAdmin.schema = self.UserLoginFormAdmin.schema or schema_create_by_schema(
-            self.auth.user_model, "UserLoginIn", include={"username", "password"}
-        )
-        self.UserLoginFormAdmin.schema_submit_out = self.UserLoginFormAdmin.schema_submit_out or self.schema_user_login_out
-        self.UserRegFormAdmin.schema = self.UserRegFormAdmin.schema or schema_create_by_schema(
-            self.auth.user_model, "UserRegIn", include={"username", "password", "email"}
-        )
-        self.UserRegFormAdmin.schema_submit_out = self.UserRegFormAdmin.schema_submit_out or self.schema_user_login_out
-        self.UserInfoFormAdmin.user_model = self.auth.user_model
-        self.UserInfoFormAdmin.schema = self.UserInfoFormAdmin.schema or schema_create_by_schema(
-            self.auth.user_model,
-            "UserInfoForm",
-            include={"nickname", "password", "avatar", "email"},
-            set_none=True,
-        )
-        self.UserInfoFormAdmin.schema_submit_out = self.UserInfoFormAdmin.schema_submit_out or self.schema_user_info
-        # register admin
-        self.register_admin(
-            self.UserLoginFormAdmin,
-            self.UserRegFormAdmin,
-            self.UserInfoFormAdmin,
-            self.UserAdmin,
-            self.RoleAdmin,
-            self.GroupAdmin,
-            self.PermissionAdmin,
-        )
-
-    async def has_page_permission(self, request: Request) -> bool:
-        return await super().has_page_permission(request) and await request.auth.requires(roles="admin", response=False)(request)
+from typing import Type
+
+from fastapi_amis_admin.admin import AdminApp, ModelAdmin, PageSchemaAdmin
+from fastapi_amis_admin.amis.components import PageSchema
+from fastapi_amis_admin.crud.utils import schema_create_by_schema
+from fastapi_amis_admin.utils.translation import i18n as _
+from starlette.requests import Request
+
+from fastapi_user_auth.admin import GroupAdmin as DefaultGroupAdmin
+from fastapi_user_auth.admin import PermissionAdmin as DefaultPermissionAdmin
+from fastapi_user_auth.admin import RoleAdmin as DefaultRoleAdmin
+from fastapi_user_auth.admin import UserAdmin as DefaultUserAdmin
+from fastapi_user_auth.admin import UserInfoFormAdmin as DefaultUserInfoFormAdmin
+from fastapi_user_auth.admin import UserLoginFormAdmin as DefaultUserLoginFormAdmin
+from fastapi_user_auth.admin import UserRegFormAdmin as DefaultUserRegFormAdmin
+from fastapi_user_auth.auth import AuthRouter
+
+
+class UserAuthApp(AdminApp, AuthRouter):
+    page_schema = PageSchema(label=_("User Authentication"), icon="fa fa-lock", sort=99)
+    router_prefix = "/auth"
+    # default admin
+    UserLoginFormAdmin: Type[DefaultUserLoginFormAdmin] = DefaultUserLoginFormAdmin
+    UserRegFormAdmin: Type[DefaultUserRegFormAdmin] = DefaultUserRegFormAdmin
+    UserInfoFormAdmin: Type[DefaultUserInfoFormAdmin] = DefaultUserInfoFormAdmin
+    UserAdmin: Type[DefaultUserAdmin] = DefaultUserAdmin
+    RoleAdmin: Type[ModelAdmin] = DefaultRoleAdmin
+    GroupAdmin: Type[ModelAdmin] = DefaultGroupAdmin
+    PermissionAdmin: Type[ModelAdmin] = DefaultPermissionAdmin
+
+    def __init__(self, app: "AdminApp"):
+        AdminApp.__init__(self, app)
+        self.auth = self.auth or self.site.auth
+        AuthRouter.__init__(self)
+        self.UserAdmin.model = self.UserAdmin.model or self.auth.user_model
+        self.UserLoginFormAdmin.schema = self.UserLoginFormAdmin.schema or schema_create_by_schema(
+            self.auth.user_model, "UserLoginIn", include={"username", "password"}
+        )
+        self.UserLoginFormAdmin.schema_submit_out = self.UserLoginFormAdmin.schema_submit_out or self.schema_user_login_out
+        self.UserRegFormAdmin.schema = self.UserRegFormAdmin.schema or schema_create_by_schema(
+            self.auth.user_model, "UserRegIn", include={"username", "password", "email"}
+        )
+        self.UserRegFormAdmin.schema_submit_out = self.UserRegFormAdmin.schema_submit_out or self.schema_user_login_out
+        self.UserInfoFormAdmin.user_model = self.auth.user_model
+        self.UserInfoFormAdmin.schema = self.UserInfoFormAdmin.schema or schema_create_by_schema(
+            self.auth.user_model,
+            "UserInfoForm",
+            include={"nickname", "password", "avatar", "email"},
+            set_none=True,
+        )
+        self.UserInfoFormAdmin.schema_submit_out = self.UserInfoFormAdmin.schema_submit_out or self.schema_user_info
+        # register admin
+        self.register_admin(
+            self.UserLoginFormAdmin,
+            self.UserRegFormAdmin,
+            self.UserInfoFormAdmin,
+            self.UserAdmin,
+            self.RoleAdmin,
+            self.GroupAdmin,
+            self.PermissionAdmin,
+        )
+
+    async def has_page_permission(self, request: Request, obj: PageSchemaAdmin = None, action: str = None) -> bool:
+        return await super().has_page_permission(request) and await request.auth.requires(roles="admin", response=False)(request)
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/auth/auth.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,316 +1,312 @@
-import asyncio
-import contextlib
-import functools
-import inspect
-from collections.abc import Coroutine
-from typing import (
-    Any,
-    Callable,
-    Generic,
-    Optional,
-    Sequence,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
-
-from fastapi import Depends, FastAPI, Form, HTTPException, params
-from fastapi.security import OAuth2PasswordBearer
-from fastapi.security.utils import get_authorization_scheme_param
-from fastapi_amis_admin.crud.base import RouterMixin
-from fastapi_amis_admin.crud.schema import BaseApiOut
-from fastapi_amis_admin.crud.utils import schema_create_by_schema
-from fastapi_amis_admin.utils.functools import cached_property
-from fastapi_amis_admin.utils.translation import i18n as _
-from passlib.context import CryptContext
-from pydantic import BaseModel, SecretStr
-from sqlalchemy.orm import Session
-from sqlalchemy_database import AsyncDatabase, Database
-from sqlmodel import select
-from starlette.authentication import AuthenticationBackend
-from starlette.middleware.authentication import AuthenticationMiddleware
-from starlette.requests import Request
-from starlette.responses import RedirectResponse, Response
-from starlette.websockets import WebSocket
-
-from .backends.base import BaseTokenStore
-from .backends.db import DbTokenStore
-from .models import BaseUser, Role, User, UserRoleLink
-from .schemas import UserLoginOut
-
-_UserModelT = TypeVar("_UserModelT", bound=BaseUser)
-
-
-class AuthBackend(AuthenticationBackend, Generic[_UserModelT]):
-    def __init__(self, auth: "Auth", token_store: BaseTokenStore):
-        self.auth = auth
-        self.token_store = token_store
-
-    @staticmethod
-    def get_user_token(request: Request) -> Optional[str]:
-        authorization: str = request.headers.get("Authorization") or request.cookies.get("Authorization")
-        scheme, token = get_authorization_scheme_param(authorization)
-        return None if not authorization or scheme.lower() != "bearer" else token
-
-    async def authenticate(self, request: Request) -> Tuple["Auth", Optional[_UserModelT]]:
-        return self.auth, await self.auth.get_current_user(request)
-
-    def attach_middleware(self, app: FastAPI):
-        app.add_middleware(AuthenticationMiddleware, backend=self)  # 添加auth中间件
-
-
-class Auth(Generic[_UserModelT]):
-    user_model: Type[_UserModelT] = None
-    db: Union[AsyncDatabase, Database] = None
-    backend: AuthBackend[_UserModelT] = None
-
-    def __init__(
-        self,
-        db: Union[AsyncDatabase, Database],
-        token_store: BaseTokenStore = None,
-        user_model: Type[_UserModelT] = User,
-        pwd_context: CryptContext = CryptContext(schemes=["bcrypt"], deprecated="auto"),
-    ):
-        self.user_model = user_model or self.user_model
-        assert self.user_model, "user_model is None"
-        self.db = db or self.db
-        self.backend = self.backend or AuthBackend(self, token_store or DbTokenStore(self.db))
-        self.pwd_context = pwd_context
-
-    async def authenticate_user(self, username: str, password: Union[str, SecretStr]) -> Optional[_UserModelT]:
-        user = await self.db.async_scalar(select(self.user_model).where(self.user_model.username == username))
-        if user:
-            pwd = password.get_secret_value() if isinstance(password, SecretStr) else password
-            pwd2 = user.password.get_secret_value() if isinstance(user.password, SecretStr) else user.password
-            if self.pwd_context.verify(pwd, pwd2):  # 用户存在 且 密码验证通过
-                return user
-        return None
-
-    @cached_property
-    def get_current_user(self):
-        async def _get_current_user(request: Request) -> Optional[_UserModelT]:
-            if request.scope.get("auth"):  # 防止重复授权
-                return request.scope.get("user")
-            request.scope["auth"], request.scope["user"] = self, None
-            token = self.backend.get_user_token(request)
-            if not token:
-                return None
-            token_data = await self.backend.token_store.read_token(token)
-            if token_data is not None:
-                request.scope["user"]: _UserModelT = await self.db.async_get(self.user_model, token_data.id)
-            return request.user
-
-        return _get_current_user
-
-    def requires(
-        self,
-        roles: Union[str, Sequence[str]] = None,
-        groups: Union[str, Sequence[str]] = None,
-        permissions: Union[str, Sequence[str]] = None,
-        status_code: int = 403,
-        redirect: str = None,
-        response: Union[bool, Response] = None,
-    ) -> Callable:  # sourcery no-metrics
-        groups_ = (groups,) if not groups or isinstance(groups, str) else tuple(groups)
-        roles_ = (roles,) if not roles or isinstance(roles, str) else tuple(roles)
-        permissions_ = (permissions,) if not permissions or isinstance(permissions, str) else tuple(permissions)
-
-        async def has_requires(user: _UserModelT) -> bool:
-            return user and await self.db.async_run_sync(user.has_requires, roles=roles, groups=groups, permissions=permissions)
-
-        async def depend(
-            request: Request,
-            user: _UserModelT = Depends(self.get_current_user),
-        ) -> Union[bool, Response]:
-            user_auth = request.scope.get("__user_auth__", None)
-            if user_auth is None:
-                request.scope["__user_auth__"] = {}
-            cache_key = (groups_, roles_, permissions_)
-            if cache_key not in request.scope["__user_auth__"]:  # 防止重复授权
-                if isinstance(user, params.Depends):
-                    user = await self.get_current_user(request)
-                result = await has_requires(user)
-                request.scope["__user_auth__"][cache_key] = result
-            if not request.scope["__user_auth__"][cache_key]:
-                if response is not None:
-                    return response
-                code, headers = status_code, {}
-                if redirect is not None:
-                    code = 307
-                    headers = {"location": request.url_for(redirect)}
-                raise HTTPException(status_code=code, headers=headers)
-            return True
-
-        def decorator(func: Callable = None) -> Union[Callable, Coroutine]:
-            if func is None:
-                return depend
-            if isinstance(func, Request):
-                return depend(func)
-            sig = inspect.signature(func)
-            for idx, parameter in enumerate(sig.parameters.values()):  # noqa: B007
-                if parameter.name in ["request", "websocket"]:
-                    type_ = parameter.name
-                    break
-            else:
-                raise Exception(f'No "request" or "websocket" argument on function "{func}"')
-
-            if type_ == "websocket":
-                # Handle websocket functions. (Always async)
-                @functools.wraps(func)
-                async def websocket_wrapper(*args: Any, **kwargs: Any) -> None:
-                    websocket = kwargs.get("websocket", args[idx] if args else None)
-                    assert isinstance(websocket, WebSocket)
-                    user = await self.get_current_user(websocket)  # type: ignore
-                    if not await has_requires(user):
-                        await websocket.close()
-                    else:
-                        await func(*args, **kwargs)
-
-                return websocket_wrapper
-
-            elif asyncio.iscoroutinefunction(func):
-                # Handle async request/response functions.
-                @functools.wraps(func)
-                async def async_wrapper(*args: Any, **kwargs: Any) -> Response:
-                    request = kwargs.get("request", args[idx] if args else None)
-                    assert isinstance(request, Request)
-                    response = await depend(request)
-                    if response is True:
-                        return await func(*args, **kwargs)
-                    return response
-
-                return async_wrapper
-
-            else:
-                # Handle sync request/response functions.
-                @functools.wraps(func)
-                def sync_wrapper(*args: Any, **kwargs: Any) -> Response:
-                    request = kwargs.get("request", args[idx] if args else None)
-                    assert isinstance(request, Request)
-                    loop = asyncio.new_event_loop()
-                    asyncio.set_event_loop(loop)
-                    response = loop.run_until_complete(loop.create_task(depend(request)))
-                    if response is True:
-                        return func(*args, **kwargs)
-                    return response
-
-                return sync_wrapper
-
-        return decorator
-
-    def _create_role_user_sync(self, session: Session, role_key: str = "admin") -> User:
-        # create admin role
-        role = session.scalar(select(Role).where(Role.key == role_key))
-        if not role:
-            role = Role(key=role_key, name=f"{role_key} role")
-            session.add(role)
-            session.flush()
-
-        # create admin user
-        user = session.scalar(
-            select(self.user_model)
-            .join(UserRoleLink, UserRoleLink.user_id == self.user_model.id)
-            .where(UserRoleLink.role_id == role.id)
-        )
-        if not user:
-            user = self.user_model(
-                username=role_key,
-                password=self.pwd_context.hash(role_key),
-                email=f"{role_key}@amis.work",  # type:ignore
-                roles=[role],
-            )
-            session.add(user)
-            session.flush()
-        return user
-
-    async def create_role_user(self, role_key: str = "admin", commit: bool = True) -> User:
-        user = await self.db.async_run_sync(self._create_role_user_sync, role_key)
-        if commit:
-            await self.db.async_commit()
-        return user
-
-
-class AuthRouter(RouterMixin):
-    auth: Auth = None
-    schema_user_login_out: Type[UserLoginOut] = UserLoginOut
-    router_prefix = "/auth"
-    schema_user_info: Type[BaseModel] = None
-
-    def __init__(self, auth: Auth = None):
-        self.auth = auth or self.auth
-        assert self.auth, "auth is None"
-        RouterMixin.__init__(self)
-        self.router.dependencies.insert(0, Depends(self.auth.backend.authenticate))
-        self.schema_user_info = self.schema_user_info or schema_create_by_schema(
-            self.auth.user_model, "UserInfo", exclude={"password"}
-        )
-
-        self.router.add_api_route(
-            "/userinfo",
-            self.route_userinfo,
-            methods=["GET"],
-            description=_("User Profile"),
-            dependencies=None,
-            response_model=BaseApiOut[self.schema_user_info],
-        )
-        self.router.add_api_route(
-            "/logout",
-            self.route_logout,
-            methods=["GET"],
-            description=_("Sign out"),
-            dependencies=None,
-            response_model=BaseApiOut,
-        )
-        # oauth2
-        self.router.dependencies.append(Depends(self.OAuth2(tokenUrl=f"{self.router_path}/gettoken", auto_error=False)))
-        self.router.add_api_route(
-            "/gettoken",
-            self.route_gettoken,
-            methods=["POST"],
-            description="OAuth2 Token",
-            response_model=BaseApiOut[self.schema_user_login_out],
-        )
-
-    @cached_property
-    def router_path(self) -> str:
-        return self.router.prefix
-
-    @property
-    def route_userinfo(self):
-        @self.auth.requires()
-        async def userinfo(request: Request):
-            return BaseApiOut(data=request.user)
-
-        return userinfo
-
-    @property
-    def route_logout(self):
-        @self.auth.requires()
-        async def user_logout(request: Request):
-            token_value = request.auth.backend.get_user_token(request=request)
-            with contextlib.suppress(Exception):
-                await self.auth.backend.token_store.destroy_token(token=token_value)
-            response = RedirectResponse(url="/")
-            response.delete_cookie("Authorization")
-            return response
-
-        return user_logout
-
-    @property
-    def route_gettoken(self):
-        async def oauth_token(request: Request, response: Response, username: str = Form(...), password: str = Form(...)):
-            if request.scope.get("user") is None:
-                request.scope["user"] = await request.auth.authenticate_user(username=username, password=password)
-            if request.scope.get("user") is None:
-                return BaseApiOut(status=-1, msg=_("Incorrect username or password!"))
-            token_info = self.schema_user_login_out.parse_obj(request.user)
-            token_info.access_token = await request.auth.backend.token_store.write_token(request.user.dict())
-            response.set_cookie("Authorization", f"bearer {token_info.access_token}")
-            return BaseApiOut(data=token_info)
-
-        return oauth_token
-
-    class OAuth2(OAuth2PasswordBearer):
-        async def __call__(self, request: Request) -> Optional[str]:
-            return request.auth.backend.get_user_token(request)
+import asyncio
+import contextlib
+import functools
+import inspect
+from collections.abc import Coroutine
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+
+from fastapi import Depends, FastAPI, Form, HTTPException, params
+from fastapi.security import OAuth2PasswordBearer
+from fastapi.security.utils import get_authorization_scheme_param
+from fastapi_amis_admin.crud.base import RouterMixin
+from fastapi_amis_admin.crud.schema import BaseApiOut
+from fastapi_amis_admin.crud.utils import schema_create_by_schema
+from fastapi_amis_admin.utils.functools import cached_property
+from fastapi_amis_admin.utils.translation import i18n as _
+from passlib.context import CryptContext
+from pydantic import BaseModel, SecretStr
+from sqlalchemy.orm import Session
+from sqlalchemy_database import AsyncDatabase, Database
+from sqlmodel import select
+from starlette.authentication import AuthenticationBackend
+from starlette.middleware.authentication import AuthenticationMiddleware
+from starlette.requests import Request
+from starlette.responses import RedirectResponse, Response
+from starlette.websockets import WebSocket
+
+from .backends.base import BaseTokenStore
+from .backends.db import DbTokenStore
+from .models import BaseUser, Role, User, UserRoleLink
+from .schemas import UserLoginOut
+
+UserModelT = TypeVar("UserModelT", bound=BaseUser)
+
+
+class AuthBackend(AuthenticationBackend, Generic[UserModelT]):
+    def __init__(self, auth: "Auth", token_store: BaseTokenStore):
+        self.auth = auth
+        self.token_store = token_store
+
+    @staticmethod
+    def get_user_token(request: Request) -> Optional[str]:
+        authorization: str = request.headers.get("Authorization") or request.cookies.get("Authorization")
+        scheme, token = get_authorization_scheme_param(authorization)
+        return None if not authorization or scheme.lower() != "bearer" else token
+
+    async def authenticate(self, request: Request) -> Tuple["Auth", Optional[UserModelT]]:
+        return self.auth, await self.auth.get_current_user(request)
+
+    def attach_middleware(self, app: FastAPI):
+        app.add_middleware(AuthenticationMiddleware, backend=self)  # 添加auth中间件
+
+
+class Auth(Generic[UserModelT]):
+    user_model: Type[UserModelT] = None
+    db: Union[AsyncDatabase, Database] = None
+    backend: AuthBackend[UserModelT] = None
+
+    def __init__(
+        self,
+        db: Union[AsyncDatabase, Database],
+        token_store: BaseTokenStore = None,
+        user_model: Type[UserModelT] = User,
+        pwd_context: CryptContext = CryptContext(schemes=["bcrypt"], deprecated="auto"),
+    ):
+        self.user_model = user_model or self.user_model
+        assert self.user_model, "user_model is None"
+        self.db = db or self.db
+        self.backend = self.backend or AuthBackend(self, token_store or DbTokenStore(self.db))
+        self.pwd_context = pwd_context
+
+    async def authenticate_user(self, username: str, password: Union[str, SecretStr]) -> Optional[UserModelT]:
+        user = await self.db.async_scalar(select(self.user_model).where(self.user_model.username == username))
+        if user:
+            pwd = password.get_secret_value() if isinstance(password, SecretStr) else password
+            pwd2 = user.password.get_secret_value() if isinstance(user.password, SecretStr) else user.password
+            if self.pwd_context.verify(pwd, pwd2):  # 用户存在 且 密码验证通过
+                return user
+        return None
+
+    async def get_current_user(self, request: Request) -> Optional[UserModelT]:
+        if request.scope.get("auth"):  # 防止重复授权
+            return request.scope.get("user")
+        request.scope["auth"], request.scope["user"] = self, None
+        token = self.backend.get_user_token(request)
+        if not token:
+            return None
+        token_data = await self.backend.token_store.read_token(token)
+        if token_data is not None:
+            request.scope["user"]: UserModelT = await self.db.async_get(self.user_model, token_data.id)
+        return request.user
+
+    def requires(
+        self,
+        roles: Union[str, Sequence[str]] = None,
+        groups: Union[str, Sequence[str]] = None,
+        permissions: Union[str, Sequence[str]] = None,
+        status_code: int = 403,
+        redirect: str = None,
+        response: Union[bool, Response] = None,
+    ) -> Callable:  # sourcery no-metrics
+        groups_ = (groups,) if not groups or isinstance(groups, str) else tuple(groups)
+        roles_ = (roles,) if not roles or isinstance(roles, str) else tuple(roles)
+        permissions_ = (permissions,) if not permissions or isinstance(permissions, str) else tuple(permissions)
+
+        async def has_requires(user: UserModelT) -> bool:
+            return user and await self.db.async_run_sync(user.has_requires, roles=roles, groups=groups, permissions=permissions)
+
+        async def depend(
+            request: Request,
+            user: UserModelT = Depends(self.get_current_user),
+        ) -> Union[bool, Response]:
+            user_auth = request.scope.get("__user_auth__", None)
+            if user_auth is None:
+                request.scope["__user_auth__"] = {}
+            cache_key = (groups_, roles_, permissions_)
+            if cache_key not in request.scope["__user_auth__"]:  # 防止重复授权
+                if isinstance(user, params.Depends):
+                    user = await self.get_current_user(request)
+                result = await has_requires(user)
+                request.scope["__user_auth__"][cache_key] = result
+            if not request.scope["__user_auth__"][cache_key]:
+                if response is not None:
+                    return response
+                code, headers = status_code, {}
+                if redirect is not None:
+                    code = 307
+                    headers = {"location": request.url_for(redirect)}
+                raise HTTPException(status_code=code, headers=headers)
+            return True
+
+        def decorator(func: Callable = None) -> Union[Callable, Coroutine]:
+            if func is None:
+                return depend
+            if isinstance(func, Request):
+                return depend(func)
+            sig = inspect.signature(func)
+            for idx, parameter in enumerate(sig.parameters.values()):  # noqa: B007
+                if parameter.name in ["request", "websocket"]:
+                    type_ = parameter.name
+                    break
+            else:
+                raise Exception(f'No "request" or "websocket" argument on function "{func}"')
+
+            if type_ == "websocket":
+                # Handle websocket functions. (Always async)
+                @functools.wraps(func)
+                async def websocket_wrapper(*args: Any, **kwargs: Any) -> None:
+                    websocket = kwargs.get("websocket", args[idx] if args else None)
+                    assert isinstance(websocket, WebSocket)
+                    user = await self.get_current_user(websocket)  # type: ignore
+                    if not await has_requires(user):
+                        await websocket.close()
+                    else:
+                        await func(*args, **kwargs)
+
+                return websocket_wrapper
+
+            elif asyncio.iscoroutinefunction(func):
+                # Handle async request/response functions.
+                @functools.wraps(func)
+                async def async_wrapper(*args: Any, **kwargs: Any) -> Response:
+                    request = kwargs.get("request", args[idx] if args else None)
+                    assert isinstance(request, Request)
+                    response = await depend(request)
+                    if response is True:
+                        return await func(*args, **kwargs)
+                    return response
+
+                return async_wrapper
+
+            else:
+                # Handle sync request/response functions.
+                @functools.wraps(func)
+                def sync_wrapper(*args: Any, **kwargs: Any) -> Response:
+                    request = kwargs.get("request", args[idx] if args else None)
+                    assert isinstance(request, Request)
+                    loop = asyncio.new_event_loop()
+                    asyncio.set_event_loop(loop)
+                    response = loop.run_until_complete(loop.create_task(depend(request)))
+                    if response is True:
+                        return func(*args, **kwargs)
+                    return response
+
+                return sync_wrapper
+
+        return decorator
+
+    def _create_role_user_sync(self, session: Session, role_key: str = "admin") -> User:
+        # create admin role
+        role = session.scalar(select(Role).where(Role.key == role_key))
+        if not role:
+            role = Role(key=role_key, name=f"{role_key} role")
+            session.add(role)
+            session.flush()
+
+        # create admin user
+        user = session.scalar(
+            select(self.user_model)
+            .join(UserRoleLink, UserRoleLink.user_id == self.user_model.id)
+            .where(UserRoleLink.role_id == role.id)
+        )
+        if not user:
+            user = self.user_model(
+                username=role_key,
+                password=self.pwd_context.hash(role_key),
+                email=f"{role_key}@amis.work",  # type:ignore
+                roles=[role],
+            )
+            session.add(user)
+            session.flush()
+        return user
+
+    async def create_role_user(self, role_key: str = "admin", commit: bool = True) -> User:
+        user = await self.db.async_run_sync(self._create_role_user_sync, role_key)
+        if commit:
+            await self.db.async_commit()
+        return user
+
+
+class AuthRouter(RouterMixin):
+    auth: Auth = None
+    schema_user_login_out: Type[UserLoginOut] = UserLoginOut
+    router_prefix = "/auth"
+    schema_user_info: Type[BaseModel] = None
+
+    def __init__(self, auth: Auth = None):
+        self.auth = auth or self.auth
+        assert self.auth, "auth is None"
+        RouterMixin.__init__(self)
+        self.router.dependencies.insert(0, Depends(self.auth.backend.authenticate))
+        self.schema_user_info = self.schema_user_info or schema_create_by_schema(
+            self.auth.user_model, "UserInfo", exclude={"password"}
+        )
+
+        self.router.add_api_route(
+            "/userinfo",
+            self.route_userinfo,
+            methods=["GET"],
+            description=_("User Profile"),
+            dependencies=None,
+            response_model=BaseApiOut[self.schema_user_info],
+        )
+        self.router.add_api_route(
+            "/logout",
+            self.route_logout,
+            methods=["GET"],
+            description=_("Sign out"),
+            dependencies=None,
+            response_model=BaseApiOut,
+        )
+        # oauth2
+        self.router.dependencies.append(Depends(self.OAuth2(tokenUrl=f"{self.router_path}/gettoken", auto_error=False)))
+        self.router.add_api_route(
+            "/gettoken",
+            self.route_gettoken,
+            methods=["POST"],
+            description="OAuth2 Token",
+            response_model=BaseApiOut[self.schema_user_login_out],
+        )
+
+    @cached_property
+    def router_path(self) -> str:
+        return self.router.prefix
+
+    @property
+    def route_userinfo(self):
+        @self.auth.requires()
+        async def userinfo(request: Request):
+            return BaseApiOut(data=request.user)
+
+        return userinfo
+
+    @property
+    def route_logout(self):
+        @self.auth.requires()
+        async def user_logout(request: Request):
+            token_value = request.auth.backend.get_user_token(request=request)
+            with contextlib.suppress(Exception):
+                await self.auth.backend.token_store.destroy_token(token=token_value)
+            response = RedirectResponse(url="/")
+            response.delete_cookie("Authorization")
+            return response
+
+        return user_logout
+
+    @property
+    def route_gettoken(self):
+        async def oauth_token(request: Request, response: Response, username: str = Form(...), password: str = Form(...)):
+            if request.scope.get("user") is None:
+                request.scope["user"] = await request.auth.authenticate_user(username=username, password=password)
+            if request.scope.get("user") is None:
+                return BaseApiOut(status=-1, msg=_("Incorrect username or password!"))
+            token_info = self.schema_user_login_out.parse_obj(request.user)
+            token_info.access_token = await request.auth.backend.token_store.write_token(request.user.dict())
+            response.set_cookie("Authorization", f"bearer {token_info.access_token}")
+            return BaseApiOut(data=token_info)
+
+        return oauth_token
+
+    class OAuth2(OAuth2PasswordBearer):
+        async def __call__(self, request: Request) -> Optional[str]:
+            return request.auth.backend.get_user_token(request)
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/base.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/base.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Generic, Optional, TypeVar, Union
-
-from fastapi_user_auth.auth.schemas import BaseTokenData
-
-_TokenDataSchemaT = TypeVar("_TokenDataSchemaT", bound=BaseTokenData)
-
-
-class BaseTokenStore(Generic[_TokenDataSchemaT]):
-    TokenDataSchema: _TokenDataSchemaT
-
-    def __init__(self, expire_seconds: Optional[int] = 60 * 60 * 24 * 3, TokenDataSchema: _TokenDataSchemaT = None) -> None:
-        self.TokenDataSchema = TokenDataSchema or BaseTokenData
-        self.expire_seconds = expire_seconds
-
-    async def read_token(self, token: Optional[str]) -> Optional[_TokenDataSchemaT]:
-        raise NotImplementedError
-
-    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
-        raise NotImplementedError
-
-    async def destroy_token(self, token: str) -> None:
-        raise NotImplementedError
+from typing import Generic, Optional, TypeVar, Union
+
+from fastapi_user_auth.auth.schemas import BaseTokenData
+
+_TokenDataSchemaT = TypeVar("_TokenDataSchemaT", bound=BaseTokenData)
+
+
+class BaseTokenStore(Generic[_TokenDataSchemaT]):
+    TokenDataSchema: _TokenDataSchemaT
+
+    def __init__(self, expire_seconds: Optional[int] = 60 * 60 * 24 * 3, TokenDataSchema: _TokenDataSchemaT = None) -> None:
+        self.TokenDataSchema = TokenDataSchema or BaseTokenData
+        self.expire_seconds = expire_seconds
+
+    async def read_token(self, token: Optional[str]) -> Optional[_TokenDataSchemaT]:
+        raise NotImplementedError
+
+    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
+        raise NotImplementedError
+
+    async def destroy_token(self, token: str) -> None:
+        raise NotImplementedError
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/db.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/db.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import secrets
-from datetime import datetime, timedelta
-from typing import Optional, Union
-
-from sqlalchemy import Column, String, delete
-from sqlalchemy_database import AsyncDatabase, Database
-from sqlmodel import Field, select
-
-from ..backends.base import BaseTokenStore, _TokenDataSchemaT
-from ..models import CreateTimeMixin, PkMixin
-
-
-class TokenStoreModel(PkMixin, CreateTimeMixin, table=True):
-    __tablename__ = "auth_token"
-    token: str = Field(..., max_length=48, sa_column=Column(String(48), unique=True, index=True, nullable=False))
-    data: str = Field(default="")
-
-
-class DbTokenStore(BaseTokenStore):
-    def __init__(
-        self,
-        db: Union[AsyncDatabase, Database],
-        expire_seconds: Optional[int] = 60 * 60 * 24 * 3,
-        TokenDataSchema: _TokenDataSchemaT = None,
-    ):
-        super().__init__(expire_seconds, TokenDataSchema)
-        self.db = db
-
-    async def read_token(self, token: str) -> Optional[_TokenDataSchemaT]:
-        stmt = select(TokenStoreModel).where(TokenStoreModel.token == token)
-        obj: TokenStoreModel = await self.db.async_scalar(stmt)
-        if obj is None:
-            return None
-        # expire
-        if obj.create_time < datetime.now() - timedelta(seconds=self.expire_seconds):
-            await self.destroy_token(token=token)
-            return None
-        return self.TokenDataSchema.parse_raw(obj.data)
-
-    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
-        obj = self.TokenDataSchema.parse_obj(token_data) if isinstance(token_data, dict) else token_data
-        token = secrets.token_urlsafe()
-        model = TokenStoreModel(token=token, data=obj.json())
-        self.db.add(model)
-        await self.db.async_flush()
-        return token
-
-    async def destroy_token(self, token: str) -> None:
-        stmt = delete(TokenStoreModel).where(TokenStoreModel.token == token)
-        await self.db.async_execute(stmt)
-        await self.db.async_flush()
+import secrets
+from datetime import datetime, timedelta
+from typing import Optional, Union
+
+from sqlalchemy import Column, String, delete
+from sqlalchemy_database import AsyncDatabase, Database
+from sqlmodel import Field, select
+
+from ..backends.base import BaseTokenStore, _TokenDataSchemaT
+from ..models import CreateTimeMixin, PkMixin
+
+
+class TokenStoreModel(PkMixin, CreateTimeMixin, table=True):
+    __tablename__ = "auth_token"
+    token: str = Field(..., max_length=48, sa_column=Column(String(48), unique=True, index=True, nullable=False))
+    data: str = Field(default="")
+
+
+class DbTokenStore(BaseTokenStore):
+    def __init__(
+        self,
+        db: Union[AsyncDatabase, Database],
+        expire_seconds: Optional[int] = 60 * 60 * 24 * 3,
+        TokenDataSchema: _TokenDataSchemaT = None,
+    ):
+        super().__init__(expire_seconds, TokenDataSchema)
+        self.db = db
+
+    async def read_token(self, token: str) -> Optional[_TokenDataSchemaT]:
+        stmt = select(TokenStoreModel).where(TokenStoreModel.token == token)
+        obj: TokenStoreModel = await self.db.async_scalar(stmt)
+        if obj is None:
+            return None
+        # expire
+        if obj.create_time < datetime.now() - timedelta(seconds=self.expire_seconds):
+            await self.destroy_token(token=token)
+            return None
+        return self.TokenDataSchema.parse_raw(obj.data)
+
+    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
+        obj = self.TokenDataSchema.parse_obj(token_data) if isinstance(token_data, dict) else token_data
+        token = secrets.token_urlsafe()
+        model = TokenStoreModel(token=token, data=obj.json())
+        self.db.add(model)
+        await self.db.async_flush()
+        return token
+
+    async def destroy_token(self, token: str) -> None:
+        stmt = delete(TokenStoreModel).where(TokenStoreModel.token == token)
+        await self.db.async_execute(stmt)
+        await self.db.async_flush()
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/jwt.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/jwt.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from datetime import datetime, timedelta
-from typing import Optional, Union
-
-from jose import JWTError, jwt
-
-from ..backends.base import BaseTokenStore, _TokenDataSchemaT
-
-
-class JwtTokenStore(BaseTokenStore):
-    def __init__(
-        self,
-        secret_key: str,
-        algorithm: str = "HS256",
-        expire_seconds: Optional[int] = 60 * 60 * 24 * 3,
-        TokenDataSchema: _TokenDataSchemaT = None,
-    ):
-        super().__init__(expire_seconds, TokenDataSchema)
-        self.secret_key = secret_key
-        self.algorithm = algorithm
-
-    async def read_token(self, token: str) -> Optional[_TokenDataSchemaT]:
-        try:
-            payload = jwt.decode(token, self.secret_key, algorithms=self.algorithm)
-            return self.TokenDataSchema.parse_obj(payload)
-        except JWTError:
-            return None
-
-    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
-        obj = self.TokenDataSchema.parse_obj(token_data) if isinstance(token_data, dict) else token_data
-        data = obj.dict()
-        expire = datetime.now() + timedelta(seconds=self.expire_seconds)
-        data.update({"exp": expire})
-        return jwt.encode(data, self.secret_key, algorithm=self.algorithm)
-
-    async def destroy_token(self, token: str) -> None:
-        raise NotImplementedError
+from datetime import datetime, timedelta
+from typing import Optional, Union
+
+from jose import JWTError, jwt
+
+from ..backends.base import BaseTokenStore, _TokenDataSchemaT
+
+
+class JwtTokenStore(BaseTokenStore):
+    def __init__(
+        self,
+        secret_key: str,
+        algorithm: str = "HS256",
+        expire_seconds: Optional[int] = 60 * 60 * 24 * 3,
+        TokenDataSchema: _TokenDataSchemaT = None,
+    ):
+        super().__init__(expire_seconds, TokenDataSchema)
+        self.secret_key = secret_key
+        self.algorithm = algorithm
+
+    async def read_token(self, token: str) -> Optional[_TokenDataSchemaT]:
+        try:
+            payload = jwt.decode(token, self.secret_key, algorithms=self.algorithm)
+            return self.TokenDataSchema.parse_obj(payload)
+        except JWTError:
+            return None
+
+    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
+        obj = self.TokenDataSchema.parse_obj(token_data) if isinstance(token_data, dict) else token_data
+        data = obj.dict()
+        expire = datetime.now() + timedelta(seconds=self.expire_seconds)
+        data.update({"exp": expire})
+        return jwt.encode(data, self.secret_key, algorithm=self.algorithm)
+
+    async def destroy_token(self, token: str) -> None:
+        raise NotImplementedError
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/auth/backends/redis.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/redis.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import secrets
-from typing import Optional, Union
-
-from aioredis import Redis
-
-from ..backends.base import BaseTokenStore, _TokenDataSchemaT
-
-
-class RedisTokenStore(BaseTokenStore):
-    def __init__(self, redis: Redis, expire_seconds: Optional[int] = 60 * 60 * 24 * 3, TokenDataSchema: _TokenDataSchemaT = None):
-        super().__init__(expire_seconds, TokenDataSchema)
-        self.redis = redis
-
-    async def read_token(self, token: str) -> Optional[_TokenDataSchemaT]:
-        data = await self.redis.get(self.get_key(token))
-        if data is None:
-            return None
-        return self.TokenDataSchema.parse_raw(data)
-
-    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
-        obj = self.TokenDataSchema.parse_obj(token_data) if isinstance(token_data, dict) else token_data
-        token = secrets.token_urlsafe()
-        await self.redis.set(self.get_key(token), obj.json(), ex=self.expire_seconds)
-        return token
-
-    async def destroy_token(self, token: str) -> None:
-        await self.redis.delete(self.get_key(token))
-
-    def get_key(self, token: str):
-        return f"auth:token:{token}"
+import secrets
+from typing import Optional, Union
+
+from aioredis import Redis
+
+from ..backends.base import BaseTokenStore, _TokenDataSchemaT
+
+
+class RedisTokenStore(BaseTokenStore):
+    def __init__(self, redis: Redis, expire_seconds: Optional[int] = 60 * 60 * 24 * 3, TokenDataSchema: _TokenDataSchemaT = None):
+        super().__init__(expire_seconds, TokenDataSchema)
+        self.redis = redis
+
+    async def read_token(self, token: str) -> Optional[_TokenDataSchemaT]:
+        data = await self.redis.get(self.get_key(token))
+        if data is None:
+            return None
+        return self.TokenDataSchema.parse_raw(data)
+
+    async def write_token(self, token_data: Union[_TokenDataSchemaT, dict]) -> str:
+        obj = self.TokenDataSchema.parse_obj(token_data) if isinstance(token_data, dict) else token_data
+        token = secrets.token_urlsafe()
+        await self.redis.set(self.get_key(token), obj.json(), ex=self.expire_seconds)
+        return token
+
+    async def destroy_token(self, token: str) -> None:
+        await self.redis.delete(self.get_key(token))
+
+    def get_key(self, token: str):
+        return f"auth:token:{token}"
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/auth/models.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/models.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,305 +1,305 @@
-from datetime import datetime
-from typing import Any, List, Optional, Sequence, Union
-
-from fastapi_amis_admin.amis.components import ColumnImage, InputImage
-from fastapi_amis_admin.models.fields import Field
-from fastapi_amis_admin.utils.translation import i18n as _
-from pydantic import EmailStr, SecretStr
-from sqlalchemy import and_, func
-from sqlalchemy.orm import Session
-from sqlalchemy.schema import ForeignKey
-from sqlalchemy.sql.selectable import Exists
-from sqlmodel import Relationship, select
-
-try:
-    from sqlmodelx import SQLModel
-except ImportError:
-    from sqlmodel import SQLModel
-
-
-class PkMixin(SQLModel):
-    id: int = Field(default=None, primary_key=True, nullable=False)
-
-
-class CreateTimeMixin(SQLModel):
-    create_time: datetime = Field(default_factory=datetime.now, title=_("Create Time"))
-
-
-class UpdateTimeMixin(SQLModel):
-    update_time: Optional[datetime] = Field(
-        default_factory=datetime.now,
-        title=_("Update Time"),
-        sa_column_kwargs={"onupdate": func.now(), "server_default": func.now()},
-    )
-
-
-class UsernameMixin(SQLModel):
-    username: str = Field(title=_("Username"), max_length=32, unique=True, index=True, nullable=False)
-
-
-class PasswordStr(SecretStr, str):
-    pass
-
-
-class PasswordMixin(SQLModel):
-    password: PasswordStr = Field(title=_("Password"), max_length=128, nullable=False, amis_form_item="input-password")
-
-
-class EmailMixin(SQLModel):
-    """If you need to define the email field as unique, you can achieve it by adding the following parameters in the subclass:
-    __table_args__ = (UniqueConstraint("email", name="email"),)
-    """
-
-    email: EmailStr = Field(None, title=_("Email"), index=True, nullable=True, amis_form_item="input-email")
-
-
-class UserRoleLink(SQLModel, table=True):
-    __tablename__ = "auth_user_roles"
-    user_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_user.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-    role_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_role.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-
-
-class UserGroupLink(SQLModel, table=True):
-    __tablename__ = "auth_user_groups"
-    user_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_user.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-    group_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_group.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-
-
-class GroupRoleLink(SQLModel, table=True):
-    __tablename__ = "auth_group_roles"
-    group_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_group.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-    role_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_role.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-
-
-class RolePermissionLink(SQLModel, table=True):
-    __tablename__ = "auth_role_permissions"
-    role_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_role.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-    permission_id: int = Field(
-        primary_key=True,
-        sa_column_args=(
-            ForeignKey(
-                "auth_permission.id",
-                ondelete="CASCADE",
-            ),
-        ),
-    )
-
-
-class BaseUser(PkMixin, UsernameMixin, PasswordMixin, EmailMixin, CreateTimeMixin):
-    __tablename__ = "auth_user"
-    is_active: bool = Field(default=True, title=_("Is Active"))
-    nickname: str = Field(None, title=_("Nickname"), max_length=40)
-    avatar: str = Field(
-        None,
-        title=_("Avatar"),
-        max_length=255,
-        amis_form_item=InputImage(maxLength=1, maxSize=2 * 1024 * 1024),
-        amis_table_column=ColumnImage(width=50, height=50, enlargeAble=True),
-    )
-
-    @property
-    def is_authenticated(self) -> bool:
-        return self.is_active
-
-    @property
-    def display_name(self) -> str:
-        return self.nickname or self.username
-
-    @property
-    def identity(self) -> str:
-        return self.username
-
-    def _exists_role(self, *role_whereclause: Any) -> Exists:
-        # check user role
-        user_role_ids = (
-            select(Role.id)
-            .join(UserRoleLink, (UserRoleLink.user_id == self.id) & (UserRoleLink.role_id == Role.id))
-            .where(*role_whereclause)
-        )
-        # check user group
-        role_group_ids = select(GroupRoleLink.group_id).join(Role, and_(*role_whereclause, Role.id == GroupRoleLink.role_id))
-        group_user_ids = (
-            select(UserGroupLink.user_id)
-            .where(UserGroupLink.user_id == self.id)
-            .where(UserGroupLink.group_id.in_(role_group_ids))
-        )
-        return user_role_ids.exists() | group_user_ids.exists()
-
-    def _exists_roles(self, roles: List[str]) -> Exists:
-        """
-        检查用户是否属于指定用户角色,或属于包含指定用户角色的用户组
-        Args:
-            roles:
-
-        Returns:
-
-        """
-        return self._exists_role(Role.key.in_(roles))
-
-    def _exists_groups(self, groups: List[str]) -> Exists:
-        """
-        检查用户是否属于指定用户组
-        Args:
-            groups:
-
-        Returns:
-
-        """
-        group_ids = (
-            select(Group.id)
-            .join(UserGroupLink, (UserGroupLink.user_id == self.id) & (UserGroupLink.group_id == Group.id))
-            .where(Group.key.in_(groups))
-        )
-        return group_ids.exists()
-
-    def _exists_permissions(self, permissions: List[str]) -> Exists:
-        """
-        检查用户是否属于拥有指定权限的用户角色
-        Args:
-            permissions:
-
-        Returns:
-
-        """
-        role_ids = select(RolePermissionLink.role_id).join(
-            Permission, Permission.key.in_(permissions) & (Permission.id == RolePermissionLink.permission_id)
-        )
-        return self._exists_role(Role.id.in_(role_ids))
-
-    def has_requires(
-        self,
-        session: Session,
-        *,
-        roles: Union[str, Sequence[str]] = None,
-        groups: Union[str, Sequence[str]] = None,
-        permissions: Union[str, Sequence[str]] = None,
-    ) -> bool:
-        """
-        检查用户是否属于拥有指定的RBAC权限
-        Args:
-            session: sqlalchemy `Session`;异步`AsyncSession`,请使用`run_sync`方法.
-            roles: 角色列表
-            groups: 用户组列表
-            permissions: 权限列表
-
-        Returns:
-            检测成功返回`True`
-        """
-        if not groups and not roles and not permissions:
-            return True
-        stmt = select(1)
-        if groups:
-            groups_list = [groups] if isinstance(groups, str) else list(groups)
-            stmt = stmt.where(self._exists_groups(groups_list))
-        if roles:
-            roles_list = [roles] if isinstance(roles, str) else list(roles)
-            stmt = stmt.where(self._exists_roles(roles_list))
-        if permissions:
-            permissions_list = [permissions] if isinstance(permissions, str) else list(permissions)
-            stmt = stmt.where(self._exists_permissions(permissions_list))
-        return bool(session.scalar(stmt))
-
-
-class User(BaseUser, table=True):
-    """用户"""
-
-    roles: List["Role"] = Relationship(link_model=UserRoleLink)
-    groups: List["Group"] = Relationship(link_model=UserGroupLink)
-
-
-class BaseRBAC(PkMixin):
-    __table_args__ = {"extend_existing": True}
-    key: str = Field(title=_("Identify"), max_length=40, unique=True, index=True, nullable=False)
-    name: str = Field(default="", title=_("Name"), max_length=40)
-    desc: str = Field(default="", title=_("Description"), max_length=400, amis_form_item="textarea")
-
-
-class Role(BaseRBAC, table=True):
-    """角色"""
-
-    __tablename__ = "auth_role"
-    groups: List["Group"] = Relationship(back_populates="roles", link_model=GroupRoleLink)
-    permissions: List["Permission"] = Relationship(back_populates="roles", link_model=RolePermissionLink)
-
-
-class BaseGroup(BaseRBAC):
-    __tablename__ = "auth_group"
-    parent_id: Optional[int] = Field(
-        None,
-        title=_("Parent"),
-        sa_column_args=(
-            ForeignKey(
-                "auth_group.id",
-                ondelete="SET NULL",
-            ),
-        ),
-    )
-
-
-class Group(BaseGroup, table=True):
-    """用户组"""
-
-    roles: List["Role"] = Relationship(back_populates="groups", link_model=GroupRoleLink)
-
-
-class Permission(BaseRBAC, table=True):
-    """权限"""
-
-    __tablename__ = "auth_permission"
-    roles: List["Role"] = Relationship(back_populates="permissions", link_model=RolePermissionLink)
+from datetime import datetime
+from typing import Any, List, Optional, Sequence, Union
+
+from fastapi_amis_admin.amis.components import ColumnImage, InputImage
+from fastapi_amis_admin.models.fields import Field
+from fastapi_amis_admin.utils.translation import i18n as _
+from pydantic import EmailStr, SecretStr
+from sqlalchemy import and_, func
+from sqlalchemy.orm import Session
+from sqlalchemy.schema import ForeignKey
+from sqlalchemy.sql.selectable import Exists
+from sqlmodel import Relationship, select
+
+try:
+    from sqlmodelx import SQLModel
+except ImportError:
+    from sqlmodel import SQLModel
+
+
+class PkMixin(SQLModel):
+    id: int = Field(default=None, primary_key=True, nullable=False)
+
+
+class CreateTimeMixin(SQLModel):
+    create_time: datetime = Field(default_factory=datetime.now, title=_("Create Time"))
+
+
+class UpdateTimeMixin(SQLModel):
+    update_time: Optional[datetime] = Field(
+        default_factory=datetime.now,
+        title=_("Update Time"),
+        sa_column_kwargs={"onupdate": func.now(), "server_default": func.now()},
+    )
+
+
+class UsernameMixin(SQLModel):
+    username: str = Field(title=_("Username"), max_length=32, unique=True, index=True, nullable=False)
+
+
+class PasswordStr(SecretStr, str):
+    pass
+
+
+class PasswordMixin(SQLModel):
+    password: PasswordStr = Field(title=_("Password"), max_length=128, nullable=False, amis_form_item="input-password")
+
+
+class EmailMixin(SQLModel):
+    """If you need to define the email field as unique, you can achieve it by adding the following parameters in the subclass:
+    __table_args__ = (UniqueConstraint("email", name="email"),)
+    """
+
+    email: EmailStr = Field(None, title=_("Email"), index=True, nullable=True, amis_form_item="input-email")
+
+
+class UserRoleLink(SQLModel, table=True):
+    __tablename__ = "auth_user_roles"
+    user_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_user.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+    role_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_role.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+
+
+class UserGroupLink(SQLModel, table=True):
+    __tablename__ = "auth_user_groups"
+    user_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_user.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+    group_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_group.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+
+
+class GroupRoleLink(SQLModel, table=True):
+    __tablename__ = "auth_group_roles"
+    group_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_group.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+    role_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_role.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+
+
+class RolePermissionLink(SQLModel, table=True):
+    __tablename__ = "auth_role_permissions"
+    role_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_role.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+    permission_id: int = Field(
+        primary_key=True,
+        sa_column_args=(
+            ForeignKey(
+                "auth_permission.id",
+                ondelete="CASCADE",
+            ),
+        ),
+    )
+
+
+class BaseUser(PkMixin, UsernameMixin, PasswordMixin, EmailMixin, CreateTimeMixin):
+    __tablename__ = "auth_user"
+    is_active: bool = Field(default=True, title=_("Is Active"))
+    nickname: str = Field(None, title=_("Nickname"), max_length=40)
+    avatar: str = Field(
+        None,
+        title=_("Avatar"),
+        max_length=255,
+        amis_form_item=InputImage(maxLength=1, maxSize=2 * 1024 * 1024),
+        amis_table_column=ColumnImage(width=50, height=50, enlargeAble=True),
+    )
+
+    @property
+    def is_authenticated(self) -> bool:
+        return self.is_active
+
+    @property
+    def display_name(self) -> str:
+        return self.nickname or self.username
+
+    @property
+    def identity(self) -> str:
+        return self.username
+
+    def _exists_role(self, *role_whereclause: Any) -> Exists:
+        # check user role
+        user_role_ids = (
+            select(Role.id)
+            .join(UserRoleLink, (UserRoleLink.user_id == self.id) & (UserRoleLink.role_id == Role.id))
+            .where(*role_whereclause)
+        )
+        # check user group
+        role_group_ids = select(GroupRoleLink.group_id).join(Role, and_(*role_whereclause, Role.id == GroupRoleLink.role_id))
+        group_user_ids = (
+            select(UserGroupLink.user_id)
+            .where(UserGroupLink.user_id == self.id)
+            .where(UserGroupLink.group_id.in_(role_group_ids))
+        )
+        return user_role_ids.exists() | group_user_ids.exists()
+
+    def _exists_roles(self, roles: List[str]) -> Exists:
+        """
+        检查用户是否属于指定用户角色,或属于包含指定用户角色的用户组
+        Args:
+            roles:
+
+        Returns:
+
+        """
+        return self._exists_role(Role.key.in_(roles))
+
+    def _exists_groups(self, groups: List[str]) -> Exists:
+        """
+        检查用户是否属于指定用户组
+        Args:
+            groups:
+
+        Returns:
+
+        """
+        group_ids = (
+            select(Group.id)
+            .join(UserGroupLink, (UserGroupLink.user_id == self.id) & (UserGroupLink.group_id == Group.id))
+            .where(Group.key.in_(groups))
+        )
+        return group_ids.exists()
+
+    def _exists_permissions(self, permissions: List[str]) -> Exists:
+        """
+        检查用户是否属于拥有指定权限的用户角色
+        Args:
+            permissions:
+
+        Returns:
+
+        """
+        role_ids = select(RolePermissionLink.role_id).join(
+            Permission, Permission.key.in_(permissions) & (Permission.id == RolePermissionLink.permission_id)
+        )
+        return self._exists_role(Role.id.in_(role_ids))
+
+    def has_requires(
+        self,
+        session: Session,
+        *,
+        roles: Union[str, Sequence[str]] = None,
+        groups: Union[str, Sequence[str]] = None,
+        permissions: Union[str, Sequence[str]] = None,
+    ) -> bool:
+        """
+        检查用户是否属于拥有指定的RBAC权限
+        Args:
+            session: sqlalchemy `Session`;异步`AsyncSession`,请使用`run_sync`方法.
+            roles: 角色列表
+            groups: 用户组列表
+            permissions: 权限列表
+
+        Returns:
+            检测成功返回`True`
+        """
+        if not groups and not roles and not permissions:
+            return True
+        stmt = select(1)
+        if groups:
+            groups_list = [groups] if isinstance(groups, str) else list(groups)
+            stmt = stmt.where(self._exists_groups(groups_list))
+        if roles:
+            roles_list = [roles] if isinstance(roles, str) else list(roles)
+            stmt = stmt.where(self._exists_roles(roles_list))
+        if permissions:
+            permissions_list = [permissions] if isinstance(permissions, str) else list(permissions)
+            stmt = stmt.where(self._exists_permissions(permissions_list))
+        return bool(session.scalar(stmt))
+
+
+class User(BaseUser, table=True):
+    """用户"""
+
+    roles: List["Role"] = Relationship(link_model=UserRoleLink)
+    groups: List["Group"] = Relationship(link_model=UserGroupLink)
+
+
+class BaseRBAC(PkMixin):
+    __table_args__ = {"extend_existing": True}
+    key: str = Field(title=_("Identify"), max_length=40, unique=True, index=True, nullable=False)
+    name: str = Field(default="", title=_("Name"), max_length=40)
+    desc: str = Field(default="", title=_("Description"), max_length=400, amis_form_item="textarea")
+
+
+class Role(BaseRBAC, table=True):
+    """角色"""
+
+    __tablename__ = "auth_role"
+    groups: List["Group"] = Relationship(back_populates="roles", link_model=GroupRoleLink)
+    permissions: List["Permission"] = Relationship(back_populates="roles", link_model=RolePermissionLink)
+
+
+class BaseGroup(BaseRBAC):
+    __tablename__ = "auth_group"
+    parent_id: Optional[int] = Field(
+        None,
+        title=_("Parent"),
+        sa_column_args=(
+            ForeignKey(
+                "auth_group.id",
+                ondelete="SET NULL",
+            ),
+        ),
+    )
+
+
+class Group(BaseGroup, table=True):
+    """用户组"""
+
+    roles: List["Role"] = Relationship(back_populates="groups", link_model=GroupRoleLink)
+
+
+class Permission(BaseRBAC, table=True):
+    """权限"""
+
+    __tablename__ = "auth_permission"
+    roles: List["Role"] = Relationship(back_populates="permissions", link_model=RolePermissionLink)
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/auth/schemas.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/schemas.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from fastapi_amis_admin.utils.translation import i18n as _
-from pydantic import BaseModel, SecretStr, validator
-from sqlmodel import Field
-
-from .models import BaseUser, EmailMixin, PasswordMixin, UsernameMixin
-
-
-class BaseTokenData(BaseModel):
-    id: int
-    username: str
-
-
-class UserLoginOut(BaseUser):
-    """用户登录返回信息"""
-
-    token_type: str = "bearer"
-    access_token: str = None
-    password: SecretStr = None
-
-
-class UserRegIn(UsernameMixin, PasswordMixin, EmailMixin):
-    """用户注册"""
-
-    password2: str = Field(title=_("Confirm Password"), max_length=128)
-
-    @validator("password2")
-    def passwords_match(cls, v, values, **kwargs):
-        if "password" in values and v != values["password"]:
-            raise ValueError("passwords do not match!")
-        return v
+from fastapi_amis_admin.utils.translation import i18n as _
+from pydantic import BaseModel, SecretStr, validator
+from sqlmodel import Field
+
+from .models import BaseUser, EmailMixin, PasswordMixin, UsernameMixin
+
+
+class BaseTokenData(BaseModel):
+    id: int
+    username: str
+
+
+class UserLoginOut(BaseUser):
+    """用户登录返回信息"""
+
+    token_type: str = "bearer"
+    access_token: str = None
+    password: SecretStr = None
+
+
+class UserRegIn(UsernameMixin, PasswordMixin, EmailMixin):
+    """用户注册"""
+
+    password2: str = Field(title=_("Confirm Password"), max_length=128)
+
+    @validator("password2")
+    def passwords_match(cls, v, values, **kwargs):
+        if "password" in values and v != values["password"]:
+            raise ValueError("passwords do not match!")
+        return v
```

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_user_auth-0.5.0/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.4.3/fastapi_user_auth/site.py` & `fastapi_user_auth-0.5.0/fastapi_user_auth/site.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from typing import Type
-
-from fastapi import FastAPI
-from fastapi_amis_admin.admin import AdminSite, Settings
-from fastapi_amis_admin.amis.components import ActionType, App, Dialog, Flex, Service
-from fastapi_amis_admin.amis.constants import SizeEnum
-from fastapi_amis_admin.amis.types import AmisAPI
-from fastapi_amis_admin.crud.utils import SqlalchemyDatabase
-from fastapi_amis_admin.utils.translation import i18n as _
-from starlette.requests import Request
-
-from fastapi_user_auth.app import UserAuthApp as DefaultUserAuthApp
-from fastapi_user_auth.auth import Auth
-
-
-class AuthAdminSite(AdminSite):
-    auth: Auth = None
-    UserAuthApp: Type[DefaultUserAuthApp] = DefaultUserAuthApp
-
-    def __init__(self, settings: Settings, fastapi: FastAPI = None, engine: SqlalchemyDatabase = None, auth: Auth = None):
-        super().__init__(settings, fastapi, engine)
-        self.auth = auth or self.auth or Auth(db=self.db)
-        self.register_admin(self.UserAuthApp)
-
-    async def get_page(self, request: Request) -> App:
-        app = await super().get_page(request)
-        user_auth_app = self.get_admin_or_create(self.UserAuthApp)
-        app.header = Flex(
-            className="w-full",
-            justify="flex-end",
-            alignItems="flex-end",
-            items=[
-                app.header,
-                {
-                    "type": "dropdown-button",
-                    "label": f"{request.user.username}",
-                    "trigger": "hover",
-                    "icon": "fa fa-user",
-                    "buttons": [
-                        ActionType.Dialog(
-                            label=_("User Profile"),
-                            dialog=Dialog(
-                                title=_("User Profile"),
-                                actions=[],
-                                size=SizeEnum.lg,
-                                body=Service(
-                                    schemaApi=AmisAPI(
-                                        method="post",
-                                        url=f"{user_auth_app.router_path}/form/userinfo",
-                                        cache=600000,
-                                        responseData={"&": "${body}"},
-                                    )
-                                ),
-                            ),
-                        ),
-                        ActionType.Url(label=_("Sign out"), url=f"{user_auth_app.router_path}/logout"),
-                    ],
-                },
-            ],
-        )
-        return app
-
-    async def has_page_permission(self, request: Request) -> bool:
-        return await self.auth.requires(response=False)(request)
+from typing import Type
+
+from fastapi import FastAPI
+from fastapi_amis_admin.admin import AdminSite, PageSchemaAdmin, Settings
+from fastapi_amis_admin.amis.components import ActionType, App, Dialog, Flex, Service
+from fastapi_amis_admin.amis.constants import SizeEnum
+from fastapi_amis_admin.amis.types import AmisAPI
+from fastapi_amis_admin.crud.utils import SqlalchemyDatabase
+from fastapi_amis_admin.utils.translation import i18n as _
+from starlette.requests import Request
+
+from fastapi_user_auth.app import UserAuthApp as DefaultUserAuthApp
+from fastapi_user_auth.auth import Auth
+
+
+class AuthAdminSite(AdminSite):
+    auth: Auth = None
+    UserAuthApp: Type[DefaultUserAuthApp] = DefaultUserAuthApp
+
+    def __init__(self, settings: Settings, fastapi: FastAPI = None, engine: SqlalchemyDatabase = None, auth: Auth = None):
+        super().__init__(settings, fastapi, engine)
+        self.auth = auth or self.auth or Auth(db=self.db)
+        self.register_admin(self.UserAuthApp)
+
+    async def get_page(self, request: Request) -> App:
+        app = await super().get_page(request)
+        user_auth_app = self.get_admin_or_create(self.UserAuthApp)
+        app.header = Flex(
+            className="w-full",
+            justify="flex-end",
+            alignItems="flex-end",
+            items=[
+                app.header,
+                {
+                    "type": "dropdown-button",
+                    "label": f"{request.user.username}",
+                    "trigger": "hover",
+                    "icon": "fa fa-user",
+                    "buttons": [
+                        ActionType.Dialog(
+                            label=_("User Profile"),
+                            dialog=Dialog(
+                                title=_("User Profile"),
+                                actions=[],
+                                size=SizeEnum.lg,
+                                body=Service(
+                                    schemaApi=AmisAPI(
+                                        method="post",
+                                        url=f"{user_auth_app.router_path}/form/userinfo",
+                                        cache=600000,
+                                        responseData={"&": "${body}"},
+                                    )
+                                ),
+                            ),
+                        ),
+                        ActionType.Url(label=_("Sign out"), url=f"{user_auth_app.router_path}/logout"),
+                    ],
+                },
+            ],
+        )
+        return app
+
+    async def has_page_permission(self, request: Request, obj: PageSchemaAdmin = None, action: str = None) -> bool:
+        return await self.auth.requires(response=False)(request)
```

### Comparing `fastapi_user_auth-0.4.3/pyproject.toml` & `fastapi_user_auth-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "fastapi_user_auth"
-authors = [
-    { name = "Atomi", email = "1456417373@qq.com" },
-]
-maintainers = [
-    { name = "Atomi", email = "1456417373@qq.com" },
-]
-description = "FastAPI-User-Auth is a simple and powerful FastAPI user RBAC authentication and authorization library. Based on FastAPI-Amis-Admin and provides a freely extensible visual management interface."
-readme = "README.md"
-requires-python = ">=3.7"
-dynamic = ["version"]
-keywords = [
-    "fastapi",
-    "fastapi-user-auth",
-    "fastapi-amis-admin",
-    "fastapi-auth",
-    "fastapi-users",
-    "fastapi-jwt-auth",
-    "sqlmodel",
-]
-classifiers = [
-    "Framework :: FastAPI",
-    "Environment :: Web Environment",
-    "Topic :: System :: Systems Administration",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
-dependencies = [
-    "pydantic>=1.9",
-    "fastapi-amis-admin>=0.4.0,<0.5.0",
-    "email-validator",
-    "passlib>=1.7.4",
-    "bcrypt>=4.0.0",
-    "sqlmodelx>=0.0.2",
-]
-
-[project.urls]
-Documentation = "http://docs.amis.work/"
-Source = "https://github.com/amisadmin/fastapi_user_auth"
-FastAPI-Amis-Admin = "https://github.com/amisadmin/fastapi_amis_admin"
-
-[project.optional-dependencies]
-jwt = [
-    "python-jose==3.3.0",
-]
-redis = ["aioredis"]
-db = []
-test = [
-    "uvicorn[standard] >=0.19.0,<1.0",
-    "pytest >=6.2.4",
-    "pytest-asyncio>=0.17",
-    "aiosqlite>=0.15.0",
-    "python-jose==3.3.0",
-    "jinja2 >=2.11.2,<4.0.0",
-    "ujson>=5.5.0",
-    "requests>=2.28.1",
-]
-dev = [
-    "fastapi-user-auth[test]",
-    "pre-commit>=2.20.0",
-]
-all = [
-    "fastapi-user-auth[dev]",
-]
-# pytest
-[tool.pytest.ini_options]
-minversion = "6.0"
-testpaths = [
-    "tests",
-]
-# pytest-asyncio
-asyncio_mode = "auto"
-filterwarnings = [
-    "ignore::RuntimeWarning",
-]
-[tool.isort]
-profile = "black"
-atomic = true
-filter_files = true
-
-[tool.black]
-line-length = 130
-include = '\.pyi?$'
-[tool.pdm.scripts]
-lint = "pre-commit run --all-files"
-test = "pytest"
-[tool.pdm.dev-dependencies]
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "fastapi_user_auth"
+authors = [
+    { name = "Atomi", email = "1456417373@qq.com" },
+]
+maintainers = [
+    { name = "Atomi", email = "1456417373@qq.com" },
+]
+description = "FastAPI-User-Auth is a simple and powerful FastAPI user RBAC authentication and authorization library. Based on FastAPI-Amis-Admin and provides a freely extensible visual management interface."
+readme = "README.md"
+requires-python = ">=3.7"
+dynamic = ["version"]
+keywords = [
+    "fastapi",
+    "fastapi-user-auth",
+    "fastapi-amis-admin",
+    "fastapi-auth",
+    "fastapi-users",
+    "fastapi-jwt-auth",
+    "sqlmodel",
+]
+classifiers = [
+    "Framework :: FastAPI",
+    "Environment :: Web Environment",
+    "Topic :: System :: Systems Administration",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+dependencies = [
+    "pydantic>=1.9",
+    "fastapi-amis-admin>=0.5.0,<0.6.0",
+    "email-validator",
+    "passlib>=1.7.4",
+    "bcrypt>=4.0.0",
+    "sqlmodelx>=0.0.2",
+]
+
+[project.urls]
+Documentation = "http://docs.amis.work/"
+Source = "https://github.com/amisadmin/fastapi_user_auth"
+FastAPI-Amis-Admin = "https://github.com/amisadmin/fastapi_amis_admin"
+
+[project.optional-dependencies]
+jwt = [
+    "python-jose==3.3.0",
+]
+redis = ["aioredis"]
+db = []
+test = [
+    "uvicorn[standard] >=0.19.0,<1.0",
+    "pytest >=6.2.4",
+    "pytest-asyncio>=0.17",
+    "aiosqlite>=0.15.0",
+    "python-jose==3.3.0",
+    "jinja2 >=2.11.2,<4.0.0",
+    "ujson>=5.5.0",
+    "requests>=2.28.1",
+]
+dev = [
+    "fastapi-user-auth[test]",
+    "pre-commit>=2.20.0",
+]
+all = [
+    "fastapi-user-auth[dev]",
+]
+# pytest
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = [
+    "tests",
+]
+# pytest-asyncio
+asyncio_mode = "auto"
+filterwarnings = [
+    "ignore::RuntimeWarning",
+]
+[tool.isort]
+profile = "black"
+atomic = true
+filter_files = true
+
+[tool.black]
+line-length = 130
+include = '\.pyi?$'
+[tool.pdm.scripts]
+lint = "pre-commit run --all-files"
+test = "pytest"
+[tool.pdm.dev-dependencies]
```

### Comparing `fastapi_user_auth-0.4.3/PKG-INFO` & `fastapi_user_auth-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_auth
-Version: 0.4.3
+Version: 0.5.0
 Summary: FastAPI-User-Auth is a simple and powerful FastAPI user RBAC authentication and authorization library. Based on FastAPI-Amis-Admin and provides a freely extensible visual management interface.
 Keywords: fastapi,fastapi-user-auth,fastapi-amis-admin,fastapi-auth,fastapi-users,fastapi-jwt-auth,sqlmodel
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic>=1.9
-Requires-Dist: fastapi-amis-admin>=0.4.0,<0.5.0
+Requires-Dist: fastapi-amis-admin>=0.5.0,<0.6.0
 Requires-Dist: email-validator
 Requires-Dist: passlib>=1.7.4
 Requires-Dist: bcrypt>=4.0.0
 Requires-Dist: sqlmodelx>=0.0.2
 Requires-Dist: fastapi-user-auth[dev] ; extra == "all"
 Requires-Dist: fastapi-user-auth[test] ; extra == "dev"
 Requires-Dist: pre-commit>=2.20.0 ; extra == "dev"
@@ -115,15 +115,15 @@
 # Mount the Site management system to the FastAPI instance
 site.mount_app(app)
 
 # Create initialization database table
 @app.on_event("startup")
 async def startup():
     await site.db.async_run_sync(SQLModel.metadata.create_all, is_session=False)
-    # Create default test user, Please change your password in time!!!
+    # Create default admin user,user name:admin,password:admin,please change it after login!!!
     await auth.create_role_user('admin')
     await auth.create_role_user('vip')
 
 # Requirements: User must be logged in
 @app.get("/auth/get_user")
 @auth.requires()
 def get_user(request: Request):
@@ -354,15 +354,14 @@
 Default management classes can be overridden and replaced by inheritance.
 For Example: `UserLoginFormAdmin`,`UserRegFormAdmin`,`UserInfoFormAdmin`,
 `UserAdmin`,`GroupAdmin`,`RoleAdmin`,`PermissionAdmin`
 
 ```python
 # Customize the model management class, inherit and override the corresponding default management class
 class MyGroupAdmin(admin.ModelAdmin):
-    group_schema = None
     page_schema = PageSchema(label='用户组管理', icon='fa fa-group')
     model = MyGroup
     link_model_fields = [Group.roles]
     readonly_fields = ['key']
 
 # Customize the user authentication application, inherit and override the default user authentication application
 class MyUserAuthApp(UserAuthApp):
```

