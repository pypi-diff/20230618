# Comparing `tmp/mlfactory-0.0.7.tar.gz` & `tmp/mlfactory-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfactory-0.0.7.tar", last modified: Mon May 22 15:56:39 2023, max compression
+gzip compressed data, was "mlfactory-0.0.8.tar", last modified: Sun Jun 18 16:33:40 2023, max compression
```

## Comparing `mlfactory-0.0.7.tar` & `mlfactory-0.0.8.tar`

### file list

```diff
@@ -1,126 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.376442 mlfactory-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     2793 2023-05-22 15:56:39.376442 mlfactory-0.0.7/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     2254 2023-05-22 12:56:59.000000 mlfactory-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.364442 mlfactory-0.0.7/mlfactory/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 19:40:33.000000 mlfactory-0.0.7/mlfactory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.364442 mlfactory-0.0.7/mlfactory/applications/
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.0.7/mlfactory/applications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.364442 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-17 19:41:17.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-05-22 15:53:45.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/mapper.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-05-22 15:20:53.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/read_video.py
--rw-r--r--   0 root         (0) root         (0)    16458 2023-05-17 23:39:19.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.364442 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5309 2023-05-21 17:44:26.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py
--rw-r--r--   0 root         (0) root         (0)     7013 2023-05-22 15:16:40.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-05-22 15:05:37.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-03-24 18:22:37.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
--rw-r--r--   0 root         (0) root         (0)    10274 2023-05-22 15:49:41.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
--rw-r--r--   0 root         (0) root         (0)     1324 2022-08-18 10:40:00.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
--rw-r--r--   0 root         (0) root         (0)     4761 2023-04-21 14:19:44.000000 mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2947 2023-04-20 19:13:46.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-04-02 23:52:08.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/datahandler.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-04-02 23:52:08.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/main.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-04-02 23:52:08.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/model.py
--rw-r--r--   0 root         (0) root         (0)     5507 2023-04-02 23:52:08.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/segdataset.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-04-20 20:15:23.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/test.py
--rw-r--r--   0 root         (0) root         (0)     3578 2023-04-02 23:52:08.000000 mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/applications/superglue_inference/
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 19:44:47.000000 mlfactory-0.0.7/mlfactory/applications/superglue_inference/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8832 2023-05-22 14:19:20.000000 mlfactory-0.0.7/mlfactory/applications/superglue_inference/match_pair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-07 16:11:34.000000 mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3417 2022-10-07 16:11:34.000000 mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/matching.py
--rw-r--r--   0 root         (0) root         (0)    11781 2022-10-07 16:11:34.000000 mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/superglue.py
--rw-r--r--   0 root         (0) root         (0)     8142 2022-10-07 16:11:34.000000 mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/superpoint.py
--rw-r--r--   0 root         (0) root         (0)    20039 2022-10-07 16:11:34.000000 mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/custom_losses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/custom_losses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/custom_losses/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/custom_losses/pytorch/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4036 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/custom_losses/pytorch/depth.py
--rw-r--r--   0 root         (0) root         (0)     1448 2022-10-05 16:29:32.000000 mlfactory-0.0.7/mlfactory/custom_losses/pytorch/pointnetloss.py
--rwxr-xr-x   0 root         (0) root         (0)      190 2023-04-15 14:33:36.000000 mlfactory-0.0.7/mlfactory/custom_losses/pytorch/regress.py
--rwxr-xr-x   0 root         (0) root         (0)      957 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/custom_losses/pytorch/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/custom_losses/tensorflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/custom_losses/tensorflow/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1445 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/custom_losses/tensorflow/feature_detect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/datacreators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/datacreators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/datacreators/ai2thor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/datacreators/ai2thor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7962 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/datacreators/ai2thor/create_dataset.py
--rwxr-xr-x   0 root         (0) root         (0)     5970 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/datacreators/ai2thor/register_pcds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/datacreators/lidar_contours/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/datacreators/lidar_contours/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6484 2022-11-05 15:28:48.000000 mlfactory-0.0.7/mlfactory/datacreators/lidar_contours/human_contours.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/datacreators/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/datacreators/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-14 17:50:57.000000 mlfactory-0.0.7/mlfactory/datacreators/utils/colab_poly_anot.py
--rwxr-xr-x   0 root         (0) root         (0)    10241 2022-11-04 20:33:18.000000 mlfactory-0.0.7/mlfactory/datacreators/utils/cv_annotator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.368442 mlfactory-0.0.7/mlfactory/dataloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/dataloaders/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    11455 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/dataloaders/ade20k.py
--rwxr-xr-x   0 root         (0) root         (0)     3651 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/dataloaders/cihp.py
--rwxr-xr-x   0 root         (0) root         (0)     9524 2023-04-13 01:43:27.000000 mlfactory-0.0.7/mlfactory/dataloaders/coco.py
--rwxr-xr-x   0 root         (0) root         (0)     7066 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/dataloaders/diode.py
--rwxr-xr-x   0 root         (0) root         (0)    11385 2022-11-06 16:02:08.000000 mlfactory-0.0.7/mlfactory/dataloaders/imgcsvloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/dataloaders/lidar_datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/dataloaders/lidar_datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18754 2022-10-05 16:29:32.000000 mlfactory-0.0.7/mlfactory/dataloaders/lidar_datasets/loader.py
--rw-r--r--   0 root         (0) root         (0)    21285 2022-09-09 17:47:12.000000 mlfactory-0.0.7/mlfactory/dataloaders/lidar_datasets/nuscenes.py
--rwxr-xr-x   0 root         (0) root         (0)     8461 2022-09-28 13:48:03.000000 mlfactory-0.0.7/mlfactory/dataloaders/modelnet.py
--rwxr-xr-x   0 root         (0) root         (0)    13990 2023-03-31 14:21:57.000000 mlfactory-0.0.7/mlfactory/dataloaders/nyuv2.py
--rwxr-xr-x   0 root         (0) root         (0)    11237 2023-04-23 12:18:32.000000 mlfactory-0.0.7/mlfactory/dataloaders/ouster_extract.py
--rwxr-xr-x   0 root         (0) root         (0)    10154 2022-09-28 13:48:03.000000 mlfactory-0.0.7/mlfactory/dataloaders/shapenet.py
--rwxr-xr-x   0 root         (0) root         (0)    12429 2023-04-15 20:17:10.000000 mlfactory-0.0.7/mlfactory/dataloaders/tum_rgbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/dataloaders/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/dataloaders/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3421 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/dataloaders/utils/augmentations.py
--rwxr-xr-x   0 root         (0) root         (0)     6487 2022-09-28 13:48:03.000000 mlfactory-0.0.7/mlfactory/dataloaders/utils/pointcloud_voxelize.py
--rwxr-xr-x   0 root         (0) root         (0)    12996 2022-11-04 23:51:47.000000 mlfactory-0.0.7/mlfactory/dataloaders/utils/read_supervisely.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/misctools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/misctools/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5880 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/misctools/median_filter.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-03-30 12:42:54.000000 mlfactory-0.0.7/mlfactory/misctools/pretrained_od.py
--rwxr-xr-x   0 root         (0) root         (0)     5121 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/misctools/random_homography.py
--rwxr-xr-x   0 root         (0) root         (0)     1663 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/misctools/sift_matching.py
--rwxr-xr-x   0 root         (0) root         (0)     6140 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/misctools/trifocal_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-03-30 12:42:54.000000 mlfactory-0.0.7/mlfactory/misctools/video_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/models/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/models/pytorch/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10250 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/models/pytorch/deeplabv3.py
--rwxr-xr-x   0 root         (0) root         (0)     4228 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/models/pytorch/feature_pyramid.py
--rw-r--r--   0 root         (0) root         (0)    10977 2022-09-28 13:48:03.000000 mlfactory-0.0.7/mlfactory/models/pytorch/pointnet.py
--rwxr-xr-x   0 root         (0) root         (0)     3269 2023-04-15 19:06:02.000000 mlfactory-0.0.7/mlfactory/models/pytorch/regressor.py
--rwxr-xr-x   0 root         (0) root         (0)     1305 2022-11-28 13:47:33.000000 mlfactory-0.0.7/mlfactory/models/pytorch/simple_conv.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/models/pytorch/unet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/trainers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/trainers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/trainers/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/trainers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5027 2022-10-05 16:29:32.000000 mlfactory-0.0.7/mlfactory/trainers/pytorch/train_pointcloud.py
--rwxr-xr-x   0 root         (0) root         (0)     2632 2023-04-15 19:06:56.000000 mlfactory-0.0.7/mlfactory/trainers/pytorch/train_reg.py
--rwxr-xr-x   0 root         (0) root         (0)     3375 2022-08-06 01:28:36.000000 mlfactory-0.0.7/mlfactory/trainers/pytorch/train_seg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/trainers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/trainers/tensorflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/trainers/tensorflow/object_detection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/trainers/tensorflow/object_detection/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5095 2022-11-05 18:56:21.000000 mlfactory-0.0.7/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.372442 mlfactory-0.0.7/mlfactory/visualizers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.7/mlfactory/visualizers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9415 2023-04-19 21:27:23.000000 mlfactory-0.0.7/mlfactory/visualizers/pointcloud.py
--rw-r--r--   0 root         (0) root         (0)    12514 2023-04-19 22:14:46.000000 mlfactory-0.0.7/mlfactory/visualizers/project_rgbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:56:39.364442 mlfactory-0.0.7/mlfactory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2793 2023-05-22 15:56:39.000000 mlfactory-0.0.7/mlfactory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4456 2023-05-22 15:56:39.000000 mlfactory-0.0.7/mlfactory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 15:56:39.000000 mlfactory-0.0.7/mlfactory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-22 15:56:39.000000 mlfactory-0.0.7/mlfactory.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-22 15:55:48.000000 mlfactory-0.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 15:56:39.376442 mlfactory-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      811 2023-05-22 15:55:54.000000 mlfactory-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.883071 mlfactory-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-06-18 16:33:40.883071 mlfactory-0.0.8/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     2438 2023-06-18 16:32:03.000000 mlfactory-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.859071 mlfactory-0.0.8/mlfactory/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 19:40:33.000000 mlfactory-0.0.8/mlfactory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.859071 mlfactory-0.0.8/mlfactory/applications/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.0.8/mlfactory/applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.859071 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-17 19:41:17.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-05-22 15:53:45.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/mapper.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-05-22 15:20:53.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/read_video.py
+-rw-r--r--   0 root         (0) root         (0)    16458 2023-05-17 23:39:19.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.863071 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5309 2023-05-21 17:44:26.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2023-05-22 15:16:40.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-05-22 15:05:37.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-03-24 18:22:37.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    10274 2023-05-22 15:49:41.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2022-08-18 10:40:00.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-04-21 14:19:44.000000 mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.863071 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2947 2023-04-20 19:13:46.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-04-02 23:52:08.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/datahandler.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-04-02 23:52:08.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/main.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-04-02 23:52:08.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/model.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-04-02 23:52:08.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/segdataset.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-04-20 20:15:23.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/test.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2023-04-02 23:52:08.000000 mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.863071 mlfactory-0.0.8/mlfactory/applications/superglue_inference/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 19:44:47.000000 mlfactory-0.0.8/mlfactory/applications/superglue_inference/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8832 2023-05-22 14:19:20.000000 mlfactory-0.0.8/mlfactory/applications/superglue_inference/match_pair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.867071 mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-10-07 16:11:34.000000 mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2022-10-07 16:11:34.000000 mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/matching.py
+-rw-r--r--   0 root         (0) root         (0)    11781 2022-10-07 16:11:34.000000 mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/superglue.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2022-10-07 16:11:34.000000 mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/superpoint.py
+-rw-r--r--   0 root         (0) root         (0)    20039 2022-10-07 16:11:34.000000 mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.867071 mlfactory-0.0.8/mlfactory/applications/visual_odometry/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.0.8/mlfactory/applications/visual_odometry/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21828 2023-06-18 16:23:04.000000 mlfactory-0.0.8/mlfactory/applications/visual_odometry/sfm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.867071 mlfactory-0.0.8/mlfactory/custom_losses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/custom_losses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.867071 mlfactory-0.0.8/mlfactory/custom_losses/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/custom_losses/pytorch/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4036 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/custom_losses/pytorch/depth.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2022-10-05 16:29:32.000000 mlfactory-0.0.8/mlfactory/custom_losses/pytorch/pointnetloss.py
+-rwxr-xr-x   0 root         (0) root         (0)      190 2023-04-15 14:33:36.000000 mlfactory-0.0.8/mlfactory/custom_losses/pytorch/regress.py
+-rwxr-xr-x   0 root         (0) root         (0)      957 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/custom_losses/pytorch/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.867071 mlfactory-0.0.8/mlfactory/custom_losses/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/custom_losses/tensorflow/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1445 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/custom_losses/tensorflow/feature_detect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.867071 mlfactory-0.0.8/mlfactory/datacreators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/datacreators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.871071 mlfactory-0.0.8/mlfactory/datacreators/ai2thor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/datacreators/ai2thor/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7962 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/datacreators/ai2thor/create_dataset.py
+-rwxr-xr-x   0 root         (0) root         (0)     5970 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/datacreators/ai2thor/register_pcds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.871071 mlfactory-0.0.8/mlfactory/datacreators/lidar_contours/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/datacreators/lidar_contours/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6484 2022-11-05 15:28:48.000000 mlfactory-0.0.8/mlfactory/datacreators/lidar_contours/human_contours.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.871071 mlfactory-0.0.8/mlfactory/datacreators/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/datacreators/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-14 17:50:57.000000 mlfactory-0.0.8/mlfactory/datacreators/utils/colab_poly_anot.py
+-rwxr-xr-x   0 root         (0) root         (0)    10241 2022-11-04 20:33:18.000000 mlfactory-0.0.8/mlfactory/datacreators/utils/cv_annotator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.875071 mlfactory-0.0.8/mlfactory/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/dataloaders/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    11455 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/dataloaders/ade20k.py
+-rwxr-xr-x   0 root         (0) root         (0)     3651 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/dataloaders/cihp.py
+-rwxr-xr-x   0 root         (0) root         (0)     9524 2023-04-13 01:43:27.000000 mlfactory-0.0.8/mlfactory/dataloaders/coco.py
+-rwxr-xr-x   0 root         (0) root         (0)     7066 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/dataloaders/diode.py
+-rwxr-xr-x   0 root         (0) root         (0)    11385 2022-11-06 16:02:08.000000 mlfactory-0.0.8/mlfactory/dataloaders/imgcsvloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.875071 mlfactory-0.0.8/mlfactory/dataloaders/lidar_datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/dataloaders/lidar_datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18754 2022-10-05 16:29:32.000000 mlfactory-0.0.8/mlfactory/dataloaders/lidar_datasets/loader.py
+-rw-r--r--   0 root         (0) root         (0)    21285 2022-09-09 17:47:12.000000 mlfactory-0.0.8/mlfactory/dataloaders/lidar_datasets/nuscenes.py
+-rwxr-xr-x   0 root         (0) root         (0)     8461 2022-09-28 13:48:03.000000 mlfactory-0.0.8/mlfactory/dataloaders/modelnet.py
+-rwxr-xr-x   0 root         (0) root         (0)    13990 2023-03-31 14:21:57.000000 mlfactory-0.0.8/mlfactory/dataloaders/nyuv2.py
+-rwxr-xr-x   0 root         (0) root         (0)    11237 2023-04-23 12:18:32.000000 mlfactory-0.0.8/mlfactory/dataloaders/ouster_extract.py
+-rwxr-xr-x   0 root         (0) root         (0)    10154 2022-09-28 13:48:03.000000 mlfactory-0.0.8/mlfactory/dataloaders/shapenet.py
+-rwxr-xr-x   0 root         (0) root         (0)    12429 2023-04-15 20:17:10.000000 mlfactory-0.0.8/mlfactory/dataloaders/tum_rgbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.875071 mlfactory-0.0.8/mlfactory/dataloaders/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/dataloaders/utils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3421 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/dataloaders/utils/augmentations.py
+-rwxr-xr-x   0 root         (0) root         (0)     6487 2022-09-28 13:48:03.000000 mlfactory-0.0.8/mlfactory/dataloaders/utils/pointcloud_voxelize.py
+-rwxr-xr-x   0 root         (0) root         (0)    12996 2022-11-04 23:51:47.000000 mlfactory-0.0.8/mlfactory/dataloaders/utils/read_supervisely.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.879071 mlfactory-0.0.8/mlfactory/misctools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/misctools/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5880 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/misctools/median_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-03-30 12:42:54.000000 mlfactory-0.0.8/mlfactory/misctools/pretrained_od.py
+-rwxr-xr-x   0 root         (0) root         (0)     5121 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/misctools/random_homography.py
+-rwxr-xr-x   0 root         (0) root         (0)     1663 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/misctools/sift_matching.py
+-rwxr-xr-x   0 root         (0) root         (0)     6140 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/misctools/trifocal_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-03-30 12:42:54.000000 mlfactory-0.0.8/mlfactory/misctools/video_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.879071 mlfactory-0.0.8/mlfactory/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.879071 mlfactory-0.0.8/mlfactory/models/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/models/pytorch/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10250 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/models/pytorch/deeplabv3.py
+-rwxr-xr-x   0 root         (0) root         (0)     4228 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/models/pytorch/feature_pyramid.py
+-rw-r--r--   0 root         (0) root         (0)    10977 2022-09-28 13:48:03.000000 mlfactory-0.0.8/mlfactory/models/pytorch/pointnet.py
+-rwxr-xr-x   0 root         (0) root         (0)     3269 2023-04-15 19:06:02.000000 mlfactory-0.0.8/mlfactory/models/pytorch/regressor.py
+-rwxr-xr-x   0 root         (0) root         (0)     1305 2022-11-28 13:47:33.000000 mlfactory-0.0.8/mlfactory/models/pytorch/simple_conv.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/models/pytorch/unet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.879071 mlfactory-0.0.8/mlfactory/trainers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/trainers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.879071 mlfactory-0.0.8/mlfactory/trainers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/trainers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2022-10-05 16:29:32.000000 mlfactory-0.0.8/mlfactory/trainers/pytorch/train_pointcloud.py
+-rwxr-xr-x   0 root         (0) root         (0)     2632 2023-04-15 19:06:56.000000 mlfactory-0.0.8/mlfactory/trainers/pytorch/train_reg.py
+-rwxr-xr-x   0 root         (0) root         (0)     3375 2022-08-06 01:28:36.000000 mlfactory-0.0.8/mlfactory/trainers/pytorch/train_seg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.879071 mlfactory-0.0.8/mlfactory/trainers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/trainers/tensorflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.879071 mlfactory-0.0.8/mlfactory/trainers/tensorflow/object_detection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/trainers/tensorflow/object_detection/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5095 2022-11-05 18:56:21.000000 mlfactory-0.0.8/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.883071 mlfactory-0.0.8/mlfactory/visualizers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.8/mlfactory/visualizers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9415 2023-04-19 21:27:23.000000 mlfactory-0.0.8/mlfactory/visualizers/pointcloud.py
+-rw-r--r--   0 root         (0) root         (0)    12514 2023-04-19 22:14:46.000000 mlfactory-0.0.8/mlfactory/visualizers/project_rgbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:33:40.859071 mlfactory-0.0.8/mlfactory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-06-18 16:33:40.000000 mlfactory-0.0.8/mlfactory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-06-18 16:33:40.000000 mlfactory-0.0.8/mlfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 16:33:40.000000 mlfactory-0.0.8/mlfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-18 16:33:40.000000 mlfactory-0.0.8/mlfactory.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-18 16:29:25.000000 mlfactory-0.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 16:33:40.883071 mlfactory-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      811 2023-06-18 16:29:34.000000 mlfactory-0.0.8/setup.py
```

### Comparing `mlfactory-0.0.7/PKG-INFO` & `mlfactory-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfactory
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collection of several machine learning modules which can be applied to diverse projects
 Home-page: https://github.com/Homagn/mlfactory
 Author: Homagni Saha
 Author-email: Homagni Saha <homagnisaha@gmail.com>
 Project-URL: Homepage, https://github.com/Homagn/mlfactory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,16 @@
 
 Machine Learning and AI applications full pipeline
 --------------------------------------------------
 
 1. High definition mapping using monocular camera (using monocular depth estimation and superglue feature extractor)
 - https://colab.research.google.com/drive/1lZYHjYszROIvMjtZgAp7r5eL1YZC9x9M?usp=sharing
 
