# Comparing `tmp/fedbadges-2.0.0.tar.gz` & `tmp/fedbadges-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedbadges-2.0.0.tar", max compression
+gzip compressed data, was "fedbadges-2.1.1.tar", max compression
```

## Comparing `fedbadges-2.0.0.tar` & `fedbadges-2.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    22636 2024-04-16 15:45:34.113835 fedbadges-2.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0    18092 2022-06-27 10:24:28.000000 fedbadges-2.0.0/LICENSE
--rw-r--r--   0        0        0    10839 2024-04-11 10:05:52.136691 fedbadges-2.0.0/README.rst
--rw-r--r--   0        0        0        0 2022-06-27 10:24:28.000000 fedbadges-2.0.0/fedbadges/__init__.py
--rw-r--r--   0        0        0     1559 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/aio.py
--rw-r--r--   0        0        0     5857 2024-04-16 15:39:38.330818 fedbadges-2.0.0/fedbadges/consumer.py
--rw-r--r--   0        0        0        0 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/__init__.py
--rw-r--r--   0        0        0     1987 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/badges_dev.py
--rw-r--r--   0        0        0     1996 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/group_membership.py
--rw-r--r--   0        0        0     1873 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/libravatar.py
--rw-r--r--   0        0        0     2195 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/lifecycle.py
--rw-r--r--   0        0        0     1338 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/mirror.py
--rw-r--r--   0        0        0      827 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/manual/utils.py
--rw-r--r--   0        0        0    17499 2024-04-12 17:12:53.328051 fedbadges-2.0.0/fedbadges/rules.py
--rw-r--r--   0        0        0     3614 2024-04-11 10:05:52.137691 fedbadges-2.0.0/fedbadges/rulesrepo.py
--rw-r--r--   0        0        0     5001 2024-04-12 17:24:32.882079 fedbadges-2.0.0/fedbadges/utils.py
--rw-r--r--   0        0        0     5246 2024-04-11 13:38:19.306992 fedbadges-2.0.0/fedbadges.toml.example
--rw-r--r--   0        0        0     5574 2024-04-16 15:39:38.414819 fedbadges-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2572 2024-04-16 15:39:38.330818 fedbadges-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1286 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/test_badges/rules/bodhi-update-fancy.yaml
--rw-r--r--   0        0        0      990 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/test_badges/rules/bodhi-update-simple.yaml
--rw-r--r--   0        0        0      986 2024-04-11 10:05:52.138691 fedbadges-2.0.0/tests/test_badges/rules/irc-speak-up.yml
--rw-r--r--   0        0        0      919 2022-06-27 10:24:28.000000 fedbadges-2.0.0/tests/test_badges/rules/pagure-long-live.yaml
--rw-r--r--   0        0        0     1143 2024-04-11 10:05:52.138691 fedbadges-2.0.0/tests/test_badges/rules/tagger-01.yml
--rw-r--r--   0        0        0     2822 2024-04-12 15:35:16.765374 fedbadges-2.0.0/tests/test_complicated_recipient.py
--rw-r--r--   0        0        0     2096 2024-04-12 15:35:28.525487 fedbadges-2.0.0/tests/test_complicated_trigger.py
--rw-r--r--   0        0        0     6796 2024-04-12 17:21:08.460290 fedbadges-2.0.0/tests/test_criteria_datanommer.py
--rw-r--r--   0        0        0    11977 2024-04-12 17:17:56.689566 fedbadges-2.0.0/tests/test_rule_matching.py
--rw-r--r--   0        0        0     3171 2024-04-12 17:09:42.594579 fedbadges-2.0.0/tests/test_triggers.py
--rw-r--r--   0        0        0     5087 2024-04-16 15:39:38.414819 fedbadges-2.0.0/tests/test_utils.py
--rw-r--r--   0        0        0      485 2024-04-12 14:52:01.331404 fedbadges-2.0.0/tests/test_yaml_collector.py
--rw-r--r--   0        0        0     3348 2024-04-12 17:21:17.025367 fedbadges-2.0.0/tests/utils.py
--rw-r--r--   0        0        0      878 2024-04-16 15:39:38.414819 fedbadges-2.0.0/tox.ini
--rw-r--r--   0        0        0    13431 1970-01-01 00:00:00.000000 fedbadges-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-05-24 07:39:23.823718 fedbadges-2.1.1/LICENSE
+-rw-r--r--   0        0        0    10793 2024-05-24 07:39:23.823718 fedbadges-2.1.1/README.rst
+-rw-r--r--   0        0        0        0 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/__init__.py
+-rw-r--r--   0        0        0     1559 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/aio.py
+-rw-r--r--   0        0        0     9720 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/cached.py
+-rw-r--r--   0        0        0     7277 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/consumer.py
+-rw-r--r--   0        0        0        0 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/manual/__init__.py
+-rw-r--r--   0        0        0     1987 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/manual/badges_dev.py
+-rw-r--r--   0        0        0     1996 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/manual/group_membership.py
+-rw-r--r--   0        0        0     2199 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/manual/libravatar.py
+-rw-r--r--   0        0        0     2195 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/manual/lifecycle.py
+-rw-r--r--   0        0        0     1338 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/manual/mirror.py
+-rw-r--r--   0        0        0      827 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/manual/utils.py
+-rw-r--r--   0        0        0    19393 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/rules.py
+-rw-r--r--   0        0        0     3614 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges/rulesrepo.py
+-rw-r--r--   0        0        0     6654 2024-05-24 07:39:23.831718 fedbadges-2.1.1/fedbadges/utils.py
+-rw-r--r--   0        0        0     5423 2024-05-24 07:39:23.827718 fedbadges-2.1.1/fedbadges.toml.example
+-rw-r--r--   0        0        0     5972 2024-05-24 07:39:23.831718 fedbadges-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1286 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_badges/rules/bodhi-update-fancy.yaml
+-rw-r--r--   0        0        0      990 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_badges/rules/bodhi-update-simple.yaml
+-rw-r--r--   0        0        0      986 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_badges/rules/irc-speak-up.yml
+-rw-r--r--   0        0        0      919 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_badges/rules/pagure-long-live.yaml
+-rw-r--r--   0        0        0     1143 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_badges/rules/tagger-01.yml
+-rw-r--r--   0        0        0     2877 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_complicated_recipient.py
+-rw-r--r--   0        0        0     2096 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_complicated_trigger.py
+-rw-r--r--   0        0        0     7091 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_criteria_datanommer.py
+-rw-r--r--   0        0        0    12064 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_rule_matching.py
+-rw-r--r--   0        0        0     3171 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_triggers.py
+-rw-r--r--   0        0        0     5121 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0      485 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/test_yaml_collector.py
+-rw-r--r--   0        0        0     3348 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tests/utils.py
+-rw-r--r--   0        0        0      878 2024-05-24 07:39:23.831718 fedbadges-2.1.1/tox.ini
+-rw-r--r--   0        0        0    13659 1970-01-01 00:00:00.000000 fedbadges-2.1.1/PKG-INFO
```

### Comparing `fedbadges-2.0.0/LICENSE` & `fedbadges-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/README.rst` & `fedbadges-2.1.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -47,20 +47,20 @@
   **Aside:** Although datanommer is the only currently supported backend, we
   can implement other queryable backend in the future as needed like FAS
   (to see if the user is in X number of groups) or even off-site services
   like libravatar (to award a badge if the user is a user of the AGPL web
   service).
 
 * If a badge's ``trigger`` and ``criteria`` both match, then the badge is
-  awarded.  If the BadgeRule doesn't specify, we award the badge to all
-  usernames returned by the message's ``usernames`` property.
+  awarded.  If the BadgeRule doesn't specify, we award the badge to the
+  author of the action using the message's ``agent_name`` property.
 
   That is usually correct -- but sometimes, a BadgeRule needs to specify
