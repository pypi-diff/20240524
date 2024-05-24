# Comparing `tmp/Moore_SDK-1.0.12-py3-none-any.whl.zip` & `tmp/Moore_SDK-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 52732 bytes, number of entries: 56
+Zip file size: 52746 bytes, number of entries: 56
 -rw-rw-rw-  2.0 fat     6677 b- defN 24-May-13 09:04 moore/__init__.py
 -rw-rw-rw-  2.0 fat       76 b- defN 24-May-13 08:56 moore/_version.py
 -rw-rw-rw-  2.0 fat      837 b- defN 24-May-13 09:02 moore/api.py
 -rw-rw-rw-  2.0 fat       84 b- defN 24-May-13 09:04 moore/const.py
 -rw-rw-rw-  2.0 fat     1014 b- defN 24-May-13 09:02 moore/exception.py
 -rw-rw-rw-  2.0 fat     1851 b- defN 24-May-13 09:04 moore/moore_data.py
 -rw-rw-rw-  2.0 fat       23 b- defN 24-Jan-02 08:40 moore/check/__init__.py
@@ -33,26 +33,26 @@
 -rw-rw-rw-  2.0 fat     1629 b- defN 24-May-13 09:04 moore/post_process/process.py
 -rw-rw-rw-  2.0 fat       52 b- defN 24-Mar-12 09:24 moore/post_process/coco/__init__.py
 -rw-rw-rw-  2.0 fat     4743 b- defN 24-May-13 09:04 moore/post_process/coco/coco_postprocess.py
 -rw-rw-rw-  2.0 fat     3648 b- defN 24-Mar-26 10:24 moore/post_process/coco/test.py
 -rw-rw-rw-  2.0 fat       72 b- defN 24-Jan-02 08:40 moore/utils/__init__.py
 -rw-rw-rw-  2.0 fat    23727 b- defN 24-Jan-10 15:16 moore/utils/cv_tools.py
 -rw-rw-rw-  2.0 fat     6088 b- defN 24-May-13 09:02 moore/utils/general.py
--rw-rw-rw-  2.0 fat    19245 b- defN 24-May-24 03:18 moore/utils/pc_tools.py
+-rw-rw-rw-  2.0 fat    19192 b- defN 24-May-15 11:34 moore/utils/pc_tools.py
 -rw-rw-rw-  2.0 fat       21 b- defN 24-Jan-02 08:40 moore/visualize/__init__.py
 -rw-rw-rw-  2.0 fat     4649 b- defN 24-Jan-02 08:40 moore/visualize/visual.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/coco/__init__.py
 -rw-rw-rw-  2.0 fat     1864 b- defN 24-May-13 09:04 moore/visualize/coco/visual_coco.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/labelme/__init__.py
 -rw-rw-rw-  2.0 fat     2343 b- defN 24-May-13 09:04 moore/visualize/labelme/visual_labelme.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/source/__init__.py
 -rw-rw-rw-  2.0 fat     2691 b- defN 24-May-13 09:04 moore/visualize/source/visual_source.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/voc/__init__.py
 -rw-rw-rw-  2.0 fat     3035 b- defN 24-Jan-02 08:40 moore/visualize/voc/visual_voc.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/yolo/__init__.py
 -rw-rw-rw-  2.0 fat     2213 b- defN 24-Jan-02 08:40 moore/visualize/yolo/visual_yolo.py
--rw-rw-rw-  2.0 fat     1079 b- defN 24-May-24 03:20 Moore_SDK-1.0.12.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2044 b- defN 24-May-24 03:20 Moore_SDK-1.0.12.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 03:20 Moore_SDK-1.0.12.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-24 03:20 Moore_SDK-1.0.12.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4830 b- defN 24-May-24 03:20 Moore_SDK-1.0.12.dist-info/RECORD
-56 files, 159141 bytes uncompressed, 44978 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     1079 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2096 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     4825 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/RECORD
+56 files, 159135 bytes uncompressed, 45002 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -147,23 +147,23 @@
 
 Filename: moore/visualize/yolo/__init__.py
 Comment: 
 
 Filename: moore/visualize/yolo/visual_yolo.py
 Comment: 
 
