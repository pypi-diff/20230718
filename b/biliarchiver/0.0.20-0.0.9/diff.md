# Comparing `tmp/biliarchiver-0.0.20.tar.gz` & `tmp/biliarchiver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biliarchiver-0.0.20.tar", max compression
+gzip compressed data, was "biliarchiver-0.0.9.tar", max compression
```

## Comparing `biliarchiver-0.0.20.tar` & `biliarchiver-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,13 @@
--rw-r--r--   0        0        0      131 2023-07-07 09:38:51.631616 biliarchiver-0.0.20/README.md
--rw-r--r--   0        0        0     9388 2023-07-18 04:44:07.535293 biliarchiver-0.0.20/biliarchiver/_biliarchiver_upload_bvid.py
--rw-r--r--   0        0        0     9224 2023-07-07 09:38:51.631616 biliarchiver-0.0.20/biliarchiver/archive_bvid.py
--rw-r--r--   0        0        0     7211 2023-07-18 04:24:04.652661 biliarchiver-0.0.20/biliarchiver/cli_tools/bili_archive_bvids.py
--rw-r--r--   0        0        0     4133 2023-07-07 09:38:51.635616 biliarchiver-0.0.20/biliarchiver/cli_tools/bili_get_bvids.py
--rw-r--r--   0        0        0     1845 2023-07-18 04:24:04.652661 biliarchiver-0.0.20/biliarchiver/cli_tools/bili_upload.py
--rw-r--r--   0        0        0      413 2023-07-07 09:38:51.635616 biliarchiver-0.0.20/biliarchiver/cli_tools/biliarchiver.py
--rw-r--r--   0        0        0     2139 2023-07-07 09:38:51.635616 biliarchiver-0.0.20/biliarchiver/config.py
--rw-r--r--   0        0        0      194 2023-07-07 09:38:51.635616 biliarchiver-0.0.20/biliarchiver/exception.py
--rw-r--r--   0        0        0     2724 2023-07-07 09:38:51.635616 biliarchiver-0.0.20/biliarchiver/utils/dirLock.py
--rw-r--r--   0        0        0      237 2023-07-07 09:38:51.635616 biliarchiver-0.0.20/biliarchiver/utils/ffmpeg.py
--rw-r--r--   0        0        0     1085 2023-07-18 04:24:04.652661 biliarchiver-0.0.20/biliarchiver/utils/http_patch.py
--rw-r--r--   0        0        0     1278 2023-07-07 09:38:51.635616 biliarchiver-0.0.20/biliarchiver/utils/string.py
--rw-r--r--   0        0        0       32 2023-07-18 04:52:44.755864 biliarchiver-0.0.20/biliarchiver/version.py
--rw-r--r--   0        0        0      665 2023-07-18 04:52:52.943937 biliarchiver-0.0.20/pyproject.toml
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 biliarchiver-0.0.20/setup.py
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 biliarchiver-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-06 20:05:41.529385 biliarchiver-0.0.9/README.md
+-rw-r--r--   0        0        0     7575 2023-06-06 19:48:46.123664 biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py
+-rw-r--r--   0        0        0     7157 2023-06-06 19:12:07.431306 biliarchiver-0.0.9/biliarchiver/archive_bvid.py
+-rw-r--r--   0        0        0     4734 2023-06-07 04:48:33.598085 biliarchiver-0.0.9/biliarchiver/bili_archive_bvids.py
+-rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py
+-rw-r--r--   0        0        0     1490 2023-06-07 04:52:11.184454 biliarchiver-0.0.9/biliarchiver/bili_uploade.py
+-rw-r--r--   0        0        0     2018 2023-06-06 19:20:55.302758 biliarchiver-0.0.9/biliarchiver/config.py
+-rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.9/biliarchiver/utils/dirLock.py
+-rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.9/biliarchiver/utils/string.py
+-rw-r--r--   0        0        0       31 2023-06-06 19:35:41.648702 biliarchiver-0.0.9/biliarchiver/version.py
+-rw-r--r--   0        0        0      530 2023-06-07 04:58:02.482737 biliarchiver-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/setup.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/PKG-INFO
```

### Comparing `biliarchiver-0.0.20/biliarchiver/_biliarchiver_upload_bvid.py` & `biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 import json
 import os
 from pathlib import Path
 import time
