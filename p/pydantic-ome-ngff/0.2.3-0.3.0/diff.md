# Comparing `tmp/pydantic_ome_ngff-0.2.3.tar.gz` & `tmp/pydantic_ome_ngff-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_ome_ngff-0.2.3.tar", max compression
+gzip compressed data, was "pydantic_ome_ngff-0.3.0.tar", max compression
```

## Comparing `pydantic_ome_ngff-0.2.3.tar` & `pydantic_ome_ngff-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1466 2023-02-14 18:55:46.264580 pydantic_ome_ngff-0.2.3/LICENSE
--rw-r--r--   0        0        0     1928 2023-02-27 17:33:34.485461 pydantic_ome_ngff-0.2.3/README.md
--rw-r--r--   0        0        0     1008 2023-05-11 13:42:31.501598 pydantic_ome_ngff-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       85 2023-03-22 18:16:41.323863 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/__init__.py
--rw-r--r--   0        0        0      446 2023-03-22 18:16:41.327918 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/base.py
--rw-r--r--   0        0        0      360 2023-03-08 00:10:20.528092 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/__init__.py
--rw-r--r--   0        0        0     2402 2023-05-11 13:42:02.972582 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/axes.py
--rw-r--r--   0        0        0       20 2023-03-08 00:10:20.167824 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/base.py
--rw-r--r--   0        0        0     1661 2023-05-11 13:42:02.972870 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/coordinateTransformations.py
--rw-r--r--   0        0        0      470 2023-05-11 13:42:02.973348 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/imageLabel.py
--rw-r--r--   0        0        0     8749 2023-05-11 13:42:05.518320 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/multiscales.py
--rw-r--r--   0        0        0      441 2023-05-11 13:42:02.974346 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/plate.py
--rw-r--r--   0        0        0      432 2023-05-11 13:42:02.974828 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/well.py
--rw-r--r--   0        0        0        0 2023-03-22 18:28:17.442462 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/py.typed
--rw-r--r--   0        0        0     1690 2023-05-11 13:42:02.975172 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/tree.py
--rw-r--r--   0        0        0      441 2023-03-20 21:12:39.874223 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/utils.py
--rw-r--r--   0        0        0      430 2023-03-08 00:10:20.188881 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/__init__.py
--rw-r--r--   0        0        0     3851 2023-05-11 13:42:02.975993 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/axes.py
--rw-r--r--   0        0        0       16 2023-03-08 00:10:20.185875 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/base.py
--rw-r--r--   0        0        0     2307 2023-05-11 13:42:02.976547 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/coordinateTransformations.py
--rw-r--r--   0        0        0     2136 2023-05-11 13:42:02.977224 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/imageLabel.py
--rw-r--r--   0        0        0     8753 2023-05-11 13:42:05.519709 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/multiscales.py
--rw-r--r--   0        0        0      920 2023-05-11 13:42:02.978134 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/plate.py
--rw-r--r--   0        0        0      560 2023-05-11 13:42:02.978576 pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/well.py
--rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 pydantic_ome_ngff-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1466 2023-02-14 18:55:46.264580 pydantic_ome_ngff-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1928 2023-07-18 15:15:47.646176 pydantic_ome_ngff-0.3.0/README.md
+-rw-r--r--   0        0        0     1008 2023-08-02 04:30:40.060360 pydantic_ome_ngff-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-03-22 18:16:41.323863 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/__init__.py
+-rw-r--r--   0        0        0      465 2023-08-02 04:30:09.334347 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/base.py
+-rw-r--r--   0        0        0      360 2023-03-08 00:10:20.528092 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/__init__.py
+-rw-r--r--   0        0        0      269 2023-08-02 04:30:09.335243 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/axes.py
+-rw-r--r--   0        0        0       20 2023-03-08 00:10:20.167824 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/base.py
+-rw-r--r--   0        0        0     1735 2023-08-02 04:30:09.335461 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/coordinateTransformations.py
+-rw-r--r--   0        0        0      505 2023-08-02 04:30:09.336062 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/imageLabel.py
+-rw-r--r--   0        0        0     8876 2023-08-02 04:30:09.336360 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/multiscales.py
+-rw-r--r--   0        0        0      476 2023-08-02 04:30:09.336573 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/plate.py
+-rw-r--r--   0        0        0      467 2023-08-02 04:30:09.336954 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/well.py
+-rw-r--r--   0        0        0        0 2023-03-22 18:28:17.442462 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/py.typed
+-rw-r--r--   0        0        0     1770 2023-08-02 04:30:09.337128 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/tree.py
+-rw-r--r--   0        0        0      441 2023-07-18 15:15:47.648220 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/utils.py
+-rw-r--r--   0        0        0      430 2023-03-08 00:10:20.188881 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/__init__.py
+-rw-r--r--   0        0        0     3797 2023-08-02 04:30:09.337390 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/axes.py
+-rw-r--r--   0        0        0       16 2023-03-08 00:10:20.185875 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/base.py
+-rw-r--r--   0        0        0     2361 2023-08-02 04:30:09.337850 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/coordinateTransformations.py
+-rw-r--r--   0        0        0     2207 2023-08-02 04:30:09.338008 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/imageLabel.py
+-rw-r--r--   0        0        0     8942 2023-08-02 04:30:09.338261 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/multiscales.py
+-rw-r--r--   0        0        0      980 2023-08-02 04:30:09.338403 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/plate.py
+-rw-r--r--   0        0        0      595 2023-08-02 04:30:09.338686 pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/well.py
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 pydantic_ome_ngff-0.3.0/PKG-INFO
```

### Comparing `pydantic_ome_ngff-0.2.3/LICENSE` & `pydantic_ome_ngff-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.3/README.md` & `pydantic_ome_ngff-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_ome_ngff-0.2.3/pyproject.toml` & `pydantic_ome_ngff-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-ome-ngff"
-version = "0.2.3"
+version = "0.3.0"
 description = "Pydantic models for the OME-NGFF"
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_ome_ngff", from="src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/coordinateTransformations.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/coordinateTransformations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+import textwrap
 from typing import Union
 import pydantic_ome_ngff.v04.coordinateTransformations as ctx
 
 
 class IdentityTransform(ctx.IdentityTransform):
     """
     An identity transform with no parameters.
@@ -27,28 +29,28 @@
     """
     A scale transform with a `scale` field that is a vector.
     See https://ngff.openmicroscopy.org/latest/#trafo-md
     """
 
 
 def get_transform_ndim(
-    transform: Union[VectorScaleTransform, VectorTranslationTransform]
+    transform: Union[VectorScaleTransform, VectorTranslationTransform],
 ) -> int:
     """
     Get the dimensionality of a vector transform (scale or translation).
     """
     if transform.type == "scale" and hasattr(transform, "scale"):
         return len(transform.scale)
     elif transform.type == "translation" and hasattr(transform, "translation"):
         return len(transform.translation)
     else:
-        raise ValueError(
-            f"""
-        Transform must be either VectorScaleTransform or VectorTranslationTransform.
-        Got {type(transform)} instead.
-        """
+        msg = (
+            f"Transform must be either VectorScaleTransform or "
+            f"VectorTranslationTransform. Got {type(transform)} instead."
         )
 
+        raise ValueError(textwrap.fill(msg))
+
 
 ScaleTransform = Union[VectorScaleTransform, PathTransform]
 TranslationTransform = Union[VectorTranslationTransform, PathTransform]
 CoordinateTransform = Union[ScaleTransform, TranslationTransform, IdentityTransform]
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/latest/multiscales.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/multiscales.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
 from collections import Counter
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+import textwrap
 import warnings
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
+
+from pydantic import BaseModel, conlist, root_validator, validator
 
-from pydantic import conlist, root_validator, validator, Field
-from pydantic_ome_ngff.base import StrictBase, StrictVersionedBase
-from pydantic_ome_ngff.latest.base import version
-from pydantic_ome_ngff.latest import coordinateTransformations as ctx
-from pydantic_ome_ngff.tree import Array, Attrs, Group
 from pydantic_ome_ngff.utils import duplicates
-from pydantic_ome_ngff.v04.axes import AxisType
-from pydantic_ome_ngff.latest.axes import Axis
+from pydantic_ome_ngff.base import VersionedBase
+from pydantic_ome_ngff.tree import Group, Attrs, Array
+from pydantic_ome_ngff.v04.base import version
+from pydantic_ome_ngff.v04.axes import Axis, AxisType
+import pydantic_ome_ngff.v04.coordinateTransformations as ctx
 
 
-class MultiscaleDataset(StrictBase):
+class MultiscaleDataset(BaseModel):
     path: str
     coordinateTransformations: conlist(
         Union[ctx.ScaleTransform, ctx.TranslationTransform], min_items=1, max_items=2
     )
 
     @validator("coordinateTransformations")
     def check_transforms_dimensionality(
@@ -27,48 +29,49 @@
     ) -> List[Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]]:
         ndims = []
         for tx in transforms:
             # this repeated conditional logic around transforms is so awful.
             if type(tx) in (ctx.VectorScaleTransform, ctx.VectorTranslationTransform):
                 ndims.append(ctx.get_transform_ndim(tx))
         if len(set(ndims)) > 1:
-            raise ValueError(
-                f"""
-            Elements of coordinateTransformations must have the same dimensionality. Got
-            elements with dimensionality = {ndims}.
-            """
+            msg = (
+                "Elements of coordinateTransformations must have the same "
+                f"dimensionality. Got elements with dimensionality = {ndims}."
             )
+            raise ValueError(textwrap.fill(msg))
         return transforms
 
     @validator("coordinateTransformations")
     def check_transforms_types(
-        cls, transforms: List[ctx.CoordinateTransform]
-    ) -> List[ctx.CoordinateTransform]:
+        cls,
+        transforms: List[
+            Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]
+        ],
+    ) -> List[Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]]:
         if (tform := transforms[0].type) != "scale":
-            raise ValueError(
-                f"""
-            The first element of coordinateTransformations must be a scale transform.
-            Got {tform} instead.
-            """
+            msg = (
+                "The first element of coordinateTransformations must be a scale "
+                f"transform. Got {tform} instead."
             )
+            raise ValueError(textwrap.fill(msg))
         if len(transforms) == 2:
             if (tform := transforms[1].type) != "translation":
-                raise ValueError(
-                    f"""
-                The second element of coordinateTransformations must be a translation 
-                transform. got {tform} instead.
-                """
+                msg = (
+                    "The second element of coordinateTransformations must be a "
+                    f"translation transform. Got {tform} instead."
                 )
+                raise ValueError(textwrap.fill(msg))
+
         return transforms
 
 
-class Multiscale(StrictVersionedBase):
+class Multiscale(VersionedBase):
     """
     Multiscale image metadata.
