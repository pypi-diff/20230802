# Comparing `tmp/pydantic_compat-0.0.3.tar.gz` & `tmp/pydantic_compat-0.0.4.tar.gz`

## Comparing `pydantic_compat-0.0.3.tar` & `pydantic_compat-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/__init__.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_shared.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v1_decorators.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v1_mixin.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v2_decorators.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/_v2_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/src/pydantic_compat/py.typed
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/tests/test_base_model.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/tests/test_decorators.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/.gitignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/LICENSE
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/README.md
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pydantic_compat-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/__init__.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/py.typed
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/_v1/__init__.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/_v1/decorators.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/_v1/mixin.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/_v2/__init__.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/_v2/decorators.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/src/pydantic_compat/_v2/mixin.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/tests/test_base_model.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/tests/test_decorators.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/tests/test_fields.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/README.md
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7960 2020-02-02 00:00:00.000000 pydantic_compat-0.0.4/PKG-INFO
```

### Comparing `pydantic_compat-0.0.3/src/pydantic_compat/__init__.py` & `pydantic_compat-0.0.4/src/pydantic_compat/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """CompatibilityMixin for pydantic v1/1/v2."""
 
 try:
     from importlib.metadata import PackageNotFoundError, version
 except ImportError:
-    from importlib_metadata import PackageNotFoundError, version
+    from importlib_metadata import PackageNotFoundError, version  # type: ignore
 
 from typing import TYPE_CHECKING
 
 try:
     __version__ = version("pydantic-compat")
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "uninstalled"
@@ -18,34 +18,54 @@
     "__version__",
     "field_validator",
     "model_validator",
     "PYDANTIC2",
     "PydanticCompatMixin",
     "root_validator",
     "validator",
+    "Field",
+    "BaseModel",
 ]
 
 from ._shared import PYDANTIC2
 
 if TYPE_CHECKING:
-    from pydantic import field_validator, model_validator, root_validator, validator
+    from pydantic import (
+        Field,
+        field_validator,
+        model_validator,
+        root_validator,
+        validator,
+    )
 
     # using this to avoid breaking pydantic mypy plugin
-    # not that it will be hard to provide proper names AND proper signatures for
-    # both versions of pydantic without a ton of potentially outdated signatures
+    # not that we could use a protocol. but it will be hard to provide proper names
+    # AND proper signatures for both versions of pydantic without a ton of potentially
+    # outdated signatures
     PydanticCompatMixin = type
+else:
+    from ._shared import Field
 
-elif PYDANTIC2:
-    from pydantic import field_validator, model_validator
+    if PYDANTIC2:
+        from pydantic import field_validator, model_validator
 
-    from ._v2_decorators import root_validator, validator
-    from ._v2_mixin import PydanticCompatMixin
+        from ._v2 import PydanticCompatMixin, root_validator, validator
 
-else:
-    from pydantic import validator  # type: ignore
+    else:
+        from pydantic import validator
 
-    from ._v1_decorators import (  # type: ignore
-        field_validator,
-        model_validator,
-        root_validator,
-    )
-    from ._v1_mixin import PydanticCompatMixin  # type: ignore
+        from ._v1 import (
+            PydanticCompatMixin,
+            field_validator,
+            model_validator,
+            root_validator,
+        )
+
+
+import pydantic
+
+
+class BaseModel(PydanticCompatMixin, pydantic.BaseModel):
+    """BaseModel with pydantic_compat mixins."""
+
+
+del pydantic
```

### Comparing `pydantic_compat-0.0.3/src/pydantic_compat/_v1_decorators.py` & `pydantic_compat-0.0.4/src/pydantic_compat/_v1/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from __future__ import annotations
 
 from functools import wraps
-from typing import TYPE_CHECKING, Callable
-
-import pydantic.version
-
-if not pydantic.version.VERSION.startswith("1"):  # pragma: no cover
-    raise ImportError("pydantic_compat._v1 only supports pydantic v1.x")
+from typing import TYPE_CHECKING, Any, Callable
 
 import pydantic
 
 if TYPE_CHECKING:
     from typing import Literal
 
 
