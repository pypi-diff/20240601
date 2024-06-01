# Comparing `tmp/haniwers-0.15.2.tar.gz` & `tmp/haniwers-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haniwers-0.15.2.tar", max compression
+gzip compressed data, was "haniwers-0.16.0.tar", max compression
```

## Comparing `haniwers-0.15.2.tar` & `haniwers-0.16.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.15.2/LICENSE
--rw-r--r--   0        0        0     6942 2024-05-26 12:45:22.524830 haniwers-0.15.2/README.md
--rw-r--r--   0        0        0       23 2024-05-28 22:00:03.530327 haniwers-0.15.2/haniwers/__init__.py
--rw-r--r--   0        0        0    12494 2024-05-28 01:19:45.569454 haniwers-0.15.2/haniwers/cli.py
--rw-r--r--   0        0        0    16792 2024-05-27 02:58:41.796496 haniwers-0.15.2/haniwers/config.py
--rw-r--r--   0        0        0    22568 2024-05-28 01:19:45.569719 haniwers-0.15.2/haniwers/daq.py
--rw-r--r--   0        0        0     9820 2024-05-27 02:58:41.797488 haniwers-0.15.2/haniwers/dataset.py
--rw-r--r--   0        0        0     2618 2024-05-27 02:58:41.797813 haniwers-0.15.2/haniwers/mimic.py
--rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.15.2/haniwers/postprocess.py
--rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.15.2/haniwers/preprocess.py
--rw-r--r--   0        0        0     8512 2024-05-27 02:58:41.798249 haniwers-0.15.2/haniwers/threshold.py
--rw-r--r--   0        0        0     1506 2024-05-28 22:00:03.531977 haniwers-0.15.2/pyproject.toml
--rw-r--r--   0        0        0     8443 1970-01-01 00:00:00.000000 haniwers-0.15.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.16.0/LICENSE
+-rw-r--r--   0        0        0     6942 2024-05-26 12:45:22.524830 haniwers-0.16.0/README.md
+-rw-r--r--   0        0        0       23 2024-06-01 11:33:35.326076 haniwers-0.16.0/haniwers/__init__.py
+-rw-r--r--   0        0        0    12960 2024-06-01 11:33:35.326605 haniwers-0.16.0/haniwers/cli.py
+-rw-r--r--   0        0        0    16792 2024-05-27 02:58:41.796496 haniwers-0.16.0/haniwers/config.py
+-rw-r--r--   0        0        0    28051 2024-06-01 11:33:35.326953 haniwers-0.16.0/haniwers/daq.py
+-rw-r--r--   0        0        0     9820 2024-05-27 02:58:41.797488 haniwers-0.16.0/haniwers/dataset.py
+-rw-r--r--   0        0        0     2965 2024-06-01 11:33:35.328010 haniwers-0.16.0/haniwers/mimic.py
+-rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.16.0/haniwers/postprocess.py
+-rw-r--r--   0        0        0    13030 2024-05-30 08:29:00.070036 haniwers-0.16.0/haniwers/preprocess.py
+-rw-r--r--   0        0        0     8814 2024-06-01 11:33:35.329144 haniwers-0.16.0/haniwers/threshold.py
+-rw-r--r--   0        0        0     1506 2024-06-01 11:33:35.330710 haniwers-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0     8443 1970-01-01 00:00:00.000000 haniwers-0.16.0/PKG-INFO
```

### Comparing `haniwers-0.15.2/LICENSE` & `haniwers-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.2/README.md` & `haniwers-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.2/haniwers/cli.py` & `haniwers-0.16.0/haniwers/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,68 @@
 import pendulum
 import typer
 from loguru import logger
 
 from . import __version__
 
 
-def setup_logger(level="INFO") -> None:
+def setup_logger(level="INFO") -> Path:
+    """ロガーの設定"""
+
+    format_short = (" | ").join(
+        ["{time:YYYY-MM-DDTHH:mm:ss}", "<level>{level:8}</level>", "<level>{message}</level>"]
+    )
+    format_long = (" | ").join(
+        [
+            "{time:YYYY-MM-DDTHH:mm:ss}",
+            "<level>{level:8}</level>",
+            "<cyan>{name}.{function}:{line}</cyan>",
+            "<level>{message}</level>",
+        ]
+    )
+
     # ロガーをリセット
     logger.remove()
