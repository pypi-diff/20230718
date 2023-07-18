# Comparing `tmp/freepaths-1.4.1.tar.gz` & `tmp/freepaths-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freepaths-1.4.1.tar", last modified: Tue Jun  6 02:30:55 2023, max compression
+gzip compressed data, was "freepaths-1.6.tar", last modified: Tue Jul 18 06:54:19 2023, max compression
```

## Comparing `freepaths-1.4.1.tar` & `freepaths-1.6.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-06-06 02:30:55.244647 freepaths-1.4.1/
--rw-r--r--   0 r         (1000) r         (1000)     5300 2023-06-06 02:30:55.244647 freepaths-1.4.1/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     4542 2023-02-22 13:18:35.000000 freepaths-1.4.1/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-06-06 02:30:55.241314 freepaths-1.4.1/freepaths/
--rw-r--r--   0 r         (1000) r         (1000)      871 2023-06-06 02:30:40.000000 freepaths-1.4.1/freepaths/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     3677 2023-05-11 08:30:00.000000 freepaths-1.4.1/freepaths/animation.py
--rw-r--r--   0 r         (1000) r         (1000)    10197 2023-05-25 05:32:25.000000 freepaths-1.4.1/freepaths/config.py
--rw-r--r--   0 r         (1000) r         (1000)     8371 2023-05-25 08:12:01.000000 freepaths-1.4.1/freepaths/data.py
--rw-r--r--   0 r         (1000) r         (1000)     3122 2023-05-25 06:39:51.000000 freepaths-1.4.1/freepaths/default_config.py
--rw-r--r--   0 r         (1000) r         (1000)     2721 2023-05-25 08:50:50.000000 freepaths-1.4.1/freepaths/flight.py
--rw-r--r--   0 r         (1000) r         (1000)     4366 2023-02-03 02:30:26.000000 freepaths-1.4.1/freepaths/main_mfp_sampling.py
--rw-r--r--   0 r         (1000) r         (1000)     3330 2023-05-11 07:20:52.000000 freepaths-1.4.1/freepaths/main_tracing.py
--rw-r--r--   0 r         (1000) r         (1000)     8647 2023-01-25 08:49:48.000000 freepaths-1.4.1/freepaths/maps.py
--rw-r--r--   0 r         (1000) r         (1000)     3797 2023-01-25 08:49:48.000000 freepaths-1.4.1/freepaths/materials.py
--rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.4.1/freepaths/move.py
--rw-r--r--   0 r         (1000) r         (1000)      479 2023-05-25 02:30:36.000000 freepaths-1.4.1/freepaths/options.py
--rw-r--r--   0 r         (1000) r         (1000)     4837 2023-01-25 08:49:48.000000 freepaths-1.4.1/freepaths/output_info.py
--rw-r--r--   0 r         (1000) r         (1000)    16123 2023-05-25 08:52:51.000000 freepaths-1.4.1/freepaths/output_plots.py
--rw-r--r--   0 r         (1000) r         (1000)     2348 2023-02-03 08:43:58.000000 freepaths-1.4.1/freepaths/output_structure.py
--rw-r--r--   0 r         (1000) r         (1000)     8034 2023-05-25 02:30:40.000000 freepaths-1.4.1/freepaths/phonon.py
--rw-r--r--   0 r         (1000) r         (1000)      580 2023-01-24 09:16:58.000000 freepaths-1.4.1/freepaths/progress.py
--rw-r--r--   0 r         (1000) r         (1000)     2312 2023-05-25 02:30:38.000000 freepaths-1.4.1/freepaths/run_phonon.py
--rw-r--r--   0 r         (1000) r         (1000)    28765 2023-05-25 05:20:49.000000 freepaths-1.4.1/freepaths/scattering.py
--rw-r--r--   0 r         (1000) r         (1000)     1550 2023-01-25 08:51:17.000000 freepaths-1.4.1/freepaths/scattering_types.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-06-06 02:30:55.244647 freepaths-1.4.1/freepaths.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     5300 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      702 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       53 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       31 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)       10 2023-06-06 02:30:55.000000 freepaths-1.4.1/freepaths.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.4.1/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-06-06 02:30:55.244647 freepaths-1.4.1/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-03 05:40:49.000000 freepaths-1.4.1/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-07-18 06:54:19.805313 freepaths-1.6/
+-rw-r--r--   0 r         (1000) r         (1000)     5298 2023-07-18 06:54:19.805313 freepaths-1.6/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     4542 2023-02-22 13:18:35.000000 freepaths-1.6/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-07-18 06:54:19.805313 freepaths-1.6/freepaths/
+-rw-r--r--   0 r         (1000) r         (1000)      876 2023-07-18 06:11:07.000000 freepaths-1.6/freepaths/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     3730 2023-07-18 05:51:58.000000 freepaths-1.6/freepaths/animation.py
+-rw-r--r--   0 r         (1000) r         (1000)     9528 2023-07-18 05:52:01.000000 freepaths-1.6/freepaths/config.py
+-rw-r--r--   0 r         (1000) r         (1000)     8118 2023-07-18 05:33:50.000000 freepaths-1.6/freepaths/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     2550 2023-07-18 05:34:15.000000 freepaths-1.6/freepaths/default_config.py
+-rw-r--r--   0 r         (1000) r         (1000)     2563 2023-07-18 05:34:49.000000 freepaths-1.6/freepaths/flight.py
+-rw-r--r--   0 r         (1000) r         (1000)     4366 2023-02-03 02:30:26.000000 freepaths-1.6/freepaths/main_mfp_sampling.py
+-rw-r--r--   0 r         (1000) r         (1000)     3374 2023-07-18 06:22:06.000000 freepaths-1.6/freepaths/main_tracing.py
+-rw-r--r--   0 r         (1000) r         (1000)    10945 2023-07-18 06:21:48.000000 freepaths-1.6/freepaths/maps.py
+-rw-r--r--   0 r         (1000) r         (1000)     3822 2023-06-16 05:34:54.000000 freepaths-1.6/freepaths/materials.py
+-rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.6/freepaths/move.py
+-rw-r--r--   0 r         (1000) r         (1000)      479 2023-07-07 01:48:51.000000 freepaths-1.6/freepaths/options.py
+-rw-r--r--   0 r         (1000) r         (1000)     4805 2023-06-16 05:39:39.000000 freepaths-1.6/freepaths/output_info.py
+-rw-r--r--   0 r         (1000) r         (1000)    20210 2023-07-18 06:22:06.000000 freepaths-1.6/freepaths/output_plots.py
+-rw-r--r--   0 r         (1000) r         (1000)     4334 2023-07-18 05:52:02.000000 freepaths-1.6/freepaths/output_structure.py
+-rw-r--r--   0 r         (1000) r         (1000)     6642 2023-07-13 09:00:28.000000 freepaths-1.6/freepaths/phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)      580 2023-06-16 05:18:51.000000 freepaths-1.6/freepaths/progress.py
+-rw-r--r--   0 r         (1000) r         (1000)     2455 2023-07-18 05:35:03.000000 freepaths-1.6/freepaths/run_phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)     2263 2023-06-16 05:15:40.000000 freepaths-1.6/freepaths/scatterers.py
+-rw-r--r--   0 r         (1000) r         (1000)    46299 2023-07-18 06:14:19.000000 freepaths-1.6/freepaths/scattering.py
+-rw-r--r--   0 r         (1000) r         (1000)     3223 2023-06-16 05:19:57.000000 freepaths-1.6/freepaths/scattering_parabolic.py
+-rw-r--r--   0 r         (1000) r         (1000)     9181 2023-06-16 05:23:51.000000 freepaths-1.6/freepaths/scattering_primitives.py
+-rw-r--r--   0 r         (1000) r         (1000)    31827 2023-07-18 06:19:04.000000 freepaths-1.6/freepaths/scattering_semicircle.py
+-rw-r--r--   0 r         (1000) r         (1000)     1651 2023-06-16 05:18:43.000000 freepaths-1.6/freepaths/scattering_types.py
+-rw-r--r--   0 r         (1000) r         (1000)     2257 2023-07-07 04:08:38.000000 freepaths-1.6/freepaths/sources.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-07-18 06:54:19.805313 freepaths-1.6/freepaths.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     5298 2023-07-18 06:54:19.000000 freepaths-1.6/freepaths.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      851 2023-07-18 06:54:19.000000 freepaths-1.6/freepaths.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-07-18 06:54:19.000000 freepaths-1.6/freepaths.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       53 2023-07-18 06:54:19.000000 freepaths-1.6/freepaths.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       31 2023-07-18 06:54:19.000000 freepaths-1.6/freepaths.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)       10 2023-07-18 06:54:19.000000 freepaths-1.6/freepaths.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.6/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-07-18 06:54:19.805313 freepaths-1.6/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-03 05:40:49.000000 freepaths-1.6/setup.py
```

### Comparing `freepaths-1.4.1/PKG-INFO` & `freepaths-1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.4.1
+Version: 1.6
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.4.1/README.md` & `freepaths-1.6/README.md`

 * *Files identical despite different names*

### Comparing `freepaths-1.4.1/freepaths/__main__.py` & `freepaths-1.6/freepaths/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """FreePATHS - Free Phonon and THermal Simulator"""
 
 import argparse
 
 import freepaths.main_tracing
 import freepaths.main_mfp_sampling
 
