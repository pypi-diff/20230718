# Comparing `tmp/desy-mento-0.1.5.tar.gz` & `tmp/desy-mento-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/fs-sc/mento/dist/.tmp-_hbgyh0f/desy-mento-0.1.5.tar", last modified: Fri Jul  7 14:36:52 2023, max compression
+gzip compressed data, was "/builds/fs-sc/mento/dist/.tmp-ctaco6zk/desy-mento-0.2.1.tar", last modified: Tue Jul 18 12:48:15 2023, max compression
```

## Comparing `desy-mento-0.1.5.tar` & `desy-mento-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/
--rw-r--r--   0 root         (0) root         (0)      664 2023-07-07 14:36:52.000000 desy-mento-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6809 2023-07-07 14:36:33.000000 desy-mento-0.1.5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-07 14:36:52.000000 desy-mento-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-07-07 14:36:33.000000 desy-mento-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/
--rw-r--r--   0 root         (0) root         (0)      664 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/mento/
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11594 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11937 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)     9696 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     8285 2023-07-07 14:36:33.000000 desy-mento-0.1.5/tests/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     5242 2023-07-07 14:36:33.000000 desy-mento-0.1.5/tests/test_trigger.py
--rw-rw-rw-   0 root         (0) root         (0)     3684 2023-07-07 14:36:33.000000 desy-mento-0.1.5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:15.000000 desy-mento-0.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:15.000000 desy-mento-0.2.1/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    34670 2023-07-18 12:47:51.000000 desy-mento-0.2.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)    44408 2023-07-18 12:48:15.000000 desy-mento-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-18 12:47:51.000000 desy-mento-0.2.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-07-18 12:47:51.000000 desy-mento-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 12:48:15.000000 desy-mento-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/desy_mento.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    44408 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/desy_mento.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/desy_mento.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/desy_mento.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/desy_mento.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/desy_mento.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:15.000000 desy-mento-0.2.1/src/mento/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-18 12:47:51.000000 desy-mento-0.2.1/src/mento/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11512 2023-07-18 12:47:51.000000 desy-mento-0.2.1/src/mento/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11929 2023-07-18 12:47:51.000000 desy-mento-0.2.1/src/mento/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     9725 2023-07-18 12:47:51.000000 desy-mento-0.2.1/src/mento/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:15.000000 desy-mento-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7838 2023-07-18 12:47:51.000000 desy-mento-0.2.1/tests/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5261 2023-07-18 12:47:51.000000 desy-mento-0.2.1/tests/test_trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3684 2023-07-18 12:47:51.000000 desy-mento-0.2.1/tests/test_utils.py
```

### Comparing `desy-mento-0.1.5/README.rst` & `desy-mento-0.2.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 Here is a minimum working example::
 
     from mento import Trigger
 
     my_trigger = Trigger()  # default trigger will submit Slurm jobs on an HPC node
 
     my_analysis = 'maxwell_program.exe'  # path to analysis program available on Maxwell
+
     my_args = ['analysis', 'parameters', 'list', 'inputdatafile']  # arguments required by analysis program, including input data
 
     my_trigger.run([my_analysis, my_args])  # connect to a remote machine with appropriate credentials and start the analysis job there
 
 
 Note that paths to input data files and output directories can be specified as you see them at
 the beamline, and they will be automagically found in the remote core filesystem on Maxwell.
```

### Comparing `desy-mento-0.1.5/src/mento/metadata.py` & `desy-mento-0.2.1/src/mento/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,49 +104,52 @@
     beamtime: str
     corefs_path: str
     tag: str  # 'current' or 'commissioning'
     online: Optional[OnlineInfo] = None
     asapo: Optional[AsapoInfo] = None
 
 
+def get_active_session_root(root_dir='/gpfs') -> Path:
+    top_dir = Path(root_dir)
+    possible_beamtime = top_dir/'current'
+    possible_commissioning = top_dir/'commissioning'
+
+    if possible_beamtime.exists() and possible_beamtime.is_dir():
+        return possible_beamtime
+    elif possible_commissioning.exists() and possible_commissioning.is_dir():
+        return possible_commissioning
+    elif not top_dir.exists():
+        raise FileNotFoundError(f'{top_dir} not found')
+    else:
+        raise FileNotFoundError(f'No user beamtime or commissioning directory found under {root_dir}')
+
+
 # Unclear what type hint to provide when a function argument is a path. typing.Union[str, bytes, os.Pathlike]?