+
     # stderr用
-    logger.add(
-        sys.stderr,
-        format="{time:YYYY-MM-DDTHH:mm:ss} | <level>{level:8}</level> | <level>{message}</level>",
-        level=level,
-    )
+    if level in ["DEBUG"]:
+        logger.add(
+            sys.stderr,
+            format=format_long,
+            level=level,
+        )
+    else:
+        logger.add(
+            sys.stderr,
+            format=format_short,
+            level=level,
+        )
+
     # ファイル出力用
     p = PlatformDirs(appname="haniwers", version=__version__)
     fname = p.user_log_path / "haniwers_log.json"
-    logger.info(fname)
     logger.add(
         sink=fname,
-        format="{time:YYYY-MM-DDTHH:mm:ss} | <level>{level:8}</level> | <cyan>{name}.{function}:{line}</cyan> | <level>{message}</level>",
+        format=format_long,
         level="DEBUG",
         serialize=True,
         retention="10 days",
         rotation="1 MB",
     )
+    return fname
 
 
 app = typer.Typer()
 
 
 @app.command()
 def version(env: bool = False, log_level: str = "INFO"):
     """Show version."""
 
-    setup_logger(level=log_level)
+    fname = setup_logger(level=log_level)
 
     msg = f"haniwers {__version__}"
     print(msg)
     logger.debug(msg)
 
     if env:
         msg = f"Python: {platform.python_version()}"
@@ -55,14 +78,18 @@
         print(msg)
         logger.debug(msg)
 
         msg = f"OS: {platform.platform()}"
         print(msg)
         logger.debug(msg)
 