-__version__ = "1.4.1"
+__version__ = "1.6"
 
 # Parse user arguments:
 parser = argparse.ArgumentParser(
                 prog = 'FreePATHS',
-                description = 'Monte Carlo simulator',
+                description = 'Phonon Monte Carlo simulator',
                 epilog = 'For more information, visit: https://anufrievroman.gitbook.io/freepaths'
                 )
 parser.add_argument('input_file', nargs='?', default=None, help='The input file')
 parser.add_argument("-s", "--sampling", help="Run in MFP sampling mode", action="store_true")
 args = parser.parse_args()
```

### Comparing `freepaths-1.4.1/freepaths/animation.py` & `freepaths-1.6/freepaths/animation.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     number_of_steps = np.shape(data)[0]
     number_of_phonons = np.shape(data)[1]//3
 
     for step in range(1, number_of_steps):
         fig, ax = plt.subplots()
 
         # Draw the structure:
-        patches = draw_structure(cf)
+        patches = draw_structure(cf, color_back=cf.output_structure_color)
+
         for patch in patches:
             ax.add_patch(patch)
 
         # Draw the paths:
         for phonon_num in range(number_of_phonons):
             x_coords = np.trim_zeros(data[:, 3 * phonon_num], trim='b')
             y_coords = np.trim_zeros(data[:, 3 * phonon_num + 1], trim='b')
@@ -79,15 +80,15 @@
     images = []
     filenames = os.listdir("Frames/")
     for filename in filenames:
         images.append(imageio.imread(f"Frames/{filename}"))
 
     # Create a GIF file:
     imageio.mimsave("Animated paths XY.gif", images,
-                    fps=cf.output_animation_fps, subrectangles=True)
+                    duration=1000 * 1/cf.output_animation_fps, subrectangles=True)
 
     # Create an MP4 file:
     # writer = imageio.get_writer('Animated paths XY.mp4', fps=cf.output_animation_fps)
 
     # for im in images:
         # writer.append_data(imageio.imread(im))
     # writer.close()
