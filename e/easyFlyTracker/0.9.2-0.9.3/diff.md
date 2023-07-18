# Comparing `tmp/easyFlyTracker-0.9.2.tar.gz` & `tmp/easyFlyTracker-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easyFlyTracker-0.9.2.tar", last modified: Fri Dec 10 05:54:56 2021, max compression
+gzip compressed data, was "dist\easyFlyTracker-0.9.3.tar", last modified: Fri Dec 10 09:16:46 2021, max compression
```

## Comparing `easyFlyTracker-0.9.2.tar` & `easyFlyTracker-0.9.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2021-12-10 05:54:56.000000 easyFlyTracker-0.9.2/
--rw-rw-rw-   0        0        0     5836 2021-12-10 05:54:56.000000 easyFlyTracker-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     3954 2021-08-13 10:32:47.000000 easyFlyTracker-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2021-12-10 05:54:56.000000 easyFlyTracker-0.9.2/easyFlyTracker/
--rw-rw-rw-   0        0        0      325 2021-12-10 01:21:58.000000 easyFlyTracker-0.9.2/easyFlyTracker/__init__.py
--rw-rw-rw-   0        0        0     1534 2021-12-10 01:22:55.000000 easyFlyTracker-0.9.2/easyFlyTracker/cli.py
-drwxrwxrwx   0        0        0        0 2021-12-10 05:54:56.000000 easyFlyTracker-0.9.2/easyFlyTracker/fonts/
--rw-rw-rw-   0        0        0  1195688 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.2/easyFlyTracker/fonts/times.ttf
--rw-rw-rw-   0        0        0  1175904 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.2/easyFlyTracker/fonts/timesbd.ttf
--rw-rw-rw-   0        0        0   881860 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.2/easyFlyTracker/fonts/timesbi.ttf
--rw-rw-rw-   0        0        0   940288 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.2/easyFlyTracker/fonts/timesi.ttf
-drwxrwxrwx   0        0        0        0 2021-12-10 05:54:56.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/
--rw-rw-rw-   0        0        0     5167 2021-12-08 09:49:59.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/Camera_Calibration.py
--rw-rw-rw-   0        0        0     4035 2020-12-07 02:15:32.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/SignificanceTest.py
--rw-rw-rw-   0        0        0      801 2021-06-02 08:48:10.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/__init__.py
--rw-rw-rw-   0        0        0    30668 2021-12-10 05:47:19.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/analysis.py
--rw-rw-rw-   0        0        0     4231 2021-12-08 09:48:44.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/fly_angle.py
--rw-rw-rw-   0        0        0    17185 2021-12-08 09:51:16.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/fly_seg.py
--rw-rw-rw-   0        0        0    13834 2021-12-08 09:51:15.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/gui_config.py
--rw-rw-rw-   0        0        0     3090 2021-12-10 05:14:50.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/kernel_density_estimation.py
--rw-rw-rw-   0        0        0     1986 2021-12-08 09:51:16.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/load_configyaml.py
--rw-rw-rw-   0        0        0    24335 2021-12-10 05:47:19.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/show.py
--rw-rw-rw-   0        0        0     9951 2021-12-08 10:00:44.000000 easyFlyTracker-0.9.2/easyFlyTracker/src_code/utils.py
-drwxrwxrwx   0        0        0        0 2021-12-10 05:54:56.000000 easyFlyTracker-0.9.2/easyFlyTracker.egg-info/
--rw-rw-rw-   0        0        0     5836 2021-12-10 05:54:55.000000 easyFlyTracker-0.9.2/easyFlyTracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      859 2021-12-10 05:54:55.000000 easyFlyTracker-0.9.2/easyFlyTracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-10 05:54:55.000000 easyFlyTracker-0.9.2/easyFlyTracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      223 2021-12-10 05:54:55.000000 easyFlyTracker-0.9.2/easyFlyTracker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2021-12-10 05:54:55.000000 easyFlyTracker-0.9.2/easyFlyTracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-12-10 05:54:55.000000 easyFlyTracker-0.9.2/easyFlyTracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-10 05:54:56.000000 easyFlyTracker-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     2041 2021-08-13 06:31:04.000000 easyFlyTracker-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/
+-rw-rw-rw-   0        0        0     5836 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3954 2021-08-13 10:32:47.000000 easyFlyTracker-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker/
+-rw-rw-rw-   0        0        0      325 2021-12-10 08:19:18.000000 easyFlyTracker-0.9.3/easyFlyTracker/__init__.py
+-rw-rw-rw-   0        0        0     1534 2021-12-10 01:22:55.000000 easyFlyTracker-0.9.3/easyFlyTracker/cli.py
+drwxrwxrwx   0        0        0        0 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker/fonts/
+-rw-rw-rw-   0        0        0  1195688 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.3/easyFlyTracker/fonts/times.ttf
+-rw-rw-rw-   0        0        0  1175904 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.3/easyFlyTracker/fonts/timesbd.ttf
+-rw-rw-rw-   0        0        0   881860 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.3/easyFlyTracker/fonts/timesbi.ttf
+-rw-rw-rw-   0        0        0   940288 2019-12-07 09:08:27.000000 easyFlyTracker-0.9.3/easyFlyTracker/fonts/timesi.ttf
+drwxrwxrwx   0        0        0        0 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/
+-rw-rw-rw-   0        0        0     5167 2021-12-08 09:49:59.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/Camera_Calibration.py
+-rw-rw-rw-   0        0        0     4035 2020-12-07 02:15:32.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/SignificanceTest.py
+-rw-rw-rw-   0        0        0      801 2021-06-02 08:48:10.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/__init__.py
+-rw-rw-rw-   0        0        0    30668 2021-12-10 05:47:19.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/analysis.py
+-rw-rw-rw-   0        0        0     4231 2021-12-08 09:48:44.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/fly_angle.py
+-rw-rw-rw-   0        0        0    17185 2021-12-08 09:51:16.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/fly_seg.py
+-rw-rw-rw-   0        0        0    13834 2021-12-08 09:51:15.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/gui_config.py
+-rw-rw-rw-   0        0        0     3090 2021-12-10 05:14:50.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/kernel_density_estimation.py
+-rw-rw-rw-   0        0        0     1986 2021-12-08 09:51:16.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/load_configyaml.py
+-rw-rw-rw-   0        0        0    26032 2021-12-10 09:00:58.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/show.py
+-rw-rw-rw-   0        0        0     9951 2021-12-08 10:00:44.000000 easyFlyTracker-0.9.3/easyFlyTracker/src_code/utils.py
+drwxrwxrwx   0        0        0        0 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker.egg-info/
+-rw-rw-rw-   0        0        0     5836 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      859 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      223 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/easyFlyTracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-12-10 09:16:46.000000 easyFlyTracker-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     2041 2021-08-13 06:31:04.000000 easyFlyTracker-0.9.3/setup.py
```

### Comparing `easyFlyTracker-0.9.2/PKG-INFO` & `easyFlyTracker-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFlyTracker
-Version: 0.9.2
+Version: 0.9.3
 Summary: An easy-to-use program for analyzing Drosophila Activity.
 Home-page: https://github.com/azzhu/EasyFlyTracker
 Author: azzhu
 Author-email: zhu.qingjie@qq.com
 License: MIT
 Project-URL: Source Code, https://github.com/azzhu/EasyFlyTracker
 Project-URL: Bug Tracker, https://github.com/azzhu/EasyFlyTracker/issues
