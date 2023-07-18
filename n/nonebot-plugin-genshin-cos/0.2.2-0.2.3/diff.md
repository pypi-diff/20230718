# Comparing `tmp/nonebot_plugin_genshin_cos-0.2.2.tar.gz` & `tmp/nonebot_plugin_genshin_cos-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshin_cos-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshin_cos-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_genshin_cos-0.2.2.tar` & `nonebot_plugin_genshin_cos-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/LICENSE
--rw-r--r--   0        0        0     3973 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/README.md
--rw-r--r--   0        0        0    13942 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/__init__.py
--rw-r--r--   0        0        0      271 2023-06-29 11:26:08.100934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/config.py
--rw-r--r--   0        0        0   459180 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
--rw-r--r--   0        0        0    12330 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/hoyospider.py
--rw-r--r--   0        0        0     4931 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/utils.py
--rw-r--r--   0        0        0      612 2023-06-29 11:26:08.104934 nonebot_plugin_genshin_cos-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-18 06:59:21.003252 nonebot_plugin_genshin_cos-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4176 2023-07-18 06:59:21.003252 nonebot_plugin_genshin_cos-0.2.3/README.md
+-rw-r--r--   0        0        0    16302 2023-07-18 06:59:21.003252 nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/__init__.py
+-rw-r--r--   0        0        0      226 2023-07-18 06:59:21.003252 nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/config.py
+-rw-r--r--   0        0        0   459180 2023-07-18 06:59:21.007252 nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
+-rw-r--r--   0        0        0    12292 2023-07-18 06:59:21.007252 nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/hoyospider.py
+-rw-r--r--   0        0        0     5001 2023-07-18 06:59:21.007252 nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/utils.py
+-rw-r--r--   0        0        0      651 2023-07-18 06:59:21.007252 nonebot_plugin_genshin_cos-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5108 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_genshin_cos-0.2.2/LICENSE` & `nonebot_plugin_genshin_cos-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.2.2/README.md` & `nonebot_plugin_genshin_cos-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+![056131D4](https://github.com/Cvandia/nonebot_plugin_genshin_cos/assets/106718176/da116fce-d24f-4f89-8f6c-1f2509fd56be)
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
 
 </div>
 
 <div align="center">
@@ -20,17 +20,19 @@
 
 
 ## ⭐ 介绍
 
 受到[教程](https://juejin.cn/post/6990320268010848286)的启发，所以写了这个插件，更多功能后续更新~~我很懒，学业重~~
 
 
+
 <div align="center">
 
 ### 或者你有啥关于该插件的新想法的，可以提issue或者pr (>A<)
+### 不仅有原神，现在支持崩坏3、星穹铁道、大别野的cos图！
 
 </div>
 
 ## 💿 安装
 
 <details>
 <summary>安装</summary>
@@ -121,8 +123,8 @@
 coser的创作权
 
 
 
 ## 💝 特别鸣谢
 
 - [x] [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
-- [x] [@qxdn](https://github.com/qxdn):感谢qxdn的[博客文章](https://qianxu.run/2021/11/12/mihoyo-bbs-crawler/),有兴趣大家也去看看咯
+- [x] [@qxdn](https://github.com/qxdn):感谢qxdn的[博客文章](https://qianxu.run/2021/11/12/mihoyo-bbs-crawler/),有兴趣大家也去看看咯
```

#### html2text {}

```diff
@@ -1,17 +1,20 @@
+![056131D4](https://github.com/Cvandia/nonebot_plugin_genshin_cos/assets/
+106718176/da116fce-d24f-4f89-8f6c-1f2509fd56be)
                               [NoneBotPluginLogo]
                          # nonebot-plugin-genshin-cos
           _â­åºäºNonebot2çä¸æ¬¾è·åç±³æ¸¸ç¤¾cosçæä»¶â­_
 [https://img.shields.io/badge/python-3.8+-blue] [https://img.shields.io/badge/
 QQ-1141538825-yellow] [https://img.shields.io/badge/license-MIT-blue] [https://
                     img.shields.io/badge/Nonebot2-rc1+-red]
 ## â­ ä»ç» åå°[æç¨](https://juejin.cn/post/
 6990320268010848286)çå¯åï¼æä»¥åäºè¿ä¸ªæä»¶ï¼æ´å¤åè½åç»­æ´æ°~~æå¾æï¼å­¦ä¸é~~
   ### æèä½ æå¥å³äºè¯¥æä»¶çæ°æ³æ³çï¼å¯ä»¥æissueæèpr
-                                     (>A<)
+                                   (>A<) ###
+ ä¸ä»æåç¥ï¼ç°å¨æ¯æå´©å3ãæç©¹ééãå¤§å«éçcoså¾ï¼
 ## ð¿ å®è£  å®è£ pip å®è£ ``` pip install nonebot-plugin-genshin-cos
 ``` - å¨nonebotçpyproject.tomlä¸­çplugins = ["xxx"]æ·»å æ­¤æä»¶ nb-
 cliå®è£ ``` nb plugin install nonebot-plugin-genshin-cos --upgrade ``` git
 cloneå®è£(ä¸æ¨è) - è¿è¡ ```git clone https://github.com/Cvandia/
 nonebot_plugin_genshin_cos``` - å¨è¿è¡å¤ ææä»¶å¤¹`nonebot-plugin-
 genshen-cos`å¤å¶å°botæ ¹ç®å½ä¸ç`src/plugins`
 (æèä½ åå»ºbotæ¶çå¶ä»åç§°`xxx/plugins`)   æ³¨æ
```

### Comparing `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/__init__.py` & `nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from nonebot.adapters.onebot.v11 import (
-    Bot,
-    Message,
-    MessageEvent,
-    MessageSegment,
-    GroupMessageEvent
-)
+from random import choice
+from typing import Annotated
+
+from nonebot import get_bot
+from nonebot.adapters.onebot.v11 import MessageSegment
+from nonebot.params import RegexGroup, ArgPlainText, CommandArg, CommandStart
 from nonebot.plugin import on_regex, on_command, require, PluginMetadata
-from nonebot.params import RegexGroup, ArgPlainText, CommandArg
-from nonebot.log import logger
-from nonebot import get_driver, get_bot
-from nonebot.matcher import Matcher
 from nonebot.rule import to_me
-from nonebot.exception import ActionFailed
-from typing import Tuple, Any
-from random import choice
-from datetime import datetime
+
 from .config import Config
-from .utils import *
 from .hoyospider import *
+from .utils import *
+
+require("nonebot_plugin_templates")
+from nonebot_plugin_templates.template_types import *
+from nonebot_plugin_templates.templates_render import menu_render
+
 try:
     scheduler = require("nonebot_plugin_apscheduler").scheduler
 except:
     scheduler = None
 try:
     import ujson as json
 except ModuleNotFoundError:
@@ -39,86 +36,145 @@
     homepage="https://github.com/Cvandia/nonebot_plugin_genshin_cos",
     supported_adapters={"~onebot.v11"},
     extra={
         "unique_name": "genshin_cos",
         "example": "保存cos:保存cos图片至本地文件",
         "author": "divandia <106718176+Cvandia@users.noreply.github.com>",
         "version": "0.2.0",
-    }
+    },
 )
 logo = """<g>
   /$$$$$$                                /$$       /$$                  /$$$$$$                     
  /$$__  $$                              | $$      |__/                 /$$__  $$                    
 | $$  \__/  /$$$$$$  /$$$$$$$   /$$$$$$$| $$$$$$$  /$$ /$$$$$$$       | $$  \__/  /$$$$$$   /$$$$$$$
 | $$ /$$$$ /$$__  $$| $$__  $$ /$$_____/| $$__  $$| $$| $$__  $$      | $$       /$$__  $$ /$$_____/
 | $$|_  $$| $$$$$$$$| $$  \ $$|  $$$$$$ | $$  \ $$| $$| $$  \ $$      | $$      | $$  \ $$|  $$$$$$ 
 | $$  \ $$| $$_____/| $$  | $$ \____  $$| $$  | $$| $$| $$  | $$      | $$    $$| $$  | $$ \____  $$
 |  $$$$$$/|  $$$$$$$| $$  | $$ /$$$$$$$/| $$  | $$| $$| $$  | $$      |  $$$$$$/|  $$$$$$/ /$$$$$$$/
  \______/  \_______/|__/  |__/|_______/ |__/  |__/|__/|__/  |__/       \______/  \______/ |_______/ 
  </g>"""
 
-
 logger.opt(colors=True).info(logo)
 
-#用户cd数据
+# 用户cd数据
 user_data = {}
-CONFIG: Dict[str, Dict[str,str]] = {'原神':{},'崩坏3':{},'大别野':{},'星穹铁道':{}}
+CONFIG: Dict[str, Dict[str, str]] = {"原神": {}, "崩坏3": {}, "大别野": {}, "星穹铁道": {}}
 DRIVER = get_driver()
 
 # 读取配置文件
 config_path = Path("config/genshincos.json")
 config_path.parent.mkdir(parents=True, exist_ok=True)
 if config_path.exists():
     with open(config_path, "r", encoding="utf8") as f:
         CONFIG = json.load(f)
 else:
     with open(config_path, "w", encoding="utf8") as f:
         json.dump(CONFIG, f, ensure_ascii=False, indent=4)
 
-#事件响应器
-download_cos = on_command('下载cos', aliases={'cos保存', '保存cos'}, block=False, priority=5, permission=SUPER_PERMISSION)
-hot_cos = on_command('热门cos', aliases={'热门coser', '热门cos图'}, block=False, priority=5)
-rank_cos = on_regex(r'^(日|月|周)榜cos[r]?[图]?(.+)?',priority=5, block=False, flags=re.I)
-latest_cos = on_command('最新cos', aliases={'最新coser', '最新cos图'}, block=False, priority=5)
-good_cos = on_command('精品cos', aliases={'精品coser', '精品cos图'}, block=False, priority=5)
-turn_aps = on_regex(r'^(开启|关闭)每日推送(原神|崩坏3|星穹铁道|大别野)(\s)?(.+)?', block=False, priority=5, flags=re.I, permission=SUPER_PERMISSION)
-show_aps = on_command('查看本群推送', aliases={'查看推送','查看订阅'}, block=False, priority=5, rule=to_me())
+# 事件响应器
+help = on_command("原神cos", aliases={"genshincos"})
+download_cos = on_command(
+    "下载cos",
+    aliases={"cos保存", "保存cos"},
+    block=False,
+    priority=5,
+    permission=SUPER_PERMISSION,
+)
+hot_cos = on_command("热门cos", aliases={"热门coser", "热门cos图"}, block=False, priority=5)
+rank_cos = on_regex(r"^(日|月|周)榜cos[r]?[图]?(.+)?", priority=5, block=False, flags=re.I)
+latest_cos = on_command("最新cos", aliases={"最新coser", "最新cos图"}, block=False, priority=5)
+good_cos = on_command("精品cos", aliases={"精品coser", "精品cos图"}, block=False, priority=5)
+turn_aps = on_regex(
+    r"^(开启|关闭)每日推送(原神|崩坏3|星穹铁道|大别野)(\s)?(.+)?",
+    block=False,
+    priority=5,
+    flags=re.I,
+    permission=SUPER_PERMISSION,
+)
+show_aps = on_command(
+    "查看本群推送", aliases={"查看推送", "查看订阅"}, block=False, priority=5, rule=to_me()
+)
+
+Generated_pic = False
+Help_Path = Path(__file__).parent / "Help.jpeg"
+
+
+@help.handle()
+async def _(matcher: Matcher, event: MessageEvent, foo: Annotated[str, CommandStart()]):
+    global Generated_pic
+    command_start = str(foo)
+    if not Generated_pic:
+        menu = Menu(
+            "原神cos",
+            des="获取原神cos图片",
+            funcs=Funcs(
+                Func(f"{command_start}日、周、月榜cos", "获取排行榜cos图。如日榜cos 原神 x3")
+                + Func(f"{command_start}热门cos", "获取指定游戏热门cos图，如热门cos 原神 x3	")
+                + Func(f"{command_start}最新cos", "获取指定游戏最新cos图，如最新cos 原神 x3	")
+                + Func(f"{command_start}精品cos", "获取指定游戏精品cos图，如精品cos 原神 x3	")
+                + Func(f"{command_start}查看本群推送", "查看本群的订阅cos目录")
+                + Func(
+                    f"{command_start}下载cos", "仅超管、群主、管理员可用\n获取指定游戏热门cos图，如热门cos 原神 x3	"
+                )
+                + Func(
+                    f"{command_start}开启每日推送xx (时间)",
+                    "仅超管、群主、管理员可用\n如开启每日推送原神 8:30,注意时间的格式",
+                )
+            ),
+        )
+        pic_bytes = await menu_render(Menus(menu), 700)
+        with open(Help_Path, "wb") as f:
+            f.write(pic_bytes)
+        Generated_pic = True
+    else:
+        with open(Help_Path, "rb") as f:
+            pic_bytes = f.read()
+    await matcher.send(MessageSegment.image(pic_bytes))
+
 
 @show_aps.handle()
 async def _(bot: Bot, event: GroupMessageEvent):
-    send_msg = '本群订阅的推送有:\n'
+    send_msg = "本群订阅的推送有:\n"
     for game_type, dict in CONFIG.items():
-        if game_type == "": continue
+        if game_type == "":
+            continue
         for goup_id, time in dict.items():
             if str(event.group_id) == goup_id:
                 send_msg += f"{game_type}的每日{time}推送\n"
     await show_aps.finish(send_msg)
 
 
 @turn_aps.handle()
 async def _(event: GroupMessageEvent, args: Tuple[str, ...] = RegexGroup()):
     # 检查是否安装了apscheduler插件，并且是否开启了定时推送
     if scheduler == None:
         await turn_aps.finish("未安装apscheduler插件,无法使用此功能")
-    mode = args[0] 
+    mode = args[0]
     game_type = args[1]
     time = args[3]
     aps_group_id = str(event.group_id)
     MyConfig = CONFIG.copy()
     if mode == "开启":
         for name in MyConfig.keys():
             if name == game_type:
                 if aps_group_id in MyConfig[name].keys():
                     await turn_aps.finish("该群已开启,无需重复开启")
                 elif not time:
                     await turn_aps.finish("请指定推送时间")
                 else:
                     CONFIG[name][aps_group_id] = time
                     try:
-                        scheduler.add_job(aps_send, trigger="cron", hour=time.split(":")[0], minute=time.split(":")[1], id=f"{game_type}{aps_group_id}",args=(aps_group_id,)) 
+                        scheduler.add_job(
+                            aps_send,
+                            trigger="cron",
+                            hour=time.split(":")[0],
+                            minute=time.split(":")[1],
+                            id=f"{game_type}{aps_group_id}",
+                            args=(aps_group_id,),
+                        )
                         logger.debug(f"已成功添加{aps_group_id}的{game_type}定时推送")
                     except Exception as e:
                         logger.error(e)
     else:
         for name in MyConfig.keys():
             if name == game_type:
                 if aps_group_id in MyConfig[name].keys():
@@ -132,32 +188,40 @@
                     await turn_aps.finish("该群已关闭,无需重复关闭")
     with open(config_path, "w", encoding="utf8") as f:
         f.write(json.dumps(CONFIG, ensure_ascii=False, indent=4))
     await turn_aps.finish(f"已成功{mode}{aps_group_id}的{game_type}定时推送")
 
 
 @hot_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
+async def _(
+        bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()
+):
     if not arg:
         await hot_cos.finish("请指定cos类型")
     args = arg.extract_plain_text().split()
     if args[0] in GENSHIN_NAME:
         send_type = genshin_hot
     elif args[0] in HONKAI3RD_NAME:
         send_type = honkai3rd_hot
     elif args[0] in DBY_NAME:
         send_type = dbycos_hot
     elif args[0] in STAR_RAIL:
         send_type = starrail_hot
     else:
         await hot_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
+    await send_images(bot, matcher, args, event, send_type)
+
 
 @rank_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, group: Tuple[str, ...] = RegexGroup()):