```

### Comparing `freepaths-1.4.1/freepaths/config.py` & `freepaths-1.6/freepaths/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module that reads the user input file, provides default values, and converts the variables into enums"""
 
 import sys
 import argparse
 
 from freepaths.options import Materials, Distributions
+from freepaths.scatterers import *
 
 # Import a default input file:
 from freepaths.default_config import *
 
 
 # Parse user arguments:
 WEBSITE = 'https://anufrievroman.gitbook.io/freepaths'
@@ -40,15 +41,14 @@
         self.temp = T
         self.plots_in_terminal = PLOTS_IN_TERMINAL
         self.output_scattering_map = OUTPUT_SCATTERING_MAP
         self.output_raw_thermal_map = OUTPUT_RAW_THERMAL_MAP
         self.output_trajectories_of_first = OUTPUT_TRAJECTORIES_OF_FIRST
         self.output_structure_color = OUTPUT_STRUCTURE_COLOR
         self.number_of_length_segments = NUMBER_OF_LENGTH_SEGMENTS
-        self.phonon_source_angle_distribution = PHONON_SOURCE_ANGLE_DISTRIBUTION
 
         # Animation:
         self.output_path_animation = OUTPUT_PATH_ANIMATION
         self.output_animation_fps = OUTPUT_ANIMATION_FPS
 
         # Map & profiles parameters:
         self.number_of_pixels_x = NUMBER_OF_PIXELS_X
@@ -75,19 +75,15 @@
 
         # Hot side positions:
         self.hot_side_position_top = HOT_SIDE_POSITION_TOP
         self.hot_side_position_bottom = HOT_SIDE_POSITION_BOTTOM
         self.hot_side_position_right = HOT_SIDE_POSITION_RIGHT
         self.hot_side_position_left = HOT_SIDE_POSITION_LEFT
 
-        self.frequency_detector_size = FREQUENCY_DETECTOR_SIZE
-        self.phonon_source_x = PHONON_SOURCE_X
-        self.phonon_source_y = PHONON_SOURCE_Y
-        self.phonon_source_width_x = PHONON_SOURCE_WIDTH_X
-        self.phonon_source_width_y = PHONON_SOURCE_WIDTH_Y
+        self.phonon_sources = PHONON_SOURCES
 
         # Cold side positions:
         self.cold_side_position_top = COLD_SIDE_POSITION_TOP
         self.cold_side_position_bottom = COLD_SIDE_POSITION_BOTTOM
         self.cold_side_position_right = COLD_SIDE_POSITION_RIGHT
         self.cold_side_position_left = COLD_SIDE_POSITION_LEFT
 
@@ -104,44 +100,30 @@
         self.top_parabola_tip = TOP_PARABOLA_TIP
         self.top_parabola_focus = TOP_PARABOLA_FOCUS
         self.include_bottom_parabola = INCLUDE_BOTTOM_PARABOLA
         self.bottom_parabola_tip = BOTTOM_PARABOLA_TIP
         self.bottom_parabola_focus = BOTTOM_PARABOLA_FOCUS
 
         # Hole array parameters:
-        self.include_holes = INCLUDE_HOLES
-        self.circular_hole_diameter = CIRCULAR_HOLE_DIAMETER
-        self.rectangular_hole_side_x = RECTANGULAR_HOLE_SIDE_X
-        self.rectangular_hole_side_y = RECTANGULAR_HOLE_SIDE_Y
-        self.period_x = PERIOD_X
-        self.period_y = PERIOD_Y
-
-        # Lattice of holes:
-        self.hole_coordinates = HOLE_COORDINATES
-        self.hole_shapes = HOLE_SHAPES
-
-        # Pillar array parameters [m]
-        self.include_pillars = INCLUDE_PILLARS
-        self.pillar_coordinates = PILLAR_COORDINATES
-        self.pillar_height = PILLAR_HEIGHT
-        self.pillar_wall_angle = PILLAR_WALL_ANGLE
-
+        self.holes = HOLES
+        self.pillars = PILLARS
 
     def convert_to_enums(self):
         """Convert some user generated parameters into enums"""
 
         # Distributions:
         valid_distributions =[member.name.lower() for member in Distributions]
-        if self.phonon_source_angle_distribution in valid_distributions:
-            self.phonon_source_angle_distribution = Distributions[self.phonon_source_angle_distribution.upper()]
-        else:
-            print("ERROR: Parameter phonon_source_ANGLE_DISTRIBUTION is not set correctly.")
-            print("phonon_source_ANGLE_DISTRIBUTION should be one of the following:")
-            print(*valid_distributions, sep = ", ")
-            sys.exit()
+        for source in self.phonon_sources:
+            if source.angle_distribution in valid_distributions:
+                source.angle_distribution = Distributions[source.angle_distribution.upper()]
+            else:
+                print("ERROR: Parameter angle_distribution of a source is not set correctly.")
+                print("The angle_distribution should be one of the following:")
+                print(*valid_distributions, sep = ", ")
+                sys.exit()
 
         # Materials:
         valid_materials = [member.name for member in Materials]
         if self.media in valid_materials:
             self.media = Materials[self.media]
         else:
             print(f"ERROR: Material {self.media} is not in the database.")
@@ -152,33 +134,42 @@
 
     def check_parameter_validity(self):
         """Check if various parameters are valid"""
         if self.number_of_phonons < self.output_trajectories_of_first:
             self.output_trajectories_of_first = self.number_of_phonons
             print("WARNING: Parameter OUTPUT_TRAJECTORIES_OF_FIRST exceeded NUMBER_OF_PHONONS.\n")
 
-        if self.phonon_source_y > self.length:
-            self.phonon_source_y = self.length
-            print("WARNING: Parameter phonon_source_Y exceeded LENGHT.\n")
-
-        if self.phonon_source_y < 0:
-            self.phonon_source_y = 0
-            print("WARNING: Parameter PHONON_SOURCE_Y was negative.\n")
-
-        if self.phonon_source_y - self.phonon_source_width_y / 2 < 0:
-            self.phonon_source_width_y = self.phonon_source_y * 2
-            print("WARNING: Parameter PHONON_SOURCE_WIDTH_Y was too large.\n")
-
-        if self.phonon_source_x > self.width/2:
-            self.phonon_source_x = 0
-            print("WARNING: Parameter PHONON_SOURCE_X was larger than WIDTH.\n")
-
-        if self.phonon_source_width_x > self.width:
-            self.phonon_source_width_x = self.width
-            print("WARNING: Parameter PHONON_SOURCE_WIDTH_X exceeds WIDTH.\n")
+        for source in self.phonon_sources:
+            if source.y > self.length:
+                print("ERROR: Y coordinate of a source exceeded LENGHT.\n")
+                sys.exit()
+
+            if source.y < 0:
+                print("ERROR: Y coordinate of a source is negative.\n")
+                sys.exit()
+
+            if source.y - source.size_y / 2 < 0:
+                print("ERROR: Source size along Y coordinate is too large.\n")
+                sys.exit()
+
+            if abs(source.x) > self.width/2:
+                print("ERROR: X coordinate of a source exceeds WIDTH.\n")
+                sys.exit()
+
+            if abs(source.x + source.size_x / 2) > self.width/2:
+                print("ERROR: Source size along X coordinate is too large.\n")
+                sys.exit()
+
+            if abs(source.z) > self.thickness/2:
+                print("ERROR: Z coordinate of a source exceeds THICKNESS.\n")
+                sys.exit()
+
+            if abs(source.z + source.size_z / 2) > self.thickness/2:
+                print("ERROR: Source size along Z coordinate is too large.\n")
+                sys.exit()
 
         if self.output_path_animation and self.number_of_timesteps > 5000:
             print("WARNING: NUMBER_OF_TIMESTEPS is rather large for animation.\n")
 
         if (self.cold_side_position_top and self.include_top_sidewall or
             self.hot_side_position_top and self.include_top_sidewall or
             self.cold_side_position_top and self.hot_side_position_top):
@@ -204,33 +195,33 @@
             sys.exit()
 
 
     def check_depricated_parameters(self):
         """Check for depricated parameters and warn about them"""
 
         if 'COLD_SIDE_POSITION' in globals():
-            print("WARNING: parameter COLD_SIDE_POSITION is depricated. ")
+            print("ERROR: parameter COLD_SIDE_POSITION is depricated. ")
             print("Use specific boolean parameters like COLD_SIDE_POSITION_TOP = True.\n")
+            sys.exit()
 
-        if 'HOT_SIDE_POSITION' in globals():
-            print("WARNING: parameter HOT_SIDE_POSITION is depricated. ")
-            print("Use specific boolean parameters like HOT_SIDE_POSITION_BOTTOM = True.\n")
-
-        if 'HOT_SIDE_X' in globals():
-            print("WARNING: parameter HOT_SIDE_X was renamed to PHONON_SOURCE_X.\n")
-
-        if 'HOT_SIDE_Y' in globals():
-            print("WARNING: parameter HOT_SIDE_Y was renamed to PHONON_SOURCE_Y.\n")
-
-        if 'HOT_SIDE_WIDTH_X' in globals():
-            print("WARNING: parameter HOT_SIDE_WIDTH_X was renamed to PHONON_SOURCE_WIDTH_X.\n")
-
-        if 'HOT_SIDE_WIDTH_Y' in globals():
-            print("WARNING: parameter HOT_SIDE_WIDTH_Y was renamed to PHONON_SOURCE_WIDTH_Y.\n")
-
-        if 'HOT_SIDE_ANGLE_DISTRIBUTION' in globals():
-            print("WARNING: parameter HOT_SIDE_ANGLE_DISTRIBUTION was renamed to PHONON_SOURCE_ANGLE_DISTRIBUTION.\n")
+        if any([
+            'HOT_SIDE_POSITION' in globals(),
+            'HOT_SIDE_X' in globals(),
+            'HOT_SIDE_Y' in globals(),
+            'HOT_SIDE_WIDTH_X' in globals(),
+            'HOT_SIDE_WIDTH_Y' in globals(),
+            'HOT_SIDE_ANGLE_DISTRIBUTION' in globals(),
+            'PHONON_SOURCE_X' in globals(),
+            'PHONON_SOURCE_Y' in globals(),
+            'PHONON_SOURCE_WIDTH_X' in globals(),
+            'PHONON_SOURCE_WIDTH_Y' in globals(),
+            'PHONON_SOURCE_ANGLE_DISTRIBUTION' in globals(),
+            ]):
+            print("ERROR: parameters related to HOT_SIDE_... or PHONON_SOURCE_.. are depricated. ")
+            print("Phonon source should be defined through the PHONON_SOURCES variable.\n")
+            print("See updated documentation for more details.\n")
+            sys.exit()
 
 cf = Config()
 cf.convert_to_enums()
 cf.check_parameter_validity()
 cf.check_depricated_parameters()
```

### Comparing `freepaths-1.4.1/freepaths/data.py` & `freepaths-1.6/freepaths/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     def __init__(self):
         """Initialize arrays for writing various properties"""
         self.initial_angles = []
         self.exit_angles = []
         self.free_paths = []
         self.free_paths_along_y = []
         self.frequencies = []
-        self.detected_frequencies = []
         self.group_velocities = []
         self.travel_times = []
         self.mean_free_paths = []
 
     def save_phonon_data(self, ph):
         """Add information about the phonon to the dataset"""
         self.frequencies.append(ph.f)
@@ -56,23 +55,21 @@
     def save_flight_data(self, flight):
         """Add information about the phonon flight to the dataset"""
         self.initial_angles.append(flight.initial_theta)
         self.exit_angles.append(flight.exit_theta)
         self.free_paths.extend(flight.free_paths)
         self.free_paths_along_y.extend(flight.free_paths_along_y)
         self.travel_times.append(flight.travel_time)
-        self.detected_frequencies.append(flight.detected_frequency)
         self.mean_free_paths.append(flight.mean_free_path)
 
     def write_into_files(self):
         """Write all the data into files"""
         np.savetxt("Data/All free paths.csv", self.free_paths, fmt='%2.4e', delimiter=",", header="L [m]", encoding='utf-8')
         np.savetxt("Data/All free paths in plane.csv", self.free_paths_along_y, fmt='%2.4e', delimiter=",", header="Ly [m]", encoding='utf-8')
         np.savetxt("Data/All initial frequencies.csv", self.frequencies, fmt='%2.4e', delimiter=",", header="f [Hz]", encoding='utf-8')
-        np.savetxt("Data/All detected frequencies.csv", self.detected_frequencies, fmt='%2.4e', delimiter=",", header="f [Hz]", encoding='utf-8')
         np.savetxt("Data/All exit angles.csv", self.exit_angles, fmt='%2.4e', delimiter=",", header="Angle [rad]", encoding='utf-8')
         np.savetxt("Data/All initial angles.csv", self.initial_angles, fmt='%2.4e', delimiter=",", header="Angle [rad]", encoding='utf-8')
         np.savetxt("Data/All group velocities.csv", self.group_velocities, fmt='%2.4e', delimiter=",", header="Vg [rad]", encoding='utf-8')
         np.savetxt("Data/All travel times.csv", self.travel_times, fmt='%2.4e', delimiter=",", header="Travel time [s]", encoding='utf-8')
         np.savetxt("Data/All mean free paths.csv", self.mean_free_paths, fmt='%2.4e', delimiter=",", header="MFPs [m]", encoding='utf-8')
```

### Comparing `freepaths-1.4.1/freepaths/flight.py` & `freepaths-1.6/freepaths/flight.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     def __init__(self, phonon):
         """Initialize a phonon flight"""
         self.phonon = phonon
         self.initial_frequency = self.phonon.f
         self.initial_theta = self.phonon.theta
         self.path = Path(self.phonon.x, self.phonon.y, self.phonon.z)
         self.exit_theta = 0.0
-        self.detected_frequency = 0.0
         self.free_path = 0.0
         self.free_path_along_y = 0.0
         self.travel_time = 0.0
         self.time_since_previous_scattering = 0.0
         self.free_paths = []
         self.free_paths_along_y = []
 
@@ -63,20 +62,18 @@
 
     def restart(self):
         """Restart the flight after a scattering event"""
         self.time_since_previous_scattering = 0.0
         self.free_path = 0.0
         self.free_path_along_y = 0.0
 
-    def finish(self, step, timestep, detector_size):
+    def finish(self, step, timestep):
         """Finish the flight and record final state"""
         self.exit_theta = self.phonon.theta
         self.travel_time = step * timestep
-        if abs(self.phonon.x) < detector_size / 2.0:
-            self.detected_frequency = self.phonon.f
 
     def add_step(self, timestep):
         """Increase parameters of the flight by length of one step"""
         step_length = self.phonon.speed * timestep
         self.free_path += step_length
         self.free_path_along_y += step_length * abs(cos(self.phonon.phi)) * abs(cos(self.phonon.theta))
         self.time_since_previous_scattering += timestep
```

### Comparing `freepaths-1.4.1/freepaths/main_mfp_sampling.py` & `freepaths-1.6/freepaths/main_mfp_sampling.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4.1/freepaths/main_tracing.py` & `freepaths-1.6/freepaths/main_tracing.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         # Record trajectories of the first N phonons:
         if index < cf.output_trajectories_of_first:
             path_stats.save_phonon_path(flight)
 
     # Run additional calculations:
     thermal_maps.calculate_thermal_conductivity()
-
+    thermal_maps.calculate_normalized_flux()
     # Create the folder if it does not exist and copy input file there:
     if not os.path.exists(f"Results/{cf.output_folder_name}"):
         os.makedirs(f"Results/{cf.output_folder_name}")
         os.makedirs(f"Results/{cf.output_folder_name}/Data")
     if cf.output_path_animation and not os.path.exists(f"Results/{cf.output_folder_name}/Frames"):
         os.makedirs(f"Results/{cf.output_folder_name}/Frames")
     if input_file:
```

### Comparing `freepaths-1.4.1/freepaths/maps.py` & `freepaths-1.6/freepaths/maps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module that controles recording and calculation of maps"""
 
 import random
 from math import cos
 from scipy.constants import hbar, pi
 import numpy as np