+2. Simple and fast visual odometry directly from MOV files and output pose trajectory in open3d
+- https://colab.research.google.com/drive/1Nr1nYFBKieDQG6UeNsnrV4gHh-l-65G0?usp=sharing
 
 Compose machine learning applications in a modular way
 ------------------------------------------------------
 
 1. (NYUV2 dataloader) Easy monocular depth estimation 
 - https://colab.research.google.com/drive/1T2gONs_gst4zpdS7fBoIaQclgg3J2Jgk?usp=sharing
```

### Comparing `mlfactory-0.0.7/README.md` & `mlfactory-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 Machine Learning and AI applications full pipeline
 --------------------------------------------------
 
 1. High definition mapping using monocular camera (using monocular depth estimation and superglue feature extractor)
 - https://colab.research.google.com/drive/1lZYHjYszROIvMjtZgAp7r5eL1YZC9x9M?usp=sharing
 
+2. Simple and fast visual odometry directly from MOV files and output pose trajectory in open3d
+- https://colab.research.google.com/drive/1Nr1nYFBKieDQG6UeNsnrV4gHh-l-65G0?usp=sharing
 
 Compose machine learning applications in a modular way
 ------------------------------------------------------
 
 1. (NYUV2 dataloader) Easy monocular depth estimation 
 - https://colab.research.google.com/drive/1T2gONs_gst4zpdS7fBoIaQclgg3J2Jgk?usp=sharing
