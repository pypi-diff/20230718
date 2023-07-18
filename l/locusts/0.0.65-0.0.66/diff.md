# Comparing `tmp/locusts-0.0.65.tar.gz` & `tmp/locusts-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/TMB-CSB/Sarti/Work/locusts_pkg/dist/tmp6n944r6c/locusts-0.0.65.tar", last modified: Fri Nov  4 09:15:26 2022, max compression
+gzip compressed data, was "/data/TMB-CSB/Sarti/Work/locusts_pkg/dist/.tmp-zqiglycz/locusts-0.0.66.tar", last modified: Tue Jul 18 13:07:31 2023, max compression
```

## Comparing `locusts-0.0.65.tar` & `locusts-0.0.66.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-x---   0 sartie   (200184947) sartie   (200184947)        0 2022-11-04 09:15:26.000000 locusts-0.0.65/
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     1074 2020-10-04 13:43:43.000000 locusts-0.0.65/LICENSE
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      140 2020-11-24 18:17:40.000000 locusts-0.0.65/MANIFEST.in
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     7250 2022-11-04 09:15:26.000000 locusts-0.0.65/PKG-INFO
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     6034 2020-10-17 23:43:16.000000 locusts-0.0.65/README.md
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      104 2021-02-08 19:14:59.000000 locusts-0.0.65/pyproject.toml
--rw-r-----   0 sartie   (200184947) sartie   (200184947)       38 2022-11-04 09:15:26.000000 locusts-0.0.65/setup.cfg
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     2106 2020-09-11 14:54:56.000000 locusts-0.0.65/setup.py
-drwxr-x---   0 sartie   (200184947) sartie   (200184947)        0 2022-11-04 09:15:26.000000 locusts-0.0.65/src/
-drwxr-x---   0 sartie   (200184947) sartie   (200184947)        0 2022-11-04 09:15:26.000000 locusts-0.0.65/src/locusts/
--rw-r-----   0 sartie   (200184947) sartie   (200184947)       23 2022-11-04 09:15:06.000000 locusts-0.0.65/src/locusts/__init__.py
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      124 2021-03-16 00:17:06.000000 locusts-0.0.65/src/locusts/data_transfer_protocol.sh
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     7934 2021-04-22 09:30:56.000000 locusts-0.0.65/src/locusts/environment.py
--rwxr-x---   0 sartie   (200184947) sartie   (200184947)     2504 2021-05-03 22:40:39.000000 locusts-0.0.65/src/locusts/inner_template_manager.txt
--rwxr-x---   0 sartie   (200184947) sartie   (200184947)    57255 2022-11-04 09:14:16.000000 locusts-0.0.65/src/locusts/manager.py
--rwxr-x---   0 sartie   (200184947) sartie   (200184947)      730 2021-06-05 15:50:01.000000 locusts-0.0.65/src/locusts/outer_template_manager.txt
--rw-rw----   0 sartie   (200184947) sartie   (200184947)     5931 2022-08-19 17:56:29.000000 locusts-0.0.65/src/locusts/support.py
--rw-r-----   0 sartie   (200184947) sartie   (200184947)    11287 2022-10-15 09:46:32.000000 locusts-0.0.65/src/locusts/swarm.py
-drwxr-x---   0 sartie   (200184947) sartie   (200184947)        0 2022-11-04 09:15:26.000000 locusts-0.0.65/src/locusts.egg-info/
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     7250 2022-11-04 09:15:26.000000 locusts-0.0.65/src/locusts.egg-info/PKG-INFO
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      427 2022-11-04 09:15:26.000000 locusts-0.0.65/src/locusts.egg-info/SOURCES.txt
--rw-r-----   0 sartie   (200184947) sartie   (200184947)        1 2022-11-04 09:15:26.000000 locusts-0.0.65/src/locusts.egg-info/dependency_links.txt
--rw-r-----   0 sartie   (200184947) sartie   (200184947)        8 2022-11-04 09:15:26.000000 locusts-0.0.65/src/locusts.egg-info/top_level.txt
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     1074 2020-10-04 13:43:43.000000 locusts-0.0.66/LICENSE
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      140 2020-11-24 18:17:40.000000 locusts-0.0.66/MANIFEST.in
+-rw-r--r--   0 sartie   (200184947) sartie   (200184947)     7250 2023-07-18 13:07:31.000000 locusts-0.0.66/PKG-INFO
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     6034 2020-10-17 23:43:16.000000 locusts-0.0.66/README.md
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      104 2021-02-08 19:14:59.000000 locusts-0.0.66/pyproject.toml
+-rw-r--r--   0 sartie   (200184947) sartie   (200184947)       38 2023-07-18 13:07:31.000000 locusts-0.0.66/setup.cfg
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     2106 2020-09-11 14:54:56.000000 locusts-0.0.66/setup.py
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/src/
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts/
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)       23 2023-07-18 13:07:11.000000 locusts-0.0.66/src/locusts/__init__.py
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      158 2023-03-15 16:41:53.000000 locusts-0.0.66/src/locusts/data_transfer_protocol.sh
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     7934 2021-04-22 09:30:56.000000 locusts-0.0.66/src/locusts/environment.py
+-rwxr-x---   0 sartie   (200184947) sartie   (200184947)     2504 2021-05-03 22:40:39.000000 locusts-0.0.66/src/locusts/inner_template_manager.txt
+-rwxr-x---   0 sartie   (200184947) sartie   (200184947)    55729 2023-03-01 15:34:55.000000 locusts-0.0.66/src/locusts/manager.py
+-rwxr-x---   0 sartie   (200184947) sartie   (200184947)      730 2021-06-05 15:50:01.000000 locusts-0.0.66/src/locusts/outer_template_manager.txt
+-rw-rw----   0 sartie   (200184947) sartie   (200184947)     5931 2022-08-19 17:56:29.000000 locusts-0.0.66/src/locusts/support.py
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)    11287 2022-10-15 09:46:32.000000 locusts-0.0.66/src/locusts/swarm.py
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     7250 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/PKG-INFO
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      427 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/SOURCES.txt
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)        1 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/dependency_links.txt
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)        8 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/top_level.txt
```

### Comparing `locusts-0.0.65/LICENSE` & `locusts-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/PKG-INFO` & `locusts-0.0.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locusts
-Version: 0.0.65
+Version: 0.0.66
 Summary: Distributes many short tasks on multicore and hpc systems
 Home-page: https://github.com/pypa/sampleproject
 Author: Edoardo Sarti
 Author-email: edoardo.sarti@gmail.com
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
```

### Comparing `locusts-0.0.65/README.md` & `locusts-0.0.66/README.md`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/setup.py` & `locusts-0.0.66/setup.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/src/locusts/environment.py` & `locusts-0.0.66/src/locusts/environment.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/src/locusts/inner_template_manager.txt` & `locusts-0.0.66/src/locusts/inner_template_manager.txt`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/src/locusts/manager.py` & `locusts-0.0.66/src/locusts/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -548,97 +548,22 @@
         # Start/stop chronometer
         for job_id, task_list in tasks_per_job:
             if chrono_on[job_id] and not time_start[job_id]:
                 time_start[job_id] = time.time()
             if not chrono_on[job_id] and time_start[job_id]:
                 time_end[job_id] = time.time()
 