-from typing import List
 from internetarchive import get_item
 from requests import Response
 from rich import print
-from biliarchiver.exception import VideosBasePathNotFoundError
 
 from biliarchiver.utils.string import human_readable_upper_part_map
 from biliarchiver.config import BILIBILI_IDENTIFIER_PERFIX, config
 from biliarchiver.utils.dirLock import UploadLock, AlreadyRunningError
 from biliarchiver.version import BILI_ARCHIVER_VERSION
 
-def upload_bvid(bvid: str, *, update_existing: bool = False):
+def upload_bvid(bvid):
     try:
         lock_dir = config.storage_home_dir / '.locks' / bvid
         os.makedirs(lock_dir, exist_ok=True)
         with UploadLock(lock_dir): # type: ignore
-            _upload_bvid(bvid, update_existing=update_existing)
+            _upload_bvid(bvid)
     except AlreadyRunningError:
         print(f'已经有一个上传 {bvid} 的进程在运行，跳过')
-    except VideosBasePathNotFoundError:
-        print(f'没有找到 {bvid} 对应的文件夹。可能是因已存在 IA item 而跳过了下载，或者你传入了错误的 bvid')
     except Exception as e:
         print(f'上传 {bvid} 时出错：')
         raise e
 
-def _upload_bvid(bvid: str, *, update_existing: bool = False):
+def _upload_bvid(bvid: str):
     access_key, secret_key = read_ia_keys(config.ia_key_file)
 
     # identifier format: BiliBili-{bvid}_p{pid}-{upper_part} 
     upper_part = human_readable_upper_part_map(string=bvid, backward=True)
     OLD_videos_basepath: Path = config.storage_home_dir / 'videos' / bvid
     videos_basepath: Path = config.storage_home_dir / 'videos' / f'{bvid}-{upper_part}'
-
     if os.path.exists(OLD_videos_basepath):
         print(f'检测到旧的视频主目录 {OLD_videos_basepath}，将其重命名为 {videos_basepath}...')
         os.rename(OLD_videos_basepath, videos_basepath)
-
-    if not os.path.exists(videos_basepath):
-        raise VideosBasePathNotFoundError(f'{videos_basepath}')
     for local_identifier in os.listdir(videos_basepath):
         remote_identifier = f'{local_identifier}-{upper_part}'
-        if os.path.exists(f'{videos_basepath}/{local_identifier}/_uploaded.mark') and not update_existing:
+        if os.path.exists(f'{videos_basepath}/{local_identifier}/_uploaded.mark'):
             print(f'{local_identifier} => {remote_identifier} 已经上传过了(_uploaded.mark)')
             continue
         if local_identifier.startswith('_') :
             print(f'跳过 {local_identifier}')
             continue
         if not local_identifier.startswith(BILIBILI_IDENTIFIER_PERFIX):
             print(f'{local_identifier} 不是以 {BILIBILI_IDENTIFIER_PERFIX} 开头的正确 local_identifier')
@@ -57,15 +49,15 @@
             continue
 
         pid = local_identifier.split('_')[-1][1:]
         file_basename = local_identifier[len(BILIBILI_IDENTIFIER_PERFIX)+1:]
 
         print(f'=== 开始上传 {local_identifier} => {remote_identifier} ===')
         item = get_item(remote_identifier)
