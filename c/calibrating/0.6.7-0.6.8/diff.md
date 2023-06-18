# Comparing `tmp/calibrating-0.6.7.tar.gz` & `tmp/calibrating-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calibrating-0.6.7.tar", last modified: Thu Apr 27 03:23:07 2023, max compression
+gzip compressed data, was "dist/calibrating-0.6.8.tar", last modified: Sun Jun 18 17:32:07 2023, max compression
```

## Comparing `calibrating-0.6.7.tar` & `calibrating-0.6.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-27 03:23:07.000000 calibrating-0.6.7/
--rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.7/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-27 03:23:07.000000 calibrating-0.6.7/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.7/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating/
--rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-27 03:21:56.000000 calibrating-0.6.7/calibrating/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      280 2023-04-25 05:33:13.000000 calibrating-0.6.7/calibrating/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    18323 2023-04-16 15:28:48.000000 calibrating-0.6.7/calibrating/boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    22684 2023-04-27 03:22:15.000000 calibrating-0.6.7/calibrating/camera.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.7/calibrating/feature_libs.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.7/calibrating/multi_boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.7/calibrating/reconstruction.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    17456 2023-04-25 06:03:55.000000 calibrating-0.6.7/calibrating/stereo.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     6901 2023-04-26 05:50:03.000000 calibrating-0.6.7/calibrating/stereo_matching.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    27170 2023-04-27 03:22:15.000000 calibrating-0.6.7/calibrating/utils.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-27 03:23:07.000000 calibrating-0.6.7/calibrating.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      473 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-27 03:23:06.000000 calibrating-0.6.7/calibrating.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:27:46.000000 calibrating-0.6.7/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-27 03:23:07.000000 calibrating-0.6.7/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.7/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-06-18 17:32:07.000000 calibrating-0.6.8/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.8/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-06-18 17:32:07.000000 calibrating-0.6.8/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.8/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-06-18 17:32:07.000000 calibrating-0.6.8/calibrating/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-06-18 17:31:41.000000 calibrating-0.6.8/calibrating/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      280 2023-04-25 05:33:13.000000 calibrating-0.6.8/calibrating/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    19948 2023-06-16 06:53:09.000000 calibrating-0.6.8/calibrating/boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    22694 2023-05-27 16:24:33.000000 calibrating-0.6.8/calibrating/camera.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.8/calibrating/feature_libs.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.8/calibrating/multi_boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.8/calibrating/reconstruction.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    18022 2023-06-16 06:53:09.000000 calibrating-0.6.8/calibrating/stereo.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     6901 2023-04-26 05:50:03.000000 calibrating-0.6.8/calibrating/stereo_matching.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    27349 2023-06-18 15:56:41.000000 calibrating-0.6.8/calibrating/utils.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-06-18 17:32:07.000000 calibrating-0.6.8/calibrating.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-06-18 17:32:07.000000 calibrating-0.6.8/calibrating.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      473 2023-06-18 17:32:07.000000 calibrating-0.6.8/calibrating.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-06-18 17:32:07.000000 calibrating-0.6.8/calibrating.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-06-18 17:32:07.000000 calibrating-0.6.8/calibrating.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-06-18 17:32:07.000000 calibrating-0.6.8/calibrating.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:27:46.000000 calibrating-0.6.8/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-06-18 17:32:07.000000 calibrating-0.6.8/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.8/setup.py
```

### Comparing `calibrating-0.6.7/PKG-INFO` & `calibrating-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.7
+Version: 0.6.8
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.7/README.md` & `calibrating-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.7/calibrating/__info__.py` & `calibrating-0.6.8/calibrating/__info__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 __description__ = "Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `calibrating-0.6.7/calibrating/boards.py` & `calibrating-0.6.8/calibrating/boards.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,14 +90,54 @@
     def set_origin_to_center(points):
         if isinstance(points, dict):
             center = np.mean(utils.convert_points_for_cv2(points), 0, keepdims=True)
             return {k: v - center for k, v in points.items()}
         else:
             return points - points.mean(0, keepdims=True)
 
