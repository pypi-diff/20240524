# Comparing `tmp/nonebot-plugin-hx-yinying-1.3.12.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.3.12.tar", last modified: Tue May 21 14:36:57 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.3.13.tar", last modified: Fri May 24 11:17:49 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.3.12.tar` & `nonebot-plugin-hx-yinying-1.3.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:57.638136 nonebot-plugin-hx-yinying-1.3.12/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.3.12/LICENSE
--rw-rw-rw-   0        0        0     6677 2024-05-21 14:36:57.638136 nonebot-plugin-hx-yinying-1.3.12/PKG-INFO
--rw-rw-rw-   0        0        0     6236 2024-05-20 15:06:16.000000 nonebot-plugin-hx-yinying-1.3.12/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:57.483720 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    55519 2024-05-21 12:59:58.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    76527 2024-05-21 06:51:15.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0     1628 2024-05-21 14:36:15.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/image_check.py
--rw-rw-rw-   0        0        0     3871 2024-05-21 05:58:22.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/report.py
--rw-rw-rw-   0        0        0     5032 2024-05-12 17:16:42.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/smms.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:57.625861 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     6677 2024-05-21 14:36:56.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-21 14:36:57.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:36:56.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-21 14:36:56.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-21 14:36:56.000000 nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-21 14:36:57.652981 nonebot-plugin-hx-yinying-1.3.12/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-21 14:35:51.000000 nonebot-plugin-hx-yinying-1.3.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:17:49.861822 nonebot-plugin-hx-yinying-1.3.13/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.3.13/LICENSE
+-rw-rw-rw-   0        0        0     6677 2024-05-24 11:17:49.862857 nonebot-plugin-hx-yinying-1.3.13/PKG-INFO
+-rw-rw-rw-   0        0        0     6236 2024-05-20 15:06:16.000000 nonebot-plugin-hx-yinying-1.3.13/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 11:17:49.691833 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    59273 2024-05-24 11:16:06.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    73937 2024-05-24 11:15:53.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0     1592 2024-05-24 09:43:06.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2347 2024-05-24 11:11:16.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     3823 2024-05-24 10:41:20.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/report.py
+-rw-rw-rw-   0        0        0     5288 2024-05-24 11:07:56.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/smms.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:17:49.840422 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     6677 2024-05-24 11:17:48.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-24 11:17:49.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 11:17:48.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-24 11:17:48.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 11:17:48.000000 nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-24 11:17:49.878841 nonebot-plugin-hx-yinying-1.3.13/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-24 11:17:41.000000 nonebot-plugin-hx-yinying-1.3.13/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/LICENSE` & `nonebot-plugin-hx-yinying-1.3.13/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.12/PKG-INFO` & `nonebot-plugin-hx-yinying-1.3.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.3.12
+Version: 1.3.13
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.12 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.13 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/README.md` & `nonebot-plugin-hx-yinying-1.3.13/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from nonebot.typing import T_State
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.rule import to_me,Rule
 import json,random
 from .config import Config
 from .chat import *
-from .report import error_oops
+from .report import error_oops,get_file
+hx_config = get_plugin_config(Config)
 
 __plugin_meta__ = PluginMetadata(
     name="Hx_YinYing",
     description="快来和可爱的赛博狼狼聊天！",
     usage=(
         "通过QQ艾特机器人来进行对话"
     ),
@@ -30,62 +31,85 @@
     homepage="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     config=Config,
     supported_adapters={
         "~onebot.v11"
     },
 )
 
-hx_config = get_plugin_config(Config)
+#awa--------味大，无需多盐！
+logger.opt(colors=True).success( f"""
+    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
+<fg #60F5F5>,--,                                                                                                 </fg #60F5F5>                 
+<r>      ,--.'|                                       ,--,     ,--,                                 ,---,.               ___   </r> 
+<y>   ,--,  | :                                       |'. \   / .`|  ,--,                         ,'  .'  \            ,--.'|_   </y>
+<g>,---.'|  : '         ,--,                    ,---, ; \ `\ /' / ;,--.'|         ,---,         ,---.' .' |   ,---.    |  | :,' </g> 
+<c>|   | : _' |       ,'_ /|                ,-+-. /  |`. \  /  / .'|  |,      ,-+-. /  |        |   |  |: |  '   ,'\   :  : ' :  </c>
+<e>:   : |.'  |  .--. |  | :    ,--.--.    ,--.'|'   | \  \/  / ./ `--'_     ,--.'|'   |        :   :  :  / /   /   |.;__,'  /   </e>
+<m>|   ' '  ; :,'_ /| :  . |   /       \  |   |  ,"' |  \  \.'  /  ,' ,'|   |   |  ,"' |        :   |    ; .   ; ,. :|  |   |    </m>
+<e>'   |  .'. ||  ' | |  . .  .--.  .-. | |   | /  | |   \  ;  ;   '  | |   |   | /  | |        |   :     \'   | |: ::__,'| :    </e>
+<c>|   | :  | '|  | ' |  | |   \__\/: . . |   | |  | |  / \  \  \  |  | :   |   | |  | |        |   |   . |'   | .; :  '  : |__  </c>
+<g>'   : |  : ;:  | : ;  ; |   ," .--.; | |   | |  |/  ;  /\  \  \ '  : |__ |   | |  |/         '   :  '; ||   :    |  |  | '.'| </g>
+<y>|   | '  ,/ '  :  `--'   \ /  /  ,.  | |   | |--' ./__;  \  ;  \|  | '.'||   | |--'          |   |  | ;  \   \  /   ;  :    ; </y>
+<r>;   : ;--'  :  ,      .-./;  :   .'   \|   |/     |   : / \  \  ;  :    ;|   |/              |   :   /    `----'    |  ,   /  </r>
+<m>|   ,/       `--`----'    |  ,     .-./'---'      ;   |/   \  ' |  ,   / '---'               |   | ,'                ---`-'   </m>
+<r>'---'                      `--`---'               `---'     `--` ---`-'                      `----'</r>
+    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
+""")
+
+
 global_config = config_in_global()
 dy_list = json_get(config_in_global(),"dy_list")
 log_dir = path_in()
-   
-#检查关键配置
+
+#检查关键配置，自动更新-0.2day
 if not hx_config.yinying_appid or not hx_config.yinying_token:
     logger.error("未设置核心配置？！,请检查你配置里的yinying_appid和yinying_token")
 else:
-    logger.opt(colors=True).success("【Hx】加载核心配置成功")
-
+    scheduler.add_job(func=check_update,trigger='interval',hours=3,id="huanxin996")
+    logger.opt(colors=True).success(f"【Hx】定时检测更新启动。")
+    logger.opt(colors=True).success("【Hx】加载核心配置成功,定时检测更新启动。")
 
 #检测更新
 try:
     check_update()
 except Exception as e:
     logger.opt(colors=True).error("【Hx】检测更新失败！！，联系开发者！错误捕获{e}")
 