-  that one particular user (not all related users) should be recipients of
-  the badge.  In this case, the BadgeRule may define a ``recipient``
+  that one particular user should be recipient of the badge.
+  In this case, the BadgeRule may define a ``recipient``
   in dot-notation that instructs the ``Consumer`` how to extract the
   recipient's username from the received message.
 
   The badge is awarded to our deserving user via the `tahrir_api
   <https://github.com/fedora-infra/tahrir-api>`_.  At the end of the day,
   this amounts to adding a row in a database table for the `Tahrir
   <https://github.com/fedora-infra/tahrir>`_ application.
@@ -186,15 +186,15 @@
 off by *any* user at any time in the past.  Pretty generic.
 Here's a more interesting criteria definition::
 
     criteria:
       filter:
         topics:
         - org.fedoraproject.prod.git.receive
-        usernames:
+        users:
         - "%(msg.commit.username)s"
       operation: count
       condition:
         greater than or equal to: 50
 
 This criteria would match if there existed 50 messages of the topic
 ``"org.fedoraproject.prod.git.receive"`` that were also kicked off by whatever
@@ -225,52 +225,53 @@
 statement you provide into a callable and use that at runtime.  For example::
 
 
     criteria:
       filter:
         topics:
         - org.fedoraproject.prod.git.receive
-        usernames:
+        users:
         - "%(msg.commit.username)s"
       operation: count
       condition:
         lambda: value != 0 and ((value & (value - 1)) == 0)
 
 Who knows why you would want to do this, but the above criteria check will
 succeed if the number of messages returned from the filtered datanommer query
 is exactly a power of 2.
 
 Specifying Recipients
 ~~~~~~~~~~~~~~~~~~~~~
 
 By default, if the trigger and criteria match, fedbadges will award badges
-to all the users returned by the message's ``usernames`` property.
-This *usually* corresponds with "what users are responsible" for this message.
+to the user returned by the message's ``agent_name`` property.
+This *usually* corresponds with "which user is responsible" for this message.
 That is *usually* what we want to award badges for.
 
 There are some instances for which that is not what we want.
 
-Take the `org.fedoraproject.prod.fas.group.member.sponsor
-<https://fedora-messaging.readthedocs.io/en/stable/user-guide/schemas.html#fas>`_
-message for example.  When user A sponsors user B to a group, both
-usernames are returned by the message's ``usernames`` property with no
-further distinction as to which was adding and which was added.
-
-Imagine we have a "Group Sponsor" badge that's awarded to group admins who
-sponsor users to groups.  We don't want to inadvertently award that badge
-to the persons who *were sponsored*, only to those who *sponsored them*.
+Take the `org.fedoraproject.prod.bodhi.update.comment
+<https://fedora-messaging.readthedocs.io/en/stable/user-guide/schemas.html#bodhi>`_
+message for example.  When user A comments on user B's update, user A is returned
+by the message's ``agent_name`` property.
+
+Imagine we have a "Received Comments" badge that's awarded to packagers that
+received comments on their updates.  We don't want to inadvertently award that
+badge to the person who *commented*, only to the one who *created the update*.
 
 To allow for this scenario, badges may optionally define a ``recipient``
 in dotted notation that tells fedbadges where to find the username of the
 recipient in the originating message.  For instance, the following would
 handle the fas case we described above::
 
     trigger:
-      topic: org.fedoraproject.prod.fas.group.member.sponsor
+      topic: org.fedoraproject.prod.bodhi.update.comment
     criteria:
       filter:
         topics:
         - "%(topic)s"
+        users:
+        - "%(msg.update.user.name)s"
       operation: count
       condition:
         greater than or equal to: 1
