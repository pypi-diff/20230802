# Comparing `tmp/xarray_ome_ngff-1.2.0.tar.gz` & `tmp/xarray_ome_ngff-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_ome_ngff-1.2.0.tar", max compression
+gzip compressed data, was "xarray_ome_ngff-1.2.1.tar", max compression
```

## Comparing `xarray_ome_ngff-1.2.0.tar` & `xarray_ome_ngff-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1511 2023-02-15 20:59:22.209367 xarray_ome_ngff-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     4282 2023-02-15 21:39:36.100583 xarray_ome_ngff-1.2.0/README.md
--rw-r--r--   0        0        0      546 2023-03-10 21:39:08.377766 xarray_ome_ngff-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      141 2023-03-10 21:37:50.404713 xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/__init__.py
--rw-r--r--   0        0        0      189 2023-03-10 21:37:50.406081 xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/core.py
--rw-r--r--   0        0        0        0 2023-03-10 21:37:50.406126 xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/latest/__init__.py
--rw-r--r--   0        0        0    10849 2023-03-10 21:37:50.406742 xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/latest/multiscales.py
--rw-r--r--   0        0        0     1427 2023-03-10 21:38:01.666642 xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/registry.py
--rw-r--r--   0        0        0        0 2023-03-10 21:37:50.406964 xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/v04/__init__.py
--rw-r--r--   0        0        0    10840 2023-03-10 21:37:50.407165 xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/v04/multiscales.py
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 xarray_ome_ngff-1.2.0/setup.py
--rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 xarray_ome_ngff-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1511 2023-02-15 20:59:22.209367 xarray_ome_ngff-1.2.1/LICENSE.md
+-rw-r--r--   0        0        0     4282 2023-02-15 21:39:36.100583 xarray_ome_ngff-1.2.1/README.md
+-rw-r--r--   0        0        0      564 2023-08-02 14:40:17.426579 xarray_ome_ngff-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-03-23 18:12:34.307869 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/__init__.py
+-rw-r--r--   0        0        0      189 2023-03-10 21:37:50.406081 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/core.py
+-rw-r--r--   0        0        0        0 2023-03-10 21:37:50.406126 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/latest/__init__.py
+-rw-r--r--   0        0        0    10928 2023-08-02 14:23:01.853008 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/latest/multiscales.py
+-rw-r--r--   0        0        0        0 2023-03-22 18:23:46.045591 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/py.typed
+-rw-r--r--   0        0        0     1427 2023-03-22 18:46:56.675792 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/registry.py
+-rw-r--r--   0        0        0        0 2023-03-10 21:37:50.406964 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/v04/__init__.py
+-rw-r--r--   0        0        0    10924 2023-08-02 14:23:01.853882 xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/v04/multiscales.py
+-rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 xarray_ome_ngff-1.2.1/PKG-INFO
```

### Comparing `xarray_ome_ngff-1.2.0/LICENSE.md` & `xarray_ome_ngff-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xarray_ome_ngff-1.2.0/README.md` & `xarray_ome_ngff-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/latest/multiscales.py` & `xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/latest/multiscales.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     arrays: Sequence[DataArray],
     array_paths: Optional[List[str]] = None,
     name: Optional[str] = None,
     type: Optional[str] = None,
     metadata: Optional[Dict[str, Any]] = None,
     normalize_units: bool = True,
     infer_axis_type: bool = True,
-):
+) -> Multiscale:
     """
     Create Multiscale metadata from a collection of xarray.DataArrays
 
     Parameters
     ----------
 
     arrays: sequence of DataArray
@@ -59,36 +59,34 @@
     -------
 
     An instance of Multiscale metadata.
 
     """
     for arr in arrays:
         if not isinstance(arr, DataArray):