```

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/mapper.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/read_video.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/read_video.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py` & `mlfactory-0.0.8/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py` & `mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/datahandler.py` & `mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/datahandler.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/main.py` & `mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/main.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/model.py` & `mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/model.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/segdataset.py` & `mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/segdataset.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/test.py` & `mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/test.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/segmentation_finetune/trainer.py` & `mlfactory-0.0.8/mlfactory/applications/segmentation_finetune/trainer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/superglue_inference/match_pair.py` & `mlfactory-0.0.8/mlfactory/applications/superglue_inference/match_pair.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/matching.py` & `mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/superglue.py` & `mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/superglue.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/superpoint.py` & `mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/applications/superglue_inference/models/utils.py` & `mlfactory-0.0.8/mlfactory/applications/superglue_inference/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/custom_losses/pytorch/depth.py` & `mlfactory-0.0.8/mlfactory/custom_losses/pytorch/depth.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/custom_losses/pytorch/pointnetloss.py` & `mlfactory-0.0.8/mlfactory/custom_losses/pytorch/pointnetloss.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/custom_losses/pytorch/segment.py` & `mlfactory-0.0.8/mlfactory/custom_losses/pytorch/segment.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/custom_losses/tensorflow/feature_detect.py` & `mlfactory-0.0.8/mlfactory/custom_losses/tensorflow/feature_detect.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/datacreators/ai2thor/create_dataset.py` & `mlfactory-0.0.8/mlfactory/datacreators/ai2thor/create_dataset.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/datacreators/ai2thor/register_pcds.py` & `mlfactory-0.0.8/mlfactory/datacreators/ai2thor/register_pcds.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/datacreators/lidar_contours/human_contours.py` & `mlfactory-0.0.8/mlfactory/datacreators/lidar_contours/human_contours.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/datacreators/utils/colab_poly_anot.py` & `mlfactory-0.0.8/mlfactory/datacreators/utils/colab_poly_anot.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/datacreators/utils/cv_annotator.py` & `mlfactory-0.0.8/mlfactory/datacreators/utils/cv_annotator.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/ade20k.py` & `mlfactory-0.0.8/mlfactory/dataloaders/ade20k.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/cihp.py` & `mlfactory-0.0.8/mlfactory/dataloaders/cihp.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/coco.py` & `mlfactory-0.0.8/mlfactory/dataloaders/coco.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/diode.py` & `mlfactory-0.0.8/mlfactory/dataloaders/diode.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/imgcsvloader.py` & `mlfactory-0.0.8/mlfactory/dataloaders/imgcsvloader.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/lidar_datasets/loader.py` & `mlfactory-0.0.8/mlfactory/dataloaders/lidar_datasets/loader.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/lidar_datasets/nuscenes.py` & `mlfactory-0.0.8/mlfactory/dataloaders/lidar_datasets/nuscenes.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/modelnet.py` & `mlfactory-0.0.8/mlfactory/dataloaders/modelnet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/nyuv2.py` & `mlfactory-0.0.8/mlfactory/dataloaders/nyuv2.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/ouster_extract.py` & `mlfactory-0.0.8/mlfactory/dataloaders/ouster_extract.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/shapenet.py` & `mlfactory-0.0.8/mlfactory/dataloaders/shapenet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/tum_rgbd.py` & `mlfactory-0.0.8/mlfactory/dataloaders/tum_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/utils/augmentations.py` & `mlfactory-0.0.8/mlfactory/dataloaders/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/utils/pointcloud_voxelize.py` & `mlfactory-0.0.8/mlfactory/dataloaders/utils/pointcloud_voxelize.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/dataloaders/utils/read_supervisely.py` & `mlfactory-0.0.8/mlfactory/dataloaders/utils/read_supervisely.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/misctools/median_filter.py` & `mlfactory-0.0.8/mlfactory/misctools/median_filter.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/misctools/pretrained_od.py` & `mlfactory-0.0.8/mlfactory/misctools/pretrained_od.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/misctools/random_homography.py` & `mlfactory-0.0.8/mlfactory/misctools/random_homography.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/misctools/sift_matching.py` & `mlfactory-0.0.8/mlfactory/misctools/sift_matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/misctools/trifocal_tensor.py` & `mlfactory-0.0.8/mlfactory/misctools/trifocal_tensor.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/misctools/video_writer.py` & `mlfactory-0.0.8/mlfactory/misctools/video_writer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/models/pytorch/deeplabv3.py` & `mlfactory-0.0.8/mlfactory/models/pytorch/deeplabv3.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/models/pytorch/feature_pyramid.py` & `mlfactory-0.0.8/mlfactory/models/pytorch/feature_pyramid.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/models/pytorch/pointnet.py` & `mlfactory-0.0.8/mlfactory/models/pytorch/pointnet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/models/pytorch/regressor.py` & `mlfactory-0.0.8/mlfactory/models/pytorch/regressor.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/models/pytorch/simple_conv.py` & `mlfactory-0.0.8/mlfactory/models/pytorch/simple_conv.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/models/pytorch/unet.py` & `mlfactory-0.0.8/mlfactory/models/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/trainers/pytorch/train_pointcloud.py` & `mlfactory-0.0.8/mlfactory/trainers/pytorch/train_pointcloud.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/trainers/pytorch/train_reg.py` & `mlfactory-0.0.8/mlfactory/trainers/pytorch/train_reg.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/trainers/pytorch/train_seg.py` & `mlfactory-0.0.8/mlfactory/trainers/pytorch/train_seg.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py` & `mlfactory-0.0.8/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/visualizers/pointcloud.py` & `mlfactory-0.0.8/mlfactory/visualizers/pointcloud.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory/visualizers/project_rgbd.py` & `mlfactory-0.0.8/mlfactory/visualizers/project_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.7/mlfactory.egg-info/PKG-INFO` & `mlfactory-0.0.8/mlfactory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfactory
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collection of several machine learning modules which can be applied to diverse projects
 Home-page: https://github.com/Homagn/mlfactory
 Author: Homagni Saha
 Author-email: Homagni Saha <homagnisaha@gmail.com>
 Project-URL: Homepage, https://github.com/Homagn/mlfactory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,16 @@
 
 Machine Learning and AI applications full pipeline
 --------------------------------------------------
 
 1. High definition mapping using monocular camera (using monocular depth estimation and superglue feature extractor)
 - https://colab.research.google.com/drive/1lZYHjYszROIvMjtZgAp7r5eL1YZC9x9M?usp=sharing
 
+2. Simple and fast visual odometry directly from MOV files and output pose trajectory in open3d
+- https://colab.research.google.com/drive/1Nr1nYFBKieDQG6UeNsnrV4gHh-l-65G0?usp=sharing
 
 Compose machine learning applications in a modular way
 ------------------------------------------------------
 
 1. (NYUV2 dataloader) Easy monocular depth estimation 
 - https://colab.research.google.com/drive/1T2gONs_gst4zpdS7fBoIaQclgg3J2Jgk?usp=sharing
```