+async def _(
+        bot: Bot,
+        matcher: Matcher,
+        event: MessageEvent,
+        group: Tuple[str, ...] = RegexGroup(),
+):
     if not group[1]:
         await rank_cos.finish("请指定cos类型")
     args = group[1].split()
     if group[0] == "日":
         rank_type = RankType.Daily
     elif group[0] == "周":
         rank_type = RankType.Weekly
@@ -170,83 +234,94 @@
         send_type = Rank(ForumType.Honkai3rdPic, rank_type)
     elif args[0] in DBY_NAME:
         send_type = Rank(ForumType.DBYCOS, rank_type)
     elif args[0] in STAR_RAIL:
         send_type = Rank(ForumType.StarRailCos, rank_type)
     else:
         await rank_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
+    await send_images(bot, matcher, args, event, send_type)
+
 
 @latest_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
+async def _(
+        bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()
+):
     if not arg:
         await latest_cos.finish("请指定cos类型")
     args = arg.extract_plain_text().split()
     if args[0] in GENSHIN_NAME:
         send_type = genshin_latest_comment
     elif args[0] in HONKAI3RD_NAME:
         send_type = honkai3rd_latest_comment
     elif args[0] in DBY_NAME:
         send_type = dbycos_latest_comment
     elif args[0] in STAR_RAIL:
         send_type = starrail_latest_comment
     else:
         await latest_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