-        """
-        if protocol != 'local':
-            manager_cmd = ["ssh", remote_machine, "bash", fs_locations["runtime_exec"] + 'periodic_check.sh']
-            smallscp_cmd = ["bash", data_transfer_protocol, "{0}:{1}".format(remote_machine, fs_locations["runtime_exec"] + 'periodic_check.log.txt'), log_folder]
-        else:
-            manager_cmd = ["bash", fs_locations["build_exec"] + 'periodic_check.sh']
-            smallscp_cmd = ["cp", "{0}".format(fs_locations["runtime_exec"] + 'periodic_check.log.txt'), log_folder]
-
-        if DEBUG:
-            print("COMMAND", " ".join(manager_cmd))
-            p = subprocess.Popen(
-                manager_cmd,
-                stdout=subprocess.PIPE
-            )
-        else:
-            p = subprocess.Popen(
-                manager_cmd, 
-                stderr=devnull, 
-                stdout=subprocess.PIPE
-           )
-        p.wait()
-        if DEBUG:
-            print("COMMAND", " ".join(smallscp_cmd))
-            p = subprocess.Popen(
-                smallscp_cmd,
-                stdout=subprocess.PIPE
-            )
-        else:
-            p = subprocess.Popen(
-                smallscp_cmd, 
-                stderr=devnull, 
-                stdout=subprocess.PIPE
-           )
-        p.wait()
-        """
-
         if protocol != 'local':
             jh_cmd = ["ssh", "-t", remote_machine, "bash", fs_locations["runtime_exec"] + 'submit_status.sh']
             jhcp_cmd = ["bash", data_transfer_protocol, "{0}:{1}".format(remote_machine, fs_locations["runtime_exec"] + 'submit_status.log'), log_folder]