-    See https://ngff.openmicroscopy.org/latest/#multiscale-md
+    See https://ngff.openmicroscopy.org/0.4/#multiscale-md
     """
 
     # we need to put the version here as a private class attribute because the version
     # is not required by the spec...
     _version = version
     # SPEC: why is this optional? why is it untyped?
     version: Optional[Any] = version
@@ -79,89 +82,83 @@
     # SPEC: untyped!
     type: Optional[Any]
     # SPEC: should default to empty dict instead of None
     metadata: Optional[Dict[str, Any]] = None
     datasets: List[MultiscaleDataset]
     # SPEC: should not exist at top level and instead
     # live in dataset metadata or in .datasets
-    axes: List[Axis] = Field(..., min_items=2, max_items=5)
+    axes: conlist(Axis, min_items=2, max_items=5)
     # SPEC: should not live here, and if it is here,
     # it should default to an empty list instead of being nullable
     coordinateTransformations: Optional[
         List[Union[ctx.ScaleTransform, ctx.TranslationTransform]]
     ]
 
     @validator("name")
-    def check_name(cls, name: Optional[str]) -> Optional[str]:
+    def check_name(cls, name: str) -> str:
         if name is None:
-            warnings.warn(
-                f"""
-            The name field was set to None. Version {cls._version} of the OME-NGFF spec 
-            states that the `name` field of a Multiscales object should not be None.
-            """
+            msg = (
+                f"The name field was set to `None`. Version {cls._version} of the "
+                "OME-NGFF spec states that the `name` field of a Multiscales object "
+                "should not be None."
             )
+            warnings.warn(textwrap.fill(msg))
         return name
 
     @validator("axes")
     def check_axes(cls, axes: List[Axis]) -> List[Axis]:
         name_dupes = duplicates(a.name for a in axes)
         if len(name_dupes) > 0:
-            raise ValueError(
-                f"""
-                Axis names must be unique. Axis names {tuple(name_dupes.keys())} are 
-                repeated.
-                """
+            msg = (
+                f"Axis names must be unique. Axis names {tuple(name_dupes.keys())} "
+                "are repeated."
             )
-        axis_types = tuple(ax.type for ax in axes)
+            raise ValueError(textwrap.fill(msg))
+        axis_types = [ax.type for ax in axes]
         type_census = Counter(axis_types)
         num_spaces = type_census["space"]
         if num_spaces < 2 or num_spaces > 3:
-            raise ValueError(
-                f"""
-                Invalid number of space axes: {num_spaces}. Only 2 or 3 space axes 
-                are allowed.
-                """
+            msg = (
+                f"Invalid number of space axes: {num_spaces}. Only 2 or 3 space "
+                "axes are allowed."
             )
+            raise ValueError(textwrap.fill(msg))
 
         elif not all(a == "space" for a in axis_types[-num_spaces:]):
-            raise ValueError(
-                f"""
-                Space axes must come last. Got axes with order: {axis_types}
-                """
-            )
+            msg = f"Space axes must come last. Got axes with order: {axis_types}"
+            raise ValueError(textwrap.fill(msg))
 
         if (num_times := type_census["time"]) > 1:
-            raise ValueError(
-                f"""
-                Invalid number of time axes: {num_times}. Only 1 time axis is allowed.
-                """
+            msg = (
+                f"Invalid number of time axes: {num_times}. "
+                "Only 1 time axis is allowed."
             )
+            raise ValueError(textwrap.fill(msg))
 
         if (num_channels := type_census["channel"]) > 1:
-            raise ValueError(
-                f"""
-                Invalid number of channel axes: {num_channels}. Only 1 channel axis is 
-                allowed.
-                """
+            msg = (
+                f"Invalid number of channel axes: {num_channels}. "
+                "Only 1 channel axis is allowed."
             )
+            raise ValueError(textwrap.fill(msg))
 
         custom_axes = set(axis_types) - set(AxisType._member_names_)
         if len(custom_axes) > 1:
-            raise ValueError(
-                f"""Invalid number of custom axes: {custom_axes}. Only 1 custom axis is
-                allowed.
-                """
+            msg = (
+                f"Invalid number of custom axes: {custom_axes}. "
+                "Only 1 custom axis is allowed."
             )
+            raise ValueError(textwrap.fill(msg))
         return axes
 
 
 class MultiscaleAttrs(Attrs):
     """
     Attributes of a multiscale group.