+    await send_images(bot, matcher, args, event, send_type)
+
 
 @good_cos.handle()
-async def _(bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()):
+async def _(
+        bot: Bot, matcher: Matcher, event: MessageEvent, arg: Message = CommandArg()
+):
     if not arg:
         await good_cos.finish("请指定cos类型")
     args = arg.extract_plain_text().split()
     if args[0] in GENSHIN_NAME:
         await good_cos.finish("原神暂不支持精品cos")
     elif args[0] in HONKAI3RD_NAME:
         send_type = honkai3rd_good
     elif args[0] in DBY_NAME:
         send_type = dbycos_good
     elif args[0] in STAR_RAIL:
         await good_cos.finish("星穹铁道暂不支持精品cos")
     else:
         await good_cos.finish("暂不支持该类型")
-    await send_images(bot,matcher,args,event,send_type)
+    await send_images(bot, matcher, args, event, send_type)
 
 
-@download_cos.got('game_type', prompt='你想下载哪种类型的,有原神和大别野,崩坏3,星穹铁道')
+@download_cos.got("game_type", prompt="你想下载哪种类型的,有原神和大别野,崩坏3,星穹铁道")
 async def got_type(game_type: str = ArgPlainText()):
     if game_type in GENSHIN_NAME:
         hot = genshin_hot
     elif game_type in DBY_NAME:
         hot = dbycos_hot
     elif game_type in HONKAI3RD_NAME:
         hot = honkai3rd_hot
     elif game_type in STAR_RAIL:
         hot = starrail_hot
     image_urls = await hot.async_get_urls()
     if not image_urls:
-        await download_cos.finish(f'没有找到{game_type}的cos图片')
+        await download_cos.finish(f"没有找到{game_type}的cos图片")
     else:
-        await download_cos.send(f'正在下载{game_type}的cos图片')
+        await download_cos.send(f"正在下载{game_type}的cos图片")
         try:
-            await download_from_urls(image_urls, SAVE_PATH / f'{game_type}cos')
-            await download_cos.finish(f'已成功保存{len(image_urls)}张{game_type}的cos图片')
+            await download_from_urls(image_urls, SAVE_PATH / f"{game_type}cos")
+            await download_cos.finish(f"已成功保存{len(image_urls)}张{game_type}的cos图片")
         except WriteError as e:
-            await download_cos.finish(f'保存部分{game_type}的cos图片失败,原因:{e}')
+            await download_cos.finish(f"保存部分{game_type}的cos图片失败,原因:{e}")
+
 
 ###########################################################################################
 
-#定时任务
+
+# 定时任务
 async def aps_send(aps_goup_id: str):
     logger.debug("正在发送定时推送")
     bot: Bot = get_bot()
     for game_type, dict in CONFIG.items():
         if game_type == "":
             continue
         for saved_group_id, time in dict.items():
-            if not (datetime.now().hour == int(time.split(":")[0]) and datetime.now().minute == int(time.split(":")[1])):
+            if not (
+                    datetime.now().hour == int(time.split(":")[0])
+                    and datetime.now().minute == int(time.split(":")[1])
+            ):
                 continue
             elif saved_group_id != aps_goup_id:
                 continue
             try:
                 group_id = int(saved_group_id)
                 if game_type in GENSHIN_NAME:
                     send_type = genshin_rank_daily