-    recipient: "%(msg.agent_name)s"
+    recipient: "%(msg.update.user.name)s"
```

### Comparing `fedbadges-2.0.0/fedbadges/aio.py` & `fedbadges-2.1.1/fedbadges/aio.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/fedbadges/consumer.py` & `fedbadges-2.1.1/fedbadges/consumer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 
 Authors:  Ross Delinger
           Ralph Bean
           Aurelien Bompard
 """
 
 import asyncio
+import datetime
 import logging
 import threading
 import time
 from functools import partial
 
 import datanommer.models
 import fasjson_client
 import tahrir_api.dbapi
 from fedora_messaging.api import Message
 from fedora_messaging.config import conf as fm_config
 
 from .aio import Periodic
+from .cached import configure as configure_cache
+from .cached import on_message as update_cached_values
 from .rulesrepo import RulesRepo
-from .utils import notification_callback
+from .utils import datanommer_has_message, notification_callback
 
 
 log = logging.getLogger(__name__)
 
 DEFAULT_DELAY_LIMIT = 100
-RULES_RELOAD_INTERVAL = 15 * 60  # 15 minutes
+DEFAULT_RULES_RELOAD_INTERVAL = 15  # in minutes
+MAX_WAIT_DATANOMMER = 5  # seconds
 
 
 class FedoraBadgesConsumer:
     delay_limit = 100
 
     def __init__(self):
         self.config = fm_config["consumer_config"]
@@ -44,14 +48,16 @@
 
     async def setup(self):
         # Five things need doing at start up time
         # 0) Set up a request local to hang thread-safe db sessions on.
         # 1) Initialize our connection to the Tahrir DB
         # 2) Initialize our connection to the datanommer DB.
         # 3) Load our badge definitions and rules from YAML.
+        # Cache
+        await self.loop.run_in_executor(None, self._initialize_cache)
 
         # Tahrir stuff.
         await self.loop.run_in_executor(None, self._initialize_tahrir_connection)
 
         # Datanommer stuff
         await self.loop.run_in_executor(None, self._initialize_datanommer_connection)
 
@@ -60,19 +66,26 @@
             None, fasjson_client.Client, self.config["fasjson_base_url"]
         )
 
         # Load badge definitions
         self._rules_repo = RulesRepo(self.config, self.issuer_id, self.fasjson)
         self._rules_repo.setup()
 
+        rules_reload_inteval = self.config.get(
+            "rules_reload_interval", DEFAULT_RULES_RELOAD_INTERVAL
+        )
         self._refresh_badges_task = Periodic(
-            partial(self.loop.run_in_executor, None, self._reload_rules), RULES_RELOAD_INTERVAL
+            partial(self.loop.run_in_executor, None, self._reload_rules), rules_reload_inteval * 60
         )
         await self._refresh_badges_task.start(run_now=True)
 
+    def _initialize_cache(self):
+        cache_args = self.config.get("cache")
+        configure_cache(**cache_args)
+
     def _initialize_tahrir_connection(self):
         database_uri = self.config.get("database_uri")
         if not database_uri:
             raise ValueError("Badges consumer requires a database uri")
         issuer = self.config["badge_issuer"]
         self.tahrir = tahrir_api.dbapi.TahrirDatabase(
             dburi=database_uri,
@@ -91,20 +104,19 @@
         return self.tahrir
 
     def _initialize_datanommer_connection(self):
         datanommer.models.init(self.config["datanommer_db_uri"])
 
     def award_badge(self, username, badge_rule, link=None):
         email = f"{username}@fedoraproject.org"
-        with self.TahrirDbSession() as session:
-            client = self._get_tahrir_client(session)
-            client.add_person(email)
-            session.commit()
-            client.add_assertion(badge_rule.badge_id, email, None, link)
-            session.commit()
+        client = self._get_tahrir_client(self.tahrir.session)
+        client.add_person(email)
+        self.tahrir.session.commit()
+        client.add_assertion(badge_rule.badge_id, email, None, link)
+        self.tahrir.session.commit()
 
     def __call__(self, message: Message):
         # First thing, we receive the message, but we put ourselves to sleep to
         # wait for a moment.  The reason for this is that, when things are
         # 'calm' on the bus, we receive messages "too fast".  A message that
         # arrives to the badge awarder triggers (usually) a check against
         # datanommer to count messages.  But if we try to count them before
@@ -114,22 +126,26 @@
         # TODO: Option 1, easy: make a SQL query in datanommer instead of waiting
         # TODO: Option 2, a bit harder: check if the current message is in the
         #       matched messages when querying datanommer, and if it's not add 1
         #       to the count.
 
         self._wait_for_datanommer(message)
 
+        log.debug("Updating cached values for %s on %s", message.id, message.topic)
+        update_cached_values(message)
+
         datagrepper_url = self.config["datagrepper_url"]
         link = f"{datagrepper_url}/id?id={message.id}&is_raw=true&size=extra-large"
 
         # Define this so we can refer to it in error handling below
         badge_rule = None
 
         # Award every badge as appropriate.
-        log.debug("Received %s, %s", message.topic, message.id)
+        log.debug("Processing rules for %s on %s", message.id, message.topic)
+
         tahrir = self._get_tahrir_client()
         for badge_rule in self.badge_rules:
             try:
                 for recipient in badge_rule.matches(message, tahrir):
                     log.debug(
                         "Rule %s matched for %s (message %s on %s)",
                         badge_rule.badge_id,
@@ -145,12 +161,27 @@
 
     def _reload_rules(self):
         log.debug("Check for badges updates in the repo")
         tahrir = self._get_tahrir_client()
         self.badge_rules = self._rules_repo.load_all(tahrir)
 
     def _wait_for_datanommer(self, message: Message):
-        while True:
-            dn_msg = datanommer.models.Message.from_msg_id(message.id)
-            if dn_msg is not None:
+        now = datetime.datetime.now(tz=datetime.timezone.utc)
+        a_minute_ago = now - datetime.timedelta(minutes=1)
+        try:
+            sent_at = message._headers["sent-at"]
+            if sent_at.endswith("Z"):
+                # Python 3.10 compatibility
+                sent_at = sent_at[:-1] + "+00:00"
+            sent_at = datetime.datetime.fromisoformat(sent_at)
+        except (KeyError, TypeError, ValueError) as e:
+            log.debug("Could not read the sent-at value: %s: %s", e.__class__.__name__, e)
+            sent_at = None
+        if sent_at is not None and sent_at < a_minute_ago:
+            return  # It's kinda old, datanommer surely has it already
+
+        yesterday = now - datetime.timedelta(days=1)
+        for _i in range(MAX_WAIT_DATANOMMER * 2):
+            if datanommer_has_message(message.id, since=yesterday):
                 break
+            log.debug("Waiting for the message to land in datanommer")
             time.sleep(0.5)
```

### Comparing `fedbadges-2.0.0/fedbadges/manual/badges_dev.py` & `fedbadges-2.1.1/fedbadges/manual/badges_dev.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/fedbadges/manual/group_membership.py` & `fedbadges-2.1.1/fedbadges/manual/group_membership.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/fedbadges/manual/libravatar.py` & `fedbadges-2.1.1/fedbadges/manual/libravatar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import hashlib
 import logging
+import sys
+import traceback
 
+import backoff
 import click
 import requests
 from fedora_messaging.config import conf as fm_config
 from tahrir_api.dbapi import TahrirDatabase
 
 import fedbadges.utils
 
@@ -12,57 +15,71 @@
 
 
 log = logging.getLogger(__name__)
 
 HTTP_TIMEOUT = 5
 
 
+def _backoff_hdlr(details):
+    log.warning("Request to Libravatar failed, retrying.")
+
+
+def _giveup_hdlr(details):
+    log.warning(
+        f"Request to Libravatar failed, giving up. {traceback.format_tb(sys.exc_info()[2])}"
+    )
+
+
+@backoff.on_exception(
+    backoff.expo,
+    (requests.exceptions.SSLError, requests.exceptions.ConnectionError),
+    max_tries=10,
+    on_backoff=_backoff_hdlr,
+    on_giveup=_giveup_hdlr,
+    raise_on_giveup=False,
+)
+def query_libravatar(nickname):
+    openid = f"http://{nickname}.id.fedoraproject.org/"
+    hash = hashlib.sha256(openid.encode("utf-8")).hexdigest()
+    url = f"https://seccdn.libravatar.org/avatar/{hash}?d=404"
+    return requests.get(url, timeout=HTTP_TIMEOUT)
+
+
 @click.command()
 @option_debug
 def main(debug):
     setup_logging(debug=debug)
     config = fm_config["consumer_config"]
     uri = config["database_uri"]
     tahrir = TahrirDatabase(
         uri,
         notification_callback=fedbadges.utils.notification_callback,
     )
-    badge = tahrir.get_badge("mugshot")
+    badge = tahrir.get_badge(badge_id="mugshot")
 
     persons = tahrir.get_all_persons()
     already_has_it = [assertion.person for assertion in badge.assertions]
 
     good, bad = [], []
     for person in persons:
 
         if person in already_has_it:
             good.append(person)
             log.debug("Skipping %s", person)
             continue
 
-        openid = f"http://{person.nickname}.id.fedoraproject.org/"
-        hash = hashlib.sha256(openid.encode("utf-8")).hexdigest()
-        url = f"https://seccdn.libravatar.org/avatar/{hash}?d=404"
-
-        response = None
-        for i in range(10):
-            log.debug("Try %s on %s", i, url)
-            try:
-                response = requests.get(url, timeout=HTTP_TIMEOUT)
-                break
-            except requests.exceptions.SSLError as e:
-                print(" * failed, trying again", str(e))
-
+        response = query_libravatar(person.nickname)
         if response is None:
-            raise
+            # Query failed, ignore
+            continue
 
-        if response.status_code == 200:
+        if response.ok:
             log.info("%s totally gets the mugshot badge.", person.nickname)
             good.append(person)
-            award_badge(tahrir, badge.id, person.email, check_existing=False)
+            award_badge(tahrir, badge, person.email, check_existing=False)
         else:
             bad.append(person)
 
     log.info("%s good peoples", len(good))
     log.info("%s bad peoples", len(bad))
```

### Comparing `fedbadges-2.0.0/fedbadges/manual/lifecycle.py` & `fedbadges-2.1.1/fedbadges/manual/lifecycle.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/fedbadges/manual/mirror.py` & `fedbadges-2.1.1/fedbadges/manual/mirror.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/fedbadges/manual/utils.py` & `fedbadges-2.1.1/fedbadges/manual/utils.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/fedbadges/rules.py` & `fedbadges-2.1.1/fedbadges/rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 import logging
 import re
 
 import datanommer.models
 from fedora_messaging.api import Message
 from tahrir_api.dbapi import TahrirDatabase
 
+from fedbadges.cached import CachedDatanommerQuery, DATANOMMER_CACHED_VALUES
 from fedbadges.utils import (
     # These are all in-process utilities
     construct_substitutions,
     email2fas,
     format_args,
     get_pagure_authors,
     graceful,
     nick2fas,
     recursive_lambda_factory,
+    single_argument_lambda,
     single_argument_lambda_factory,
     # These make networked API calls
     user_exists_in_fas,
 )
 
 
 log = logging.getLogger(__name__)
@@ -46,15 +48,15 @@
 
 def github2fas(uri, config, fasjson):
     m = re.search(r"^https?://api.github.com/users/([a-z][a-z0-9-]+)$", uri)
     if not m:
         log.warning("Can't extract the username from %r", uri)
         return None
     github_username = m.group(1)
-    result = fasjson.search_users(github_username__exact=github_username)
+    result = fasjson.search(github_username__exact=github_username).result
     if len(result) != 1:
         return None
     return result[0]["username"]
 
 
 def distgit2fas(uri, config):
     distgit_hostname = re.escape(config["distgit_hostname"])
@@ -76,15 +78,15 @@
         raise KeyError(
             f"{fields_set.difference(possible)!r} are not possible fields. "
             f"Choose from {possible!r}"
         )
 
 
 def validate_badge(required, possible, badge_dict):
-    fields = frozenset(list(badge_dict.keys()))
+    fields = set(list(badge_dict.keys()))
     validate_possible(possible, fields)
     if required and not required.issubset(fields):
         raise ValueError(
             f"BadgeRule requires {required!r}. Missing {required.difference(fields)!r}"
         )
 
 
@@ -134,14 +136,19 @@
         [
             "bodhi",
             "oscar",
             "apache",
             "koji",
             "bodhi",
             "taskotron",
+            "pagure",
+            "packit",
+            "koschei",
+            "distrobuildsync-eln/jenkins-continuous-infra.apps.ci.centos.org",
+            "osbuild-automation-bot",
         ]
     )
 
     def __init__(self, badge_dict, issuer_id, config, fasjson):
         validate_badge(self.required, self.possible, badge_dict)
         self._d = badge_dict
         self.issuer_id = issuer_id
@@ -177,18 +184,19 @@
 
     def matches(self, msg: Message, tahrir: TahrirDatabase):
 
         # First, do a lightweight check to see if the msg matches a pattern.
         if not self.trigger.matches(msg):
             return set()
 
+        log.debug("Checking match for rule %s", self.badge_id)
         # Before proceeding further, let's see who would get this badge if
         # our more heavyweight checks matched up.  If the user specifies a
         # recipient_key, we can use that to extract the potential awardee.  If
-        # that is not specified, we just use `msg.usernames`.
+        # that is not specified, we just use `msg.agent_name`.
         if self.recipient_key:
             subs = construct_substitutions(msg)
             obj = format_args(self.recipient_key, subs)
 
             if isinstance(obj, (str, int, float)):
                 obj = [obj]
 
@@ -228,16 +236,18 @@
             if self.recipient_distgit2fas:
                 awardees = frozenset([distgit2fas(uri, self.config) for uri in awardees])
 
             if self.recipient_krb2fas:
                 awardees = frozenset([krb2fas(uri) for uri in awardees])
 
             awardees = frozenset([e for e in awardees if e is not None])
+        elif msg.agent_name is not None:
+            awardees = frozenset([msg.agent_name])
         else:
-            awardees = frozenset(msg.usernames)
+            awardees = frozenset()
 
         awardees = awardees.difference(self.banned_usernames)
 
         # Strip anyone who is an IP address
         awardees = frozenset(
             [
                 user
@@ -257,32 +267,31 @@
                 user
                 for user in awardees
                 if not tahrir.assertion_exists(self.badge_id, f"{user}@fedoraproject.org")
                 and not tahrir.person_opted_out(f"{user}@fedoraproject.org")
             ]
         )
 
+        # Make sure the person actually has a FAS account before we award anything.
+        # https://github.com/fedora-infra/tahrir/issues/225
+        awardees = set([u for u in awardees if user_exists_in_fas(self.fasjson, u)])
+
         # If no-one would get the badge at this point, then no reason to waste
         # time doing any further checks.  No need to query datanommer.
         if not awardees:
             return awardees
 
         # Check our backend criteria -- likely, perform datanommer queries.
         try:
             if not self.criteria.matches(msg):
                 return set()
         except OSError:
             log.exception("Failed checking criteria for rule %s", self.badge_id)
             return set()
 
-        # Lastly, and this is probably most expensive.  Make sure the person
-        # actually has a FAS account before we award anything.
-        # https://github.com/fedora-infra/tahrir/issues/225
-        awardees = set([u for u in awardees if user_exists_in_fas(self.fasjson, u)])
-
         return awardees
 
 
 class AbstractComparator(metaclass=abc.ABCMeta):
     """Base class for shared behavior between trigger and criteria."""
 
     possible = required = frozenset()
@@ -304,29 +313,29 @@
 class AbstractTopLevelComparator(AbstractComparator):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         cls = type(self)
 
         if len(self._d) > 1:
             raise ValueError(
-                "No more than one trigger allowed.  " "Use an operator, one of %r" % operators
+                f"No more than one trigger allowed. Use an operator, one of {operators!r}"
             )
         self.attribute = next(iter(self._d))
         self.expected_value = self._d[self.attribute]
 
         # XXX - Check if we should we recursively nest Trigger/Criteria?
 
         # First, trick negation into thinking it is not a unary operator.
         if self.attribute == "not":
             self.expected_value = [self.expected_value]
 
         # Then, treat everything as if it accepts an arbitrary # of args.
         if self.attribute in operators:
             if not isinstance(self.expected_value, list):
-                raise TypeError("Operators only accept lists, not %r" % type(self.expected_value))
+                raise TypeError(f"Operators only accept lists, not {type(self.expected_value)}")
             self.children = [cls(child, self) for child in self.expected_value]
 
 
 class Trigger(AbstractTopLevelComparator):
     possible = (
         frozenset(
             [
@@ -341,19 +350,19 @@
     @graceful(set())
     def matches(self, msg):
         # Check if we should just aggregate the results of our children.
         # Otherwise, we are a leaf-node doing a straightforward comparison.
         if self.children:
             return operator_lookup[self.attribute](child.matches(msg) for child in self.children)
         elif self.attribute == "lambda":
-            return single_argument_lambda_factory(
+            func = single_argument_lambda_factory(
                 expression=self.expected_value,
-                argument={"msg": msg.body, "message": msg},
                 name="msg",
             )
+            return func({"msg": msg.body, "message": msg})
         elif self.attribute == "category":
             return msg.topic.split(".")[3] == self.expected_value
         elif self.attribute == "topic":
             return msg.topic.endswith(self.expected_value)
         else:
             raise RuntimeError(f"Unexpected attribute: {self.attribute}")
 
@@ -408,27 +417,27 @@
         "is less than or equal to": lambda t, v: v <= t,
         "less than or equal to": lambda t, v: v <= t,
         "less than": lambda t, v: v < t,
         "equal to": lambda t, v: v == t,
         "is equal to": lambda t, v: v == t,
         "is not": lambda t, v: v != t,
         "is not equal to": lambda t, v: v != t,
-        "lambda": single_argument_lambda_factory,
+        "lambda": single_argument_lambda,
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if len(self._d["condition"]) > 1:
             conditions = list(self.condition_callbacks.keys())
-            raise ValueError("No more than one condition allowed.  " "Use one of %r" % conditions)
+            raise ValueError(f"No more than one condition allowed. Use one of {conditions}")
 
         # Determine what arguments datanommer.models.Message.grep accepts
-        argspec = inspect.getfullargspec(datanommer.models.Message.grep)
-        irrelevant = frozenset(["defer"])
-        grep_arguments = frozenset(argspec.args[1:]).difference(irrelevant)
+        argspec = inspect.getfullargspec(datanommer.models.Message.make_query)
+        grep_arguments = set(argspec.args[1:])
+        grep_arguments.update({"rows_per_page", "page", "order"})
 
         # Validate the filter
         validate_possible(grep_arguments, self._d["filter"])
 
         # Validate the condition
         condition_key, condition_val = next(iter(self._d["condition"].items()))
         if condition_key not in self.condition_callbacks:
@@ -460,46 +469,83 @@
         if kwargs.get("users") is not None:
             for item in kwargs["users"]:
                 if isinstance(item, list):
                     kwargs["users"] = item
             users = get_pagure_authors(kwargs["users"])
             if users:
                 kwargs["users"] = users
-        kwargs["defer"] = True
-        total, pages, query = datanommer.models.Message.grep(**kwargs)
+        return kwargs
+
+    def _make_query(self, search_kwargs):
+        log.debug("Making datanommer query: %r", search_kwargs)
+        search_kwargs["defer"] = True
+        total, pages, query = datanommer.models.Message.grep(**search_kwargs)
+        query.all = lambda: datanommer.models.session.scalars(query).all()
         return total, pages, query
 
+    def _try_cache_or_make_query(self, msg: Message):
+        search_kwargs = self._construct_query(msg)
+        # Try cached values
+        for CachedValue in DATANOMMER_CACHED_VALUES:
+            cached_value = CachedValue()
+            if not cached_value.is_applicable(search_kwargs, self._d):
+                log.debug(
+                    "%s with kwargs %r is not applicable to %r",
+                    CachedValue.__name__,
+                    search_kwargs,
+                    self._d,
+                )
+                continue
+            log.debug(
+                "Using the cached datanommer value for %s on %r",
+                CachedValue.__name__,
+                search_kwargs,
+            )
+            # Don't update the cache here, there are ~100 rules for a single incoming message and
+            # each could be increasing the value while there's only one actual message.
+            # cached_value.on_message(msg)
+            total, messages = cached_value.get(**search_kwargs)
+            log.debug("Got %s results from cache", total)
+            query = CachedDatanommerQuery(messages)
+            return total, query
+
+        total, pages, query = self._make_query(search_kwargs)
+        return total, query
+
     def _format_lambda_operation(self, msg):
         """Format the string representation of a lambda operation.
 
         The lambda operation can be formatted here to include strings that
         appear in the message being evaluated like
         %(msg.comment.update_submitter)s.  Placeholders like that will have
         their value substituted with whatever appears in the incoming message.
         """
         subs = construct_substitutions(msg)
         operation = format_args(copy.copy(self._d["operation"]), subs)
         return operation["lambda"]
 
+    def _get_value(self, msg: Message):
+        total, query = self._try_cache_or_make_query(msg)
+        if self._d["operation"] == "count":
+            result = total
+        elif isinstance(self._d["operation"], dict):
+            expression = self._format_lambda_operation(msg)
+            func = single_argument_lambda_factory(expression=expression, name="query")
+            result = func(query)
+        else:
+            operation = getattr(query, self._d["operation"])
+            result = operation()
+        return result
+
     def matches(self, msg: Message):
         """A datanommer criteria check is composed of three steps.
 
         - A datanommer query is constructed by combining our yaml definition
           with the incoming fedmsg message that triggered us.
         - An operation in python is constructed by comining our yaml definition
           with the incoming fedmsg message that triggered us.  That operation
           is then executed against the datanommer query object.
         - A condition, derived from our yaml definition, is evaluated with the
           result of the operation from the previous step and is returned.
         """
-        total, pages, query = self._construct_query(msg)
-        if self._d["operation"] == "count":
-            result = total
-        elif isinstance(self._d["operation"], dict):
-            expression = self._format_lambda_operation(msg)
-            result = single_argument_lambda_factory(
-                expression=expression, argument=query, name="query"
-            )
-        else:
-            operation = getattr(query, self._d["operation"])
-            result = operation()
+        result = self._get_value(msg)
         return self.condition(result)
```

### Comparing `fedbadges-2.0.0/fedbadges/rulesrepo.py` & `fedbadges-2.1.1/fedbadges/rulesrepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 except ValueError as e:
                     log.error("Initializing rule for %r failed with %r", fname, e)
 
         log.info("Loaded %s total badge definitions", len(badges))
         return badges
 
     def _load_badge_from_yaml(self, fname):
-        log.debug("Loading %r" % fname)
+        log.debug(f"Loading {fname!r}")
         try:
             with open(fname) as f:
                 return yaml.safe_load(f.read())
         except Exception as e:
             log.error("Loading %r failed with %r", fname, e)
             return None
```

### Comparing `fedbadges-2.0.0/fedbadges.toml.example` & `fedbadges-2.1.1/fedbadges.toml.example`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,22 @@
 # Datanommer database URI
 datanommer_db_uri = "sqlite:////tmp/datanommer.db"
 datagrepper_url = "https://apps.fedoraproject.org/datagrepper"
 distgit_hostname = "src.fedoraproject.org"
 id_provider_hostname = "id.fedoraproject.org"
 fasjson_base_url = "https://fasjson.fedoraproject.org"
 
+# Check for new rules every these many minutes
+rules_reload_interval = 15
+
+# Cache configuation
+[consumer_config.cache]
+backend = "dogpile.cache.memory"
+expiration_time = 3600
+
 # This is a set of data that tells our consumer what Open Badges Issuer
 # should be kept as the issuer of all the badges we create.
 [consumer_config.badge_issuer]
 issuer_id = "fedora"
 issuer_name = "Fedora Project"
 issuer_origin = "http://badges.fedoraproject.org"
 issuer_url = "http://fedoraproject.org"
```

### Comparing `fedbadges-2.0.0/pyproject.toml` & `fedbadges-2.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fedbadges"
-version = "2.0.0"
+version = "2.1.1"
 description = "Fedora Messaging consumer for awarding open badges"
 
 license = "GPL-2.0-or-later"
 
 authors = [
   "Fedora Infrastructure <admin@fedoraproject.org>"
 ]
@@ -32,22 +32,26 @@
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic-settings = "^2.0.2"
 pyyaml = "^6.0.1"
-datanommer-models = "^1.2.0"
+datanommer-models = "^1.3.0"
+#datanommer-models = { git = "https://github.com/fedora-infra/datanommer.git", branch = "develop", subdirectory = "datanommer.models" }
 requests = "^2.31.0"
 psutil = "^5.9.8"
 fedora-messaging = "^3.5.0"
 backoff = "^2.2.1"
 fasjson-client = "^1.0.8"
 click = "^8.0.0"
 tahrir-api = "^1.0.0"
+dogpile-cache = "^1.3.2"
+pymemcache = {version = "^4.0.0", optional = true}
+redis = {version = "^5.0.4", optional = true}
 
 # Message schemas. The reference list of all message schemas is in
 # https://github.com/fedora-infra/fedora-messaging/blob/develop/docs/schema-packages.txt
 anitya-schema = {version = "*", optional = true}
 bodhi-messages = {version = "*", optional = true}
 bugzilla2fedmsg-schema = {version = "*", optional = true}
 ci-messages = {version = "*", optional = true}
@@ -59,14 +63,15 @@
 fedora-messaging-git-hook-messages = {version = "*", optional = true}
 fedora-messaging-the-new-hotness-schema = {version = "*", optional = true}
 fedora-planet-messages = {version = "*", optional = true}
 fmn-messages = {version = "*", optional = true}
 kerneltest-messages = {version = "^1.0.0", optional = true}
 koji-fedoramessaging-messages = {version = "^1.2.2", optional = true}
 koschei-messages = {version = "*", optional = true}
+maubot-fedora-messages = {version = "*", optional = true}
 mediawiki-messages = {version = "*", optional = true}
 meetbot-messages = {version = "*", optional = true}
 mdapi-messages = {version = "*", optional = true}
 noggin-messages = {version = "*", optional = true}
 nuancier-messages = {version = "*", optional = true}
 pagure-messages = {version = "*", optional = true}
 tahrir-messages = {version = "*", optional = true}
@@ -100,22 +105,29 @@
   "fedora-messaging-git-hook-messages",
   "fedora-messaging-the-new-hotness-schema",
   "fedora-planet-messages",
   "fmn-messages",
   "kerneltest-messages",
   "koji-fedoramessaging-messages",
   "koschei-messages",
+  "maubot-fedora-messages",
   "mediawiki-messages",
   "meetbot-messages",
   "mdapi-messages",
   "noggin-messages",
   "nuancier-messages",
   "pagure-messages",
   "tahrir-messages",
 ]
+memcache = [
+  "pymemcache",
+]
+redis = [
+  "redis",
+]
 
 [tool.poetry.scripts]
 award-badges-dev = "fedbadges.manual.badges_dev:main"
 award-libravatar = "fedbadges.manual.libravatar:main"
 award-lifecycle = "fedbadges.manual.lifecycle:main"
 award-mirror = "fedbadges.manual.mirror:main"
 award-group-membership = "fedbadges.manual.group_membership:main"
```

### Comparing `fedbadges-2.0.0/tests/conftest.py` & `fedbadges-2.1.1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from unittest.mock import Mock, patch
 
 import datanommer
 import pytest
 from fedora_messaging.config import conf
 from tahrir_api import dbapi
 
+from fedbadges.cached import configure as configure_cache
 from fedbadges.consumer import FedoraBadgesConsumer
 from fedbadges.rulesrepo import RulesRepo
 
 
 @pytest.fixture()
 def grep():
     grep_spec = inspect.getfullargspec(datanommer.models.Message.grep)
@@ -24,14 +25,15 @@
         badges_repo="tests/test_badges",
         database_uri=f"sqlite:///{tmp_path.as_posix()}/badges.db",
         datanommer_db_uri=f"sqlite:///{tmp_path.as_posix()}/datanommer.db",
         datagrepper_url="https://example.com/datagrepper",
         distgit_hostname="src.example.com",
         id_provider_hostname="id.example.com",
         fasjson_base_url="https://fasjson.example.com",
+        cache=dict(backend="dogpile.cache.null", expiration_time=0),
         badge_issuer=dict(
             issuer_id="test-issuer",
             issuer_name="Testing",
             issuer_origin="http://badges.example.com",
             issuer_url="http://example.com",
             issuer_email="badges@example.com",
         ),
@@ -83,7 +85,13 @@
     yield badges_db
 
 
 @pytest.fixture()
 def rules(fm_config, fasjson_client, tahrir_client):
     repo = RulesRepo(conf["consumer_config"], 1, fasjson_client)
     return repo.load_all(tahrir_client=tahrir_client)
+
+
+@pytest.fixture()
+def cache_configured(fm_config):
+    cache_args = conf["consumer_config"]["cache"]
+    configure_cache(**cache_args)
```

### Comparing `fedbadges-2.0.0/tests/test_badges/rules/bodhi-update-fancy.yaml` & `fedbadges-2.1.1/tests/test_badges/rules/bodhi-update-fancy.yaml`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tests/test_badges/rules/bodhi-update-simple.yaml` & `fedbadges-2.1.1/tests/test_badges/rules/bodhi-update-simple.yaml`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tests/test_badges/rules/irc-speak-up.yml` & `fedbadges-2.1.1/tests/test_badges/rules/irc-speak-up.yml`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tests/test_badges/rules/pagure-long-live.yaml` & `fedbadges-2.1.1/tests/test_badges/rules/pagure-long-live.yaml`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tests/test_badges/rules/tagger-01.yml` & `fedbadges-2.1.1/tests/test_badges/rules/tagger-01.yml`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tests/test_complicated_recipient.py` & `fedbadges-2.1.1/tests/test_complicated_recipient.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class MockQuery:
     def count(self):
         return float("inf")  # Master tagger
 
 
 def test_complicated_recipient_real(
+    cache_configured,
     rules,
     tahrir_client,
 ):
     rule = get_rule(rules, "Speak Up!")
     msg = Message(
         topic="org.fedoraproject.prod.meetbot.meeting.complete",
         body={
@@ -26,17 +27,17 @@
             "url": "fedora-meeting.2013-06-24-19.52",
             "owner": "threebean",
             "channel": "#fedora-meeting",
         },
     )
     with (
         patch("fedbadges.rules.user_exists_in_fas") as g,
-        patch("datanommer.models.Message.grep") as grep,
+        patch("fedbadges.cached.CachedDatanommerValue._year_split_query") as run_query,
     ):
-        grep.return_value = float("inf"), 1, MockQuery()
+        run_query.return_value = float("inf"), MockQuery()
         g.return_value = True
         assert rule.matches(msg, tahrir_client) == {"zodbot", "threebean"}
 
 
 def test_complicated_recipient_pagure(
     rules,
     tahrir_client,
```

### Comparing `fedbadges-2.0.0/tests/test_complicated_trigger.py` & `fedbadges-2.1.1/tests/test_complicated_trigger.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tests/test_criteria_datanommer.py` & `fedbadges-2.1.1/tests/test_criteria_datanommer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,38 +12,38 @@
     def __init__(self, returned_count):
         self.returned_count = returned_count
 
     def count(self):
         return self.returned_count
 
 
-def test_malformed_criteria():
+def test_malformed_criteria(cache_configured):
     """Test that an error is raised when nonsense is provided."""
     with pytest.raises(KeyError):
         fedbadges.rules.Criteria(
             dict(
                 watwat="does not exist",
             )
         )
 
 
-def test_underspecified_criteria():
+def test_underspecified_criteria(cache_configured):
     """Test that an error is raised when condition is missing."""
     with pytest.raises(ValueError):
         fedbadges.rules.Criteria(
             dict(
                 datanommer={
                     "filter": {"topics": ["%(topic)s"], "wat": "baz"},
                     "operation": "count",
                 }
             )
         )
 
 
-def test_malformed_filter():
+def test_malformed_filter(cache_configured):
     """Test that an error is raised for malformed filters"""
     with pytest.raises(KeyError):
         fedbadges.rules.Criteria(
             dict(
                 datanommer={
                     "filter": {"topics": ["%(topic)s"], "wat": "baz"},
                     "operation": "count",
@@ -59,15 +59,15 @@
     ["returned_count", "expectation"],
     [
         (499, False),
         (500, True),
         (501, True),
     ],
 )
-def test_basic_datanommer(returned_count, expectation):
+def test_basic_datanommer(cache_configured, returned_count, expectation):
     criteria = fedbadges.rules.Criteria(
         dict(
             datanommer={
                 "filter": {
                     "topics": ["%(topic)s"],
                 },
                 "operation": "count",
@@ -76,33 +76,33 @@
                 },
             }
         )
     )
     message = Message(
         topic="org.fedoraproject.dev.something.sometopic",
     )
-    with patch("datanommer.models.Message.grep") as grep:
-        grep.return_value = returned_count, 1, MockQuery(returned_count)
+    with patch("fedbadges.cached.CachedDatanommerValue._year_split_query") as run_query:
+        run_query.return_value = returned_count, MockQuery(returned_count)
         result = criteria.matches(message)
         assert result == expectation
-        grep.assert_called_once_with(
+        run_query.assert_called_once_with(
             topics=["org.fedoraproject.dev.something.sometopic"],
             defer=True,
         )
 
 
 @pytest.mark.parametrize(
     ["returned_count", "expectation"],
     [
         (499, False),
         (500, True),
         (501, True),
     ],
 )
-def test_datanommer_with_lambda_condition(returned_count, expectation):
+def test_datanommer_with_lambda_condition(cache_configured, returned_count, expectation):
     criteria = fedbadges.rules.Criteria(
         dict(
             datanommer={
                 "filter": {
                     "topics": ["%(topic)s"],
                 },
                 "operation": "count",
@@ -111,29 +111,29 @@
                 },
             }
         )
     )
     message = Message(
         topic="org.fedoraproject.dev.something.sometopic",
     )
-    with patch("datanommer.models.Message.grep") as f:
-        f.return_value = returned_count, 1, MockQuery(returned_count)
+    with patch("fedbadges.cached.CachedDatanommerValue._year_split_query") as run_query:
+        run_query.return_value = returned_count, MockQuery(returned_count)
         result = criteria.matches(message)
         assert result == expectation
 
 
 @pytest.mark.parametrize(
     ["returned_count", "expectation"],
     [
         (4, False),
         (5, True),
         (6, False),
     ],
 )
-def test_datanommer_formatted_operations(returned_count, expectation):
+def test_datanommer_formatted_operations(cache_configured, returned_count, expectation):
     criteria = fedbadges.rules.Criteria(
         dict(
             datanommer={
                 "filter": {
                     "topics": ["%(topic)s"],
                 },
                 "operation": {
@@ -147,29 +147,29 @@
     )
     message = Message(
         topic="org.fedoraproject.dev.something.sometopic",
         body=dict(
             some_value=5,
         ),
     )
-    with patch("datanommer.models.Message.grep") as grep:
-        grep.return_value = returned_count, 1, MockQuery(returned_count)
+    with patch("fedbadges.cached.CachedDatanommerValue._year_split_query") as run_query:
+        run_query.return_value = returned_count, MockQuery(returned_count)
         result = criteria.matches(message)
         assert result == expectation
 
 
 @pytest.mark.parametrize(
     ["returned_count", "expectation"],
     [
         (499, False),
         (500, True),
         (501, True),
     ],
 )
-def test_datanommer_with_lambda_operation(returned_count, expectation):
+def test_datanommer_with_lambda_operation(cache_configured, returned_count, expectation):
     criteria = fedbadges.rules.Criteria(
         dict(
             datanommer={
                 "filter": {
                     "topics": ["%(topic)s"],
                 },
                 "operation": {
@@ -180,21 +180,21 @@
                 },
             }
         )
     )
     message = Message(
         topic="org.fedoraproject.dev.something.sometopic",
     )
-    with patch("datanommer.models.Message.grep") as grep:
-        grep.return_value = returned_count, 1, MockQuery(returned_count)
+    with patch("fedbadges.cached.CachedDatanommerValue._year_split_query") as run_query:
+        run_query.return_value = returned_count, MockQuery(returned_count)
         result = criteria.matches(message)
         assert result == expectation
 
 
-def test_datanommer_with_lambda_filter():
+def test_datanommer_with_lambda_filter(cache_configured):
     criteria = fedbadges.rules.Criteria(
         dict(
             datanommer={
                 "filter": {
                     "users": {
                         "lambda": "[u for u in msg['message'].usernames "
                         "if not u in ['bodhi', 'hadess']]",
@@ -214,15 +214,15 @@
     with patch("datanommer.models.Message.grep") as grep:
         grep.return_value = returned_count, 1, MockQuery(returned_count)
         result = criteria.matches(message)
         assert result is True
         grep.assert_called_once_with(users=["lmacken"], defer=True)
 
 
-def test_datanommer_with_dotted_filter():
+def test_datanommer_with_dotted_filter(cache_configured):
     criteria = fedbadges.rules.Criteria(
         dict(
             datanommer={
                 "filter": {
                     "users": [
                         "%(msg.update.user.name)s",
                     ]
```

### Comparing `fedbadges-2.0.0/tests/test_rule_matching.py` & `fedbadges-2.1.1/tests/test_rule_matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from types import SimpleNamespace
 from unittest.mock import Mock, patch
 
 import pytest
 from fedora_messaging.message import Message
 from noggin_messages import MemberSponsorV1
 
 import fedbadges.rules
@@ -66,15 +67,15 @@
 
     msg = example_real_bodhi_message
 
     with patch("datanommer.models.Message.grep") as f:
         f.return_value = 1, 1, MockQuery()
         with patch("fedbadges.rules.user_exists_in_fas") as g:
             g.return_value = True
-            assert rule.matches(msg, tahrir_client) == set(["lmacken", "hadess"])
+            assert rule.matches(msg, tahrir_client) == {"lmacken"}
 
 
 def test_full_simple_match_almost_succeed(fasjson_client, tahrir_client):
     """A simple integration test for messages with zero users"""
     rule = fedbadges.rules.BadgeRule(
         dict(
             name="Test",
@@ -130,15 +131,15 @@
             criteria=dict(
                 datanommer=dict(
                     filter=dict(categories=["pkgdb"]),
                     operation="count",
                     condition={"greater than or equal to": 1},
                 )
             ),
-            recipient="%(msg.agent.username)s",
+            recipient=["%(msg.agent.username)s", "%(msg.user.username)s"],
         ),
         1,
         None,
         fasjson_client,
     )
     rule.setup(tahrir_client)
 
@@ -151,15 +152,15 @@
         },
     )
 
     with patch("datanommer.models.Message.grep") as f:
         f.return_value = 1, 1, MockQuery()
         with patch("fedbadges.rules.user_exists_in_fas") as g:
             g.return_value = True
-            assert rule.matches(msg, tahrir_client) == set(["toshio"])
+            assert rule.matches(msg, tahrir_client) == {"toshio", "ralph"}
 
 
 def test_yaml_specified_awardee_failure(fasjson_client, tahrir_client):
     """Test that when we don't override msg.usernames, we get 2 awardees."""
     rule = fedbadges.rules.BadgeRule(
         dict(
             name="Test",
@@ -194,15 +195,15 @@
         },
     )
 
     with patch("datanommer.models.Message.grep") as f:
         f.return_value = 1, 1, MockQuery()
         with patch("fedbadges.rules.user_exists_in_fas") as g:
             g.return_value = True