@@ -40,15 +35,15 @@
         always=True,  # should it be?
         check_fields=bool(check_fields),
         allow_reuse=True,
     )
 
 
 # V2 signature
-def model_validator(*, mode: Literal["wrap", "before", "after"]) -> Callable:
+def model_validator(*, mode: Literal["wrap", "before", "after"]) -> Any:
     """Adaptor from v2.model_validator -> v1.root_validator."""
 
     # V1 signature
     # def root_validator(
     #     _func: Optional[AnyCallable] = None,
     #     *,
     #     pre: bool = False,
@@ -64,29 +59,30 @@
 def root_validator(
     _func: Callable | None = None,
     *,
     pre: bool = False,
     allow_reuse: bool = False,
     skip_on_failure: bool = False,
     construct_object: bool = False,
-) -> Callable:
-    def _inner(_func: Callable):
+) -> Any:
+    def _inner(_func: Callable) -> Any:
         func = _func
         if construct_object and not pre:
             if isinstance(_func, classmethod):
                 _func = _func.__func__
 
             @wraps(_func)
-            def func(cls: type[pydantic.BaseModel], *args, **kwargs):
+            def func(cls: type[pydantic.BaseModel], *args: Any, **kwargs: Any) -> Any:
                 arg0, *rest = args
                 # cast dict to model to match the v2 model_validator signature
                 # using construct because it should already be valid
                 new_args = (cls.construct(**arg0), *rest)
-                result: pydantic.BaseModel= _func(cls, *new_args, **kwargs)
+                result: pydantic.BaseModel = _func(cls, *new_args, **kwargs)
                 # cast back to dict of field -> value
                 return {k: getattr(result, k) for k in result.__fields__}
 
