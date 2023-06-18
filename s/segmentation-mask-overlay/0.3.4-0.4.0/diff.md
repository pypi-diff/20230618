# Comparing `tmp/segmentation-mask-overlay-0.3.4.tar.gz` & `tmp/segmentation-mask-overlay-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation-mask-overlay-0.3.4.tar", last modified: Fri Dec 23 11:53:58 2022, max compression
+gzip compressed data, was "segmentation-mask-overlay-0.4.0.tar", last modified: Sun Jun 18 20:44:45 2023, max compression
```

## Comparing `segmentation-mask-overlay-0.3.4.tar` & `segmentation-mask-overlay-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-12-23 11:53:58.059198 segmentation-mask-overlay-0.3.4/
--rw-r--r--   0 artem      (501) staff       (20)     1072 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/LICENSE
--rw-r--r--   0 artem      (501) staff       (20)       48 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/MANIFEST.in
--rw-r--r--   0 artem      (501) staff       (20)     1866 2022-12-23 11:53:58.059284 segmentation-mask-overlay-0.3.4/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)     1536 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/README.md
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-12-23 11:53:58.052282 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/
--rw-r--r--   0 artem      (501) staff       (20)       32 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/__init__.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-12-23 11:53:58.056366 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/examples/
--rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/examples/cat.jpg
--rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/examples/cat_masked.jpg
--rw-r--r--   0 artem      (501) staff       (20)     3524 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/label_color.py
--rw-r--r--   0 artem      (501) staff       (20)     5344 2022-12-23 11:52:36.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/main.py
--rw-r--r--   0 artem      (501) staff       (20)     2904 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/utils.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-12-23 11:53:58.055114 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay.egg-info/
--rw-r--r--   0 artem      (501) staff       (20)     1866 2022-12-23 11:53:57.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay.egg-info/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)      533 2022-12-23 11:53:57.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (501) staff       (20)        1 2022-12-23 11:53:57.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (501) staff       (20)       74 2022-12-23 11:53:57.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay.egg-info/requires.txt
--rw-r--r--   0 artem      (501) staff       (20)       26 2022-12-23 11:53:57.000000 segmentation-mask-overlay-0.3.4/segmentation_mask_overlay.egg-info/top_level.txt
--rw-r--r--   0 artem      (501) staff       (20)       69 2022-12-23 11:53:58.066712 segmentation-mask-overlay-0.3.4/setup.cfg
--rwx------   0 artem      (501) staff       (20)      858 2022-12-23 11:53:50.000000 segmentation-mask-overlay-0.3.4/setup.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.687200 segmentation-mask-overlay-0.4.0/
+-rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.0/LICENSE
+-rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.0/MANIFEST.in
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-18 20:44:45.687317 segmentation-mask-overlay-0.4.0/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/README.md
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.674756 segmentation-mask-overlay-0.4.0/examples/
+-rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.0/examples/cat.jpg
+-rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.0/examples/cat.py
+-rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.0/examples/cat_masked.jpg
+-rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.0/pyproject.toml
+-rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-18 20:44:45.688393 segmentation-mask-overlay-0.4.0/setup.cfg
+-rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.0/setup.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.641708 segmentation-mask-overlay-0.4.0/src/
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.678713 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/
+-rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-18 20:39:50.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/__init__.py
+-rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/main.py
+-rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/utils.py
+-rw-r--r--   0 artem      (501) staff       (20)     8442 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/video.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.685934 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/
+-rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/requires.txt
+-rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-18 20:44:45.000000 segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay.egg-info/top_level.txt
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-18 20:44:45.686694 segmentation-mask-overlay-0.4.0/tests/
+-rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.0/tests/test_overlay.py
```

### Comparing `segmentation-mask-overlay-0.3.4/LICENSE` & `segmentation-mask-overlay-0.4.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Artem Lobantsev
+Copyright (c) 2023 Artem Lobantsev
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `segmentation-mask-overlay-0.3.4/PKG-INFO` & `segmentation-mask-overlay-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: segmentation-mask-overlay
-Version: 0.3.4
-Summary: Plotting the segmentation masks has never been so exciting!
-Home-page: https://github.com/lobantseff/segmentation-mask-overlay
-Author: armavox
-Author-email: armavox@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Segmentation mask overlay
 
 If you ever wonder to overlay your segmentations onto a picture in the smoothiest way, you're in a right place.
 
 ## Installation
 
     pip install segmentation-mask-overlay
@@ -29,32 +18,32 @@
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image
 from segmentation_mask_overlay import overlay_masks
 
-# [Example] Load image. If you are sure of you masks
+# [Example] Load image
 image = Image.open("cat.jpg").convert("L")
 image = np.array(image)
 
 # [Example] Mimic list of masks
 masks = []
 for i in np.linspace(0, image.shape[1], 10, dtype="int"):
     mask = np.zeros(image.shape, dtype="bool")
     mask[i : i + 100, i : i + 200] = 1
     masks.append(mask)
 
 # [Optional] prepare labels
 mask_labels = [f"Mask_{i}" for i in range(len(masks))]
 
 # [Optional] prepare colors
-cmap = plt.cm.tab20(np.arange(len(mask_labels)))
+cmap = plt.cm.tab20(np.arange(len(mask_labels)))[..., :-1]
 
 # Laminate your image!
-fig = overlay_masks(image, masks, labels=mask_labels, colors=cmap, mask_alpha=0.5)
+fig = array = overlay_masks(image, np.stack(masks, -1), mask_labels, return_type="mpl")
 
 # Do with that image whatever you want to do.
 fig.savefig("cat_masked.png", bbox_inches="tight", dpi=300)
 ```
 