-            assert rule.matches(msg, tahrir_client) == set(["toshio", "ralph"])
+            assert rule.matches(msg, tahrir_client) == {"toshio"}
 
 
 def test_against_duplicates(fasjson_client, tahrir_client):
     """Test that matching fails if user already has the badge."""
 
     rule = fedbadges.rules.BadgeRule(
         dict(
@@ -216,14 +217,15 @@
             criteria=dict(
                 datanommer=dict(
                     filter=dict(categories=["pkgdb"]),
                     operation="count",
                     condition={"greater than or equal to": 1},
                 )
             ),
+            recipient="%(usernames)s",
         ),
         1,
         None,
         fasjson_client,
     )
     rule.setup(tahrir_client)
     tahrir_client.add_person("toshio@fedoraproject.org")
@@ -282,17 +284,17 @@
     msg = Message(
         topic="org.fedoraproject.prod.bodhi.update.request.testing",
         body={"user": "https://api.github.com/users/dummygh"},
     )
 
     with patch("datanommer.models.Message.grep") as f:
         f.return_value = 1, 1, MockQuery()
-        fasjson_client.search_users.return_value = [{"username": "dummy"}]
+        fasjson_client.search.return_value = SimpleNamespace(result=[{"username": "dummy"}])
         assert rule.matches(msg, tahrir_client) == set(["dummy"])