```

### Comparing `easyFlyTracker-0.9.2/README.md` & `easyFlyTracker-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/cli.py` & `easyFlyTracker-0.9.3/easyFlyTracker/cli.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/fonts/times.ttf` & `easyFlyTracker-0.9.3/easyFlyTracker/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/fonts/timesbd.ttf` & `easyFlyTracker-0.9.3/easyFlyTracker/fonts/timesbd.ttf`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/fonts/timesbi.ttf` & `easyFlyTracker-0.9.3/easyFlyTracker/fonts/timesbi.ttf`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/fonts/timesi.ttf` & `easyFlyTracker-0.9.3/easyFlyTracker/fonts/timesi.ttf`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/Camera_Calibration.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/Camera_Calibration.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/SignificanceTest.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/SignificanceTest.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/__init__.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/__init__.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/analysis.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/analysis.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/fly_angle.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/fly_angle.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/fly_seg.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/fly_seg.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/gui_config.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/gui_config.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/kernel_density_estimation.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/kernel_density_estimation.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/load_configyaml.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/load_configyaml.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/show.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/show.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,17 +325,17 @@
 
         plt.close()
         plt.rcParams['figure.figsize'] = (15.0, 8.0)
         plt.grid(linewidth=1)
         plt.xlim((-10, 190))
         ax = plt.gca()
         ax.set_xticks([i * 10 for i in range(19)])
-        plt.xlabel('Angle region (degree)', fontproperties=self.font_timesbd)
+        plt.xlabel('Angle (degree)', fontproperties=self.font_timesbd)
         plt.ylabel('Probability Density', fontproperties=self.font_timesbd)
-        plt.title('Histogram of angle change per duration', fontproperties=self.font_timesbd)
+        plt.title('Probability density of angle change per duration', fontproperties=self.font_timesbd)
         for i, hi in enumerate(hists):
             plt.plot(xs, hi, label=f'Duration {i + 1}')
         plt.xticks(fontproperties=self.font_times)
         plt.yticks(fontproperties=self.font_times)
         plt.legend(prop={'family': 'Times New Roman', 'size': 12})
         plt.legend(loc='upper right')
         plt.savefig(str(Path(self.saved_dir, f'angle_change_per_duration_[{self.saved_suffix}].png')))
@@ -413,14 +413,71 @@
     df.to_excel(Path(excel_dir, f'average_sleep_time_per_{sleep_time_duration}_mins_[merge].xlsx'))
     df = pd.DataFrame(data=np.array([da[1] for da in das]),
                       index=suffixs,
                       columns=[str(_ + 1) for _ in range(len(das[0][0]))])
     df.to_excel(Path(excel_dir, f'proportion_of_sleep_flies_{sleep_time_duration}_mins_[merge].xlsx'))
 
 
+def merge_angle_changes_result(params):
+    '''
+    已有的结果每个图上的线是按照duration来区分，现在是按照group来区分。
+    几个group几条线，时间维度是整个视频。
+    :return:
+    '''
+    from easyFlyTracker.src_code.kernel_density_estimation import get_KernelDensity
+
+    cap = cv2.VideoCapture(params['video_path'])
+    fps = int(round(cap.get(cv2.CAP_PROP_FPS)))
+    cap.release()
+
+    rois = params['rois']
+    flags = [r[1] for r in rois]
+    rois = [r[0] for r in rois]
+
+    npy_file_path_cor = Path(params['output_dir'], '.cache', 'analysis_result', 'fly_angles_cor.npy')
+    ang = np.load(npy_file_path_cor)
+    ang_sec = ang[::fps]
+    as1 = ang_sec[:-1]
+    as2 = ang_sec[1:]
+    changes = np.abs(as2 - as1)
+    changes = np.where(changes > 180, 360 - changes, changes)  # 相比前一秒的变化角度（0-180）
+    changes_gps = [changes[:, r] for r in rois]
+
+    hists = [get_KernelDensity(cg, bins=500, range=(0, 180)) for cg in changes_gps]
+    xs = hists[0][0]
+    hists = np.array([h[1] for h in hists])
+
+    font_times = FontProperties(fname=str(Path(Path(__file__).parent.parent, 'fonts/times.ttf')), size=12)
+    font_timesbd = FontProperties(fname=str(Path(Path(__file__).parent.parent, 'fonts/timesbd.ttf')), size=15)
+    plt.close()
+    plt.rcParams['figure.figsize'] = (15.0, 8.0)
+    plt.grid(linewidth=1)
+    plt.xlim((-10, 190))
+    ax = plt.gca()
+    ax.set_xticks([i * 10 for i in range(19)])
+    plt.xlabel('Angle (degree)', fontproperties=font_timesbd)
+    plt.ylabel('Probability Density', fontproperties=font_timesbd)
+    plt.title('Probability density of angle change per group', fontproperties=font_timesbd)
+    for i, hi in enumerate(hists):
+        plt.plot(xs, hi, label=f'{flags[i]}')
+    plt.xticks(fontproperties=font_times)
+    plt.yticks(fontproperties=font_times)
+    plt.legend(prop={'family': 'Times New Roman', 'size': 12})
+    plt.legend(loc='upper right')
+
+    saved_dir = Path(params['output_dir']) / 'plot_images'
+    saved_dir_npys = saved_dir / '.npys'
+    saved_dir_excels = Path(params['output_dir']) / 'plot_excels'
+    plt.savefig(str(Path(saved_dir, f'angle_change_per_group.png')))
+    np.save(str(Path(saved_dir_npys, f'angle_change_per_group.npy')), hists)
+    df = pd.DataFrame(data=hists, columns=xs, index=flags)
+    df.to_excel(Path(saved_dir_excels, f'angle_change_per_group.xlsx'))
+    ...
+
+
 def merge_result(params):
     suffixs = [v[-1] for v in params['rois']]
     ana_time_duration = params['ana_time_duration']
     sleep_time_duration = params['sleep_time_duration']
     prefixs = [  # 前缀、x轴标签、y轴标签，title
         [f'average_distances_per_flies_per_{ana_time_duration}_mins',
          f'Video Time (per {ana_time_duration} mins)',
@@ -498,33 +555,13 @@
         with Wait():
             s = Show(**show_params)
             s.show_all()
 
     if len(rois) > 1:
         merge_result(params)
 
+    # 最后再生成一张angle_changes的merge结果
+    merge_angle_changes_result(params)
 
-if __name__ == '__main__':
-    p = r'D:\Pycharm_Projects\qu_holmes_su_release\tests\output2\config.pkl'
-    with open(p, 'rb') as f:
-        data = pickle.load(f)
-    exit()
-
-    rois = [
-        [[0, 1, 2, 3], '1'],
-        [[4, 5, 6, 7], '2'],
-    ]
-    ana_params = {
-        'video_path': r'D:\Pycharm_Projects\qu_holmes_su_release\tests\demo.mp4',
-        'roi_flys_flag': '1', 'area_th': 0.5, 'ana_time_duration': 0.5,
-    }
 
-    for ids, flag in rois:
-        ana_params['roi_flys_flag'] = flag
-        ana_params['roi_flys_ids'] = ids
-        print(f'---------- {flag} ----------')
-        s = Show(video_path=r'D:\Pycharm_Projects\qu_holmes_su_release\tests\demo.mp4',
-                 roi_flys_ids=ids,
-                 suffix=flag,
-                 ana_params=ana_params,
-                 dish_radius_mm=10)
-        s.show_all()
+if __name__ == '__main__':
+    pass
```

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker/src_code/utils.py` & `easyFlyTracker-0.9.3/easyFlyTracker/src_code/utils.py`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker.egg-info/PKG-INFO` & `easyFlyTracker-0.9.3/easyFlyTracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFlyTracker
-Version: 0.9.2
+Version: 0.9.3
 Summary: An easy-to-use program for analyzing Drosophila Activity.
 Home-page: https://github.com/azzhu/EasyFlyTracker
 Author: azzhu
 Author-email: zhu.qingjie@qq.com
 License: MIT
 Project-URL: Source Code, https://github.com/azzhu/EasyFlyTracker
 Project-URL: Bug Tracker, https://github.com/azzhu/EasyFlyTracker/issues
```

### Comparing `easyFlyTracker-0.9.2/easyFlyTracker.egg-info/SOURCES.txt` & `easyFlyTracker-0.9.3/easyFlyTracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easyFlyTracker-0.9.2/setup.py` & `easyFlyTracker-0.9.3/setup.py`

 * *Files identical despite different names*

