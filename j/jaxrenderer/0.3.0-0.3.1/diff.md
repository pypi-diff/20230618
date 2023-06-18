# Comparing `tmp/jaxrenderer-0.3.0.tar.gz` & `tmp/jaxrenderer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.3.0.tar", max compression
+gzip compressed data, was "jaxrenderer-0.3.1.tar", max compression
```

## Comparing `jaxrenderer-0.3.0.tar` & `jaxrenderer-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    11367 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/LICENSE
--rw-r--r--   0        0        0     2312 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/README.md
--rw-r--r--   0        0        0     5935 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/changelog.md
--rw-r--r--   0        0        0     1559 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5637 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/README.md
--rw-r--r--   0        0        0      539 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/__init__.py
--rw-r--r--   0        0        0      741 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/_meta_utils.py
--rw-r--r--   0        0        0    34989 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/geometry.py
--rw-r--r--   0        0        0    17431 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/model.py
--rw-r--r--   0        0        0    17457 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/pipeline.py
--rw-r--r--   0        0        0    14617 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/renderer.py
--rw-r--r--   0        0        0     9130 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/scene.py
--rw-r--r--   0        0        0    14563 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/README.md
--rw-r--r--   0        0        0     1373 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3413 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     5009 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5284 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9820 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     8035 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9759 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4517 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/types.py
--rw-r--r--   0        0        0     3284 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/value_checker.py
--rw-r--r--   0        0        0     3719 1970-01-01 00:00:00.000000 jaxrenderer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2312 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/README.md
+-rw-r--r--   0        0        0     6059 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/changelog.md
+-rw-r--r--   0        0        0     1683 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5637 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/README.md
+-rw-r--r--   0        0        0      539 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/__init__.py
+-rw-r--r--   0        0        0     1342 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/_backport.py
+-rw-r--r--   0        0        0      764 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/_meta_utils.py
+-rw-r--r--   0        0        0    35017 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/geometry.py
+-rw-r--r--   0        0        0    17560 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/model.py
+-rw-r--r--   0        0        0    17577 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/pipeline.py
+-rw-r--r--   0        0        0    14697 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/renderer.py
+-rw-r--r--   0        0        0     9561 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/scene.py
+-rw-r--r--   0        0        0    14672 2023-06-18 16:00:17.093956 jaxrenderer-0.3.1/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1453 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3493 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     5089 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5364 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9900 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     8115 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9839 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4517 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3588 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/types.py
+-rw-r--r--   0        0        0     3364 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-06-18 16:00:17.097956 jaxrenderer-0.3.1/renderer/value_checker.py
+-rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 jaxrenderer-0.3.1/PKG-INFO
```

### Comparing `jaxrenderer-0.3.0/LICENSE` & `jaxrenderer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/README.md` & `jaxrenderer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/changelog.md` & `jaxrenderer-0.3.1/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,7 +53,12 @@
 ## 0.3.0
 
 1. Fix `gl_FrontFacing` computation in pipeline so it is consistent to comment: `True` if not backfacing (i.e. frontfacing & side facing).
 2. Add an extra stage `Shader.primitive_chooser` to choose which primitive to be rendered for each fragment. The default implementation is provided, which assumes that the depth is just the interpolated `z` value in the eye space. It just picks the values of the single primitive that is closest to the camera and is not discarded in the previous pipeline.
 3. Expose `loop_unroll` static option to allow unrolling several operations (row rendering) within a single iteration of the outmost loop (iterating along first axis of the canvas). This may be useful in some cases for performance improvement, but careful benchmarking is needed to determine the optimal value. The default value is `1` (no unrolling) as it is the most general case in larger canvases (benchmarked on `960x540` using [GPU T4 in Colab](https://colab.research.google.com/drive/1xhkYNz5WjvUCjQWpp72CLf9SIy3i5PnN)).
 4. Bump the minimum Python version to Python 3.10
 5. Lower the minimum jax & jaxlib version to 0.3.25.
+
+## 0.3.1
+
+1. Lower minimum Python version to 3.8
+2. Introducing `type_extensions` package and improved typing annotations.
```

### Comparing `jaxrenderer-0.3.0/pyproject.toml` & `jaxrenderer-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.3.0"
+version = "0.3.1"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
@@ -28,20 +28,24 @@
     "README.md",
     "changelog.md",
     "pyproject.toml",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 jax = ">=0.3.25,<5.0.0"
 numpy = "^1.22.0"
 jaxlib = {version = ">=0.3.25,<5.0.0", source = "jax"}
-jaxtyping = "^0.2.19"
+jaxtyping = [
+    {version = ">=0.2.13,<0.2.20", python = ">=3.8,<3.9"},
+    {version = "^0.2.19", python = "^3.9"}
+]
 importlib-metadata = "^6.6.0"
+typing_extensions = "^4.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.6.2"
 pillow = "^9.4.0"
 importlib-resources = "^5.12.0"
```

### Comparing `jaxrenderer-0.3.0/renderer/README.md` & `jaxrenderer-0.3.1/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/renderer/__init__.py` & `jaxrenderer-0.3.1/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/renderer/_meta_utils.py` & `jaxrenderer-0.3.1/renderer/_meta_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import functools
 import inspect
-from typing import Callable, ParamSpec, TypeVar
+from typing import Callable, TypeVar
 
 import jax
 
+from ._backport import ParamSpec
+
 ArgT = ParamSpec("ArgT")
 RetT = TypeVar("RetT")
 
 
 def add_tracing_name(func: Callable[ArgT, RetT]) -> Callable[ArgT, RetT]:
     """Add tracing name to function."""
```

### Comparing `jaxrenderer-0.3.0/renderer/geometry.py` & `jaxrenderer-0.3.1/renderer/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 import enum
 from functools import partial
-from typing import Any, NamedTuple, Optional, Union
+from typing import NamedTuple, Optional, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Float, Integer, Num, jaxtyped
 
 from ._meta_utils import add_tracing_name
-from .types import Triangle2Df, Vec2f, Vec3f, Vec4f
+from .types import JaxFloating, Triangle2Df, Vec2f, Vec3f, Vec4f
 
 # Transform matrix that takes a batch of homogeneous 3D vertices and transform
 # them into 2D cartesian vertices in screen space + Z value (making it 3D)
 #
 # The result of x-y values in screen space may be float, and thus further
 # conversion to integers are needed.
 World2Screen = Float[Array, "4 4"]
@@ -593,18 +595,18 @@
         return view_matrix_inv
 
     @staticmethod
     @jaxtyped
     @partial(jax.jit, inline=True)
     @add_tracing_name
     def perspective_projection_matrix(
-        fovy: jnp.floating[Any],
-        aspect: jnp.floating[Any],
-        z_near: jnp.floating[Any],
-        z_far: jnp.floating[Any],
+        fovy: JaxFloating,
+        aspect: JaxFloating,
+        z_near: JaxFloating,
+        z_far: JaxFloating,
     ) -> Projection:
         """Create a projection matrix to map the model in the camera frame (eye
             coordinates) onto the viewing volume (clip coordinates), using
             perspective transformation. This follows the implementation in
             OpenGL (gluPerspective)
 
         Parameters:
@@ -668,20 +670,20 @@
         return inv
 
     @staticmethod
     @jaxtyped
     @partial(jax.jit, inline=True)
     @add_tracing_name
     def orthographic_projection_matrix(
-        left: jnp.floating[Any],
-        right: jnp.floating[Any],
-        bottom: jnp.floating[Any],
-        top: jnp.floating[Any],
-        z_near: jnp.floating[Any],
-        z_far: jnp.floating[Any],
+        left: JaxFloating,
+        right: JaxFloating,
+        bottom: JaxFloating,
+        top: JaxFloating,
+        z_near: JaxFloating,
+        z_far: JaxFloating,
     ) -> Projection:
         """Create a projection matrix to map the model in the camera frame (eye
             coordinates) onto the viewing volume (clip coordinates), using
             orthographic transformation. This follows the implementation in
             OpenGL (glOrtho).
 
         Parameters:
```

### Comparing `jaxrenderer-0.3.0/renderer/model.py` & `jaxrenderer-0.3.1/renderer/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
-from typing import NamedTuple, Optional, Sequence, Union
+from typing import Optional
 
 import jax
 import jax.experimental.checkify as checkify
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
 from jaxtyping import (Array, Bool, Float, Integer, Num, PyTree, Shaped,
                        jaxtyped)
 
+from ._backport import NamedTuple, Sequence, Tuple, TypeAlias
 from ._meta_utils import add_tracing_name
 from .geometry import Camera, transform_matrix_from_rotation
 from .types import (FALSE_ARRAY, FaceIndices, Normals, SpecularMap, Texture,
                     UVCoordinates, Vec3f, Vec4f, Vertices)
 from .value_checker import index_in_bound
 
-ModelMatrix = Float[Array, "4 4"]
+ModelMatrix: TypeAlias = Float[Array, "4 4"]
 
 
 class Model(NamedTuple):
     """Model with vertices specification and attached maps.
 
     NormalMap is not included for now as it is not used in the reference
     implementation
@@ -123,22 +126,22 @@
             index_in_bound(self.faces_uv, self.uvs.shape[0]),
             f"faces_uv out of bound, expected [0, {self.uvs.shape[0]}),"
             " got {max_idx}.",
             max_idx=self.faces_uv.max(),
         )
 
 
-VertT = Num[Array, "_dim ..."]
-VertsT = Union[list[VertT], tuple[VertT, ...]]
-FaceIndicesT = Num[Array, "_faces 3"]
-FaceIndicessT = Union[list[FaceIndicesT], tuple[FaceIndicesT, ...]]
-
-MapT = Num[Array, "_width _height ..."]
-MapsT = Union[list[MapT], tuple[MapT, ...]]
-Shape2DT = tuple[Integer[Array, ""], Integer[Array, ""]]
+VertT: TypeAlias = Num[Array, "_dim ..."]
+VertsT: TypeAlias = Sequence[VertT]
+FaceIndicesT: TypeAlias = Num[Array, "_faces 3"]
+FaceIndicessT: TypeAlias = Sequence[FaceIndicesT]
+
+MapT: TypeAlias = Num[Array, "_width _height ..."]
+MapsT: TypeAlias = Sequence[MapT]
+Shape2DT: TypeAlias = Tuple[Integer[Array, ""], Integer[Array, ""]]
 """Shape of first two components of a map, i.e., (width, height)."""
 
 
 class MergedModel(NamedTuple):
     """Merged model with vertices, normals, uv coordinates, and faces."""
     verts: Vertices
     norms: Normals
```

### Comparing `jaxrenderer-0.3.0/renderer/pipeline.py` & `jaxrenderer-0.3.1/renderer/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import Any, NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax import lax
 from jax.tree_util import tree_map
 from jaxtyping import Array, Bool, Float, Integer, Num, jaxtyped
 
+from ._backport import Tuple, TypeAlias
 from ._meta_utils import add_tracing_name
 from .geometry import Camera, Interpolation, Viewport, interpolate
 from .shader import (ID, MixedExtraT, MixerOutput, PerFragment, PerVertex,
                      Shader, ShaderExtraInputT, VaryingT)
 from .types import (FALSE_ARRAY, Buffers, CanvasMask, FaceIndices, Triangle,
                     Vec2f, Vec2i, Vec3f, Vec4f, ZBuffer)
 
@@ -108,15 +111,15 @@
     @jaxtyped
     @partial(jax.jit, inline=True)
     @add_tracing_name
     def _per_pixel(coord: Vec2i) -> tuple[MixerOutput, MixedExtraT]:
 
         assert isinstance(coord, Vec2i), f"expected Vec2i, got {coord}"
 
-        ReturnT = tuple[  #
+        ReturnT = Tuple[  #
             Float[Array, "kept_primitives 4"],  #
             Bool[Array, "kept_primitives"],  #
             Float[Array, "kept_primitives 2"],  #
             Bool[Array, "kept_primitives"],  #
             VaryingT,  #
             Float[Array, "kept_primitives 3"],  #
             Float[Array, "kept_primitives 3"],  #
```

### Comparing `jaxrenderer-0.3.0/renderer/renderer.py` & `jaxrenderer-0.3.1/renderer/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple, Optional, Sequence, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
```

### Comparing `jaxrenderer-0.3.0/renderer/scene.py` & `jaxrenderer-0.3.1/renderer/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from typing import NamedTuple, NewType, Optional, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
 
+from ._backport import replace_dict
 from .model import Model, ModelObject
 from .shapes.capsule import UpAxis, create_capsule
 from .shapes.cube import create_cube
 from .types import SpecularMap, Texture, Vec3f, Vec4f
 
 GUID = NewType("GUID", int)
 
@@ -176,14 +179,27 @@
         _object = self.objects[object_id]
         objects = {k: v for k, v in self.objects.items() if k != object_id}
         del _object
 
         return self._replace(objects=objects)
 
     @jaxtyped
+    def _replace_obj(self, object_id: GUID, new_obj: ModelObject) -> "Scene":
+        """Replace an object in the scene.
+
+        Parameters:
+          - object_id: the unique identifier of the object to replace.
+          - new_obj: the new object.
+        """
+        return self._replace(objects=replace_dict(
+            self.objects,
+            {object_id: new_obj},
+        ))
+
+    @jaxtyped
     def set_object_position(
         self,
         object_id: GUID,
         position: Union[Vec3f, tuple[float, float, float]],
     ) -> "Scene":
         """Set the position of an object in the scene.
 
@@ -192,15 +208,15 @@
           - position: the new position of the object.
         """
         position = jnp.asarray(position, dtype=float)
         assert isinstance(position, Vec3f), f"{position}"
 
         new_obj = self.objects[object_id].replace_with_position(position)
 
-        return self._replace(objects=self.objects | {object_id: new_obj})
+        return self._replace_obj(object_id, new_obj)
 
     @jaxtyped
     def set_object_orientation(
         self,
         object_id: GUID,
         orientation: Optional[Union[Vec4f, tuple[float, float, float,
                                                  float]]] = None,
@@ -222,15 +238,15 @@
             rotation_matrix = jnp.asarray(rotation_matrix)
 
         new_obj = self.objects[object_id].replace_with_orientation(
             orientation=orientation,
             rotation_matrix=rotation_matrix,
         )
 
-        return self._replace(objects=self.objects | {object_id: new_obj})
+        return self._replace_obj(object_id, new_obj)
 
     @jaxtyped
     def set_object_local_scaling(
         self,
         object_id: GUID,
         local_scaling: Union[Vec3f, tuple[float, float, float]],
     ) -> "Scene":
@@ -241,15 +257,15 @@
           - local_scaling: the new local scaling of the object.
         """
         scaling = jnp.asarray(local_scaling, dtype=float)
         assert isinstance(scaling, Vec3f), f"{scaling}"
 
         new_obj = self.objects[object_id].replace_with_local_scaling(scaling)
 
-        return self._replace(objects=self.objects | {object_id: new_obj})
+        return self._replace_obj(object_id, new_obj)
 
     @jaxtyped
     def set_object_double_sided(
         self,
         object_id: GUID,
         double_sided: Union[bool, Bool[Array, ""]],
     ) -> "Scene":
@@ -258,8 +274,8 @@
         Parameters:
           - object_id: the unique identifier of the object.
           - double_sided: whether the object is double-sided.
         """
         new_obj = self.objects[object_id].replace_with_double_sided(
             jnp.asarray(double_sided))
 
-        return self._replace(objects=self.objects | {object_id: new_obj})
+        return self._replace_obj(object_id, new_obj)
```

### Comparing `jaxrenderer-0.3.0/renderer/shader.py` & `jaxrenderer-0.3.1/renderer/shader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from abc import ABC, abstractmethod
 from functools import partial
 from typing import Generic, NamedTuple, TypeVar
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import Partial, tree_map
 from jaxtyping import Array, Bool, Float, Integer, PyTree, Shaped, jaxtyped
 
+from ._backport import Tuple
 from ._meta_utils import add_tracing_name
 from .geometry import Camera, Interpolation, interpolate
 from .types import FALSE_ARRAY, INF_ARRAY, TRUE_ARRAY, Vec2f, Vec3f, Vec4f
 
 jax.config.update('jax_array', True)
 
 ID = Integer[Array, ""]
@@ -44,21 +47,21 @@
     # not discard
     keeps: Bool[Array, ""] = TRUE_ARRAY
     use_default_depth: Bool[Array, ""] = FALSE_ARRAY
 
 
 VaryingT = TypeVar(
     "VaryingT",
-    bound=tuple[Shaped[Array, "..."], ...],
+    bound=Tuple[Shaped[Array, "..."], ...],
 )
 """The user-defined input and second (extra) output of fragment shader."""
 
 MixedExtraT = TypeVar(
     "MixedExtraT",
-    bound=tuple[Shaped[Array, "..."], ...],
+    bound=Tuple[Shaped[Array, "..."], ...],
 )
 """The user-defined second (extra) output of mix shader."""
 
 
 class MixerOutput(NamedTuple):
     """Built-in output from `Shader.mix`.
```

### Comparing `jaxrenderer-0.3.0/renderer/shaders/README.md` & `jaxrenderer-0.3.1/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/renderer/shaders/depth.py` & `jaxrenderer-0.3.1/renderer/shaders/depth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple
 
 import jax
 from jaxtyping import Array, Float, jaxtyped
 
 from .._meta_utils import add_tracing_name
```

### Comparing `jaxrenderer-0.3.0/renderer/shaders/gouraud.py` & `jaxrenderer-0.3.1/renderer/shaders/gouraud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
```

### Comparing `jaxrenderer-0.3.0/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.3.1/renderer/shaders/gouraud_texture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
```

### Comparing `jaxrenderer-0.3.0/renderer/shaders/phong.py` & `jaxrenderer-0.3.1/renderer/shaders/phong.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
```

### Comparing `jaxrenderer-0.3.0/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.3.1/renderer/shaders/phong_darboux.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import Partial
```

### Comparing `jaxrenderer-0.3.0/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.3.1/renderer/shaders/phong_reflection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, Integer, jaxtyped
```

### Comparing `jaxrenderer-0.3.0/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.3.1/renderer/shaders/phong_reflection_shadow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, Integer, jaxtyped
```

### Comparing `jaxrenderer-0.3.0/renderer/shadow.py` & `jaxrenderer-0.3.1/renderer/shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/renderer/shapes/capsule.py` & `jaxrenderer-0.3.1/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/renderer/shapes/cube.py` & `jaxrenderer-0.3.1/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/renderer/types.py` & `jaxrenderer-0.3.1/renderer/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-from typing import Any, NamedTuple, Union
+from typing import Generic, TypeVar, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, Integer, Shaped, jaxtyped
+from jaxtyping import Array, Bool, Float, Integer, jaxtyped
+
+from ._backport import JaxFloating, JaxInteger, NamedTuple, TypeAlias
 
 jax.config.update('jax_array', True)
 
 TRUE_ARRAY: Bool[Array, ""] = lax.full((), True, dtype=jnp.bool_)
 FALSE_ARRAY: Bool[Array, ""] = lax.full((), False, dtype=jnp.bool_)
 INF_ARRAY: Float[Array, ""] = lax.full((), jnp.inf)
 
-Index = Integer[Array, ""]
+Index: TypeAlias = Integer[Array, ""]
 
-CanvasMask = Bool[Array, "#width #height"]
-BatchCanvasMask = Bool[Array, "#batch #width #height"]
-Canvas = Float[Array, "width height channel"]
-ZBuffer = Float[Array, "width height"]
-Colour = Float[Array, "channel"]
-# triangle thus 3 "colour"s
-TriangleColours = Float[Array, "3 channel"]
-Vec2i = Integer[Array, "2"]
-Vec3i = Integer[Array, "3"]
-Vec2f = Float[Array, "2"]
-Vec3f = Float[Array, "3"]
+CanvasMask: TypeAlias = Bool[Array, "#width #height"]
+BatchCanvasMask: TypeAlias = Bool[Array, "#batch #width #height"]
+Canvas: TypeAlias = Float[Array, "width height channel"]
+ZBuffer: TypeAlias = Float[Array, "width height"]
+Colour: TypeAlias = Float[Array, "channel"]
+
+Vec2i: TypeAlias = Integer[Array, "2"]
+Vec3i: TypeAlias = Integer[Array, "3"]
+Vec2f: TypeAlias = Float[Array, "2"]
+Vec3f: TypeAlias = Float[Array, "3"]
 # usually used only for 3D homogeneous coordinates
-Vec4f = Float[Array, "4"]
+Vec4f: TypeAlias = Float[Array, "4"]
 # 3 vertices, with each vertex defined in Vec2i in screen(canvas) space
-Triangle2D = Integer[Array, "3 2"]
+Triangle2D: TypeAlias = Integer[Array, "3 2"]
 # 3 vertices, with each vertex defined in Vec2f
-Triangle2Df = Float[Array, "3 2"]
+Triangle2Df: TypeAlias = Float[Array, "3 2"]
 # 3 vertices, each vertex defined in Vec2i in 3d (world/model) space + Float z
-Triangle = Float[Array, "3 4"]
+Triangle: TypeAlias = Float[Array, "3 4"]
 # Barycentric coordinates has 3 components
-TriangleBarycentric = Float[Array, "3 3"]
+TriangleBarycentric: TypeAlias = Float[Array, "3 3"]
 
 # each face has 3 vertices
-FaceIndices = Integer[Array, "faces 3"]
+FaceIndices: TypeAlias = Integer[Array, "faces 3"]
 # each vertex is defined by 3 float numbers, x-y-z
-Vertices = Float[Array, "vertices 3"]
-Normals = Float[Array, "normals 3"]
-UVCoordinates = Float[Array, "uv_counts 2"]
-Texture = Float[Array, "textureWidth textureHeight channel"]
-SpecularMap = Float[Array, "textureWidth textureHeight"]
-NormalMap = Float[Array, "textureWidth textureHeight 3"]
+Vertices: TypeAlias = Float[Array, "vertices 3"]
+Normals: TypeAlias = Float[Array, "normals 3"]
+UVCoordinates: TypeAlias = Float[Array, "uv_counts 2"]
+Texture: TypeAlias = Float[Array, "textureWidth textureHeight channel"]
+SpecularMap: TypeAlias = Float[Array, "textureWidth textureHeight"]
+NormalMap: TypeAlias = Float[Array, "textureWidth textureHeight 3"]
+
+_DtypeT = TypeVar("_DtypeT", bound=Union[JaxFloating, JaxInteger])
 
 
-class DtypeInfo(NamedTuple):
-    # TODO: use Generic NamedTuple when bump to Python 3.11
-    min: Union[jnp.floating[Any], jnp.integer[Any]]
-    max: Union[jnp.floating[Any], jnp.integer[Any]]
+class DtypeInfo(NamedTuple, Generic[_DtypeT]):
+    min: _DtypeT
+    max: _DtypeT
     bits: int
     dtype: type
 
     @classmethod
     @jaxtyped
     # cannot be jitted as `dtype` will not be a valid JAX type
     def create(cls, dtype: type) -> "DtypeInfo":
@@ -86,12 +88,18 @@
 
     For example, if direction = camera's eye, full specular will be applied to
     triangles with normal towards camera.
     """
     colour: Colour = jax.numpy.ones(3)
 
 
-class Buffers(NamedTuple):
-    """Use lax.full to create buffers and attach here."""
-    # TODO: use Generic NamedTuple when bump to Python 3.11
+_TargetsT = TypeVar("_TargetsT", bound=tuple)
+"""Extra target buffers, must be in shape of (width, height, ...)."""
+
+
+class Buffers(NamedTuple, Generic[_TargetsT]):
+    """Use lax.full to create buffers and attach here.
+
+    targets must be a tuple of arrays with shape of (width, height, ...).
+    """
     zbuffer: ZBuffer
-    targets: tuple[Shaped[Array, "width height ..."]]
+    targets: _TargetsT
```

### Comparing `jaxrenderer-0.3.0/renderer/utils.py` & `jaxrenderer-0.3.1/renderer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations  # tolerate "subscriptable 'type' for < 3.9
+
 from functools import partial
 from typing import Sequence, Union
 
 import jax
 import jax.numpy as jnp
 from jax import lax
 from jaxtyping import Array, Integer, Num, Shaped, jaxtyped
```

### Comparing `jaxrenderer-0.3.0/renderer/value_checker.py` & `jaxrenderer-0.3.1/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.3.0/PKG-INFO` & `jaxrenderer-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
 Requires-Dist: jax (>=0.3.25,<5.0.0)
 Requires-Dist: jaxlib (>=0.3.25,<5.0.0)
-Requires-Dist: jaxtyping (>=0.2.19,<0.3.0)
+Requires-Dist: jaxtyping (>=0.2.13,<0.2.20) ; python_version >= "3.8" and python_version < "3.9"
+Requires-Dist: jaxtyping (>=0.2.19,<0.3.0) ; python_version >= "3.9" and python_version < "4.0"
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
+Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/JoeyTeng/jaxrenderer/issues
 Project-URL: Repository, https://github.com/JoeyTeng/jaxrenderer
 Description-Content-Type: text/markdown
 
 # JAX Renderer
 
 ## Key Difference from [erwincoumans/tinyrenderer](https://github.com/erwincoumans/tinyrenderer)
```