-    See https://ngff.openmicroscopy.org/latest/#multiscale-md
+    See https://ngff.openmicroscopy.org/0.4/#multiscale-md
     """
 
     multiscales: List[Multiscale]
 
 
 class MultiscaleGroup(Group):
     attrs: MultiscaleAttrs
@@ -178,55 +175,53 @@
             else:
                 child_arrays.append(child)
         child_array_names = [a.name for a in child_arrays]
         multiscales: List[Multiscale] = values["attrs"].multiscales
         for multiscale in multiscales:
             for dataset in multiscale.datasets:
                 if (dpath := dataset.path) not in child_array_names:
-                    raise ValueError(
-                        f"""
-                    Dataset {dpath} was specified in multiscale metadata, but no 
-                    array with that name was found in the children of that group. All 
-                    arrays in multiscale metadata must be children of the group.
-                    """
+                    msg = (
+                        f"Dataset {dpath} was specified in multiscale metadata, "
+                        "but no array with that name was found in the children of "
+                        "that group. All arrays in multiscale metadata must be "
+                        "children of the group."
                     )
+                    raise ValueError(textwrap.fill(msg))
         return values
 
     @root_validator
     def check_array_ndim(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         array_children: Tuple[Array, ...] = tuple(
             filter(lambda v: hasattr(v, "shape"), values["children"])
         )
         multiscales: List[Multiscale] = values["attrs"].multiscales
 
-        ndims = [len(a.shape) for a in array_children]
+        ndims = tuple(len(a.shape) for a in array_children)
         if len(set(ndims)) > 1:
-            raise ValueError(
-                f"""
-            All arrays must have the same dimensionality. Got arrays with dimensionality
-            {ndims}. 
-            """
+            msg = (
+                "All arrays must have the same dimensionality. "
+                f"Got arrays with dimensionality {ndims}."
             )
+            raise ValueError(textwrap.fill(msg))
 
         # check that each transform has compatible rank
         for multiscale in multiscales:
-            tforms: List[ctx.CoordinateTransform] = []
+            tforms = []
             if multiscale.coordinateTransformations is not None:
                 tforms.extend(multiscale.coordinateTransformations)
             for dataset in multiscale.datasets:
                 tforms.extend(dataset.coordinateTransformations)
             for tform in tforms:
                 if hasattr(tform, "scale") or hasattr(tform, "translation"):
                     tform = cast(
                         Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform],
                         tform,
                     )
                     if (tform_dims := ctx.get_transform_ndim(tform)) not in set(ndims):
-                        raise ValueError(
-                            f"""
-                        Transform {tform} has dimensionality {tform_dims} which does not
-                        match the dimensionality of the arrays in this group ({ndims}). 
-                        Transform dimensionality must match array 
-                        dimensionality.
-                        """
+                        msg = (
+                            f"Transform {tform} has dimensionality {tform_dims} which "
+                            "does not match the dimensionality of the arrays in this "
+                            "group ({ndims}). Transform dimensionality must match "
+                            "array dimensionality."
                         )
+                        raise ValueError(textwrap.fill(msg))
         return values
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/tree.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from __future__ import annotations
 from typing import (
-    Union,
     Protocol,
     Tuple,
     Dict,
     Any,
     Iterable,
     Literal,
     List,
+    Union,
     runtime_checkable,
 )
+import textwrap
 from pydantic import BaseModel, Field
 from pydantic_ome_ngff.base import StrictBase
 
 NodeType = Literal["array", "group"]
 
 
 class Attrs(BaseModel):
@@ -29,15 +31,15 @@
     node_type: NodeType = Field("array", const=True)
     shape: Tuple[int, ...]
     dtype: str
 
 
 class Group(Node):
     node_type: NodeType = Field("group", const=True)
-    children: List[Union["Group", Array]]
+    children: List[Union[Group, Array]]
 
 
 class NodeLike(Protocol):
     basename: str
     attrs: Dict[str, Any]
 
 
@@ -45,15 +47,15 @@
 class ArrayLike(NodeLike, Protocol):
     shape: Tuple[int, ...]
     dtype: Any
 
 
 @runtime_checkable
 class GroupLike(NodeLike, Protocol):
-    def values(self) -> Iterable[Union["GroupLike", ArrayLike]]:
+    def values(self) -> Iterable[Union[GroupLike, ArrayLike]]:
         """
         Iterable of the children of this group
         """
         ...
 
 
 def build_tree(element: Union[GroupLike, ArrayLike]) -> Union[Group, Array]:
@@ -68,9 +70,10 @@
         result = Array(
             shape=element.shape, name=name, dtype=str(element.dtype), attrs=attrs
         )
     elif isinstance(element, GroupLike):
         children = list(map(build_tree, element.values()))
         result = Group(name=name, attrs=attrs, children=children)
     else:
-        raise ValueError(f"Object of type {type(element)} cannot be processed.")
+        msg = f"Object of type {type(element)} cannot be processed."
+        raise ValueError(textwrap.fill(msg))
     return result
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/axes.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/axes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
 from pydantic_ome_ngff.base import StrictVersionedBase
 from pydantic_ome_ngff.v04.base import version
 import warnings
 from enum import Enum
 from typing import Any, Dict, Optional
 from pydantic import validator
+import textwrap
 
 
 class AxisType(str, Enum):
     space = "space"
     time = "time"
     channel = "channel"
 
@@ -77,55 +79,45 @@
     # SPEC: this should almost certainly be a string, but the spec doesn't specify the type: https://github.com/ome/ngff/blob/ee4d5dab677636a28f1f65c248a751e279a0d1fe/0.4/index.bs#L243
     name: Any
     type: Optional[str]
     unit: Optional[str]
 
     @validator("unit")
     def check_unit(cls, unit: str, values: Dict[str, AxisType]) -> str:
-        type = values["type"]
-        if type == AxisType.space:
+        typ = values["type"]
+        if typ == AxisType.space:
             if unit not in SpaceUnit.__members__:
-                warnings.warn(
-                    f"""
-                Unit "{unit}" is not recognized as a standard unit for an axis with 
-                type "{type}".
-                """,
-                    UserWarning,
+                msg = (
+                    f'Unit "{unit}" is not recognized as a standard unit for an '
+                    f'axis with type "{typ}".'
                 )
-        elif type == AxisType.time:
+                warnings.warn(textwrap.fill(msg))
+
+        elif typ == AxisType.time:
             if unit not in TimeUnit.__members__:
-                warnings.warn(
-                    f"""
-                Unit "{unit}" is not recognized as a standard unit for an axis with 
-                type "{type}".
-                """,
-                    UserWarning,
+                msg = (
+                    f'Unit "{unit}" is not recognized as a standard unit for an '
+                    f'axis with type "{typ}".'
                 )
-        elif type == AxisType.channel:
+                warnings.warn(textwrap.fill(msg))
+        elif typ == AxisType.channel:
             pass
-        elif type is None:
-            warnings.warn(
-                f"""
-             Null axis type. Version {cls._version} of the OME-NGFF spec states that 
-             the "type" field of an axis should be set to a string.
-            """,
-                UserWarning,
+        elif typ is None:
+            msg = (
+                f"Null axis type. Version {cls._version} of the OME-NGFF spec "
+                "states that the `type` field of an axis should be a string."
             )
+            warnings.warn(textwrap.fill(msg))
         else:
-            warnings.warn(
-                f"""
-            Unknown axis type "{type}". Version {cls._version} of the OME-NGFF spec 
-            states that the "type" field of an axis should be one of 
-            {AxisType._member_names_}.
-            """,
-                UserWarning,
+            msg = (
+                f'Unknown axis type "{typ}". Version {cls._version} of the '
+                "OME-NGFF spec states that the `type` field of an axis should be "
+                f"one of {AxisType._member_names_}."
             )
-
+            warnings.warn(textwrap.fill(msg))
         if unit is None:
-            warnings.warn(
-                f"""
-            Null unit. Version {cls._version} of the OME-NGFF spec states
-            that the `unit` field of an axis should be set to a string.
-            """,
-                UserWarning,
+            msg = (
+                f"Null unit. Version {cls._version} of the OME-NGFF spec states "
+                "that the `unit` field of an axis should be a string."
             )
+            warnings.warn(textwrap.fill(msg))
         return unit
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/coordinateTransformations.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/coordinateTransformations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,73 @@
+from __future__ import annotations
+import textwrap
 from typing import List, Literal, Union
-from pydantic_ome_ngff.base import StrictBase
+from pydantic import BaseModel
 
 
-class IdentityTransform(StrictBase):
+class IdentityTransform(BaseModel):
     """
     An identity transform with no parameters.
     See https://ngff.openmicroscopy.org/0.4/#trafo-md
     """
 
     # SPEC why does this exist, as opposed to translation by 0 or scale by 1?
     type: str = "identity"
 
 
-class PathTransform(StrictBase):
+class PathTransform(BaseModel):
     """
     A coordinateTransform with a `path` field.
     See https://ngff.openmicroscopy.org/0.4/#trafo-md
     """
 
     # SPEC: the existence of this type is a massive sinkhole in the spec
     # translate and scale are both so simple that nobody should be using a path
     # argument to refer to some remote resource representing a translation
     # or a scale transform
     type: Union[Literal["scale"], Literal["translation"]]
     path: str
 
 
-class VectorTranslationTransform(StrictBase):
+class VectorTranslationTransform(BaseModel):
     """
     A translation transform with a `translate` field that is a vector.
     See https://ngff.openmicroscopy.org/0.4/#trafo-md
     """
 
     type: Literal["translation"] = "translation"
     translation: List[
         float
     ]  # SPEC: redundant field name -- we already know it's translation
 
 
-class VectorScaleTransform(StrictBase):
+class VectorScaleTransform(BaseModel):
     """
     A scale transform with a `scale` field that is a vector.
     See https://ngff.openmicroscopy.org/0.4/#trafo-md
     """
 
     type: Literal["scale"] = "scale"
     scale: List[float]  # SPEC: redundant field name -- we already know it's scale
 
 
 def get_transform_ndim(
-    transform: Union[VectorScaleTransform, VectorTranslationTransform]
+    transform: Union[VectorScaleTransform, VectorTranslationTransform],
 ) -> int:
     """
     Get the dimensionality of a vector transform (scale or translation).
     """
     if transform.type == "scale" and hasattr(transform, "scale"):
         return len(transform.scale)
     elif transform.type == "translation" and hasattr(transform, "translation"):
         return len(transform.translation)
     else:
-        raise ValueError(
-            f"""
-        Transform must be either VectorScaleTransform or VectorTranslationTransform.
-        Got {type(transform)} instead.
-        """
+        msg = (
+            f"Transform must be either VectorScaleTransform or "
+            f"VectorTranslationTransform. Got {type(transform)} instead."
         )
+        raise ValueError(textwrap.fill(msg))
 
 
 ScaleTransform = Union[VectorScaleTransform, PathTransform]
 TranslationTransform = Union[VectorTranslationTransform, PathTransform]
 CoordinateTransform = Union[ScaleTransform, TranslationTransform, IdentityTransform]
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/imageLabel.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/imageLabel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from __future__ import annotations
 import warnings
 from typing import List, Optional, Tuple
-
+import textwrap
 from pydantic import BaseModel, Field, validator
 from pydantic_ome_ngff.base import VersionedBase
 from pydantic_ome_ngff.utils import duplicates
-
 from pydantic_ome_ngff.v04.base import version
 
 
 class Color(BaseModel):
     label_value: int = Field(..., alias="label-value")
     rgba: Optional[Tuple[int, int, int, int]]
 
@@ -30,43 +30,40 @@
     # we need to put the version here as a private class attribute because the version
     # field is not required by the spec...
     _version = version
 
     # SPEC: version is either unset or a string?
     version: Optional[str] = version
     colors: Optional[List[Color]]
-    properties: Optional[Properties]
+    properties: Optional[List[Properties]]
     source: Optional[Source]
 
     @validator("version")
     def check_version(cls, ver: str) -> str:
         if ver is None:
-            warnings.warn(
-                f"""
+            msg = f"""
             The field "version" is "None". Version {cls._version} of
             the OME-NGFF spec states that "version" must either be unset or the string
             "{cls._version}"
             """
