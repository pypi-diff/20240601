# Comparing `tmp/dyno_viewer-0.21.4.tar.gz` & `tmp/dyno_viewer-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyno_viewer-0.21.4.tar", max compression
+gzip compressed data, was "dyno_viewer-0.22.0.tar", max compression
```

## Comparing `dyno_viewer-0.21.4.tar` & `dyno_viewer-0.22.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/LICENSE
--rw-r--r--   0        0        0     2390 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/README.md
--rw-r--r--   0        0        0       58 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/__main__.py
--rw-r--r--   0        0        0    10418 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/app.py
--rw-r--r--   0        0        0      181 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/app_types.py
--rw-r--r--   0        0        0     7792 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/aws/ddb.py
--rw-r--r--   0        0        0      211 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/aws/session.py
--rw-r--r--   0        0        0      558 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/css/query.tcss
--rw-r--r--   0        0        0       56 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/css/table.tcss
--rw-r--r--   0        0        0      390 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/help/help-doc.md
--rw-r--r--   0        0        0     2233 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/query/filter_query.py
--rw-r--r--   0        0        0     2440 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/query/key_filter.py
--rw-r--r--   0        0        0     2057 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/query/sort_key_filter.py
--rw-r--r--   0        0        0      149 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/__init__.py
--rw-r--r--   0        0        0      794 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/error.py
--rw-r--r--   0        0        0      576 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/help.py
--rw-r--r--   0        0        0      912 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/profile_select.py
--rw-r--r--   0        0        0     6497 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/query.py
--rw-r--r--   0        0        0      857 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/region_select.py
--rw-r--r--   0        0        0     4341 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/table_select.py
--rw-r--r--   0        0        0     2177 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/table.py
--rw-r--r--   0        0        0       20 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/util/__init__.py
--rw-r--r--   0        0        0      565 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/util/util.py
--rw-r--r--   0        0        0     1085 2024-05-13 00:58:37.117987 dyno_viewer-0.21.4/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 dyno_viewer-0.21.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-06-01 01:48:13.172167 dyno_viewer-0.22.0/LICENSE
+-rw-r--r--   0        0        0     2390 2024-06-01 01:48:13.172167 dyno_viewer-0.22.0/README.md
+-rw-r--r--   0        0        0       58 2024-06-01 01:48:13.172167 dyno_viewer-0.22.0/dyno_viewer/__main__.py
+-rw-r--r--   0        0        0     8401 2024-06-01 01:48:13.172167 dyno_viewer-0.22.0/dyno_viewer/app.py
+-rw-r--r--   0        0        0      181 2024-06-01 01:48:13.172167 dyno_viewer-0.22.0/dyno_viewer/app_types.py
+-rw-r--r--   0        0        0     7687 2024-06-01 01:48:13.172167 dyno_viewer-0.22.0/dyno_viewer/aws/ddb.py
+-rw-r--r--   0        0        0      192 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/aws/session.py
+-rw-r--r--   0        0        0      558 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/css/query.tcss
+-rw-r--r--   0        0        0       56 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/css/table.tcss
+-rw-r--r--   0        0        0      390 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/help/help-doc.md
+-rw-r--r--   0        0        0     2203 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/query/filter_query.py
+-rw-r--r--   0        0        0     2437 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/query/key_filter.py
+-rw-r--r--   0        0        0     2027 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/query/sort_key_filter.py
+-rw-r--r--   0        0        0      149 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/screens/__init__.py
+-rw-r--r--   0        0        0      670 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/screens/error.py
+-rw-r--r--   0        0        0      524 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/screens/help.py
+-rw-r--r--   0        0        0      871 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/screens/profile_select.py
+-rw-r--r--   0        0        0     6405 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/screens/query.py
+-rw-r--r--   0        0        0      801 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/screens/region_select.py
+-rw-r--r--   0        0        0     4291 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/screens/table_select.py
+-rw-r--r--   0        0        0     4301 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/components/table.py
+-rw-r--r--   0        0        0       20 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/util/__init__.py
+-rw-r--r--   0        0        0      535 2024-06-01 01:48:13.176167 dyno_viewer-0.22.0/dyno_viewer/util/util.py
+-rw-r--r--   0        0        0     2653 2024-06-01 01:48:33.568087 dyno_viewer-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 dyno_viewer-0.22.0/PKG-INFO
```

### Comparing `dyno_viewer-0.21.4/LICENSE` & `dyno_viewer-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.4/README.md` & `dyno_viewer-0.22.0/README.md`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.4/dyno_viewer/app.py` & `dyno_viewer-0.22.0/dyno_viewer/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,33 @@
+from textual import log, on, work
 from textual.app import App, ComposeResult
-from textual.widgets import (
-    Footer,
-)
+from textual.message import Message
 from textual.reactive import reactive
-from dyno_viewer.aws.session import get_available_profiles
+from textual.widgets import Footer
+from textual.worker import get_current_worker
+
+from dyno_viewer.app_types import TableInfo
 from dyno_viewer.aws.ddb import (
     get_ddb_client,
     query_items,
     scan_items,
     table_client_exist,
 )
+from dyno_viewer.aws.session import get_available_profiles
 from dyno_viewer.components.screens import (
+    HelpMenu,
     ProfileSelectScreen,
+    QueryScreen,
     RegionSelectScreen,
     TableSelectScreen,
-    QueryScreen,
-    HelpMenu,
 )
-from dyno_viewer.components.table import DataDynTable
-from textual.worker import get_current_worker
-from textual.binding import Binding
-from textual import work, log, on
-import pyclip
-from itertools import cycle
-from dyno_viewer.app_types import TableInfo
-from textual.message import Message
-from dyno_viewer.util import output_to_csv_str
-from dyno_viewer.util.util import format_output
-
-cursors = cycle(["column", "row", "cell"])
+from dyno_viewer.components.table import DataTableManager
 
 
-class UpdateDynDataTable(Message):
+class QueryResult(Message):
     def __init__(self, data, next_token, update_existing_data=False) -> None:
         self.data = data
         self.next_token = next_token
         self.update_existing_data = update_existing_data
         super().__init__()
 
 
@@ -49,16 +41,14 @@
     BINDINGS = [
         ("x", "exit", "Exit"),
         ("p", "push_screen('profile')", "Profile"),
         ("t", "push_screen('tableSelect')", "Table"),
         ("r", "push_screen('regionSelect')", "Region"),
         ("q", "push_screen_query", "Query"),
         ("?", "push_screen('help')", "help"),
-        Binding("ctrl+c", "copy_table_data", "Copy", show=False),
-        Binding("ctrl+r", "change_cursor_type", "Change Cursor type", show=False),
     ]
     SCREENS = {
         "tableSelect": TableSelectScreen(),
         "regionSelect": RegionSelectScreen(),
         "profile": ProfileSelectScreen(),
         "query": QueryScreen(),
         "help": HelpMenu(),
@@ -79,44 +69,45 @@
     # set always_update=True because otherwise textual thinks that the client hasn't changed when it actually has :(
     table_client = reactive(None, always_update=True)
 
     dyn_client = reactive(get_ddb_client())
 
     table_info = reactive(None)
 
+    data = reactive([], always_update=True)
+
     def compose(self) -> ComposeResult:
-        yield DataDynTable()
+        yield DataTableManager().data_bind(DynCli.data, DynCli.table_info)
         yield Footer()
 
     def update_table_client(self):
         if self.table_name != "":
             log.info(f"updating table client with profile {self.aws_profile}")
             new_table_client = table_client_exist(
                 self.table_name, self.aws_region, self.aws_profile
             )
             if new_table_client:
                 self.table_client = new_table_client
-            else:
-                table = self.query_one(DataDynTable)
-                table.clear()
+
+            self.data = []
 
     def set_pagination_token(self, next_token: str | None) -> None:
         if next_token:
             self.dyn_query_params["ExclusiveStartKey"] = next_token
         else:
             self.dyn_query_params.pop("ExclusiveStartKey", None)
 
     # worker methods
 
     @work(exclusive=True, group="update_dyn_table_info", thread=True)
     def get_dyn_table_info(self) -> None:
         worker = get_current_worker()
         if not worker.is_cancelled:
             # temp disable logging doesn't work
-            self.log(f"updating table info")
+            self.log("updating table info")
             self.log("key schema=", self.table_client.key_schema)
             self.log("gsi schema=", self.table_client.global_secondary_indexes)
             main_keys = {
                 ("primaryKey" if key["KeyType"] == "HASH" else "sortKey"): key[
                     "AttributeName"
                 ]
                 for key in self.table_client.key_schema
@@ -152,32 +143,25 @@
                 else scan_items(
                     self.table_client,
                     paginate=False,
                     Limit=50,
                     **dyn_query_params,
                 )
             )
-
-            self.post_message(UpdateDynDataTable(result, next_token, update_existing))
+            self.post_message(QueryResult(result, next_token, update_existing))
 
     # on methods
 
-    def on_mount(self):
-        table = self.query_one(DataDynTable)
-        table.focus()
-
-    @on(DataDynTable.CellHighlighted)
-    async def paginate_dyn_data(
-        self, highlighted: DataDynTable.CellHighlighted
-    ) -> None:
-        if highlighted.coordinate.row == highlighted.data_table.row_count - 1:
-            if "ExclusiveStartKey" in self.dyn_query_params:
-                log.info("adding more items")
-
-                self.run_table_query(self.dyn_query_params, update_existing=True)
+    @on(DataTableManager.PaginateRequest)
+    async def paginate_table(self, _) -> None:
+        table = self.query_one(DataTableManager)
+        if "ExclusiveStartKey" in self.dyn_query_params:
+            self.run_table_query(self.dyn_query_params, update_existing=True)
+        else:
+            table.loading = False
 
     @on(UpdateDynTableInfo)
     async def update_table_info(self, update: UpdateDynTableInfo) -> None:
         self.table_info = update.table_info
 
     async def on_region_select_screen_region_selected(
         self, selected_region: RegionSelectScreen.RegionSelected
@@ -209,81 +193,50 @@
             {"KeyConditionExpression": run_query.key_cond_exp}
             if run_query.key_cond_exp
             else {}
         )
 
         if run_query.filter_cond_exp:
             params["FilterExpression"] = run_query.filter_cond_exp
-        
+
         if run_query.index != "table":
             params["IndexName"] = run_query.index
-        
+
         self.dyn_query_params = params
         self.run_table_query(params)
 
-    async def on_update_dyn_data_table(self, update_data: UpdateDynDataTable) -> None:
-        table = self.query_one(DataDynTable)
-        if update_data.update_existing_data:
-            table.add_dyn_data_existing(update_data.data)
-            self.set_pagination_token(update_data.next_token)
-        else:
-            table.add_dyn_data(self.table_info, update_data.data)
-            self.set_pagination_token(update_data.next_token)
+    @on(QueryResult)
+    async def update_table(self, update_data: QueryResult) -> None:
+        table = self.query_one(DataTableManager)
+        self.data = self.data + [update_data.data]
+        self.set_pagination_token(update_data.next_token)
+        table.loading = False
 
     # action methods
 
     async def action_exit(self) -> None:
-        table = self.query_one(DataDynTable)
-        # ensure we don't have any dirty data for next time app runs
-        table.clear()
         self.app.exit()
 
     async def action_push_screen_query(self) -> None:
         if self.table_client:
             self.push_screen("query")
         else:
             self.notify("No table selected")
 
-    async def action_copy_table_data(self) -> None:
-        query_table = self.query(DataDynTable)
-        if query_table:
-            table = query_table[0]
-            if table.row_count > 0:
-                if table.cursor_type == "cell":
-                    cell = table.get_cell_at(table.cursor_coordinate)
-                    if cell is not None:
-                        pyclip.copy(format_output(cell))
-                elif table.cursor_type == "row":
-                    row = table.get_row_at(table.cursor_row)
-                    if row:
-                        pyclip.copy(output_to_csv_str(row))
-                elif table.cursor_type == "column":
-                    col = table.get_column_at(table.cursor_column)
-                    if col:
-                        pyclip.copy(output_to_csv_str(col))
-
-    async def action_change_cursor_type(self) -> None:
-        query_table = self.query(DataDynTable)
-        if query_table:
-            table = query_table[0]
-            next_cursor = next(cursors)
-            self.notify(f"selection mode: {next_cursor}", timeout=1)
-            table.cursor_type = next_cursor
-
     # watcher methods
 
     async def watch_table_client(self, new_table_client) -> None:
         """update DynTable with new table data"""
         if new_table_client:
             log.info("table client changed and table found, Update table data")
             self.get_dyn_table_info()
             self.run_table_query(self.dyn_query_params)
         else:
             log.info("table client changed and table not found, Clear table data")
-            self.query_one(DataDynTable).clear()
+            self.data = []
 
     def watch_dyn_client(self, new_dyn_client):
         with self.SCREENS["tableSelect"].prevent(TableSelectScreen.TableName):
             self.SCREENS["tableSelect"].dyn_client = new_dyn_client
 
     def watch_table_info(self, new_table_info: TableInfo) -> None:
         with self.SCREENS["query"].prevent(QueryScreen.RunQuery):
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/aws/ddb.py` & `dyno_viewer-0.22.0/dyno_viewer/aws/ddb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 import logging
+import re
+from decimal import Decimal
 
+import boto3
 import simplejson as json
-from decimal import Decimal as D
-
 from boto3.dynamodb.conditions import Attr, Key
-from dynamodb_json import json_util as dyn_json
 from boto3.session import Session
-import boto3
-from botocore.exceptions import ClientError
-from decimal import Decimal
-import re
-from textual import log
-
+from dynamodb_json import json_util as dyn_json
 
 LOG_LEVEL = logging.INFO
 
 
 def get_logger():
     import logging
 
@@ -29,19 +24,20 @@
 
 
 def table_client_exist(table_name, region_name, profile_name):
     try:
         client = get_table(table_name, region_name, profile_name)
         if client.table_status in ("CREATING", "UPDATING", "ACTIVE"):
             return client
+        return None
     except Exception as error:
         if error.response["Error"]["Code"] in [
             "ResourceNotFoundException",
         ]:
-            return
+            return None
         raise error
 
 
 def get_table(table_name, region_name, profile_name):
     return get_dyn_resource(region_name, profile_name).Table(table_name)
 
 
@@ -94,41 +90,41 @@
     :return:
     """
     resp = get_table_client(table).get_item(
         Key=item_key, ConsistentRead=consistent_read
     )
     if not return_none:
         return resp["Item"]
-    else:
-        return resp.get("Item")
 
+    return resp.get("Item")
 
-def get_items(table_name, item_keys, return_none=False, **kwargs):
+
+def get_items(table_name, item_keys, **kwargs):
     """
     Use the BatchGetItem API to bulk read items.
     """
 
     def make_key(key):
         return {"pk": {"S": key["pk"]}, "sk": {"S": key["sk"]}}
 
     items = []
     keys = [make_key(d) for d in item_keys]
-    logger.info(f"Batch reading {len(keys)} item keys.")
+    logger.info("Batch reading %s item keys.", len(keys))
     batch_size = 100  # the max ddb supports.
     batches = [keys[n : n + batch_size] for n in range(0, len(keys), batch_size)]
 
     client = get_ddb_client()
     request = {"RequestItems": {table_name: {"Keys": None, **kwargs}}}
 
     for n, batch in enumerate(batches):
         request["RequestItems"][table_name]["Keys"] = batch
         res = client.batch_get_item(**request)
-        for k, v in res["Responses"].items():
+        for v in res["Responses"].values():
             items.extend(v)
-        logger.info(f"{n}/{len(batches)}")
+        logger.info("%s/%s", n, len(batches))
 
     return items
 
 
 def query_items(
     table,
     paginate=True,
@@ -153,15 +149,15 @@
     items = query_items(table, **query_kwargs)
     items_count = len(items)
 
     if items_count == 0 and return_none:
         return None
 
     if items_count == 0:
-        raise Exception(f"Item not found")
+        raise ValueError("Item not found")
 
     return items[0]
 
 
 def check_attr_exists(table, pk, attr, sk=None):
     """
     Check an attribute exists given a pk/sk.
@@ -189,42 +185,44 @@
             )
             items.extend(resp["Items"])
         return items
 
     return items, resp.get("LastEvaluatedKey")
 
 
-def covert_comparator_exp(cond, attr_name, value, is_key=True) -> Key | Attr:
+def covert_comparator_exp(cond, attr_name, value, is_key=True) -> Key | Attr | None:
     attr_class = Key if is_key else Attr
     if cond == "==":
         return attr_class(attr_name).eq(value)
     if cond == "!=":
         return attr_class(attr_name).ne(value)
-    elif cond == ">=":
+    if cond == ">=":
         return attr_class(attr_name).gte(value)
-    elif cond == ">":
+    if cond == ">":
         return attr_class(attr_name).gt(value)
-    elif cond == "<=":
+    if cond == "<=":
         return attr_class(attr_name).lte(value)
-    elif cond == "<":
+    if cond == "<":
         return attr_class(attr_name).lt(value)
 
+    return None
+
 
 def convert_filter_exp_key_cond(cond, attr_name, value) -> Key:
     comparator = covert_comparator_exp(cond, attr_name, value)
 
     if comparator:
         return comparator
 
     if cond == "between":
         return Key(attr_name).between(value[0], value[1])
     if cond == "begins_with":
         return Key(attr_name).begins_with(value)
 
-    raise Exception("passed incorrect condition for key filter expression")
+    raise ValueError("passed incorrect condition for key filter expression")
 
 
 def convert_filter_exp_attr_cond(cond, attr_name, value=None) -> Attr:
     comparator = covert_comparator_exp(cond, attr_name, value, is_key=False)
 
     if comparator:
         return comparator
@@ -242,32 +240,32 @@
     if cond == "attribute_type":
         return Attr(attr_name).attribute_type(value)
     if cond == "contains":
         return Attr(attr_name).contains(value)
     if cond == "size":
         return Attr(attr_name).size()
 
-    raise Exception("passed incorrect condition for key filter expression")
+    raise ValueError("passed incorrect condition for key filter expression")
 
 
 def convert_filter_exp_value(value: str, type: str):
     if type == "number":
         return Decimal(value)
-    elif type == "list":
+    if type == "list":
         return list(value)
-    elif type == "map":
+    if type == "map":
         return json.loads(value)
-    elif type == "boolean":
+    if type == "boolean":
         return bool(value)
-    elif type == "set":
+    if type == "set":
         value_formatted = re.sub(r"[\(\)]", "", value)
         return set(value_formatted.split(","))
-    else:
-        return value
+
+    return value
 
 
 def float_to_decimal(payload):
-    return json.loads(json.dumps(payload), parse_float=D)
+    return json.loads(json.dumps(payload), parse_float=Decimal)
 
 
 def serialise_dynamodb_json(json_obj):
     return json.loads(dyn_json.dumps(json_obj))
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/css/query.tcss` & `dyno_viewer-0.22.0/dyno_viewer/components/css/query.tcss`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/query/filter_query.py` & `dyno_viewer-0.22.0/dyno_viewer/components/query/filter_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from textual.app import ComposeResult
 from textual.widget import Widget