+    @classmethod
+    def get_roi_class(cls, roi_udlr=None):
+        class BoardWithRoi(cls):
+            def find_image_points(self, dic):
+                raw_img = dic["img"]
+                h, w = raw_img.shape[:2]
+                if roi_udlr is not None and (
+                    isinstance(roi_udlr, slice) or isinstance(roi_udlr[0], slice)
+                ):
+                    slicee = roi_udlr
+                else:
+                    if roi_udlr is None:
+                        u, d, l, r = (
+                            h // 4,
+                            h * 3 // 4,
+                            w // 4,
+                            w * 3 // 4,
+                        )
+                    else:
+                        u, d, l, r = roi_udlr
+                    slicee = slice(u, d, None), slice(l, r, None)
+                dic["img"] = raw_img[slicee]
+                super().find_image_points(dic)
+                dic["img"] = raw_img
+                l, u = slicee[1].start or 0, slicee[0].start or 0
+                if l < 0:
+                    l = w + l
+                if u < 0:
+                    u = h + u
+                for key in ["image_points", "corners", "marker_corners"]:
+                    if key in dic:
+                        if isinstance(dic[key], dict):
+                            dic[key] = {k: v + (l, u) for k, v in dic[key].items()}
+                        else:
+                            dic[key] = np.ascontiguousarray(
+                                np.float32(dic[key] + (l, u))
+                            )
+
+        return BoardWithRoi
+
 
 class Chessboard(BaseBoard):
     def __init__(self, checkboard=(11, 8), size_mm=25):
         self.init_kwargs = dict(checkboard=checkboard, size_mm=size_mm)
         self.checkboard = checkboard
         self.size_mm = size_mm
         self.object_points = np.zeros(
@@ -107,16 +147,17 @@
             np.mgrid[: self.checkboard[0], : self.checkboard[1]].T.reshape(-1, 2)
             * self.size_mm
             / 1000
         )
         self.object_points = self.set_origin_to_center(self.object_points)
 
     def find_image_points(self, d):
-        img = d["img"]
-        gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        gray = img = d["img"]
+        if img.ndim == 3:
+            gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
         ret, corners = cv2.findChessboardCorners(gray, self.checkboard, None)
         criteria = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 30, 0.01)
         if ret:
             cv2.cornerSubPix(
                 gray,
                 corners,
                 (4, 4),
```

### Comparing `calibrating-0.6.7/calibrating/camera.py` & `calibrating-0.6.8/calibrating/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,22 +550,22 @@
         )
         camd = Cam(
             glob(os.path.join(example_data_dir, "*", "depth_cam_color.jpg")),
             board,
             name="depth",
             enable_cache=True,
         )
