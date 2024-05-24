# Comparing `tmp/nonebot_plugin_dcqg_relay-1.0.0.tar.gz` & `tmp/nonebot_plugin_dcqg_relay-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_dcqg_relay-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_dcqg_relay-1.1.0.tar", max compression
```

## Comparing `nonebot_plugin_dcqg_relay-1.0.0.tar` & `nonebot_plugin_dcqg_relay-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1068 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/LICENSE
--rw-r--r--   0        0        0     3019 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/README.md
--rw-r--r--   0        0        0     3682 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/__init__.py
--rw-r--r--   0        0        0      524 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/config.py
--rw-r--r--   0        0        0     9268 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/dc_to_qq.py
--rw-r--r--   0        0        0     6949 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/qq_emoji_dict.py
--rw-r--r--   0        0        0     8386 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/qq_to_dc.py
--rw-r--r--   0        0        0     3116 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/utils.py
--rw-r--r--   0        0        0     1604 2024-04-20 08:08:55.620264 nonebot_plugin_dcqg_relay-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 nonebot_plugin_dcqg_relay-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3019 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/README.md
+-rw-r--r--   0        0        0     2676 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/config.py
+-rw-r--r--   0        0        0     9466 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/dc_to_qq.py
+-rw-r--r--   0        0        0     1749 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/migrations/0105684994ff_move_from_sqlite.py
+-rw-r--r--   0        0        0     1190 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/migrations/a9b783356705_init_db.py
+-rw-r--r--   0        0        0      206 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/model.py
+-rw-r--r--   0        0        0     6949 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/qq_emoji_dict.py
+-rw-r--r--   0        0        0     8600 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/qq_to_dc.py
+-rw-r--r--   0        0        0     3135 2024-05-24 12:28:57.487232 nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/utils.py
+-rw-r--r--   0        0        0     1645 2024-05-24 12:28:57.491232 nonebot_plugin_dcqg_relay-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 nonebot_plugin_dcqg_relay-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/LICENSE` & `nonebot_plugin_dcqg_relay-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/README.md` & `nonebot_plugin_dcqg_relay-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/__init__.py` & `nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-import contextlib
 import re
-import sqlite3
 from typing import Union
 
-from nonebot import get_driver, logger, on, on_command, on_regex, require
+from nonebot import get_driver, logger, on, on_command, on_regex
 from nonebot.adapters.discord import (
     Bot as dc_Bot,
     MessageCreateEvent as dc_MessageCreateEvent,
     MessageDeleteEvent as dc_MessageDeleteEvent,
 )
 from nonebot.adapters.qq import (
     Bot as qq_Bot,
     GuildMessageEvent as qq_GuildMessageEvent,
     MessageDeleteEvent as qq_MessageDeleteEvent,
 )
 from nonebot.plugin import PluginMetadata
 
-require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler
-
-require("nonebot_plugin_localstore")
-import nonebot_plugin_localstore as store
-
 from .config import Config, Link, plugin_config
 from .dc_to_qq import create_dc_to_qq, delete_dc_to_qq
 from .qq_to_dc import create_qq_to_dc, delete_qq_to_dc