-def locate_metadata_file(root_dir='/gpfs/current') -> str:
+def locate_metadata_file(root_dir='/gpfs') -> str:
     """
-    Get the path to the metadata JSON file for the current beamtime
-
-    This function only works in the online situation where there is a currently
-    running beamtime.
+    Get the path to the metadata JSON file for the currently active beamtime or commissioning run
 
-    :param root_dir: top directory of beamtime
-    :returns: full path to metadata JSON file provided for the current beamtime
+    :param root_dir: parent directory of current session, usually '/gpfs'
+    :returns: full path to metadata JSON file provided for the current beamtime/commissioning run
     """
     # root_dir for beamline filesystems is, AFAIK, always '/gpfs' at PETRA III
     # /gpfs/local is always present, we want to ignore it. Normally there should be
     # either a /gpfs/current, or /gpfs/commissioning subdirectory (sometimes both).
     # The metadata file should be located directly in this subdirectory
     # When both 'current' and 'commissioning' directories are present, we usually want the 'current'
-    # directory corresponding to the user beamtime. Hence the default parameter value.
-    root_dir = Path(root_dir)
-    try:
-        beamtime_dirs = [path for path in root_dir.iterdir()
-                         if path.is_dir() and (path.name != 'local')]
-    except FileNotFoundError:  # if root_dir does not exist
-        raise FileNotFoundError(f'Root directory not found: {root_dir}')
-    metadata_files = []
-    for curr_dir in beamtime_dirs + [root_dir]:  # also check root_dir, in case the root directory contains a metadata file (e..g when root_dir = '/gpfs/current')
-        curr_dir_metadata_files = list(curr_dir.glob('*metadata*.json'))
-        metadata_files.extend(curr_dir_metadata_files)  # if there happens to be more than one directory with a metadata json file - which is BAD
+    # directory corresponding to the user beamtime.
+    currently_active_dir = get_active_session_root(root_dir)
+    metadata_files = list(currently_active_dir.glob('*metadata*.json'))
     num_metadata_files = len(metadata_files)
     if num_metadata_files == 1:  # Desired case, with specific user or commissioning run
         return str(metadata_files[0])
     elif num_metadata_files == 0:  # No metadata file is found
-        raise FileNotFoundError(f'Metadata file not found under {root_dir}')
-    elif num_metadata_files > 1:  # Both user run and commissioning directories present, AND root=/gpfs
-        # A more specific root_dir is needed, to have a unique metadata file
-        raise RuntimeError(f'Multiple metadata files found under {root_dir}')
+        raise FileNotFoundError(f'Metadata file not found under {currently_active_dir}')
+    elif num_metadata_files > 1:  # IT only writes one *metadata*.json at startBeamtime/startCommissioning. so this shouldn't happen
+        raise RuntimeError(f'Multiple metadata files found under {currently_active_dir}')
 
 
 # Unclear what type hint to provide when a function argument is a path. typing.Union[str, bytes, os.Pathlike]?
 def parse_metadata_file(metadatafile_path) -> BeamtimeMetadata:
     """
     Parse beamtime metadata file to get information relevant to current beamtime and online analysis.
 
@@ -231,15 +234,15 @@
             raise FileNotFoundError(f'File not found (but mentioned in metadata): {asapo_info.token_rw}')
     return BeamtimeMetadata(beamline=beamline, beamtime=beamtime,
                             corefs_path=corefs_path, tag=tag,
                             online=online_info, asapo=asapo_info)
 
 
 # Unclear what type hint to provide when a function argument is a path. typing.Union[str, bytes, os.Pathlike]?
-def get_beamtime_metadata(root_dir='/gpfs/current') -> BeamtimeMetadata:
+def get_beamtime_metadata(root_dir='/gpfs') -> BeamtimeMetadata:
     """
     Convenience function to load partial beamtime metadata relevant for online analysis.
 
     Automatically finds a metadata file and parses it for information required for online analysis.
 
     :param root_dir: top directory for beamtime
     :returns: tuple containing 'relevant' metadata for later use in online analysis
```

### Comparing `desy-mento-0.1.5/src/mento/trigger.py` & `desy-mento-0.2.1/src/mento/trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class Trigger:
     """
     Collective information needed to trigger an online analysis run.
 
     Information about access to remote online computing resources
     """
     # Unclear what type hint to provide when a function argument is a path. typing.Union[str, bytes, os.Pathlike]?
