# Comparing `tmp/svcs-23.6.0.tar.gz` & `tmp/svcs-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 31 07:59:54 2023, max compression
+gzip compressed data, last modified: Wed Aug  2 14:41:14 2023, max compression
```

## Comparing `svcs-23.6.0.tar` & `svcs-23.7.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
--rw-r--r--   0        0        0      125 2023-07-31 07:59:54.000000 svcs-23.6.0/.git_archival.txt
--rw-r--r--   0        0        0      131 2023-07-31 07:59:54.000000 svcs-23.6.0/.gitattributes
--rw-r--r--   0        0        0      596 2023-07-31 07:59:54.000000 svcs-23.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-07-31 07:59:54.000000 svcs-23.6.0/.python-version-default
--rw-r--r--   0        0        0     2887 2023-07-31 07:59:54.000000 svcs-23.6.0/CHANGELOG.md
--rw-r--r--   0        0        0    16213 2023-07-31 07:59:54.000000 svcs-23.6.0/README.md
--rw-r--r--   0        0        0      841 2023-07-31 07:59:54.000000 svcs-23.6.0/conftest.py
--rw-r--r--   0        0        0      840 2023-07-31 07:59:54.000000 svcs-23.6.0/tox.ini
--rw-r--r--   0        0        0     5482 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      285 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       18 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      865 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4136 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      749 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1610 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0     1094 2023-07-31 07:59:54.000000 svcs-23.6.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      476 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/__init__.py
--rw-r--r--   0        0        0     9466 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/_core.py
--rw-r--r--   0        0        0      234 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/exceptions.py
--rw-r--r--   0        0        0     3509 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/flask.py
--rw-r--r--   0        0        0        0 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/py.typed
--rw-r--r--   0        0        0       91 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/__init__.py
--rw-r--r--   0        0        0     4555 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/test_async.py
--rw-r--r--   0        0        0    10917 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/test_core.py
--rw-r--r--   0        0        0     6426 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/test_flask.py
--rw-r--r--   0        0        0     1366 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/typing/core.py
--rw-r--r--   0        0        0     1018 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/typing/flask_.py
--rw-r--r--   0        0        0      112 2023-07-31 07:59:54.000000 svcs-23.6.0/.gitignore
--rw-r--r--   0        0        0     1072 2023-07-31 07:59:54.000000 svcs-23.6.0/LICENSE
--rw-r--r--   0        0        0     4531 2023-07-31 07:59:54.000000 svcs-23.6.0/pyproject.toml
--rw-r--r--   0        0        0     7031 2023-07-31 07:59:54.000000 svcs-23.6.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-08-02 14:41:14.000000 svcs-23.7.0/.git_archival.txt
+-rw-r--r--   0        0        0      131 2023-08-02 14:41:14.000000 svcs-23.7.0/.gitattributes
+-rw-r--r--   0        0        0      732 2023-08-02 14:41:14.000000 svcs-23.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-08-02 14:41:14.000000 svcs-23.7.0/.python-version-default
+-rw-r--r--   0        0        0     3288 2023-08-02 14:41:14.000000 svcs-23.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0    18022 2023-08-02 14:41:14.000000 svcs-23.7.0/README.md
+-rw-r--r--   0        0        0     1052 2023-08-02 14:41:14.000000 svcs-23.7.0/conftest.py
+-rw-r--r--   0        0        0      840 2023-08-02 14:41:14.000000 svcs-23.7.0/tox.ini
+-rw-r--r--   0        0        0     5482 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      285 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4136 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1642 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     1093 2023-08-02 14:41:14.000000 svcs-23.7.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0     2735 2023-08-02 14:41:14.000000 svcs-23.7.0/docs/_static/logo_with_name.svg
+-rw-r--r--   0        0        0      650 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/__init__.py
+-rw-r--r--   0        0        0    11383 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/_core.py
+-rw-r--r--   0        0        0      234 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/exceptions.py
+-rw-r--r--   0        0        0     3508 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/flask.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/py.typed
+-rw-r--r--   0        0        0       91 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      405 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/fake_factories.py
+-rw-r--r--   0        0        0      481 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/ifaces.py
+-rw-r--r--   0        0        0     2394 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_container.py
+-rw-r--r--   0        0        0     1663 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_fake_factories.py
+-rw-r--r--   0        0        0     6457 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_flask.py
+-rw-r--r--   0        0        0     8045 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_integration.py
+-rw-r--r--   0        0        0     8089 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_registry.py
+-rw-r--r--   0        0        0     1457 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/typing/core.py
+-rw-r--r--   0        0        0     1018 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/typing/flask_.py
+-rw-r--r--   0        0        0      112 2023-08-02 14:41:14.000000 svcs-23.7.0/.gitignore
+-rw-r--r--   0        0        0     1098 2023-08-02 14:41:14.000000 svcs-23.7.0/LICENSE
+-rw-r--r--   0        0        0     4845 2023-08-02 14:41:14.000000 svcs-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7535 2023-08-02 14:41:14.000000 svcs-23.7.0/PKG-INFO
```

### Comparing `svcs-23.6.0/.pre-commit-config.yaml` & `svcs-23.7.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,31 @@
 repos:
   - repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.280
+    rev: v0.0.282
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/econchick/interrogate
     rev: 1.5.0
     hooks:
       - id: interrogate
         args: [tests]
 
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.5
+    hooks:
+      - id: codespell
+
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
+        exclude: ".*\\.svg$"
       - id: check-toml
       - id: check-yaml