@@ -256,76 +331,94 @@
                     send_type = honkai3rd_rank_daily
                 elif game_type in STAR_RAIL:
                     send_type = starrail_rank_daily
                 else:
                     continue
                 image_list = await send_type.async_get_urls(page_size=5)
                 name_list = await send_type.async_get_name(page_size=5)
-                rank_text = '\n'.join([f"{i+1}.{name_list[i]}" for i in range(len(name_list))])
+                rank_text = "\n".join(
+                    [f"{i + 1}.{name_list[i]}" for i in range(len(name_list))]
+                )
                 msg_list = [f"✅米游社{game_type}cos每日榜单✅"]
                 msg_list.append(rank_text)
                 msg_list.append([MessageSegment.image(img) for img in image_list])
-                msg_list = msglist2forward('米游社cos', '2854196306', msg_list)
-                await bot.call_api("send_group_forward_msg", group_id=group_id, messages=msg_list)
+                msg_list = msglist2forward("米游社cos", "2854196306", msg_list)
+                await bot.call_api(
+                    "send_group_forward_msg", group_id=group_id, messages=msg_list
+                )
                 await asyncio.sleep(1)
             except Exception as e:
                 logger.error(e)
 
 
-async def send_images(bot:Bot, matcher: Matcher, args: list, event: MessageEvent, send_type: HoyoBasicSpider):
-    '''
+async def send_images(
+        bot: Bot,
+        matcher: Matcher,
+        args: list,
+        event: MessageEvent,
+        send_type: HoyoBasicSpider,
+):
+    """
     发送图片
 
     params:
         bot: 当前bot
         matcher: 事件响应器
         args: 命令参数(0:类型 1:数量)
         event: 消息事件类型
         send_type: 爬虫类型
-    '''
+    """
     global user_data
     out_cd, deletime, user_data = check_cd(event.user_id, user_data)
     if out_cd:
-        if len(args)<2:
+        if len(args) < 2:
             await matcher.send("获取图片中…请稍等")
             try:
                 image_list = await send_type.async_get_urls()
                 await matcher.send(MessageSegment.image(choice(image_list)))
             except ActionFailed:
                 await matcher.finish("账户风控了,发送不了图片", at_sender=True)
         else:
             num = int(re.sub(r"[x|*|X]", "", args[1]))
             num = num if num <= MAX else MAX
-            msg_list = [f'✅找到最新的一些{args[0]}图如下:✅']
+            msg_list = [f"✅找到最新的一些{args[0]}图如下:✅"]
             image_list = await send_type.async_get_urls()
             if num > len(image_list):
                 await matcher.finish(f"最多只能获取{len(image_list)}张图片", at_sender=True)
             for i in range(num):
                 msg_list.append(MessageSegment.image(image_list[i]))
             if IS_FORWARD:
                 await send_forward_msg(bot, event, "米游社cos", bot.self_id, msg_list)
             else:
                 await send_regular_msg(matcher, msg_list)
     else:
         await matcher.finish(f"cd冷却中,还剩{deletime}秒", at_sender=True)
 
+
 @DRIVER.on_startup
 async def start_aps():
     try:
         if scheduler == None:
             logger.error("未安装apscheduler插件,无法使用此功能")
         with open(config_path, "r", encoding="utf8") as f:
             CONFIG = json.load(f)
         for game_type, dict in CONFIG.items():
             if game_type == "":
                 continue
             for aps_group_id, time in dict.items():
                 if time == "":
                     continue
                 try:
-                    scheduler.add_job(aps_send, trigger="cron", hour=time.split(":")[0], minute=time.split(":")[1], id=f"{game_type}{aps_group_id}",args=(aps_group_id,))
+                    scheduler.add_job(
+                        aps_send,
+                        trigger="cron",
+                        hour=time.split(":")[0],
+                        minute=time.split(":")[1],
+                        id=f"{game_type}{aps_group_id}",
+                        args=(aps_group_id,),
+                    )
                     logger.debug(f"已成功添加{aps_group_id}的{game_type}定时推送")
                 except Exception as e:
                     logger.error(e)
                     continue
     except Exception as e:
-        logger.error(e)
+        logger.error(e)
```

### Comparing `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF` & `nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/hoyospider.py` & `nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/hoyospider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from enum import Enum, unique
 from typing import Dict, List
+
 import httpx
 from httpx import Response
 
+
 ##########################################################################################
 
 # 类定义
 
 class HoyoBasicSpider:
     def __init__(self) -> None:
         self.base_url = 'https://bbs-api.mihoyo.com/post/wapi/'  # 基础url
@@ -33,15 +35,15 @@
 
     def sync_get_urls(self, page_size: int) -> str:
         """同步获取urls
         :param page_size: 每页数量
         :return: urls
         """
         pass
-    
+
     def sync_get_name(self, page_size: int) -> str:
         """同步获取names
         :param page_size: 每页数量
         :return: urls
         """
         pass
 
@@ -50,15 +52,15 @@
         :param params: 参数
         :param is_good: 是否精品
         :return: 响应list
         """
 
         response = httpx.get(self.api, params=params, headers=self.headers)
         return self.handle_response(response, is_good)