-            )
+            warnings.warn(textwrap.fill(msg))
         return ver
 
     @validator("colors")
     def check_colors(cls, colors: Optional[List[Color]]) -> Optional[List[Color]]:
         if colors is None:
-            warnings.warn(
-                f"""
+            msg = f"""
             The field "colors" is "None". Version {cls._version} of
-            the OME-NGFF spec states that "colors" should be a list of label 
+            the OME-NGFF spec states that "colors" should be a list of label
             descriptors.
             """
-            )
+            warnings.warn(textwrap.fill(msg))
         else:
             dupes = duplicates(x.label_value for x in colors)
             if len(dupes) > 1:
-                raise ValueError(
-                    f"""
+                msg = f"""
                     Duplicated label-value: {tuple(dupes.keys())}.
                     label-values must be unique across elements of `colors`
                     """
-                )
+                raise ValueError(textwrap.fill(msg))
 
         return colors
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/multiscales.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/latest/multiscales.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
 from collections import Counter
+import textwrap
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 import warnings
-from typing import Any, Dict, List, Optional, Union, Tuple, cast
-
-from pydantic import Field, conlist, root_validator, validator
 
+from pydantic import BaseModel, conlist, root_validator, validator
+from pydantic_ome_ngff.base import VersionedBase
+from pydantic_ome_ngff.latest.base import version
+from pydantic_ome_ngff.latest import coordinateTransformations as ctx
+from pydantic_ome_ngff.tree import Array, Attrs, Group
 from pydantic_ome_ngff.utils import duplicates