+        msg = f"Logs: {fname}"
+        print(msg)
+        logger.debug(msg)
+
         print("\n🤖 Please use 'poetry env info' to see more details.\n")
 
     return
 
 
 @app.command()
 def raw2tmp(
```

### Comparing `haniwers-0.15.2/haniwers/config.py` & `haniwers-0.16.0/haniwers/config.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.2/haniwers/daq.py` & `haniwers-0.16.0/haniwers/daq.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 import pendulum
 import serial
 from deprecated import deprecated
 from loguru import logger
 from pydantic import BaseModel
 from tqdm import tqdm
+from typing import TextIO, Generator
 
 from .config import Daq
 
 
 class RealEvent(BaseModel):
     """実イベント
 
@@ -105,22 +106,23 @@
         values = [f"{k}:{v}" for k, v in data]
         ltsv_string = ("\t").join(values)
         return ltsv_string
 
 
 @deprecated(version="0.15.0", reason="Use mkdir_saved")
 def init_saved(daq: Daq) -> None:
+    """（削除予定）"""
     logger.warning("Deprecated since 0.15.0: Use mkdir_saved")
     return mkdir_saved(daq)
 
 
 def mkdir_saved(daq: Daq) -> None:
-    """Initialize destination directory to save data files
+    """データを保存するディレクトリを作成
 
-    保存先のディレクトリを初期化します。
+    データを保存するディレクトリを初期化します。
     ディレクトリが存在しない場合は、新しく作成します。
     ディレクトリが存在する場合は、そのままにします。
 
     :Args:
     - daq(Daq): DAQ設定オブジェクト
     ```
     """
@@ -130,15 +132,15 @@
     msg = f"Save files to : {p}"
     logger.info(msg)
 
     return
 
 
 def get_savef(args: Daq, fid: int | str) -> Path:
-    """Get filename to save data
+    """（削除予定）データを保存するファイル名を生成する
 
     保存するファイル名を生成します。
     DAQ設定の接頭辞（``prefix``）と拡張子（``suffix``）の値を使って
     ``{prefix}_{連番:06}.{suffix}``の形式で生成します。
 
     :Args:
     - args(Daq): DAQ設定オブジェクト
@@ -161,15 +163,15 @@
     msg = "deprecation warning: use get_savef_with_timestamp instaed."
     logger.warning(msg)
 
     return savef
 
 
 def get_savef_with_timestamp(args: Daq, fid: int | str) -> Path:
-    """Get filename to save data with timestamp
+    """データを保存するファイル名を生成する（時刻付き）
 
     作成日を含んだファイル名を生成する。
     ファイル名は、DAQ設定の接頭辞（``prefix``）、ファイルを開いた時刻（``pendulum.now``）と
     拡張子（``suffix``）の値を使って生成する。
 
     時刻のフォーマットは、ファイル名が分かりやすいように独自フォーマットにした。
 
@@ -195,15 +197,15 @@
     stem = f"{args.prefix}_{ts}_{fid:07}"
     fname = Path(stem).with_suffix(args.suffix)
     savef = Path(args.saved, fname)
     return savef
 
 
 def open_serial_connection(daq: Daq) -> serial.Serial:
-    """Open and return a serial connection.
+    """シリアル通信を開始する
 
     シリアル通信（UART）に使うポートを準備します。
     ``with``構文で使う想定です。
 
     通信に使うUSBポート名（``device``）、
     ボーレート（``baudrate``）、
     通信開始／書き込みのタイムアウト秒（``timeout``）は
@@ -375,73 +377,37 @@
             return True
         msg = f"Retry: {i} / {max_retry} times."
         logger.warning(msg)
 
     return False
 
 
-@deprecated(
-    version="0.15.0",
-    reason="Will be deprecated. Use _read_serial_data_as_event with validation.",
-)
-def _read_serial_data_as_list(port: serial.Serial) -> list:
-    """(Will be deprecated) Read serial data from port.
+def _read_event(port: serial.Serial) -> RealEvent:
+    """OSECHIから1イベントを読み出す
 
     OSECHIが接続されているポートからデータを読み出します。
     引数に指定するポートは、あらかじめ開いたものを渡してください。
     ``run_daq``や``time_daq``でデータを取得するために使います。
 
     :Args:
     - port (serial.Serial): Serialオブジェクト
 
     :Returns:
-    - row (list): 読み出した時刻を追加したデータのリスト
+    - event (RealEvent): 読み出した時刻を追加したデータ
 
     :Examples:
     ```python
     >>> with open_serial_connection() as port:
-    >>>     row = read_serial_data(port)
-    >>>     row
-    [日付, top, mid, btm, adc, tmp, atm, hmd]
-    ```
-
-    """
-    msg = "Will be deprecated."
-    logger.warning(msg)
-    now = pendulum.now().to_iso8601_string()
-    data = port.readline().decode("UTF-8").strip()
-    if len(data) == 0:
-        msg = f"No data to readout. Timed-out: {port.timeout}"
-        logger.warning(msg)
-    row = f"{now} {data}".split()
-    return row
-
-
-def _read_serial_data_as_event(port: serial.Serial) -> RealEvent:
-    """Read serial data from port.
-
-    OSECHIが接続されているポートからデータを読み出します。
-    引数に指定するポートは、あらかじめ開いたものを渡してください。
-    ``run_daq``や``time_daq``でデータを取得するために使います。
-
-    :Args:
-    - port (serial.Serial): Serialオブジェクト
-
-    :Returns:
-    - row (list): 読み出した時刻を追加したデータのリスト
-
-    :Examples:
-    ```python
-    >>> with open_serial_connection() as port:
-    >>>     row = read_serialc_data(port)
-    >>>     row
-    [日付, top, mid, btm, adc, tmp, atm, hmd]
+    >>>     event = _read_event(port)
+    >>> event
+    [pendulum.now(), top, mid, btm, adc, tmp, atm, hmd]
     ```
 
     """
+    # logger.debug("[_read_event]")
     data = port.readline().decode("UTF-8").strip().split()
     if len(data) == 0:
         msg = f"No data to readout. Timed-out: {port.timeout}"
         logger.warning(msg)
     event = RealEvent()
     event.timestamp = pendulum.now()
     event.top = int(data[0])
@@ -450,111 +416,154 @@
     event.adc = int(data[3])
     event.tmp = float(data[4])
     event.atm = float(data[5])
     event.hmd = float(data[6])
     return event
 
 
-def read_serial_data(port: serial.Serial) -> list:
-    # data = _read_serial_data_as_list(port)
-    data = _read_serial_data_as_event(port)
-    return data.to_list_string()
-
+def _loop_events_for_rows(port: serial.Serial, max_rows: int) -> Generator[RealEvent, None, None]:
+    """イベント取得ループ（回数指定）
 
-def _loop_events(port: serial.Serial, rows: list) -> RealEvent:
-    """イベント取得ループ
+    指定した回数内にOSECHIからイベントを読み取るジェネレーター関数
 
     :Args:
     - `port (serial.Serial)`: 接続済みのSerialオブジェクト
-    - `rows (list)`: ループする回数
+    - `max_rows (int)`: イベントを読み取る最大回数
 
-    :Yield:
-    - event (RealEvent): OSECHIの測定データ
+    :Yields:
+    - `event (RealEvent)`: OSECHIの測定データ
 
     """
+    logger.success("[_loop_events_for_rows]")
+    rows = range(max_rows)
     for _ in tqdm(rows, leave=False, desc="loops"):
-        event = _read_serial_data_as_event(port)
+        event = _read_event(port)
         yield event
 
 
-def loop_and_save_events(f, daq: Daq, port: serial.Serial) -> list[RealEvent]:
-    rows = range(daq.max_rows)
-    events = []
-    for event in _loop_events(port, rows):
-        events.append(event.model_dump_json())
-        row = event.to_list_string()
-        if daq.suffix in [".csv"]:
-            row = event.to_csv_string()
-            f.write(row + "\n")
-        elif daq.suffix in [".dat", ".tsv"]:
-            row = event.to_tsv_string()
-            f.write(row + "\n")
-        elif daq.suffix in [".json", ".jsonl"]:
-            row = event.model_dump_json()
-            f.write(row + "\n")
-        f.flush()
-    return events
+def _loop_events_for_duration(
+    port: serial.Serial, max_duration: int
+) -> Generator[RealEvent, None, None]:
+    """イベント取得ループ（時間指定）
 
+    指定した時間内にOSECHIからイベントを読み取るジェネレーター関数
+
+    :Args:
+    - `port (serial.Serial)`: 接続済みのSerialオブジェクト
+    - `max_duration (int)`: イベントを読み取る最大時間（秒）
+
+    :Yields:
+    - `event (RealEvent)`: OSECHIの測定データ
 
-@deprecated(version="0.15.0", reason="Will be deprecated. Use loop_and_save_events instead.")
-def save_serial_data(f, daq: Daq, port: serial.Serial) -> list:
     """
+    logger.success("[_loop_events_for_duration]")
+    start = pendulum.now()
+    stop = start.add(seconds=max_duration)
+
+    logger.debug(f"- DAQ Started: {start}")
+    logger.debug(f"- DAQ Stop   : {stop}")
+
+    while pendulum.now() < stop:
+        event = _read_event(port)
+        yield event
+
+    end = pendulum.now()
+    diff = end - start
+    elapsed_time = diff.in_seconds()
+    logger.debug(f"- DAQ Closed : {end} / Elapsed: {elapsed_time} sec.")
+
+
+def loop_and_save(fname: Path, generator: Generator) -> list[RealEvent]:
+    """イベント保存ループ
+
+    ファイル名を指定して、イベントを保存します。
+    保存形式はファイル名の拡張子で判定します。
+    有効な拡張子は``[".csv", ".dat", ".tsv", ".json", ".jsonl"]``です。
+
+    イベントの取得方法は``generator``で指定します。
+    有効なジェネレーターは``[_loop_events_for_rows, _loop_events_for_duration]``です。
+
     :Args:
-    - f: ファイルポインタ
-    - daq (Daq): Daqオブジェクト
-    - port (serial.Serial): Serialオブジェクト
+    - fname (Path): データを追記するファイル名
+    - generator (Generator): イベントの取得方法 [`_loop_events_for_rows``, ``_loop_events_for_duration``]
 
-    :Return:
-    - rows (list[list]): 取得したデータのリスト
+    :Returns:
+    - events (list[RealEvent]): OSECHIの測定データのリスト
 
-    :TODO:
-    - Daqオブジェクトに依存しない関数にしたい（ジェネレーターにするのがいいのかな？）
-    - pd.DataFrameを返した方がいいかもしれない？
     """
-    max_rows = daq.max_rows
-    rows = []
-    for _ in tqdm(range(max_rows), leave=False, desc="rows"):
-        row = read_serial_data(port)
-        rows.append(row)
-        if daq.suffix == ".csv":
-            writer = csv.writer(f)
-            writer.writerow(row)
-        else:
-            writer = csv.writer(f, delimiter=" ")
-            writer.writerow(row)
-        f.flush()
-    return rows
+    suffix = fname.suffix
+    logger.success("[loop_and_save]")
+    events = []
+    with fname.open("x") as f:
+        for event in generator:
+            events.append(event)
+            if suffix in [".csv"]:
+                row = event.to_csv_string()
+                f.write(row + "\n")
+            if suffix in [".dat", ".tsv"]:
+                row = event.to_tsv_string()
+                f.write(row + "\n")
+            if suffix in [".json", ".jsonl"]:
+                row = event.model_dump_json()
+                f.write(row + "\n")
+            f.flush()
+    return events
 
 
 def run_daq(daq: Daq) -> None:
-    """メインDAQ
+    """DAQを実行する（回数指定）
 
     OSECHIが接続されたUSBポートとシリアル通信をして、データ取得する。
     指定したファイル数と行数をでループ処理する。
 
-    :TODO:
-    - 関数名をより適切なものに変えたい
-    - while_daq みたいなのを作ってもいいかもしれない
     """
     # Open serial connection
     with open_serial_connection(daq) as port:
         mkdir_saved(daq)
 
+        logger.debug(f"Port opend : {port.name}")
         for nfile in tqdm(range(daq.max_files), desc="files"):
             savef = get_savef_with_timestamp(daq, nfile)
             msg = f"Saving data to: {savef}."
             logger.info(msg)
             logger.info("Press Ctrl-c to stop.")
-
-            with savef.open("a") as f:
-                # save_serial_data(f, daq, port)
-                loop_and_save_events(f, daq, port)
-
+            loop_and_save(
+                fname=savef,
+                generator=_loop_events_for_rows(port=port, max_rows=daq.max_rows),
+            )
             msg = f"Saved data to: {savef}."
             logger.success(msg)
+    logger.debug(f"Port closed : {port.name}")
+
+
+def scan_daq(args: Daq, fname: str, duration: int) -> pd.DataFrame:
+    """DAQを実行する（時間指定）
+
+    :Args:
+    - args (Daq): Daqオブジェクト
+    - duration (int): 測定時間を秒で指定
+
+    :Returns:
+    - data (pd.DataFrame): 測定結果のデータフレーム
+    """
+
+    with open_serial_connection(args) as port:
+        mkdir_saved(args)
+
+        logger.debug(f"Port opened : {port.name}")
+        events = loop_and_save(
+            fname=Path(fname),
+            generator=_loop_events_for_duration(port=port, max_duration=duration),
+        )
+        msg = f"Saved data to: {fname}."
+        logger.success(msg)
+
+    logger.debug(f"Port closed : {port.name}")
+    # data = pd.DataFrame(rows)
+    return events
 
 
 def run(args: Daq):
     """メインのDAQ
 
     run_daqのラッパー。例外処理などで囲んだもの。
 
@@ -582,17 +591,20 @@
         Unaware error occurred.
         Please think if you need to handle this error.
         """
         logger.error(msg)
         sys.exit()
 
 
+"""削除予定の関数"""
+
+
+@deprecated(version="0.15.3", reason="Will be deprecated. Use scan_daq instead.")
 def time_daq(args: Daq, duration: int) -> pd.DataFrame:
-    """
-    測定時間を指定してDAQを走らせます。
+    """（削除予定）測定時間を指定してDAQを走らせます。
 
     :Args:
     - args (Daq): Daqオブジェクト
     - duration (int): 測定時間を秒で指定
 
     :Returns:
     - data (pd.DataFrame): 測定結果のデータフレーム
@@ -630,16 +642,15 @@
 
 
 @deprecated(
     version="0.14.0",
     reason="Will be deprecated. Use threshold.scan_threshold_by_channel instead.",
 )
 def scan_ch_vth(daq: Daq, duration: int, ch: int, vth: int) -> list:
-    """
-    Run threshold scan.
+    """（削除予定）Run threshold scan.
 
     :Args:
     - daq (Daq): Daqオブジェクト
     - duration (int): 測定時間（秒）
     - ch (int): 測定するチャンネル番号
     - vth (int): スレッショルド値
 
@@ -688,16 +699,15 @@
 
 
 @deprecated(
     version="0.14.0",
     reason="Will be deprecated. Use threshold.scan_thresholds instead.",
 )
 def scan_ch_thresholds(daq: Daq, duration: int, ch: int, thresholds: list[int]) -> list[list]:
-    """
-    Run threshold scan.
+    """（削除予定）Run threshold scan.
 
     :Args:
     - daq (Daq): Daqオブジェクト
     - duration (int): 測定時間（秒）
     - ch (int): チャンネル番号
     - thresholds (list[int]): スレッショルド値のリスト
 
@@ -724,7 +734,150 @@
         msg = "-" * 40 + f"[{i+1:2d}/{n:2d}: {vth}]"
         logger.info(msg)
         row = scan_ch_vth(daq, duration, ch, vth)
         if row:
             rows.append(row)
 
     return rows
+
+
+@deprecated(
+    version="0.15.0",
+    reason="Will be deprecated. Use _read_event (RealEvent).",
+)
+def _read_serial_data_as_list(port: serial.Serial) -> list:
+    """（削除予定）Read serial data from port.
+
+    OSECHIが接続されているポートからデータを読み出します。
+    引数に指定するポートは、あらかじめ開いたものを渡してください。
+    ``run_daq``や``time_daq``でデータを取得するために使います。
+
+    :Args:
+    - port (serial.Serial): Serialオブジェクト
+
+    :Returns:
+    - row (list): 読み出した時刻を追加したデータのリスト
+
+    :Examples:
+    ```python
+    >>> with open_serial_connection() as port:
+    >>>     row = read_serial_data(port)
+    >>>     row
+    [日付, top, mid, btm, adc, tmp, atm, hmd]
+    ```
+
+    """
+    msg = "Will be deprecated. Use _read_event."
+    logger.warning(msg)
+    now = pendulum.now().to_iso8601_string()
+    data = port.readline().decode("UTF-8").strip()
+    if len(data) == 0:
+        msg = f"No data to readout. Timed-out: {port.timeout}"
+        logger.warning(msg)
+    row = f"{now} {data}".split()
+    return row
+
+
+@deprecated(
+    version="0.15.0",
+    reason="Will be deprecated. Use _read_event (RealEvent).",
+)
+def read_serial_data(port: serial.Serial) -> list:
+    """（削除予定）"""
+    msg = "Will be deprecated. Use _read_event."
+    logger.warning(msg)
+    data = _read_serial_data_as_list(port)
+    return data
+
+
+@deprecated(version="0.15.3", reason="Will be deprecated. Use loop_and_save instead.")
+def _loop_and_save_events(
+    fname: Path, port: serial.Serial, max_rows: int, suffix: str = ".csv"
+) -> list:
+    """（削除予定）イベント保存ループ
+
+    :Args:
+    - `f (typing.TextIO)`: 開いたファイルオブジェクト
+    - `port (serial.Serial)` : 接続済みのSerialオブジェクト
+    - `max_rows (int)`: 1ファイルあたりの行数の最大値
+    - `suffix (str)`: ファイルの拡張子
+
+    :Return:
+    - `events (list)`: 複数イベントの測定データ
+
+    """
+    logger.warning("Will be deprecated. Use loop_and_save instead.")
+    events = []
+    with fname.open("x") as f:
+        for event in _loop_events_for_rows(port, max_rows):
+            events.append(event)
+            if suffix in [".csv"]:
+                row = event.to_csv_string()
+                f.write(row + "\n")
+            if suffix in [".dat", ".txv"]:
+                row = event.to_tsv_string()
+                f.write(row + "\n")
+            if suffix in [".json", ".jsonl"]:
+                row = event.model_dump_json()
+                f.write(row + "\n")
+            f.flush()
+    return events
+
+
+@deprecated(version="0.15.3", reason="Will be deprecated. Use _loop_and_save_events instead.")
+def loop_and_save_events(f: TextIO, daq: Daq, port: serial.Serial) -> list[str]:
+    """（削除予定）イベント保存ループ
+
+    :Args:
+    - f (TextIO): データを書き込むファイルオブジェクト
+    - daq (Daq): Daqオブジェクト
+    - port (serial.Serial): 接続済みのSerialオブジェクト
+
+    """
+    logger.warning("Will be deprecated. Use _loop_and_save_events instead.")
+    rows = daq.max_rows
+    events = []
+    for event in _loop_events_for_rows(port, max_rows=rows):
+        events.append(event.model_dump_json())
+        if daq.suffix in [".csv"]:
+            row = event.to_csv_string()
+            f.write(row + "\n")
+        elif daq.suffix in [".dat", ".tsv"]:
+            row = event.to_tsv_string()
+            f.write(row + "\n")
+        elif daq.suffix in [".json", ".jsonl"]:
+            row = event.model_dump_json()
+            f.write(row + "\n")
+        f.flush()
+    return events
+
+
+@deprecated(version="0.15.0", reason="Will be deprecated. Use _loop_and_save_events instead.")
+def save_serial_data(f, daq: Daq, port: serial.Serial) -> list:
+    """（削除予定）
+
+    :Args:
+    - f: ファイルポインタ
+    - daq (Daq): Daqオブジェクト
+    - port (serial.Serial): Serialオブジェクト
+
+    :Return:
+    - rows (list[list]): 取得したデータのリスト
+
+    :TODO:
+    - Daqオブジェクトに依存しない関数にしたい（ジェネレーターにするのがいいのかな？）
+    - pd.DataFrameを返した方がいいかもしれない？
+    """
+    logger.warning("Will be deprecated. Use _loop_and_save_events instead.")
+    max_rows = daq.max_rows
+    rows = []
+    for _ in tqdm(range(max_rows), leave=False, desc="rows"):
+        row = read_serial_data(port)
+        rows.append(row)
+        if daq.suffix == ".csv":
+            writer = csv.writer(f)
+            writer.writerow(row)
+        else:
+            writer = csv.writer(f, delimiter=" ")
+            writer.writerow(row)
+        f.flush()
+    return rows
```

### Comparing `haniwers-0.15.2/haniwers/dataset.py` & `haniwers-0.16.0/haniwers/dataset.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.2/haniwers/mimic.py` & `haniwers-0.16.0/haniwers/mimic.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,28 @@
         self.tmp = random.gauss(mu=25.0, sigma=3) + random.gauss()
         self.atm = random.gauss(mu=101000, sigma=1000) + random.gauss()
         self.hmd = random.gauss(mu=50, sigma=15) + random.gauss()
 
         if self.top > 0:
             self.adc = random.randint(1, 1024)
 
+    def to_mock_string(self) -> str:
+        """モックしたデータ列
+
+        時刻が入ってないスペース区切りの文字列
+
+        :Example
+        ```
+        top mid btm adc tmp atm hmd
+        ```
+        """
+        values_ = self.to_list_string()[1:]
+        mock_string = (" ").join(values_)
+        return mock_string
+
 
 def fake_events_generator(n: int, seed: int | None = None, interval: str | int = "random"):
     """指定した回数のFakeEventを任意の間隔で生成する
 
     :Args:
         - n (int): 生成するFakeEventの数
         - seed (int | None) : 乱数シード。デフォルトは `None`
```

### Comparing `haniwers-0.15.2/haniwers/postprocess.py` & `haniwers-0.16.0/haniwers/postprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.2/haniwers/preprocess.py` & `haniwers-0.16.0/haniwers/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,24 +77,28 @@
     :Returns:
     - merged (pd.DataFrame): すべての測定データを結合したデータフレーム
     """
     names = ["datetime", "top", "mid", "btm", "adc", "tmp", "atm", "hmd"]
     data = []
     for fname in fnames:
         _suffix = fname.suffix
+        _stem = fname.stem
         if _suffix in [".dat"]:
             datum = pl.read_csv(
                 fname,
                 has_header=False,
                 new_columns=names,
                 separator=" ",
                 comment_char="t",
             )
         elif _suffix in [".csv"]:
-            datum = pl.read_csv(fname, has_header=False, new_columns=names)
+            if _stem.startswith("osechi_data"):
+                datum = pl.read_csv(fname, has_header=False, new_columns=names)
+            elif _stem.startswith("scan_data"):
+                datum = pl.read_csv(fname, has_header=False, new_columns=names, skip_rows=1)
         else:
             msg = f"Unknown suffix: {_suffix}"
             logger.warning(msg)
             break
         data.append(datum)
     merged = pl.concat(data).to_pandas().dropna(how="all")
```

### Comparing `haniwers-0.15.2/haniwers/threshold.py` & `haniwers-0.16.0/haniwers/threshold.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,31 @@
 import pendulum
 from loguru import logger
 from scipy.optimize import curve_fit
 from scipy.special import erfc
 from pydantic import BaseModel
 
 from .config import Daq
-from .daq import get_savef_with_timestamp, set_vth_retry, time_daq
+from .daq import (
+    get_savef_with_timestamp,
+    set_vth_retry,
+    time_daq,
+    scan_daq,
+)
+
+
+def scan_threshold(args: Daq, fname: str, duration: int) -> pd.DataFrame:
+    events = scan_daq(args, fname, duration)
+    # logger.debug(events)
+    rows = []
+    for event in events:
+        rows.append(event.model_dump())
+    data = pd.DataFrame(rows)
+    # logger.debug(data)
+    return data
 
 
 def scan_threshold_by_channel(daq: Daq, duration: int, ch: int, vth: int) -> list:
     """
     Run threshold scan by channel.
 
     :Args:
@@ -31,23 +47,22 @@
     if not set_vth_retry(daq, ch, vth, 3):
         msg = f"Failed to set threshold: ch{ch} - {vth}"
         logger.error(msg)
         return []
 
     # Collect data
     try:
-        rows = time_daq(daq, duration)
+        # fidは7ケタまで使える
+        fid = f"{ch:02}_{vth:04}"
+        fname = get_savef_with_timestamp(daq, fid)
+        rows = scan_threshold(daq, fname, duration)
         counts = len(rows)
         tmp = rows["tmp"].mean()
         atm = rows["atm"].mean()
         hmd = rows["hmd"].mean()
-        # fidは7ケタまで使える
-        fid = f"{ch:02}_{vth:04}"
-        fname = get_savef_with_timestamp(daq, fid)
-        rows.to_csv(fname, index=False)
         msg = f"Saved data to: {fname}"
         logger.info(msg)
     except Exception as e:
         msg = f"Failed to collect data due to: {str(e)}"
         logger.error(msg)
         counts = 0
         tmp = 0
```

### Comparing `haniwers-0.15.2/pyproject.toml` & `haniwers-0.16.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.15.2"
+version = "0.16.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "haniwers/__init__.py:__version__",
 ]
 
 [tool.poetry]
 name = "haniwers"
-version = "0.15.2"
+version = "0.16.0"
 description = "Analysis tool for TanQ/FunQ project"
 authors = ["Shota Takahashi (KMI) <shotakaha@kmi.nagoya-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://qumasan.gitlab.io/haniwers/docs/"
 repository = "https://gitlab.com/qumasan/haniwers/"
 keywords = ["muon"]
```

### Comparing `haniwers-0.15.2/PKG-INFO` & `haniwers-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haniwers
-Version: 0.15.2
+Version: 0.16.0
 Summary: Analysis tool for TanQ/FunQ project
 Home-page: https://qumasan.gitlab.io/haniwers/docs/
 License: MIT
 Keywords: muon
 Author: Shota Takahashi (KMI)
 Author-email: shotakaha@kmi.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
```

