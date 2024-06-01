# Comparing `tmp/shifts-0.0.2.tar.gz` & `tmp/shifts-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shifts-0.0.2.tar", max compression
+gzip compressed data, was "shifts-0.0.3.tar", max compression
```

## Comparing `shifts-0.0.2.tar` & `shifts-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-05-31 14:51:23.577219 shifts-0.0.2/LICENSE
--rw-r--r--   0        0        0       42 2024-05-31 21:57:43.156003 shifts-0.0.2/README.md
--rw-r--r--   0        0        0     1245 2024-05-31 22:03:21.279794 shifts-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       42 2024-05-31 19:51:41.125669 shifts-0.0.2/src/shifts/__init__.py
--rw-r--r--   0        0        0     3880 2024-05-31 22:01:56.387477 shifts-0.0.2/src/shifts/shifts.py
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 shifts-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-31 14:51:23.577219 shifts-0.0.3/LICENSE
+-rw-r--r--   0        0        0       42 2024-05-31 21:57:43.156003 shifts-0.0.3/README.md
+-rw-r--r--   0        0        0     1245 2024-05-31 22:06:41.107939 shifts-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-05-31 19:51:41.125669 shifts-0.0.3/src/shifts/__init__.py
+-rw-r--r--   0        0        0     3719 2024-05-31 22:05:21.262779 shifts-0.0.3/src/shifts/shifts.py
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 shifts-0.0.3/PKG-INFO
```

### Comparing `shifts-0.0.2/LICENSE` & `shifts-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shifts-0.0.2/pyproject.toml` & `shifts-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "shifts"
-version = "0.0.2"
+version = "0.0.3"
 description = "Converts shifts to a ical file"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "shifts", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `shifts-0.0.2/src/shifts/shifts.py` & `shifts-0.0.3/src/shifts/shifts.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,22 @@
                 begin=datetime(
                     year, s.begin_month, s.begin_day, s.begin_hour, s.begin_minute, 0
                 ),
                 end=datetime(year, s.end_month, s.end_day, s.end_hour, s.end_minute, 0),
             )
         )
 
-    # Read the environment variable SCHEDULE_FILE
     schedule_file = os.getenv("SCHEDULE_FILE")
     if not schedule_file:
         schedule_file = "schedule.ics"
 
     with open(schedule_file, "w") as my_file:
         my_file.writelines(c.serialize_iter())
 
-    print("Calendar file 'schedule.ics' created successfully.")
+    print(f"Calendar file 'f{schedule_file}' created successfully.")
 
 
 def next_year_month() -> Tuple[int, int]:
     now = datetime.now()
     next_month = now + relativedelta(months=1)
     return next_month.year, next_month.month
 
@@ -64,28 +63,25 @@
 
     :param shifts: The string with of shifts to validate
     :param year: The year the shifts will be in
     :param month: The month the shifts will be in
     :return: A list of shifts
     """
 
-    # Calculate the number of days given the year and month
     _, number_of_days = calendar.monthrange(year, month)
     shifts = [item.upper() for item in list(shifts) if item.strip()]  # type: ignore
     if len(shifts) != number_of_days:
         return []
 
     return shifts
 
 
 class Shift:
     def __init__(self, shift, year, month, day):
         self._shift = shift
-        # self._month = month
-        # self._day = day
 
         start_hour = {
             "M": 8,
             "T": 14,
             "N": 20,
         }
         start_minute = {
```

### Comparing `shifts-0.0.2/PKG-INFO` & `shifts-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shifts
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converts shifts to a ical file
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