-from pydantic_ome_ngff.base import StrictBase, StrictVersionedBase
-from pydantic_ome_ngff.tree import Group, Attrs, Array
-from pydantic_ome_ngff.v04.base import version
-from pydantic_ome_ngff.v04.axes import Axis, AxisType
-import pydantic_ome_ngff.v04.coordinateTransformations as ctx
+from pydantic_ome_ngff.v04.axes import AxisType
+from pydantic_ome_ngff.latest.axes import Axis
 
 
-class MultiscaleDataset(StrictBase):
+class MultiscaleDataset(BaseModel):
     path: str
     coordinateTransformations: conlist(
         Union[ctx.ScaleTransform, ctx.TranslationTransform], min_items=1, max_items=2
     )
 
     @validator("coordinateTransformations")
     def check_transforms_dimensionality(
@@ -27,144 +29,132 @@
     ) -> List[Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]]:
         ndims = []
         for tx in transforms:
             # this repeated conditional logic around transforms is so awful.
             if type(tx) in (ctx.VectorScaleTransform, ctx.VectorTranslationTransform):
                 ndims.append(ctx.get_transform_ndim(tx))
         if len(set(ndims)) > 1:
-            raise ValueError(
-                f"""
-            Elements of coordinateTransformations must have the same dimensionality. Got
-            elements with dimensionality = {ndims}.
-            """
+            msg = (
+                "Elements of coordinateTransformations must have the same "
+                f"dimensionality. Got elements with dimensionality = {ndims}."
             )
+            raise ValueError(textwrap.fill(msg))
         return transforms
 
     @validator("coordinateTransformations")
     def check_transforms_types(
-        cls,
-        transforms: List[
-            Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]
-        ],
-    ) -> List[Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform]]:
+        cls, transforms: List[ctx.CoordinateTransform]
+    ) -> List[ctx.CoordinateTransform]:
         if (tform := transforms[0].type) != "scale":