-
+from math import cos , sin
 from freepaths.config import cf
 
 
 class ScatteringMap:
     """Map of scattering in the structure"""
 
     def __init__(self):
@@ -70,53 +70,71 @@
         """Initialize arrays of thermal maps"""
         self.thermal_map = np.zeros((cf.number_of_pixels_y, cf.number_of_pixels_x))
         self.heat_flux_profile_x = np.zeros((cf.number_of_pixels_x, cf.number_of_timeframes))
         self.heat_flux_profile_y = np.zeros((cf.number_of_pixels_y, cf.number_of_timeframes))
         self.temperature_profile_x = np.zeros((cf.number_of_pixels_x, cf.number_of_timeframes))
         self.temperature_profile_y = np.zeros((cf.number_of_pixels_y, cf.number_of_timeframes))
         self.thermal_conductivity = np.zeros((cf.number_of_timeframes, 2))
+        self.heat_flux_map_norm = np.zeros((cf.number_of_pixels_y, cf.number_of_pixels_x))
+        self.heat_flux_map_x = np.zeros((cf.number_of_pixels_y, cf.number_of_pixels_x))
+        self.heat_flux_map_y = np.zeros((cf.number_of_pixels_y, cf.number_of_pixels_x))
+        self.nor = np.zeros((cf.number_of_pixels_y, cf.number_of_pixels_x))
+        self.nor_heat_flux_y_map = np.zeros((cf.number_of_pixels_y, cf.number_of_pixels_x))
+        self.nor_heat_flux_x_map = np.zeros((cf.number_of_pixels_y, cf.number_of_pixels_x))
 
     def add_energy_to_maps(self, ph, timestep_number, material):
         """This function registers the phonon in the pixel corresponding to its current position
         and at certain timesteps and adds it to thermal maps and thermal profiles"""
 
         # Calculate the index of the pixel in which this phonon is now:
         index_x = int(((ph.x + cf.width / 2) * cf.number_of_pixels_x) // cf.width)
         # index_y = int((ph.y*number_of_pixels_y) // length)
         index_y = int(ph.y // (cf.length / cf.number_of_pixels_y))
 
         # Calculate the volume of this pixel:
         vol_cell = cf.length * cf.thickness * cf.width
         vol_cell_x = vol_cell / cf.number_of_pixels_x
         vol_cell_y = vol_cell / cf.number_of_pixels_y
-
+        vol_pixel =  vol_cell/(cf.number_of_pixels_x*cf.number_of_pixels_y)
         # Here we arbitrarily correct the volume of the unit cells in pillars:
-        if cf.include_pillars == 'yes':
-            vol_cell_x += 2.5 * 0.3333 * cf.pillar_height * (cf.circular_hole_diameter / 2) ** 2
-            vol_cell_y += 2.5 * 0.3333 * cf.pillar_height * (cf.circular_hole_diameter / 2) ** 2
+        # if cf.pillars:
+            # vol_cell_x += 2.5 * 0.3333 * cf.pillar_height * (cf.circular_hole_diameter / 2) ** 2
+            # vol_cell_y += 2.5 * 0.3333 * cf.pillar_height * (cf.circular_hole_diameter / 2) ** 2
 
         # Prevent error if the phonon is outside the structure:
         if (0 <= index_x < cf.number_of_pixels_x) and (0 <= index_y < cf.number_of_pixels_y):
 
             # Record energy h*w of this phonon into the pixel of thermal map:
             energy = hbar * 2 * pi * ph.f
             self.thermal_map[index_y, index_x] += energy
-
+            self.heat_flux_map_norm[index_y, index_x] += np.sqrt((energy * sin(ph.theta) * abs(cos(ph.phi)) * ph.speed /vol_pixel)**2 +(energy * cos(ph.theta) * abs(cos(ph.phi)) * ph.speed /vol_pixel)**2)
+            self.heat_flux_map_x[index_y, index_x] += (energy * sin(ph.theta) * abs(cos(ph.phi)) * ph.speed /cf.thickness/ vol_pixel)
+            self.heat_flux_map_y[index_y, index_x] += (energy * cos(ph.theta) * abs(cos(ph.phi)) * ph.speed /cf.thickness/ vol_pixel)
+            self.nor[index_y, index_x] += 1
             # Record energy of this phonon into flux and temperature profiles: (DOUBLE-CHECK THIS)
             random_timeframe = random.randint(0, cf.number_of_timesteps)
             assigned_time = (timestep_number + random_timeframe) * cf.timestep * cf.number_of_timeframes
             total_time = cf.number_of_timesteps * cf.timestep
             timeframe_number = int(assigned_time // total_time)
 
             if timeframe_number < cf.number_of_timeframes:
                 self.heat_flux_profile_x[index_x, timeframe_number] += energy * cos(ph.theta) * abs(cos(ph.phi)) * ph.speed / vol_cell_x
                 self.heat_flux_profile_y[index_y, timeframe_number] += energy * cos(ph.theta) * abs(cos(ph.phi)) * ph.speed / vol_cell_y
                 self.temperature_profile_x[index_x, timeframe_number] += energy / (cf.specific_heat_capacity * material.density) / vol_cell_x
                 self.temperature_profile_y[index_y, timeframe_number] += energy / (cf.specific_heat_capacity * material.density) / vol_cell_y
+    
+    def calculate_normalized_flux(self):
 
+        for j in range(cf.number_of_pixels_x):
+            for i in range(cf.number_of_pixels_y):
+                if self.nor[i,j] != 0:
+                    self.nor_heat_flux_y_map[i,j] = self.heat_flux_map_y[i,j] / self.nor[i,j]
+                    self.nor_heat_flux_x_map[i,j] = self.heat_flux_map_x[i,j] / self.nor[i,j]
+
+    
     def calculate_thermal_conductivity(self):
         """Calculate the thermal conductivity for each time interval from heat flux
         and temperature profiles accumulated in that interval"""
 
         # Initialize array for thermal conductivity in each time interval
         self.thermal_conductivity[:, 0] = range(cf.number_of_timeframes)
         total_time = cf.number_of_timesteps * cf.timestep * 1e9
@@ -141,15 +159,23 @@
             self.thermal_conductivity[timeframe_number, 1] = J * d_L / d_T
 
     def write_into_files(self):
         """Write thermal map into file"""
 
         if cf.output_raw_thermal_map:
             np.savetxt("Data/Thermal map.csv", self.thermal_map, fmt='%1.2e', delimiter=",", encoding='utf-8')
-
+        if cf.output_raw_thermal_map:
+            np.savetxt("Data/heat_flux_map_norm map.csv", self.heat_flux_map_norm, fmt='%1.2e', delimiter=",", encoding='utf-8')
+        if cf.output_raw_thermal_map:
+            np.savetxt("Data/heat_flux_map_x map.csv", self.heat_flux_map_x, fmt='%1.2e', delimiter=",", encoding='utf-8')
+        if cf.output_raw_thermal_map:
+            np.savetxt("Data/heat_flux_map_y map.csv", self.heat_flux_map_y, fmt='%1.2e', delimiter=",", encoding='utf-8')
+        if cf.output_raw_thermal_map:
+            np.savetxt("Data/nor_heat_flux_y map.csv", self.nor_heat_flux_y_map, fmt='%1.2e', delimiter=",", encoding='utf-8')
+            np.savetxt("Data/nor_heat_flux_x map.csv", self.nor_heat_flux_x_map, fmt='%1.2e', delimiter=",", encoding='utf-8')
         # Create coordinate arrays [um]
         num_of_points_x = self.temperature_profile_x.shape[0]
         num_of_points_y = self.temperature_profile_y.shape[0]
         coordinates_x = np.arange(num_of_points_x) * 1e6 * cf.width / num_of_points_x
         coordinates_y = np.arange(num_of_points_y) * 1e6 * cf.length / num_of_points_y
 
         # Saving all the profiles in the files:
@@ -159,7 +185,8 @@
         data_flux_y = np.vstack((coordinates_y, self.heat_flux_profile_y.T)).T
         data_tc = self.thermal_conductivity
         np.savetxt("Data/Temperature profiles x.csv", data_temp_x, fmt='%1.3e', delimiter=",", header="X (um), T (K)", encoding='utf-8')
         np.savetxt("Data/Temperature profiles y.csv", data_temp_y, fmt='%1.3e', delimiter=",", header="Y (um), T (K)", encoding='utf-8')
         np.savetxt("Data/Heat flux profiles x.csv", data_flux_x, fmt='%1.3e', delimiter=",", header="Y (um), J (a.u.)", encoding='utf-8')
         np.savetxt("Data/Heat flux profiles y.csv", data_flux_y, fmt='%1.3e', delimiter=",", header="Y (um), J (a.u.)", encoding='utf-8')
         np.savetxt("Data/Thermal conductivity.csv", data_tc, fmt='%1.3e', delimiter=",", header="t(ns), K (W/mK)", encoding='utf-8')
+
```

### Comparing `freepaths-1.4.1/freepaths/materials.py` & `freepaths-1.6/freepaths/materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-"""Module that assigns physical properties according to chosen material"""
+"""
+Module that assigns physical properties according to chosen material. References:
+Si - Ref. APL 95 161901 (2009)
+SiC - Ref. PRB 50 17054 (1994)
+Diamond - Carbon 91 266-274 (2015)
+AlN - Ref. PRB 58 12899 (1998)
+"""
 
 import numpy as np
 from freepaths.options import Materials
 
 
 class Material:
     """Material of the simulated media with certain physical properties"""
 
     def __init__(self, material, num_points=1000):
         self.name = material
 
-        if self.name == Materials.Si:  # Ref. APL 95 161901 (2009)
+        if self.name == Materials.Si:
             A1 = 1369.42
             B1 = -2.405e-8
             C1 = -9.70e-19
             A2 = 1081.74
             B2 = -7.711e-8
             C2 = 5.674e-19
             D2 = 7.967e-29
@@ -22,45 +28,45 @@
             self.density = 2330         # [kg/m^3]
             self.dispersion = np.zeros((num_points, 4))
             self.dispersion[:, 0] = [k * 12e9 / (num_points - 1) for k in range(num_points)]                         # Wavevectors
             self.dispersion[:, 1] = [abs(A1 * k + B1 * k**2 + C1 * k**3) for k in self.dispersion[:, 0]]             # LA branch
             self.dispersion[:, 2] = [abs(A2 * k + B2 * k**2 + C2 * k**3 + D2 * k**4) for k in self.dispersion[:, 0]] # TA branch
             self.dispersion[:, 3] = self.dispersion[:, 2]
 
-        elif self.name == Materials.SiC:  # Ref. PRB 50 17054 (1994)
+        elif self.name == Materials.SiC:
             A1 = 1737.36296
             B1 = 1.7604452e-08
             C1 = -3.48834e-18
             A2 = 1077.98941
             B2 = -3.43668e-08
             C2 = -2.21696e-19
             self.default_speed = 6500   # [m/s] Need to change this probably!
             self.density = 3215         # [kg/m^3]
             self.dispersion = np.zeros((num_points, 4))
             self.dispersion[:, 0] = [k * 14414281503 / (num_points - 1) for k in range(num_points)]       # Wavevectors
             self.dispersion[:, 1] = [abs(C1 * k**3 + B1 * k**2 + A1 * k) for k in self.dispersion[:, 0]]  # LA branch
             self.dispersion[:, 2] = [abs(C2 * k**3 + B2 * k**2 + A2 * k) for k in self.dispersion[:, 0]]  # TA branch
             self.dispersion[:, 3] = self.dispersion[:, 2]
 
-        elif self.name == Materials.Diamond:  # Ref. Carbon 91 266-274 (2015)
+        elif self.name == Materials.Diamond:
             A1 = 4309.95222
             B1 = -8.855338e-08
             C1 = -1.347265e-18
             A2 = 3185.66561
             B2 = -4.104260e-08
             C2 = -5.042335e-18
             self.default_speed = 20000  # [m/s]
             self.density = 3500         # [kg/m^3]
             self.dispersion = np.zeros((num_points, 4))
             self.dispersion[:, 0] = [k * 11707071561.7 / (num_points - 1) for k in range(num_points)]     # Wavevectors
             self.dispersion[:, 1] = [abs(C1 * k**3 + B1 * k**2 + A1 * k) for k in self.dispersion[:, 0]]  # LA branch
             self.dispersion[:, 2] = [abs(C2 * k**3 + B2 * k**2 + A2 * k) for k in self.dispersion[:, 0]]  # TA branch
             self.dispersion[:, 3] = self.dispersion[:, 2]
 
-        elif self.name == Materials.AlN:  # Ref. PRB 58 12899 (1998)
+        elif self.name == Materials.AlN:
             A1 = 946.677
             B1 = 3.08258e-08
             C1 = -2.990977e-18
             A2 = 1852.27
             B2 = -2.08813e-08
             C2 = -3.047928e-18
             self.default_speed = 6200     # [m/s]
```

### Comparing `freepaths-1.4.1/freepaths/move.py` & `freepaths-1.6/freepaths/move.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4.1/freepaths/output_info.py` & `freepaths-1.6/freepaths/output_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,36 +63,36 @@
             f'\n{scat_on_topbot:.2f}% - scattering on top and bottom walls ',
             f'({scat_on_topbot_diff:.2f}% - diffuse, ',
             f'{scat_on_topbot_spec:.2f}% - specular)',
             f'\n{retherm:.2f}% - rethermalization at the hot side',
             f'\n{internal:.2f}% - internal scattering processes',
     )
 
-    if cf.include_holes:
+    if cf.holes:
         scat_on_holes = 100*(np.sum(scatter_stats.hole_diffuse) +
                              np.sum(scatter_stats.hole_specular)) / total
         scat_on_holes_diff = 100*np.sum(scatter_stats.hole_diffuse) / total_hole
         scat_on_holes_spec = 100*np.sum(scatter_stats.hole_specular) / total_hole
         info2 = (
                 f'\n{scat_on_holes:.2f}% - scattering on hole walls ',
                 f'({scat_on_holes_diff:.2f}% - diffuse, ',
                 f'{scat_on_holes_spec:.2f}% - specular)',
         )
 
-    if cf.include_pillars:
+    if cf.pillars:
         scat_on_pill = 100*(np.sum(scatter_stats.pillar_diffuse) +
                             np.sum(scatter_stats.pillar_specular)) / total
         scat_on_pill_diff = 100*np.sum(scatter_stats.pillar_diffuse) / total_pill
         scat_on_pill_spec = 100*np.sum(scatter_stats.pillar_specular) / total_pill
         info3 = (
                 f'\n{scat_on_pill:.2f}% - scattering on pillar walls ',
                 f'({scat_on_pill_diff:.2f}% - diffuse, ',
                 f'{scat_on_pill_spec:.2f}% - specular)'
         )
 
     # Write info into a text file:
     with open("Information.txt", "a", encoding="utf-8") as file:
         file.writelines(info1)
-        if cf.include_holes:
+        if cf.holes:
             file.writelines(info2)
-        if cf.include_pillars:
+        if cf.pillars:
             file.writelines(info3)
```

### Comparing `freepaths-1.4.1/freepaths/output_plots.py` & `freepaths-1.6/freepaths/output_plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -135,26 +135,14 @@
     ax.set_xlabel('Mean free path (nm)', fontsize=12)
     ax.set_ylabel('Number of phonons', fontsize=12)
     fig.savefig("Distribution of MFPs.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of MFPs.csv', mean_free_path_distribution, fmt='%1.3e', delimiter=",")
 
 
-def plot_detected_frequency_distribution():
-    """Plot distribution of detected frequencies"""
-    detected_frequency_distribution = distribution_calculation("Data/All detected frequencies.csv", None, cf.number_of_nodes)
-    fig, ax = plt.subplots()
-    ax.plot(detected_frequency_distribution[:, 0], detected_frequency_distribution[:, 1], 'royalblue')
-    ax.set_xlabel('Frequency (Hz)', fontsize=12)
-    ax.set_ylabel('Number of phonons', fontsize=12)
-    fig.savefig("Distribution of detected frequencies.pdf", dpi=300, format='pdf', bbox_inches="tight")
-    if cf.plots_in_terminal: plt.show()
-    np.savetxt('Data/Distribution of detected frequencies.csv', detected_frequency_distribution, fmt='%1.3e', delimiter=",")
-
-
 def plot_velocity_distribution():
     """Plot distribution of group velocities"""
     fig, ax = plt.subplots()
     speeds = np.loadtxt("Data/All group velocities.csv")
     frequencies = np.loadtxt("Data/All initial frequencies.csv")
     ax.plot(frequencies, speeds, '.', c='royalblue')
     ax.set_xlabel('Frequency (Hz)', fontsize=12)
@@ -221,14 +209,93 @@
     plt.xlabel('X (μm)', fontsize=12)
     plt.ylabel('Y (μm)', fontsize=12)
     cbar = plt.colorbar()
     cbar.set_label('Energy density', rotation=90)
     fig.savefig("Thermal map.pdf", bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
 
+def plot_heat_flux_map_norm():
+    """Plot thermal map as color map"""
+    fig = plt.figure()
+    heat_flux_map = np.genfromtxt("Data/heat_flux_map_norm map.csv", unpack=False, delimiter=',', skip_header=0, encoding='utf-8')
+    heat_flux_map = np.flipud(heat_flux_map)
+    minimum_of_colorbar = 1e5  # Cannot be zero!
+    boundaries = [(-cf.width / 2) * 1e6, (cf.width / 2) * 1e6, 0, cf.length * 1e6]
+    plt.imshow(heat_flux_map, cmap='hot', interpolation='none', extent=boundaries,
+               norm=LogNorm(vmin=minimum_of_colorbar, vmax=np.amax(heat_flux_map)))
+    plt.xlabel('X (μm)', fontsize=12)
+    plt.ylabel('Y (μm)', fontsize=12)
+    cbar = plt.colorbar()
+    cbar.set_label('Energy flux norm', rotation=90)
+    fig.savefig("Heat flux map norm.pdf", bbox_inches="tight")
+    if cf.plots_in_terminal: plt.show()
+
+def plot_heat_flux_map_x():
+    """Plot thermal map as color map"""
+    fig = plt.figure()
+    heat_flux_map = np.genfromtxt("Data/heat_flux_map_x map.csv", unpack=False, delimiter=',', skip_header=0, encoding='utf-8')
+    heat_flux_map = np.flipud(heat_flux_map)
+    minimum_of_colorbar = 1e5  # Cannot be zero!
+    boundaries = [(-cf.width / 2) * 1e6, (cf.width / 2) * 1e6, 0, cf.length * 1e6]
+    plt.imshow(heat_flux_map, cmap='hot', interpolation='none', extent=boundaries,
+               norm=LogNorm(vmin=minimum_of_colorbar, vmax=np.amax(heat_flux_map)))
+    plt.xlabel('X (μm)', fontsize=12)
+    plt.ylabel('Y (μm)', fontsize=12)
+    cbar = plt.colorbar()
+    cbar.set_label('Energy flux x', rotation=90)
+    fig.savefig("Heat flux map x.pdf", bbox_inches="tight")
+    if cf.plots_in_terminal: plt.show()
+
+def plot_heat_flux_map_y():
+    """Plot thermal map as color map"""
+    fig = plt.figure()
+    heat_flux_map = np.genfromtxt("Data/heat_flux_map_y map.csv", unpack=False, delimiter=',', skip_header=0, encoding='utf-8')
+    heat_flux_map = np.flipud(heat_flux_map)
+    minimum_of_colorbar = 1e5  # Cannot be zero!
+    boundaries = [(-cf.width / 2) * 1e6, (cf.width / 2) * 1e6, 0, cf.length * 1e6]
+    plt.imshow(heat_flux_map, cmap='hot', interpolation='none', extent=boundaries,
+               norm=LogNorm(vmin=minimum_of_colorbar, vmax=np.amax(heat_flux_map)))
+    plt.xlabel('X (μm)', fontsize=12)
+    plt.ylabel('Y (μm)', fontsize=12)
+    cbar = plt.colorbar()
+    cbar.set_label('Energy flux y', rotation=90)
+    fig.savefig("Heat flux map y.pdf", bbox_inches="tight")
+    if cf.plots_in_terminal: plt.show()
+
+def plot_nor_heat_flux_map_x():
+    """Plot thermal map as color map"""
+    fig = plt.figure()
+    heat_flux_map = np.genfromtxt("Data/nor_heat_flux_x map.csv", unpack=False, delimiter=',', skip_header=0, encoding='utf-8')
+    heat_flux_map = np.flipud(heat_flux_map)
+    minimum_of_colorbar = 1e9  # Cannot be zero!
+    boundaries = [(-cf.width / 2) * 1e6, (cf.width / 2) * 1e6, 0, cf.length * 1e6]
+    plt.imshow(heat_flux_map, cmap='hot', interpolation='none', extent=boundaries,
+               norm=LogNorm(vmin=minimum_of_colorbar, vmax=np.amax(heat_flux_map)))
+    plt.xlabel('X (μm)', fontsize=12)
+    plt.ylabel('Y (μm)', fontsize=12)
+    cbar = plt.colorbar()
+    cbar.set_label('Energy flux normalized x', rotation=90)
+    fig.savefig("Heat flux map normalised.pdf", bbox_inches="tight")
+    if cf.plots_in_terminal: plt.show()
+
+def plot_nor_heat_flux_map_y():
+    """Plot thermal map as color map"""
+    fig = plt.figure()
+    heat_flux_map = np.genfromtxt("Data/nor_heat_flux_y map.csv", unpack=False, delimiter=',', skip_header=0, encoding='utf-8')
+    heat_flux_map = np.flipud(heat_flux_map)
+    minimum_of_colorbar = 1e9  # Cannot be zero!
+    boundaries = [(-cf.width / 2) * 1e6, (cf.width / 2) * 1e6, 0, cf.length * 1e6]
+    plt.imshow(heat_flux_map, cmap='hot', interpolation='none', extent=boundaries,
+               norm=LogNorm(vmin=minimum_of_colorbar, vmax=np.amax(heat_flux_map)))
+    plt.xlabel('X (μm)', fontsize=12)
+    plt.ylabel('Y (μm)', fontsize=12)
+    cbar = plt.colorbar()
+    cbar.set_label('Energy flux normalizedy', rotation=90)
+    fig.savefig("Heat flux map normalised.pdf", bbox_inches="tight")
+    if cf.plots_in_terminal: plt.show()  
 
 def plot_scattering_map():
     """Plot the map of scattering events"""
     fig, ax = plt.subplots()
     filename = "Data/Scattering map.csv"
     spec_x, spec_y, diff_x, diff_y, int_x, int_y = np.genfromtxt(filename, unpack=True, delimiter=',', skip_header=1, encoding='utf-8')
     ax.plot(diff_x[diff_x != 0], diff_y[diff_y != 0], 'o', color='b', markersize=0.1, alpha=0.3)
@@ -247,15 +314,15 @@
 
     data = np.genfromtxt("Data/Phonon paths.csv", unpack=False, delimiter=',', skip_header=1, encoding='utf-8')
 
     # Create XY plot:
     fig, ax = plt.subplots()
 
     # Draw structures:
-    patches = draw_structure(cf)
+    patches = draw_structure(cf, color_holes='white', color_back=cf.output_structure_color)
     for patch in patches:
         ax.add_patch(patch)
 
     # Draw paths:
     for index in range(cf.output_trajectories_of_first):
         x_coordinates = np.trim_zeros(data[:, 3 * index], trim='b')
         y_coordinates = np.trim_zeros(data[:, 3 * index + 1], trim='b')
@@ -316,24 +383,45 @@
     header2 = "Top & bottom specular [1/ns], Holes diffuse [1/ns], Holes specular [1/ns], Hot side [1/ns], "
     header3 = "Internal [1/ns], Pillars diffuse [1/ns], Pillars specular [1/ns]"
     header = header1 + header2 + header3
     data = np.vstack((segments, all_scattering_rates)).T
     np.savetxt(filename, data, fmt='%1.2e', delimiter=",", header=header)
 
 
+def plot_structure():
+    """Plot the structure with all the elements"""
+
+    # Create XY plot:
+    fig, ax = plt.subplots()
+
+    # Draw structures:
+    patches = draw_structure(cf, color_holes='black', color_back='royalblue')
+    for patch in patches:
+        ax.add_patch(patch)
+
+    # Set labels:
+    ax.set_xlabel('X (μm)', fontsize=12)
+    ax.set_ylabel('Y (μm)', fontsize=12)
+    ax.set_aspect('equal', 'datalim')
+    ax.set_xlim(1.2*-cf.width*1e6, 1.2*cf.width*1e6)
+    ax.set_ylim(0, cf.length*1e6)
+    fig.savefig("Structure XY.pdf", dpi=600, format='pdf', bbox_inches="tight")
+    if cf.plots_in_terminal: plt.show()
+
+
 def plot_data():
     """Create plots of various distributions"""
+    plot_structure()
     plot_trajectories()
     plot_angle_distribution()
     plot_free_path_distribution()
     plot_frequency_distribution()
     plot_wavelength_distribution()
     plot_travel_time_distribution()
     plot_mean_free_path_distribution()
-    plot_detected_frequency_distribution()
     plot_velocity_distribution()
     plot_time_in_segments()
     plot_thermal_conductivity()
     plot_temperature_profile()
     plot_heat_flux_profile()
     plot_thermal_map()
     plot_scattering_statistics()
```

### Comparing `freepaths-1.4.1/freepaths/phonon.py` & `freepaths-1.6/freepaths/phonon.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,34 +12,42 @@
 import freepaths.move
 
 
 class Phonon:
     """A phonon particle with various physical properties"""
 
     def __init__(self, material, polarization=None, phonon_number=None):
-        """Initialize a phonon by assigning coordinates and other properties"""
+        """Initialize a phonon by assigning initial properties"""
         self.polarization = polarization
         self.phonon_number = phonon_number
         self.x = None
         self.y = None
         self.z = None
         self.f = None
         self.phi = None
         self.theta = None
         self.speed = None
 
+        # Assigning initial properties of the phonon:
         if polarization is None:
-            self.assign_polarization()
-        self.assign_coordinates()
-        self.assign_angles()
+            self.polarization = choice([Polarizations.TA, Polarizations.TA, Polarizations.LA])
+        source = choice(cf.phonon_sources)
+        self.x, self.y, self.z = source.generate_coordinates()
+        self.theta, self.phi = source.generate_angles()
+
+        # Frequency is assigned based on Planckian distribution in case MFP sampling mode:
         if phonon_number is None:
             self.assign_frequency(material)
+
+        # Otherwise, frequency is just asigned depending on the phonon number:
         else:
             branch = polarization.value
             self.f = abs((material.dispersion[phonon_number+1, branch] + material.dispersion[phonon_number, branch]) / 2)
+
+        # self.f = 6e12 # FIX THIS
         self.assign_speed(material)
         self.assign_internal_scattering_time(material)
 
     @property
     def wavelength(self):
         """Calculate wavelength of the phonon"""
         return self.speed/self.f
@@ -53,49 +61,14 @@
         is_inside_right = self.x < cf.width / 2.0
         is_inside_left = self.x > - cf.width / 2.0
         return ((not cf.cold_side_position_top or is_inside_top) and
                 (not cf.cold_side_position_bottom or is_inside_bottom) and
                 (not cf.cold_side_position_right or is_inside_right) and
                 (not cf.cold_side_position_left or is_inside_left))
 
-    def assign_polarization(self):
-        """Assign branch of phonon dispersion"""
-        self.polarization = choice([Polarizations.TA, Polarizations.TA, Polarizations.LA])
-
-    def assign_coordinates(self):
-        """Assign initial coordinates at the hot side"""
-        self.x = cf.phonon_source_x + 0.49 * cf.phonon_source_width_x * (2 * random() - 1)
-        self.y = cf.phonon_source_y + 0.49 * cf.phonon_source_width_y * (2 * random() - 1)
-        self.z = 0.49 * cf.thickness * (2 * random() - 1)
-
-    def assign_angles(self):
-        """Depending on angle distribution, assign angles"""
-        if cf.phonon_source_angle_distribution == Distributions.RANDOM_UP:
-            self.theta = -pi/2 + pi*random()
-            self.phi = asin(2*random() - 1)
-        if cf.phonon_source_angle_distribution == Distributions.RANDOM_DOWN:
-            rand_sign = sign((2*random() - 1))
-            self.theta = rand_sign*(pi/2 + pi/2*random())
-            self.phi = asin(2*random() - 1)
-        if cf.phonon_source_angle_distribution == Distributions.RANDOM_RIGHT:
-            self.theta = pi*random()
-            self.phi = asin(2*random() - 1)
-        if cf.phonon_source_angle_distribution == Distributions.RANDOM_LEFT:
-            self.theta = - pi*random()
-            self.phi = asin(2*random() - 1)
-        if cf.phonon_source_angle_distribution == Distributions.DIRECTIONAL:
-            self.theta = 0
-            self.phi = -pi/2 + pi*random()
-        if cf.phonon_source_angle_distribution == Distributions.LAMBERT:
-            self.theta = asin(2*random() - 1)
-            self.phi = asin((asin(2*random() - 1))/(pi/2))
-        if cf.phonon_source_angle_distribution == Distributions.UNIFORM:
-            self.theta = -pi + 2*pi*random()
-            self.phi = asin(2*random() - 1)
-
     def assign_frequency(self, material):
         """Assigning frequency with probability according to Planckian distribution"""
 
         # Frequency of the peak of the Plank distribution:
         f_max = material.default_speed/(2*pi*hbar*material.default_speed/(2.82*k*cf.temp))
 
         # Density of states for f_max in Debye apparoximation:
```

### Comparing `freepaths-1.4.1/freepaths/progress.py` & `freepaths-1.6/freepaths/progress.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.4.1/freepaths/run_phonon.py` & `freepaths-1.6/freepaths/run_phonon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-"""Module that runs one phonon through the structure"""
-
+"""
+Module that runs one phonon through the structure, from phonon source to a cold side.
+After the run, we record various parameters of this run into flight object.
+"""
 
 from freepaths.config import cf
 from freepaths.scattering import internal_scattering, surface_scattering, reinitialization
 from freepaths.scattering_types import ScatteringTypes
 
 
 def run_phonon(phonon, flight, scatter_stats, segment_stats, thermal_maps, scatter_maps, material):
     """Run one phonon through the system and record parameters of this run"""
 
+    # Initialize object that will store scattering types:
     scattering_types = ScatteringTypes()
 
     # Run the phonon step-by-step:
     for step_number in range(cf.number_of_timesteps):
         if phonon.is_in_system:
 
             # Check if different scattering events happened during current time step:
@@ -47,9 +50,9 @@
             scattering_types.reset()
             phonon.move()
 
         # If the phonon reached cold side, record it and break the loop:
         else:
             flight.add_point_to_path()
             flight.save_free_paths()
-            flight.finish(step_number, cf.timestep, cf.frequency_detector_size)
+            flight.finish(step_number, cf.timestep)
             break
```

### Comparing `freepaths-1.4.1/freepaths/scattering_types.py` & `freepaths-1.6/freepaths/scattering_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""Module that provides phonon scattering types that occur on each step"""
+"""
+Module that provides types of phonon scattering that might occur.
+These scattering types are returned on each step
+so that higher level modules know what has happened.
+"""
 
 import enum
 
 
 class Scattering(enum.Enum):
     """Possible scattering types"""
     DIFFUSE = 1
```

### Comparing `freepaths-1.4.1/freepaths.egg-info/PKG-INFO` & `freepaths-1.6/freepaths.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.4.1
+Version: 1.6
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.4.1/freepaths.egg-info/SOURCES.txt` & `freepaths-1.6/freepaths.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 freepaths/options.py
 freepaths/output_info.py
 freepaths/output_plots.py
 freepaths/output_structure.py
 freepaths/phonon.py
 freepaths/progress.py
 freepaths/run_phonon.py
+freepaths/scatterers.py
 freepaths/scattering.py
+freepaths/scattering_parabolic.py
+freepaths/scattering_primitives.py
+freepaths/scattering_semicircle.py
 freepaths/scattering_types.py
+freepaths/sources.py
 freepaths.egg-info/PKG-INFO
 freepaths.egg-info/SOURCES.txt
 freepaths.egg-info/dependency_links.txt
 freepaths.egg-info/entry_points.txt
 freepaths.egg-info/requires.txt
 freepaths.egg-info/top_level.txt
```

### Comparing `freepaths-1.4.1/setup.py` & `freepaths-1.6/setup.py`

 * *Files identical despite different names*