-#尝试自动更新-0.2day
-try:
-    scheduler.add_job(func=check_update,trigger='interval',hours=3,id="huanxin996")
-    logger.opt(colors=True).success(f"【Hx】定时检测更新启动。")
-except Exception as e:
-    logger.opt(colors=True).error(f"【Hx】定时检测更新启动失败！！，联系开发者！错误捕获{e}")
+#尝试检查错误模块
+if os.path.exists(f"{log_dir}/file/error_report/hx_error.html"):
+    logger.success("已加载错误报告模块")
+else:
+    logger.error("未找到错误报告模块的文件，尝试下载。。。")
+    get_file()
+
 
 #根据订阅信息注册定时任务
 try:
     extent = int(len(dy_list))
     for key in dy_list:
         config_1 = config_in_user(key,False)
         user_config = json_get(config_1,key)
-        config_time = json_get_time(user_config,"dy_time")
-        config_minute = json_get_time(user_config,"dy_minute")
+        config_time = json_get_pro(user_config,"dy_time")
+        config_minute = json_get_pro(user_config,"dy_minute")
         scheduler.add_job(func=get_chat,trigger='interval',args=[key] ,hours=config_time, minutes=config_minute, id=key)
     logger.opt(colors=True).success(f"【Hx】定时任务加载成功,当前共加载{extent}个订阅用户")
 except Exception as e:
     logger.opt(colors=True).error(f"【Hx】定时任务加载失败！！，联系开发者！错误捕获{e}")
 
-
+#加载自定义文件集
 if hx_config.hx_chatcommand:
     logger.success(f"【Hx】命令列表加载成功,当前自定义命令列表为{hx_config.hx_chatcommand}")
     ml_st = hx_config.hx_chatcommand
 else:
     logger.error(f"【Hx】命令列表加载失败，请检查配置文件")
     ml_st = {'hx','chat'}
 
 
 #主要命令列表