-![Segmented cat](https://raw.githubusercontent.com/lobantseff/segmentation-mask-overlay/master/segmentation_mask_overlay/examples/cat_masked.jpg)
+![Segmented cat](https://raw.githubusercontent.com/lobantseff/segmentation-mask-overlay/master/examples/cat_masked.jpg)
```

### Comparing `segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/examples/cat.jpg` & `segmentation-mask-overlay-0.4.0/examples/cat.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/examples/cat_masked.jpg` & `segmentation-mask-overlay-0.4.0/examples/cat_masked.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.3.4/segmentation_mask_overlay/main.py` & `segmentation-mask-overlay-0.4.0/src/segmentation_mask_overlay/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,150 +1,155 @@
-import os
 from collections.abc import Iterable
 from typing import Optional, Tuple, Union, List
 
+import cv2
 import numpy as np
 import matplotlib.pyplot as plt
+import matplotlib.cm as colormap
 from matplotlib import colors as C
 from matplotlib.patches import Patch
 from PIL import Image as PILImage
-
-from .label_color import LabelColor
-from .utils import open_with_PIL
+from segmentation_mask_overlay.utils import check_convert_image, check_convert_mask
 
 
 def overlay_masks(
-    image: Union[os.PathLike, PILImage.Image, np.ndarray],
-    boolean_masks: Union[np.ndarray, List[np.ndarray]],
-    labels: Optional[List[str]] = None,
+    image: np.ndarray,
+    masks: np.ndarray,
+    labels: List[str],
     colors: Optional[Union[np.ndarray, List[Union[str, List[float]]]]] = None,
-    figsize: Tuple[int, int] = (8, 8),
-    dpi: int = 90,
-    mask_alpha: float = 0.4,
-    mpl_colormap: str = "tab20",
-    return_pil_image: bool = False,
+    alpha: float = 1.0,
+    beta: float = 0.5,
+    return_type: str = "numpy",
+    mpl_figsize: Tuple[int, int] = (8, 8),
+    mpl_dpi: int = 90,
+    concat_original: Optional[str] = None,
 ):
     """Overlays masks on the image.
     Parameters
     ----------
-    image : Union[str, PIL.Image.Image, np.ndarray]
-        Image path or PIl.Image or numpy array. If image size inconsistent with
-        the masks size, image will be resized.
-    boolean_masks : List[np.ndarray[bool]]
-        List of segmentation masks or numpy array of shape (height, width, n_classes).
-        All masks should be the same size, equal to size of the image.
+    image : np.ndarray
+        Image as a numpy array of shape: HWC or HW.
+        The image will be mormalized to [0, 255] and casted to uint8 RGB. Do it manually
+        if you want to control this.
+    mask : np.ndarray[bool | int]
+        Mask should be a numpy array of shape of the image in one of the following forms:
+        - H W C, with bool mask per channel, where each channel represents a class.
+        - H W, with an pixel integer value representing a class.
     labels : Optional[List[str]], optional
-        Optional label names. Provide in the same order as the corresponding masks.
-        If not provided, will be set as range(len(boolean_masks)), by default None
+        Names of expected labels. Provide in the same order as the channels in the masks.
+        If provided, defines 
+        If not provided, will be set as range(mask.shape[-1] | max(mask) + 1), by default None
     colors : Union[np.ndarray, List[Union[str, List[float]]]], optional
-        Array of shape (n_labels x 4) or list of matplotlib acceptable colornames.
-        Example to get persistent colormap: `plt.cm.tab20(np.arange(NUM_LABELS))`
-    figsize : tuple, optional
-        Size in inches of the output image, by default (12, 12)
-    dpi : int, optional
-        Resolution of the output image. Note: 'px, py = w * dpi, h * dpi', by default 120
-    mask_alpha : float, optional
-        Masks opaque value, by default 0.4
+        Array of shape (n_labels x 3) or list of matplotlib acceptable colornames.
+        Example to get persistent colormap: `plt.cm.tab20(np.arange(NUM_LABELS))[..., :-1]`
+    alpha : float, optional
+        Image alpha, by default 1.0
+    beta : float, optional
+        Masks alpha, by default 0.4
     mpl_colormap : str
         Matplotlib colormap name
-    return_pil_image : bool
-        If True, will return PIL image instead of matpotlib figure.
+    return_type : bool, should be numpy | pil | mpl
+        Return numpy array, or PIL image, or matpotlib figure.
+    mpl_figsize : tuple, optional
+        Size in inches of the output matpotlib figure.
+        Valid only if return_type="mpl", by default (12, 12)
+    mpl_dpi : int, optional
+        Resolution of the output matpotlib figure. Note: 'px, py = w * dpi, h * dpi'.
+        Valid only if return_type="mpl", by default 120
+    concat_original: str, optional
+        If provided, should be 'v' or 'h', represention vericat or horisontal concatenation
+        of original image to the image with overlayed masks, by default: None
 
     Returns
     -------
-    plt.Figure | PIL.Image
+    plt.Figure | PIL.Image | np.ndarray
         Output mpl figure or pillow image with masks.
     """
 
-    if isinstance(boolean_masks, np.ndarray):
-        assert (boolean_masks.ndim == 3 and boolean_masks.dtype == bool), (
-            "boolean_masks should be a list boolean numpy"
-            + " arrays or 3-dim numpy array with the last dim"
-            + " as a channel to store masks of different classes"
-        )
-        boolean_masks = [boolean_masks[:, :, i] for i in range(boolean_masks.shape[-1])]
-
-    if labels is not None:
-        assert len(labels) == len(boolean_masks), (
-            "Number of provided labels != number of masks"
-        )
-    else:
-        labels = [f"{_:02d}" for _ in range(len(boolean_masks))]
+    assert image.shape[:2] == masks.shape[:2], "Image and mask should be of the same size"
 
-    pil_image = open_with_PIL(image)
-    image_size = tuple(np.array(pil_image.size)[::-1])
+    num_classes = len(labels)
 
-    assert all(
-        mask.shape == image_size for mask in boolean_masks
-    ), "Label mask size is not equal to image size"
+    image = check_convert_image(image)
+    masks = check_convert_mask(masks, num_classes)
 
     if colors is None:
-        cbar = LabelColor(
-            num_labels=len(boolean_masks),
-            alpha=mask_alpha,
-            return_legend_color=True,
-            mpl_colormap=mpl_colormap,
-        )
+        if num_classes <= 10:
+            colors = colormap.get_cmap("tab10", 10).colors[:num_classes, :-1]
+        else:
+            colors = colormap.get_cmap("rainbow_r", num_classes)(np.arange(num_classes))[:, :-1]
 
     else:
-        assert len(colors) == len(boolean_masks), (
-            "Number of provided colors != number of masks"
-        )
+        assert len(colors) == num_classes, "Number of provided colors != number of labels"
         if all(isinstance(c, str) for c in colors):
-            colors = [C.to_rgba(c) for c in colors]
+            colors = [C.to_rgb(c) for c in colors]
 
         if isinstance(colors, Iterable):
             colors = np.array(colors)
 
-        assert colors.ndim == 2 and colors.shape[-1] == 4, (
+        assert colors.ndim == 2 and colors.shape[-1] == 3, (
             "Unsupported color format:"
             + " should be list of matplotlib colorname strings for each mask/mask_channel,"
-            + " list of RGBA arrays or 2-dim numpy array of shape (n_labels x 4)"
+            + " list of RGB arrays or 2-dim numpy array of shape (n_labels x 3)"
         )
 
-        mask_colors = colors.copy()
-        mask_colors[:, -1] *= mask_alpha
-        mask_colors = (mask_colors * 255).astype("uint8")
-        cbar = zip(mask_colors, colors)
+    mask_colors = colors.copy()
+    mask_colors = (mask_colors * 255).astype(np.uint8)
+    cbar = list(zip(mask_colors, colors))
 
-    segmentation_overlay = np.zeros((*image_size, 4), dtype=np.uint16)
-    segmentation_mask = np.zeros(image_size, dtype=bool)
+    segmentation_overlay = np.zeros_like(image, dtype=np.uint16)
+    segmentation_mask = np.zeros(image.shape[:2], dtype=bool)
     legend_elements = []
 
-    for mask, label, (color, legend_color) in zip(boolean_masks, labels, cbar):
-
-        assert mask.dtype == "bool"
+    for i in range(num_classes):
+        label = labels[i]
+        mask = masks[..., i]
+        color, legend_color = cbar[i]
 
         intersection = mask & segmentation_mask
         segmentation_mask = mask | segmentation_mask
 
         # Paint non-overlapping area
         segmentation_overlay[mask ^ intersection] = color
 
         # Blend overlapping area
-        segmentation_overlay[intersection] = (
-            segmentation_overlay[intersection] + color
-        ) / 2
+        segmentation_overlay[intersection] = (segmentation_overlay[intersection] + color) // 2
 
         legend_elements.append(Patch(color=legend_color, label=label))
 
-    segmentation_overlay = PILImage.fromarray(segmentation_overlay.astype("uint8"))
-    pil_image.paste(segmentation_overlay, mask=segmentation_overlay)
+    overlayed = cv2.addWeighted(image, alpha, segmentation_overlay.astype(np.uint8), beta, 0)
 
-    if return_pil_image:
+    if concat_original is not None:
+        if concat_original == "h":
+            overlayed = np.concatenate((image, overlayed), 1)
+            mpl_figsize = (mpl_figsize[0] * 2, mpl_figsize[1])
+        elif concat_original == "v":
+            overlayed = np.concatenate((image, overlayed), 0)
+            mpl_figsize = (mpl_figsize[0], mpl_figsize[1] * 2)
+        else:
+            raise AssertionError("If provided, concat_original should be in v | h")
+
+    if return_type == "numpy":
+        return overlayed
+
+    elif return_type == "pil":
+        pil_image = PILImage.fromarray(overlayed)
         return pil_image
-    
-    else:
-        fig = plt.figure(figsize=figsize, dpi=dpi)
-        plt.imshow(pil_image)
+
+    elif return_type == "mpl":
+        fig = plt.figure(figsize=mpl_figsize, dpi=mpl_dpi)
+        plt.subplots_adjust(left=0, right=1, bottom=0, top=1, wspace=0, hspace=0)
+        plt.imshow(overlayed, vmin=0, vmax=255)
         plt.axis("off")
         mask_legend = plt.legend(
             handles=legend_elements,
             loc="upper left",
             frameon=False,
             bbox_to_anchor=(1.01, 1),
         )
         plt.subplots_adjust(left=0.8)
         plt.tight_layout()
         plt.gca().add_artist(mask_legend)
-
         return fig
+
+    else:
+        raise AssertionError("return_type arg should be numpy | pil | mpl")
```

### Comparing `segmentation-mask-overlay-0.3.4/segmentation_mask_overlay.egg-info/PKG-INFO` & `segmentation-mask-overlay-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.3.4
+Version: 0.4.0
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
-Author: armavox
-Author-email: armavox@gmail.com
+Author: Artem Lobantsev
+Author-email: lobantseff@gmail.com
 License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Segmentation mask overlay
 
 If you ever wonder to overlay your segmentations onto a picture in the smoothiest way, you're in a right place.
 
@@ -29,32 +33,32 @@
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image
 from segmentation_mask_overlay import overlay_masks
 
-# [Example] Load image. If you are sure of you masks
+# [Example] Load image
 image = Image.open("cat.jpg").convert("L")
 image = np.array(image)
 
 # [Example] Mimic list of masks
 masks = []
 for i in np.linspace(0, image.shape[1], 10, dtype="int"):
     mask = np.zeros(image.shape, dtype="bool")
     mask[i : i + 100, i : i + 200] = 1
     masks.append(mask)
 
 # [Optional] prepare labels
 mask_labels = [f"Mask_{i}" for i in range(len(masks))]
 
 # [Optional] prepare colors
-cmap = plt.cm.tab20(np.arange(len(mask_labels)))
+cmap = plt.cm.tab20(np.arange(len(mask_labels)))[..., :-1]
 
 # Laminate your image!
-fig = overlay_masks(image, masks, labels=mask_labels, colors=cmap, mask_alpha=0.5)
+fig = array = overlay_masks(image, np.stack(masks, -1), mask_labels, return_type="mpl")
 
 # Do with that image whatever you want to do.
 fig.savefig("cat_masked.png", bbox_inches="tight", dpi=300)
 ```
 
-![Segmented cat](https://raw.githubusercontent.com/lobantseff/segmentation-mask-overlay/master/segmentation_mask_overlay/examples/cat_masked.jpg)
+![Segmented cat](https://raw.githubusercontent.com/lobantseff/segmentation-mask-overlay/master/examples/cat_masked.jpg)
```