-        if item.exists and not update_existing:
+        if item.exists:
             print(f'item {remote_identifier} 已存在(item.exists)')
             if item.metadata.get("upload-state") == "uploaded":
                 print(f'{remote_identifier} 已经上传过了，跳过(item.metadata.uploaded)')
                 with open(f'{videos_basepath}/{local_identifier}/_uploaded.mark', 'w', encoding='utf-8') as f:
                     f.write('')
                 continue
         filedict = {} # "remote filename": "local filename"
@@ -78,18 +70,17 @@
 
         for filename in os.listdir(f'{videos_basepath}/{local_identifier}'):
             file = f'{videos_basepath}/{local_identifier}/{filename}'
             if os.path.isfile(file):
                 if os.path.basename(file).startswith('_'):
                     continue
                 if not os.path.isfile(file):
-                   continue
+                    continue
                 filedict[filename] = file
-
-        assert f'{file_basename}.mp4' in filedict
+        
 
         # IA 去重
         for file_in_item in item.files:
             if file_in_item["name"] in filedict:
                 filedict.pop(file_in_item["name"])
                 print(f"File {file_in_item['name']} already exists in {remote_identifier}.")
 
@@ -110,46 +101,27 @@
                 cid = page['cid']
                 p_part = page['part']
                 break
 
         assert cid is not None
         assert p_part is not None
 
-        aid = bv_info['data']['View']['aid']
-        owner_mid = bv_info['data']['View']['owner']['mid']
-        owner_creator: str = bv_info['data']['View']['owner']['name'] # UP 主
-
-        mids: List[int] = [owner_mid]
-        creators: List[str] = [owner_creator]
-        if bv_info['data']['View'].get('staff') is not None:
-            mids = [] # owner_mid 在 staff 也有
-            creators = []
-            for staff in bv_info['data']['View']['staff']:
-                mids.append(staff['mid']) if staff['mid'] not in mids else None
-                creators.append(staff['name']) if staff['name'] not in creators else None
-        external_identifier = [f"urn:bilibili:video:aid:{aid}",
-                               f"urn:bilibili:video:bvid:{bvid}",
-                               f"urn:bilibili:video:cid:{cid}"]
-        for mid in mids:
-            external_identifier.append(f"urn:bilibili:video:mid:{mid}")
-
         md = {
             "mediatype": "movies",
             "collection": 'opensource_movies',
             "title": bv_info['data']['View']['title'] + f' P{pid} ' + p_part ,
             "description": remote_identifier + ' uploading...',
-            'creator': creators if len(creators) > 1 else owner_creator, # type: list[str] | str
+            'creator': bv_info['data']['View']['owner']['name'], # UP 主
             # UTC time
-            'date': time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(pubdate)),
+            'date': time.strftime("%Y-%m-%d", time.gmtime(pubdate)),
             'year': time.strftime("%Y", time.gmtime(pubdate)),
-            # 'aid': aid,
-            # 'bvid': bvid,
-            # 'cid': cid,
-            # 'mid': mid,
-            "external-identifier": external_identifier,
+            'aid': bv_info['data']['View']['aid'],
+            'bvid': bvid,
+            'cid': cid,
+            'mid': bv_info['data']['View']['owner']['mid'],
             "subject": "; ".join(
                 tags
             ),  # Keywords should be separated by ; but it doesn't matter much; the alternative is to set one per field with subject[0], subject[1], ...
             "upload-state": "uploading",
             'originalurl': f'https://www.bilibili.com/video/{bvid}/?p={pid}',
             'scanner': f'biliarchiver v{BILI_ARCHIVER_VERSION} (dev)',
         }
@@ -163,33 +135,29 @@
                 access_key=access_key,
                 secret_key=secret_key,
                 verbose=True,
                 queue_derive=True,
                 retries=5,
             )
 
-        tries = 100
+        tries = 30
         item = get_item(remote_identifier) # refresh item
         while not item.exists and tries > 0:
             print(f"Waiting for item to be created ({tries})  ...", end='\r')
             time.sleep(30)
             item = get_item(remote_identifier)
             tries -= 1
 
         new_md = {}
         if item.metadata.get("upload-state") != "uploaded":
             new_md.update({"upload-state": "uploaded"})