-Filename: Moore_SDK-1.0.12.dist-info/LICENSE
+Filename: Moore_SDK-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: Moore_SDK-1.0.12.dist-info/METADATA
+Filename: Moore_SDK-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: Moore_SDK-1.0.12.dist-info/WHEEL
+Filename: Moore_SDK-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: Moore_SDK-1.0.12.dist-info/top_level.txt
+Filename: Moore_SDK-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: Moore_SDK-1.0.12.dist-info/RECORD
+Filename: Moore_SDK-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moore/utils/pc_tools.py

```diff
@@ -269,28 +269,28 @@
         mask = np.all((box_pcd_np >= -0.5 * box_size) & (box_pcd_np <= 0.5 * box_size), axis=1)
         xyz_point = xyz_point[~mask]
         intensity_point = intensity_point[~mask]
     filtered_point = np.concatenate([xyz_point, intensity_point.reshape(-1, 1)], axis=1)
     return filtered_point
 
 
-def voxel_subsample(pcd_path, voxel_size, intensity=None, iten_idx=3, output_path='./subsampled.pcd'):
+def voxel_subsample(pcd_path, voxel_size, intensity=None, output_path='./subsampled.pcd'):
     """
     Retain points within the intensity information threshold and downsample the remaining points based on voxels
     :param pcd_path: pcd format point cloud path
     :param intensity: intensity range (list) example: [20, 200]
     :param voxel_size: voxel size
     :param output_path: Point cloud file save path
     :return:
     """
-    pc_points, headers = read_pcd(pcd_path)
+    pc_points, headers = read_pcd(pcd_path)[:, :4]
     # We default the first four columns of the point cloud to x, y, z, intensity
     if intensity:
-        points_intensity = pc_points[(pc_points[:, iten_idx] >= intensity[0]) & (pc_points[:, iten_idx] <= intensity[1])]
-        points_other = pc_points[(pc_points[:, iten_idx] < intensity[0]) | (pc_points[:, iten_idx] > intensity[1])]
+        points_intensity = pc_points[(pc_points[:, 3] >= intensity[0]) & (pc_points[:, 3] <= intensity[1])]
+        points_other = pc_points[(pc_points[:, 3] < intensity[0]) | (pc_points[:, 3] > intensity[1])]
         voxel_coords = np.floor(points_other[:, 0:3] / voxel_size).astype(np.int32)
         voxel_indices = np.unique(voxel_coords, axis=0, return_index=True)[1]
         downsampled_points_other = points_other[voxel_indices]
         final_points = np.concatenate((points_intensity, downsampled_points_other), axis=0)
     else:
         voxel_coords = np.floor(pc_points[:, 0:3] / voxel_size).astype(np.int32)
         voxel_indices = np.unique(voxel_coords, axis=0, return_index=True)[1]
@@ -298,15 +298,15 @@
 
     head = {
         "FIELDS": headers['FIELDS'],
         "SIZE": headers['SIZE'],
         "TYPE": headers['TYPE'],
         "COUNT": headers['COUNT']
     }
-    write_pcd(final_points, output_path, head, data_mode='binary')
+    write_pcd(final_points, output_path, head)
 
 
 def random_subsample(pcd_path, sampling_ratio, intensity, output_path='./subsampled.pcd'):
     """
     Retain points within the intensity information threshold and randomly downsample the remaining points
     :param pcd_path: pcd format point cloud path
     :param intensity: intensity range (list) example: [20, 200]
```