-    
+
     def sync_name(self, params: dict = None, is_good: bool = False):
         """同步获取
         :param params: 参数
         :param is_good: 是否精品
         :return: 响应list
         """
 
@@ -97,15 +99,15 @@
         :param is_good: 是否精品
         :return: 响应list
         """
 
         async with httpx.AsyncClient() as client:
             response = await client.get(self.api, params=params, headers=self.headers)
         return self.get_rsp_name(response, is_good)
-    
+
     def handle_response(self, response: Response, is_good: bool = False) -> List:
         """处理响应
         :param response: 响应
         :param is_good: 是否精品
         :return: urls list
         """
 
@@ -129,14 +131,15 @@
             posts = response.json()['data']['posts']
         else:
             posts = response.json()['data']['list']
         for post in posts:
             names.append(post['post']['subject'])
         return names
 
+
 @unique
 class RankType(Enum):
     '''
     排行榜类型
     '''
     Daily = 1  # 日榜
     Weekly = 2  # 周榜
@@ -171,15 +174,15 @@
     '''
     GenshinCos = 49  # 原神cos
     GenshinPic = 29  # 原神同人图
     Honkai3rdPic = 4  # 崩坏3同人图
     DBYCOS = 47  # 大别野cos
     DBYPIC = 39  # 大别野同人图
     StarRailPic = 56  # 星穹铁道同人图
-    StarRailCos = 62 # 星穹铁道cos
+    StarRailCos = 62  # 星穹铁道cos
     Honkai2Pic = 40  # 崩坏2同人图
     TearsOfThemisPic = 38  # 泪水同人图
 
 
 def get_gids(forum: str) -> GameType:
     '''
     根据论坛名获取游戏id
@@ -228,19 +231,20 @@
     async def async_get_urls(self, page_size: int = 21) -> List:
         params = self.get_params(page_size)
         return await self.async_get(params)
 
     async def async_get_name(self, page_size: int = 21) -> List:
         params = self.get_params(page_size)
         return await self.async_name(params)
-    
+
     def sync_get_name(self, page_size: int = 21) -> List:
         params = self.get_params(page_size)
         return self.sync_name(params)
 
+
 class Hot(HoyoBasicSpider):
     '''
     获取热门帖子
     url: https://bbs.mihoyo.com/ys/home/49?type=hot
     '''
 
     def __init__(self, forum_id: ForumType) -> None:
@@ -263,19 +267,19 @@
     def sync_get_urls(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return self.sync_get(params)
 
     async def async_get_urls(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return await self.async_get(params)
-    
+
     def sync_get_name(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return self.sync_name(params)
-    
+
     async def async_get_name(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return await self.async_name(params)
 
 
 class Good(HoyoBasicSpider):
     '''
@@ -302,19 +306,19 @@
     def sync_get_urls(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return self.sync_get(params, is_good=True)
 
     async def async_get_urls(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return await self.async_get(params, is_good=True)
-    
+
     def sync_get_name(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return self.sync_name(params, is_good=True)
-    
+
     async def async_get_name(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return await self.async_name(params, is_good=True)
 
 
 class Latest(HoyoBasicSpider):
     '''
@@ -342,25 +346,25 @@
     def sync_get_urls(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return self.sync_get(params)
 
     async def async_get_urls(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return await self.async_get(params)
-    
+
     def sync_get_name(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return self.sync_name(params)
-    
+
     async def async_get_name(self, page_size: int = 20) -> List:
         params = self.get_params(page_size)
         return await self.async_name(params)
-    
 
-#实例化对象
+
+# 实例化对象
 
 genshin_rank_daily = Rank(ForumType.GenshinCos, RankType.Daily)
 genshin_hot = Hot(ForumType.GenshinCos)
 genshin_good = Good(ForumType.GenshinCos)
 genshin_latest_comment = Latest(ForumType.GenshinCos, LatestType.LatestComment)
 
 honkai3rd_rank_daily = Rank(ForumType.Honkai3rdPic, RankType.Daily)
```

### Comparing `nonebot_plugin_genshin_cos-0.2.2/nonebot_plugin_genshin_cos/utils.py` & `nonebot_plugin_genshin_cos-0.2.3/nonebot_plugin_genshin_cos/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+from asyncio import sleep
+from datetime import datetime, timedelta
 from pathlib import Path
-from nonebot import get_driver
-from .config import Config
 from typing import Dict, List, Tuple
-from datetime import datetime, timedelta
-from httpx import TimeoutException
+
 import httpx
+from httpx import TimeoutException
+from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, Message, GROUP_ADMIN, GROUP_OWNER
-from nonebot.permission import SUPERUSER
-from nonebot.matcher import Matcher
-from nonebot.log import logger
 from nonebot.exception import ActionFailed
-from asyncio import sleep
+from nonebot.log import logger
+from nonebot.matcher import Matcher
+from nonebot.permission import SUPERUSER
+
+from .config import Config
+
 #######################################################
 
 # 拓展的异常类和函数
 SUPER_PERMISSION = GROUP_ADMIN | GROUP_OWNER | SUPERUSER
-GENSHIN_NAME = ["原神",'OP','op','欧泡','⭕','🅾️','🅾️P','🅾️p','原','圆']
-HONKAI3RD_NAME = ['崩坏3', '崩崩崩', '蹦蹦蹦','崩坏三','崩三','崩崩崩三','崩坏3rd','崩坏3Rd','崩坏3RD','崩坏3rd','崩坏3RD','崩坏3Rd']
-DBY_NAME = ['大别野','DBY','dby']
-STAR_RAIL = ['星穹铁道','星穹','崩铁','铁道','星铁','穹p','穹铁']
+GENSHIN_NAME = ["原神", 'OP', 'op', '欧泡', '⭕', '🅾️', '🅾️P', '🅾️p', '原', '圆']
+HONKAI3RD_NAME = ['崩坏3', '崩崩崩', '蹦蹦蹦', '崩坏三', '崩三', '崩崩崩三', '崩坏3rd', '崩坏3Rd', '崩坏3RD', '崩坏3rd',
+                  '崩坏3RD', '崩坏3Rd']
+DBY_NAME = ['大别野', 'DBY', 'dby']
+STAR_RAIL = ['星穹铁道', '星穹', '崩铁', '铁道', '星铁', '穹p', '穹铁']
+
 
 class WriteError(Exception):
     """写入错误"""
     pass
 
 
 # 加载配置
@@ -85,29 +90,30 @@
             if is_download_error:
                 raise WriteError(f'有{error_cnt}张图片由于超时下载失败了')
             success_cnt += 1
             logger.success(f'下载{success_cnt}张成功')
 
 
 async def send_forward_msg(
-    bot: Bot,
-    event: MessageEvent,
-    name: str,
-    uin: str,
-    msgs: list,
+        bot: Bot,
+        event: MessageEvent,
+        name: str,
+        uin: str,
+        msgs: list,
 ) -> dict:
     """调用合并转发API
 
     params:
         bot: Bot,
         event: 消息事件类型,
         name: 发送者昵称,
         uin: 发送者账号,
         msgs: 消息列表,
     """
+
     def to_json(msg: Message):
         return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
 
     messages = [to_json(msg) for msg in msgs]
 
     if isinstance(event, GroupMessageEvent):
         return await bot.call_api(
@@ -124,20 +130,22 @@
 
     params:
         bot: Bot
         name: 发送者昵称
         uin: 发送者账号
         msgs: 消息列表
     """