-        if item.metadata.get("creator") != md['creator']:
-            new_md.update({"creator": md['creator']})
-        if item.metadata.get("description", "") != bv_info['data']['View']['desc']:
+        if item.metadata.get("description") != bv_info['data']['View']['desc']:
             new_md.update({"description": bv_info['data']['View']['desc']})
         if item.metadata.get("scanner") != md['scanner']:
             new_md.update({"scanner": md['scanner']})
-        if item.metadata.get("external-identifier") != md['external-identifier']:
-            new_md.update({"external-identifier": md['external-identifier']})
         if new_md:
             print(f"Updating metadata:")
             print(new_md)
             r = item.modify_metadata(
                 metadata=new_md,
                 access_key=access_key,
                 secret_key=secret_key,
```

### Comparing `biliarchiver-0.0.20/biliarchiver/archive_bvid.py` & `biliarchiver-0.0.9/biliarchiver/archive_bvid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import os
 from pathlib import Path
-from typing import Union
 
 import aiofiles
 import httpx
 from bilix.download.utils import raise_api_error, req_retry
 from bilix.exception import APIError
 
 from bilix.sites.bilibili import api
@@ -70,23 +69,14 @@
         file_basename = f'{bvid}_p{pid}'
         video_basepath = videos_basepath / f'{BILIBILI_IDENTIFIER_PERFIX}-{file_basename}'
         video_extrapath = video_basepath / 'extra'
         if os.path.exists(f'{video_basepath}/_downloaded.mark'):
             print(f'{file_basename}: 已经下载过了')
             continue
 
-        def delete_cache(reason: str = ''):
-            if not os.path.exists(video_basepath):
-                return
-            _files_in_video_basepath = os.listdir(video_basepath)
-            for _file in _files_in_video_basepath:
-                if _file.startswith(file_basename):
-                    print(f'{file_basename}: {reason}，删除缓存: {_file}')
-                    os.remove(video_basepath / _file)
-        delete_cache('为防出错，清空上次未完成的下载缓存')
         video_info = await api.get_video_info(d.client, page.p_url)
         print(f'{file_basename}: {video_info.title}...')
         os.makedirs(video_basepath, exist_ok=True)
         os.makedirs(video_extrapath, exist_ok=True)
 
 
         old_p_name = video_info.pages[video_info.p].p_name
@@ -96,78 +86,51 @@
         video_info.pages[video_info.p].p_name = file_basename # 所以这里覆盖 p_name 为 file_basename
         video_info.h1_title = 'iiiiii' * 50 # 然后假装超长标题
         # 这样 bilix 保存的文件名就是我们想要的了（谁叫 bilix 不支持自定义文件名呢）
         # NOTE: p_name 似乎也不宜过长，否则还是会被 bilix 截断。
         # 但是我们以 {bvid}_p{pid} 作为文件名，这个长度是没问题的。
 
 
+        # 选择编码，优先 hevc，没有的话就 avc
+        # 不选 av0 ，毕竟目前没几个设备能拖得动
         codec = None
-        quality = None
         if video_info.dash:
-            # 选择编码 dvh->hev->avc
-            # 不选 av0 ，毕竟目前没几个设备能拖得动
-            codec_candidates = ['dvh', 'hev', 'avc']
-            for codec_candidate in codec_candidates:
+            for media in video_info.dash.videos:
+                if media.codec.startswith('hev'):
+                    codec = media.codec
+                    print(f'{file_basename}: "{codec}" "{media.quality}" ...')
+                    break
+            if codec is None:
                 for media in video_info.dash.videos:
-                    if media.codec.startswith(codec_candidate):
+                    if media.codec.startswith('avc'):
                         codec = media.codec
-                        quality = media.quality
                         print(f'{file_basename}: "{codec}" "{media.quality}" ...')
                         break
-                if codec is not None:
-                    break
-            assert codec is not None and quality is not None, f'{file_basename}: 没有 dvh、avc 或 hevc 编码的视频'
+            assert codec is not None, f'{file_basename}: 没有 avc 或 hevc 编码的视频'
         elif video_info.other:
-            print(f'{file_basename}: 未解析到 dash 资源，交给 bilix 处理 ...')
+            print(f'{file_basename}: 未解析到dash资源，交给 bilix 处理 ...')
             codec = ''
-            quality = 0
         else:
             raise APIError(f'{file_basename}: 未解析到视频资源', page.p_url)
 
         assert codec is not None
-        assert isinstance(quality, (int, str))
 
         cor1 = d.get_video(page.p_url ,video_info=video_info, path=video_basepath,
-                    quality=quality, # 选择最高画质
+                    quality=0, # 选择最高画质
                     codec=codec, # 编码
                     # 下载 ass 弹幕(bilix 会自动调用 danmukuC 将 pb 弹幕转为 ass)、封面、字幕
                     # 弹幕、封面、字幕都会被放进 extra 子目录里，所以需要 d.hierarchy is True
                     dm=True, image=True, subtitle=True
                     )
         # 下载原始的 pb 弹幕
         cor2 = d.get_dm(page.p_url, video_info=video_info, path=video_extrapath)
         # 下载视频超详细信息（BV 级别，不是分 P 级别）
         cor3 = download_bilibili_video_detail(d.client, bvid, f'{video_extrapath}/{file_basename}.info.json')
         await asyncio.gather(cor1, cor2, cor3)
 
-        if codec.startswith('hev') and not os.path.exists(video_basepath / f'{file_basename}.mp4'):
-
-            # 如果有下载缓存文件（以 file_basename 开头的文件），说明这个 hevc 的 dash 资源存在，只是可能因为网络之类的原因下载中途失败了
-            delete_cache('下载出错')
-
-            # 下载缓存文件都不存在，应该是对应的 dash 资源根本就没有，一些老视频会出现这种情况。
-            # 换 avc 编码
-            print(f'{file_basename}: 视频文件没有被下载？也许是 hevc 对应的 dash 资源不存在，尝试 avc ……')
-            for media in video_info.dash.videos:
-                if media.codec.startswith('avc'):
-                    codec = media.codec
-                    print(f'{file_basename}: "{codec}" "{media.quality}" ...')
-                    break
-            cor4 = d.get_video(page.p_url ,video_info=video_info, path=video_basepath,
-                    quality=0, # 选择最高画质
-                    codec=codec, # 编码
-                    # 下载 ass 弹幕(bilix 会自动调用 danmukuC 将 pb 弹幕转为 ass)、封面、字幕
-                    # 弹幕、封面、字幕都会被放进 extra 子目录里，所以需要 d.hierarchy is True
-                    dm=True, image=True, subtitle=True
-                    )
-            await asyncio.gather(cor4)
-
-
-        assert os.path.exists(video_basepath / f'{file_basename}.mp4')
-
         # 还原为了自定义文件名而做的覆盖
         video_info.pages[video_info.p].p_name = old_p_name
         video_info.h1_title = old_h1_title
 
         # 单 p 下好了
         async with aiofiles.open(f'{video_basepath}/_downloaded.mark', 'w', encoding='utf-8') as f:
             await f.write('')
```

### Comparing `biliarchiver-0.0.20/biliarchiver/cli_tools/bili_get_bvids.py` & `biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.20/biliarchiver/cli_tools/bili_upload.py` & `biliarchiver-0.0.9/biliarchiver/bili_uploade.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,48 +6,43 @@
 from biliarchiver._biliarchiver_upload_bvid import upload_bvid
 from biliarchiver.config import config
 
 @dataclass
 class Args:
     bvids: str
     by_storage_home_dir: bool
-    update_existing: bool
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
     bvids_file_group = parser.add_argument_group()
     bvids_file_group.title = 'bvids'
     bvids_file_group.add_argument('--bvids', type=str, dest='bvids',
         help='bvids 列表的文件路径')
     storage_home_dir_group = parser.add_argument_group()
     storage_home_dir_group.title = 'storage_home_dir'
     storage_home_dir_group.add_argument('--by-storage_home_dir', action='store_true', dest='by_storage_home_dir',
         help='从 config.json 中读取 storage_home_dir，然后上传 storage_home_dir/videos 下的所有视频')
-    update_existing_group = parser.add_argument_group()
-    update_existing_group.title = 'update_existing'
-    update_existing_group.add_argument('--update_existing', action='store_true', dest='update_existing',
-        help='更新已存在的 item')
 
     args = Args(**vars(parser.parse_args()))
 
     return args
 
 def main():
     args = parse_args()
     if args.by_storage_home_dir:
         for bvid_with_upper_part in os.listdir(config.storage_home_dir / 'videos'):
             bvid = bvid_with_upper_part
             if '-' in bvid_with_upper_part:
                 bvid = bvid_with_upper_part.split('-')[0]
 
-            upload_bvid(bvid, update_existing=args.update_existing)
+            upload_bvid(bvid)
     
     if args.bvids:
         with open(args.bvids, 'r', encoding='utf-8') as f:
             bvids_from_file = f.read().splitlines()
         for bvid in bvids_from_file:
 
-            upload_bvid(bvid, update_existing=args.update_existing)
+            upload_bvid(bvid)
 
 if __name__ == '__main__':
     main()
```

### Comparing `biliarchiver-0.0.20/biliarchiver/config.py` & `biliarchiver-0.0.9/biliarchiver/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,28 @@
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 @dataclass
-class _Config(metaclass=singleton):
+class Config(metaclass=singleton):
     video_concurrency: int = 3 
     part_concurrency: int = 10
     stream_retry: int = 20
     storage_home_dir: Path = Path('bilibili_archive_dir/').expanduser()
     ia_key_file: Path = Path('~/.bili_ia_keys.txt').expanduser()
-    cookies_file: Path = Path('~/.cookies.txt').expanduser()
 
     def __init__(self):
         self.is_right_pwd()
         if not os.path.exists(CONFIG_FILE):
             print(f'{CONFIG_FILE} 不存在，创建中...')
             self.save()
         with open(CONFIG_FILE, 'r', encoding='utf-8') as f:
-            print(f'Loading {CONFIG_FILE} ...')
+            print(f'读取 {CONFIG_FILE}...')
             config_file = json.load(f)
 
         self.video_concurrency: int = config_file['video_concurrency']
         self.part_concurrency: int = config_file['part_concurrency']
         self.stream_retry: int = config_file['stream_retry']
 
         self.storage_home_dir: Path = Path(config_file['storage_home_dir']).expanduser()
@@ -44,15 +43,14 @@
         with open(CONFIG_FILE, 'w', encoding='utf-8') as f:
             json.dump({
                 'video_concurrency': self.video_concurrency,
                 'part_concurrency': self.part_concurrency,
                 'stream_retry': self.stream_retry,
                 'storage_home_dir': str(self.storage_home_dir),
                 'ia_key_file': str(self.ia_key_file),
-                'cookies_file': str(self.cookies_file),
             }, f, ensure_ascii=False, indent=4)
 
     def is_right_pwd(self):
         if not os.path.exists('biliarchiver.home'):
             raise Exception('先在当前工作目录创建 biliarchiver.home 文件')
 
-config = _Config()
+config = Config()
```

### Comparing `biliarchiver-0.0.20/biliarchiver/utils/dirLock.py` & `biliarchiver-0.0.9/biliarchiver/utils/dirLock.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.20/biliarchiver/utils/string.py` & `biliarchiver-0.0.9/biliarchiver/utils/string.py`

 * *Files identical despite different names*