-        built_in_intrinsics = dict(
+        camd_built_in_intrinsics = dict(
             fx=1474.1182177692722,
             fy=1474.125874583105,
             cx=1037.599716850734,
             cy=758.3072639103259,
         )
         # depth need to be used in pairs with depth camera's built-in intrinsics
-        camd.load(built_in_intrinsics)
+        camd.load(camd_built_in_intrinsics)
         return caml, camr, camd
 
     @classmethod
     def get_example_720p(cls):
         return cls.load(
             dict(
                 fx=1000,
```

### Comparing `calibrating-0.6.7/calibrating/feature_libs.py` & `calibrating-0.6.8/calibrating/feature_libs.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.7/calibrating/multi_boards.py` & `calibrating-0.6.8/calibrating/multi_boards.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.7/calibrating/reconstruction.py` & `calibrating-0.6.8/calibrating/reconstruction.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.7/calibrating/stereo.py` & `calibrating-0.6.8/calibrating/stereo.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,29 @@
             self.cam1.K, self.cam1.D, self.R1, self.K_target, xy, cv2.CV_32FC1
         )
 
         self.undistort_rectify_map2 = cv2.initUndistortRectifyMap(
             self.cam2.K, self.cam2.D, self.R2, self.K_target, xy, cv2.CV_32FC1
         )
 
+        valid_mask_from_remap = (
+            lambda mapx, mapy, x, y: (-0.5 < mapx)
+            & (mapx < x - 0.5)
+            & (-0.5 < mapy)
+            & (mapy < y - 0.5)
+        )
+
+        self.rectify_valid_mask1 = valid_mask_from_remap(
+            *self.undistort_rectify_map1, *self.cam1.xy
+        )
+        # self.rectify_valid_mask2 = valid_mask_from_remap(*self.undistort_rectify_map2, *self.cam2.xy)
+
+        # TODO add two info
+        # 1. sensor_area_usage% 2. stereo_matching_efficent_rate%
+
         # TODO rm
         # assert (utils.R_t_to_T(self.R2.T) @ utils.R_t_to_T(self.R, self.t))[
         #     0, 3
         # ] < 0, "The left and right cameras may be wrong. Please try to switch the camera order of Stereo(cam1, cam2)"
 
     def stereo_recitfy_by_cv2(self):
         """When the right eye camera is rotated 180° around the z axis, a BUG will appear"""
@@ -464,15 +479,15 @@
         rectify_img1, rectify_img2 = self.rectify(img1, img2)
         disparity = self.stereo_matching(rectify_img1, rectify_img2)
         if isinstance(disparity, dict):
             result.update(disparity)
             disparity = disparity["disparity"]
         if getattr(self, "translation_rectify_img"):
             disparity += self.min_disparity
-
+        disparity = self.rectify_valid_mask1 * disparity
         rectify_depth = self.disparity_to_depth(disparity)
 
         result.update(
             rectify_img1=rectify_img1,
             rectify_depth=rectify_depth,
             disparity=disparity,
             rectify_img2=rectify_img2,
```

### Comparing `calibrating-0.6.7/calibrating/stereo_matching.py` & `calibrating-0.6.8/calibrating/stereo_matching.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.7/calibrating/utils.py` & `calibrating-0.6.8/calibrating/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,26 +314,28 @@
     if constrained_type == True, then only interpolate convexHull area
     """
     mask_to_uvzs = (sparse2d != 0) & np.isfinite(sparse2d)
     uvzs = arr2d_to_uvzs(sparse2d, mask_to_uvzs)
     return interpolate_uvzs(uvzs, sparse2d.shape[:2], constrained_type, inter_type)
 
 
-def interpolate_uvzs(uvzs, hw=None, constrained_type=None, inter_type="lstsq"):
+def interpolate_uvzs(
+    uvzs, hw=None, constrained_type=None, inter_type="lstsq", distance=2
+):
     if hw is None:
         hw = int(uvzs[:, 1].max()) + 2, int(uvzs[:, 0].max()) + 2
     if not uvzs.size:
         return np.zeros(hw, uvzs.dtype)
     input_mask = np.zeros(hw, np.uint8)
     if constrained_type is not None and constrained_type:
         convex_hull = cv2.convexHull(np.int32(uvzs[:, :2].round()))
         cv2.drawContours(input_mask, [convex_hull], -1, 1, -1)
-        input_uvs = arr2d_to_uvzs(input_mask, input_mask)
+        input_uvs = arr2d_to_uvzs(np.zeros_like(input_mask), input_mask)
     else:
-        input_uvs = arr2d_to_uvzs(input_mask)
+        input_uvs = arr2d_to_uvzs(np.zeros_like(input_mask))
 
     # TODO replaced by Solving equations of the z = ay+bx+c
     # fit uvzs linearly
     if inter_type == "rbf":
         import scipy.interpolate
 
         spline = scipy.interpolate.Rbf(
@@ -361,17 +363,17 @@
         from scipy.spatial import KDTree
 
         # with boxx.timeit("KDTree"):
         kdtree = KDTree(uvzs[:, :2])
         output_uvzs = np.float32(input_uvs)
 
         # with boxx.timeit("KDTree.query"):
-        distance, nearest_index = kdtree.query(output_uvzs[:, :2])
+        distance_, nearest_index = kdtree.query(output_uvzs[:, :2])
         # output_uvzs[:, 2] = uvzs[nearest_index, 2]
-        distance_idx = distance < 1.5
+        distance_idx = distance_ < distance
         output_uvzs[distance_idx, 2] = uvzs[nearest_index[distance_idx], 2]
 
         # for i, uv in __import__("tqdm").tqdm(list(enumerate(output_uvzs[:, :2]))):
         #     distance, nearest_index = kdtree.query(uv)
         #     output_uvzs[i, 2] = uvzs[nearest_index, 2]
     # dense = uvzs_to_arr2d(output_uvzs, sparse2d.shape, arr2d=sparse2d.copy())
     dense = uvzs_to_arr2d(output_uvzs, hw)
@@ -502,14 +504,18 @@
     img_or_shape=None,
     size=None,
     color=None,
     contour=False,
     convex_hull=False,
     full_connect=False,
 ):
+    if not isinstance(uvs, np.ndarray):
+        uvs = boxx.npa(uvs)
+    if uvs.ndim == 1:
+        uvs = uvs[None]
     if uvs.ndim == 3 and uvs.shape[1] == 1:
         uvs = uvs[:, 0]
     uvs = np.int32(uvs.round())
     if isinstance(img_or_shape, np.ndarray) and img_or_shape.ndim >= 2:
         vis = img_or_shape.copy()
     else:
         if img_or_shape is None:
@@ -680,22 +686,22 @@
         )
         camd = Cam(
             glob(os.path.join(example_data_dir, "*", "depth_cam_color.jpg")),
             board,
             name="camd",
             enable_cache=True,
         )
-        built_in_intrinsics = dict(
+        camd_built_in_intrinsics = dict(
             fx=1474.1182177692722,
             fy=1474.125874583105,
             cx=1037.599716850734,
             cy=758.3072639103259,
         )
         # depth need to be used in pairs with camera's built-in intrinsics
-        camd.load(built_in_intrinsics)
+        camd.load(camd_built_in_intrinsics)
         return dict(caml=caml, camr=camr, camd=camd)
 
 
 class CvShow:
     """
     Object-oriented Pythonic cv2.imshow
```

### Comparing `calibrating-0.6.7/calibrating.egg-info/PKG-INFO` & `calibrating-0.6.8/calibrating.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.7
+Version: 0.6.8
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.7/setup.py` & `calibrating-0.6.8/setup.py`

 * *Files identical despite different names*

