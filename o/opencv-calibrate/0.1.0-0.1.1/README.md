# Comparing `tmp/opencv_calibrate-0.1.0.tar.gz` & `tmp/opencv_calibrate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_calibrate-0.1.0.tar", last modified: Sun Apr  7 10:30:02 2024, max compression
+gzip compressed data, was "opencv_calibrate-0.1.1.tar", last modified: Fri May 24 11:46:27 2024, max compression
```

## Comparing `opencv_calibrate-0.1.0.tar` & `opencv_calibrate-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-04-07 10:30:02.809647 opencv_calibrate-0.1.0/
--rw-r--r--   0 alfie      (501) staff       (20)     1068 2024-04-06 11:02:23.000000 opencv_calibrate-0.1.0/LICENSE
--rw-r--r--   0 alfie      (501) staff       (20)     3396 2024-04-07 10:30:02.809407 opencv_calibrate-0.1.0/PKG-INFO
--rw-r--r--   0 alfie      (501) staff       (20)     2653 2024-04-07 10:24:11.000000 opencv_calibrate-0.1.0/README.md
-drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-04-07 10:30:02.808159 opencv_calibrate-0.1.0/opencv_calibrate/
--rw-r--r--   0 alfie      (501) staff       (20)      184 2024-04-06 12:25:48.000000 opencv_calibrate-0.1.0/opencv_calibrate/__init__.py
--rw-r--r--   0 alfie      (501) staff       (20)     6848 2024-04-06 12:58:33.000000 opencv_calibrate-0.1.0/opencv_calibrate/calibrate.py
--rw-r--r--   0 alfie      (501) staff       (20)     3561 2024-04-06 12:58:42.000000 opencv_calibrate-0.1.0/opencv_calibrate/camera.py
--rw-r--r--   0 alfie      (501) staff       (20)       46 2024-04-06 10:30:51.000000 opencv_calibrate-0.1.0/opencv_calibrate/debug.py
--rw-r--r--   0 alfie      (501) staff       (20)     2157 2024-04-06 11:14:26.000000 opencv_calibrate-0.1.0/opencv_calibrate/io.py
--rw-r--r--   0 alfie      (501) staff       (20)      770 2024-04-06 10:31:24.000000 opencv_calibrate-0.1.0/opencv_calibrate/utils.py
-drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-04-07 10:30:02.809153 opencv_calibrate-0.1.0/opencv_calibrate.egg-info/
--rw-r--r--   0 alfie      (501) staff       (20)     3396 2024-04-07 10:30:02.000000 opencv_calibrate-0.1.0/opencv_calibrate.egg-info/PKG-INFO
--rw-r--r--   0 alfie      (501) staff       (20)      435 2024-04-07 10:30:02.000000 opencv_calibrate-0.1.0/opencv_calibrate.egg-info/SOURCES.txt
--rw-r--r--   0 alfie      (501) staff       (20)        1 2024-04-07 10:30:02.000000 opencv_calibrate-0.1.0/opencv_calibrate.egg-info/dependency_links.txt
--rw-r--r--   0 alfie      (501) staff       (20)       62 2024-04-07 10:30:02.000000 opencv_calibrate-0.1.0/opencv_calibrate.egg-info/entry_points.txt
--rw-r--r--   0 alfie      (501) staff       (20)       74 2024-04-07 10:30:02.000000 opencv_calibrate-0.1.0/opencv_calibrate.egg-info/requires.txt
--rw-r--r--   0 alfie      (501) staff       (20)       17 2024-04-07 10:30:02.000000 opencv_calibrate-0.1.0/opencv_calibrate.egg-info/top_level.txt
--rw-r--r--   0 alfie      (501) staff       (20)      863 2024-04-06 12:24:28.000000 opencv_calibrate-0.1.0/pyproject.toml
--rw-r--r--   0 alfie      (501) staff       (20)       38 2024-04-07 10:30:02.809696 opencv_calibrate-0.1.0/setup.cfg
+drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-05-24 11:46:27.608208 opencv_calibrate-0.1.1/
+-rw-r--r--   0 alfie      (501) staff       (20)     1068 2024-04-06 11:02:23.000000 opencv_calibrate-0.1.1/LICENSE
+-rw-r--r--   0 alfie      (501) staff       (20)     3475 2024-05-24 11:46:27.607963 opencv_calibrate-0.1.1/PKG-INFO
+-rw-r--r--   0 alfie      (501) staff       (20)     2732 2024-05-24 11:40:22.000000 opencv_calibrate-0.1.1/README.md
+drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-05-24 11:46:27.606609 opencv_calibrate-0.1.1/opencv_calibrate/
+-rw-r--r--   0 alfie      (501) staff       (20)      184 2024-04-06 12:25:48.000000 opencv_calibrate-0.1.1/opencv_calibrate/__init__.py
+-rw-r--r--   0 alfie      (501) staff       (20)     6971 2024-05-24 11:43:59.000000 opencv_calibrate-0.1.1/opencv_calibrate/calibrate.py
+-rw-r--r--   0 alfie      (501) staff       (20)     3561 2024-05-24 11:39:41.000000 opencv_calibrate-0.1.1/opencv_calibrate/camera.py
+-rw-r--r--   0 alfie      (501) staff       (20)       46 2024-04-06 10:30:51.000000 opencv_calibrate-0.1.1/opencv_calibrate/debug.py
+-rw-r--r--   0 alfie      (501) staff       (20)     2157 2024-04-16 14:06:50.000000 opencv_calibrate-0.1.1/opencv_calibrate/io.py
+-rw-r--r--   0 alfie      (501) staff       (20)      770 2024-04-06 10:31:24.000000 opencv_calibrate-0.1.1/opencv_calibrate/utils.py
+drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-05-24 11:46:27.607653 opencv_calibrate-0.1.1/opencv_calibrate.egg-info/
+-rw-r--r--   0 alfie      (501) staff       (20)     3475 2024-05-24 11:46:27.000000 opencv_calibrate-0.1.1/opencv_calibrate.egg-info/PKG-INFO
+-rw-r--r--   0 alfie      (501) staff       (20)      435 2024-05-24 11:46:27.000000 opencv_calibrate-0.1.1/opencv_calibrate.egg-info/SOURCES.txt
+-rw-r--r--   0 alfie      (501) staff       (20)        1 2024-05-24 11:46:27.000000 opencv_calibrate-0.1.1/opencv_calibrate.egg-info/dependency_links.txt
+-rw-r--r--   0 alfie      (501) staff       (20)       62 2024-05-24 11:46:27.000000 opencv_calibrate-0.1.1/opencv_calibrate.egg-info/entry_points.txt
+-rw-r--r--   0 alfie      (501) staff       (20)       74 2024-05-24 11:46:27.000000 opencv_calibrate-0.1.1/opencv_calibrate.egg-info/requires.txt
+-rw-r--r--   0 alfie      (501) staff       (20)       17 2024-05-24 11:46:27.000000 opencv_calibrate-0.1.1/opencv_calibrate.egg-info/top_level.txt
+-rw-r--r--   0 alfie      (501) staff       (20)      863 2024-05-24 11:46:10.000000 opencv_calibrate-0.1.1/pyproject.toml
+-rw-r--r--   0 alfie      (501) staff       (20)       38 2024-05-24 11:46:27.608255 opencv_calibrate-0.1.1/setup.cfg
```

### Comparing `opencv_calibrate-0.1.0/LICENSE` & `opencv_calibrate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_calibrate-0.1.0/PKG-INFO` & `opencv_calibrate-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv_calibrate
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple OpenCV checkerboard camera calibration python package
 Author: Alfie
 Project-URL: Homepage, https://github.com/alfieroddan/camera-calibration-opencv
 Project-URL: Bug Tracker, https://github.com/alfieroddan/camera-calibration-opencv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,17 +25,19 @@
 ![Checkerboard calibration images](assets/smaller_checkerboards.gif "Calibration")
 
 A simple tool for checkerboard camera calibration if you are tired of re-writing from the [OpenCV docs](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html) on camera calibration.
 
 # Install
 
 ```bash
-pip install opencv_calibrate 
+pip install opencv-calibrate 
 ```
 
