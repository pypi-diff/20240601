# Comparing `tmp/correct-hours-1.2.0.tar.gz` & `tmp/correct_hours-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "correct-hours-1.2.0.tar", max compression
+gzip compressed data, was "correct_hours-2.0.0.tar", max compression
```

## Comparing `correct-hours-1.2.0.tar` & `correct_hours-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      130 2023-03-13 07:26:43.260548 correct-hours-1.2.0/correct_hours/__init__.py
--rw-r--r--   0        0        0     2459 2023-03-13 07:26:43.260859 correct-hours-1.2.0/correct_hours/__main__.py
--rw-r--r--   0        0        0        0 2022-08-07 01:19:34.871181 correct-hours-1.2.0/correct_hours/report_processors/__init__.py
--rw-r--r--   0        0        0      280 2022-08-08 12:28:51.252969 correct-hours-1.2.0/correct_hours/report_processors/myob.py
--rw-r--r--   0        0        0     5469 2023-03-12 11:17:23.183116 correct-hours-1.2.0/correct_hours/report_processors/xero/__init__.py
--rw-r--r--   0        0        0     2905 2023-03-12 11:17:23.183404 correct-hours-1.2.0/correct_hours/report_processors/xero/rate_processor.py
--rw-r--r--   0        0        0     1604 2023-03-12 11:17:23.183669 correct-hours-1.2.0/correct_hours/types.py
--rw-r--r--   0        0        0      563 2023-03-12 11:17:23.183919 correct-hours-1.2.0/correct_hours/utils.py
--rw-r--r--   0        0        0      330 2023-03-13 07:27:11.493680 correct-hours-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      688 2023-03-13 07:27:25.475576 correct-hours-1.2.0/setup.py
--rw-r--r--   0        0        0      402 2023-03-13 07:27:25.475764 correct-hours-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2024-05-29 07:32:07.142794 correct_hours-2.0.0/correct_hours/__init__.py
+-rw-r--r--   0        0        0     4927 2024-06-01 09:14:49.637302 correct_hours-2.0.0/correct_hours/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:32:07.143793 correct_hours-2.0.0/correct_hours/report_processors/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-29 07:32:07.143793 correct_hours-2.0.0/correct_hours/report_processors/myob.py
+-rw-r--r--   0        0        0     5596 2024-05-29 07:32:07.143793 correct_hours-2.0.0/correct_hours/report_processors/xero/__init__.py
+-rw-r--r--   0        0        0     2991 2024-05-29 07:32:07.144793 correct_hours-2.0.0/correct_hours/report_processors/xero/rate_processor.py
+-rw-r--r--   0        0        0     1665 2024-05-29 07:32:07.144793 correct_hours-2.0.0/correct_hours/types.py
+-rw-r--r--   0        0        0      585 2024-05-29 07:32:07.144793 correct_hours-2.0.0/correct_hours/utils.py
+-rw-r--r--   0        0        0      450 2024-06-01 09:14:49.638816 correct_hours-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 correct_hours-2.0.0/PKG-INFO
```

### Comparing `correct-hours-1.2.0/correct_hours/report_processors/xero/__init__.py` & `correct_hours-2.0.0/correct_hours/report_processors/xero/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from datetime import datetime
-from typing import Tuple
-
-from openpyxl import Workbook
-from openpyxl.styles import Font
-
-from correct_hours.report_processors.xero.rate_processor import XeroRateProcessor
-from correct_hours.types import InvalidRateLabel
-from correct_hours.utils import get_col_number, trim_rate_label
-
-ROW_OFFSET = 6
-
-
-class XeroReportProcessor:
-
-    def __init__(self, hours_workbook: Workbook, rates_workbook: Workbook) -> None:
-        self.hours_workbook = hours_workbook
-        self.rates_workbook = rates_workbook
-        self.hours_original_sheet = self.hours_workbook.active
-        self.hours_new_sheet = self.hours_workbook.copy_worksheet(from_worksheet=self.hours_original_sheet)
-
-    def add_new_column_headings(self) -> None:
-        # new column headings
-        self.hours_new_sheet.cell(5, 15, "New total").font = Font(bold=True)
-        self.hours_new_sheet.cell(5, 16, "New total per day").font = Font(bold=True)
-        self.hours_new_sheet.cell(5, 17, "Days worked").font = Font(bold=True)
-        self.hours_new_sheet.cell(5, 18, "Rates").font = Font(bold=True)
-
-    def add_up_hours_of_the_same_day(self, current_date: datetime, current_employee: str, row_start: int) -> Tuple[int, int]:
-        rows_added_count = 0
-        total_hours = 0
-        for row in self.hours_new_sheet.iter_rows(min_row=row_start, min_col=1, max_col=14, values_only=True):
-            date = row[0]
-            employee = row[1]
-            if date != current_date or employee != current_employee:
-                break
-            total = row[13]
-            total_hours += total
-            rows_added_count += 1
-        return rows_added_count, total_hours
-
-    def correct_hours(self, row_start: int, row_end: int, overtime: int) -> None:
-        time_left = overtime
-        for col_idx in range(13, 7, -1):
-            for row_idx in range(row_end, row_start - 1, -1):
-                value = self.hours_new_sheet.cell(row_idx, col_idx).value
-                if value <= 0:
-                    continue
-                corrected_value = value - time_left
-                if corrected_value < 0:
-                    time_left = corrected_value * -1
-                    corrected_value = 0
-                    self.hours_new_sheet.cell(row_idx, col_idx, corrected_value).font = Font(bold=True, color="FF0000")
-                else:
-                    self.hours_new_sheet.cell(row_idx, col_idx, corrected_value).font = Font(bold=True, color="FF0000")
-                    return
-
-    def process_rows(self) -> None:
-        # load hour rates to keep them handy
-        rate_processor = XeroRateProcessor(self.rates_workbook)
-        rate_processor.process()
-        # start processing hour rows
-        rows_processed_count = 0
-        for row_idx, row in enumerate(
-                self.hours_new_sheet.iter_rows(min_row=1, min_col=1, max_col=14, values_only=True)
-        ):
-            row_number = row_idx + 1
-            # validating row
-            if not row[0]:
-                # skip empty row
-                rows_processed_count += 1
-                continue
-            if row_number < ROW_OFFSET:
-                # skip the header rows
-                rows_processed_count += 1
-                continue
-            rate_label = row[3]
-            rate_label_trimmed = trim_rate_label(rate_label)
-            if not rate_label_trimmed:
-                raise InvalidRateLabel(rate_label, row_number)
-
-            # add new total
-            self.hours_new_sheet.cell(row_number, 15, f"=SUM(G{row_number}:M{row_number})")
-            # apply rate
-            date = row[0]
-            rate = rate_processor.get_rate(rate_label_trimmed, date)
-            rate_cell = self.hours_new_sheet.cell(row_number, 18, f"=O{row_number}*{rate}")
-            rate_cell.style = 'Currency'
-            if row_number <= rows_processed_count:
-                # skip the rows of the same day
-                continue
-            employee = row[1]
-            rows_added_count, total_hours = self.add_up_hours_of_the_same_day(date, employee, row_number)
-            # last row of the same day
-            last_row_number = (row_number + rows_added_count) - 1
-            did_overtime = False
-            if total_hours > 38:
-                overtime = total_hours - 38
-                self.correct_hours(row_number, last_row_number, overtime)
-                did_overtime = True
-            # new total per day
-            new_total_of_hours = self.hours_new_sheet.cell(
-                last_row_number, 16, f"=SUM(O{row_number}:O{last_row_number})"
-            )
-            if did_overtime:
-                new_total_of_hours.font = Font(bold=True, color="FF0000")
-            # number of days worked
-            days_worked_cell = self.hours_new_sheet.cell(last_row_number, 17, f"=P{last_row_number}/7.6")
-            days_worked_cell.style = 'Comma [0]'
-
-            rows_processed_count += rows_added_count
-        # add total cells at the bottom
-        bottom_row = rows_processed_count + 1
-        self.hours_new_sheet.cell(
-            bottom_row,
-            get_col_number("Q"),
-            f"=SUM(Q{ROW_OFFSET}:Q{rows_processed_count})"
-        ).style = "Comma [0]"
-        self.hours_new_sheet.cell(
-            bottom_row,
-            get_col_number("R"),
-            f"=SUM(R{ROW_OFFSET}:R{rows_processed_count})"
-        ).style = "Currency"
-
-    def process(self) -> None:
-        self.add_new_column_headings()
-        self.process_rows()
+from datetime import datetime
+from typing import Tuple
+
+from openpyxl import Workbook
+from openpyxl.styles import Font
+
+from correct_hours.report_processors.xero.rate_processor import XeroRateProcessor
+from correct_hours.types import InvalidRateLabel
+from correct_hours.utils import get_col_number, trim_rate_label
+
+ROW_OFFSET = 6
+
+
+class XeroReportProcessor:
+
+    def __init__(self, hours_workbook: Workbook, rates_workbook: Workbook) -> None:
+        self.hours_workbook = hours_workbook
+        self.rates_workbook = rates_workbook
+        self.hours_original_sheet = self.hours_workbook.active
+        self.hours_new_sheet = self.hours_workbook.copy_worksheet(from_worksheet=self.hours_original_sheet)
+
+    def add_new_column_headings(self) -> None:
+        # new column headings
+        self.hours_new_sheet.cell(5, 15, "New total").font = Font(bold=True)
+        self.hours_new_sheet.cell(5, 16, "New total per day").font = Font(bold=True)
+        self.hours_new_sheet.cell(5, 17, "Days worked").font = Font(bold=True)
+        self.hours_new_sheet.cell(5, 18, "Rates").font = Font(bold=True)
+
+    def add_up_hours_of_the_same_day(self, current_date: datetime, current_employee: str, row_start: int) -> Tuple[int, int]:
+        rows_added_count = 0
+        total_hours = 0
+        for row in self.hours_new_sheet.iter_rows(min_row=row_start, min_col=1, max_col=14, values_only=True):
+            date = row[0]
+            employee = row[1]
+            if date != current_date or employee != current_employee:
+                break
+            total = row[13]
+            total_hours += total
+            rows_added_count += 1
+        return rows_added_count, total_hours
+
+    def correct_hours(self, row_start: int, row_end: int, overtime: int) -> None:
+        time_left = overtime
+        for col_idx in range(13, 7, -1):
+            for row_idx in range(row_end, row_start - 1, -1):
+                value = self.hours_new_sheet.cell(row_idx, col_idx).value
+                if value <= 0:
+                    continue
+                corrected_value = value - time_left
+                if corrected_value < 0:
+                    time_left = corrected_value * -1
+                    corrected_value = 0
+                    self.hours_new_sheet.cell(row_idx, col_idx, corrected_value).font = Font(bold=True, color="FF0000")
+                else:
+                    self.hours_new_sheet.cell(row_idx, col_idx, corrected_value).font = Font(bold=True, color="FF0000")
+                    return
+
+    def process_rows(self) -> None:
+        # load hour rates to keep them handy
+        rate_processor = XeroRateProcessor(self.rates_workbook)
+        rate_processor.process()
+        # start processing hour rows
+        rows_processed_count = 0
+        for row_idx, row in enumerate(
+                self.hours_new_sheet.iter_rows(min_row=1, min_col=1, max_col=14, values_only=True)
+        ):
+            row_number = row_idx + 1
+            # validating row
+            if not row[0]:
+                # skip empty row
+                rows_processed_count += 1
+                continue
+            if row_number < ROW_OFFSET:
+                # skip the header rows
+                rows_processed_count += 1
+                continue
+            rate_label = row[3]
+            rate_label_trimmed = trim_rate_label(rate_label)
+            if not rate_label_trimmed:
+                raise InvalidRateLabel(rate_label, row_number)
+
+            # add new total
+            self.hours_new_sheet.cell(row_number, 15, f"=SUM(G{row_number}:M{row_number})")
+            # apply rate
+            date = row[0]
+            rate = rate_processor.get_rate(rate_label_trimmed, date)
+            rate_cell = self.hours_new_sheet.cell(row_number, 18, f"=O{row_number}*{rate}")
+            rate_cell.style = 'Currency'
+            if row_number <= rows_processed_count:
+                # skip the rows of the same day
+                continue
+            employee = row[1]
+            rows_added_count, total_hours = self.add_up_hours_of_the_same_day(date, employee, row_number)
+            # last row of the same day
+            last_row_number = (row_number + rows_added_count) - 1
+            did_overtime = False
+            if total_hours > 38:
+                overtime = total_hours - 38
+                self.correct_hours(row_number, last_row_number, overtime)
+                did_overtime = True
+            # new total per day
+            new_total_of_hours = self.hours_new_sheet.cell(
+                last_row_number, 16, f"=SUM(O{row_number}:O{last_row_number})"
+            )
+            if did_overtime:
+                new_total_of_hours.font = Font(bold=True, color="FF0000")
+            # number of days worked
+            days_worked_cell = self.hours_new_sheet.cell(last_row_number, 17, f"=P{last_row_number}/7.6")
+            days_worked_cell.style = 'Comma [0]'
+
+            rows_processed_count += rows_added_count
+        # add total cells at the bottom
+        bottom_row = rows_processed_count + 1
+        self.hours_new_sheet.cell(
+            bottom_row,
+            get_col_number("Q"),
+            f"=SUM(Q{ROW_OFFSET}:Q{rows_processed_count})"
+        ).style = "Comma [0]"
+        self.hours_new_sheet.cell(
+            bottom_row,
+            get_col_number("R"),
+            f"=SUM(R{ROW_OFFSET}:R{rows_processed_count})"
+        ).style = "Currency"
+
+    def process(self) -> None:
+        self.add_new_column_headings()
+        self.process_rows()
```

### Comparing `correct-hours-1.2.0/correct_hours/report_processors/xero/rate_processor.py` & `correct_hours-2.0.0/correct_hours/report_processors/xero/rate_processor.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import dataclasses
-from datetime import datetime
-from typing import Optional, List
-
-from openpyxl import Workbook
-
-from correct_hours.types import RateNotFound
-from correct_hours.utils import trim_rate_label
-
-ROWS_OFFSET = 2
-COLS_OFFSET = 3
-
-
-@dataclasses.dataclass
-class Rate:
-    label: str
-    start_date: Optional[datetime]
-    end_date: Optional[datetime]
-    rate: float
-
-    def is_within_date_range(self, date: datetime) -> bool:
-        if self.start_date is None:
-            return date < self.end_date
-        if self.end_date is None:
-            return date >= self.start_date
-        return self.start_date <= date < self.end_date
-
-
-class XeroRateProcessor:
-
-    def __init__(self, workbook: Workbook) -> None:
-        self.workbook = workbook
-        self.rates = []
-
-    def process(self) -> None:
-        return self.process_sheets()
-
-    def process_sheets(self):
-        for sheet in self.workbook.worksheets:
-            rates = self.process_rows(sheet=sheet)
-            self.rates += rates
-
-    @staticmethod
-    def process_rows(sheet) -> List[Rate]:
-        rates = []
-        for row_idx, row in enumerate(sheet.iter_rows(min_row=ROWS_OFFSET, values_only=True)):
-            row_number = row_idx + ROWS_OFFSET
-            rate_label = row[0]
-            rate_label_trimmed = trim_rate_label(rate_label)
-            if not rate_label_trimmed:
-                print(f"Rate label is empty on row {row_number}. Ignoring this rate.")
-                continue
-            for col_idx, col in enumerate(row):
-                col_number = col_idx + 1
-                if col_number < COLS_OFFSET:
-                    # skip first columns
-                    continue
-                elif col_number == COLS_OFFSET:
-                    # starting rate
-                    start_date = None
-                    end_date = sheet.cell(1, col_number + 1).value
-                elif col_idx >= len(row):
-                    # latest rate
-                    start_date = sheet.cell(1, col_number).value
-                    end_date = None
-                else:
-                    start_date = sheet.cell(1, col_number).value
-                    end_date = sheet.cell(1, col_number + 1).value
-                try:
-                    rate = float(col)
-                except:
-                    print(f"Rate on row {row_number} is not a numeric value. Ignoring this rate.")
-                    continue
-                rates.append(
-                    Rate(rate_label_trimmed, start_date, end_date, rate)
-                )
-        return rates
-
-    def get_rate(self, rate_label: str, date: datetime) -> int:
-        matching_rates = [
-            r.rate for r in self.rates if str.lower(r.label) == str.lower(rate_label) and r.is_within_date_range(date)
-        ]
-        if matching_rates:
-            return matching_rates[0]
-        else:
-            raise RateNotFound(rate_label, date)
+import dataclasses
+from datetime import datetime
+from typing import Optional, List
+
+from openpyxl import Workbook
+
+from correct_hours.types import RateNotFound
+from correct_hours.utils import trim_rate_label
+
+ROWS_OFFSET = 2
+COLS_OFFSET = 3
+
+
+@dataclasses.dataclass
+class Rate:
+    label: str
+    start_date: Optional[datetime]
+    end_date: Optional[datetime]
+    rate: float
+
+    def is_within_date_range(self, date: datetime) -> bool:
+        if self.start_date is None:
+            return date < self.end_date
+        if self.end_date is None:
+            return date >= self.start_date
+        return self.start_date <= date < self.end_date
+
+
+class XeroRateProcessor:
+
+    def __init__(self, workbook: Workbook) -> None:
+        self.workbook = workbook
+        self.rates = []
+
+    def process(self) -> None:
+        return self.process_sheets()
+
+    def process_sheets(self):
+        for sheet in self.workbook.worksheets:
+            rates = self.process_rows(sheet=sheet)
+            self.rates += rates
+
+    @staticmethod
+    def process_rows(sheet) -> List[Rate]:
+        rates = []
+        for row_idx, row in enumerate(sheet.iter_rows(min_row=ROWS_OFFSET, values_only=True)):
+            row_number = row_idx + ROWS_OFFSET
+            rate_label = row[0]
+            rate_label_trimmed = trim_rate_label(rate_label)
+            if not rate_label_trimmed:
+                print(f"Rate label is empty on row {row_number}. Ignoring this rate.")
+                continue
+            for col_idx, col in enumerate(row):
+                col_number = col_idx + 1
+                if col_number < COLS_OFFSET:
+                    # skip first columns
+                    continue
+                elif col_number == COLS_OFFSET:
+                    # starting rate
+                    start_date = None
+                    end_date = sheet.cell(1, col_number + 1).value
+                elif col_idx >= len(row):
+                    # latest rate
+                    start_date = sheet.cell(1, col_number).value
+                    end_date = None
+                else:
+                    start_date = sheet.cell(1, col_number).value
+                    end_date = sheet.cell(1, col_number + 1).value
+                try:
+                    rate = float(col)
+                except:
+                    print(f"Rate on row {row_number} is not a numeric value. Ignoring this rate.")
+                    continue
+                rates.append(
+                    Rate(rate_label_trimmed, start_date, end_date, rate)
+                )
+        return rates
+
+    def get_rate(self, rate_label: str, date: datetime) -> int:
+        matching_rates = [
+            r.rate for r in self.rates if str.lower(r.label) == str.lower(rate_label) and r.is_within_date_range(date)
+        ]
+        if matching_rates:
+            return matching_rates[0]
+        else:
+            raise RateNotFound(rate_label, date)
```

### Comparing `correct-hours-1.2.0/correct_hours/types.py` & `correct_hours-2.0.0/correct_hours/types.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import dataclasses
-from datetime import datetime
-
-RATES_FILENAME = "rates.xlsx"
-OUTPUT_FOLDER = "output"
-HOURS_NEW_FILE_PREFIX = "copy_"
-ASCII_OFFSET = 64
-
-class CorrectHoursError(Exception):
-    pass
-
-
-@dataclasses.dataclass
-class UnsupportedReportType(CorrectHoursError):
-    report_type: str
-
-    def __str__(self) -> str:
-        return f"Report not supported: {self.report_type}"
-
-
-@dataclasses.dataclass
-class InvalidRateLabel(CorrectHoursError):
-    rate_label: str
-    row_number: int
-
-    def __str__(self) -> str:
-        return (
-            f"Invalid rate label on row {self.row_number}: \"{self.rate_label}\"."
-        )
-
-@dataclasses.dataclass
-class RateNotFound(CorrectHoursError):
-    rate_label: str
-    date: datetime
-
-    def __str__(self) -> str:
-        return (
-            f"Rate not found for label \"{self.rate_label}\" and date \"{self.date.date()}\". "
-            "Make sure the rates file has an entry for this combination. "
-            "Also make sure the entry in the rate file doesn't have any trailing spaces."
-        )
-
-
-@dataclasses.dataclass
-class RateFileNotFound(CorrectHoursError):
-    rate_filePath: str
-
-    def __str__(self) -> str:
-        return (
-            f"Rate file not found in this location: \"{self.rate_filePath}\". "
-            f"Please make sure you have a file \"{RATES_FILENAME}\" in the same directory where your "
-            f"reports are located."
-        )
-
-
-@dataclasses.dataclass
-class InvalidReportType(CorrectHoursError):
-    report_type: str
-
-    def __str__(self):
-        return f"Invalid report type provided: {self.report_type}"
+import dataclasses
+from datetime import datetime
+
+RATES_FILENAME = "rates.xlsx"
+OUTPUT_FOLDER = "output"
+HOURS_NEW_FILE_PREFIX = "copy_"
+ASCII_OFFSET = 64
+
+class CorrectHoursError(Exception):
+    pass
+
+
+@dataclasses.dataclass
+class UnsupportedReportType(CorrectHoursError):
+    report_type: str
+
+    def __str__(self) -> str:
+        return f"Report not supported: {self.report_type}"
+
+
+@dataclasses.dataclass
+class InvalidRateLabel(CorrectHoursError):
+    rate_label: str
+    row_number: int
+
+    def __str__(self) -> str:
+        return (
+            f"Invalid rate label on row {self.row_number}: \"{self.rate_label}\"."
+        )
+
+@dataclasses.dataclass
+class RateNotFound(CorrectHoursError):
+    rate_label: str
+    date: datetime
+
+    def __str__(self) -> str:
+        return (
+            f"Rate not found for label \"{self.rate_label}\" and date \"{self.date.date()}\". "
+            "Make sure the rates file has an entry for this combination. "
+            "Also make sure the entry in the rate file doesn't have any trailing spaces."
+        )
+
+
+@dataclasses.dataclass
+class RateFileNotFound(CorrectHoursError):
+    rate_filePath: str
+
+    def __str__(self) -> str:
+        return (
+            f"Rate file not found in this location: \"{self.rate_filePath}\". "
+            f"Please make sure you have a file \"{RATES_FILENAME}\" in the same directory where your "
+            f"reports are located."
+        )
+
+
+@dataclasses.dataclass
+class InvalidReportType(CorrectHoursError):
+    report_type: str
+
+    def __str__(self):
+        return f"Invalid report type provided: {self.report_type}"
```

### Comparing `correct-hours-1.2.0/correct_hours/utils.py` & `correct_hours-2.0.0/correct_hours/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import datetime
-from typing import Optional
-
-from correct_hours.types import ASCII_OFFSET
-
-
-def parse_date(date_string: str) -> datetime.date:
-    parsed_datetime = datetime.datetime.strptime(date_string, "%d/%m/%Y")
-    return parsed_datetime.date()
-
-
-def get_col_number(col_name: str) -> int:
-    col_number_ascii = ord(col_name)
-    return col_number_ascii - ASCII_OFFSET
-
-
-def get_col_name(col_number: int) -> str:
-    return chr(col_number + ASCII_OFFSET)
-
-
-def trim_rate_label(rate_label: str) -> str:
-    return str.strip(rate_label) if rate_label else ""
+import datetime
+from typing import Optional
+
+from correct_hours.types import ASCII_OFFSET
+
+
+def parse_date(date_string: str) -> datetime.date:
+    parsed_datetime = datetime.datetime.strptime(date_string, "%d/%m/%Y")
+    return parsed_datetime.date()
+
+
+def get_col_number(col_name: str) -> int:
+    col_number_ascii = ord(col_name)
+    return col_number_ascii - ASCII_OFFSET
+
+
+def get_col_name(col_number: int) -> str:
+    return chr(col_number + ASCII_OFFSET)
+
+
+def trim_rate_label(rate_label: str) -> str:
+    return str.strip(rate_label) if rate_label else ""
```