-            raise ValueError(
-                f"""
-            The first element of coordinateTransformations must be a scale transform.
-            Got {tform} instead.
-            """
+            msg = (
+                "The first element of coordinateTransformations must be a scale "
+                f"transform. Got {tform} instead."
             )
+            raise ValueError(textwrap.fill(msg))
         if len(transforms) == 2:
             if (tform := transforms[1].type) != "translation":
-                raise ValueError(
-                    f"""
-                The second element of coordinateTransformations must be a translation 
-                transform. got {tform} instead.
-                """
+                msg = (
+                    "The second element of coordinateTransformations must be a "
+                    f"translation transform. Got {tform} instead."
                 )
+                raise ValueError(textwrap.fill(msg))
         return transforms
 
 
-class Multiscale(StrictVersionedBase):
+class Multiscale(VersionedBase):
     """
     Multiscale image metadata.
-    See https://ngff.openmicroscopy.org/0.4/#multiscale-md
+    See https://ngff.openmicroscopy.org/latest/#multiscale-md
     """
 
     # we need to put the version here as a private class attribute because the version
     # is not required by the spec...
     _version = version
-    # SPEC: why is this optional? why is it untyped?
-    version: Optional[Any] = version
+
+    version: str = version
     # SPEC: why is this nullable instead of reserving the empty string
     # SPEC: untyped!
     name: Optional[Any]
     # SPEC: not clear what this field is for, given the existence of .metadata
     # SPEC: untyped!
     type: Optional[Any]
     # SPEC: should default to empty dict instead of None
     metadata: Optional[Dict[str, Any]] = None
     datasets: List[MultiscaleDataset]
     # SPEC: should not exist at top level and instead
     # live in dataset metadata or in .datasets
-    axes: List[Axis] = Field(..., min_items=2, max_items=5)
+    axes: conlist(Axis, min_items=2, max_items=5)
     # SPEC: should not live here, and if it is here,
     # it should default to an empty list instead of being nullable
     coordinateTransformations: Optional[
         List[Union[ctx.ScaleTransform, ctx.TranslationTransform]]
     ]
 
     @validator("name")
-    def check_name(cls, name: str) -> str:
+    def check_name(cls, name: Optional[str]) -> Optional[str]:
         if name is None:
-            warnings.warn(
-                f"""
-            The name field was set to None. Version {cls._version} of the OME-NGFF spec 
-            states that the `name` field of a Multiscales object should not be None.
-            """
+            msg = (
+                f"The name field was set to `None`. Version {cls._version} of the "
+                "OME-NGFF spec states that the `name` field of a Multiscales object "
+                "should not be None."
             )
+            warnings.warn(textwrap.fill(msg))
         return name
 
     @validator("axes")
     def check_axes(cls, axes: List[Axis]) -> List[Axis]:
         name_dupes = duplicates(a.name for a in axes)
         if len(name_dupes) > 0:
-            raise ValueError(
-                f"""
-                Axis names must be unique. Axis names {tuple(name_dupes.keys())} are 
-                repeated.
-                """
+            msg = (
+                f"Axis names must be unique. Axis names {tuple(name_dupes.keys())} "
+                "are repeated."
             )
-        axis_types = [ax.type for ax in axes]
+            raise ValueError(textwrap.fill(msg))
+        axis_types = tuple(ax.type for ax in axes)
         type_census = Counter(axis_types)
         num_spaces = type_census["space"]
         if num_spaces < 2 or num_spaces > 3:
-            raise ValueError(
-                f"""
-                Invalid number of space axes: {num_spaces}. Only 2 or 3 space axes 
-                are allowed.
-                """
+            msg = (
+                f"Invalid number of space axes: {num_spaces}. Only 2 or 3 space "
+                "axes are allowed."
             )
+            raise ValueError(textwrap.fill(msg))
 
         elif not all(a == "space" for a in axis_types[-num_spaces:]):
-            raise ValueError(
-                f"""
-                Space axes must come last. Got axes with order: {axis_types}
-                """
-            )
+            msg = f"Space axes must come last. Got axes with order: {axis_types}"
+            raise ValueError(textwrap.fill(msg))
 
         if (num_times := type_census["time"]) > 1:
-            raise ValueError(
-                f"""
-                Invalid number of time axes: {num_times}. Only 1 time axis is allowed.
-                """
+            msg = (
+                f"Invalid number of time axes: {num_times}. "
+                "Only 1 time axis is allowed."
             )
+            raise ValueError(textwrap.fill(msg))
 
         if (num_channels := type_census["channel"]) > 1:
-            raise ValueError(
-                f"""
-                Invalid number of channel axes: {num_channels}. Only 1 channel axis is 
-                allowed.
-                """
+            msg = (
+                f"Invalid number of channel axes: {num_channels}. "
+                "Only 1 channel axis is allowed."
             )
+            raise ValueError(textwrap.fill(msg))
 
         custom_axes = set(axis_types) - set(AxisType._member_names_)
         if len(custom_axes) > 1:
-            raise ValueError(
-                f"""Invalid number of custom axes: {custom_axes}. Only 1 custom axis is
-                allowed.
-                """
+            msg = (
+                f"Invalid number of custom axes: {custom_axes}. "
+                "Only 1 custom axis is allowed."
             )
+            raise ValueError(textwrap.fill(msg))
         return axes
 
 
 class MultiscaleAttrs(Attrs):
     """
     Attributes of a multiscale group.
-    See https://ngff.openmicroscopy.org/0.4/#multiscale-md
+    See https://ngff.openmicroscopy.org/latest/#multiscale-md
     """
 
     multiscales: List[Multiscale]
 
 
 class MultiscaleGroup(Group):
     attrs: MultiscaleAttrs
@@ -181,56 +171,53 @@
             else:
                 child_arrays.append(child)
         child_array_names = [a.name for a in child_arrays]
         multiscales: List[Multiscale] = values["attrs"].multiscales
         for multiscale in multiscales:
             for dataset in multiscale.datasets:
                 if (dpath := dataset.path) not in child_array_names:
-                    raise ValueError(
-                        f"""
-                    Dataset {dpath} was specified in multiscale metadata, but no 
-                    array with that name was found in the children of that group. All 
-                    arrays in multiscale metadata must be children of the group.
-                    """
+                    msg = (
+                        f"Dataset {dpath} was specified in multiscale metadata, "
+                        "but no array with that name was found in the children of "
+                        "that group. All arrays in multiscale metadata must be "
+                        "children of the group."
                     )
+                    raise ValueError(textwrap.fill(msg))
         return values
 
     @root_validator
     def check_array_ndim(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         array_children: Tuple[Array, ...] = tuple(
             filter(lambda v: hasattr(v, "shape"), values["children"])
         )
         multiscales: List[Multiscale] = values["attrs"].multiscales
 
-        ndims = tuple(len(a.shape) for a in array_children)
+        ndims = [len(a.shape) for a in array_children]
         if len(set(ndims)) > 1:
-            raise ValueError(
-                f"""
-            All arrays must have the same dimensionality. Got arrays with dimensionality
-            {ndims}. 
-            """
+            msg = (
+                "All arrays must have the same dimensionality. "
+                f"Got arrays with dimensionality {ndims}."
             )
+            raise ValueError(textwrap.fill(msg))
 
         # check that each transform has compatible rank
         for multiscale in multiscales:
-            tforms = []
+            tforms: List[ctx.CoordinateTransform] = []
             if multiscale.coordinateTransformations is not None:
                 tforms.extend(multiscale.coordinateTransformations)
             for dataset in multiscale.datasets:
                 tforms.extend(dataset.coordinateTransformations)
             for tform in tforms:
-
                 if hasattr(tform, "scale") or hasattr(tform, "translation"):
                     tform = cast(
                         Union[ctx.VectorScaleTransform, ctx.VectorTranslationTransform],
                         tform,
                     )
                     if (tform_dims := ctx.get_transform_ndim(tform)) not in set(ndims):
-                        raise ValueError(
-                            f"""
-                        Transform {tform} has dimensionality {tform_dims} which does not
-                        match the dimensionality of the arrays in this group ({ndims}). 
-                        Transform dimensionality must match array 
-                        dimensionality.
-                        """
+                        msg = (
+                            f"Transform {tform} has dimensionality {tform_dims} which "
+                            "does not match the dimensionality of the arrays in this "
+                            "group ({ndims}). Transform dimensionality must match "
+                            "array dimensionality."
                         )
+                        raise ValueError(textwrap.fill(msg))
         return values
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/plate.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/plate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+from __future__ import annotations
 from typing import List, Optional
 
-from pydantic import BaseModel, PositiveInt
+from pydantic import BaseModel, PositiveInt, NonNegativeInt
 from pydantic_ome_ngff.base import VersionedBase
 
 from pydantic_ome_ngff.v04.base import version
 
 
 class Acquisition(BaseModel):
-    id: PositiveInt
+    id: NonNegativeInt
     name: Optional[str]
     maximumfieldcount: PositiveInt
 
 
 class Entry(BaseModel):
     name: str
 
 
 class Well(BaseModel):
     # must be {rowName}/{columnName}
     path: str
-    rowIndex: PositiveInt
-    columnIndex: PositiveInt
+    rowIndex: NonNegativeInt
+    columnIndex: NonNegativeInt
 
 
 class Plate(VersionedBase):
     """
     Plate metadata
     see https://ngff.openmicroscopy.org/0.4/#plate-md
     """
```

### Comparing `pydantic_ome_ngff-0.2.3/src/pydantic_ome_ngff/v04/well.py` & `pydantic_ome_ngff-0.3.0/src/pydantic_ome_ngff/v04/well.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import List, Optional
 
 from pydantic import BaseModel
 from pydantic_ome_ngff.base import VersionedBase
 
 from pydantic_ome_ngff.v04.base import version
```

### Comparing `pydantic_ome_ngff-0.2.3/PKG-INFO` & `pydantic_ome_ngff-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-ome-ngff
-Version: 0.2.3
+Version: 0.3.0
 Summary: Pydantic models for the OME-NGFF
 License: MIT
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