-            raise ValueError(
-                f"""
-                This function requires a list of xarray.DataArrays. Got an element with 
-                type = '{builtins.type(arr)}' instead.
-                """
+            msg = (
+                "This function requires a list of xarray.DataArrays. Got an element "
+                f"with type = '{builtins.type(arr)}' instead."
             )
+            raise ValueError(msg)
     # sort arrays by decreasing shape
-    ranks = [a.ndim for a in arrays]
-    if len(set(ranks)) > 1:
-        raise ValueError(
-            f"""
-        All arrays must have the same number of dimensions. Found arrays with different 
-        numbers of dimensions: {set(ranks)}.
-        """
+    ndims = [a.ndim for a in arrays]
+    if len(set(ndims)) > 1:
+        msg = (
+            "All arrays must have the same number of dimensions. Found arrays with "
+            f"different numbers of dimensions: {set(ndims)}."
         )
+        raise ValueError(msg)
     arrays_sorted = tuple(reversed(sorted(arrays, key=lambda arr: np.prod(arr.shape))))
     base_transforms = [
         VectorScaleTransform(
             scale=[
                 1,
             ]
-            * ranks[0]
+            * ndims[0]
         )
     ]
     axes, transforms = tuple(
         zip(
             *(
                 coords_to_transforms(
                     tuple(array.coords.values()),
@@ -100,17 +98,15 @@
         )
     )
     if array_paths is None:
         paths = [d.name for d in arrays_sorted]
     else:
         assert len(array_paths) == len(
             arrays
-        ), f"""
-        Length of array_paths {len(array_paths)} doesn't match {len(arrays)}
-        """
+        ), f"Length of array_paths {len(array_paths)} doesn't match {len(arrays)}"
         paths = array_paths
 
     datasets = list(
         MultiscaleDataset(path=p, coordinateTransformations=t)
         for p, t in zip(paths, transforms)
     )
     return Multiscale(
@@ -160,72 +156,69 @@
     """
 
     translate = []
     scale = []
     axes = []
     for coord in coords:
         if ndim := len(coord.dims) != 1:
-            raise ValueError(
-                f"""
-            Each coordinate must have one and only one dimension.
-            Got a coordinate with {ndim}.
-                             """
+            msg = (
+                "Each coordinate must have one and only one dimension. "
+                f"Got a coordinate with {ndim}."
             )
+            raise ValueError(msg)
         dim = coord.dims[0]
         translate.append(float(coord[0]))
         # impossible to infer a scale coordinate from a coordinate with 1 sample
         if len(coord) > 1:
             scale.append(abs(float(coord[1]) - float(coord[0])))
         else:
             scale.append(1)
         unit = coord.attrs.get("unit", None)
         units = coord.attrs.get("units", None)
         if unit is None and units is not None:
-            warnings.warn(
-                f"""
-            The key 'unit' was unset, but 'units' was found in array attrs, with a value
-            of '{units}'. The 'unit' property of the corresponding axis will be set to
-            '{units}', but this behavior may change in the future.
-            """
+            msg = (
+                "The key 'unit' was unset, but 'units' was found in array attrs, "
+                f"with a value of \"{units}\". The 'unit' property of the "
+                f'corresponding axis will be set to "{units}", but this behavior '
+                "may change in the future."
             )
+            warnings.warn(msg)
             unit = units
         elif units is not None:
-            warnings.warn(
-                f"""
-            Both 'unit' and 'units' were found in array attrs, with values '{unit}' and 
-            '{units}', respectively. The value associated with 'unit' ({unit}) will be
-            used in the axis metadata.
-            """
+            msg = (
+                'Both "unit" and "units" were found in array attrs, with values '
+                f'"{unit}" and "{units}", respectively. The value associated '
+                f'with "unit" ({unit}) will be used in the axis metadata.'
             )
+            warnings.warn(msg)
         if normalize_units and unit is not None:
             unit = ureg.get_name(unit, case_sensitive=True)
         if (type := coord.attrs.get("type", None)) is None and infer_axis_type:
             unit_dimensionality = ureg.get_dimensionality(unit)
             if len(unit_dimensionality) > 1:
+                msg = (
+                    f'Failed to infer the type of axis with unit = "{unit}"',
+                    f'because it appears that unit "{unit}" is a compound unit, '
+                    'which cannot be mapped to a single axis type. "type" will be '
+                    'set to "None" for this axis.',
+                )
                 warnings.warn(
-                    """
-                Failed to infer the type of axis with unit = "{unit}", because it 
-                appears that unit "{unit}" is a compound unit, which cannot be mapped
-                to a single axis type. "type" will be set to None for this axis.
-                """,
                     RuntimeWarning,
                 )
             if "[length]" in unit_dimensionality:
                 type = "space"
             elif "[time]" in unit_dimensionality:
                 type = "time"
             else:
-                warnings.warn(
-                    """
-                Failed to infer the type of axis with unit = "{unit}", because it could 
-                not be mapped to either a time or space dimension. "type" will be set to
-                None for this axis.
-                """,
-                    RuntimeWarning,
+                msg = (
+                    f'Failed to infer the type of axis with unit = "{unit}", '
+                    "because it could not be mapped to either a time or space "
+                    'dimension. "type" will be set to None for this axis.'
                 )
+                warnings.warn(msg, RuntimeWarning)
                 type = None
 
         axes.append(
             Axis(
                 name=dim,
                 unit=unit,
                 type=type,
@@ -244,62 +237,60 @@
 ) -> List[DataArray]:
     """
     Given an output shape, convert a sequence of Axis objects and a corresponding
     sequence of coordinateTransform objects into xarray-compatible coordinates.
     """
 
     if len(axes) != len(shape):
-        raise ValueError(
-            f"""Length of axes must match length of shape. 
-            Got {len(axes)} axes but shape has {len(shape)} elements"""
+        msg = (
+            "Length of axes must match length of shape. "
+            f"Got {len(axes)} axes but shape has {len(shape)} elements"
         )
+        raise ValueError(msg)
 
     result = []
 
     for idx, axis in enumerate(axes):
         base_coord = np.arange(shape[idx], dtype="float")
         name = axis.name
         unit = axis.unit
         # apply transforms in order
         for tx in transforms:
             if type(getattr(tx, "path", None)) == str:
-                raise ValueError(
-                    f"""
-                    Problematic transform: {tx}. 
-                    This library does not handle transforms with paths.
-                    """
+                msg = (
+                    f"Problematic transform: {tx}. This library cannot handle "
+                    "transforms with paths. Resolve this path to a literal scale or "
+                    "translation"
                 )
+                raise ValueError(msg)
 
             if tx.type == "translation":
                 if len(tx.translation) != len(axes):
-                    raise ValueError(
-                        f"""
-                    Translation parameter has length {len(tx.translation)}. This does 
-                    not match the number of axes {len(axes)}.
-                    """
+                    msg = (
+                        f"Translation parameter has length {len(tx.translation)}. "
+                        f"This does not match the number of axes {len(axes)}."
                     )
+                    raise ValueError(msg)
                 base_coord += tx.translation[idx]
             elif tx.type == "scale":
                 if len(tx.scale) != len(axes):
-                    raise ValueError(
-                        f"""
-                    Scale parameter has length {len(tx.scale)}. This does not match the 
-                    number of axes {len(axes)}.
-                    """
+                    msg = (
+                        f"Scale parameter has length {len(tx.scale)}. "
+                        f"This does not match the number of axes {len(axes)}."
                     )
+                    raise ValueError(msg)
                 base_coord *= tx.scale[idx]
             elif tx.type == "identity":
                 pass
             else:
-                raise ValueError(
-                    f"""
-                    Transform type {tx.type} not recognized. Must be one of scale, 
-                    translate, or identity
-                    """
+                msg = (
+                    f"Transform type {tx.type} not recognized. Must be one of scale, "
+                    "translation, or identity"
                 )
+                raise ValueError(msg)
 
         result.append(
             DataArray(
                 base_coord,
                 attrs={"unit": unit},
                 dims=(name,),
             )
```

### Comparing `xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/registry.py` & `xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from typing import NamedTuple, Callable, Any
 from xarray_ome_ngff.core import ngff_versions
 
 
-class Metadataadapters(NamedTuple):
+class MetadataAdapters(NamedTuple):
     ngff_version: str
     multiscale_metadata: Callable[[Any], Any]
     transforms_to_coords: Callable[[Any], Any]
     coords_to_transforms: Callable[[Any], Any]
 
 
 def get_adapters(version: str):
     if version == "0.4":
         from xarray_ome_ngff.v04.multiscales import (
             multiscale_metadata,
             transforms_to_coords,
             coords_to_transforms,
         )
 
-        return Metadataadapters(
+        return MetadataAdapters(
             ngff_version="0.4",
             multiscale_metadata=multiscale_metadata,
             transforms_to_coords=transforms_to_coords,
             coords_to_transforms=coords_to_transforms,
         )
 
     elif version == "0.5-dev" or version == "latest":
         from xarray_ome_ngff.latest.multiscales import (
             multiscale_metadata,
             transforms_to_coords,
             coords_to_transforms,
         )
 
-        return Metadataadapters(
+        return MetadataAdapters(
             ngff_version="0.5-dev",
             multiscale_metadata=multiscale_metadata,
             transforms_to_coords=transforms_to_coords,
             coords_to_transforms=coords_to_transforms,
         )
 
     else:
```

### Comparing `xarray_ome_ngff-1.2.0/src/xarray_ome_ngff/v04/multiscales.py` & `xarray_ome_ngff-1.2.1/src/xarray_ome_ngff/v04/multiscales.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     arrays: Sequence[DataArray],
     array_paths: Optional[List[str]] = None,
     name: Optional[str] = None,
     type: Optional[str] = None,
     metadata: Optional[Dict[str, Any]] = None,
     normalize_units: bool = True,
     infer_axis_type: bool = True,
-):
+) -> Multiscale:
     """
     Create Multiscale metadata from a collection of xarray.DataArrays
 
     Parameters
     ----------
 
     arrays: sequence of DataArray
@@ -59,36 +59,34 @@
     -------
 
     An instance of Multiscale metadata.
 
     """
     for arr in arrays:
         if not isinstance(arr, DataArray):
-            raise ValueError(
-                f"""
-                This function requires a list of xarray.DataArrays. Got an element with 
-                type = '{builtins.type(arr)}' instead.
-                """
+            msg = (
+                "This function requires a list of xarray.DataArrays. Got an element "
+                f"with type = '{builtins.type(arr)}' instead."
             )
+            raise ValueError(msg)
     # sort arrays by decreasing shape
-    ranks = [a.ndim for a in arrays]
-    if len(set(ranks)) > 1:
-        raise ValueError(
-            f"""
-        All arrays must have the same number of dimensions. Found arrays with different 
-        numbers of dimensions: {set(ranks)}.
-        """
+    ndims = [a.ndim for a in arrays]
+    if len(set(ndims)) > 1:
+        msg = (
+            "All arrays must have the same number of dimensions. Found arrays with "
+            f"different numbers of dimensions: {set(ndims)}."
         )
+        raise ValueError(msg)
     arrays_sorted = tuple(reversed(sorted(arrays, key=lambda arr: np.prod(arr.shape))))
     base_transforms = [
         VectorScaleTransform(
             scale=[
                 1,
             ]
-            * ranks[0]
+            * ndims[0]
         )
     ]
     axes, transforms = tuple(
         zip(
             *(
                 coords_to_transforms(
                     tuple(array.coords.values()),
@@ -96,21 +94,19 @@
                     infer_axis_type=infer_axis_type,
                 )
                 for array in arrays_sorted
             )
         )
     )
     if array_paths is None:
-        paths = [d.name for d in arrays_sorted]
+        paths = [str(d.name) for d in arrays_sorted]
     else:
         assert len(array_paths) == len(
             arrays
-        ), f"""
-        Length of array_paths {len(array_paths)} doesn't match {len(arrays)}
-        """
+        ), f"Length of array_paths {len(array_paths)} doesn't match {len(arrays)}"
         paths = array_paths
 
     datasets = list(
         MultiscaleDataset(path=p, coordinateTransformations=t)
         for p, t in zip(paths, transforms)
     )
     return Multiscale(
@@ -160,72 +156,69 @@
     """
 
     translate = []
     scale = []
     axes = []
     for coord in coords:
         if ndim := len(coord.dims) != 1:
-            raise ValueError(
-                f"""
-            Each coordinate must have one and only one dimension.
-            Got a coordinate with {ndim}.
-                             """
+            msg = (
+                "Each coordinate must have one and only one dimension. "
+                f"Got a coordinate with {ndim}."
             )
+            raise ValueError(msg)
         dim = coord.dims[0]
         translate.append(float(coord[0]))
         # impossible to infer a scale coordinate from a coordinate with 1 sample
         if len(coord) > 1:
             scale.append(abs(float(coord[1]) - float(coord[0])))
         else:
             scale.append(1)
         unit = coord.attrs.get("unit", None)
         units = coord.attrs.get("units", None)
         if unit is None and units is not None:
-            warnings.warn(
-                f"""
-            The key 'unit' was unset, but 'units' was found in array attrs, with a value
-            of '{units}'. The 'unit' property of the corresponding axis will be set to
-            '{units}', but this behavior may change in the future.
-            """
+            msg = (
+                "The key 'unit' was unset, but 'units' was found in array attrs, "
+                f"with a value of \"{units}\". The 'unit' property of the "
+                f'corresponding axis will be set to "{units}", but this behavior '
+                "may change in the future."
             )
+            warnings.warn(msg)
             unit = units
         elif units is not None:
-            warnings.warn(
-                f"""
-            Both 'unit' and 'units' were found in array attrs, with values '{unit}' and 
-            '{units}', respectively. The value associated with 'unit' ({unit}) will be
-            used in the axis metadata.
-            """
+            msg = (
+                'Both "unit" and "units" were found in array attrs, with values '
+                f'"{unit}" and "{units}", respectively. The value associated '
+                f'with "unit" ({unit}) will be used in the axis metadata.'
             )
+            warnings.warn(msg)
         if normalize_units and unit is not None:
             unit = ureg.get_name(unit, case_sensitive=True)
         if (type := coord.attrs.get("type", None)) is None and infer_axis_type:
             unit_dimensionality = ureg.get_dimensionality(unit)
             if len(unit_dimensionality) > 1:
+                msg = (
+                    f'Failed to infer the type of axis with unit = "{unit}"',
+                    f'because it appears that unit "{unit}" is a compound unit, '
+                    'which cannot be mapped to a single axis type. "type" will be '
+                    'set to "None" for this axis.',
+                )
                 warnings.warn(
-                    """
-                Failed to infer the type of axis with unit = "{unit}", because it 
-                appears that unit "{unit}" is a compound unit, which cannot be mapped
-                to a single axis type. "type" will be set to None for this axis.
-                """,
                     RuntimeWarning,
                 )
             if "[length]" in unit_dimensionality:
                 type = "space"
             elif "[time]" in unit_dimensionality:
                 type = "time"
             else:
-                warnings.warn(
-                    """
-                Failed to infer the type of axis with unit = "{unit}", because it could 
-                not be mapped to either a time or space dimension. "type" will be set to
-                None for this axis.
-                """,
-                    RuntimeWarning,
+                msg = (
+                    f'Failed to infer the type of axis with unit = "{unit}", '
+                    "because it could not be mapped to either a time or space "
+                    'dimension. "type" will be set to None for this axis.'
                 )
+                warnings.warn(msg, RuntimeWarning)
                 type = None
 
         axes.append(
             Axis(
                 name=dim,
                 unit=unit,
                 type=type,
@@ -244,62 +237,60 @@
 ) -> List[DataArray]:
     """
     Given an output shape, convert a sequence of Axis objects and a corresponding
     sequence of coordinateTransform objects into xarray-compatible coordinates.
     """
 
     if len(axes) != len(shape):
-        raise ValueError(
-            f"""Length of axes must match length of shape. 
-            Got {len(axes)} axes but shape has {len(shape)} elements"""
+        msg = (
+            "Length of axes must match length of shape. "
+            f"Got {len(axes)} axes but shape has {len(shape)} elements"
         )
+        raise ValueError(msg)
 
     result = []
 
     for idx, axis in enumerate(axes):
         base_coord = np.arange(shape[idx], dtype="float")
         name = axis.name
         unit = axis.unit
         # apply transforms in order
         for tx in transforms:
             if type(getattr(tx, "path", None)) == str:
-                raise ValueError(
-                    f"""
-                    Problematic transform: {tx}. 
-                    This library does not handle transforms with paths.
-                    """
+                msg = (
+                    f"Problematic transform: {tx}. This library cannot handle "
+                    "transforms with paths. Resolve this path to a literal scale or "
+                    "translation"
                 )
+                raise ValueError(msg)
 
             if tx.type == "translation":
                 if len(tx.translation) != len(axes):
-                    raise ValueError(
-                        f"""
-                    Translation parameter has length {len(tx.translation)}. This does 
-                    not match the number of axes {len(axes)}.
-                    """
+                    msg = (
+                        f"Translation parameter has length {len(tx.translation)}. "
+                        f"This does not match the number of axes {len(axes)}."
                     )
+                    raise ValueError(msg)
                 base_coord += tx.translation[idx]
             elif tx.type == "scale":
                 if len(tx.scale) != len(axes):
-                    raise ValueError(
-                        f"""
-                    Scale parameter has length {len(tx.scale)}. This does not match the 
-                    number of axes {len(axes)}.
-                    """
+                    msg = (
+                        f"Scale parameter has length {len(tx.scale)}. "
+                        f"This does not match the number of axes {len(axes)}."
                     )
+                    raise ValueError(msg)
                 base_coord *= tx.scale[idx]
             elif tx.type == "identity":
                 pass
             else:
-                raise ValueError(
-                    f"""
-                    Transform type {tx.type} not recognized. Must be one of scale, 
-                    translate, or identity
-                    """
+                msg = (
+                    f"Transform type {tx.type} not recognized. Must be one of scale, "
+                    "translation, or identity"
                 )
+                raise ValueError(msg)
 
         result.append(
             DataArray(
                 base_coord,
                 attrs={"unit": unit},
                 dims=(name,),
             )
```

### Comparing `xarray_ome_ngff-1.2.0/setup.py` & `xarray_ome_ngff-1.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,154 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-package_dir = \
-{'': 'src'}
-
-packages = \
-['xarray_ome_ngff', 'xarray_ome_ngff.latest', 'xarray_ome_ngff.v04']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pint>=0.20.1,<0.21.0',
- 'pydantic-ome-ngff>=0.2.0,<0.3.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'xarray>=2023.2.0,<2024.0.0']
-
-setup_kwargs = {
-    'name': 'xarray-ome-ngff',
-    'version': '1.2.0',
-    'description': 'xarray and ome-ngff',
-    'long_description': '# xarray-ome-ngff\nIntegration between xarray and the ome-ngff data model.\n\nAt present (February, 2023) this is a partial implementation of the [OME-NGFF spec](https://ngff.openmicroscopy.org/latest/#implementations). Specifcally, *only* the [`multiscales`](https://ngff.openmicroscopy.org/latest/#multiscale-md) and specs required by `multiscales` are implemented. Complete support for the spec would be welcome.\n\n## How it works\nThis library depends on [`pydantic-ome-ngff`](https://github.com/JaneliaSciComp/pydantic-ome-ngff) which implements OME-NGFF metadata as [pydantic](https://docs.pydantic.dev/) models. \n[`Axes`](https://ngff.openmicroscopy.org/latest/#axes-md) metadata is inferred from a DataArray by iterating over the dimensions of the array and checking for `units` and `type` properties in the attributes of the `coords` assigned to each dimension. Dimensions without coordinates will raise an exception. Scale and translation `CoordinateTransforms` are inferred by inspecting the values of the coordinates for each dimension. Be advised that no attempt is made to verify that arrays are sampled on a regular grid.\n\n## Usage\n\nGenerate `multiscales` metadata from a multiscale collection of DataArrays.\n\n```python\nfrom xarray import DataArray\nimport numpy as np\nfrom xarray_ome_ngff import create_multiscale_metadata\nimport json\ncoords = {\'z\' : DataArray(np.arange(100), attrs={\'units\': \'nm\', \'type\': \'space\'}, dims=(\'z\',)),\n         \'y\' : DataArray(np.arange(300) * 2.2, attrs={\'units\': \'nm\', \'type\': \'space\'}, dims=(\'y\')),\n         \'x\' : DataArray((np.arange(300) * .5) + 1, attrs={\'units\': \'nm\', \'type\': \'space\'}, dims=(\'x\',))}\n\ns0 = DataArray(data=0, coords=coords, dims=(\'z\',\'y\',\'x\'), name=\'s0\')\ns1 = s0.coarsen({dim: 2 for dim in s0.dims}).mean()\ns1.name = \'s1\'\n# create a small multiscale pyramid\nmultiscale = [s0, s1]\nmetadata = create_multiscale_metadata(name=\'test\', type=\'yes\', arrays=multiscale)\nprint(metadata.json(indent=2))\n```\n```json\n{\n  "version": "0.5-dev",\n  "name": "test",\n  "type": "yes",\n  "metadata": null,\n  "datasets": [\n    {\n      "path": "s0",\n      "coordinateTransformations": [\n        {\n          "type": "scale",\n          "scale": [\n            1.0,\n            2.2,\n            0.5\n          ]\n        },\n        {\n          "type": "translation",\n          "translation": [\n            0.0,\n            0.0,\n            1.0\n          ]\n        }\n      ]\n    },\n    {\n      "path": "s1",\n      "coordinateTransformations": [\n        {\n          "type": "scale",\n          "scale": [\n            2.0,\n            4.4,\n            1.0\n          ]\n        },\n        {\n          "type": "translation",\n          "translation": [\n            0.5,\n            1.1,\n            1.25\n          ]\n        }\n      ]\n    }\n  ],\n  "axes": [\n    {\n      "name": "z",\n      "type": "space",\n      "units": null\n    },\n    {\n      "name": "y",\n      "type": "space",\n      "units": null\n    },\n    {\n      "name": "x",\n      "type": "space",\n      "units": null\n    }\n  ],\n  "coordinateTransformations": [\n    {\n      "type": "scale",\n      "scale": [\n        1.0,\n        1.0,\n        1.0\n      ]\n    }\n  ]\n}\n```\n\nIt is not possible to create a DataArray from OME-NGFF metadata, but together the OME-NGFF [`Axes`](https://ngff.openmicroscopy.org/latest/#axes-md) and [`CoordinateTransformations`](https://ngff.openmicroscopy.org/latest/#trafo-md) metadata are sufficient to create _coordinates_ for a DataArray, provided you know the shape of the data. The function `create_coords` performs this operation:\n\n```python\nfrom xarray_ome_ngff import create_coords\nfrom pydantic_ome_ngff.v05.coordinateTransformations import VectorScaleTransform, VectorTranslationTransform\nfrom pydantic_ome_ngff.v05.axes import Axis\n\n\nshape = (3, 3)\naxes = [Axis(name=\'a\', units="meter", type="space"), Axis(name=\'b\', units="meter", type="space")]\n\ntransforms = [VectorScaleTransform(scale=[1, .5]), VectorTranslationTransform(translation=[1, 2])]\n\ncoords = create_coords(axes, transforms, shape)\nprint(coords)\n\'\'\'\n{\'a\': <xarray.DataArray (a: 3)>\narray([1., 2., 3.])\nDimensions without coordinates: a\nAttributes:\n    units:    meter, \'b\': <xarray.DataArray (b: 3)>\narray([2. , 2.5, 3. ])\nDimensions without coordinates: b\nAttributes:\n    units:    meter}\n\'\'\'\n```',
-    'author': 'Davis Vann Bennett',
-    'author_email': 'davis.v.bennett@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+Metadata-Version: 2.1
+Name: xarray-ome-ngff
+Version: 1.2.1
+Summary: xarray and ome-ngff
+Author: Davis Vann Bennett
+Author-email: davis.v.bennett@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pint (>=0.20.1,<0.21.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic-ome-ngff (>=0.3.0,<0.4.0)
+Requires-Dist: xarray (>=2023.2.0,<2024.0.0)
+Description-Content-Type: text/markdown
+
+# xarray-ome-ngff
+Integration between xarray and the ome-ngff data model.
+
+At present (February, 2023) this is a partial implementation of the [OME-NGFF spec](https://ngff.openmicroscopy.org/latest/#implementations). Specifcally, *only* the [`multiscales`](https://ngff.openmicroscopy.org/latest/#multiscale-md) and specs required by `multiscales` are implemented. Complete support for the spec would be welcome.
+
+## How it works
+This library depends on [`pydantic-ome-ngff`](https://github.com/JaneliaSciComp/pydantic-ome-ngff) which implements OME-NGFF metadata as [pydantic](https://docs.pydantic.dev/) models. 
+[`Axes`](https://ngff.openmicroscopy.org/latest/#axes-md) metadata is inferred from a DataArray by iterating over the dimensions of the array and checking for `units` and `type` properties in the attributes of the `coords` assigned to each dimension. Dimensions without coordinates will raise an exception. Scale and translation `CoordinateTransforms` are inferred by inspecting the values of the coordinates for each dimension. Be advised that no attempt is made to verify that arrays are sampled on a regular grid.
+
+## Usage
+
+Generate `multiscales` metadata from a multiscale collection of DataArrays.
+
+```python
+from xarray import DataArray
+import numpy as np
+from xarray_ome_ngff import create_multiscale_metadata
+import json
+coords = {'z' : DataArray(np.arange(100), attrs={'units': 'nm', 'type': 'space'}, dims=('z',)),
+         'y' : DataArray(np.arange(300) * 2.2, attrs={'units': 'nm', 'type': 'space'}, dims=('y')),
+         'x' : DataArray((np.arange(300) * .5) + 1, attrs={'units': 'nm', 'type': 'space'}, dims=('x',))}
+
+s0 = DataArray(data=0, coords=coords, dims=('z','y','x'), name='s0')
+s1 = s0.coarsen({dim: 2 for dim in s0.dims}).mean()
+s1.name = 's1'
+# create a small multiscale pyramid
+multiscale = [s0, s1]
+metadata = create_multiscale_metadata(name='test', type='yes', arrays=multiscale)
+print(metadata.json(indent=2))
+```
+```json
+{
+  "version": "0.5-dev",
+  "name": "test",
+  "type": "yes",
+  "metadata": null,
+  "datasets": [
+    {
+      "path": "s0",
+      "coordinateTransformations": [
+        {
+          "type": "scale",
+          "scale": [
+            1.0,
+            2.2,
+            0.5
+          ]
+        },
+        {
+          "type": "translation",
+          "translation": [
+            0.0,
+            0.0,
+            1.0
+          ]
+        }
+      ]
+    },
+    {
+      "path": "s1",
+      "coordinateTransformations": [
+        {
+          "type": "scale",
+          "scale": [
+            2.0,
+            4.4,
+            1.0
+          ]
+        },
+        {
+          "type": "translation",
+          "translation": [
+            0.5,
+            1.1,
+            1.25
+          ]
+        }
+      ]
+    }
+  ],
+  "axes": [
+    {
+      "name": "z",
+      "type": "space",
+      "units": null
+    },
+    {
+      "name": "y",
+      "type": "space",
+      "units": null
+    },
+    {
+      "name": "x",
+      "type": "space",
+      "units": null
+    }
+  ],
+  "coordinateTransformations": [
+    {
+      "type": "scale",
+      "scale": [
+        1.0,
+        1.0,
+        1.0
+      ]
+    }
+  ]
 }
+```
 
+It is not possible to create a DataArray from OME-NGFF metadata, but together the OME-NGFF [`Axes`](https://ngff.openmicroscopy.org/latest/#axes-md) and [`CoordinateTransformations`](https://ngff.openmicroscopy.org/latest/#trafo-md) metadata are sufficient to create _coordinates_ for a DataArray, provided you know the shape of the data. The function `create_coords` performs this operation:
 
-setup(**setup_kwargs)
+```python
+from xarray_ome_ngff import create_coords
+from pydantic_ome_ngff.v05.coordinateTransformations import VectorScaleTransform, VectorTranslationTransform
+from pydantic_ome_ngff.v05.axes import Axis
+
+
+shape = (3, 3)
+axes = [Axis(name='a', units="meter", type="space"), Axis(name='b', units="meter", type="space")]
+
+transforms = [VectorScaleTransform(scale=[1, .5]), VectorTranslationTransform(translation=[1, 2])]
+
+coords = create_coords(axes, transforms, shape)
+print(coords)
+'''
+{'a': <xarray.DataArray (a: 3)>
+array([1., 2., 3.])
+Dimensions without coordinates: a
+Attributes:
+    units:    meter, 'b': <xarray.DataArray (b: 3)>
+array([2. , 2.5, 3. ])
+Dimensions without coordinates: b
+Attributes:
+    units:    meter}
+'''
+```
```