## Comparing `Moore_SDK-1.0.12.dist-info/LICENSE` & `Moore_SDK-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Moore_SDK-1.0.12.dist-info/RECORD` & `Moore_SDK-1.0.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -32,25 +32,25 @@
 moore/post_process/process.py,sha256=Owgso5AQ5LJ_u36_ekqcp3PxHY4-4SN1AlsIbU4jmPs,1629
 moore/post_process/coco/__init__.py,sha256=TX_hVWaL7ZlEJDTSdLgKGojm5eLfDXtqlwnK08ShfxU,52
 moore/post_process/coco/coco_postprocess.py,sha256=58zM6wlAGnZBj1CVwHyjtMCMQpfxz1A6UAOZh66-nbo,4743
 moore/post_process/coco/test.py,sha256=O4UVeQUQYJU1uvKVGGh2xzHrgUxZmZG6l63DksN1EwE,3648
 moore/utils/__init__.py,sha256=29mYzkYNGSWT6J-GNrinnui1ZOh0ch8Q4mFIfsEq-V4,72
 moore/utils/cv_tools.py,sha256=iMqCwdEjj4MvaWcB4irlNqTFRt_qR8RfvKp82TFYvV8,23727
 moore/utils/general.py,sha256=iri2YFeSig6uXpan2achHarj_iTpTCycTmkJaNg1GHo,6088
-moore/utils/pc_tools.py,sha256=MbvpwClO2bOYMD-QcvBcrIEgoMc140jrFo_J1i4sG9Y,19245
+moore/utils/pc_tools.py,sha256=wwt3UBtoZawFv_OJX5Q14nOxi36l1ARUcbh9_dKYzxs,19192
 moore/visualize/__init__.py,sha256=Z0muVjdGwM_2xMkm3bE_P-qEN0awBcb9tXk9AyGJGnU,21
 moore/visualize/visual.py,sha256=SVO4h15MHOihJjiiOO1JrvfG22wO9ftfz9gMbJfW_vs,4649
 moore/visualize/coco/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/coco/visual_coco.py,sha256=k7Kdxa3BTN5l-dnw0yYHrLAPQw-5gReaoBBrQH-Bpk0,1864
 moore/visualize/labelme/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/labelme/visual_labelme.py,sha256=IRGZHT9VpOlUVvJvNGYFeK0curME5dIuQoVJUMYSw9U,2343
 moore/visualize/source/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/source/visual_source.py,sha256=pGyYpBslAhUlWuT-J4vWX5vNzqG8x6sVfJIrt-e_-m0,2691
 moore/visualize/voc/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/voc/visual_voc.py,sha256=Hsp92kk--tSrVIcTDIR7VV-mEDvn8tyG_FMjEWBVg9k,3035
 moore/visualize/yolo/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/yolo/visual_yolo.py,sha256=nkrSOnQc0elJCDZUo2gJy_dVg6_6UxzkntQCoL3y9Ts,2213
-Moore_SDK-1.0.12.dist-info/LICENSE,sha256=Jwv3fsn5Tp_DrJRAfUpZCprWtVOZWtWa7IQ2WMuJMZs,1079
-Moore_SDK-1.0.12.dist-info/METADATA,sha256=PO2Yp9Es2_Ah_c3ZCjMLWGQJ0py82_XWYBE1-ZfjkbE,2044
-Moore_SDK-1.0.12.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Moore_SDK-1.0.12.dist-info/top_level.txt,sha256=rLvje0QJ2e4hrGqaQ5xvQb0xC0rH4shSHmk49v3GMDs,6
-Moore_SDK-1.0.12.dist-info/RECORD,,
+Moore_SDK-1.0.9.dist-info/LICENSE,sha256=Jwv3fsn5Tp_DrJRAfUpZCprWtVOZWtWa7IQ2WMuJMZs,1079
+Moore_SDK-1.0.9.dist-info/METADATA,sha256=dbnq4ehlIR34JWa95pjM-AzxU8yi6oGaucQPcKiBgFg,2096
+Moore_SDK-1.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+Moore_SDK-1.0.9.dist-info/top_level.txt,sha256=rLvje0QJ2e4hrGqaQ5xvQb0xC0rH4shSHmk49v3GMDs,6
+Moore_SDK-1.0.9.dist-info/RECORD,,
```

