# Comparing `tmp/aws-fsx-lifecycle-status-monitor-0.0.8.tar.gz` & `tmp/aws-fsx-lifecycle-status-monitor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.8.tar", last modified: Tue Aug  1 04:17:31 2023, max compression
+gzip compressed data, was "aws-fsx-lifecycle-status-monitor-0.0.9.tar", last modified: Sat Aug 12 20:10:51 2023, max compression
```

## Comparing `aws-fsx-lifecycle-status-monitor-0.0.8.tar` & `aws-fsx-lifecycle-status-monitor-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.759951 aws-fsx-lifecycle-status-monitor-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   452794 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:17:20.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:17:31.763952 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 04:17:31.000000 aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:10:51.670833 aws-fsx-lifecycle-status-monitor-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-12 20:10:51.670833 aws-fsx-lifecycle-status-monitor-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-12 20:10:51.670833 aws-fsx-lifecycle-status-monitor-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:10:51.666833 aws-fsx-lifecycle-status-monitor-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:10:51.670833 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:10:51.670833 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   460117 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-12 20:10:36.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:10:51.670833 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-12 20:10:51.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-12 20:10:51.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-12 20:10:51.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-12 20:10:51.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-12 20:10:51.000000 aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.8/LICENSE` & `aws-fsx-lifecycle-status-monitor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.8/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.8
+Version: 0.0.9
 Summary: aws-fsx-lifecycle-status-monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.8/setup.py` & `aws-fsx-lifecycle-status-monitor-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-fsx-lifecycle-status-monitor",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "aws-fsx-lifecycle-status-monitor",
     "license": "Apache-2.0",
     "url": "https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_fsx_lifecycle_status_monitor",
         "aws_fsx_lifecycle_status_monitor._jsii"
     ],
     "package_data": {
         "aws_fsx_lifecycle_status_monitor._jsii": [
-            "aws-fsx-lifecycle-status-monitor@0.0.8.jsii.tgz"
+            "aws-fsx-lifecycle-status-monitor@0.0.9.jsii.tgz"
         ],
         "aws_fsx_lifecycle_status_monitor": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.87.0, <3.0.0",
+        "aws-cdk-lib>=2.91.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor/__init__.py` & `aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from typeguard import check_type
 
 from ._jsii import *
 
 import aws_cdk.aws_events as _aws_cdk_aws_events_ceddda9d
 import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
 import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
+import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
 import aws_cdk.aws_sns as _aws_cdk_aws_sns_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
 class FsxLifecycleStatusMonitor(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
@@ -49,30 +50,34 @@
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
+        log_retention_days: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         schedule: typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule] = None,
     ) -> None:
         '''(experimental) Creates an instance of FsxLifecycleStatusMonitor.
 
         :param scope: - parent construct.
         :param id: - unique id.
-        :param schedule: (experimental) The schedule for the FSx Lifecycle Status Monitor.
+        :param log_retention_days: (experimental) The log retention days for the FSx Lifecycle Status Monitor. Default: logs.RetentionDays.ONE_YEAR
+        :param schedule: (experimental) The schedule for the FSx Lifecycle Status Monitor. Default: "events.Schedule.cron({ minute: '0/10', hour: '*', day: '*', month: '*', year: '*' })"
 
         :stability: experimental
         :memberof: FsxLifecycleStatusMonitor - class instance
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b81cd38fb38b316d1be164277c3405c07340ac222fdb134c62c28d69a33d4354)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = FsxLifecycleStatusMonitorProps(schedule=schedule)
+        props = FsxLifecycleStatusMonitorProps(
+            log_retention_days=log_retention_days, schedule=schedule
+        )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="createIamPolicy")
     def create_iam_policy(self) -> _aws_cdk_aws_iam_ceddda9d.Policy:
         '''
         :stability: experimental
@@ -97,119 +102,194 @@
 
         :stability: experimental
         :memberof: FsxLifecycleStatusMonitor - class instance
         '''
         return typing.cast(_aws_cdk_aws_sns_ceddda9d.Topic, jsii.invoke(self, "createSNSTopic", []))
 
     @jsii.python.classproperty
+    @jsii.member(jsii_name="DEFAULT_LOG_RETENTION_PERIOD")
+    def DEFAULT_LOG_RETENTION_PERIOD(cls) -> _aws_cdk_aws_logs_ceddda9d.RetentionDays:
+        '''(experimental) Default log retention for the FSx Lifecycle Status Monitor.
+
+        :stability: experimental
+        :memberof: FsxLifecycleStatusMonitor
+        :static: true
+        '''
+        return typing.cast(_aws_cdk_aws_logs_ceddda9d.RetentionDays, jsii.sget(cls, "DEFAULT_LOG_RETENTION_PERIOD"))
+
+    @jsii.python.classproperty
     @jsii.member(jsii_name="DEFAULT_SCHEDULE")
     def DEFAULT_SCHEDULE(cls) -> _aws_cdk_aws_events_ceddda9d.Schedule:
-        '''
+        '''(experimental) Default schedule for the FSx Lifecycle Status Monitor.
+
         :stability: experimental
+        :memberof: FsxLifecycleStatusMonitor
+        :static: true
         '''
         return typing.cast(_aws_cdk_aws_events_ceddda9d.Schedule, jsii.sget(cls, "DEFAULT_SCHEDULE"))
 
     @builtins.property
     @jsii.member(jsii_name="fn")
     def fn(self) -> _aws_cdk_aws_lambda_ceddda9d.Function:
-        '''
+        '''(experimental) The Lambda function that will be triggered by the CloudWatch event.
+
         :stability: experimental
+        :memberof: FsxLifecycleStatusMonitor
+        :type: {lambda.Function}
         '''
         return typing.cast(_aws_cdk_aws_lambda_ceddda9d.Function, jsii.get(self, "fn"))
 
     @fn.setter
     def fn(self, value: _aws_cdk_aws_lambda_ceddda9d.Function) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a8b4032180c59ac1c1c0df56b2db93e26a474dc0966a18b6fe0df00ea86e84e8)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fn", value)
 
     @builtins.property
+    @jsii.member(jsii_name="logGroup")
+    def log_group(self) -> _aws_cdk_aws_logs_ceddda9d.LogGroup:
+        '''(experimental) Log group for the Lambda function.
+
+        :stability: experimental
+        :memberof: FsxLifecycleStatusMonitor
+        :type: {logs.LogGroup}
+        '''
+        return typing.cast(_aws_cdk_aws_logs_ceddda9d.LogGroup, jsii.get(self, "logGroup"))
+
+    @log_group.setter
+    def log_group(self, value: _aws_cdk_aws_logs_ceddda9d.LogGroup) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__024af8e4ffc64c7d71a3f94ccc80cee7d7dfb3945d61d0999266633b62ed2439)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "logGroup", value)
+
+    @builtins.property
     @jsii.member(jsii_name="policy")
     def policy(self) -> _aws_cdk_aws_iam_ceddda9d.Policy:
-        '''
+        '''(experimental) The IAM policy that will be attached to the Lambda function.
+
         :stability: experimental
+        :memberof: FsxLifecycleStatusMonitor
+        :type: {iam.Policy}
         '''
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.Policy, jsii.get(self, "policy"))
 
     @policy.setter
     def policy(self, value: _aws_cdk_aws_iam_ceddda9d.Policy) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__02a1148af1bfc2f0583587e22e7db7e7e8748ffaba4d54835e19a8bf66b5b136)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policy", value)
 
     @builtins.property
     @jsii.member(jsii_name="rule")
     def rule(self) -> _aws_cdk_aws_events_ceddda9d.Rule:
-        '''
+        '''(experimental) The CloudWatch event rule that will trigger the Lambda function.
+
         :stability: experimental
+        :memberof: FsxLifecycleStatusMonitor
+        :type: {events.Rule}
         '''
         return typing.cast(_aws_cdk_aws_events_ceddda9d.Rule, jsii.get(self, "rule"))
 
     @rule.setter
     def rule(self, value: _aws_cdk_aws_events_ceddda9d.Rule) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__23c10cd73da7a12439f1a5d36cb378b2bb0455726c883157646552ce5281d1cf)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "rule", value)
 
     @builtins.property
     @jsii.member(jsii_name="topic")
     def topic(self) -> _aws_cdk_aws_sns_ceddda9d.Topic:
-        '''
+        '''(experimental) Topic linked to the Lambda function.
+
         :stability: experimental
+        :memberof: FsxLifecycleStatusMonitor
+        :type: {sns.Topic}
         '''
         return typing.cast(_aws_cdk_aws_sns_ceddda9d.Topic, jsii.get(self, "topic"))
 
     @topic.setter
     def topic(self, value: _aws_cdk_aws_sns_ceddda9d.Topic) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2c8971392deb4f782b22feab8db090bb4d67e2fb89e84bbd0ac0da200604a66c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topic", value)
 
 
 @jsii.data_type(
     jsii_type="aws-fsx-lifecycle-status-monitor.FsxLifecycleStatusMonitorProps",
     jsii_struct_bases=[],
-    name_mapping={"schedule": "schedule"},
+    name_mapping={"log_retention_days": "logRetentionDays", "schedule": "schedule"},
 )
 class FsxLifecycleStatusMonitorProps:
     def __init__(
         self,
         *,
+        log_retention_days: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         schedule: typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule] = None,
     ) -> None:
-        '''(experimental) Properties for the FSx Lifecycle Status Monitor.
+        '''(experimental) Configuration properties for the FSx Lifecycle Status Monitor.
 
-        :param schedule: (experimental) The schedule for the FSx Lifecycle Status Monitor.
+        :param log_retention_days: (experimental) The log retention days for the FSx Lifecycle Status Monitor. Default: logs.RetentionDays.ONE_YEAR
+        :param schedule: (experimental) The schedule for the FSx Lifecycle Status Monitor. Default: "events.Schedule.cron({ minute: '0/10', hour: '*', day: '*', month: '*', year: '*' })"
 
         :stability: experimental
         :export: true
         :interface: FsxLifecycleStatusMonitorProps
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed85d95b85def793f715df77d38ad651d2df87abc06c2ddb33b2e3ec9da39b8b)
+            check_type(argname="argument log_retention_days", value=log_retention_days, expected_type=type_hints["log_retention_days"])
             check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if log_retention_days is not None:
+            self._values["log_retention_days"] = log_retention_days
         if schedule is not None:
             self._values["schedule"] = schedule
 
     @builtins.property
+    def log_retention_days(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays]:
+        '''(experimental) The log retention days for the FSx Lifecycle Status Monitor.
+
+        :default: logs.RetentionDays.ONE_YEAR
+
+        :stability: experimental
+        :memberof: FsxLifecycleStatusMonitorProps
+        :type: {logs.RetentionDays}
+
+        Example::
+
+            this.monitor = new FsxLifecycleStatusMonitor(this, "monitor",{
+              logRetentionDays: logs.RetentionDays.ONE_MONTH
+            });
+        '''
+        result = self._values.get("log_retention_days")
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays], result)
+
+    @builtins.property
     def schedule(self) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule]:
         '''(experimental) The schedule for the FSx Lifecycle Status Monitor.
 
+        :default: "events.Schedule.cron({ minute: '0/10', hour: '*', day: '*', month: '*', year: '*' })"
+
         :stability: experimental
         :memberof: FsxLifecycleStatusMonitorProps
         :type: {events.Schedule}
 
         Example::
 
-            "events.Schedule.cron({ minute: '0/10', hour: '*', day: '*', month: '*', year: '*' })"
+            this.monitor = new FsxLifecycleStatusMonitor(this, "monitor",{
+              logRetentionDays: logs.RetentionDays.ONE_MONTH,
+              schedule: events.Schedule.rate(cdk.Duration.hours(1)),
+            });
         '''
         result = self._values.get("schedule")
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -229,25 +309,32 @@
 
 publication.publish()
 
 def _typecheckingstub__b81cd38fb38b316d1be164277c3405c07340ac222fdb134c62c28d69a33d4354(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
+    log_retention_days: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     schedule: typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a8b4032180c59ac1c1c0df56b2db93e26a474dc0966a18b6fe0df00ea86e84e8(
     value: _aws_cdk_aws_lambda_ceddda9d.Function,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__024af8e4ffc64c7d71a3f94ccc80cee7d7dfb3945d61d0999266633b62ed2439(
+    value: _aws_cdk_aws_logs_ceddda9d.LogGroup,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__02a1148af1bfc2f0583587e22e7db7e7e8748ffaba4d54835e19a8bf66b5b136(
     value: _aws_cdk_aws_iam_ceddda9d.Policy,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__23c10cd73da7a12439f1a5d36cb378b2bb0455726c883157646552ce5281d1cf(
@@ -260,11 +347,12 @@
     value: _aws_cdk_aws_sns_ceddda9d.Topic,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ed85d95b85def793f715df77d38ad651d2df87abc06c2ddb33b2e3ec9da39b8b(
     *,
+    log_retention_days: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     schedule: typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO` & `aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-fsx-lifecycle-status-monitor
-Version: 0.0.8
+Version: 0.0.9
 Summary: aws-fsx-lifecycle-status-monitor
 Home-page: https://stefanfreitag.github.io/AWS-FSx-Lifecycle-Status-Monitor
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/AWS-FSx-Lifecycle-Status-Monitor
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-fsx-lifecycle-status-monitor-0.0.8/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt` & `aws-fsx-lifecycle-status-monitor-0.0.9/src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_fsx_lifecycle_status_monitor/py.typed
 src/aws_fsx_lifecycle_status_monitor.egg-info/PKG-INFO
 src/aws_fsx_lifecycle_status_monitor.egg-info/SOURCES.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/dependency_links.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/requires.txt
 src/aws_fsx_lifecycle_status_monitor.egg-info/top_level.txt
 src/aws_fsx_lifecycle_status_monitor/_jsii/__init__.py
-src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.8.jsii.tgz
+src/aws_fsx_lifecycle_status_monitor/_jsii/aws-fsx-lifecycle-status-monitor@0.0.9.jsii.tgz
```