### Comparing `mlfactory-0.0.7/mlfactory.egg-info/SOURCES.txt` & `mlfactory-0.0.8/mlfactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 mlfactory/applications/superglue_inference/__init__.py
 mlfactory/applications/superglue_inference/match_pair.py
 mlfactory/applications/superglue_inference/models/__init__.py
 mlfactory/applications/superglue_inference/models/matching.py
 mlfactory/applications/superglue_inference/models/superglue.py
 mlfactory/applications/superglue_inference/models/superpoint.py
 mlfactory/applications/superglue_inference/models/utils.py
+mlfactory/applications/visual_odometry/__init__.py
+mlfactory/applications/visual_odometry/sfm.py
 mlfactory/custom_losses/__init__.py
 mlfactory/custom_losses/pytorch/__init__.py
 mlfactory/custom_losses/pytorch/depth.py
 mlfactory/custom_losses/pytorch/pointnetloss.py
 mlfactory/custom_losses/pytorch/regress.py
 mlfactory/custom_losses/pytorch/segment.py
 mlfactory/custom_losses/tensorflow/__init__.py
```

### Comparing `mlfactory-0.0.7/pyproject.toml` & `mlfactory-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "mlfactory"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Homagni Saha", email="homagnisaha@gmail.com" },
 ]
 description = "Collection of several machine learning modules which can be applied to diverse projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mlfactory-0.0.7/setup.py` & `mlfactory-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='mlfactory',  
-     version='0.0.7',
+     version='0.0.8',
      author="Homagni Saha",
      author_email="homagnisaha@gmail.com",
      description="Collection of several machine learning modules which can be applied to diverse projects",
      long_description=long_description,
    long_description_content_type="text/markdown",
      url="https://github.com/Homagn/mlfactory",
      packages=setuptools.find_packages(exclude=["mlfactory/applications/superglue_inference/models/weights","mlfactory/applications/segmentation_finetune/CFExp"]),
```