-        fasjson_client.search_users.assert_called_once_with(github_username__exact="dummygh")
+        fasjson_client.search.assert_called_once_with(github_username__exact="dummygh")
 
 
 def test_krb_awardee(fasjson_client, tahrir_client):
     """Conversion from Kerberos user to FAS users"""
     rule = fedbadges.rules.BadgeRule(
         dict(
             name="Test",
```

### Comparing `fedbadges-2.0.0/tests/test_triggers.py` & `fedbadges-2.1.1/tests/test_triggers.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tests/test_utils.py` & `fedbadges-2.1.1/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from fedora_messaging.message import Message
 
 from fedbadges.utils import (
     construct_substitutions,
     format_args,
-    single_argument_lambda_factory,
+    single_argument_lambda,
 )
 
 
 def test_lambda_factory():
     expression = "value + 2"
     target = 4
-    actual = single_argument_lambda_factory(expression, 2)
+    actual = single_argument_lambda(expression, 2)
     assert actual == target
 
 
 def test_substitutions_basic():
     msg = Message(body=dict(a=dict(b=dict(c=42))))
     target = {
         "msg": dict(a=dict(b=dict(c=42))),
         "msg.a": dict(b=dict(c=42)),
         "msg.a.b": dict(c=42),
         "msg.a.b.c": 42,
         "topic": "",
+        "usernames": [],
     }
     actual = construct_substitutions(msg)
     assert actual == target
 
 
 def test_substitutions_real():
     msg = Message(
@@ -46,22 +47,23 @@
                 "pk": 2,
                 "post_type": "question",
             },
         },
         topic="org.fedoraproject.dev.askbot.post.edit",
     )
     target = {
+        "topic": "org.fedoraproject.dev.askbot.post.edit",
+        "usernames": [],
         "msg.post.text": "alskdfjalskdjf alkjasdalskdjf ...",
         "msg.thread.title": "alskdjflaksjdf lakjsf a",
         "msg.post.vote_down_count": 0,
         "msg.post.post_type": "question",
         "msg.thread.pk": 2,
         "msg.newly_mentioned_users": [],
         "msg.diff": "<p>alskdfj... the diff is actually here",
-        "topic": "org.fedoraproject.dev.askbot.post.edit",
         "msg.agent": "ralph",
         "msg.post.comment_count": 0,
         "msg.post": {
             "vote_up_count": 0,
             "text": "alskdfjalskdjf alkjasdalskdjf ...",
             "summary": "alskdfjalskdjf alkjasdalskdjf ...",
             "comment_count": 0,
```

### Comparing `fedbadges-2.0.0/tests/utils.py` & `fedbadges-2.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/tox.ini` & `fedbadges-2.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `fedbadges-2.0.0/PKG-INFO` & `fedbadges-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 Metadata-Version: 2.1
 Name: fedbadges
-Version: 2.0.0
+Version: 2.1.1
 Summary: Fedora Messaging consumer for awarding open badges
 Home-page: https://github.com/fedora-infra/fedbadges
 License: GPL-2.0-or-later
 Keywords: fedora
 Author: Fedora Infrastructure
 Author-email: admin@fedoraproject.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: memcache
+Provides-Extra: redis
 Provides-Extra: schemas
 Requires-Dist: anitya-schema ; extra == "schemas"
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: bodhi-messages ; extra == "schemas"
 Requires-Dist: bugzilla2fedmsg-schema ; extra == "schemas"
 Requires-Dist: ci-messages ; extra == "schemas"
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: copr-messaging ; extra == "schemas"
-Requires-Dist: datanommer-models (>=1.2.0,<2.0.0)
+Requires-Dist: datanommer-models (>=1.3.0,<2.0.0)
 Requires-Dist: discourse2fedmsg-messages ; extra == "schemas"
+Requires-Dist: dogpile-cache (>=1.3.2,<2.0.0)
 Requires-Dist: fasjson-client (>=1.0.8,<2.0.0)
 Requires-Dist: fedocal-messages ; extra == "schemas"
 Requires-Dist: fedora-elections-messages ; extra == "schemas"
 Requires-Dist: fedora-messaging (>=3.5.0,<4.0.0)
 Requires-Dist: fedora-messaging-git-hook-messages ; extra == "schemas"
 Requires-Dist: fedora-messaging-the-new-hotness-schema ; extra == "schemas"
 Requires-Dist: fedora-planet-messages ; extra == "schemas"
 Requires-Dist: fedorainfra-ansible-messages ; extra == "schemas"
 Requires-Dist: fmn-messages ; extra == "schemas"
 Requires-Dist: kerneltest-messages (>=1.0.0,<2.0.0) ; extra == "schemas"
 Requires-Dist: koji-fedoramessaging-messages (>=1.2.2,<2.0.0) ; extra == "schemas"
 Requires-Dist: koschei-messages ; extra == "schemas"
+Requires-Dist: maubot-fedora-messages ; extra == "schemas"
 Requires-Dist: mdapi-messages ; extra == "schemas"
 Requires-Dist: mediawiki-messages ; extra == "schemas"
 Requires-Dist: meetbot-messages ; extra == "schemas"
 Requires-Dist: noggin-messages ; extra == "schemas"
 Requires-Dist: nuancier-messages ; extra == "schemas"
 Requires-Dist: pagure-messages ; extra == "schemas"
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
+Requires-Dist: pymemcache (>=4.0.0,<5.0.0) ; extra == "memcache"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: redis (>=5.0.4,<6.0.0) ; extra == "redis"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tahrir-api (>=1.0.0,<2.0.0)
 Requires-Dist: tahrir-messages ; extra == "schemas"
 Project-URL: Repository, https://github.com/fedora-infra/fedbadges
 Description-Content-Type: text/x-rst
 
 Fedora Badges Message consumer
@@ -101,20 +107,20 @@
   **Aside:** Although datanommer is the only currently supported backend, we
   can implement other queryable backend in the future as needed like FAS
   (to see if the user is in X number of groups) or even off-site services
   like libravatar (to award a badge if the user is a user of the AGPL web
   service).
 
 * If a badge's ``trigger`` and ``criteria`` both match, then the badge is
-  awarded.  If the BadgeRule doesn't specify, we award the badge to all
-  usernames returned by the message's ``usernames`` property.
+  awarded.  If the BadgeRule doesn't specify, we award the badge to the
+  author of the action using the message's ``agent_name`` property.
 
   That is usually correct -- but sometimes, a BadgeRule needs to specify
-  that one particular user (not all related users) should be recipients of
-  the badge.  In this case, the BadgeRule may define a ``recipient``
+  that one particular user should be recipient of the badge.
+  In this case, the BadgeRule may define a ``recipient``
   in dot-notation that instructs the ``Consumer`` how to extract the
   recipient's username from the received message.
 
   The badge is awarded to our deserving user via the `tahrir_api
   <https://github.com/fedora-infra/tahrir-api>`_.  At the end of the day,
   this amounts to adding a row in a database table for the `Tahrir
   <https://github.com/fedora-infra/tahrir>`_ application.
@@ -240,15 +246,15 @@
 off by *any* user at any time in the past.  Pretty generic.
 Here's a more interesting criteria definition::
 
     criteria:
       filter:
         topics:
         - org.fedoraproject.prod.git.receive
-        usernames:
+        users:
         - "%(msg.commit.username)s"
       operation: count
       condition:
         greater than or equal to: 50
 
 This criteria would match if there existed 50 messages of the topic
 ``"org.fedoraproject.prod.git.receive"`` that were also kicked off by whatever
@@ -279,53 +285,54 @@
 statement you provide into a callable and use that at runtime.  For example::
 
 
     criteria:
       filter:
         topics:
         - org.fedoraproject.prod.git.receive
-        usernames:
+        users:
         - "%(msg.commit.username)s"
       operation: count
       condition:
         lambda: value != 0 and ((value & (value - 1)) == 0)
 
 Who knows why you would want to do this, but the above criteria check will
 succeed if the number of messages returned from the filtered datanommer query
 is exactly a power of 2.
 
 Specifying Recipients
 ~~~~~~~~~~~~~~~~~~~~~
 
 By default, if the trigger and criteria match, fedbadges will award badges
-to all the users returned by the message's ``usernames`` property.
-This *usually* corresponds with "what users are responsible" for this message.
+to the user returned by the message's ``agent_name`` property.
+This *usually* corresponds with "which user is responsible" for this message.
 That is *usually* what we want to award badges for.
 
 There are some instances for which that is not what we want.
 
-Take the `org.fedoraproject.prod.fas.group.member.sponsor
-<https://fedora-messaging.readthedocs.io/en/stable/user-guide/schemas.html#fas>`_
-message for example.  When user A sponsors user B to a group, both
-usernames are returned by the message's ``usernames`` property with no
-further distinction as to which was adding and which was added.
-
-Imagine we have a "Group Sponsor" badge that's awarded to group admins who
-sponsor users to groups.  We don't want to inadvertently award that badge
-to the persons who *were sponsored*, only to those who *sponsored them*.
+Take the `org.fedoraproject.prod.bodhi.update.comment
+<https://fedora-messaging.readthedocs.io/en/stable/user-guide/schemas.html#bodhi>`_
+message for example.  When user A comments on user B's update, user A is returned
+by the message's ``agent_name`` property.
+
+Imagine we have a "Received Comments" badge that's awarded to packagers that
+received comments on their updates.  We don't want to inadvertently award that
+badge to the person who *commented*, only to the one who *created the update*.
 
 To allow for this scenario, badges may optionally define a ``recipient``
 in dotted notation that tells fedbadges where to find the username of the
 recipient in the originating message.  For instance, the following would
 handle the fas case we described above::
 
     trigger:
-      topic: org.fedoraproject.prod.fas.group.member.sponsor
+      topic: org.fedoraproject.prod.bodhi.update.comment
     criteria:
       filter:
         topics:
         - "%(topic)s"
+        users:
+        - "%(msg.update.user.name)s"
       operation: count
       condition:
         greater than or equal to: 1
-    recipient: "%(msg.agent_name)s"
+    recipient: "%(msg.update.user.name)s"
```