+            jhcp2_cmd = ["bash", data_transfer_protocol, "{0}:{1}".format(remote_machine, fs_locations["runtime_exec"] + 'submit.log'), log_folder]
         else:
             jh_cmd = ["bash", fs_locations["build_exec"] + 'submit_status.sh']
             jhcp_cmd = ["cp", "{0}".format(fs_locations["runtime_exec"] + 'submit_status.log'), log_folder]
-
-
-        """
-        mng_lines, mac_lines, status_lines, time_line = False, False, False, False
-        mng_times, mac_names = [], []
-        with open(log_folder + '/periodic_check.log.txt') as logf:
-            print("OPENING", log_folder + '/periodic_check.log.txt')
-            for line in logf:
-                if not line.strip():
-                    continue
-                if line == "MANAGERS":
-                    mng_lines = True
-                    continue
-                elif line == "MACNAMES":
-                    mng_lines = False
-                    mac_lines = True
-                    continue
-                elif line == "STATUS":
-                    mac_lines = False
-                    status_lines = True
-                    continue
-                elif line == "TIME":
-                    status_lines = False
-                    time_line = True
-                    continue
-                if mng_lines:
-                    mng_times.append(line.strip())
-                elif mac_lines:
-                    mac_names.append(line.strip()) 
-                elif status_lines:
-#                    print(line)
-                    if line.split()[2] in [batch_job_code + str(x[0]).zfill(3) for x in tasks_per_job]:
-#                        print("YE", line)
-                        status[int(line.split()[2][len(batch_job_code):])] = line.split()[4]
-                        hasrun[int(line.split()[2][len(batch_job_code):])] = True
-                elif time_line:
-                    real_time = line.strip()
-                    real_time = int(real_time.split(":")[0])*60 + int(real_time.split(":")[1])
-            if (not (mng_times and mac_names)) and (not no_entry):
-                print("STILL NO CACHE FILES: CHECKING STATUS")
-        """
+            jhcp2_cmd = ["cp", "{0}".format(fs_locations["runtime_exec"] + 'submit.log'), log_folder]
 
         if DEBUG:
             print("COMMAND", " ".join(jh_cmd))
             p = subprocess.Popen(
                 jh_cmd,
                 stdout=subprocess.PIPE
             )
@@ -659,62 +584,102 @@
         else:
             p = subprocess.Popen(
                 jhcp_cmd,
                 stderr=devnull,
                 stdout=subprocess.PIPE
            )
         p.wait()
-        
+        time.sleep(30)
+        if DEBUG:
+            print("COMMAND", " ".join(jhcp2_cmd))
+            p = subprocess.Popen(
+                jhcp_cmd2,
+                stdout=subprocess.PIPE
+            )
+        else:
+            p = subprocess.Popen(
+                jhcp_cmd2,
+                stderr=devnull,
+                stdout=subprocess.PIPE
+           )
+        p.wait()
  
         all_completed = True
+        resubmit_IDs = []
         with open(log_folder + "/submit_status.log") as ssf:
             for fline in ssf:
                 if fline.strip():
                     print(fline.strip())
                     fields = fline.split()
-                    if not ((only_gather and (len(fields) <2 or fields[1] == "COMPLETED" or fields[1] == "CANCELLED")) or fields[1] == "COMPLETED"):
+                    if not ((only_gather and (len(fields) <2 or fields[1] == "COMPLETED" or fields[1] == "CANCELLED")) or fields[1] == "COMPLETED" or fields[1] == "TIMEOUT" or fields[1] == "NODE_FAIL"):
                         all_completed = False
                         nocache_count += 1
+                        if fields[1] == "NODE_FAIL":
+                            resubmit_IDs.append(fields[0])
         time.sleep(10)