-from textual.widgets import Input, Button, RadioSet, Select, Label
+from textual.widgets import Button, Input, Label, RadioSet, Select
 
 
 class FilterQuery(Widget):
     def compose(self) -> ComposeResult:
         yield Input(placeholder="attr", id="attr")
         yield Label("Type")
         yield Select(
@@ -59,15 +59,15 @@
     def on_mount(self) -> None:
         for radio_set in self.query(RadioSet):
             radio_set.display = False
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if str(event.button.label) == "type":
             radio_set = self.query_one("#attrType")
-            radio_set.display = False if radio_set.display else True
+            radio_set.display = not radio_set.display
             self.scroll_visible()
         if str(event.button.label) == "condition":
             radio_set = self.query_one("#condition")
-            radio_set.display = False if radio_set.display else True
+            radio_set.display = not radio_set.display
             self.scroll_visible()
         if event.button.id == "removeFilter":
             self.remove()
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/query/key_filter.py` & `dyno_viewer-0.22.0/dyno_viewer/components/query/key_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from textual import on
 from textual.app import ComposeResult
 from textual.reactive import reactive
 from textual.widget import Widget
-from textual.widgets import  OptionList, Input
+from textual.widgets import Input, OptionList
 
 from dyno_viewer.components.query.sort_key_filter import SortKeyFilter
 
 
 class KeyFilter(Widget):
     index_mode = reactive("table")
 
@@ -36,20 +36,18 @@
 
             self.log("new_primary_key=", new_primary_key)
             self.log("new_sort_key=", new_sort_key)
 
             self.query_one("#partitionKey").placeholder = new_primary_key
             self.query_one("#sortKeyFilter").attr_name = new_sort_key
 
-
         else:
             self.query_one("#partitionKey").placeholder = self.partition_key_attr_name
             self.query_one("#sortKeyFilter").attr_name = self.sort_key_attr_name
 
-
     # watch methods
 
     def watch_gsi_indexes(self, new_gsi_indexes) -> None:
         if new_gsi_indexes:
             option_list: OptionList = self.query_one("#queryIndex")
             option_list.clear_options()
             for option in ["table", *list(new_gsi_indexes.keys())]:
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/query/sort_key_filter.py` & `dyno_viewer-0.22.0/dyno_viewer/components/query/sort_key_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from textual.app import ComposeResult
 from textual.reactive import reactive
 from textual.widget import Widget
-from textual.widgets import Label, Button, RadioSet, Input, Select
+from textual.widgets import Button, Input, Label, RadioSet, Select
 
 
 class SortKeyFilter(Widget):
     attr_name = reactive("", layout=True)
 
     def compose(self) -> ComposeResult:
         yield Label(self.attr_name, id="attr")
@@ -52,19 +52,19 @@
     def on_mount(self) -> None:
         for radio_set in self.query(RadioSet):
             radio_set.display = False
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if str(event.button.label) == "type":
             radio_set = self.query_one("#attrType")
-            radio_set.display = False if radio_set.display else True
+            radio_set.display = not radio_set.display
             self.scroll_visible()
         if str(event.button.label) == "condition":
             radio_set = self.query_one("#condition")
-            radio_set.display = False if radio_set.display else True
+            radio_set.display = not radio_set.display
             self.scroll_visible()
 
     # watch methods
 
     def watch_attr_name(self, new_attr_name):
         if new_attr_name:
             self.query_one("#attr").update(new_attr_name)
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/screens/error.py` & `dyno_viewer-0.22.0/dyno_viewer/components/screens/error.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from textual.app import ComposeResult
-from textual.widgets import (
-    Label,
-)
-from textual.screen import Screen
 from textual.containers import Vertical
-from textual.widgets import Button
-from textual import log
-from botocore.exceptions import ClientError
+from textual.screen import Screen
+from textual.widgets import Button, Label
 
 
 class ErrorScreen(Screen):
     BINDINGS = [("escape", "app.pop_screen", "Pop screen")]
 
     def __init__(
         self,
@@ -21,9 +16,9 @@
     ) -> None:
         self.error_msg = error_msg
         super().__init__(name, id, classes)
 
     def compose(self) -> ComposeResult:
         yield Vertical(Label(self.error_msg), Button("OK"))
 
-    def on_button_pressed(self, event: Button.Pressed) -> None:
+    def on_button_pressed(self, _) -> None:
         self.app.pop_screen()
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/screens/profile_select.py` & `dyno_viewer-0.22.0/dyno_viewer/components/screens/profile_select.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from textual.app import ComposeResult
-from textual.widgets import (
-    ListItem,
-    ListView,
-    Label,
-)
-from textual.screen import Screen
 from textual.message import Message
-from textual import log
+from textual.screen import Screen
+from textual.widgets import Label, ListItem, ListView
 
 from dyno_viewer.aws.session import get_available_profiles
 
 
 class ProfileSelectScreen(Screen):
     BINDINGS = [("escape", "app.pop_screen", "Pop screen")]
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/screens/query.py` & `dyno_viewer-0.22.0/dyno_viewer/components/screens/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+from boto3.dynamodb.conditions import Attr, Key
+from textual import log, on
 from textual.app import ComposeResult
-from textual.css.query import NoMatches
-from textual.widgets import ListItem, ListView, Button, Input, Switch, Label, RadioSet
-from textual.widget import Widget
-from textual.widgets import Footer
 from textual.containers import Container, Horizontal
-from textual.screen import Screen
+from textual.css.query import NoMatches
 from textual.message import Message
 from textual.reactive import reactive
-from textual import log, on
-from dyno_viewer.components.query.filter_query import FilterQuery
-from dyno_viewer.components.query.key_filter import KeyFilter
-from boto3.dynamodb.conditions import Key, Attr
+from textual.screen import Screen
+from textual.widgets import Button, Footer, Label, Switch
+
+from dyno_viewer.app_types import TableInfo
 from dyno_viewer.aws.ddb import (
-    convert_filter_exp_key_cond,
     convert_filter_exp_attr_cond,
+    convert_filter_exp_key_cond,
     convert_filter_exp_value,
 )
-from dyno_viewer.app_types import TableInfo
+from dyno_viewer.components.query.filter_query import FilterQuery
+from dyno_viewer.components.query.key_filter import KeyFilter
 
 
 class QueryScreen(Screen):
     BINDINGS = [
         ("escape", "app.pop_screen", "Pop screen"),
         (("r", "run_query", "Run Query")),
     ]
@@ -83,15 +82,15 @@
         return sort_key_name, sort_key_value, cond
 
     def get_key_query(self) -> Key | None:
         log("generating key expression from input data")
         primary_key_name, primary_key_value = self.get_primary_key()
 
         if not primary_key_value:
-            return
+            return None
 
         sort_key_name, sort_key_value, cond = self.get_sort_key_()
 
         if sort_key_value:
             return Key(primary_key_name).eq(
                 primary_key_value
             ) & convert_filter_exp_key_cond(cond, sort_key_name, sort_key_value)
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/screens/region_select.py` & `dyno_viewer-0.22.0/dyno_viewer/components/screens/region_select.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 from textual.app import ComposeResult
-from textual.widgets import (
-    ListItem,
-    ListView,
-    Label,
-)
-from textual.screen import Screen
 from textual.message import Message
+from textual.screen import Screen
+from textual.widgets import Label, ListItem, ListView
+
 from dyno_viewer.aws.session import get_all_regions
-from textual import log
 
 
 class RegionSelectScreen(Screen):
     BINDINGS = [("escape", "app.pop_screen", "Pop screen")]
 
     class RegionSelected(Message):
-        """"""
-
         def __init__(self, region: str) -> None:
             self.region = region
             super().__init__()
 
     def compose(self) -> ComposeResult:
         yield ListView(
             *[ListItem(Label(region), id=region) for region in get_all_regions()],
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/components/screens/table_select.py` & `dyno_viewer-0.22.0/dyno_viewer/components/screens/table_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from textual import log, on, work
+from textual import on, work
 from textual.app import ComposeResult
-from textual.containers import Vertical
-from textual.events import Key, ScreenResume
+from textual.events import ScreenResume
 from textual.message import Message
 from textual.reactive import reactive
 from textual.screen import Screen
 from textual.widgets import Input, OptionList
 from textual.worker import get_current_worker
 
 from dyno_viewer.aws.ddb import list_all_tables
```

### Comparing `dyno_viewer-0.21.4/dyno_viewer/util/util.py` & `dyno_viewer-0.22.0/dyno_viewer/util/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from decimal import Decimal
-import io
 import csv
+import io
+from decimal import Decimal
+
 
 def chunk(list_to_split, amount):
     """split a list into n amount"""
     for i in range(0, len(list_to_split), amount):
         yield list_to_split[i : i + amount]
 
 
 def format_output(value):
     if isinstance(value, Decimal):
         return str(value)
-    else:
-        return value
+
+    return value
+
 
 def output_to_csv_str(iterable):
-        output = io.StringIO()
-        iterable = [format_output(item) for item in iterable]
-        writer = csv.writer(output)
-        writer.writerow(iterable)
-        return output.getvalue()
+    output = io.StringIO()
+    iterable = [format_output(item) for item in iterable]
+    writer = csv.writer(output)
+    writer.writerow(iterable)
+    return output.getvalue()
```

### Comparing `dyno_viewer-0.21.4/PKG-INFO` & `dyno_viewer-0.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyno-viewer
-Version: 0.21.4
+Version: 0.22.0
 Summary: 
 Author: Rowan Self
 Author-email: piesrule123@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