-from .utils import check_messages, init_db
+from .utils import check_messages
 
 __plugin_meta__ = PluginMetadata(
     name="QQ频道-Discord 互通",
     description="在QQ频道与 Discord 之间同步消息的 nonebot2 插件",
     usage="",
     type="application",
     homepage="https://github.com/Autuamn/nonebot-plugin-dcqg-relay",
@@ -39,19 +31,14 @@
 
 
 driver = get_driver()
 channel_links: list[Link] = plugin_config.dcqg_relay_channel_links
 discord_proxy = plugin_config.discord_proxy
 unmatch_beginning = plugin_config.dcqg_relay_unmatch_beginning
 
-cache_dir = store.get_cache_dir("sync_message_to_discord")
-data_dir = store.get_data_dir("sync_message_to_discord")
-database_file = store.get_data_file("sync_message_to_discord", "msgid.db")
-config_file = store.get_config_file("sync_message_to_discord", "webhook.json")
-
 just_delete = []
 
 commit_db_m = on_command("commit_db", priority=0, block=True)
 unmatcher = on_regex(
     rf'\A *?[{re.escape("".join(unmatch_beginning))}].*', priority=1, block=True
 )
 matcher = on(rule=check_messages, priority=2, block=False)
@@ -65,62 +52,37 @@
 
 @driver.on_bot_connect
 async def get_qq_bot(bot: qq_Bot):
     global qq_bot
     qq_bot = bot
 
 
-@driver.on_startup
-async def connect_db():
-    global conn
-    conn = (
-        (await init_db(database_file))
-        if not database_file.exists()
-        else sqlite3.connect(database_file)
-    )
-
-
-@driver.on_shutdown
-async def close_db():
-    conn.commit()
-    conn.close()
-
-
-@scheduler.scheduled_job("cron", minute="*/30", id="commit_db")
-@commit_db_m.handle()
-async def commit_db():
-    await close_db()
-    await connect_db()
-    with contextlib.suppress(LookupError):
-        await commit_db_m.finish("commit!")
-
-
 @unmatcher.handle()
 async def unmatcher_pass():
     pass
 
 
 @matcher.handle()
 async def create_message(
     bot: Union[qq_Bot, dc_Bot],
     event: Union[qq_GuildMessageEvent, dc_MessageCreateEvent],
 ):
     logger.debug("create_handle")
     if isinstance(bot, qq_Bot) and isinstance(event, qq_GuildMessageEvent):
-        await create_qq_to_dc(bot, event, dc_bot, conn)
+        await create_qq_to_dc(bot, event, dc_bot, channel_links)
     elif isinstance(bot, dc_Bot) and isinstance(event, dc_MessageCreateEvent):
-        await create_dc_to_qq(bot, event, qq_bot, conn)
+        await create_dc_to_qq(bot, event, qq_bot)
     else:
         logger.error("bot type and event type not match")
 
 
 @matcher.handle()
 async def delete_message(
     bot: Union[qq_Bot, dc_Bot],
     event: Union[qq_MessageDeleteEvent, dc_MessageDeleteEvent],
 ):
     if isinstance(bot, qq_Bot) and isinstance(event, qq_MessageDeleteEvent):
-        await delete_qq_to_dc(event, dc_bot, conn, just_delete)
+        await delete_qq_to_dc(event, dc_bot, channel_links, just_delete)
     elif isinstance(bot, dc_Bot) and isinstance(event, dc_MessageDeleteEvent):
-        await delete_dc_to_qq(event, qq_bot, conn, just_delete)
+        await delete_dc_to_qq(event, qq_bot, just_delete)
     else:
         logger.error("bot type and event type not match")
```

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/config.py` & `nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/dc_to_qq.py` & `nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/dc_to_qq.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import asyncio
 import io
 import re
-from sqlite3 import Connection
 from typing import Optional
 
 import filetype
 from nonebot import logger
 from nonebot.adapters.discord import (
     Bot as dc_Bot,
     MessageCreateEvent as dc_MessageCreateEvent,
     MessageDeleteEvent as dc_MessageDeleteEvent,
 )
 from nonebot.adapters.discord.api import UNSET
-from nonebot.adapters.discord.exception import ActionFailed
 from nonebot.adapters.qq import (
     Bot as qq_Bot,
     Message as qq_SegmentMessage,
     MessageSegment as qq_MessageSegment,
 )
 from nonebot.adapters.qq.exception import AuditException
 from nonebot.adapters.qq.models import Message as qq_Message
+from nonebot_plugin_orm import get_session
+from sqlalchemy import select
 from PIL import Image
 
 from .config import Link, plugin_config
+from .model import MsgID
 from .utils import get_dc_member_name, get_file_bytes
 
 channel_links: list[Link] = plugin_config.dcqg_relay_channel_links
 discord_proxy = plugin_config.discord_proxy
 
 
 async def get_qq_img(url: str, proxy: Optional[str]) -> io.BytesIO:
@@ -60,70 +61,67 @@
 
 async def build_qq_message(
     bot: dc_Bot, event: dc_MessageCreateEvent
 ) -> tuple[qq_SegmentMessage, list[str]]:
     qq_message = qq_SegmentMessage(
         qq_MessageSegment.text(
             (
-                await get_dc_member_name(bot, event.guild_id, event.author.id)
-                if event.guild_id is not UNSET
-                else ""
+                event.member.nick
+                if event.member is not UNSET
+                and event.member.nick is not UNSET
+                and event.member.nick
+                else event.author.global_name or ""
             )
             + f"(@{event.author.username}):\n"
         )
     )
     img_list: list[str] = []
-    msg = (
-        event.content
+    message = (
+        event
         if event.content
         else (
             await bot.get_channel_message(
                 channel_id=event.channel_id, message_id=event.message_id
             )
-        ).content
+        )
     )
+    content = message.content
     text_begin = 0
     for embed in re.finditer(
         r"<(?P<type>(@!|@&|@|#|/|:|a:|t:))(?P<param>.+?)>",
-        msg,
+        content,
     ):
-        if content := msg[text_begin : embed.pos + embed.start()]:
+        if content := content[text_begin : embed.pos + embed.start()]:
             qq_message += qq_MessageSegment.text(content)
         text_begin = embed.pos + embed.end()
         if embed.group("type") in ("@!", "@"):
-            try:
-                qq_message += qq_MessageSegment.text(
-                    "@"
-                    + (await bot.get_user(user_id=int(embed.group("param")))).username
-                )
-            except ActionFailed as e:
-                if e.message == "Unknown User":
-                    qq_message += qq_MessageSegment.text(f'@({embed.group("param")})')
-                else:
-                    raise e
+            nick, username = await get_dc_member_name(
+                bot, event.guild_id, int(embed.group("param"))
+            )
+            qq_message += qq_MessageSegment.text("@" + nick + f"({username})")
         elif embed.group("type") == "@&":
             qq_message += qq_MessageSegment.text(
                 "@"
                 + (
                     await get_dc_role_name(
                         bot, event.guild_id, int(embed.group("param"))
                     )
                     if event.guild_id is not UNSET
-                    else "(error:未知用户组)"
+                    else f"(error:未知用户组)({embed.group('param')})"
                 )
             )
         elif embed.group("type") == "#":
             qq_message += qq_MessageSegment.text(
                 "#"
                 + (
                     await get_dc_channel_name(
                         bot, event.guild_id, int(embed.group("param"))
                     )
                     if event.guild_id is not UNSET
-                    else "(error:未知频道)"
+                    else f"(error:未知频道)({embed.group('param')})"
                 )
             )
         elif embed.group("type") == "/":
             pass
         elif embed.group("type") in (":", "a:"):
             if len(cut := embed.group("param").split(":")) == 2:
                 if not cut[1]:
@@ -138,73 +136,75 @@
             else:
                 qq_message += qq_MessageSegment.text(embed.group())
         else:
             if embed.group().isdigit():
                 qq_message += qq_MessageSegment.text(f'<t:{embed.group("param")}>')
             else:
                 qq_message += qq_MessageSegment.text(embed.group())
-    if content := msg[text_begin:]:
+    if content := content[text_begin:]:
         qq_message += qq_MessageSegment.text(content)
 
-    if event.mention_everyone:
+    if message.mention_everyone:
         qq_message += qq_MessageSegment.mention_everyone()
-    if attachments := event.attachments:
+
+    if attachments := message.attachments:
         for attachment in attachments:
             if attachment.content_type is not UNSET and re.match(
                 r"image/(gif|jpeg|png|webp)", attachment.content_type, 0
             ):
                 img_list.append(attachment.url)
             else:
                 pass
     return qq_message, img_list
 
 
-async def create_dc_to_qq(
-    bot: dc_Bot, event: dc_MessageCreateEvent, qq_bot: qq_Bot, conn: Connection
-):
+async def create_dc_to_qq(bot: dc_Bot, event: dc_MessageCreateEvent, qq_bot: qq_Bot):
     """discord 消息转发到 QQ"""
     event.get_message()
     message, img_list = await build_qq_message(bot, event)
     link = next(
         link for link in channel_links if link.dc_channel_id == event.channel_id
     )
     if img_list:
         get_img_tasks = [get_qq_img(img, discord_proxy) for img in img_list]
         img_data_list = await asyncio.gather(*get_img_tasks)
     else:
         img_data_list = ["0"]
-    if (
-        event.message_reference is not UNSET
-        and (message_id := event.message_reference.message_id)
-        and message_id is not UNSET
-        and (
-            db_select := conn.execute(
-                f"SELECT QQID FROM ID WHERE DCID LIKE {message_id}"
-            ).fetchone()
-        )
-        and (reference := db_select[0])
-    ):
-        message += qq_MessageSegment.reference(reference)
 
+    async with get_session() as session:
+        if (
+            event.message_reference is not UNSET
+            and (message_id := event.message_reference.message_id)
+            and message_id is not UNSET
+            and (
+                reference := await session.scalar(
+                    select(MsgID.qqid).filter(MsgID.dcid == message_id).fetch(1)
+                )
+            )
+        ):
+            message += qq_MessageSegment.reference(reference)
+
+    sends: list = []
     for i, img_data in enumerate(img_data_list):
         try_times = 1
         while True:
             try:
                 if isinstance(img_data, io.BytesIO):
                     message = (
                         message.append(qq_MessageSegment.file_image(img_data))
                         if i == 0
                         else qq_SegmentMessage(qq_MessageSegment.file_image(img_data))
                     )
-                send = await qq_bot.send_to_channel(link.qq_channel_id, message)
+                sends.append(await qq_bot.send_to_channel(link.qq_channel_id, message))
                 break
             except AuditException as e:
                 try_times = 1
                 while True:
-                    if send := (await e.get_audit_result()).message_id:
+                    if id := (await e.get_audit_result()).message_id:
+                        sends.append(id)
                         break
                     else:
                         logger.warning(f"get_audit_result retry {try_times}")
                         if try_times >= 5:
                             logger.warning(
                                 "message audit fail: "
                                 + f"[audit_id:{e.audit_id}, dc_message_id: {event.id}]"
@@ -216,43 +216,50 @@
             except NameError as e:
                 logger.warning(f"retry {try_times}")
                 if try_times >= 3:
                     raise e
                 try_times += 1
                 await asyncio.sleep(5)
 
-        if send:
-            conn.execute(
-                "INSERT INTO ID (DCID, QQID) VALUES (?, ?)",
-                (event.id, send.id if isinstance(send, qq_Message) else send),
+    async with get_session() as session:
+        for send in sends:
+            session.add(
+                MsgID(
+                    dcid=event.id,
+                    qqid=send.id if isinstance(send, qq_Message) else send,
+                )
             )
+        await session.commit()
 
 
 async def delete_dc_to_qq(
-    event: dc_MessageDeleteEvent, qq_bot: qq_Bot, conn: Connection, just_delete: list
+    event: dc_MessageDeleteEvent, qq_bot: qq_Bot, just_delete: list
 ):
     if (id := event.id) in just_delete:
         just_delete.remove(id)
         return
     try_times = 1
     while True:
         try:
-            db_selected = conn.execute(
-                f'SELECT QQID FROM ID WHERE DCID LIKE ("%{event.id}%")'
+            channel_id = next(
+                link.qq_channel_id
+                for link in channel_links
+                if link.dc_channel_id == event.channel_id
             )
-            for msgids in db_selected:
-                for msgid in msgids:
-                    channel_id = next(
-                        link.qq_channel_id
-                        for link in channel_links
-                        if link.dc_channel_id == event.channel_id
-                    )
-                    await qq_bot.delete_message(message_id=msgid, channel_id=channel_id)
-                    just_delete.append(msgid)
-                    conn.execute(f'DELETE FROM ID WHERE QQID="{msgid}"')
+            async with get_session() as session:
+                if msgids := await session.scalars(
+                    select(MsgID).filter(MsgID.dcid == event.id)
+                ):
+                    for msgid in msgids:
+                        await qq_bot.delete_message(
+                            message_id=msgid.qqid, channel_id=channel_id
+                        )
+                        just_delete.append(msgid.qqid)
+                        await session.delete(msgid)
+                    await session.commit()
             break
         except UnboundLocalError or TypeError or NameError as e:
             logger.warning(f"retry {try_times}")
             if try_times == 3:
                 raise e
             try_times += 1
             await asyncio.sleep(5)
```

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/qq_emoji_dict.py` & `nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/qq_emoji_dict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/qq_to_dc.py` & `nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/qq_to_dc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import asyncio
 import re
-from sqlite3 import Connection
 from typing import Optional
 
 import filetype
 from nonebot import logger
 from nonebot.adapters.discord import Bot as dc_Bot
 from nonebot.adapters.discord.api import UNSET, Embed, EmbedAuthor, File, MessageGet
 from nonebot.adapters.discord.exception import NetworkError
 from nonebot.adapters.qq import (
     Bot as qq_Bot,
     GuildMessageEvent as qq_GuildMessageEvent,
     MessageDeleteEvent as qq_MessageDeleteEvent,
 )
 from nonebot.adapters.qq.models import Message as qq_Message, MessageReference
+from nonebot_plugin_orm import get_session
+from sqlalchemy import select
 
-from .config import Link, plugin_config
+from .config import Link
+from .model import MsgID
 from .qq_emoji_dict import qq_emoji_dict
 from .utils import get_dc_member_name, get_file_bytes
 
-channel_links: list[Link] = plugin_config.dcqg_relay_channel_links
-
 
 async def get_qq_member_name(bot: qq_Bot, guild_id: str, user_id: str) -> str:
     member = await bot.get_member(guild_id=guild_id, user_id=user_id)
     return member.nick or (member.user.username if member.user else "") or ""
 
 
 async def get_dc_member_avatar(bot: dc_Bot, guild_id: int, user_id: int) -> str:
@@ -51,47 +51,48 @@
 
 
 async def build_dc_embeds(
     bot: qq_Bot,
     dc_bot: dc_Bot,
     reference: MessageReference,
     reply: qq_Message,
-    conn: Connection,
     channel_link: Link,
 ) -> list[Embed]:
     """处理 QQ 转 discord 中的回复部分"""
     guild_id, channel_id = channel_link.dc_guild_id, channel_link.dc_channel_id
 
     author = ""
     timestamp = f"<t:{int(reply.timestamp.timestamp())}:R>" if reply.timestamp else ""
 
-    if db_select := conn.execute(
-        f"SELECT DCID FROM ID WHERE QQID LIKE ('%{reference.message_id}%')"
-    ).fetchone():
-        reference_id = db_select[0]
-        dc_message = await dc_bot.get_channel_message(
-            channel_id=channel_id, message_id=reference_id
-        )
-        if reply.author.id == (await bot.me()).id:
-            author = EmbedAuthor(
-                name=await get_dc_member_name(dc_bot, guild_id, dc_message.author.id)
-                + f"(@{dc_message.author.username})",
-                icon_url=await get_dc_member_avatar(
+    async with get_session() as session:
+        if reference_id := await session.scalar(
+            select(MsgID.dcid).filter(MsgID.qqid == reference.message_id).fetch(1)
+        ):
+            dc_message = await dc_bot.get_channel_message(
+                channel_id=channel_id, message_id=reference_id
+            )
+            if reply.author.id == (await bot.me()).id:
+                name, _ = await get_dc_member_name(
                     dc_bot, guild_id, dc_message.author.id
-                ),
+                )
+                author = EmbedAuthor(
+                    name=name + f"(@{dc_message.author.username})",
+                    icon_url=await get_dc_member_avatar(
+                        dc_bot, guild_id, dc_message.author.id
+                    ),
+                )
+                timestamp = f"<t:{int(dc_message.timestamp.timestamp())}:R>"
+
+            description = (
+                f"{dc_message.content}\n\n"
+                + timestamp
+                + f"[[ ↑ ]](https://discord.com/channels/{guild_id}/{channel_id}/{reference_id})"
             )
-            timestamp = f"<t:{int(dc_message.timestamp.timestamp())}:R>"
-
-        description = (
-            f"{dc_message.content}\n\n"
-            + timestamp
-            + f"[[ ↑ ]](https://discord.com/channels/{guild_id}/{channel_id}/{reference_id})"
-        )
-    else:
-        description = f"{reply.content}\n\n" + timestamp + "[ ? ]"
+        else:
+            description = f"{reply.content}\n\n" + timestamp + "[ ? ]"
 
     if not author:
         member = await bot.get_member(guild_id=reply.guild_id, user_id=reply.author.id)
         author = EmbedAuthor(
             name=(member.nick or (member.user.username if member.user else "") or "")
             + f"[ID:{reply.author.id}]",
             icon_url=(member.user.avatar if member.user else "") or "",
@@ -179,25 +180,28 @@
             await asyncio.sleep(5)
 
     logger.debug("send")
     return send
 
 
 async def create_qq_to_dc(
-    bot: qq_Bot, event: qq_GuildMessageEvent, dc_bot: dc_Bot, conn: Connection
+    bot: qq_Bot,
+    event: qq_GuildMessageEvent,
+    dc_bot: dc_Bot,
+    channel_links: list[Link],
 ):
     """QQ 消息转发到 discord"""
 
     text, img_list = await build_dc_message(bot, event)
     link = next(
         link for link in channel_links if link.qq_channel_id == event.channel_id
     )
 
     if (reply := event.reply) and (reference := event.message_reference):
-        embeds = await build_dc_embeds(bot, dc_bot, reference, reply, conn, link)
+        embeds = await build_dc_embeds(bot, dc_bot, reference, reply, link)
     else:
         embeds = None
 
     username = f"{event.author.username} [ID:{event.author.id}]"
     avatar = event.author.avatar
 
     try_times = 1
@@ -217,40 +221,47 @@
         except NameError as e:
             logger.warning(f"retry {try_times}")
             if try_times == 3:
                 raise e
             try_times += 1
             await asyncio.sleep(5)
 
-    if send:
-        conn.execute(f'INSERT INTO ID (DCID, QQID) VALUES ({send.id}, "{event.id}")')
+    async with get_session() as session:
+        session.add(MsgID(dcid=send.id, qqid=event.id))
+        await session.commit()
 
 
 async def delete_qq_to_dc(
-    event: qq_MessageDeleteEvent, dc_bot: dc_Bot, conn: Connection, just_delete: list
+    event: qq_MessageDeleteEvent,
+    dc_bot: dc_Bot,
+    channel_links: list[Link],
+    just_delete: list,
 ):
     if (id := event.message.id) in just_delete:
         just_delete.remove(id)
         return
+    channel_id = next(
+        link.dc_channel_id
+        for link in channel_links
+        if link.qq_channel_id == event.message.channel_id
+    )
     try_times = 1
     while True:
         try:
-            db_selected = conn.execute(
-                f"SELECT DCID FROM ID WHERE QQID LIKE ('%{event.message.id}%')"
-            )
-            for msgids in db_selected:
-                for msgid in msgids:
-                    channel_id = next(
-                        link.dc_channel_id
-                        for link in channel_links
-                        if link.qq_channel_id == event.message.channel_id
-                    )
-                    await dc_bot.delete_message(message_id=msgid, channel_id=channel_id)
-                    just_delete.append(msgid)
-                    conn.execute(f"DELETE FROM ID WHERE DCID={msgid}")
+            async with get_session() as session:
+                if msgids := await session.scalars(
+                    select(MsgID).filter(MsgID.qqid == event.message.id)
+                ):
+                    for msgid in msgids:
+                        await dc_bot.delete_message(
+                            message_id=msgid.dcid, channel_id=channel_id
+                        )
+                        just_delete.append(msgid.dcid)
+                        await session.delete(msgid)
+                    await session.commit()
             break
         except UnboundLocalError or TypeError or NameError as e:
             logger.warning(f"retry {try_times}")
             if try_times == 3:
                 raise e
             try_times += 1
             await asyncio.sleep(5)
```

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/nonebot_plugin_dcqg_relay/utils.py` & `nonebot_plugin_dcqg_relay-1.1.0/nonebot_plugin_dcqg_relay/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from pathlib import Path
 import re
-import sqlite3
 from typing import Optional, Union
 
 import aiohttp
 from nonebot import logger
 from nonebot.adapters.discord import (
     Bot as dc_Bot,
     MessageCreateEvent as dc_MessageCreateEvent,
     MessageDeleteEvent as dc_MessageDeleteEvent,
 )
-from nonebot.adapters.discord.api import UNSET
+from nonebot.adapters.discord.api import UNSET, Missing
 from nonebot.adapters.discord.exception import ActionFailed
 from nonebot.adapters.qq import (
     Bot as qq_Bot,
     GuildMessageEvent as qq_GuildMessageEvent,
     MessageDeleteEvent as qq_MessageDeleteEvent,
 )
 
@@ -63,39 +61,35 @@
         return any(
             event.guild_id == link.dc_guild_id
             and event.channel_id == link.dc_channel_id
             for link in channel_links
         )
 
 
-async def init_db(dbpath: Path):
-    conn = sqlite3.connect(dbpath)
-    conn.execute(
-        """CREATE TABLE ID (
-            DCID    INT     NOT NULL,
-            QQID    TEXT    NOT NULL
-        );"""
-    )
-    return conn
-
-
-async def get_dc_member_name(bot: dc_Bot, guild_id: int, user_id: int) -> str:
+async def get_dc_member_name(
+    bot: dc_Bot, guild_id: Missing[int], user_id: int
+) -> tuple[str, str]:
     try:
-        member = await bot.get_guild_member(guild_id=guild_id, user_id=user_id)
-        if (nick := member.nick) and nick is not UNSET:
-            logger.trace(f"nick: {nick}")
-            return nick
-        elif member.user is not UNSET and (global_name := member.user.global_name):
-            logger.trace(f"global_name: {global_name}")
-            return global_name
+        if guild_id is not UNSET:
+            member = await bot.get_guild_member(guild_id=guild_id, user_id=user_id)
+            if (nick := member.nick) and nick is not UNSET:
+                return nick, member.user.username if member.user is not UNSET else ""
+            elif member.user is not UNSET and (global_name := member.user.global_name):
+                return global_name, member.user.username
+            else:
+                return "", str(user_id)
         else:
-            return ""
+            user = await bot.get_user(user_id=user_id)
+            return user.global_name or "", user.username
     except ActionFailed as e:
         if e.message == "Unknown User":
-            return f"({user_id})"
+            return "(error:未知用户)", str(user_id)
         else:
             raise e
 
 
 async def get_file_bytes(url: str, proxy: Optional[str] = None) -> bytes:
-    async with aiohttp.ClientSession().get(url, proxy=proxy) as response:
+    async with (
+        aiohttp.ClientSession() as session,
+        session.get(url, proxy=proxy) as response,
+    ):
         return await response.read()
```

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/pyproject.toml` & `nonebot_plugin_dcqg_relay-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-dcqg-relay"
-version = "1.0.0"
+version = "1.1.0"
 description = "在QQ频道与 Discord 之间同步消息的 nonebot2 插件"
 authors = ["Autuamn_End <autuamn@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot2 = "^2.2.1"
+nonebot2 = {extras = ["aiohttp"], version = "^2.2.1"}
 nonebot-adapter-qq = "^1.4.3"
 nonebot-adapter-discord = "^0.1.7"
-nonebot-plugin-apscheduler = "^0.4.0"
+nonebot-plugin-orm = {extras = ["default"], version = "^0.7.3"}
 nonebot-plugin-localstore = "^0.6.0"
-aiohttp = "^3.9.5"
 filetype = "^1.2.0"
 pillow = "^10.3.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.0"
 nonemoji = "^0.1.2"
 pre-commit = "^3.1.0"
```

### Comparing `nonebot_plugin_dcqg_relay-1.0.0/PKG-INFO` & `nonebot_plugin_dcqg_relay-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-dcqg-relay
-Version: 1.0.0
+Version: 1.1.0
 Summary: 在QQ频道与 Discord 之间同步消息的 nonebot2 插件
 License: MIT
 Author: Autuamn_End
 Author-email: autuamn@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: nonebot-adapter-discord (>=0.1.7,<0.2.0)
 Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.4.0,<0.5.0)
 Requires-Dist: nonebot-plugin-localstore (>=0.6.0,<0.7.0)
-Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
+Requires-Dist: nonebot-plugin-orm[default] (>=0.7.3,<0.8.0)
+Requires-Dist: nonebot2[aiohttp] (>=2.2.1,<3.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 # QQ频道-Discord 互通
 <a href="https://raw.githubusercontent.com/Autuamn/nonebot-plugin-dcqg-relay/master/LICENSE">
     <img src="https://img.shields.io/github/license/Autuamn/nonebot-plugin-dcqg-relay" alt="license">
 </a>
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-dcqg-relay Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-dcqg-relay Version: 1.1.0 Summary:
 å¨QQé¢éä¸ Discord ä¹é´åæ­¥æ¶æ¯ç nonebot2 æä»¶ License: MIT
 Author: Autuamn_End Author-email: autuamn@qq.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.5,<4.0.0) Requires-Dist: filetype
-(>=1.2.0,<2.0.0) Requires-Dist: nonebot-adapter-discord (>=0.1.7,<0.2.0)
-Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) Requires-Dist: nonebot-
-plugin-apscheduler (>=0.4.0,<0.5.0) Requires-Dist: nonebot-plugin-localstore
-(>=0.6.0,<0.7.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: pillow
-(>=10.3.0,<11.0.0) Description-Content-Type: text/markdown # QQé¢é-Discord
-äºé _[_l_i_c_e_n_s_e_][python]## åè¨
+Requires-Dist: filetype (>=1.2.0,<2.0.0) Requires-Dist: nonebot-adapter-discord
+(>=0.1.7,<0.2.0) Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) Requires-
+Dist: nonebot-plugin-localstore (>=0.6.0,<0.7.0) Requires-Dist: nonebot-plugin-
+orm[default] (>=0.7.3,<0.8.0) Requires-Dist: nonebot2[aiohttp] (>=2.2.1,<3.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0) Description-Content-Type: text/
+markdown # QQé¢é-Discord äºé _[_l_i_c_e_n_s_e_][python]## åè¨
 æ¬é¡¹ç®ä¸ºèªç¨æä»¶ï¼å¦ææéæ±ææ³æ³è¯·æåºï¼æå°½éæ»¡è¶³
 å ç¨å°äºQQå®æ¹çé¢éæºå¨äººæ¥å£ï¼åè½å°ï¼éå¶å¤ï¼èä¸å¾å¤åè½æä¹æ²¡æ³æµè¯ï¼å°±æ²¡ææ¯æãä¹åå¯è½ä¼åºä¸ä¸ªåºäº
 OneBot ééå¨ççæ¬ï¼æï¼ ç®åQQæºå¨äººä¸è½å urlï¼å¦æä»
 Discord è½¬æ¥çæ¶æ¯éå¸¦æ url
 çæ´»æ¯åä¸åºæ¥çï¼ç®åææ²¡ææ³å°è§£å³åæ³ãææ³æ³è¯·æåº
 ## åè½ å¯ä»¥å¨æå®çQQå­é¢éå Discord
 é¢éä¹é´åæ­¥æ¶æ¯ï¼åªæ¯ææ®éçæå­é¢éï¼ä¸æ¯æå¸å­é¢é
```