+
     def to_json(msg: Message):
         return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
 
-    return [to_json(msg) for msg in msgs]   
+    return [to_json(msg) for msg in msgs]
+
 
-async def send_regular_msg(matcher: Matcher,messages:list):
+async def send_regular_msg(matcher: Matcher, messages: list):
     '''
     发送常规消息
     :param matcher: Matcher
     :param messages: 消息列表
     '''
     cnt = 1
     for msg in messages:
```

### Comparing `nonebot_plugin_genshin_cos-0.2.2/PKG-INFO` & `nonebot_plugin_genshin_cos-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshin-cos
-Version: 0.2.2
+Version: 0.2.3
 Summary: 米游社原神cos图获取
 License: MIT
 Author: Cvandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,21 +12,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0)
 Requires-Dist: httpx (>=0.19.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.1.3)
+Requires-Dist: nonebot-plugin-templates (>=0.1.3,<0.2.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.1)
 Requires-Dist: pathlib (>=1.0.1)
 Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: ujson (>=5.5.0)
 Description-Content-Type: text/markdown
 
-
+![056131D4](https://github.com/Cvandia/nonebot_plugin_genshin_cos/assets/106718176/da116fce-d24f-4f89-8f6c-1f2509fd56be)
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/Cvandia/nonebot_plugin_genshin_cos/blob/main/res/ico.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
 
 </div>
 
 <div align="center">
@@ -44,17 +45,19 @@
 
 
 ## ⭐ 介绍
 
 受到[教程](https://juejin.cn/post/6990320268010848286)的启发，所以写了这个插件，更多功能后续更新~~我很懒，学业重~~
 
 
+
 <div align="center">
 
 ### 或者你有啥关于该插件的新想法的，可以提issue或者pr (>A<)
+### 不仅有原神，现在支持崩坏3、星穹铁道、大别野的cos图！
 
 </div>
 
 ## 💿 安装
 
 <details>
 <summary>安装</summary>
@@ -146,7 +149,8 @@
 
 
 
 ## 💝 特别鸣谢
 
 - [x] [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
 - [x] [@qxdn](https://github.com/qxdn):感谢qxdn的[博客文章](https://qianxu.run/2021/11/12/mihoyo-bbs-crawler/),有兴趣大家也去看看咯
+
```

#### html2text {}

```diff
@@ -1,29 +1,33 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.2.3 Summary:
 ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: Cvandia Author-email:
 106718176+Cvandia@users.noreply.github.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.0.0-beta.1) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.1.3) Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist:
-pathlib (>=1.0.1) Requires-Dist: pydantic (>=1.10.2) Requires-Dist: ujson
-(>=5.5.0) Description-Content-Type: text/markdown
+apscheduler (>=0.1.3) Requires-Dist: nonebot-plugin-templates (>=0.1.3,<0.2.0)
+Requires-Dist: nonebot2 (>=2.0.0-beta.1) Requires-Dist: pathlib (>=1.0.1)
+Requires-Dist: pydantic (>=1.10.2) Requires-Dist: ujson (>=5.5.0) Description-
+Content-Type: text/markdown ![056131D4](https://github.com/Cvandia/
+nonebot_plugin_genshin_cos/assets/106718176/da116fce-d24f-4f89-8f6c-
+1f2509fd56be)
                               [NoneBotPluginLogo]
                          # nonebot-plugin-genshin-cos
           _â­åºäºNonebot2çä¸æ¬¾è·åç±³æ¸¸ç¤¾cosçæä»¶â­_
 [https://img.shields.io/badge/python-3.8+-blue] [https://img.shields.io/badge/
 QQ-1141538825-yellow] [https://img.shields.io/badge/license-MIT-blue] [https://
                     img.shields.io/badge/Nonebot2-rc1+-red]
 ## â­ ä»ç» åå°[æç¨](https://juejin.cn/post/
 6990320268010848286)çå¯åï¼æä»¥åäºè¿ä¸ªæä»¶ï¼æ´å¤åè½åç»­æ´æ°~~æå¾æï¼å­¦ä¸é~~
   ### æèä½ æå¥å³äºè¯¥æä»¶çæ°æ³æ³çï¼å¯ä»¥æissueæèpr
-                                     (>A<)
+                                   (>A<) ###
+ ä¸ä»æåç¥ï¼ç°å¨æ¯æå´©å3ãæç©¹ééãå¤§å«éçcoså¾ï¼
 ## ð¿ å®è£  å®è£ pip å®è£ ``` pip install nonebot-plugin-genshin-cos
 ``` - å¨nonebotçpyproject.tomlä¸­çplugins = ["xxx"]æ·»å æ­¤æä»¶ nb-
 cliå®è£ ``` nb plugin install nonebot-plugin-genshin-cos --upgrade ``` git
 cloneå®è£(ä¸æ¨è) - è¿è¡ ```git clone https://github.com/Cvandia/
 nonebot_plugin_genshin_cos``` - å¨è¿è¡å¤ ææä»¶å¤¹`nonebot-plugin-
 genshen-cos`å¤å¶å°botæ ¹ç®å½ä¸ç`src/plugins`
 (æèä½ åå»ºbotæ¶çå¶ä»åç§°`xxx/plugins`)   æ³¨æ
```

