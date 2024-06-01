# Comparing `tmp/simplelogincmd-0.1.0.tar.gz` & `tmp/simplelogincmd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplelogincmd-0.1.0.tar", max compression
+gzip compressed data, was "simplelogincmd-0.2.0.tar", max compression
```

## Comparing `simplelogincmd-0.1.0.tar` & `simplelogincmd-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0     1072 2024-05-22 21:06:15.325024 simplelogincmd-0.1.0/LICENSE
--rw-r--r--   0        0        0      241 2024-05-25 04:15:18.994129 simplelogincmd-0.1.0/README.md
--rw-r--r--   0        0        0      578 2024-05-24 21:22:27.527945 simplelogincmd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-25 03:36:09.024944 simplelogincmd-0.1.0/simplelogincmd/__init__.py
--rw-r--r--   0        0        0       49 2024-05-23 21:36:44.405396 simplelogincmd-0.1.0/simplelogincmd/cli/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-24 21:06:23.628278 simplelogincmd-0.1.0/simplelogincmd/cli/commands/__init__.py
--rw-r--r--   0        0        0     2630 2024-05-24 21:06:57.868267 simplelogincmd-0.1.0/simplelogincmd/cli/commands/account.py
--rw-r--r--   0        0        0    13964 2024-05-24 21:07:18.328260 simplelogincmd-0.1.0/simplelogincmd/cli/commands/alias.py
--rw-r--r--   0        0        0     3640 2024-05-24 21:07:34.798257 simplelogincmd-0.1.0/simplelogincmd/cli/commands/mailbox.py
--rw-r--r--   0        0        0    11705 2024-05-23 21:37:46.655374 simplelogincmd-0.1.0/simplelogincmd/cli/const.py
--rw-r--r--   0        0        0      825 2024-05-24 21:07:46.658253 simplelogincmd-0.1.0/simplelogincmd/cli/exceptions.py
--rw-r--r--   0        0        0     1303 2024-05-24 21:08:06.608247 simplelogincmd-0.1.0/simplelogincmd/cli/main.py
--rw-r--r--   0        0        0     6245 2024-05-24 21:10:58.378190 simplelogincmd-0.1.0/simplelogincmd/cli/util.py
--rw-r--r--   0        0        0     2413 2024-05-24 21:17:22.588050 simplelogincmd-0.1.0/simplelogincmd/config.py
--rw-r--r--   0        0        0      286 2024-05-23 23:39:35.772839 simplelogincmd-0.1.0/simplelogincmd/const.py
--rw-r--r--   0        0        0      114 2024-05-24 21:04:25.338317 simplelogincmd-0.1.0/simplelogincmd/rest/__init__.py
--rw-r--r--   0        0        0     3279 2024-05-23 21:20:41.475728 simplelogincmd-0.1.0/simplelogincmd/rest/client.py
--rw-r--r--   0        0        0      784 2024-05-24 21:10:13.318204 simplelogincmd-0.1.0/simplelogincmd/rest/const.py
--rw-r--r--   0        0        0      197 2024-05-24 13:42:52.235821 simplelogincmd-0.1.0/simplelogincmd/rest/exceptions.py
--rw-r--r--   0        0        0     6855 2024-05-23 21:32:04.375492 simplelogincmd-0.1.0/simplelogincmd/rest/models.py
--rw-r--r--   0        0        0    20892 2024-05-24 21:09:56.998210 simplelogincmd-0.1.0/simplelogincmd/rest/simplelogin.py
--rw-r--r--   0        0        0     2419 2024-05-24 21:12:04.938165 simplelogincmd-0.1.0/simplelogincmd/rest/util.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 simplelogincmd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/LICENSE
+-rw-r--r--   0        0        0      650 2024-05-25 08:26:46.389923 simplelogincmd-0.2.0/README.md
+-rw-r--r--   0        0        0      630 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2630 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/commands/account.py
+-rw-r--r--   0        0        0    13896 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/commands/alias.py
+-rw-r--r--   0        0        0     1424 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/commands/database.py
+-rw-r--r--   0        0        0     4016 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/commands/mailbox.py
+-rw-r--r--   0        0        0    12839 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/const.py
+-rw-r--r--   0        0        0      825 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/exceptions.py
+-rw-r--r--   0        0        0     1378 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/main.py
+-rw-r--r--   0        0        0     7787 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/util.py
+-rw-r--r--   0        0        0     2956 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/config.py
+-rw-r--r--   0        0        0      322 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/const.py
+-rw-r--r--   0        0        0      106 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/__init__.py
+-rw-r--r--   0        0        0     4293 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/access_layer.py
+-rw-r--r--   0        0        0     9488 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/models.py
+-rw-r--r--   0        0        0     1087 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/session.py
+-rw-r--r--   0        0        0      114 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/__init__.py
+-rw-r--r--   0        0        0     3279 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/client.py
+-rw-r--r--   0        0        0      784 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/const.py
+-rw-r--r--   0        0        0      197 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/exceptions.py
+-rw-r--r--   0        0        0    20896 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/rest/simplelogin.py
+-rw-r--r--   0        0        0     2419 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/util.py
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 simplelogincmd-0.2.0/PKG-INFO
```

### Comparing `simplelogincmd-0.1.0/LICENSE` & `simplelogincmd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.1.0/pyproject.toml` & `simplelogincmd-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "simplelogincmd"
-version = "0.1.0"
+version = "0.2.0"
 description = "SimpleLogin command-line application"
 authors = ["truthless-dev <truthless.deviant248@simplelogin.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.32.2"
 click = "^8.1.7"
+sqlalchemy = "^2.0.30"
+sqlalchemy-utils = "^0.41.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.1"
 responses = "^0.25.0"
 black = "^24.4.2"
 Sphinx = "^7.3.7"
 toml = "^0.10.2"
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/commands/__init__.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/commands/account.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/commands/alias.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/commands/alias.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 - toggle
 - update
 """
 
 import click
 
 from simplelogincmd.cli import const, util
+from simplelogincmd.database.models import (
+    Alias,
+    Mailbox,
+)
 
 
 @click.group(
     "alias",
     short_help=const.HELP.ALIAS.SHORT,
     help=const.HELP.ALIAS.LONG,
 )
@@ -37,35 +41,36 @@
     "activity",
     short_help=const.HELP.ALIAS.ACTIVITY.SHORT,
     help=const.HELP.ALIAS.ACTIVITY.LONG,
     epilog=const.HELP.ALIAS.ACTIVITY.EPILOG,
 )
 @click.argument(
     "id",
-    type=int,
 )
 @click.option(
     "-i",
     "--include",
     help=const.HELP.ALIAS.ACTIVITY.OPTION.INCLUDE,
 )
 @click.option(
     "-e",
     "--exclude",
     help=const.HELP.ALIAS.ACTIVITY.OPTION.EXCLUDE,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
-def activity(sl, id: int, include: str | None, exclude: str | None) -> None:
+def activity(sl, db, id: int, include: str | None, exclude: str | None) -> None:
     """Display alias activities in a tabular format"""
     fields = util.get_display_fields_from_options(
         const.ACTIVITY_FIELD_ORDER, include, exclude
     )
     if len(fields) == 0:
         return
+    id = util.resolve_id(db, Alias, id)
     activities = sl.get_all_alias_activities(id)
     if len(activities) == 0:
         click.echo("No activities found")
         return
     util.display_model_list(activities, fields)
 
 
@@ -115,18 +120,20 @@
     "--yes",
     "bypass_confirmation",
     is_flag=True,
     flag_value=True,
     default=False,
     help=const.HELP.ALIAS.CUSTOM.OPTION.YES,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
 def custom(
     sl,
+    db,
     hostname: str | None,
     prefix: str,
     mailboxes: tuple[str],
     note: str | None,
     name: str | None,
     select_suffix: int | None,
     bypass_confirmation: bool,
@@ -147,31 +154,18 @@
     if (recommendation := data.get("recommendation")) is not None:
         rec_alias = recommendation.get("alias", "Another alias")
         rec_host = recommendation.get("hostname", "that site")
         click.echo(f"{rec_alias} has already been used on {rec_host}.")
         if not bypass_confirmation:
             click.confirm("Create a new alias anyway?", abort=True)
 
+    mailbox_ids = {util.resolve_id(db, Mailbox, mb_id) for mb_id in mailboxes}
     if note == "_EDIT":
         note = util.edit()
 
-    # Get the user's mailboxes and check them against the ids/addresses
-    # they provided. This allows us to accept addresses as well as ids,
-    # and to fail early if no valid mailboxes match.
-    mailbox_ids = set()
-    actual_mailboxes = sl.get_mailboxes()
-    for mailbox in actual_mailboxes:
-        id = mailbox.field_as_string("id")
-        email = mailbox.email
-        if id in mailboxes or email in mailboxes:
-            mailbox_ids.add(mailbox.id)
-    if len(mailbox_ids) == 0:
-        click.echo("Invalid mailbox list")
-        return False
-
     # If `select_suffix` is not set or out of range, prompt the user
     # for which suffix to use.
     if (suffixes := data.get("suffixes")) is None:
         click.echo("Error retrieving alias suffixes")
         return False
     if select_suffix is None or not (0 <= select_suffix < len(suffixes)):
         options = [suffix["suffix"] for suffix in suffixes]
@@ -208,75 +202,81 @@
         note=note,
         name=name,
         hostname=hostname,
     )
     if not success:
         click.echo(obj)
         return False
+    db.session.upsert(obj)
+    db.session.commit()
     click.echo(obj.email)
     return True
 
 
 @alias.command(
     "get",
     short_help=const.HELP.ALIAS.GET.SHORT,
     help=const.HELP.ALIAS.GET.LONG,
 )
 @click.argument(
     "id",
-    type=int,
 )
 @click.option(
     "-i",
     "--include",
     help=const.HELP.ALIAS.GET.OPTION.INCLUDE,
 )
 @click.option(
     "-e",
     "--exclude",
     help=const.HELP.ALIAS.GET.OPTION.EXCLUDE,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
-def get(sl, id: int, include: str | None, exclude: str | None) -> None:
+def get(sl, db, id: int, include: str | None, exclude: str | None) -> None:
     """Display a single alias in a tabular format"""
     fields = util.get_display_fields_from_options(
         const.ALIAS_FIELD_ORDER, include, exclude
     )
     if len(fields) == 0:
         return
+    id = util.resolve_id(db, Alias, id)
     success, obj = sl.get_alias(id)
     if not success:
         click.echo(obj)
         return None
+    db.session.upsert(obj)
+    db.session.commit()
     util.display_model_list([obj], fields, use_pager=False)
 
 
 @alias.command(
     "delete",
     short_help=const.HELP.ALIAS.DELETE.SHORT,
     help=const.HELP.ALIAS.DELETE.LONG,
 )
 @click.argument(
     "id",
-    type=int,
 )
 @click.option(
     "-y",
     "--yes",
     "bypass_confirmation",
     is_flag=True,
     flag_value=True,
     default=False,
     help=const.HELP.ALIAS.DELETE.OPTION.YES,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
-def delete(sl, id: int, bypass_confirmation: bool) -> bool:
+def delete(sl, db, id: int, bypass_confirmation: bool) -> bool:
     """Delete an alias"""
+    id = util.resolve_id(db, Alias, id)
     if not bypass_confirmation:
         success, obj = sl.get_alias(id)
         if not success:
             # Clarify the somewhat vague error message for invalid ID
             msg = f"Unknown ID {id}" if "Unknown" in obj else obj
             click.echo(msg)
             return False
@@ -323,26 +323,30 @@
 @click.option(
     "-d",
     "--disabled",
     "query",
     flag_value="disabled",
     help=const.HELP.ALIAS.LIST.OPTION.DISABLED,
 )
+@util.pass_db_access
 @util.pass_simplelogin
-def list(sl, include: str | None, exclude: str | None, query: str | None) -> None:
+def list(sl, db, include: str | None, exclude: str | None, query: str | None) -> None:
     """Display aliases in a tabular format"""
     fields = util.get_display_fields_from_options(
         const.ALIAS_FIELD_ORDER, include, exclude
     )
     if len(fields) == 0:
         return
     aliases = sl.get_all_aliases(query)
     if len(aliases) == 0:
         click.echo("No aliases found.")
         return
+    for alias in aliases:
+        db.session.upsert(alias)
+    db.session.commit()
     util.display_model_list(aliases, fields)
 
 
 @alias.command(
     "random",
     short_help=const.HELP.ALIAS.RANDOM.SHORT,
     help=const.HELP.ALIAS.RANDOM.LONG,
@@ -370,46 +374,51 @@
 @click.option(
     "-n",
     "--note",
     is_flag=False,
     flag_value="_EDIT",
     help=const.HELP.ALIAS.RANDOM.OPTION.NOTE,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
 def random(
     sl,
+    db,
     hostname: str | None,
     mode: str | None,
     note: str | None,
 ) -> bool:
     """Create a new random alias"""
     if note == "_EDIT":
         note = util.edit()
     success, obj = sl.create_random_alias(hostname, mode, note)
     if not success:
         click.echo(obj)
         return False
+    db.session.upsert(obj)
+    db.session.commit()
     click.echo(obj.email)
     return True
 
 
 @alias.command(
     "toggle",
     short_help=const.HELP.ALIAS.TOGGLE.SHORT,
     help=const.HELP.ALIAS.TOGGLE.LONG,
 )
 @click.argument(
     "id",
-    type=int,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
-def toggle(sl, id: int) -> bool:
+def toggle(sl, db, id: int) -> bool:
     """Enable or disable an alias"""
+    id = util.resolve_id(db, Alias, id)
     success, result = sl.toggle_alias(id)
     if not success:
         click.echo(result)
         return False
     click.echo("Enabled" if result else "Disabled")
     return True
 
@@ -417,15 +426,14 @@
 @alias.command(
     "update",
     short_help=const.HELP.ALIAS.UPDATE.SHORT,
     help=const.HELP.ALIAS.UPDATE.LONG,
 )
 @click.argument(
     "id",
-    type=int,
 )
 @click.option(
     "-n",
     "--note",
     is_flag=False,
     flag_value="_EDIT",
     help=const.HELP.ALIAS.UPDATE.OPTION.NOTE,
@@ -451,40 +459,30 @@
 )
 @click.option(
     "-p/-P",
     "--pinned/--no-pinned",
     default=None,
     help=const.HELP.ALIAS.UPDATE.OPTION.PINNED,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
 def update(
     sl,
+    db,
     id: int,
     note: str | None,
     name: str | None,
     mailboxes: tuple[str],
     disable_pgp: bool | None,
     pinned: bool | None,
 ) -> bool:
     """Modify an alias's fields"""
-    # Get the user's mailboxes and check them against the ids/addresses
-    # they provided. This allows us to accept addresses as well as ids,
-    # and to fail early if no valid mailboxes match.
-    mailbox_ids = set()
-    actual_mailboxes = sl.get_mailboxes()
-    for mailbox in actual_mailboxes:
-        id = mailbox.field_as_string("id")
-        email = mailbox.email
-        if id in mailboxes or email in mailboxes:
-            mailbox_ids.add(mailbox.id)
-    if len(mailbox_ids) == 0:
-        click.echo("Invalid mailbox list")
-        return False
-
+    id = util.resolve_id(db, Alias, id)
+    mailbox_ids = {util.resolve_id(db, Mailbox, mb_id) for mb_id in mailboxes}
     if note == "_EDIT":
         note = util.edit()
     success, msg = sl.update_alias(
         alias_id=id,
         note=note,
         name=name,
         mailbox_ids=mailbox_ids,
@@ -512,63 +510,70 @@
 @_contact.command(
     "create",
     short_help=const.HELP.ALIAS.CONTACT.CREATE.SHORT,
     help=const.HELP.ALIAS.CONTACT.CREATE.LONG,
 )
 @click.argument(
     "id",
-    type=int,
 )
 @click.option(
     "-e",
     "--email",
     help=const.HELP.ALIAS.CONTACT.CREATE.OPTION.EMAIL,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
-def contact_create(sl, id: int, email: str) -> bool:
+def contact_create(sl, db, id: int, email: str) -> bool:
     """Create a new contact"""
+    id = util.resolve_id(db, Alias, id)
     success, obj = sl.create_contact(id, email)
     if not success:
         click.echo(obj)
         return False
+    db.session.upsert(obj)
+    db.session.commit()
     click.echo(obj.reverse_alias_address)
     return True
 
 
 @_contact.command(
     "list",
     short_help=const.HELP.ALIAS.CONTACT.LIST.SHORT,
     help=const.HELP.ALIAS.CONTACT.LIST.LONG,
     epilog=const.HELP.ALIAS.CONTACT.LIST.EPILOG,
 )
 @click.argument(
     "id",
-    type=int,
 )
 @click.option(
     "-i",
     "--include",
     help=const.HELP.ALIAS.CONTACT.LIST.OPTION.INCLUDE,
 )
 @click.option(
     "-e",
     "--exclude",
     help=const.HELP.ALIAS.CONTACT.LIST.OPTION.EXCLUDE,
 )
+@util.pass_db_access
 @util.pass_simplelogin
 @util.authenticate
-def contact_list(sl, id: int, include: str | None, exclude: str | None) -> None:
+def contact_list(sl, db, id: int, include: str | None, exclude: str | None) -> None:
     """List contacts in a tabular format"""
     fields = util.get_display_fields_from_options(
         const.CONTACT_FIELD_ORDER, include, exclude
     )
     if len(fields) == 0:
         return
+    id = util.resolve_id(db, Alias, id)
     contacts = sl.get_all_alias_contacts(id)
     if len(contacts) == 0:
         click.echo("No contacts found")
         return
+    for contact in contacts:
+        db.session.upsert(contact)
+    db.session.commit()
     util.display_model_list(contacts, fields)
 
 
 alias.add_command(_contact)
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/commands/mailbox.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/commands/mailbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 - list
 - update
 """
 
 import click
 
 from simplelogincmd.cli import const, util
+from simplelogincmd.database.models import Mailbox
 
 
 @click.group(
     "mailbox", short_help=const.HELP.MAILBOX.SHORT, help=const.HELP.MAILBOX.LONG
 )
 @util.pass_simplelogin
 @util.authenticate
@@ -49,15 +50,17 @@
 
 @mailbox.command(
     "delete",
     short_help=const.HELP.MAILBOX.DELETE.SHORT,
     help=const.HELP.MAILBOX.DELETE.LONG,
     epilog=const.HELP.MAILBOX.DELETE.EPILOG,
 )
-@click.argument("id")
+@click.argument(
+    "id",
+)
 @click.option(
     "-t",
     "--transfer-aliases-to",
     default=-1,
     show_default=True,
     help=const.HELP.MAILBOX.DELETE.OPTION.TRANSFER_ALIASES_TO,
 )
@@ -66,17 +69,19 @@
     "--yes",
     "bypass_confirm",
     is_flag=True,
     flag_value=True,
     default=False,
     help=const.HELP.MAILBOX.DELETE.OPTION.YES,
 )
+@util.pass_db_access
 @util.pass_simplelogin
-def delete(sl, id: int, transfer_aliases_to: int, bypass_confirm: bool):
+def delete(sl, db, id: int, transfer_aliases_to: int, bypass_confirm: bool):
     """Delete a mailbox"""
+    id = util.resolve_id(db, Mailbox, id)
     if transfer_aliases_to == -1 and not bypass_confirm:
         click.confirm(
             "This will delete all of the mailbox's aliases. Are you sure?", abort=True
         )
     success, msg = sl.delete_mailbox(id, transfer_aliases_to)
     if not success:
         click.echo(msg)
@@ -96,37 +101,43 @@
     help=const.HELP.MAILBOX.LIST.OPTION.INCLUDE,
 )
 @click.option(
     "-e",
     "--exclude",
     help=const.HELP.MAILBOX.LIST.OPTION.EXCLUDE,
 )
+@util.pass_db_access
 @util.pass_simplelogin
-def list(sl, include: str, exclude: str) -> None:
+def list(sl, db, include: str, exclude: str) -> None:
     """Display mailboxes in a tabular format"""
     fields = util.get_display_fields_from_options(
         const.MAILBOX_FIELD_ORDER, include, exclude
     )
     if len(fields) == 0:
         return
     mailboxes = sl.get_mailboxes()
     if len(mailboxes) == 0:
         return
     # Sort by `nb_alias` descending, then by `email` ascending.
     sort_keys = lambda mailbox: (mailbox.nb_alias * -1, mailbox.email)
     mailboxes.sort(key=sort_keys)
+    for mailbox in mailboxes:
+        db.session.upsert(mailbox)
+    db.session.commit()
     util.display_model_list(mailboxes, fields)
 
 
 @mailbox.command(
     "update",
     short_help=const.HELP.MAILBOX.UPDATE.SHORT,
     help=const.HELP.MAILBOX.UPDATE.LONG,
 )
-@click.argument("id")
+@click.argument(
+    "id",
+)
 @click.option(
     "-e",
     "--email",
     help=const.HELP.MAILBOX.UPDATE.OPTION.EMAIL,
 )
 @click.option(
     "-d/-D",
@@ -136,20 +147,25 @@
 )
 @click.option(
     "-c/-C",
     "--cancel-email-change/--no-cancel-email-change",
     default=None,
     help=const.HELP.MAILBOX.UPDATE.OPTION.CANCEL_EMAIL_CHANGE,
 )
+@util.pass_db_access
 @util.pass_simplelogin
+@util.authenticate
 def update(
     sl,
+    db,
     id: int,
     email: str | None,
     default: bool | None,
     cancel_email_change: bool | None,
 ) -> bool:
+    """Modify a mailbox's attributes"""
+    id = util.resolve_id(db, Mailbox, id)
     success, msg = sl.update_mailbox(id, email, default, Cancel_email_change)
     if not success:
         click.echo(msg)
         return False
     return True
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/const.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,24 @@
     "verified",
     "default",
     "creation_timestamp",
 )
 
 
 # Help texts common to multiple commands/options
+_HELP_ALIAS_ID = (
+    "`ID` can be the alias's numeric id or, if you have a local data"
+    "base, either its email address or note. In the latter cases, if "
+    "more than one alias matches, you will be prompted to choose one."
+)
+_HELP_MAILBOX_ID = (
+    "`ID` can be the mailbox's numeric id or, if you have a local data"
+    "base, its email address. In the latter case, if more than one "
+    "mailbox matches, you will be prompted to choose one."
+)
 _HELP_OPTION_NOTE = (
     "Attach a note to the item. Setting this switch with"
     "out providing any value will open an editor in which you can enter "
     "the note."
 )
 _HELP_LIST_INCLUDE = (
     "A comma-separated list of fields to include in the "
@@ -130,15 +140,15 @@
         ),
     ),
     ALIAS=NS(
         SHORT=None,
         LONG="CRUD operations on your aliases",
         ACTIVITY=NS(
             SHORT="List alias activity",
-            LONG="List activity for the alias with the given `ID`",
+            LONG=f"List activity for the alias with the given ID. {_HELP_ALIAS_ID}",
             EPILOG=_HELP_LIST_EPILOG.format(
                 field1=ACTIVITY_FIELD_ORDER[0],
                 field2=ACTIVITY_FIELD_ORDER[1],
                 field3=ACTIVITY_FIELD_ORDER[4],
                 valid_fields=", ".join(field for field in ACTIVITY_FIELD_ORDER),
             ),
             OPTION=NS(
@@ -147,15 +157,15 @@
             ),
         ),
         CONTACT=NS(
             SHORT=None,
             LONG="CRUD operations on alias contacts",
             CREATE=NS(
                 SHORT="Create a new contact",
-                LONG="Add a contact to the alias with the given `ID`",
+                LONG=f"Add a contact to the alias with the given ID`. {_HELP_ALIAS_ID}",
                 OPTION=NS(
                     EMAIL="The contact's email address",
                 ),
             ),
             LIST=NS(
                 SHORT="List alias contacts",
                 LONG="List contacts for the alias with the given `ID`",
@@ -193,22 +203,22 @@
                 "number of suffixes offered. A value of 0 refers to "
                 "the first suffix.",
                 YES="Bypass confirmation prompts where possible",
             ),
         ),
         DELETE=NS(
             SHORT="Delete an alias",
-            LONG="Delete the alias with the given `ID`",
+            LONG=f"Delete the alias with the given ID. {_HELP_ALIAS_ID}",
             OPTION=NS(
                 YES="Bypass the confirmation prompt",
             ),
         ),
         GET=NS(
             SHORT="View a specific alias",
-            LONG="View the alias with the given `ID`",
+            LONG=f"View the alias with the given ID. {_HELP_ALIAS_ID}",
             EPILOG=_HELP_LIST_EPILOG.format(
                 field1=ALIAS_FIELD_ORDER[0],
                 field2=ALIAS_FIELD_ORDER[1],
                 field3=ALIAS_FIELD_ORDER[2],
                 valid_fields=", ".join(ALIAS_FIELD_ORDER),
             ),
             OPTION=NS(
@@ -246,31 +256,47 @@
                 WORD="Word mode: Generate an alias based on a "
                 "random series of words",
                 NOTE=_HELP_OPTION_NOTE,
             ),
         ),
         TOGGLE=NS(
             SHORT="Enable or disable an alias",
-            LONG="Enable or disable the aliase with the given `id`, ",
+            LONG=f"Enable or disable the aliase with the given ID. {_HELP_ALIAS_ID}",
         ),
         UPDATE=NS(
             SHORT="Modify an existing alias",
-            LONG="Modify the alias with the given `ID`",
+            LONG=f"Modify the alias with the given ID. {_HELP_ALIAS_ID}",
             OPTION=NS(
                 NOTE=_HELP_OPTION_NOTE,
                 NAME="The name that will appear as the user of the alias",
                 MAILBOXES="The ID(s) or email address(es) of the mail"
                 "box(es) to which the alias belongs. use this "
                 "multiple times to enter multiple mailboxes. At least "
                 "one is required.",
                 DISABLE_PGP="Whether to disable PGP",
                 PINNED="Whether to pin the alias",
             ),
         ),
     ),
+    DATABASE=NS(
+        SHORT=None,
+        LONG="Manage the local database",
+        DELETE=NS(
+            SHORT=None,
+            LONG="Delete the db",
+        ),
+        SYNC=NS(
+            SHORT="Synchronize the DB",
+            LONG="Synchronize the local database with that of SimpleLogin",
+            EPILOG="Note that this command will wipe any data "
+            "currently stored in your local database. This should "
+            "not matter to most people, so no confirmation is "
+            "required.",
+        ),
+    ),
     MAILBOX=NS(
         SHORT=None,
         LONG="CRUD operations on your mailboxes",
         CREATE=NS(
             SHORT=None,
             LONG="Create a new mailbox",
             EPILOG="If successful, the mailbox will receive a "
@@ -278,16 +304,16 @@
             "in this email in order to verify the mailbox.",
             OPTION=NS(
                 EMAIL="The email address of the new mailbox",
             ),
         ),
         DELETE=NS(
             SHORT="Delete an existing mailbox",
-            LONG="Delete the mailbox with the given `ID`, optionally "
-            "transferring all its aliases to another mailbox",
+            LONG="Delete the mailbox with the given ID, optionally "
+            f"transferring all its aliases to another mailbox. {_HELP_MAILBOX_ID}",
             EPILOG="Note that SimpleLogin does not currently support " "this command.",
             OPTION=NS(
                 TRANSFER_ALIASES_TO="The ID of the mailbox which is "
                 "to take over the deleted mailbox's aliases. A value "
                 "-1 indicates that all the aliases belonging to the "
                 "deleted mailbox are also to be deleted. If this "
                 "is the case, a confirmation prompt will appear unless "
@@ -309,15 +335,15 @@
             OPTION=NS(
                 INCLUDE=_HELP_LIST_INCLUDE,
                 EXCLUDE=_HELP_LIST_EXCLUDE,
             ),
         ),
         UPDATE=NS(
             SHORT="Update a mailbox's attributes",
-            LONG="Modify the mailbox with the given `ID`",
+            LONG=f"Modify the mailbox with the given ID. {_HELP_MAILBOX_ID}",
             OPTION=NS(
                 EMAIL="A new email address to assign to this mailbox",
                 DEFAULT="Whether to make this the default mailbox",
                 CANCEL_EMAIL_CHANGE=None,  # What does this do?
             ),
         ),
     ),
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/exceptions.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/main.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 from simplelogincmd.cli import commands, const, util
 
 
 @click.group(
     context_settings=const.CONTEXT_SETTINGS,
 )
 @click.version_option()
+@util.pass_db_access
 @util.pass_simplelogin
-def cli(sl):
+def cli(sl, db):
     """
     \f
     Application entrypoint
     """
+    config.ensure_directory()
+    db.initialize()
     # Silently log in if an API key is saved. If no API key is found,
     # don't prompt for credentials now because user may not be invoking
     # a command that requires authentication anyway. Later prompting
     # can be done via the `util.authenticate` command decorator.
     cfg = config.load()
     api_key = cfg["API"].get("api_key", "")
     if api_key != "":
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/cli/util.py` & `simplelogincmd-0.2.0/simplelogincmd/cli/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 CLI application utilities
 """
 
 from functools import wraps
+from typing import Any, Type
 
 import click
 
 from simplelogincmd.cli.exceptions import NotLoggedInError
+from simplelogincmd.database import DatabaseAccessLayer
+from simplelogincmd.database.models import Object
 from simplelogincmd.rest import SimpleLogin
 from simplelogincmd.rest.exceptions import UnauthenticatedError
-from simplelogincmd.rest.models import Object
 
 
+pass_db_access = click.make_pass_decorator(DatabaseAccessLayer, ensure=True)
 pass_simplelogin = click.make_pass_decorator(SimpleLogin, ensure=True)
 
 
 def authenticate(f):
     """
     Prompt the user to login if not already authenticated
 
@@ -59,28 +62,28 @@
     :rtype: Generator
     """
     if len(models) == 0:
         return
     header = "|".join(fields)
     yield f"{header}\n"
     for model in models:
-        properties = [model.field_as_string(field) for field in fields]
+        properties = [model.get_string(field) for field in fields]
         entry = "|".join(properties)
         yield f"{entry}\n"
 
 
 def display_model_list(
     models: list[Object],
     fields: list[str],
     use_pager: bool = True,
 ) -> None:
     """
     Print a simple table detailing each item to stdout
 
-    :param models: Series of :class:`~simplelogincmd.rest.models.Object` to
+    :param models: Series of :class:`~simplelogincmd.database.models.Object` to
         be included in the output
     :type models: list[Object]
     :param fields: The field names to display for each item, in left-
         to-right order
     :type fields: list[str]
     :param use_pager: Whether to display the table in a pager, for easier
         viewing of long lists, defaults to True
@@ -189,7 +192,41 @@
     int_range = click.IntRange(low, high)
     click.echo("")
     for index, option in enumerate(options):
         click.echo(f"{index + 1} - {option}")
     text = f"\n{text} ({low}-{high})"
     choice = click.prompt(text, type=int_range, show_choices=True)
     return choice - 1
+
+
+def resolve_id(db: DatabaseAccessLayer, model_cls: Type, id: Any) -> int | Any:
+    """
+    Search for a single db object id given an identifier
+
+    Call the model classes :meth:`~Object.resolve_identifier` method to
+    locate db objects based on the given identifier, which can be any
+    value. If multiple results match, ask the user to choose one and
+    return the id of the selected object. If one result matches, return
+    its id directly. If no matches were found, return the id as it was
+    provided.
+
+    :param db: The access layer instance to use for the lookup
+    :type db: :class:`~simplelogincmd.database.DatabaseAccessLayer`
+    :param model_cls: The type of db object for which to search
+    :type model_cls: Type, subclass of
+        :class:`~simplelogincmd.database.models.Object`
+    :param id: The id to look up
+    :type id: Any, usually int or str, as defined by the model class's
+        :meth:`~simplelogincmd.database.models.Object.identifier_query`
+
+    :return: The numeric id of the matched object, or the given id if
+        none matched
+    :rtype: int | type(id)
+    """
+    results = model_cls.resolve_identifier(db.session, id)
+    count = len(results)
+    if count == 0:
+        return id
+    if count == 1:
+        return results[0].id
+    choice = prompt_choice(f"Select {model_cls.__name__}", results)
+    return results[choice].id
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/config.py` & `simplelogincmd-0.2.0/simplelogincmd/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,37 @@
 
     :return: Application's default configuration
     :rtype: dict
     """
     return const.CONFIG_DEFAULT
 
 
+def ensure_directory(path: Path | None = None) -> bool:
+    """
+    Create a config directory if it does not already exist
+
+    :param path: The directory to check, defaults to the application's
+        default config directory
+    :type path: :class:`pathlib.Path`
+
+    :return: Whether the directory now exists
+    :rtype: bool
+    """
+    path = path or const.DIR_APPDATA
+    if path.exists():
+        return True
+    try:
+        path.mkdir(parents=True, exist_ok=True)
+    except OSError:
+        # TODO: Add logging / other notification mechanisms.
+        return False
+    path.chmod(0o755)  # drwxr-xr-x
+    return True
+
+
 def load(path: Path | None = None) -> ConfigParser:
     """
     Read configuration from a config file
 
     The config is first populated with default configuration as returned
     by :func:`default`, and then the given path (or the application's
     default config file, if none is given) is read in. Thus, no
@@ -61,20 +84,17 @@
     :type path: :class:`pathlib.Path`, optional
 
     :return: Whether the configuration saved successfully
     :rtype: bool
     """
     path = path or const.FILE_CONFIG
     directory = path.parent
-    try:
-        directory.mkdir(parents=True, exist_ok=True)
-    except OSError:
-        # TODO: Add logging / other notification mechanisms.
+    if not ensure_directory(directory):
         return False
     try:
         with path.open("w", encoding="utf-8") as file:
             config.write(file)
     except OSError:
         # TODO: Add logging / other notification mechanisms.
         return False
-    path.chmod(400)
+    path.chmod(0o600)  # -rw-------
     return True
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/rest/client.py` & `simplelogincmd-0.2.0/simplelogincmd/rest/client.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.1.0/simplelogincmd/rest/const.py` & `simplelogincmd-0.2.0/simplelogincmd/rest/const.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.1.0/simplelogincmd/rest/simplelogin.py` & `simplelogincmd-0.2.0/simplelogincmd/rest/simplelogin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Manage requests and responses to the SimpleLogin API
 """
 
 from simplelogincmd.rest import const, util
 from simplelogincmd.rest.client import Client
-from simplelogincmd.rest.models import (
+from simplelogincmd.database.models import (
     Activity,
     Alias,
     Contact,
     Mailbox,
 )
```

### Comparing `simplelogincmd-0.1.0/simplelogincmd/rest/util.py` & `simplelogincmd-0.2.0/simplelogincmd/rest/util.py`

 * *Files identical despite different names*