-        return pydantic.root_validator(
-            func, pre=pre, allow_reuse=allow_reuse, skip_on_failure=skip_on_failure
+        deco = pydantic.root_validator(  # type: ignore [call-overload]
+            pre=pre, allow_reuse=allow_reuse, skip_on_failure=skip_on_failure
         )
+        return deco(func)
 
     return _inner(_func) if _func else _inner
```

### Comparing `pydantic_compat-0.0.3/src/pydantic_compat/_v1_mixin.py` & `pydantic_compat-0.0.4/src/pydantic_compat/_v1/mixin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 from __future__ import annotations
 
 import sys
-from typing import TYPE_CHECKING, Any, Iterator, Mapping, TypeVar
-
-import pydantic.version
-
-if not pydantic.version.VERSION.startswith("1"):  # pragma: no cover
-    raise ImportError("pydantic_compat._v1 only supports pydantic v1.x")
+from typing import TYPE_CHECKING, Any, ClassVar, Iterator, Mapping
 
 from pydantic import main
 
-from ._shared import V2_RENAMED_CONFIG_KEYS, _check_mixin_order
+from pydantic_compat._shared import V2_RENAMED_CONFIG_KEYS, check_mixin_order
 
 if TYPE_CHECKING:
-    from pydantic.fields import ModelField
+    from typing import Dict
 
-    BM = TypeVar("BM", bound=main.BaseModel)
+    from pydantic.fields import ModelField  # type: ignore
+    from typing_extensions import Protocol
 
+    # fmt:off
+    class Model(Protocol):
+        def dict(self, *args: Any, **kwargs: Any) ->  Dict[str, Any]: ...  # noqa: UP006
+        def json(self, *args: Any, **kwargs: Any) -> str: ...
+        def copy(self, *args: Any, **kwargs: Any) -> Model: ...
+        @classmethod
+        def schema(cls, *args: Any, **kwargs: Any) -> Dict[str, Any]: ...  # noqa: UP006
+        @classmethod
+        def validate(cls, *args: Any, **kwargs: Any) -> Model: ...
+        @classmethod
+        def construct(cls, *args: Any, **kwargs: Any) -> Model: ...
+        @classmethod
+        def parse_raw(cls, *args: Any, **kwargs: Any) -> type[Model]: ...
+        @classmethod
+        def update_forward_refs(cls, *args: Any, **kwargs: Any) -> None: ...
+
+        __fields__: ClassVar[Dict]  # noqa: UP006
+        __fields_set__: set[str]
+        __config__: ClassVar[type]
+    # fmt:on
 
 if sys.version_info < (3, 9):
 
     def _get_fields(obj) -> dict[str, Any]:
         return obj.__fields__
 
     main.ModelMetaclass.model_fields = property(_get_fields)
@@ -33,80 +49,80 @@
     for k in sorted(deprecated_renamed_keys):
         config_dict[REVERSE_CONFIG_NAME_MAP[k]] = config_dict.pop(k)
 
     return type("Config", (), config_dict)
 
 
 class _MixinMeta(main.ModelMetaclass):
-    def __new__(mcs, name, bases, namespace, **kwargs):
+    def __new__(cls, name, bases, namespace: dict, **kwargs):  # type: ignore
         if "model_config" in namespace and isinstance(namespace["model_config"], dict):
             namespace["Config"] = _convert_config(namespace.pop("model_config"))
 
-        return super().__new__(mcs, name, bases, namespace, **kwargs)
+        return super().__new__(cls, name, bases, namespace, **kwargs)
 
 
 class PydanticCompatMixin(metaclass=_MixinMeta):
     @classmethod
     def __try_update_forward_refs__(cls, **localns: Any) -> None:
         sup = super()
         if hasattr(sup, "__try_update_forward_refs__"):
             sup.__try_update_forward_refs__(**localns)
 
     def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
-        _check_mixin_order(cls, PydanticCompatMixin, main.BaseModel)
+        check_mixin_order(cls, PydanticCompatMixin, main.BaseModel)
 
-    def model_dump(self: BM, *args: Any, **kwargs: Any) -> Any:
+    def model_dump(self: Model, *args: Any, **kwargs: Any) -> Any:
         return self.dict(*args, **kwargs)
 
-    def model_dump_json(self: BM, *args: Any, **kwargs: Any) -> Any:
+    def model_dump_json(self: Model, *args: Any, **kwargs: Any) -> Any:
         return self.json(*args, **kwargs)
 
-    def model_copy(self: BM, *args: Any, **kwargs: Any) -> Any:
+    def model_copy(self: Model, *args: Any, **kwargs: Any) -> Any:
         return self.copy(*args, **kwargs)
 
     @classmethod
-    def model_json_schema(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def model_json_schema(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.schema(*args, **kwargs)
 
     @classmethod
-    def model_validate(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def model_validate(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.validate(*args, **kwargs)
 
     @classmethod
-    def model_construct(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def model_construct(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.construct(*args, **kwargs)
 
     @classmethod
-    def model_validate_json(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def model_validate_json(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.parse_raw(*args, **kwargs)
 
     @classmethod
-    def model_rebuild(cls: type[BM], force: bool = True, **kwargs: Any) -> None:
+    def model_rebuild(cls: type[Model], force: bool = True, **kwargs: Any) -> None:
         return cls.update_forward_refs(**kwargs)
 
     if sys.version_info < (3, 9):
         # differences in the behavior of patching class properties in python<3.9
         @property
-        def model_fields(cls: type[BM]) -> Mapping[str, Any]:
+        def model_fields(cls: type[Model]) -> Mapping[str, Any]:
             return FieldInfoMap(cls.__fields__)
 
     else:
 
-        @classmethod  # type: ignore
+        @classmethod  # type: ignore [misc]
         @property
-        def model_fields(cls: type[BM]) -> Mapping[str, Any]:
+        def model_fields(cls: type[Model]) -> Mapping[str, Any]:
             return FieldInfoMap(cls.__fields__)
 
     @property
-    def model_fields_set(self: BM) -> set[str]:
-        return self.__fields_set__  # type: ignore
+    def model_fields_set(self: Model) -> set[str]:
+        return self.__fields_set__
 
-    @classmethod  # type: ignore
+    @classmethod  # type: ignore [misc]
     @property
-    def model_config(cls: type[BM]) -> Mapping[str, Any]:
+    def model_config(cls: type[Model]) -> Mapping[str, Any]:
         return DictLike(cls.__config__)
 
 
 class FieldInfoLike:
     """Wrapper to convera pydantic v1 ModelField to v2 FieldInfo."""
 
     def __init__(self, model_field: ModelField) -> None:
```

### Comparing `pydantic_compat-0.0.3/src/pydantic_compat/_v2_decorators.py` & `pydantic_compat-0.0.4/src/pydantic_compat/_v2/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 from __future__ import annotations
 
-from typing import Any, Callable
-
-import pydantic.version
-
-if int(pydantic.version.VERSION[0]) <= 1:  # pragma: no cover
-    raise ImportError("pydantic_compat._v2 only supports pydantic v2.x")
-
 import warnings
+from typing import Any, Callable
 
 from pydantic.deprecated import class_validators
 
 
 # V1 signature
 # def validator(
 #     *fields: str,
@@ -63,13 +57,13 @@
             "instead. (It works for both versions)."
         )
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", DeprecationWarning)
 
         # def model_validator( *, mode: Literal['wrap', 'before', 'after']) -> Any:
-        return class_validators.root_validator(  # type: ignore
+        return class_validators.root_validator(  # type: ignore [call-overload]
             *_args,
             pre=pre,
             skip_on_failure=bool(skip_on_failure),
             allow_reuse=allow_reuse,
         )
```

### Comparing `pydantic_compat-0.0.3/src/pydantic_compat/_v2_mixin.py` & `pydantic_compat-0.0.4/src/pydantic_compat/_v2/mixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,119 @@
 from __future__ import annotations
 
-import pydantic.version
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, cast
 
-if int(pydantic.version.VERSION[0]) <= 1:  # pragma: no cover
-    raise ImportError("pydantic_compat._v2 only supports pydantic v2.x")
-
-from typing import TYPE_CHECKING, Any, TypeVar, cast
-
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel
 from pydantic._internal import _model_construction
 
-from ._shared import V2_RENAMED_CONFIG_KEYS, _check_mixin_order
+from pydantic_compat._shared import V2_RENAMED_CONFIG_KEYS, check_mixin_order
 
 if TYPE_CHECKING:
-    BM = TypeVar("BM", bound=BaseModel)
+    from pydantic import ConfigDict
+    from typing_extensions import Protocol
+
+    # fmt:off
+    class Model(Protocol):
+        def model_dump(self, *args: Any, **kwargs: Any) ->  dict[str, Any]: ...
+        def model_dump_json(self, *args: Any, **kwargs: Any) -> str: ...
+        def model_copy(self, *args: Any, **kwargs: Any) -> Model: ...
+        @classmethod
+        def model_json_schema(cls, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
+        @classmethod
+        def model_validate(cls, *args: Any, **kwargs: Any) -> Model: ...
+        @classmethod
+        def model_construct(cls, *args: Any, **kwargs: Any) -> Model: ...
+        @classmethod
+        def model_validate_json(cls, *args: Any, **kwargs: Any) -> type[Model]: ...
+        @classmethod
+        def model_rebuild(cls, *args: Any, **kwargs: Any) -> bool | None: ...
+
+        model_fields: ClassVar[dict]
+        model_fields_set: ClassVar[set[str]]
+        model_config: ClassVar[ConfigDict]
+    # fmt:on
 
 
 def _convert_config(config: type) -> ConfigDict:
     config_dict = {k: getattr(config, k) for k in dir(config) if not k.startswith("__")}
 
     deprecated_renamed_keys = V2_RENAMED_CONFIG_KEYS.keys() & config_dict.keys()
     for k in sorted(deprecated_renamed_keys):
         config_dict[V2_RENAMED_CONFIG_KEYS[k]] = config_dict.pop(k)
 
     # leave these here for now to warn about lost functionality
     # deprecated_removed_keys = V2_REMOVED_CONFIG_KEYS & config_dict.keys()
     # for k in sorted(deprecated_removed_keys):
     #     config_dict.pop(k)
 
-    return cast(ConfigDict, config_dict)
+    return cast("ConfigDict", config_dict)
 
 
 class _MixinMeta(_model_construction.ModelMetaclass):
-    def __new__(mcs, name, bases, namespace, **kwargs):
+    def __new__(cls, name, bases, namespace, **kwargs):  # type: ignore
         if "Config" in namespace and isinstance(namespace["Config"], type):
             namespace["model_config"] = _convert_config(namespace.pop("Config"))
-        return super().__new__(mcs, name, bases, namespace, **kwargs)
+        return super().__new__(cls, name, bases, namespace, **kwargs)
 
 
 class PydanticCompatMixin(metaclass=_MixinMeta):
     def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
-        _check_mixin_order(cls, PydanticCompatMixin, BaseModel)
+        check_mixin_order(cls, PydanticCompatMixin, BaseModel)
         # the deprecation warning is on the metaclass
-        type(cls).__fields__ = property(lambda cls: cls.model_fields)
+        type(cls).__fields__ = property(lambda cls: cls.model_fields)  # type: ignore
 
-    def dict(self: BM, *args: Any, **kwargs: Any) -> Any:
+    def dict(self: Model, *args: Any, **kwargs: Any) -> Any:
         return self.model_dump(*args, **kwargs)
 
-    def json(self: BM, *args: Any, **kwargs: Any) -> Any:
+    def json(self: Model, *args: Any, **kwargs: Any) -> Any:
         return self.model_dump_json(*args, **kwargs)
 
-    def copy(self: BM, *args: Any, **kwargs: Any) -> Any:
+    def copy(self: Model, *args: Any, **kwargs: Any) -> Any:
         return self.model_copy(*args, **kwargs)
 
     @classmethod
-    def schema(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def schema(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.model_json_schema(*args, **kwargs)
 
     @classmethod
-    def validate(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def validate(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.model_validate(*args, **kwargs)
 
     @classmethod
-    def construct(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def construct(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.model_construct(*args, **kwargs)
 
     @classmethod
-    def parse_obj(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def parse_obj(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.model_validate(*args, **kwargs)
 
     @classmethod
-    def parse_raw(cls: type[BM], *args: Any, **kwargs: Any) -> Any:
+    def parse_raw(cls: type[Model], *args: Any, **kwargs: Any) -> Any:
         return cls.model_validate_json(*args, **kwargs)
 
     # this is needed in addition to the metaclass patch in __init_subclass__
     @property
-    def __fields__(self: BM) -> dict[str, Any]:
+    def __fields__(self: Model) -> Dict[str, Any]:  # noqa: UP006
         return self.model_fields
 
     @property
-    def __fields_set__(self: BM) -> set[str]:
+    def __fields_set__(self: Model) -> set[str]:
         return self.model_fields_set
 
     @classmethod
     def update_forward_refs(
-        cls: type[BM],
+        cls: type[Model],
         force: bool = False,
         raise_errors: bool = True,
         **localns: Any,
     ) -> None:
         cls.model_rebuild(
             forc=force, raise_errors=raise_errors, _types_namespace=localns
         )
 
     @classmethod
     def model_rebuild(
-        cls: type[BM], force: bool = False, raise_errors: bool = True, **kwargs: Any
-    ) -> None:
+        cls: type[Model], force: bool = False, raise_errors: bool = True, **kwargs: Any
+    ) -> bool | None:
         return super().model_rebuild(
             force=force, raise_errors=raise_errors, _types_namespace=kwargs
         )
```

### Comparing `pydantic_compat-0.0.3/tests/test_base_model.py` & `pydantic_compat-0.0.4/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.3/tests/test_decorators.py` & `pydantic_compat-0.0.4/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.3/.gitignore` & `pydantic_compat-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.3/LICENSE` & `pydantic_compat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_compat-0.0.3/README.md` & `pydantic_compat-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 For applications, this is not a big deal, as they can pin to whatever version of
 pydantic they need. But for libraries that want to exist in a broader
 environment, pinning to a specific version of pydantic is not always an option
 (as it limits the ability to co-exist with other libraries).
 
 This package provides (unofficial) compatibility mixins and function adaptors for pydantic
 v1-v2 cross compatibility. It allows you to use either v1 or v2 API names,
-regardless of the pydantic version installed. (Prefer using v2 names when possible)
+regardless of the pydantic version installed. (Prefer using v2 names when possible).
+
+Tests are run on Pydantic v1.8 and up
 
 The API conversion is not exhaustive, but suffices for many of the use cases
 I have come across. I will be using it in:
 
 - [ome-types](https://github.com/tlambert03/ome-types)
 - [psygnal](https://github.com/pyapp-kit/psygnal)
 - [app-model](https://github.com/pyapp-kit/app-model)
@@ -31,19 +33,23 @@
 Feel free to open an issue or PR if you find it useful, but lacking features
 you need.
 
 ## What does it do?
 
 Not much! :joy:
 
-Mostly serves to translate names from one API to another. While
-pydantic2 does offer deprecated access to the v1 API, if you explicitly
-wish to support pydantic1 without your users seeing deprecation warnings,
-then you need to do a lot of name adaptation depending on the runtime
-pydantic version. This package does that for you.
+Mostly it serves to translate names from one API to another. It backports
+the v2 API to v1 (so you can v2 names in a pydantic1 runtime),
+and forwards the v1 API to v2 (so you can use v1 names in a v2 runtime
+without deprecation warnings).
+
+> While pydantic2 does offer deprecated access to the v1 API, if you explicitly
+> wish to support pydantic1 without your users seeing deprecation warnings,
+> then you need to do a lot of name adaptation depending on the runtime
+> pydantic version. This package does that for you.
 
 It does _not_ do any significantly complex translation of API logic.
 For custom types, you will still likely need to add class methods to
 support both versions of pydantic.
 
 It also does not prevent you from needing to know a what's changing
 under the hood in pydantic 2. You should be running tests on both
@@ -91,14 +97,22 @@
 | `Model.validate`            | `Model.model_validate`      |
 | `Model.parse_obj`           | `Model.model_validate`      |
 | `Model.parse_raw`           | `Model.model_validate_json` |
 | `Model.update_forward_refs` | `Model.model_rebuild`       |
 | `Model.__fields__`          | `Model.model_fields`        |
 | `Model.__fields_set__`      | `Model.model_fields_set`    |
 
+## Field notes
+
+- Don't use `var = Field(..., const='val')`, use `var: Literal['val'] = 'val'`
+  it works in both v1 and v2
+- No attempt is made to convert between v1's `unique_items` and v2's `Set[]`
+  semantics. See <https://github.com/pydantic/pydantic-core/issues/296> for
+  discussion.
+
 ## API rules
 
 - both V1 and V2 names may be used (regardless of pydantic version), but
   usage of V2 names are strongly recommended.
 - But the API must match the pydantic version matching the name you are using.
   For example, if you are using `pydantic_compat.field_validator` then the
   signature must match the pydantic (v2) `field_validator` signature (regardless)
```

### Comparing `pydantic_compat-0.0.3/pyproject.toml` & `pydantic_compat-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -39,20 +39,21 @@
 
 [tool.hatch.envs.test.scripts]
 test = "pytest -v"
 test-cov = "pytest -v --cov --cov-report=term-missing"
 test-cov-xml = "pytest -v --color=yes --cov --cov-report=xml --cov-append"
 
 [[tool.hatch.envs.test.matrix]]
-# python = ["3.7", "3.11"] # good for local, too verbose for CI
-pydantic = ["v1.8", "v1", "v2"]
+# python = ["3.8", "3.11"] # good for local, too verbose for CI
+pydantic = ["v1.8", "v1.9", "v1", "v2"]
 
 [tool.hatch.envs.test.overrides]
 matrix.pydantic.extra-dependencies = [
-    { value = "pydantic==1.8.0", if = ["v1.8"] },
+    { value = "pydantic<1.9", if = ["v1.8"] },
+    { value = "pydantic<1.10", if = ["v1.9"] },
     { value = "pydantic<2.0", if = ["v1"] },
     { value = "pydantic>=2.0", if = ["v2"] },
 ]
 
 
 
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
```

### Comparing `pydantic_compat-0.0.3/PKG-INFO` & `pydantic_compat-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-compat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Compatibility layer for pydantic v1/v2
 Project-URL: homepage, https://github.com/tlambert03/pydantic-compat
 Project-URL: repository, https://github.com/tlambert03/pydantic-compat
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -51,15 +51,17 @@
 For applications, this is not a big deal, as they can pin to whatever version of
 pydantic they need. But for libraries that want to exist in a broader
 environment, pinning to a specific version of pydantic is not always an option
 (as it limits the ability to co-exist with other libraries).
 
 This package provides (unofficial) compatibility mixins and function adaptors for pydantic
 v1-v2 cross compatibility. It allows you to use either v1 or v2 API names,
-regardless of the pydantic version installed. (Prefer using v2 names when possible)
+regardless of the pydantic version installed. (Prefer using v2 names when possible).
+
+Tests are run on Pydantic v1.8 and up
 
 The API conversion is not exhaustive, but suffices for many of the use cases
 I have come across. I will be using it in:
 
 - [ome-types](https://github.com/tlambert03/ome-types)
 - [psygnal](https://github.com/pyapp-kit/psygnal)
 - [app-model](https://github.com/pyapp-kit/app-model)
@@ -68,19 +70,23 @@
 Feel free to open an issue or PR if you find it useful, but lacking features
 you need.
 
 ## What does it do?
 
 Not much! :joy:
 
-Mostly serves to translate names from one API to another. While
-pydantic2 does offer deprecated access to the v1 API, if you explicitly
-wish to support pydantic1 without your users seeing deprecation warnings,
-then you need to do a lot of name adaptation depending on the runtime
-pydantic version. This package does that for you.
+Mostly it serves to translate names from one API to another. It backports
+the v2 API to v1 (so you can v2 names in a pydantic1 runtime),
+and forwards the v1 API to v2 (so you can use v1 names in a v2 runtime
+without deprecation warnings).
+
+> While pydantic2 does offer deprecated access to the v1 API, if you explicitly
+> wish to support pydantic1 without your users seeing deprecation warnings,
+> then you need to do a lot of name adaptation depending on the runtime
+> pydantic version. This package does that for you.
 
 It does _not_ do any significantly complex translation of API logic.
 For custom types, you will still likely need to add class methods to
 support both versions of pydantic.
 
 It also does not prevent you from needing to know a what's changing
 under the hood in pydantic 2. You should be running tests on both
@@ -128,14 +134,22 @@
 | `Model.validate`            | `Model.model_validate`      |
 | `Model.parse_obj`           | `Model.model_validate`      |
 | `Model.parse_raw`           | `Model.model_validate_json` |
 | `Model.update_forward_refs` | `Model.model_rebuild`       |
 | `Model.__fields__`          | `Model.model_fields`        |
 | `Model.__fields_set__`      | `Model.model_fields_set`    |
 
+## Field notes
+
+- Don't use `var = Field(..., const='val')`, use `var: Literal['val'] = 'val'`
+  it works in both v1 and v2
+- No attempt is made to convert between v1's `unique_items` and v2's `Set[]`
+  semantics. See <https://github.com/pydantic/pydantic-core/issues/296> for
+  discussion.
+
 ## API rules
 
 - both V1 and V2 names may be used (regardless of pydantic version), but
   usage of V2 names are strongly recommended.
 - But the API must match the pydantic version matching the name you are using.
   For example, if you are using `pydantic_compat.field_validator` then the
   signature must match the pydantic (v2) `field_validator` signature (regardless)
```