+        id_to_jobname = {}
+        with open(log_folder + "/submit.log") as ssf:
+            for fline in ssf:
+                if fline.strip():
+                    fields = fline.split()
+                    id_to_jobname[fields[1]] = fields[0]
+
+        resubmit_jobnames = []
+        for i in resubmit_IDs:
+            resubmit_jobnames.append(id_to_jobname[i])
+
+        if resubmit_jobnames:
+            if protocol != 'local':
+                rsb_cmd = 'ssh -t {0} grep "'.format(remote_machine) + "\|".join(resubmit_jobnames) + '" {0}/submit.sh > {0}/resubmit.sh'.format(fs_locations["build_exec"])
+
+                if DEBUG:
+                    print("COMMAND", " ".join(rsb_cmd))
+                    p = subprocess.Popen(
+                        rsb_cmd,
+                        stdout=subprocess.PIPE
+                    )
+                else:
+                    p = subprocess.Popen(
+                        rsb_cmd,
+                        stderr=devnull,
+                        stdout=subprocess.PIPE
+                    )
+                p.wait()
+                time.sleep(40)
+
+                chk_cmd = [
+                "ssh",
+                remote_machine,
+                "bash",
+                fs_locations["runtime_exec"] + 'resubmit.sh'
+                ]
+                if DEBUG:
+                    print("COMMAND", " ".join(chk_cmd))
+                    p = subprocess.Popen(chk_cmd)
+                else:
+                    p = subprocess.Popen(chk_cmd,
+                        stderr=devnull,
+                        stdout=devnull
+                    )
+                p.wait()
+                time.sleep(20)
+                all_completed = False
+
+                print("Resubmitting jobs", resubmit_jobnames)
+            else:
+                pass
+
+
         if not (all_completed): #and (nocache_count < NOCACHE_COUNT_THR):
             print("Incomplete jobs are present. Check number", nocache_count)
             is_over = False
             continue
         else:
             print("All jobs have been completed")
 
-        """        
-        for it, t in enumerate(tasks_per_job):
-            job_id, task_list = t
-
-            if len(mng_times[it].split()) == 1:
-                job_times[job_id] = int(mng_times[it].split(":")[0])*60 + int(mng_times[it].split(":")[1])
-#            else:
-#                print("WARNING: missing manager", it, job_id, mng_times[it])
-
-            if len(mac_names[it].split()) == 1:
-                machine_names[job_id] = mac_names[it]
-#            else:
-#                print("WARNING: missing machine name", it, job_id, mac_names[it])
-
-            if status[job_id]:
-                print(job_id, "Status:", status[job_id])
-                is_over = False
-            elif not hasrun[job_id]:
-                print(job_id, "Waiting to be queued ({0}/3)".format(wc+1))
-                wc += 1
-                if wc > 3:
-                    print(job_id, "Abort")
-                else:
-                    is_over = False
-            else:
-                print(job_id, "End")
-                time_end[job_id] = job_times[job_id]
-        """
-
     log_txt = "\n\n#LOCUSTS JOBS LOG\n"
     time_now = time.time()
     tot_runtime, totsq = 0, 0
     for job_id, task_list in tasks_per_job:
         if not time_end[job_id] - time_start[job_id] == 0:
             runtime = waiting_time/2
         else: 
@@ -957,15 +922,15 @@
             if priv.startswith('-'):  # If item is not a folder
                 snapshot[dirname][filename] = (priv, usr1, usr2, s, d1, d2, d3)
         elif len(line.split()) == 11 and line[9].split() == "->":
             priv, _, usr1, usr2, s, d1, d2, d3, filename, _, slink = line.split()
             filename = filename.replace(root_dir,"")
             snapshot["::NEGLECT::"].append(filename)
         else:
-            print(("WARNING (take_snapshot): output of ls -ltrhR is not"
+            print(("WARNING (take_snapshot): output of ls -ltrhR is not "
                 "in the expected format"))
             print(line)
 
     return snapshot
 
 
 def compare_snapshots(snap1, snap2):
```

### Comparing `locusts-0.0.65/src/locusts/outer_template_manager.txt` & `locusts-0.0.66/src/locusts/outer_template_manager.txt`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/src/locusts/support.py` & `locusts-0.0.66/src/locusts/support.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/src/locusts/swarm.py` & `locusts-0.0.66/src/locusts/swarm.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.65/src/locusts.egg-info/PKG-INFO` & `locusts-0.0.66/src/locusts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locusts
-Version: 0.0.65
+Version: 0.0.66
 Summary: Distributes many short tasks on multicore and hpc systems
 Home-page: https://github.com/pypa/sampleproject
 Author: Edoardo Sarti
 Author-email: edoardo.sarti@gmail.com
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
```