```

### Comparing `svcs-23.6.0/CHANGELOG.md` & `svcs-23.7.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 The **third number** is for emergencies when we need to start branches for older releases.
 
 You can find our backwards-compatibility policy [here](https://github.com/hynek/svcs/blob/main/.github/SECURITY.md).
 
 <!-- changelog follows -->
 
 
+## [23.7.0](https://github.com/hynek/svcs/compare/23.6.0...23.7.0) - 2023-08-02
+
+### Added
+
+- Factories now may take a parameter called `svcs_container` or that is annotated to be `svcs.Container`.
+  In this case the factory will receive the current container as a first positional argument.
+  This allows for recursive factories without global state.
+  [#10](https://github.com/hynek/svcs/pull/10)
+
+
 ## [23.6.0](https://github.com/hynek/svcs/compare/23.5.0...23.6.0) - 2023-07-31
 
 ### Changed
 
 - Renamed `Container.forget_service_type()` to `Container.forget_about()`.
```

### Comparing `svcs-23.6.0/README.md` & `svcs-23.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 <!-- begin-logo -->
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
-    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="20%" alt="svcs" />
+    <img src="docs/_static/logo_with_name.svg" width="25%" alt="svcs logo showing a radar" />
   </a>
 </p>
+
+<p align="center">
+  A Lightweight Service Locator for Python.
+</p>
+
 <!-- end-logo -->
 
-# *svcs*: A Lightweight Service Locator for Python
+<p align="center">
+  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/svcs">
+  <a href="./LICENSE">
+    <img alt="PyPI - License" src="https://img.shields.io/pypi/l/svcs">
+  </a>
+  <a href="https://pypi.org/project/svcs/">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/svcs">
+  </a>
+  <a href="https://pypi.org/project/svcs/">
+    <img alt="PyPI - Supported Python versions" src="https://img.shields.io/pypi/pyversions/svcs.svg">
+  </a>
+</p>
+
+---
 
 <!-- begin-pypi -->
 
-> **Warning**
-> ☠️ Not ready yet! ☠️
+> [!WARNING] ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
@@ -29,42 +46,40 @@
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
 All of this happens *within* your application – service locators are **not** related to service discovery.
 
-If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
+If you follow the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [*abstract base class*](https://docs.python.org/3.11/library/abc.html).
 
 Benefits:
 
 - Eliminates tons of repetitive **boilerplate** code,
 - unifies **acquisition** and **cleanups** of resources,
 - simplifies **testing**,
 - and allows for easy **health checks** across *all* resources.
 
-No global mutable state is necessary – but possible for extra comfort.
-
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
     db = request.services.get(Database)
     api = request.services.get(WebAPIClient)
 ```
 
-or even:
+or, if you don't shy away from some global state, even:
 
 ```python
 def view():
     db = services.get(Database)
     api = services.get(WebAPIClient)
 ```
 
-The latter already works with [Flask](#flask).
+The latter already works with [Flask](#flask) by utilizing the [`g` object](https://flask.palletsprojects.com/en/latest/api/#flask.g).
 
 You set it up like this:
 
 <!--
 ; skip: next
 -->
 
@@ -89,19 +104,23 @@
 )
 
 @atexit.register
 def cleanup():
     registry.close()  # calls engine.dispose()
 ```
 
-The generator-based setup and cleanup may remind you of [Pytest fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
+The generator-based setup and cleanup may remind you of [*pytest* fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
 The hooks that are defined as `on_registry_close` are called when you call `Registry.close()` – e.g. when your application is shutting down.
 
 *svcs* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
 
+> [!IMPORTANT]
+> All of this may look over-engineered if you have only one or two resources.
+> However, it starts paying dividends *very fast* once you go past that.
+
 
 ## Is this Dependency Injection!?
 
 No.
 
 Although the concepts are related and share the idea of having a central registry of services, the ways they provide those services are fundamentally different:
 [Dependency injection](https://en.wikipedia.org/wiki/Dependency_injection) always passes your dependencies as arguments while you actively ask a service locator for them when you need them.
@@ -124,29 +143,31 @@
         )
 
     raise InvalidFormError()
 ```
 
 The main downside is that it's impossible to verify whether all required dependencies have been configured without running the code.
 
+If you still prefer dependency injection, check out [*incant*](https://github.com/Tinche/incant).
+
 <!-- end-pypi -->
 
 
-## Low-Level Core API
+## Low-Level API
 
-You're unlikely to use the core API directly, but knowing what's happening underneath is good to dispel any concerns about magic.
+You will probably use some framework integration and not the low-level API directly, but knowing what's happening underneath is good to dispel any concerns about magic.
 
-*svcs* has two essential concepts:
+*svcs* has two core concepts: **registries** and **containers** that have different life cycles and responsibilities.
 
 
 ### Registries
 
-A **`Registry`** allows to register factories for certain types.
+A **`svcs.Registry`** allows to register factories for types.
 It's expected to live as long as your application lives.
-Its only job is to store and retrieve factories.
+Its only job is to store and retrieve factories along with some metadata.
 
 It is possible to register either factory callables or values:
 
 ```python
 >>> import svcs
 >>> import uuid
 
@@ -163,26 +184,26 @@
 
 <!--
 ; skip: next
 -->
 
 ```python
 registry.register_factory(
-    Connection, engine_factory, on_registry_close=engine.dispose
+    Connection, connection_factory, on_registry_close=engine.dispose
 )
 ```
 
 If this callback fails, it's logged at warning level but otherwise ignored.
 For instance, you could free a database connection pool in an [`atexit` handler](https://docs.python.org/3/library/atexit.html).
 This frees you from keeping track of registered resources yourself.
 
 
 ### Containers
 
-A **`Container`** belongs to a Registry and allows to create instances of the registered types, taking care of their life-cycle:
+A **`svcs.Container`** uses a `svcs.Registry` to lookup registered types and uses that information to create instances and to take care of their life cycles:
 
 ```python
 >>> container = svcs.Container(reg)
 
 >>> u = container.get(uuid.UUID)
 >>> u
 UUID('...')
@@ -190,21 +211,41 @@
 >>> # Good for DB connections, bad for UUIDs.
 >>> u is container.get(uuid.UUID)
 True
 >>> container.get(str)
 'Hello World'
 ```
 
-A container lives as long as you want the instances to live – e.g., as long as a request lives.
+A container lives as long as you want the instances to live – for example, as long as a request lives.
+
+If a factory takes a first argument called `svcs_container` or the first argument (of any name) is annotated as being `svcs.Container`, the current container instance is passed into the factory as the first *positional* argument allowing for recursive service acquisition:
 
-Importantly: It is possible to overwrite registered service factories later – e.g., for testing – **without monkey-patching**.
-You have to remove possibly cached instances from the container though (`Container.forget_about()`).
-The Flask integration takes care of this for you.
+```python
+>>> container = svcs.Container(reg)
 
-How to achieve this in other frameworks elegantly is TBD.
+# Let's make the UUID predictable for our test!
+>>> reg.register_value(uuid.UUID, uuid.UUID('639c0a5c-8d93-4a67-8341-fe43367308a5'))
+
+>>> def factory(svcs_container) -> str:
+...     return svcs_container.get(uuid.UUID).hex  # get the UUID, then work on it
+
+>>> reg.register_factory(str, factory)
+
+>>> container.get(str)
+'639c0a5c8d934a678341fe43367308a5'
+```
+
+> [!NOTE]
+> It is possible to overwrite registered service factories later – e.g., for testing – **without monkey-patching**.
+> This is especially interesting if you want to replace a low-level service with a mock without re-jiggering all services that depend on it.
+>
+> You have to remove possibly cached instances from the container though (`Container.forget_about()`).
+> The Flask integration takes care of this for you.
+>
+> How to achieve this in other frameworks elegantly is TBD.
 
 
 #### Cleanup
 
 If a factory is a [generator](https://docs.python.org/3/tutorial/classes.html#generators) and *yields* the instance instead of returning it, the generator will be remembered by the container.
 At the end, you run `container.close()` and all generators will be finished (i.e. called `next(factory)` again).
 You can use this to close files, return database connections to a pool, et cetera.
@@ -226,32 +267,32 @@
 If you have async resources (either factory or ping callable), you can use `aping()` instead.
 `aping()` works with sync resources too, so you can use it universally in async code.
 You can look at the `is_async` property to check whether you *need* to use `aget()`, though.
 
 
 ### Summary
 
-Generally, the `Registry` object should live on an application-scoped object like Flask's `app.config` object.
-On the other hand, the `Container` object should live on a request-scoped object like Flask's `g` object or Pyramid's `request` object.
+The `svc.Registry` object should live on an application-scoped object like Flask's `app.config` object.
+On the other hand, the `svc.Container` object should live on a request-scoped object like Flask's `g` object or Pyramid's `request` object.
 
 
-> **Note**
+> [!NOTE]
 > The core APIs only use vanilla objects without any global state but also without any comfort.
-> It gets more interesting when using framework-specific integrations where the life-cycle of the container and, thus, services is handled automatically.
+> It gets more interesting when using framework-specific integrations where the life cycle of the container and, thus, services is handled automatically.
 
 
 ## Flask
 
 *svcs* has grown from my frustration with the repetitiveness of using the `get_x` that creates an `x` and then stores it on the `g` object [pattern](https://flask.palletsprojects.com/en/latest/appcontext/#storing-data).
 
 Therefore it comes with Flask support out of the box in the form of the `svcs.flask` module.
 It:
 
 - puts the registry into `app.config["svcs_registry"]`,
-- unifies the putting and caching of services on the `g` object by putting a container into `g.svcs_container`,
+- unifies the caching of services on the `g` object by putting a container into `g.svcs_container`,
 - transparently retrieves them from there for you,
 - and installs a [`teardown_appcontext()`](http://flask.pocoo.org/docs/latest/api#flask.Flask.teardown_appcontext) handler that calls `close()` on the container when a request is done.
 
 ---
 
 You can add support for *svcs* by calling `svcs.flask.init_app(app)` in your [*application factory*](https://flask.palletsprojects.com/en/latest/patterns/appfactories/).
 For instance, to create a factory that uses a SQLAlchemy engine to produce connections, you could do this:
@@ -282,24 +323,24 @@
 
     # Now, register a factory that calls `engine.connect()` if you ask for a
     # `Connection`. Since we use yield inside of a context manager, the
     # connection gets cleaned up when the container is closed.
     # If you ask for a ping, it will run `SELECT 1` on a new connection and
     # clean up the connection behind itself.
     engine = create_engine("postgresql://localhost")
-    def engine_factory():
+    def connection_factory():
         with engine.connect() as conn:
             yield conn
 
     ping = text("SELECT 1")
     svcs_flask.register_factory(
         # The app argument makes it good for custom init_app() functions.
         app,
         Connection,
-        engine_factory,
+        connection_factory,
         ping=lambda conn: conn.execute(ping),
         on_registry_close=engine.dispose,
     )
 
     # You also use svcs WITHIN factories:
     svcs_flask.register_factory(
         app, # <---
@@ -312,15 +353,15 @@
 
     @atexit.register
     def cleanup() -> None:
         """
         Clean up all pools when the application shuts down.
         """
         log.info("app.cleanup.start")
-        svcs.flask.close_registry(app)
+        svcs.flask.close_registry(app)  # calls engine.dispose()
         log.info("app.cleanup.done")
     ##########################################################################
 
     ...
 
     return app
 ```
@@ -381,18 +422,18 @@
         #################################################
 
         # Now, the endpoint should return a 500.
         response = app.test_client().get("/")
         assert response.status_code == 500
 ```
 
-> **Note**
+> [!IMPORTANT]
 > The `replace_(factory|value)` method *requires* an application context and ensures that if a factory/value has already been created *and cached*, they're removed before the new factory/value is registered.
->>
-> Possible situations where this can occur are Pytest fixtures where you don't control the order in which they're called.
+>
+> Possible situations where this can occur are *pytest* fixtures where you don't control the order in which they're called.
 
 
 ### Quality of Life
 
 In practice, you can simplify/beautify the code within your views by creating a `services` module that re-exports those Flask helpers.
 
 Say this is `app/services.py`:
@@ -468,10 +509,10 @@
 def get(svc_type: type[T]) -> T:
     return svcs.flask.get(svc_type)
 ```
 
 
 ## Credits
 
-*svcs* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+*svcs* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](./LICENSE) license.
 
 The development is kindly supported by my employer [Variomedia AG](https://www.variomedia.de/) and all my amazing [GitHub Sponsors](https://github.com/sponsors/hynek).
```

### Comparing `svcs-23.6.0/conftest.py` & `svcs-23.7.0/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from doctest import ELLIPSIS
 
 import pytest
 
 from sybil import Sybil
 from sybil.parsers import myst, rest
+from tests.ifaces import Service
 
 import svcs
 
 
 markdown_examples = Sybil(
     parsers=[
         myst.DocTestDirectiveParser(optionflags=ELLIPSIS),
@@ -28,14 +29,24 @@
     ],
     patterns=["*.py"],
 )
 
 pytest_collect_file = (markdown_examples + rest_examples).pytest()
 
 
+@pytest.fixture(name="svc")
+def _svc():
+    return Service()
+
+
+@pytest.fixture(name="rs")
+def _rs(svc):
+    return svcs.RegisteredService(Service, Service, False, False, None)
+
+
 @pytest.fixture(name="registry")
 def _registry():
     return svcs.Registry()
 
 
 @pytest.fixture(name="container")
 def _container(registry):
```

### Comparing `svcs-23.6.0/tox.ini` & `svcs-23.7.0/tox.ini`

 * *Files identical despite different names*

### Comparing `svcs-23.6.0/.github/CODE_OF_CONDUCT.md` & `svcs-23.7.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `svcs-23.6.0/.github/SECURITY.md` & `svcs-23.7.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `svcs-23.6.0/.github/workflows/ci.yml` & `svcs-23.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.6.0/.github/workflows/codeql-analysis.yml` & `svcs-23.7.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.6.0/.github/workflows/pypi-package.yml` & `svcs-23.7.0/.github/workflows/pypi-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -24,32 +24,32 @@
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v1
 
   # Upload to Test PyPI on every commit on main.
-  release-test-pypi:
-    name: Publish in-dev package to test.pypi.org
-    environment: release-test-pypi
-    if: github.event_name == 'push' && github.ref == 'refs/heads/main'
-    runs-on: ubuntu-latest
-    needs: build-package
+  # release-test-pypi:
+  #   name: Publish in-dev package to test.pypi.org
+  #   environment: release-test-pypi
+  #   if: github.event_name == 'push' && github.ref == 'refs/heads/main'
+  #   runs-on: ubuntu-latest
+  #   needs: build-package
 
-    steps:
-      - name: Download packages built by build-and-inspect-python-package
-        uses: actions/download-artifact@v3
-        with:
-          name: Packages
-          path: dist
+  #   steps:
+  #     - name: Download packages built by build-and-inspect-python-package
+  #       uses: actions/download-artifact@v3
+  #       with:
+  #         name: Packages
+  #         path: dist
 
-      - name: Upload package to Test PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          repository-url: https://test.pypi.org/legacy/
+  #     - name: Upload package to Test PyPI
+  #       uses: pypa/gh-action-pypi-publish@release/v1
+  #       with:
+  #         repository-url: https://test.pypi.org/legacy/
 
   # Upload to real PyPI on GitHub Releases.
   release-pypi:
     name: Publish released package to pypi.org
     environment: release-pypi
     if: github.event.action == 'published'
     runs-on: ubuntu-latest
```

### Comparing `svcs-23.6.0/docs/_static/logo.svg` & `svcs-23.7.0/docs/_static/logo.svg`

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 000003d0: 3620 3020 3234 2d31 302e 3833 3420 3234  6 0 24-10.834 24
 000003e0: 2d32 3473 2d31 302e 3833 342d 3234 2d32  -24s-10.834-24-2
 000003f0: 342d 3234 2d32 3420 3130 2e38 3334 2d32  4-24-24 10.834-2
 00000400: 3420 3234 2031 302e 3833 3420 3234 2032  4 24 10.834 24 2
 00000410: 3420 3234 5a22 2073 7479 6c65 3d22 6669  4 24Z" style="fi
 00000420: 6c6c 3a23 6138 3535 6637 3b66 696c 6c2d  ll:#a855f7;fill-
 00000430: 7275 6c65 3a6e 6f6e 7a65 726f 222f 3e3c  rule:nonzero"/><
-00000440: 2f73 7667 3e0a                           /svg>.
+00000440: 2f73 7667 3e                             /svg>
```

### Comparing `svcs-23.6.0/src/svcs/_core.py` & `svcs-23.7.0/src/svcs/_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
+import inspect
 import logging
 import sys
 import warnings
 
 from collections.abc import Callable
 from contextlib import suppress
 from inspect import isasyncgenfunction, isawaitable, iscoroutinefunction
@@ -47,38 +48,40 @@
     def get(self, svc_type: type) -> Any:
         """
         Get an instance of *svc_type*.
 
         Instantiate it if necessary and register its cleanup.
 
         Returns:
-             Any until https://github.com/python/mypy/issues/4717 is fixed.
+             :class:`typing.Any` until
+             https://github.com/python/mypy/issues/4717 is fixed.
         """
         if (svc := self._instantiated.get(svc_type)) is not None:
             return svc
 
         rs = self.registry.get_registered_service_for(svc_type)
-        svc = rs.factory()
+        svc = rs.factory(self) if rs.takes_container else rs.factory()
 
         if isinstance(svc, Generator):
             self._on_close.append((rs.name, svc))
             svc = next(svc)
 
-        self._instantiated[rs.svc_type] = svc
+        self._instantiated[svc_type] = svc
 
         return svc
 
     async def aget(self, svc_type: type) -> Any:
         """
         Get an instance of *svc_type*.
 
         Instantiate it asynchronously if necessary and register its cleanup.
 
         Returns:
-             Any until https://github.com/python/mypy/issues/4717 is fixed.
+             :class:`typing.Any` until
+             https://github.com/python/mypy/issues/4717 is fixed.
         """
         if (svc := self._instantiated.get(svc_type)) is not None:
             return svc
 
         rs = self.registry.get_registered_service_for(svc_type)
         svc = rs.factory()
 
@@ -175,31 +178,30 @@
         ]
 
 
 @attrs.frozen
 class RegisteredService:
     svc_type: type
     factory: Callable = attrs.field(hash=False)
+    takes_container: bool
+    is_async: bool
     ping: Callable | None = attrs.field(hash=False)
 
     @property
     def name(self) -> str:
         return f"{ self.svc_type.__module__ }.{self.svc_type.__qualname__}"
 
     def __repr__(self) -> str:
         return (
             f"<RegisteredService(svc_type="
-            f"{ self.name}, "
-            f"has_ping={ self.ping is not None})>"
-        )
-
-    @property
-    def is_async(self) -> bool:
-        return iscoroutinefunction(self.factory) or isasyncgenfunction(
-            self.factory
+            f"{self.name}, "
+            f"{self.factory}, "
+            f"takes_container={self.takes_container}, "
+            f"has_ping={ self.ping is not None}"
+            ")>"
         )
 
 
 @attrs.frozen
 class ServicePing:
     _container: Container
     _rs: RegisteredService
@@ -228,39 +230,71 @@
 
 
 @attrs.define
 class Registry:
     _services: dict[type, RegisteredService] = attrs.Factory(dict)
     _on_close: list[tuple[str, Callable]] = attrs.Factory(list)
 
+    def __repr__(self) -> str:
+        return f"<svcs.Registry(num_services={len(self._services)})>"
+
     def register_factory(
         self,
         svc_type: type,
         factory: Callable,
         *,
         ping: Callable | None = None,
         on_registry_close: Callable | None = None,
     ) -> None:
-        rs = RegisteredService(svc_type, factory, ping)
+        """
+        Register *factory* for *svc_type*.
+
+        Args:
+            svc_type: The type of the service to register.
+
+            factory: A callable that is used to instantiated *svc_type* if
+                asked. If it's a generator, a cleanup is registered after
+                instantiation. Can be also async or an async generator.
+
+            ping: A callable that marks the service as having a health check.
+                The service iss returned when :meth:`Container.get_pings` is
+                called and *ping* is called as part of :meth:`ServicePing.ping`
+                or :meth:`ServicePing.aping`.
+
+            on_registry_close: A callable that is called when the
+                :meth:`Registry.close()` method is called. Can be async, then
+                :meth:`Registry.aclose()` must be called.
+        """
+        rs = RegisteredService(
+            svc_type,
+            factory,
+            _takes_container(factory),
+            iscoroutinefunction(factory) or isasyncgenfunction(factory),
+            ping,
+        )
         self._services[svc_type] = rs
 
         if on_registry_close is not None:
             self._on_close.append((rs.name, on_registry_close))
 
     def register_value(
         self,
         svc_type: type,
-        instance: object,
+        value: object,
         *,
         ping: Callable | None = None,
         on_registry_close: Callable | None = None,
     ) -> None:
+        """
+        Syntactic sugar for ``register_factory(svc_type, lambda: value,
+        ping=ping, on_registry_close=on_registry_close)``.
+        """
         self.register_factory(
             svc_type,
-            lambda: instance,
+            lambda: value,
             ping=ping,
             on_registry_close=on_registry_close,
         )
 
     def get_registered_service_for(self, svc_type: type) -> RegisteredService:
         try:
             return self._services[svc_type]
@@ -282,15 +316,15 @@
                 )
                 continue
 
             try:
                 log.debug("closing %r", name)
                 oc()
                 log.debug("closed %r", name)
-            except Exception:  # noqa: BLE001, PERF203
+            except Exception:  # noqa: BLE001
                 log.warning(
                     "Registry's on_registry_close hook failed for %r.",
                     name,
                     exc_info=True,
                     extra={"svcs_service_name": name},
                 )
 
@@ -317,7 +351,29 @@
                     name,
                     exc_info=True,
                     extra={"svcs_service_name": name},
                 )
 
         self._services.clear()
         self._on_close.clear()
+
+
+def _takes_container(factory: Callable) -> bool:
+    """
+    Return True if *factory* takes a svcs.Container as its first argument.
+    """
+    sig = inspect.signature(factory)
+    if not sig.parameters:
+        return False
+
+    if len(sig.parameters) != 1:
+        msg = "Factories must take 0 or 1 parameters."
+        raise TypeError(msg)
+
+    ((name, p),) = tuple(sig.parameters.items())
+    if name == "svcs_container":
+        return True
+
+    if (annot := p.annotation) is Container or annot == "svcs.Container":
+        return True
+
+    return False
```

### Comparing `svcs-23.6.0/src/svcs/flask.py` & `svcs-23.7.0/src/svcs/flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     app.teardown_appcontext(teardown)
 
     return app
 
 
 def get(svc_type: type) -> Any:
     """
-    Same as :meth:`svcs.Container.get()`, but uses container on ``flask.g``.
+    Same as :meth:`svcs.Container.get()`, but uses container on :obj:`flask.g`.
     """
     _, container = _ensure_req_data()
 
     return container.get(svc_type)
 
 
 def register_factory(
@@ -55,24 +55,24 @@
         svc_type, factory, ping=ping, on_registry_close=on_registry_close
     )
 
 
 def register_value(
     app: Flask,
     svc_type: type,
-    instance: object,
+    value: object,
     *,
     ping: Callable | None = None,
     on_registry_close: Callable | None = None,
 ) -> None:
     """
     Same as :meth:`svcs.Registry.register_value()`, but uses registry on *app*.
     """
     app.config["svcs_registry"].register_value(
-        svc_type, instance, ping=ping, on_registry_close=on_registry_close
+        svc_type, value, ping=ping, on_registry_close=on_registry_close
     )
 
 
 def replace_factory(
     svc_type: type,
     factory: Callable,
     *,
@@ -88,42 +88,42 @@
     registry.register_factory(
         svc_type, factory, ping=ping, on_registry_close=on_registry_close
     )
 
 
 def replace_value(
     svc_type: type,
-    instance: object,
+    value: object,
     *,
     ping: Callable | None = None,
     on_registry_close: Callable | None = None,
 ) -> None:
     """
     Register *instance* for *svc_type* and clear any cached values for it.
     """
     registry, container = _ensure_req_data()
 
     container.forget_about(svc_type)
     registry.register_value(
-        svc_type, instance, ping=ping, on_registry_close=on_registry_close
+        svc_type, value, ping=ping, on_registry_close=on_registry_close
     )
 
 
 def get_pings() -> list[ServicePing]:
     """
     See :meth:`svcs.Container.get_pings()`.
     """
     _, container = _ensure_req_data()
 
     return container.get_pings()
 
 
 def teardown(exc: BaseException | None) -> None:
     """
-    To be used with Flask.teardown_appcontext that requires to take an
+    To be used with :meth:`Flask.teardown_appcontext` that requires to take an
     exception.
 
     The app context is torn down after the response is sent.
     """
     if has_app_context() and (container := g.pop("svcs_container", None)):
         container.close()
```

### Comparing `svcs-23.6.0/tests/test_core.py` & `svcs-23.7.0/tests/test_registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,304 +1,51 @@
 # SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
 #
 # SPDX-License-Identifier: MIT
 
-import asyncio
 import contextlib
 import inspect
 
 from unittest.mock import AsyncMock, Mock
 
 import pytest
 
 import svcs
 
+from .fake_factories import (
+    async_int_factory,
+    async_str_cleanup_factory,
+    int_factory,
+    str_cleanup_factory,
+)
+from .ifaces import AnotherService, Service
+
 
 needs_working_async_mock = pytest.mark.skipif(
     not inspect.iscoroutinefunction(AsyncMock()),
     reason="AsyncMock not working",
 )
 
 
-class Service:
-    pass
-
-
-class AnotherService:
-    pass
-
-
-class YetAnotherService:
-    pass
-
-
-@pytest.fixture(name="rs")
-def _rs(svc):
-    return svcs.RegisteredService(Service, Service, None)
-
-
-@pytest.fixture(name="svc")
-def _svc():
-    return Service()
-
-
-class TestContainer:
-    def test_register_factory_get(self, registry, container):
-        """
-        register_factory registers a factory and get returns the service.
-
-        The service is cached.
-        """
-        registry.register_factory(Service, Service)
-
-        svc = container.get(Service)
-
-        assert isinstance(svc, Service)
-        assert svc is container.get(Service)
-
-    def test_register_value_get(self, registry, container, svc):
-        """
-        register_value registers a service object and get returns it.
-        """
-        registry.register_value(Service, svc)
-
-        assert svc is container.get(Service)
-        assert svc is container.get(Service)
-
-    def test_get_not_found(self, container):
-        """
-        Asking for a service that isn't registered raises a ServiceNotFoundError.
-        """
-        with pytest.raises(svcs.exceptions.ServiceNotFoundError) as ei:
-            container.get(Service)
-
-        assert Service is ei.value.args[0]
-
-    def test_get_pings_empty(self, container):
+class TestRegistry:
+    def test_repr_empty(self, registry):
         """
-        get_pings returns an empty list if there are no pings.
+        repr of an empty registry says 0 registered services.
         """
-        assert [] == container.get_pings()
+        assert "<svcs.Registry(num_services=0)>" == repr(registry)
 
-    def test_get_pings(self, registry, container, svc):
+    def test_repr_counts(self, registry):
         """
-        get_pings returns a list of ServicePings.
+        repr counts 2 registered services as 2.
         """
+        registry.register_factory(Service, Service)
         registry.register_factory(AnotherService, AnotherService)
-        registry.register_value(Service, svc, ping=lambda _: None)
-
-        assert [Service] == [
-            ping._rs.svc_type for ping in container.get_pings()
-        ]
-
-    def test_forget_about_nothing_registered(self, container):
-        """
-        forget_about does nothing if nothing has been registered.
-        """
-        container.forget_about(Service)
-
-    def test_forget_about_no_cleanup(self, container, rs, svc):
-        """
-        forget_about removes the registered service from the container.
-        """
-        container._instantiated[rs.svc_type] = (rs, svc)
-
-        container.forget_about(Service)
-
-        assert {} == container._instantiated
-        assert [] == container._on_close
-
-    @pytest.mark.asyncio()
-    async def test_repr(self, registry, container):
-        """
-        The repr counts correctly.
-        """
-
-        def factory():
-            yield 42
-
-        async def async_factory():
-            yield 42
-
-        registry.register_factory(Service, factory)
-        registry.register_factory(AnotherService, async_factory)
-
-        container.get(Service)
-        await container.aget(AnotherService)
-
-        assert "<Container(instantiated=2, cleanups=2)>" == repr(container)
-
-    def test_cleanup_called(self, registry, container):
-        """
-        Services that have a cleanup have them called on cleanup.
-        """
-        cleaned_up = False
-
-        def factory():
-            nonlocal cleaned_up
-            yield 42
-            cleaned_up = True
-
-        registry.register_factory(Service, factory)
-
-        container.get(Service)
-
-        assert not cleaned_up
-
-        container.close()
-
-        assert cleaned_up
-        assert not container._instantiated
-        assert not container._on_close
-
-    def test_close_resilient(self, container, registry, caplog):
-        """
-        Failing cleanups are logged and ignored. They do not break the
-        cleanup process.
-        """
-
-        def factory():
-            yield 1
-            raise Exception
-
-        cleaned_up = False
-
-        def factory_no_boom():
-            nonlocal cleaned_up
-
-            yield 3
-
-            cleaned_up = True
-
-        registry.register_factory(Service, factory)
-        registry.register_factory(YetAnotherService, factory_no_boom)
-
-        assert 1 == container.get(Service)
-        assert 3 == container.get(YetAnotherService)
-
-        assert not cleaned_up
-
-        container.close()
-
-        assert "tests.test_core.Service" == caplog.records[0].svcs_service_name
-        assert cleaned_up
-
-    def test_warns_if_generator_does_not_stop_after_cleanup(
-        self, registry, container
-    ):
-        """
-        If a generator doesn't stop after cleanup, a warning is emitted.
-        """
-
-        def factory():
-            yield Service()
-            yield 42
-
-        registry.register_factory(Service, factory)
-
-        container.get(Service)
-
-        with pytest.warns(UserWarning) as wi:
-            container.close()
-
-        assert (
-            "Container clean up for 'tests.test_core.Service' "
-            "didn't stop iterating." == wi.pop().message.args[0]
-        )
-
-
-class TestRegisteredService:
-    def test_repr(self, rs):
-        """
-        repr uses the fully-qualified name of a svc type.
-        """
-
-        assert (
-            "<RegisteredService(svc_type=tests.test_core.Service, has_ping=False)>"
-        ) == repr(rs)
-
-    def test_name(self, rs):
-        """
-        The name property deducts the correct class name.
-        """
-
-        assert "tests.test_core.Service" == rs.name
-
-    def test_is_async_yep(self):
-        """
-        The is_async property returns True if the factory needs to be awaited.
-        """
-
-        async def factory():
-            return 42
-
-        async def factory_cleanup():
-            await asyncio.sleep(0)
-            yield 42
-
-        assert svcs.RegisteredService(object, factory, None).is_async
-        assert svcs.RegisteredService(object, factory_cleanup, None).is_async
 
-    def test_is_async_nope(self):
-        """
-        is_async is False for sync factories.
-        """
-
-        def factory():
-            return 42
-
-        def factory_cleanup():
-            yield 42
-
-        assert not svcs.RegisteredService(object, factory, None).is_async
-        assert not svcs.RegisteredService(
-            object, factory_cleanup, None
-        ).is_async
-
-
-class TestServicePing:
-    def test_name(self, rs):
-        """
-        The name property proxies the correct class name.
-        """
-
-        assert "tests.test_core.Service" == svcs.ServicePing(None, rs).name
-
-    def test_ping(self, registry, container):
-        """
-        Calling ping instantiates the service using its factory, appends it to
-        the cleanup list, and calls the service's ping method.
-        """
-
-        cleaned_up = False
-
-        def factory():
-            nonlocal cleaned_up
-            yield Service()
-            cleaned_up = True
-
-        ping = Mock(spec_set=["__call__"])
-        registry.register_factory(Service, factory, ping=ping)
-
-        (svc_ping,) = container.get_pings()
-
-        svc_ping.ping()
+        assert "<svcs.Registry(num_services=2)>" == repr(registry)
 
-        ping.assert_called_once()
-
-        assert not cleaned_up
-
-        container.close()
-
-        assert cleaned_up
-        assert not container._instantiated
-        assert not container._on_close
-
-
-class TestRegistry:
     def test_empty_close(self):
         """
         Closing an empty registry does nothing.
         """
         svcs.Registry().close()
 
         with contextlib.closing(svcs.Registry()):
@@ -348,30 +95,68 @@
         async def hook():
             ...
 
         registry.register_factory(Service, Service, on_registry_close=hook)
 
         with pytest.warns(
             UserWarning,
-            match="Skipped async cleanup for 'tests.test_core.Service'.",
+            match="Skipped async cleanup for 'tests.ifaces.Service'.",
         ):
             registry.close()
 
     def test_close_logs_failures(self, registry, caplog):
         """
         Closing failures are logged but ignored.
         """
         registry.register_factory(
             Service, Service, on_registry_close=Mock(side_effect=ValueError())
         )
 
         with contextlib.closing(registry):
             ...
 
-        assert "tests.test_core.Service" == caplog.records[0].svcs_service_name
+        assert "tests.ifaces.Service" == caplog.records[0].svcs_service_name
+
+    def test_detects_async_factories(self, registry):
+        """
+        The is_async property of the RegisteredService is True if the factory
+        needs to be awaited.
+        """
+
+        registry.register_factory(int, async_int_factory)
+        registry.register_factory(str, async_str_cleanup_factory)
+
+        assert (
+            svcs.RegisteredService(int, async_int_factory, False, True, None)
+            == registry._services[int]
+        )
+        assert (
+            svcs.RegisteredService(
+                str, async_str_cleanup_factory, False, True, None
+            )
+            == registry._services[str]
+        )
+
+    def test_no_false_positive_async(self, registry):
+        """
+        is_async is False for sync factories.
+        """
+        registry.register_factory(int, int_factory)
+        registry.register_factory(str, str_cleanup_factory)
+
+        assert (
+            svcs.RegisteredService(int, int_factory, False, False, None)
+            == registry._services[int]
+        )
+        assert (
+            svcs.RegisteredService(
+                str, str_cleanup_factory, False, False, None
+            )
+            == registry._services[str]
+        )
 
     @pytest.mark.skipif(
         not hasattr(contextlib, "aclosing"),
         reason="Hasn't contextlib.aclosing()",
     )
     @pytest.mark.asyncio()
     async def test_async_empty_close(self, registry):
@@ -418,8 +203,108 @@
             Service,
             on_registry_close=close_mock,
         )
 
         await registry.aclose()
 
         close_mock.assert_awaited_once()
-        assert "tests.test_core.Service" == caplog.records[0].svcs_service_name
+        assert "tests.ifaces.Service" == caplog.records[0].svcs_service_name
+
+
+class TestRegisteredService:
+    def test_repr(self, rs):
+        """
+        repr uses the fully-qualified name of a svc type.
+        """
+
+        assert (
+            "<RegisteredService(svc_type=tests.ifaces.Service, "
+            "<class 'tests.ifaces.Service'>, takes_container=False, "
+            "has_ping=False"
+            ")>"
+        ) == repr(rs)
+
+    def test_name(self, rs):
+        """
+        The name property deducts the correct class name.
+        """
+
+        assert "tests.ifaces.Service" == rs.name
+
+
+def wrong_annotation(foo: svcs.Registry) -> int:
+    ...
+
+
+def no_args():
+    ...
+
+
+def diff_name():
+    ...
+
+
+class TestTakesContainer:
+    @pytest.mark.parametrize(
+        "factory",
+        [no_args, diff_name, wrong_annotation],
+    )
+    def test_nope(self, factory):
+        """
+        Functions with different names and annotations are ignored.
+        """
+        assert not svcs._core._takes_container(factory)
+
+    def test_name(self):
+        """
+        Return True if the name is `svcs_container`.
+        """
+
+        def factory(svcs_container):
+            ...
+
+        assert svcs._core._takes_container(factory)
+
+    def test_annotation(self):
+        """
+        Return true if the first argument is annotated as `svcs.Container`.
+        """
+
+        def factory(foo: svcs.Container):
+            ...
+
+        assert svcs._core._takes_container(factory)
+
+    def test_annotation_str(self):
+        """
+        Return true if the first argument is annotated as `svcs.Container`
+        using a string.
+        """
+
+        def factory(bar: "svcs.Container"):
+            ...
+
+        assert svcs._core._takes_container(factory)
+
+    def test_catches_invalid_sigs(self):
+        """
+        If the factory takes more than one parameter, raise an TypeError.
+        """
+
+        def factory(foo, bar):
+            ...
+
+        with pytest.raises(
+            TypeError, match="Factories must take 0 or 1 parameters."
+        ):
+            svcs._core._takes_container(factory)
+
+    def test_call_works(self):
+        """
+        Does not raise if the factory is a class with __call__.
+        """
+
+        class Factory:
+            def __call__(self, svcs_container):
+                ...
+
+        assert svcs._core._takes_container(Factory())
```

### Comparing `svcs-23.6.0/tests/test_flask.py` & `svcs-23.7.0/tests/test_flask.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 from unittest.mock import Mock
 
 import pytest
 
 import svcs
 
+from .fake_factories import nop
+from .ifaces import AnotherService, Interface, Service
+
 
 try:
     import flask
 
     from svcs.flask import teardown
 except ImportError:
     pytest.skip("Flask not installed", allow_module_level=True)
@@ -30,91 +33,79 @@
 
 
 @pytest.fixture(name="container")
 def _container(clean_app_ctx):
     return svcs.flask._ensure_req_data()[1]
 
 
-class Interface:
-    pass
-
-
-class Service1:
-    pass
-
-
-class Service2:
-    pass
-
-
 @pytest.mark.usefixtures("clean_app_ctx")
 class TestFlask:
     def test_cleanup_added(self, registry):
         """
         get() handles the case where there is already a cleanup registered.
         """
 
         cleanup1 = Mock()
         cleanup2 = Mock()
 
         def factory1():
-            yield Service1()
+            yield Service()
             cleanup1()
 
         def factory2():
-            yield Service2()
+            yield AnotherService()
             cleanup2()
 
-        registry.register_factory(Service1, factory1)
-        svcs.flask.replace_factory(Service2, factory2)
+        registry.register_factory(Service, factory1)
+        svcs.flask.replace_factory(AnotherService, factory2)
 
-        svc1 = svcs.flask.get(Service1)
-        svc2 = svcs.flask.get(Service2)
+        svc1 = svcs.flask.get(Service)
+        svc2 = svcs.flask.get(AnotherService)
 
-        assert isinstance(svc1, Service1)
-        assert isinstance(svc2, Service2)
+        assert isinstance(svc1, Service)
+        assert isinstance(svc2, AnotherService)
         assert 2 == len(flask.g.svcs_container._on_close)
 
         teardown(None)
 
         cleanup1.assert_called_once_with()
         cleanup2.assert_called_once_with()
 
     def test_overwrite_value(self, registry):
         """
         It's possible to overwrite an already registered type.
         """
-        registry.register_value(Interface, Interface(), ping=lambda _: None)
+        registry.register_value(Interface, Service(), ping=nop)
 
         assert isinstance(svcs.flask.get(Interface), Interface)
 
-        svcs.flask.replace_value(Interface, Service2())
+        svcs.flask.replace_value(Interface, AnotherService())
 
-        assert isinstance(svcs.flask.get(Interface), Service2)
+        assert isinstance(svcs.flask.get(Interface), AnotherService)
         assert [] == svcs.flask.get_pings()
 
-    def test_overwrite_factory(self, container):
+    def test_overwrite_factory(self):
         """
         It's possible to overwrite an already registered type using a factory.
         """
-        svcs.flask.replace_value(Interface, Interface(), ping=lambda _: None)
+        svcs.flask.replace_value(Interface, Service(), ping=nop)
 
         assert isinstance(svcs.flask.get(Interface), Interface)
 
-        svcs.flask.replace_factory(Interface, Service2)
+        svcs.flask.replace_factory(Interface, AnotherService)
 
-        assert isinstance(svcs.flask.get(Interface), Service2)
+        assert isinstance(svcs.flask.get(Interface), AnotherService)
         assert [] == svcs.flask.get_pings()
 
     def test_cache(self):
         """
         Getting a service twice within the same request returns the same
         object.
         """
-        svcs.flask.replace_factory(Interface, Service1)
+        svcs.flask.replace_factory(Interface, Service)
 
         assert svcs.flask.get(Interface) is svcs.flask.get(Interface)
 
     def test_not_found(self):
         """
         Trying to get a service that hasn't been registered raises a
         ServiceNotFoundError.
@@ -122,81 +113,81 @@
         with pytest.raises(svcs.exceptions.ServiceNotFoundError):
             svcs.flask.get(Interface)
 
     def test_get_pingeable(self):
         """
         get_pingable returns only pingable svcs.
         """
-        svcs.flask.replace_factory(Service1, Service1)
-        svcs.flask.replace_factory(Service2, Service2, ping=lambda _: None)
+        svcs.flask.replace_factory(Service, Service)
+        svcs.flask.replace_factory(AnotherService, AnotherService, ping=nop)
 
-        assert [Service2] == [
+        assert [AnotherService] == [
             ping._rs.svc_type for ping in svcs.flask.get_pings()
         ]
 
     def test_cleanup_purge_tolerant(self, container):
         """
         If other svcs are registered, they are ignored by the cleanup
         purge.
         """
 
         def factory1():
-            yield Service1()
+            yield Service()
 
         def factory2():
-            yield Service2()
+            yield AnotherService()
 
-        svcs.flask.replace_factory(Service1, factory1)
-        svcs.flask.replace_factory(Service2, factory2)
+        svcs.flask.replace_factory(Interface, factory1)
+        svcs.flask.replace_factory(AnotherService, factory2)
 
-        svcs.flask.get(Service1)
-        svcs.flask.get(Service2)
+        svcs.flask.get(Interface)
+        svcs.flask.get(AnotherService)
 
         assert 2 == len(container._on_close)
 
-        svcs.flask.replace_factory(Service1, Interface)
+        svcs.flask.replace_factory(Interface, Service)
 
-        svcs.flask.get(Service1)
-        svcs.flask.get(Service2)
+        svcs.flask.get(Interface)
+        svcs.flask.get(AnotherService)
 
         assert 2 == len(container._on_close)
 
     @pytest.mark.asyncio()
     async def test_teardown_warns_on_async_on_close(self, container):
         """
         teardown() warns if there are async cleanups.
         """
 
         async def factory():
-            yield Service1()
+            yield Service()
 
-        svcs.flask.replace_factory(Service1, factory)
+        svcs.flask.replace_factory(Service, factory)
 
-        await container.aget(Service1)
+        await container.aget(Service)
 
         with pytest.warns(UserWarning) as wi:
             teardown(None)
 
         w = wi.pop()
 
         assert 0 == len(wi.list)
         assert (
-            "Skipped async cleanup for 'tests.test_flask.Service1'. "
+            "Skipped async cleanup for 'tests.ifaces.Service'. "
             "Use aclose() instead." == w.message.args[0]
         )
 
 
 class TestNonContextHelpers:
     def test_register_factory_helper(self, registry, app):
         """
         register_factory() registers a factory to the app that is passed.
         """
         svcs.flask.init_app(app, registry)
 
-        svcs.flask.register_factory(app, Interface, Service1)
+        svcs.flask.register_factory(app, Interface, Service)
 
         assert Interface in registry._services
 
     def test_register_value_helper(self, registry, app):
         """
         register_value() registers a value to the app that is passed.
         """
@@ -215,15 +206,15 @@
         app = flask.Flask("tests")
         svcs.flask.init_app(app)
 
         assert isinstance(app.config["svcs_registry"], svcs.Registry)
 
     def test_explicit_registry(self):
         """
-        If a registry is passsed to init_app(), it's used.
+        If a registry is passed to init_app(), it's used.
         """
         registry = svcs.Registry()
         app = flask.Flask("tests")
         svcs.flask.init_app(app, registry)
 
         assert registry is app.config["svcs_registry"]
 
@@ -241,13 +232,13 @@
         close_registry() runs the registry's close() method.
         """
         close = Mock()
 
         svcs.flask.init_app(app)
 
         svcs.flask.register_factory(
-            app, Interface, Service1, on_registry_close=close
+            app, Interface, Service, on_registry_close=close
         )
 
         svcs.flask.close_registry(app)
 
         assert close.called
```

### Comparing `svcs-23.6.0/tests/typing/core.py` & `svcs-23.7.0/tests/typing/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     yield 42
 
 
 def factory_with_cleanup() -> Generator[int, None, None]:
     yield 1
 
 
+def factory_that_takes_container_by_annotation(foo: svcs.Container) -> int:
+    return 1
+
+
 async def async_ping() -> None:
     pass
 
 
 reg.register_value(int, 1)
 reg.register_value(int, 1, ping=lambda: None)
 reg.register_value(int, 1, ping=async_ping)
```

### Comparing `svcs-23.6.0/tests/typing/flask_.py` & `svcs-23.7.0/tests/typing/flask_.py`

 * *Files identical despite different names*

### Comparing `svcs-23.6.0/LICENSE` & `svcs-23.7.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Hynek Schlawack
+Copyright (c) 2023 Hynek Schlawack and the svcs contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `svcs-23.6.0/pyproject.toml` & `svcs-23.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 
 [project]
 dynamic = ["version", "readme"]
 name = "svcs"
 description = "A Lightweight Service Locator"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = ["dependency injection"]
 authors = [{ name = "Hynek Schlawack", email = "hs@ox.cx" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Typing :: Typed",
 ]
-dependencies = ["attrs"]
+dependencies = [
+  "attrs>=21.3.0", # attrs namespace
+]
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-asyncio", "sybil"]
 typing = ["mypy>=1.4", "flask"]
 dev = ["svcs[tests,typing]", "tox>4", "flask"]
 
 [project.urls]
@@ -44,17 +45,14 @@
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 start-after = "<!-- begin-logo -->\n"
 end-before = "\n<!-- end-logo -->"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
-text = "\n\n# *svcs*: A Lightweight Service Locator\n\n"
-
-[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 start-after = "<!-- begin-pypi -->\n"
 end-before = "\n<!-- end-pypi -->"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 
@@ -81,25 +79,37 @@
 
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 start-at = "## Credits"
 
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
+pattern = '> \[!(.*)\]'
+replacement = '> **\1**'
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
+pattern = ']\(\./(.*)\)'
+replacement = '](https://github.com/hynek/svcs/blob/main/\1)'
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
+pattern = '(docs/_static/.*")'
+replacement = 'https://raw.githubusercontent.com/hynek/svcs/main/\1"'
+
 
 [tool.pytest.ini_options]
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["once::Warning"]
 
 
 [tool.coverage.run]
 branch = true
 parallel = true
-source = ["svcs"]
+source = ["svcs", "tests"]
 
 [tool.coverage.paths]
 source = ["src", ".tox/py*/**/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
```

### Comparing `svcs-23.6.0/PKG-INFO` & `svcs-23.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: svcs
-Version: 23.6.0
+Version: 23.7.0
 Summary: A Lightweight Service Locator
 Project-URL: Changelog, https://github.com/hynek/svcs/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/hynek/svcs/blob/main/README.md
 Project-URL: Source, https://github.com/hynek/svcs
 Project-URL: Funding, https://github.com/sponsors/hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
 License-Expression: MIT
 License-File: LICENSE
-Keywords: dependency injection
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: attrs
+Requires-Dist: attrs>=21.3.0
 Provides-Extra: dev
 Requires-Dist: flask; extra == 'dev'
 Requires-Dist: svcs[tests,typing]; extra == 'dev'
 Requires-Dist: tox>4; extra == 'dev'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-asyncio; extra == 'tests'
@@ -31,23 +30,23 @@
 Provides-Extra: typing
 Requires-Dist: flask; extra == 'typing'
 Requires-Dist: mypy>=1.4; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
-    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="20%" alt="svcs" />
+    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo_with_name.svg" width="25%" alt="svcs logo showing a radar"" />
   </a>
 </p>
 
-# *svcs*: A Lightweight Service Locator
-
+<p align="center">
+  A Lightweight Service Locator for Python.
+</p>
 
-> **Warning**
-> ☠️ Not ready yet! ☠️
+> **WARNING** ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
@@ -61,42 +60,40 @@
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
 All of this happens *within* your application – service locators are **not** related to service discovery.
 
-If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
+If you follow the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [*abstract base class*](https://docs.python.org/3.11/library/abc.html).
 
 Benefits:
 
 - Eliminates tons of repetitive **boilerplate** code,
 - unifies **acquisition** and **cleanups** of resources,
 - simplifies **testing**,
 - and allows for easy **health checks** across *all* resources.
 
-No global mutable state is necessary – but possible for extra comfort.
-
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
     db = request.services.get(Database)
     api = request.services.get(WebAPIClient)
 ```
 
-or even:
+or, if you don't shy away from some global state, even:
 
 ```python
 def view():
     db = services.get(Database)
     api = services.get(WebAPIClient)
 ```
 
-The latter already works with [Flask](#flask).
+The latter already works with [Flask](#flask) by utilizing the [`g` object](https://flask.palletsprojects.com/en/latest/api/#flask.g).
 
 You set it up like this:
 
 <!--
 ; skip: next
 -->
 
@@ -121,19 +118,23 @@
 )
 
 @atexit.register
 def cleanup():
     registry.close()  # calls engine.dispose()
 ```
 
-The generator-based setup and cleanup may remind you of [Pytest fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
+The generator-based setup and cleanup may remind you of [*pytest* fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
 The hooks that are defined as `on_registry_close` are called when you call `Registry.close()` – e.g. when your application is shutting down.
 
 *svcs* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
 
+> **IMPORTANT**
+> All of this may look over-engineered if you have only one or two resources.
+> However, it starts paying dividends *very fast* once you go past that.
+
 
 ## Is this Dependency Injection!?
 
 No.
 
 Although the concepts are related and share the idea of having a central registry of services, the ways they provide those services are fundamentally different:
 [Dependency injection](https://en.wikipedia.org/wiki/Dependency_injection) always passes your dependencies as arguments while you actively ask a service locator for them when you need them.
@@ -156,34 +157,34 @@
         )
 
     raise InvalidFormError()
 ```
 
 The main downside is that it's impossible to verify whether all required dependencies have been configured without running the code.
 
+If you still prefer dependency injection, check out [*incant*](https://github.com/Tinche/incant).
+
 ---
 
 For now, please refer to the [GitHub README](https://github.com/hynek/svcs/blob/main/README.md) for latest documentation.
 
 
 ## Release Information
 
-### Changed
-
-- Renamed `Container.forget_service_type()` to `Container.forget_about()`.
-
-
-### Fixed
+### Added
 
-- `svcs.flask.init_app()`'s type hints now take into account custom `flask.Flask` subclasses.
+- Factories now may take a parameter called `svcs_container` or that is annotated to be `svcs.Container`.
+  In this case the factory will receive the current container as a first positional argument.
+  This allows for recursive factories without global state.
+  [#10](https://github.com/hynek/svcs/pull/10)
 
 
 ---
 
 [→ Full Changelog](https://github.com/hynek/svcs/blob/main/CHANGELOG.md)
 
 
 ## Credits
 
-*svcs* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+*svcs* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](https://github.com/hynek/svcs/blob/main/LICENSE) license.
 
 The development is kindly supported by my employer [Variomedia AG](https://www.variomedia.de/) and all my amazing [GitHub Sponsors](https://github.com/sponsors/hynek).
```