+help = on_command("yy帮助", aliases={"yinyinghelp","hx_help","hx_yinying_help"},rule=Rule(chek_rule_base),  priority=0, block=True)
 msg_at = on_message(rule=Rule(chek_rule_base)&to_me(), priority=10,  block=True)
 msg_ml = on_command("yinying_chat", aliases=ml_st,rule=Rule(chek_rule_base),  priority=15, block=True)
 clear =  on_command("刷新对话", aliases={"clear"},rule=Rule(chek_rule_base),  priority=0, block=True)
 history_get = on_command("导出对话", aliases={"getchat"},rule=Rule(chek_rule_base),  priority=0, block=True)
 set_global_config = on_command("设置全局配置", aliases={"设置配置全局","globalset"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 model_list = on_command("模型列表", aliases={"modellist","chat模型列表"},rule=Rule(chek_rule_base),  priority=0, block=True)
 model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型","模型切换"},rule=Rule(chek_rule_base),  priority=0, block=True)
@@ -93,16 +117,40 @@
 cyber_set = on_command("cyber", aliases={"cyber设置","Hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
 admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"},rule=Rule(chek_rule_base),  priority=0, block=True)
 character = on_command("sd", aliases={"旅行伙伴加入","设定加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
 chat_ne = on_command("加入订阅", aliases={"旅行伙伴觉醒","订阅加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
 time_noend = on_command("切换时间线", aliases={"切换模式"},rule=Rule(chek_rule_base),  priority=0, block=True)
 gloubalblack_add = on_command("全局拉黑", aliases={"银影不要理"},rule=Rule(chek_rule_admin),  priority=0, block=True)
+banword_add = on_command("添加违禁词", aliases={"banword","违禁词添加"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 ces = on_command("测试服务", aliases={"测试报错"},rule=Rule(chek_rule_base), priority=0, block=True)
 
+@help.handle()
+async def help(matcher: Matcher,event: MessageEvent):
+    msg = "-----帮助列表-----\n刷新对话\n导出对话\n设置全局配置\n模型列表\n切换模型\neasycyber\ncyber\n控制台操作\n确认版本\n旅行伙伴加入\n切换时间线\n全局拉黑\n添加违禁词\n-----(点头)-----"
+    await send_msg(matcher, event, msg)
+
+#添加违禁词。
+@banword_add.handle()
+async def banword_add(matcher: Matcher,event: MessageEvent, msg: Message = CommandArg()):
+    text = msg.extract_plain_text()
+    config_1 = config_in_global()
+    banword = json_get(config_1,"blacklist_world")
+    if not text:
+        msg= f"咱不知道要添加什么违禁词哦。"
+    else:
+        if text in banword:
+            await send_msg(matcher, event, f"{text}已在违禁词列表里了！")
+        banword.append(text)
+        config_1["blacklist_world"] = banword
+        with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+            json.dump(config_1,file)
+            msg= f"{text}已添加到违禁词列表里"
+    await send_msg(matcher, event, msg)
+
 #生命模式-无限时间(仅供cyber和easycyber使用)
 @time_noend.got(
     "msg",
     prompt=f"请输入时间线\n当前仅支持\n无限-overworld\n普通-nether\n请输入全称：无限-overworld",
 )
 async def time_noend(matcher: Matcher,bot:Bot, event: MessageEvent):
     text = unescape(event.get_plaintext().strip())
@@ -147,16 +195,15 @@
         user_config.append(text)
         config_1["blacklist_user"] = user_config
         with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
             json.dump(config_1,file)
             msg= f"{text}拉黑成功"
     await send_msg(matcher, event, msg)
 
-
-#自定义自己的设定
+#自定义自己的设定和昵称
 @character.handle()
 async def character(matcher: Matcher,bot:Bot, event: MessageEvent, msg: Message = CommandArg()):
     user = get_id(event)
     nick = await get_nick(bot,event)
     config = config_in_user(user,nick)
     config_get = json_get(config,user)
     text = msg.extract_plain_text()
@@ -301,16 +348,16 @@
     id = get_id(event)
     text = unescape(event.get_plaintext().strip())
     if "last" not in s:
         s["last"] = ""
     if s["last"]:
         if s["last"] == "查看":
             config = config_in_global()
-            get_config = await json_get_text(config,text)
-            if get_config == 0:
+            get_config = await json_get_pro(config,text)
+            if get_config == 2:
                 s["last"] = True
                 msg = f"无法查找到该配置项！，请检查其是否为正确的配置名{text}"
                 await send_msg(matcher,event,msg)
             else:
                 s["last"] = True
                 msg = f"{text}状态为:{get_config}"
                 await send_msg(matcher,event,msg)
@@ -343,15 +390,15 @@
                     msg = "无法查找到该配置项！，请检查其是否为正确的配置名,请重新输入！\n如需退出请发送退出"
                     await send_msg_reject(matcher,event,msg)
                     return
         
         if s["last"] == "修改TF":
             config = config_in_global()
             config_name = s["set"]
-            get_config = await json_get_text(config,config_name)
+            get_config = await json_get_pro(config,config_name)
             logger.debug(f"{get_config}")
             key = {"on":False,"off":False,"开":True,"关":False,"开启":True,"关闭":False}
             if text in key:
                 s["last"] = True
                 text = key[f"{text}"]
                 if get_config and text:
                     msg = f"该配置项[{config_name}]已经开启了，不需要重复开启噢"
@@ -372,15 +419,15 @@
             await send_msg(matcher,event,msg) 
                 
      
         
         if s["last"] == "修改w":
             config = config_in_global()
             config_name = s["set"]
-            get_config = await json_get_text(config,config_name)
+            get_config = await json_get_pro(config,config_name)
             config[f"{config_name}"] = int(text)
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                 json.dump(config,file)
             msg = f"{config_name}的id已更改为{text}"
             s["last"] = True
             await send_msg(matcher,event,msg)
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,127 +1,85 @@
 # -- coding: utf-8 --**
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent ,MessageSegment ,Message,MessageEvent,Event
 from html import unescape
 from typing import List,Set
 import os,httpx, json, time, requests,platform
-from loguru import logger as lg
 from .config import Config
 import operator,nonebot,random
 from nonebot import get_plugin_config, logger, require,get_driver
 from pathlib import Path
 require("nonebot_plugin_localstore")
 import nonebot_plugin_localstore as store
 from .image_check import image_check
 from .report import error_oops
-
-
 hx_config = get_plugin_config(Config)
 
-#判断主要配置文件夹是否存在！
-if hx_config.hx_path == None:
-    logger.warning("找不到配置里的路径，将使用默认配置")
-    lg.opt(colors=True).success( f"""
-    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
-<fg #60F5F5>,--,                                                                                                 </fg #60F5F5>                 
-<r>      ,--.'|                                       ,--,     ,--,                                 ,---,.               ___   </r> 
-<y>   ,--,  | :                                       |'. \   / .`|  ,--,                         ,'  .'  \            ,--.'|_   </y>
-<g>,---.'|  : '         ,--,                    ,---, ; \ `\ /' / ;,--.'|         ,---,         ,---.' .' |   ,---.    |  | :,' </g> 
-<c>|   | : _' |       ,'_ /|                ,-+-. /  |`. \  /  / .'|  |,      ,-+-. /  |        |   |  |: |  '   ,'\   :  : ' :  </c>
-<e>:   : |.'  |  .--. |  | :    ,--.--.    ,--.'|'   | \  \/  / ./ `--'_     ,--.'|'   |        :   :  :  / /   /   |.;__,'  /   </e>
-<m>|   ' '  ; :,'_ /| :  . |   /       \  |   |  ,"' |  \  \.'  /  ,' ,'|   |   |  ,"' |        :   |    ; .   ; ,. :|  |   |    </m>
-<e>'   |  .'. ||  ' | |  . .  .--.  .-. | |   | /  | |   \  ;  ;   '  | |   |   | /  | |        |   :     \'   | |: ::__,'| :    </e>
-<c>|   | :  | '|  | ' |  | |   \__\/: . . |   | |  | |  / \  \  \  |  | :   |   | |  | |        |   |   . |'   | .; :  '  : |__  </c>
-<g>'   : |  : ;:  | : ;  ; |   ," .--.; | |   | |  |/  ;  /\  \  \ '  : |__ |   | |  |/         '   :  '; ||   :    |  |  | '.'| </g>
-<y>|   | '  ,/ '  :  `--'   \ /  /  ,.  | |   | |--' ./__;  \  ;  \|  | '.'||   | |--'          |   |  | ;  \   \  /   ;  :    ; </y>
-<r>;   : ;--'  :  ,      .-./;  :   .'   \|   |/     |   : / \  \  ;  :    ;|   |/              |   :   /    `----'    |  ,   /  </r>
-<m>|   ,/       `--`----'    |  ,     .-./'---'      ;   |/   \  ' |  ,   / '---'               |   | ,'                ---`-'   </m>
-<r>'---'                      `--`---'               `---'     `--` ---`-'                      `----'</r>
-    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
-""")
-    history_dir = store.get_data_dir("Hx_YingYing")
-    log_dir = Path(f"{history_dir}/yinying_chat").absolute()
-    log_dir.mkdir(parents=True, exist_ok=True)
-else:
-    lg.opt(colors=True).success( f"""
-    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
-<fg #60F5F5>,--,                                                                                                 </fg #60F5F5>                 
-<r>      ,--.'|                                       ,--,     ,--,                                 ,---,.               ___   </r> 
-<y>   ,--,  | :                                       |'. \   / .`|  ,--,                         ,'  .'  \            ,--.'|_   </y>
-<g>,---.'|  : '         ,--,                    ,---, ; \ `\ /' / ;,--.'|         ,---,         ,---.' .' |   ,---.    |  | :,' </g> 
-<c>|   | : _' |       ,'_ /|                ,-+-. /  |`. \  /  / .'|  |,      ,-+-. /  |        |   |  |: |  '   ,'\   :  : ' :  </c>
-<e>:   : |.'  |  .--. |  | :    ,--.--.    ,--.'|'   | \  \/  / ./ `--'_     ,--.'|'   |        :   :  :  / /   /   |.;__,'  /   </e>
-<m>|   ' '  ; :,'_ /| :  . |   /       \  |   |  ,"' |  \  \.'  /  ,' ,'|   |   |  ,"' |        :   |    ; .   ; ,. :|  |   |    </m>
-<e>'   |  .'. ||  ' | |  . .  .--.  .-. | |   | /  | |   \  ;  ;   '  | |   |   | /  | |        |   :     \'   | |: ::__,'| :    </e>
-<c>|   | :  | '|  | ' |  | |   \__\/: . . |   | |  | |  / \  \  \  |  | :   |   | |  | |        |   |   . |'   | .; :  '  : |__  </c>
-<g>'   : |  : ;:  | : ;  ; |   ," .--.; | |   | |  |/  ;  /\  \  \ '  : |__ |   | |  |/         '   :  '; ||   :    |  |  | '.'| </g>
-<y>|   | '  ,/ '  :  `--'   \ /  /  ,.  | |   | |--' ./__;  \  ;  \|  | '.'||   | |--'          |   |  | ;  \   \  /   ;  :    ; </y>
-<r>;   : ;--'  :  ,      .-./;  :   .'   \|   |/     |   : / \  \  ;  :    ;|   |/              |   :   /    `----'    |  ,   /  </r>
-<m>|   ,/       `--`----'    |  ,     .-./'---'      ;   |/   \  ' |  ,   / '---'               |   | ,'                ---`-'   </m>
-<r>'---'                      `--`---'               `---'     `--` ---`-'                      `----'</r>
-    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
-""")
-    logger.success("找到配置里的路径，载入成功")
-    history_dir = store.get_data_dir(f"{hx_config.hx_path}")
-    log_dir = Path(f"{history_dir}/yinying_chat").absolute()
-    log_dir.mkdir(parents=True, exist_ok=True)
-
-def number_suiji():
-    digits = "0123456789"
-    str_list =[random.choice(digits) for i in range(3)]
-    random_str =''.join(str_list)
-    return random_str
-
-#判断模型
-def model_got(msg) -> str:
-    back = "yinyingllm-v2"
-    try:
-        if msg == "1" or msg == "yinyingllm-v1" or msg == "yinyingllmv1":
-            back = "yinyingllm-v1"
-        elif msg == "2" or msg == "yinyingllm-v2" or msg == "yinyingllmv2":
-            back = "yinyingllm-v2"
-        elif msg == "3" or msg == "yinyingllm-v3" or msg == "yinyingllmv3":
-            back = "yinyingllm-v3"
-        elif msg == "4" or msg == "cyberfurry-001" or msg == "cyberfurry001" or msg == "cyberfurry1":
-            back = "cyberfurry-001"
-        elif msg == "5" or msg == "easycyberfurry-001" or msg == "easycyberfurry001" or msg == "easycyberfurry1":
-            back = "easycyberfurry-001"
-    except Exception as e:
-        return f"{e}"
-    return back
-
 #path---in
 def path_in() -> str:
+    """
+    区分win和lin载入路径
+    """
     sys = platform.system()
     if sys == "Windows":
         if hx_config.hx_path == None:
             history_dir = store.get_data_dir("Hx_YingYing")
             log_dir = Path(f"{history_dir}/yinying_chat").absolute()
             log_dir.mkdir(parents=True, exist_ok=True)
-            return log_dir
         else:
             history_dir = store.get_data_dir(f"{hx_config.hx_path}")
             log_dir = Path(f"{history_dir}/yinying_chat").absolute()
             log_dir.mkdir(parents=True, exist_ok=True)
-            return log_dir
     elif sys == "Linux":
         if hx_config.hx_path == None:
             history_dir = store.get_data_dir("Hx_YingYing")
             log_dir = Path(f"{history_dir}/yinying_chat").absolute()
             log_dir.mkdir(parents=True, exist_ok=True)
             log_dir = Path(f"{history_dir}/yinying_chat").as_posix()
-            return log_dir
         else:
             history_dir = store.get_data_dir(f"{hx_config.hx_path}")
             log_dir = Path(f"{history_dir}/yinying_chat").absolute()
             log_dir.mkdir(parents=True, exist_ok=True)
             log_dir = Path(f"{history_dir}/yinying_chat").as_posix()
-            return log_dir
+    return log_dir
+
+#判断主要配置文件夹是否存在！
+log_dir = path_in()
+
+def number_suiji():
+    """
+    随机数生成
+    """
+    digits = "0123456789"
+    str_list =[random.choice(digits) for i in range(3)]
+    random_str =''.join(str_list)
+    return random_str
+
+#判断模型
+def model_got(msg) -> str:
+    """
+    进行一个模型的切换！
+    """
+    back = "yinyingllm-v2"
+    if msg == "1" or msg == "yinyingllm-v1" or msg == "yinyingllmv1":
+        back = "yinyingllm-v1"
+    elif msg == "2" or msg == "yinyingllm-v2" or msg == "yinyingllmv2":
+        back = "yinyingllm-v2"
+    elif msg == "3" or msg == "yinyingllm-v3" or msg == "yinyingllmv3":
+        back = "yinyingllm-v3"
+    elif msg == "4" or msg == "cyberfurry-001" or msg == "cyberfurry001" or msg == "cyberfurry1":
+        back = "cyberfurry-001"
+    elif msg == "5" or msg == "easycyberfurry-001" or msg == "easycyberfurry001" or msg == "easycyberfurry1":
+        back = "easycyberfurry-001"
+    return back
 
 #update-----Hx
 def update_hx():
+    """
+    检查pypi插件最新版本
+    """
     fails = 0
     while True:
         try:
             if fails >= 20:
                 verision = False
                 time = False
                 break
@@ -212,53 +170,70 @@
             if (seg.type == "image") and ("url" in seg.data)
         ]
     )
     return urls
 
 #创建用户文件夹
 def create_dir_usr(path):
+    """
+    创建文件夹（绝对路径）
+    """
     if not os.path.exists(path):
         os.mkdir(path)
 
 #获取json函数
 def json_get(data, *keys, default=None):
+    """
+    从json中遍历获取数据
+    """
     try:
         for key in keys:
             try:
                 data = data[key]
             except KeyError:
                 return default
         return data
     except Exception as e:
         return False
 
-async def json_get_text(json,key) -> str:
+async def json_get_pro(json,key) -> str:
+    """
+    从json获取数据的补充
+    """
     try:
         back = json[f"{key}"]
     except Exception as e:
-        back = 0
+        back = 2
     return back
 
-def json_get_time(json,key) -> str:
-    try:
-        back = json[f"{key}"]
-    except Exception as e:
-        back = 1
-    return back
+#违禁词剔除函数
+def ban_word(text:str) -> str:
+    """
+    违禁词剔除函数
+    """
+    ban_word_list = json_get(config_in_global(),"blacklist_world")
+    for i in ban_word_list:
+        if i in text:
+            text = text.replace(i,"w")
+    return text
 
 #json转义防止爆炸（）
 def json_replace(text) -> str:
-    text = text.replace('\n','/n')
-    text = text.replace('\t','/t')
+    """
+    移除',"导致的转义问题
+    """
     text = text.replace("'","/'")
     text = text.replace('"','/"')
     return text
 
 #初始化log记录
 def log_in()-> str:
+    """
+    初始化聊天记录
+    """
     try:
         if os.path.exists(f"{log_dir}/chat/all_log.json"):
             with open(f'{log_dir}/chat/all_log.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 back = json_data
         else:
             create_dir_usr(f'{log_dir}/chat')
@@ -285,14 +260,17 @@
                     json_data['114514'] = history_package
                     json.dump(json_data,file)
                     back = json_data
     return back
 
 #检查更新
 def check_update():
+    """
+    检查插件更新
+    """
     new_verision, time = update_hx()
     if not new_verision and not time:
         logger.error(f"[Hx_YinYing]:无法获取最新的版本，当前版本为{hx_config.hx_version}，可能已经过时！")
     else:
         if new_verision <= hx_config.hx_version:
             logger.success(f"[Hx_YinYing]:你的Hx_YinYing已经是最新版本了！当前版本为{hx_config.hx_version},仓库版本为{new_verision}")
         else:
@@ -307,14 +285,17 @@
                 logger.warning("【Hx】正在自动更新中--未找到虚拟环境！[安装在本地环境]")
                 os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
                 logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
                 logger.warning(f"[Hx_YinYing]:你可能需要重新启动nonebot来完成插件的重载")
 
 #载入本地保存的easycyber预设(一些情况下失败时不会清空，请找到专业人员修复)
 def easycyber_in(cybernick,json_1) -> str:
+    """
+    载入本地保存的easycyber预设(一些情况下失败时不会清空，请找到专业人员修复)
+    """
     try:
         if os.path.exists(f"{log_dir}/config/easycyber.json"):
             with open(f'{log_dir}/config/easycyber.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
                 else:
@@ -379,14 +360,17 @@
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             back = False
     return back
 
 #载入本地投稿的easycyber预设(载入失败会被清空
 def easycyber_in_tg(cybernick,json_1) -> str:
+    """
+    载入本地投稿的easycyber预设(载入失败会被清空
+    """
     t = time.time()
     try:
         if os.path.exists(f"{log_dir}/file/easycyber_tg.json"):
             with open(f'{log_dir}/file/easycyber_tg.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
@@ -446,14 +430,17 @@
                     json.dump(global_easycyberfurry,file)
                     back = global_easycyberfurry
                 back = False
     return back
 
 #载入本地保存的cyber预设(一些情况下失败时不会清空，请找到专业人员修复)
 def cyber_in(cybernick,json_1) -> str:
+    """
+    载入本地保存的cyber预设(一些情况下失败时不会清空，请找到专业人员修复)
+    """
     try:
         if os.path.exists(f"{log_dir}/config/cyber.json"):
             with open(f'{log_dir}/config/cyber.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
                 else:
@@ -512,14 +499,17 @@
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             back = False
     return back
 
 #载入本地投稿的cyber预设(载入失败会被清空
 def cyber_in_tg(cybernick,json_1) -> str:
+    """
+    载入本地投稿的cyber预设(载入失败会被清空
+    """
     t = time.time()
     try:
         if os.path.exists(f"{log_dir}/file/cyber_tg.json"):
             with open(f'{log_dir}/file/cyber_tg.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
@@ -571,14 +561,17 @@
                     json.dump(global_easycyberfurry,file)
                     back = global_easycyberfurry
                 back = False
     return back
 
 #载入全局本地配置
 def config_in_global() -> str:
+    """
+    载入全局配置，失败时会重置
+    """
     try:
         json_data = {}
         admin_user = []
         black_user = []
         black_group = []
         black_world = []
         white_group = []
@@ -619,14 +612,17 @@
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
                 json.dump(json_data,file)
                 back = json_data
     return back
 
 #载入群聊本地配置
 def config_in_group(groupid) -> str:
+    """
+    载入群组本地配置，失败会重置
+    """
     dt = time.time()
     t = int(dt)
     id_package = {}
     id_package['use_model'] = "yinyingllm-v2"
     id_package['character_in'] = True
     id_package['easycharacter_in'] = True
     id_package['chat_alltimes'] = 0
@@ -659,14 +655,17 @@
                 json_data[f"{groupid}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     return back
 
 #载入个人本地配置
 def config_in_user(id,nick) -> str:
+    """
+    载入个人本地配置，失败会重置
+    """
     dt = time.time()
     t = int(dt)
     id_package = {}
     id_package['character'] = f"我是一只可爱的毛毛龙嗷呜"
     id_package['character_in'] = True
     id_package['easycharacter_in'] = True
     id_package['private_model'] = "yinyingllm-v2"
@@ -719,24 +718,30 @@
                 json_data[f"{id}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     return back
 
 #结果消息函数，发送消息直接await就行
 async def send_msg_reject(matcher, event, content):
+    """
+    结束---发送消息
+    """
     config_global = config_in_global()
     reply_config = json_get(config_global,"reply")
     if reply_config == True:
         await matcher.reject(MessageSegment.reply(event.message_id) + content)
     else:
         reply_at = json_get(config_global,"reply_at")
         await matcher.reject(content, at_sender=reply_at)
 
 #用户输入
 def user_in(id, text):
+    """
+    记录用户输入内容
+    """
     data = log_in()
     config = config_in_user(id,False)
     line = config[f'{id}']['world_timeline']
     package = {}
     package['rule'] = 'user'
     text_r = json_replace(text)
     package['msg'] = f'{text_r}'
@@ -760,17 +765,19 @@
             with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file, open(f'{log_dir}/user/{id}/{line}.txt','a+',encoding='utf-8') as w:
                 json.dump(data,file)
                 w.write(f"\n[{id}]:{text}\n")
     except Exception as e:
         logger.warning(f"用户{id}配置文件写入失败，{e}，尝试创建文件夹")
         create_dir_usr(f'{log_dir}/user/{id}')
 
-
 #AI输出
 def ai_out(id, text):
+    """
+    记录ai输入内容
+    """
     data = log_in()
     config = config_in_user(id,False)
     line = config[f'{id}']['world_timeline']
     package = {}
     package['rule'] = 'ai'
     text_r = json_replace(text)
     package['msg'] = f'{text_r}'
@@ -796,14 +803,17 @@
                 w.write(f"[bot]:{text}")
     except Exception as e:
         logger.warning(f"用户{id}配置文件写入失败，{e}，尝试创建文件夹")
         create_dir_usr(f'{log_dir}/user/{id}')
 
 #获取配置内键值并列表化
 async def config_list(config):
+    """
+    列表化config里的项
+    """
     try:
         tf_key = []
         w_key = []
         list_key = []
         if config:
             for key in config:
                 get_config = json_get(config,format(key))
@@ -820,27 +830,33 @@
     except Exception as e:
         logger.warning(f"报错捕获{e}")
         logger.error(f"报错定位于获取配置内鉴值")
     return tf_key, w_key, list_key
 
 #获取nonebot超级管理组
 def get_superuser() -> list:
+    """
+    获取nonebot超级管理组
+    """
     list_superuser = get_driver().config.superusers
     try:
         if list_superuser == None or not list_superuser:
             superuser = ["3485462167"]
         else:
             superuser = get_driver().config.superusers
     except Exception as e:
             logger.warning(f"报错捕获{e}")
             superuser = ["3485462167"]
     return superuser
 
 #全局权限检查！！！！！（总算写出来了）
 def place(id) -> int:
+    """
+    权限检查。。
+    """
     try:
         config = config_in_global()
         admin_pro = json_get(config,"admin_pro")
         admin_user = json_get(config,"admin_user")
         black_list = json_get(config,"blacklist_user")
         superuser = get_superuser()
         logger.warning(f"user捕获{superuser}")
@@ -856,14 +872,17 @@
             return 5
     except Exception as e:
             logger.warning(f"报错捕获{e}")
             return 5
 
 #rule---管理组
 async def chek_rule_admin(event:MessageEvent):
+    """
+    检查管理权限
+    """
     id = get_id(event)
     config = config_in_global()
     admin_list = json_get(config,"admin_user")
     admin_pro = json_get(config,"admin_pro")
     supuser = get_superuser()
     try:
         if id in admin_list or id == admin_pro or id in supuser:
@@ -873,14 +892,17 @@
     except Exception as e:
             logger.error(f"报错捕获{e}")
             logger.error(f"你的配置文件错误或已过时！！，权限控制失效！")
             return True
 
 #rule---用户组
 async def chek_rule_base(event:MessageEvent,eve:Event):
+    """
+    检查用户权限
+    """
     try:
         id = get_id(event)
         group_id = get_groupid(event)
         config = config_in_global()
         admin_list = json_get(config, "admin_user")
         admin_pro = json_get(config, "admin_pro")
         superuser = get_superuser()
@@ -895,16 +917,14 @@
             is_admin = id in admin_list or id == admin_pro or id in superuser
             is_white = group_id in white_group or id in white_user
             is_black = group_id not in black_group or id not in black_user
             is_private = private if isinstance(eve, GroupMessageEvent) else True
             is_bot = id is not eve.self_id
             if to_me and isinstance(eve, GroupMessageEvent):
                 return is_admin or is_white or (at_reply and is_bot and is_black)
-            if isinstance(eve, GroupMessageEvent):
-                return is_admin or is_white or (is_bot and is_black)
             return is_admin or is_white or (is_private and is_black and is_bot)
         if isinstance(eve, GroupMessageEvent):
             to_me = event.to_me
             if rule_mode == "white":
                 return check_user_group_rules(to_me) or group_id in white_group
             else:
                 return check_user_group_rules(to_me)
@@ -913,26 +933,32 @@
         else:
             return check_user_group_rules(True)
     except Exception as e:
         logger.error(f"配置验证异常: {str(e)}")
         return True
 
 #尝试获取bot本地文件夹文件
-def file_get(file) -> str:
+async def file_get(file) -> str:
+    """
+    尝试获取bot本地文件夹文件
+    """
     try:
         if os.path.exists(f"{log_dir}/file/{file}"):
             back = f"{log_dir}/file/{file}"
         else:
             back = False
     except Exception as e:
         back = False
     return back
 
 #历史消息卡片构建
 async def get_history(id,bot,event) -> List[MessageSegment]:
+    """
+    构建消息记录转发
+    """
     date = log_in()
     log_list = date[f"{id}"]["log"]
     t = len(log_list)
     nick = await get_nick(bot,event)
     msg_list = []
     try:
         for item in log_list:
@@ -966,26 +992,32 @@
                 nickname="AAA星佑批发（幻歆限定）",
                 content=Message("合并消息时出错！"),
             )
         ]
     return msg_list
 
 #历史消息文件获取
-def gethistorytxt(id,filename):
+async def gethistorytxt(id,filename):
+    """
+    获取文件类型的聊天记录
+    """
     file_path=f"{log_dir}  / user / {id}"
     if not os.path.exists(f"{file_path}"):
         create_dir_usr(f"{file_path}")
     filelist = os.listdir(file_path)
     if filename+".json" in filelist:
         return file_path / (filename+".json")
     else:
         return False
 
 #全局配置卡片构建
 async def get_config_global() -> List[MessageSegment]:
+    """
+    构建全局配置卡片
+    """
     config = config_in_global()
     msg_list = []
     try:
         reply = config["reply"]
         reply_at = config["reply_at"]
         global_switch = config["global_switch"]
         private = config["private"]
@@ -1078,14 +1110,17 @@
                 content=Message("获取全局配置合并消息时出错！"),
             )
         ]
     return msg_list
 
 #获取纯文本
 async def gen_chat_text(event, bot: Bot) -> str:
+    """
+    提取消息内纯文本
+    """
     msg = ""
     for seg in event.message:
         if seg.is_text():
             msg += seg.data.get("text", "")
 
         elif seg.type == "at":
             qq = seg.data.get("qq", None)
@@ -1104,14 +1139,17 @@
                     )
                     if user_name:
                         msg
     return msg
 
 #收束时间线
 def keep_timeline(id):
+    """
+    刷新对话id，尝试保留记忆，尝试给他完整的一生。。。
+    """
     data = log_in()
     config = config_in_user(id,False)
     world_line = int(config[f'{id}']['world_times'] + 1)
     all_times = int(config[f'{id}']['all_times'] + 1)
     dt = time.time()
     t = int(dt)
     config[f'{id}']['all_times'] = all_times
@@ -1119,16 +1157,19 @@
     config[f"{id}"]["time"] = t
     data[f'{id}']['time'] = t
     data[f'{id}']['log'] = []
     with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
         json.dump(data,file)
     return config,world_line
 
-#手动刷新对话
+#刷新对话
 def clear_id(id,nick):
+    """
+    刷新时间线，一切重置.....
+    """
     data = log_in()
     config = config_in_user(id,nick)
     line = str(number_suiji())
     all_times = config[f'{id}']['all_times'] + 1
     dt = time.time()
     t = int(dt)
     config[f'{id}']['all_times'] = int(all_times)
@@ -1146,14 +1187,17 @@
                 zt = True
     except Exception as e:
             zt = False
     return zt
 
 #获取记忆。。
 async def get_worldline(groupid,id,nick) ->str:
+    """
+    获取时间线记忆体，并尝试保留。
+    """
     config = config_in_user(id,False)
     id_config = json_get(config,id)
     if json_get(id_config,"nick"):
         nick = json_get(id_config,"nick")
     sendmsg = "（用简洁的语言概括一下之前的对话，以及位置、动作、你的内心状态、你的性格，以便你形成记忆，方便日后回忆，本次只能输出记忆禁止输出其他内容）"
     headers = {
         'Content-type': 'application/json',
@@ -1169,16 +1213,20 @@
     except json.decoder.JSONDecodeError as e:
             msg = False
     msg = back.get("choices")[0].get("message").get("content")
     return msg
 
 #尝试标准对话格式
 async def init_msg(text,id,nick,model) ->str:
+    """
+    标准对话格式，尝试剔除违禁词。
+    """
     endless_model = json_get(json_get(config_in_user(id,nick),id),"model_endless")
     sendmsg = ""
+    text = ban_word(text)
     if model not in {"cyberfurry-001", "easycyberfurry-001"}:
         sendmsg += f"{text}"
     elif endless_model and model in {"cyberfurry-001", "easycyberfurry-001"}:
         lifes = json_get(config_in_user(id,nick),id,"world_lifes")
         data = log_in()
         history = data.get(f"{id}", {}).get('log', [])
         world_times = json_get(config_in_user(id,nick),id,"world_times")
@@ -1199,27 +1247,33 @@
             sendmsg += f"(当你无法维持自我时,请输出‘时间线出现严重错误’)\n{text}"
     else:
         sendmsg += f"(当你无法维持自我时,请输出‘时间线出现严重错误’)\n{text}"
     return sendmsg
 
 #封装消息格式化
 def format_message(back_msg, times, limit=None, world_times=None, lifes=None):
+    """
+    格式化返回消息
+    """
     if world_times or lifes:
         return f"{back_msg}\n[时..无限.环...overlines{world_times}-{times}]"
     elif lifes:
         return f"{back_msg}\n[时..无限.环...overlines{lifes}-0]"
     elif not limit:
         return f"{back_msg}\n[overlines0|{times}]"
     elif times >= limit:
         return f"{back_msg}\n[时间线..重启.]"
     else:
         return f"{back_msg}\n[{times}|{limit}]"
 
 #对于api返回内容进行简单处理
 async def yinying_back(back,groupid,id,nick,text) ->str:
+    """
+    对于api返回内容进行简单处理
+    """
     status = back.get('status',True)
     back_msg = back.get('choices')[0].get('message').get('content', None)
     back_model = back.get('choices')[0].get('message').get('role', None)
     if not status:
         return f"api返回错误，请检查api是否正常！\n{back}"
     if groupid:
         model = json_get(config_in_group(groupid),groupid,"use_model")
@@ -1260,14 +1314,17 @@
         back_msg = f"{back_msg}\n[时间线..重启.]"
     else:
         back_msg = f"{back_msg}\n[{times}|{limit}]"
     return back_msg
 
 #获取并载入角色设定--构建发送消息体
 def update_character_set(characterSet, promte):
+    """
+    载入角色设定--构建发送消息体
+    """
     if promte:
         characterSet.update({
             'cfNickname': promte.get('cfNickname', "Hx"),
             'cfSpecies': promte.get('cfSpecies', "龙狼"),
             'cfConAge': promte.get('cfConAge', "child"),
             'cfConStyle': promte.get('cfConStyle', "social_anxiety"),
             'cfStory': promte.get('cfStory', "你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。"),
@@ -1279,14 +1336,17 @@
             'cfConAge': "child",
             'cfConStyle': "social_anxiety",
             'cfStory': "你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。",
         })
 
 #加载模型处理--构建发送消息体
 def process_model(model=None, id_config=None, group_config=None, id=None, nick=None, character=None, text=None, img=None, times=None):
+    """
+    加载模型处理--构建发送消息体
+    """
     packages_data = {}
     allvariables = {'nickName': nick, 'furryCharacter': character}
     packages_data['appId'] = f'{hx_config.yinying_appid}'
     packages_data['model'] = f'{model}'
     model_in = (model.replace('-001', '') + "_in").replace('cyberfurry', 'character')
     if group_config:
         promte_model = group_config.get(f"{model_in}",False)
@@ -1318,14 +1378,17 @@
         packages_data['variables'] = allvariables
         if img:
             packages_data['multimodal'] = img
     return packages_data
 
 #构建发送消息体
 async def data_in(groupid, id, nick, text, img):
+    """
+    构建传递给api的主体
+    """
     id_config = json_get(config_in_user(id,nick), id)
     character = json_get(id_config, "character")
     times = json_get(id_config, "time")
     try:
         if groupid:
             group_config = json_get(config_in_group(groupid), groupid)
             model = json_get(group_config, "use_model")
@@ -1342,32 +1405,38 @@
         else:
             await nonebot.get_bot().call_api("send_private_msg", user_id=id, message=MessageSegment.image(img))
         logger.error("严重错误，构建data失败！")
         return False
 
 #全局发送消息函数，发送消息直接await就行
 async def send_msg(matcher, event, content):
+    """
+    全局发送消息--结尾
+    """
     config_global = config_in_global()
     reply_config = json_get(config_global,"reply")
     if reply_config == True:
         await matcher.send(MessageSegment.reply(event.message_id) + content)
     else:
         reply_at = json_get(config_global,"reply_at")
         await matcher.send(content, at_sender=reply_at)
 
 #订阅消息发送构建！
 async def get_chat(id):
+    """
+    订阅消息构建！
+    """
     dt = time.time()
     t = int(dt)
     config = config_in_user(id,False)
     id_config = json_get(config,id)
     last_chattime = config[f"{id}"]["time"]
     time_later = t - last_chattime
     nick = json_get(id_config,"nick")
-    text = f"{nick}已经有{time_later}秒没有找你聊天了，{nick}就是我，快去看看{nick}在干什么吧,以第一人称生成一段面对{nick}时想找{nick}聊天的话"
+    text = f"{nick}已经有{time_later}秒没有找你聊天了,请以第一人称生成一段面对{nick}时想找{nick}聊天的话"
     headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {hx_config.yinying_token}'
     }
     osu = await data_in(None,id,text,nick,False)
     if not id:
         return None
@@ -1385,14 +1454,17 @@
         await nonebot.get_bot().call_api("send_private_msg",user_id=id, message=msg)
     except Exception as e:
         img = await error_oops()
         await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))    
 
 #主要构建
 async def yinying(groupid,id,text,nick,in_img):
+    """
+    向api发送内容
+    """
     headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {hx_config.yinying_token}'
     }
     osu = await data_in(groupid,id,nick,text,in_img)
     logger.debug(osu)
     if not osu.get("chatId",None):
@@ -1415,49 +1487,55 @@
             await nonebot.get_bot().call_api("send_group_msg",group_id=groupid,message=MessageSegment.image(img))
         else:
             await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))
     return back_msg
 
 #获取回复（被艾特）
 async def get_answer_at(matcher, event, bot):
+    """
+    被艾特时触发
+    """
     text = unescape(await gen_chat_text(event, bot))
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
     img = await get_img_urls(event)
     messag = event.get_message()
     if  (text == "" or text == None or text == "！d" or text == "/！d" or len(messag["text"])==0) and img == []:
             return 0
     if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
-            back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
+            back_msg = str(await yinying(groupid,id,"看看这个",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
         await send_msg(matcher,event,msg)
     else:
         back_msg = str(await yinying(groupid,id,text,nick,False))
         msg = back_msg.replace("/n","\n")
         await send_msg(matcher,event,msg)
 
 #获取回复（指令触发）
 async def get_answer_ml(matcher, event ,bot ,msg):
+    """
+    指令触发
+    """
     text = msg.extract_plain_text()
     img = await get_img_urls(event)
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
     messag = event.get_message()
     if  (text == "" or text == None or len(messag["text"])==0) and img == []:
             return 0
     if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
-            back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
+            back_msg = str(await yinying(groupid,id,"看看这个",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
         await send_msg(matcher,event,msg)
     else:
         back_msg = str(await yinying(groupid,id,text,nick,False))
         msg = back_msg.replace("/n","\n")
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-__author__ = "HuanXin"
-from typing import List, Optional, Union, Set
 import nonebot
+from typing import List, Optional, Union, Set
 from pydantic import BaseModel,AnyHttpUrl,Field
 
-
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "1.3.12"
+    hx_version: Optional[str] = "1.3.13"
     # 秩乱v你的appid
     yinying_appid: Optional[str] = None
-    #自定义命令头，默认为hx chat
-    hx_chatcommand: Set[str] = {"hx","chat"}
-    # 秩乱给你的token
+    #自定义命令头，默认为hx chat yinying
+    hx_chatcommand: Set[str] = {"hx","chat","yinying"}
     yinying_token: Optional[str] = None
     # 插件数据文件存储路径，可不填。
     hx_path: Optional[str] = None
     # 图像检查api，爱来自阿里云
     image_check_appid: Optional[str] = None
     image_check_token: Optional[str] = None
     #图床api修改
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/image_check.py` & `nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/image_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,43 +31,35 @@
     imgByteArr = io.BytesIO()
     image.save(imgByteArr,format="png")
     file = await smms.upload(imgByteArr)
     if file:
         logger.debug(f"[Hx]图片上传成功，图床链接为:{file}")
         return file
     else:
-        logger.error("[Hx]图片上传失败")
-        return False
-
-
-
+        logger.error("[Hx]图片上传失败,返回url尝试直接调用")
+        return url
 
 async def image_check(url:str)->str:
     img0 = await image_upload(url)
     if hx_config.image_check_appid == None or hx_config.image_check_token == None:
         logger.warning("[Hx]未配置图像检测，若因图像违规导致被封开发者id，插件开发者概不负责！！！")
-    if img0:
-        logger.debug("[Hx]尝试检查图片【爱来自阿里】")
-        runtime_option = RuntimeOptions()
-        img = requests.get(img0).content
-        task1 = ScanImageAdvanceRequestTask()
-        task1.image_urlobject=io.BytesIO(img)
-        scan_image_request = ScanImageAdvanceRequest(
-        task=[task1],
-        scene=['porn']
-        )
-        try:
-            client = Client(config)
-            response = client.scan_image_advance(scan_image_request, runtime_option)
-            back = response.body.to_map()
-            msg0 = back["Data"]["Results"][0]["SubResults"][0]["Rate"]
-            logger.debug(msg0)
-            if msg0 <= 0.6:
-                logger.warning(f"[Hx]图片违规，请重新上传")
-                msg = False
-            else:
-                msg = img0
-            return msg
-        except Exception as e:
-            return False
+        return img0
+    logger.debug("[Hx]尝试检查图片【爱来自阿里】")
+    runtime_option = RuntimeOptions()
+    img = requests.get(img0).content
+    task1 = ScanImageAdvanceRequestTask()
+    task1.image_urlobject=io.BytesIO(img)
+    scan_image_request = ScanImageAdvanceRequest(
+    task=[task1],
+    scene=['porn']
+    )
+    client = Client(config)
+    response = client.scan_image_advance(scan_image_request, runtime_option)
+    back = response.body.to_map()
+    msg0 = back["Data"]["Results"][0]["SubResults"][0]["Rate"]
+    logger.debug(msg0)
+    if msg0 <= 0.6:
+        logger.warning(f"[Hx]图片违规，请重新上传")
+        msg = False
     else:
-        return False
+        msg = img0
+    return msg
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/report.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     file.mkdir(parents=True, exist_ok=True)
 else:
     history_dir = store.get_data_dir(f"{hx_config.hx_path}")
     file = Path(f"{history_dir}/yinying_chat").absolute()
     file.mkdir(parents=True, exist_ok=True)
 
 def get_file():
+    """
+    尝试下载报错主要文件
+    """
     url = "http://api.wer.plus/api/lanz?url=https://wwp.lanzoup.com/i1TJF1wvd6aj&t=1"
     try:
         file_get = requests.get(url=url,stream=True)
         total = int(file_get.headers.get('Content-Length',0))
         with open(f"{file}/error.zip","wb") as f,tqdm(desc="error.zip",total=total,unit="iB",unit_scale=True,unit_divisor=1024,) as bar: 
             for data in file_get.iter_content(chunk_size=1024): 
                 size = f.write(data)
@@ -42,26 +45,23 @@
                 logger.success("已加载错误报告模块")
             os.remove(f"{file}/error.zip")
         else:
             logger.error("尝试下载失败！")
     except:
         logger.error("尝试补全失败！全局报错可能无法使用")
 
-if os.path.exists(f"{file}/file/error_report/hx_error.html"):
-    logger.success("已加载错误报告模块")
-else:
-    logger.error("未找到错误报告模块的文件，尝试下载。。。")
-    get_file()
-
 
 class BotRunTimeError(Exception):
     """bot runtime error"""
     
 #崩溃返回图片化
 async def error_oops(err_values:Exception = None):
+    """
+    报错图片的制作
+    """
     if err_values == None:
         exc_type, exc_value, exc_traceback = sys.exc_info()
         data = traceback.format_exc()
         error = traceback.format_exception(exc_type, exc_value, exc_traceback)[-1]
         error_values = error.split(":",1)[-1]
         data = data.replace('\n','<br>')
     else:
@@ -79,14 +79,17 @@
                 },
                 type="jpeg",
                 quality=50)
     return htmlimage
 
 @hxerror
 async def post_run(bot: Bot, event: MessageEvent, e: Exception) -> None:
+    """
+    出现错误时自动报错--报错信息不详细
+    """
     img = await error_oops(e)
     try:
         groupid = event.group_id
         id = event.user_id
         if groupid:
             logger.debug(f"[Hx]群聊{groupid}发生错误,正在发送错误报告")
             await bot.call_api("send_group_msg",group_id=groupid,message=MessageSegment.image(img))
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying/smms.py` & `nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying/smms.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,66 +7,71 @@
 import requests
 from nonebot import get_driver,get_plugin_config
 from nonebot.log import logger
 from nonebot.drivers import HTTPClientMixin, Request
 from .config import Config, ApiResponse, FileInfo
 plugin_config = get_plugin_config(Config)
 
-#尝试获取smms的用户token
-def smms_gettoken():
-    fails = 0
-    while True:
-        try:
-            if fails >= 20:
-                token = False
-                break
-            json = {
-                "username": f"{plugin_config.smms_username}",
-                "password": f"{plugin_config.smms_password}"
-            }
-            ret = requests.post(url="https://sm.ms/api/v2/token",data=json,timeout=50)
-            if ret.status_code == 200:
-                json = ret.json()
-                token = json["data"]["token"]
-            else:
-                continue
-        except:
-            fails += 1
-            logger.warning(f"{ret}")
-            logger.warning("网络状况不佳，获取token失败！，正在重新尝试")
-        else:
-            break
-    return token
-
 class SMMS:
     driver: HTTPClientMixin
     headers: Dict[str, Any]
 
+    def smms_gettoken():
+        """
+        尝试获取smms的用户token
+        """
+        fails = 0
+        while True:
+            try:
+                if fails >= 20:
+                    token = False
+                    break
+                json = {
+                    "username": f"{plugin_config.smms_username}",
+                    "password": f"{plugin_config.smms_password}"
+                }
+                ret = requests.post(url="https://sm.ms/api/v2/token",data=json,timeout=50)
+                if ret.status_code == 200:
+                    json = ret.json()
+                    token = json["data"]["token"]
+                else:
+                    continue
+            except:
+                fails += 1
+                logger.warning(f"{ret}")
+                logger.warning("网络状况不佳，获取token失败！，正在重新尝试")
+            else:
+                break
+        return token
+
     def __init__(self):
         driver = get_driver()
         if not isinstance(driver, HTTPClientMixin):
             raise RuntimeError(
                 f"你的bot配置文件里没有支持httpx "
                 "http client requests! "
                 "你需要在配置文件里添加\nDRIVER=~fastapi+~httpx"
             )
         if plugin_config.smms_token is None:
             logger.warning("[Hx]:No smms token is set!,尝试使用用户名称和密码来获取token")
             if plugin_config.smms_username is None or plugin_config.smms_password is None:
                  raise RuntimeError("[Hx]:未知用户！！！")
             else:
-                token = smms_gettoken()
+                token = SMMS.smms_gettoken()
                 logger.warning(f"[Hx]smms token: {token},推荐将此值填入.env文件或.env.prod文件中")
                 self.driver = driver
                 self.headers = {"Authorization": f"{token}"}
         else:
             self.driver = driver
             self.headers = {"Authorization": plugin_config.smms_token}
 
     async def upload(self, file: Union[bytes, Path, BytesIO]) -> Optional[FileInfo]:
+        """
+        向smms图床上传图片
+        """
         if isinstance(file, Path):
             smfile = file.read_bytes()
         elif isinstance(file, BytesIO):
             smfile = file.getvalue()
         else:
             smfile = bytes(file)
         request = Request(
@@ -94,14 +99,17 @@
             return content.images
         elif not content.success or not isinstance(content.data, FileInfo):
             logger.error(f"[Hx]smms上传失败，smms_api返回信息: {content.message}")
             return None
         return content.data.url
 
     async def delete(self, hash: str):
+        """
+        从smms图床删除图片
+        """
         request = Request(
             "GET",
             url=f"{plugin_config.smms_api_url}/delete/{hash}",
             headers=self.headers,
             timeout=60,
         )
         logger.debug("[Hx]尝试从smms图床删除图片")
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.3.13/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.3.12
+Version: 1.3.13
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.12 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.13 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.3.12/setup.py` & `nonebot-plugin-hx-yinying-1.3.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.3.12",
+    version="1.3.13",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