+[pypi](https://pypi.org/project/opencv-calibrate/0.1.0/)
+
 ## Prerequisites
 
 This package relies on ffmpeg, please ensure it is installed. See [python ffmpeg](https://github.com/kkroening/ffmpeg-python) for more.
 
 # Usage
 
 ```python
@@ -98,15 +100,15 @@
   -h, --help            show this help message and exit
   --video VIDEO         Path to the video file
   --image IMAGE_DIR
                         Path to the directory containing images
   --output_dir OUTPUT_DIR
                         Path to the output directory
   --checkerboard CHECKERBOARD
-                        Number of rows and columns in comma seperated format e.g. "9, 6"
+                        Number of rows, columns and square size (mm) in comma seperated format e.g. "9, 6, 4"
 ```
 
 This will output a YAML file with the parameters:
 
 ```yaml
 camera_matrix:
 - [f_x, 0.0, c_x]
```

### Comparing `opencv_calibrate-0.1.0/README.md` & `opencv_calibrate-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 ![Checkerboard calibration images](assets/smaller_checkerboards.gif "Calibration")
 
 A simple tool for checkerboard camera calibration if you are tired of re-writing from the [OpenCV docs](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html) on camera calibration.
 
 # Install
 
 ```bash
-pip install opencv_calibrate 
+pip install opencv-calibrate 
 ```
 
+[pypi](https://pypi.org/project/opencv-calibrate/0.1.0/)
+
 ## Prerequisites
 
 This package relies on ffmpeg, please ensure it is installed. See [python ffmpeg](https://github.com/kkroening/ffmpeg-python) for more.
 
 # Usage
 
 ```python
@@ -76,15 +78,15 @@
   -h, --help            show this help message and exit
   --video VIDEO         Path to the video file
   --image IMAGE_DIR
                         Path to the directory containing images
   --output_dir OUTPUT_DIR
                         Path to the output directory
   --checkerboard CHECKERBOARD
-                        Number of rows and columns in comma seperated format e.g. "9, 6"
+                        Number of rows, columns and square size (mm) in comma seperated format e.g. "9, 6, 4"
 ```
 
 This will output a YAML file with the parameters:
 
 ```yaml
 camera_matrix:
 - [f_x, 0.0, c_x]
```

### Comparing `opencv_calibrate-0.1.0/opencv_calibrate/calibrate.py` & `opencv_calibrate-0.1.1/opencv_calibrate/calibrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 # termination criteria
 CRITERIA = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 30, 0.001)
 
 
 def calibrate_numpy(array: np.array,
                     p_r: int,
-                    p_c: int) -> tuple[bool, CameraParameters | None]:
+                    p_c: int,
+                    p_s: int) -> tuple[bool, CameraParameters | None]:
     """
     Camera calibration from numpy array,
     images can sometimes not contain checkerboard
 
     Input:
     array (np.array): (N, H, W, C(RGB)) array of images
     p_r int: number of internal points rows
@@ -39,15 +40,15 @@
     camera matrix (array)
     distortiona matrix (array)
     rotation matrix (tuple of arrays)
     translation matrix (tuple of arrays)
     """
     # prepare object points, like (0,0,0), (1,0,0), (2,0,0) ....
     objp = np.zeros((p_r*p_c, 3), np.float32)
-    objp[:, :2] = np.mgrid[0:p_r, 0:p_c].T.reshape(-1, 2)
+    objp[:, :2] = np.mgrid[0:p_r, 0:p_c].T.reshape(-1, 2) * p_s
     # Arrays to store object points and image points from all the images.
     objpoints = []  # 3d point in real world space
     imgpoints = []  # 2d points in image plane.
 
     if DEBUG > 0:
         print("Processing frames...")
 
@@ -117,21 +118,21 @@
     video_file (str): path to video_file
     checkerboard (list or tuple): number of rows and columns in checkerboard
 
     Return:
     calibrate_numpy (fn)
     """
     # points row, points columsn
-    p_r, p_c = checkerboard[0] - 1, checkerboard[1] - 1
+    p_r, p_c, p_s = checkerboard[0] - 1, checkerboard[1] - 1, checkerboard[2]
 
     # convert video to numpy
     frames = video_to_numpy(video_file)
 
     # calibrate
-    return calibrate_numpy(frames, p_r, p_c, fast=False)
+    return calibrate_numpy(frames, p_r, p_c, p_s)
 
 
 def image_calibration(image_dir: str,
                       checkerboard: tuple) -> calibrate_numpy:
     """
     Do camera calibration on key_frmaes,
     finds checkerboard frames,
@@ -141,51 +142,52 @@
     image_dir (str): path to key frames
     checkerboard (list or tuple): number of rows and columns in checkerboard
 
     Return:
     calibrate_numpy (fn)
     """
     # points row, points columns
-    p_r, p_c = checkerboard[0] - 1, checkerboard[1] - 1
+    p_r, p_c, p_s = checkerboard[0] - 1, checkerboard[1] - 1, checkerboard[2]
 
     frames = image_dir_to_numpy(image_dir)
     if len(frames) < 11 and DEBUG > 0:
         print("Low number of images, expect around 11\
                       for good calibration")
 
-    return calibrate_numpy(frames, p_r, p_c)
+    return calibrate_numpy(frames, p_r, p_c, p_s)
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(description='Camera calibration of videos\
                                      and images containing checkerboard\
                                      run with DEBUG>1 for more outputs')
 
     parser.add_argument('--video', type=str,
                         help='Path to the video file')
     parser.add_argument('--image', type=str,
                         help='Path to the directory containing images')
     parser.add_argument('--output_dir', type=str, default=".",
                         required=False, help='Path to the output directory')
     parser.add_argument('--checkerboard', default="9, 6",
-                        help='Number of rows and columns \
-                            in comma seperated format e.g. "9, 6"', type=str)
+                        help='Number of rows, columns and square size (mm) \
+                            in comma seperated format e.g. "9, 6, 4"',
+                        type=str)
 
     args = parser.parse_args()
 
     # Validate arguments
     if not args.video and not args.image:
         parser.error('Either --video or --image_dir must be provided')
 
     if not os.path.exists(args.output_dir):
         raise Exception("Output directory does not exist")
 
     # conver checkerboard to list
     args.checkerboard = [int(item) for item in args.checkerboard.split(',')]
-    assert len(args.checkerboard) == 2, "Checkerboard row and column must be 2"
+    assert len(args.checkerboard) == 3, "Checkerboard row and column must be 3"
 
     if DEBUG > 0:
         print(f"Checkerboard size: {args.checkerboard}")
 
     if args.video:
         assert os.path.isfile(args.video), "Video file does not exist"
         if DEBUG > 0:
```

### Comparing `opencv_calibrate-0.1.0/opencv_calibrate/camera.py` & `opencv_calibrate-0.1.1/opencv_calibrate/camera.py`

 * *Files identical despite different names*

### Comparing `opencv_calibrate-0.1.0/opencv_calibrate/io.py` & `opencv_calibrate-0.1.1/opencv_calibrate/io.py`

 * *Files identical despite different names*

### Comparing `opencv_calibrate-0.1.0/opencv_calibrate/utils.py` & `opencv_calibrate-0.1.1/opencv_calibrate/utils.py`

 * *Files identical despite different names*

### Comparing `opencv_calibrate-0.1.0/opencv_calibrate.egg-info/PKG-INFO` & `opencv_calibrate-0.1.1/opencv_calibrate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv_calibrate
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple OpenCV checkerboard camera calibration python package
 Author: Alfie
 Project-URL: Homepage, https://github.com/alfieroddan/camera-calibration-opencv
 Project-URL: Bug Tracker, https://github.com/alfieroddan/camera-calibration-opencv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,17 +25,19 @@
 ![Checkerboard calibration images](assets/smaller_checkerboards.gif "Calibration")
 
 A simple tool for checkerboard camera calibration if you are tired of re-writing from the [OpenCV docs](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html) on camera calibration.
 
 # Install
 
 ```bash
-pip install opencv_calibrate 
+pip install opencv-calibrate 
 ```
 
+[pypi](https://pypi.org/project/opencv-calibrate/0.1.0/)
+
 ## Prerequisites
 
 This package relies on ffmpeg, please ensure it is installed. See [python ffmpeg](https://github.com/kkroening/ffmpeg-python) for more.
 
 # Usage
 
 ```python
@@ -98,15 +100,15 @@
   -h, --help            show this help message and exit
   --video VIDEO         Path to the video file
   --image IMAGE_DIR
                         Path to the directory containing images
   --output_dir OUTPUT_DIR
                         Path to the output directory
   --checkerboard CHECKERBOARD
-                        Number of rows and columns in comma seperated format e.g. "9, 6"
+                        Number of rows, columns and square size (mm) in comma seperated format e.g. "9, 6, 4"
 ```
 
 This will output a YAML file with the parameters:
 
 ```yaml
 camera_matrix:
 - [f_x, 0.0, c_x]
```

### Comparing `opencv_calibrate-0.1.0/pyproject.toml` & `opencv_calibrate-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opencv_calibrate"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Alfie"},
 ]
 description = "A simple OpenCV checkerboard camera calibration python package"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