-    def __init__(self, trigger_method=TriggerMethod.REMOTE_SBATCH_SCRIPT, beamline_root_dir='/gpfs/current'):
+    def __init__(self, trigger_method=TriggerMethod.REMOTE_SBATCH_SCRIPT, beamline_root_dir='/gpfs'):
         """
         Construct a Trigger object with relevant information for remote computing resource access.
 
         :param trigger_method: method to use for triggering processing, either locally or remotely
         :param beamline_root_dir: full path to root directory of beamline filesystem
         """
         self.bt_info = get_beamtime_metadata(root_dir=beamline_root_dir)
```

### Comparing `desy-mento-0.1.5/src/mento/utils.py` & `desy-mento-0.2.1/src/mento/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,20 +149,20 @@
     make_writable_dir(results_dir)  # creates directory with 777 permissions
     results_filename = _name_resultfile_with_suffix(data_file_path, '_results')
     results_file_path = Path(results_dir, results_filename)  # Note: results_filename doesn't exist at this point
 
     return str(results_file_path)
 
 
-def get_path_core(local_path, remote_dir):
-    return _map_local_to_remote_path(local_path, remote_dir, 'raw')
+def get_path_core(local_path, remote_dir, split_at='raw'):
+    return _map_local_to_remote_path(local_path, remote_dir, split_at)
 
 
-def get_path_mountpoint(local_path, remote_dir, tag='current'):
-    remote_dir = Path(remote_dir, tag)
+def get_path_mountpoint(local_path, remote_dir, split_at='current'):
+    remote_dir = Path(remote_dir, split_at)
     return _map_local_to_remote_path(local_path, str(remote_dir), 'processed')
 
 
 def run_subprocess(arg_list: list) -> None:
     """
     Use Python's subprocess module to run a command with arguments.
```

### Comparing `desy-mento-0.1.5/tests/test_metadata.py` & `desy-mento-0.2.1/tests/test_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 import pytest
 
 bad_files_root = Path('tests/data/gpfs/local')
 incomplete_metadata_file = bad_files_root / 'incomplete-metadata-12345678.json'
 noonline_metadata_file = bad_files_root / 'noonline-metadata-12345678.json'
 noonlinenoasapo_metadata_file = bad_files_root / 'noonlinenoasapo-metadata-12345678.json'
 
-beamtime_root = Path('tests/data/gpfs/current')
+beamline_root = Path('tests/data/gpfs')
+active_root = beamline_root / 'current'
 complete_metadata_file = 'beamtime-metadata-12345678.json'
 sshkey_path = 'shared/id_rsa'
 asapo_token_ro = 'shared/asapo-token-clbt.txt'
 asapo_token_rw = 'shared/asapo-token.txt'
 
-ssh = SSHInfo(user='bttest01', key=str((beamtime_root / sshkey_path).resolve()))
+ssh = SSHInfo(user='bttest01', key=str((active_root / sshkey_path).resolve()))
 slurm = SlurmInfo(partition='ponline', reservation='12345678')
-asapo = AsapoInfo(token_ro=str((beamtime_root / asapo_token_ro).resolve()),
-                  token_rw=str((beamtime_root / asapo_token_rw).resolve()),
+asapo = AsapoInfo(token_ro=str((active_root / asapo_token_ro).resolve()),
+                  token_rw=str((active_root / asapo_token_rw).resolve()),
                   endpoint='asapo-ps-0.desy.de:8400')
 online = OnlineInfo(ssh=ssh, slurm=slurm,
                     nodes=['hpc01', 'hpc02'],
                     blfs_mountpoint='/beamline/p9999')
 bt_info = BeamtimeMetadata(beamline='p9999', beamtime='12345678',
                            corefs_path='/asap3/petra3/gpfs/', tag='current',
                            online=online, asapo=asapo)
@@ -98,50 +99,40 @@
                                        corefs_path='remote/data/dir', tag='current')
 
     # Shows keyword args keep the code robust, users don't need to remember positions
     assert test_bt_info_01 == test_bt_info_02
 
 
 def test_locate_metadata_file_success():
-    root_dir = 'tests/data/gpfs'
-    assert locate_metadata_file(root_dir) == str(beamtime_root / complete_metadata_file)
+    assert locate_metadata_file(beamline_root) == str(active_root / complete_metadata_file)
 
 
-def test_locate_metadata_file_bad_root():
+def test_locate_metadata_file_nonexistent_root():
     bad_root_dir = '/non/existent/path'
-    with pytest.raises(FileNotFoundError, match='Root directory not found'):
+    with pytest.raises(FileNotFoundError):
         _ = locate_metadata_file(bad_root_dir)
 
 
-def test_locate_metadata_file_no_file():
+def test_locate_metadata_file_wrong_dir_structure():
     bad_root_dir = 'tests/data'
-    with pytest.raises(FileNotFoundError, match='Metadata file not found'):
+    with pytest.raises(FileNotFoundError):
         _ = locate_metadata_file(bad_root_dir)
 
 
-def test_locate_metadata_file_multiple_files(tmp_beamtime_dirtree, tmp_path):
-    # Ensure multiple metadata files appear under tmp_path
-    # by temporarily duplicating entire directory tree
-    tmp_beamtime_dirtree('current')
-    tmp_beamtime_dirtree('commissioning')
-    with pytest.raises(RuntimeError, match='Multiple metadata files found'):
-        _ = locate_metadata_file(tmp_path)
-
-
 def test_locate_metadata_file_ignore_local_dir(tmp_beamtime_dirtree, tmp_path):
     # Ensure multiple metadata files appear under tmp_path
     # by temporarily duplicating entire directory tree
     # But the directory tree under 'local' should be ignored
     tmp_beamtime_dirtree('current')
     tmp_beamtime_dirtree('local')
     assert locate_metadata_file(tmp_path) == str(tmp_path / 'current' / complete_metadata_file)
 
 
 def test_parse_metadata_file_success():
-    test_bt_info = parse_metadata_file(beamtime_root / complete_metadata_file)
+    test_bt_info = parse_metadata_file(active_root / complete_metadata_file)
     assert test_bt_info == bt_info
 
 
 def test_parse_metadata_file_no_online_no_asapo():
     test_bt_info = parse_metadata_file(noonlinenoasapo_metadata_file)
     assert test_bt_info.online is None  # valid field value for BeamtimeMetadata.online
     assert test_bt_info.asapo is None  # valid field value for BeamtimeMetadata.asapo
@@ -166,15 +157,15 @@
     with pytest.raises(FileNotFoundError, match='Metadata file not found'):
         _ = parse_metadata_file(nonexistent_file)
 
 
 def test_parse_metadata_file_bad_format():
     not_json_file = sshkey_path  # empty file, obviously not JSON
     with pytest.raises(ValueError, match='Parsing of metadata file failed'):
-        _ = parse_metadata_file(beamtime_root / not_json_file)
+        _ = parse_metadata_file(active_root / not_json_file)
 
 
 def test_parse_metadata_file_missing_keys():
     with pytest.raises(ValueError, match='Required metadata not found'):
         _ = parse_metadata_file(incomplete_metadata_file)
```

### Comparing `desy-mento-0.1.5/tests/test_trigger.py` & `desy-mento-0.2.1/tests/test_trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,22 +65,22 @@
     with pytest.raises(FileNotFoundError):
         test_trigger.run([script_file])
 
 
 def test_trigger_run_local_bash_script_success(tmp_beamtime_dirtree):
     sample_bash_script = 'tests/data/gpfs/local/dump_args_to_file_bash.sh'
     # Create temporary directory tree as scratch space for bash script, output, etc.
-    tmp_beamtime_root = tmp_beamtime_dirtree('scratch')
+    tmp_beamtime_root = tmp_beamtime_dirtree('commissioning')
     local_bash_script = copy(sample_bash_script, tmp_beamtime_root)
     local_bash_log = Path(local_bash_script).with_suffix('.log')
     local_args = [5, 'dummy', 'arguments', 'to script', 0]
     arg_list_string = ' '.join(str(item) for item in local_args)
 
     test_trigger = Trigger(trigger_method=TriggerMethod.LOCAL_BASH_SCRIPT,
-                           beamline_root_dir=tmp_beamtime_root)
+                           beamline_root_dir=Path(tmp_beamtime_root).parent)
     test_trigger.run([local_bash_script, local_args])
 
     # Let the bash script finish before asserting if script log file exists
     assert _poll_with_timeout(lambda: local_bash_log.exists())
     with open(local_bash_log, 'r') as f:
         local_bash_output = f.readline().rstrip()
     assert local_bash_output == arg_list_string
```

### Comparing `desy-mento-0.1.5/tests/test_utils.py` & `desy-mento-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

