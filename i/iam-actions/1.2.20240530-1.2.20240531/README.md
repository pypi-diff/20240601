# Comparing `tmp/iam_actions-1.2.20240530.tar.gz` & `tmp/iam_actions-1.2.20240531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240530.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240531.tar", max compression
```

## Comparing `iam_actions-1.2.20240530.tar` & `iam_actions-1.2.20240531.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/README.md
--rw-r--r--   0        0        0      228 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/__init__.py
--rw-r--r--   0        0        0  4858362 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/services.py
--rw-r--r--   0        0        0   632940 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/policies.json
--rw-r--r--   0        0        0   209776 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   613908 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-30 02:26:25.677532 iam_actions-1.2.20240530/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240530/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240530/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/README.md
+-rw-r--r--   0        0        0      228 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4855406 2024-05-31 02:25:52.808221 iam_actions-1.2.20240531/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-31 02:24:44.988417 iam_actions-1.2.20240531/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   632977 2024-05-31 02:25:52.808221 iam_actions-1.2.20240531/iam_actions/policies.json
+-rw-r--r--   0        0        0   208678 2024-05-31 02:25:52.808221 iam_actions-1.2.20240531/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   613944 2024-05-31 02:25:52.808221 iam_actions-1.2.20240531/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-31 02:25:53.492219 iam_actions-1.2.20240531/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240531/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240531/PKG-INFO
```

### Comparing `iam_actions-1.2.20240530/LICENSE` & `iam_actions-1.2.20240531/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/README.md` & `iam_actions-1.2.20240531/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/iam_actions/actions.json` & `iam_actions-1.2.20240531/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997783752273696%*

 * *Differences: {"'emr-serverless'": "{'ListJobRunAttempts': OrderedDict([('access_level', 'List'), ('action', "*

 * *                     "'ListJobRunAttempts'), ('condition_keys', []), ('description', 'Grants "*

 * *                     "permission to list job run attempts associated with a job run'), ('orphan', "*

 * *                     "False), ('resources', ['jobRun'])])}",*

 * * "'workspaces-web'": "{'AssociateBrowserSettings': {'access_level': 'Undocumented', 'description': "*

 * *                     "'Not Documented by AWS', 'resources' […]*

```diff
@@ -67265,14 +67265,24 @@
             "access_level": "List",
             "action": "ListApplications",
             "condition_keys": [],
             "description": "Grants permission to list applications",
             "orphan": false,
             "resources": []
         },
+        "ListJobRunAttempts": {
+            "access_level": "List",
+            "action": "ListJobRunAttempts",
+            "condition_keys": [],
+            "description": "Grants permission to list job run attempts associated with a job run",
+            "orphan": false,
+            "resources": [
+                "jobRun"
+            ]
+        },
         "ListJobRuns": {
             "access_level": "List",
             "action": "ListJobRuns",
             "condition_keys": [],
             "description": "Grants permission to list job runs associated with an application",
             "orphan": false,
             "resources": [
@@ -173372,608 +173382,476 @@
             "resources": [
                 "workspaceimage"
             ]
         }
     },
     "workspaces-web": {
         "AssociateBrowserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateBrowserSettings",
             "condition_keys": [],
-            "description": "Grants permission to associate browser settings to web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "browserSettings",
-                "portal"
-            ]
+            "resources": []
         },
         "AssociateIpAccessSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateIpAccessSettings",
             "condition_keys": [],
-            "description": "Grants permission to associate ip access settings with web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipAccessSettings",
-                "portal"
-            ]
+            "resources": []
         },
         "AssociateNetworkSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateNetworkSettings",
             "condition_keys": [],
-            "description": "Grants permission to associate network settings to web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "networkSettings",
-                "portal"
-            ]
+            "resources": []
         },
         "AssociateTrustStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateTrustStore",
             "condition_keys": [],
-            "description": "Grants permission to associate trust stores with web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal",
-                "trustStore"
-            ]
+            "resources": []
         },
         "AssociateUserAccessLoggingSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateUserAccessLoggingSettings",
             "condition_keys": [],
-            "description": "Grants permission to associate user access logging settings with web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal",
-                "userAccessLoggingSettings"
-            ]
+            "resources": []
         },
         "AssociateUserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateUserSettings",
             "condition_keys": [],
-            "description": "Grants permission to associate user settings with web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal",
-                "userSettings"
-            ]
+            "resources": []
         },
         "CreateBrowserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateBrowserSettings",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create browser settings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateIdentityProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateIdentityProvider",
             "condition_keys": [],
-            "description": "Grants permission to create identity providers",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "identityProvider",
-                "portal"
-            ]
+            "resources": []
         },
         "CreateIpAccessSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateIpAccessSettings",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create ip access settings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateNetworkSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateNetworkSettings",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create network settings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreatePortal": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreatePortal",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create web portals",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateTrustStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTrustStore",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create trust stores",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateUserAccessLoggingSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateUserAccessLoggingSettings",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create user access logging settings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateUserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateUserSettings",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create user settings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteBrowserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteBrowserSettings",
             "condition_keys": [],
-            "description": "Grants permission to delete browser settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "browserSettings"
-            ]
+            "resources": []
         },
         "DeleteIdentityProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteIdentityProvider",
             "condition_keys": [],
-            "description": "Grants permission to delete identity providers",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "identityProvider",
-                "portal"
-            ]
+            "resources": []
         },
         "DeleteIpAccessSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteIpAccessSettings",
             "condition_keys": [],
-            "description": "Grants permission to delete ip access settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipAccessSettings"
-            ]
+            "resources": []
         },
         "DeleteNetworkSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkSettings",
             "condition_keys": [],
-            "description": "Grants permission to delete network settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "networkSettings"
-            ]
+            "resources": []
         },
         "DeletePortal": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeletePortal",
             "condition_keys": [],
-            "description": "Grants permission to delete web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "DeleteTrustStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTrustStore",
             "condition_keys": [],
-            "description": "Grants permission to delete trust stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "trustStore"
-            ]
+            "resources": []
         },
         "DeleteUserAccessLoggingSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteUserAccessLoggingSettings",
             "condition_keys": [],
-            "description": "Grants permission to delete user access logging settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "userAccessLoggingSettings"
-            ]
+            "resources": []
         },
         "DeleteUserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteUserSettings",
             "condition_keys": [],
-            "description": "Grants permission to delete user settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "userSettings"
-            ]
+            "resources": []
         },
         "DisassociateBrowserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateBrowserSettings",
             "condition_keys": [],
-            "description": "Grants permission to disassociate browser settings from web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "DisassociateIpAccessSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateIpAccessSettings",
             "condition_keys": [],
-            "description": "Grants permission to disassociate ip access logging from web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "DisassociateNetworkSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateNetworkSettings",
             "condition_keys": [],
-            "description": "Grants permission to disassociate network settings from web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "DisassociateTrustStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateTrustStore",
             "condition_keys": [],
-            "description": "Grants permission to disassociate trust stores from web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "DisassociateUserAccessLoggingSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateUserAccessLoggingSettings",
             "condition_keys": [],
-            "description": "Grants permission to disassociate user access logging settings from web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "DisassociateUserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateUserSettings",
             "condition_keys": [],
-            "description": "Grants permission to disassociate user settings from web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "GetBrowserSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetBrowserSettings",
             "condition_keys": [],
-            "description": "Grants permission to get details on browser settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "browserSettings"
-            ]
+            "resources": []
         },
         "GetIdentityProvider": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetIdentityProvider",
             "condition_keys": [],
-            "description": "Grants permission to get details on identity providers",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "identityProvider"
-            ]
+            "resources": []
         },
         "GetIpAccessSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetIpAccessSettings",
             "condition_keys": [],
-            "description": "Grants permission to get details on ip access settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipAccessSettings"
-            ]
+            "resources": []
         },
         "GetNetworkSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetNetworkSettings",
             "condition_keys": [],
-            "description": "Grants permission to get details on network settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "networkSettings"
-            ]
+            "resources": []
         },
         "GetPortal": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetPortal",
             "condition_keys": [],
-            "description": "Grants permission to get details on web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "GetPortalServiceProviderMetadata": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetPortalServiceProviderMetadata",
             "condition_keys": [],
-            "description": "Grants permission to get service provider metadata information for web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "GetTrustStore": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetTrustStore",
             "condition_keys": [],
-            "description": "Grants permission to get details on trust stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "trustStore"
-            ]
+            "resources": []
         },
         "GetTrustStoreCertificate": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetTrustStoreCertificate",
             "condition_keys": [],
-            "description": "Grants permission to get certificates from trust stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "trustStore"
-            ]
+            "resources": []
         },
         "GetUserAccessLoggingSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetUserAccessLoggingSettings",
             "condition_keys": [],
-            "description": "Grants permission to get details on user access logging settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "userAccessLoggingSettings"
-            ]
+            "resources": []
         },
         "GetUserSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetUserSettings",
             "condition_keys": [],
-            "description": "Grants permission to get details on user settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "userSettings"
-            ]
+            "resources": []
         },
         "ListBrowserSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListBrowserSettings",
             "condition_keys": [],
-            "description": "Grants permission to list browser settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListIdentityProviders": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListIdentityProviders",
             "condition_keys": [],
-            "description": "Grants permission to list identity providers",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "identityProvider"
-            ]
+            "resources": []
         },
         "ListIpAccessSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListIpAccessSettings",
             "condition_keys": [],
-            "description": "Grants permission to list ip access settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListNetworkSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListNetworkSettings",
             "condition_keys": [],
-            "description": "Grants permission to list network settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPortals": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListPortals",
             "condition_keys": [],
-            "description": "Grants permission to list web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
-            "description": "Grants permission to list tags for a resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTrustStoreCertificates": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListTrustStoreCertificates",
             "condition_keys": [],
-            "description": "Grants permission to list certificates in a trust store",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTrustStores": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListTrustStores",
             "condition_keys": [],
-            "description": "Grants permission to list trust stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListUserAccessLoggingSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListUserAccessLoggingSettings",
             "condition_keys": [],
-            "description": "Grants permission to list user access logging settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListUserSettings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListUserSettings",
             "condition_keys": [],
-            "description": "Grants permission to list user settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "TagResource",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to add one or more tags to a resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "browserSettings",
-                "ipAccessSettings",
-                "networkSettings",
-                "portal",
-                "trustStore",
-                "userAccessLoggingSettings",
-                "userSettings"
-            ]
+            "resources": []
         },
         "UntagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "UntagResource",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to remove one or more tags from a resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "browserSettings",
-                "ipAccessSettings",
-                "networkSettings",
-                "portal",
-                "trustStore",
-                "userAccessLoggingSettings",
-                "userSettings"
-            ]
+            "resources": []
         },
         "UpdateBrowserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateBrowserSettings",
             "condition_keys": [],
-            "description": "Grants permission to update browser settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "browserSettings"
-            ]
+            "resources": []
         },
         "UpdateIdentityProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateIdentityProvider",
             "condition_keys": [],
-            "description": "Grants permission to update identity provider",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "identityProvider",
-                "portal"
-            ]
+            "resources": []
         },
         "UpdateIpAccessSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateIpAccessSettings",
             "condition_keys": [],
-            "description": "Grants permission to update ip access settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipAccessSettings"
-            ]
+            "resources": []
         },
         "UpdateNetworkSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateNetworkSettings",
             "condition_keys": [],
-            "description": "Grants permission to update network settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "networkSettings"
-            ]
+            "resources": []
         },
         "UpdatePortal": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdatePortal",
             "condition_keys": [],
-            "description": "Grants permission to update web portals",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "portal"
-            ]
+            "resources": []
         },
         "UpdateTrustStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateTrustStore",
             "condition_keys": [],
-            "description": "Grants permission to update trust stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "trustStore"
-            ]
+            "resources": []
         },
         "UpdateUserAccessLoggingSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateUserAccessLoggingSettings",
             "condition_keys": [],
-            "description": "Grants permission to update user access logging settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "userAccessLoggingSettings"
-            ]
+            "resources": []
         },
         "UpdateUserSettings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateUserSettings",
             "condition_keys": [],
-            "description": "Grants permission to update user settings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "userSettings"
-            ]
+            "resources": []
         }
     },
     "xray": {
         "BatchGetTraceSummaryById": {
             "access_level": "Read",
             "action": "BatchGetTraceSummaryById",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20240530/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240531/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240531/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/iam_actions/generate/generate.py` & `iam_actions-1.2.20240531/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240531/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240531/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/iam_actions/generate/services.py` & `iam_actions-1.2.20240531/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240530/iam_actions/policies.json` & `iam_actions-1.2.20240531/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995186743233617%*

 * *Differences: {"'serviceMap'": "{'Amazon EMR Serverless': {'Actions': {insert: [(9, 'ListJobRunAttempts')]}}, "*

 * *                 "'Amazon WorkSpaces Secure Browser': OrderedDict([('StringPrefix', "*

 * *                 "'workspaces-web'), ('Actions', ['AssociateBrowserSettings', "*

 * *                 "'AssociateIpAccessSettings', 'AssociateNetworkSettings', 'AssociateTrustStore', "*

 * *                 "'AssociateUserAccessLoggingSettings', 'AssociateUserSettings', "*

 * *                 "'CreateBrowserSettings', 'CreateIdentityProvide […]*

```diff
@@ -14963,14 +14963,15 @@
                 "CancelJobRun",
                 "CreateApplication",
                 "DeleteApplication",
                 "GetApplication",
                 "GetDashboardForJobRun",
                 "GetJobRun",
                 "ListApplications",
+                "ListJobRunAttempts",
                 "ListJobRuns",
                 "ListTagsForResource",
                 "StartApplication",
                 "StartJobRun",
                 "StopApplication",
                 "TagResource",
                 "UntagResource",
@@ -22416,45 +22417,15 @@
         "Amazon WorkSpaces Application Manager": {
             "Actions": [
                 "AuthenticatePackager"
             ],
             "HasResource": false,
             "StringPrefix": "wam"
         },
-        "Amazon WorkSpaces Thin Client": {
-            "ARNFormat": "arn:aws:thinclient:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}",
-            "ARNRegex": "^arn:aws:thinclient:.+:.+:.+",
-            "Actions": [
-                "CreateEnvironment",
-                "DeleteDevice",
-                "DeleteEnvironment",
-                "DeregisterDevice",
-                "GetDevice",
-                "GetEnvironment",
-                "GetSoftwareSet",
-                "ListDeviceSessions",
-                "ListDevices",
-                "ListEnvironments",
-                "ListSoftwareSets",
-                "ListTagsForResource",
-                "TagResource",
-                "UntagResource",
-                "UpdateDevice",
-                "UpdateEnvironment",
-                "UpdateSoftwareSet"
-            ],
-            "HasResource": true,
-            "StringPrefix": "thinclient",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
-            ]
-        },
-        "Amazon WorkSpaces Web": {
+        "Amazon WorkSpaces Secure Browser": {
             "ARNFormat": "arn:aws:workspaces-web:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}",
             "ARNRegex": "^arn:aws:workspaces-web:.+",
             "Actions": [
                 "AssociateBrowserSettings",
                 "AssociateIpAccessSettings",
                 "AssociateNetworkSettings",
                 "AssociateTrustStore",
@@ -22517,14 +22488,44 @@
             "StringPrefix": "workspaces-web",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "Amazon WorkSpaces Thin Client": {
+            "ARNFormat": "arn:aws:thinclient:${Region}:${Account}:${ResourceType}/${ResourceIdentifier}",
+            "ARNRegex": "^arn:aws:thinclient:.+:.+:.+",
+            "Actions": [
+                "CreateEnvironment",
+                "DeleteDevice",
+                "DeleteEnvironment",
+                "DeregisterDevice",
+                "GetDevice",
+                "GetEnvironment",
+                "GetSoftwareSet",
+                "ListDeviceSessions",
+                "ListDevices",
+                "ListEnvironments",
+                "ListSoftwareSets",
+                "ListTagsForResource",
+                "TagResource",
+                "UntagResource",
+                "UpdateDevice",
+                "UpdateEnvironment",
+                "UpdateSoftwareSet"
+            ],
+            "HasResource": true,
+            "StringPrefix": "thinclient",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "AmazonMediaImport": {
             "ARNFormat": "arn:aws:mediaimport:${Region}:${Account}/*",
             "Actions": [
                 "CreateDatabaseBinarySnapshot"
             ],
             "HasResource": false,
             "StringPrefix": "mediaimport"
```

### Comparing `iam_actions-1.2.20240530/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240531/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987373737373737%*

 * *Differences: {"'workspaces-web'": '{replace: OrderedDict()}'}*

```diff
@@ -7015,48 +7015,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "workspaceipgroup": {
             "arn_pattern": "arn:*:workspaces:*:*:workspaceipgroup/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
-    "workspaces-web": {
-        "browserSettings": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:browserSettings/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "identityProvider": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:identityProvider/*/*",
-            "condition_keys": null
-        },
-        "ipAccessSettings": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:ipAccessSettings/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "networkSettings": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:networkSettings/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "portal": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:portal/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "trustStore": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:trustStore/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "userAccessLoggingSettings": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:userAccessLoggingSettings/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "userSettings": {
-            "arn_pattern": "arn:*:workspaces-web:*:*:userSettings/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        }
-    },
+    "workspaces-web": {},
     "xray": {
         "group": {
             "arn_pattern": "arn:*:xray:*:*:group/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "sampling-rule": {
             "arn_pattern": "arn:*:xray:*:*:sampling-rule/*",
```

### Comparing `iam_actions-1.2.20240530/iam_actions/services.json` & `iam_actions-1.2.20240531/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998889356528244%*

 * *Differences: {"'emr-serverless'": "{'Actions': {insert: [(9, 'ListJobRunAttempts')]}}",*

 * * "'workspaces-web'": "{'ServiceNames': ['Amazon WorkSpaces Secure Browser']}"}*

```diff
@@ -9179,14 +9179,15 @@
             "CancelJobRun",
             "CreateApplication",
             "DeleteApplication",
             "GetApplication",
             "GetDashboardForJobRun",
             "GetJobRun",
             "ListApplications",
+            "ListJobRunAttempts",
             "ListJobRuns",
             "ListTagsForResource",
             "StartApplication",
             "StartJobRun",
             "StopApplication",
             "TagResource",
             "UntagResource",
@@ -24544,15 +24545,15 @@
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
-            "Amazon WorkSpaces Web"
+            "Amazon WorkSpaces Secure Browser"
         ]
     },
     "xray": {
         "ARNFormats": [
             "arn:aws:xray:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
```

### Comparing `iam_actions-1.2.20240530/pyproject.toml` & `iam_actions-1.2.20240531/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240530"
+version = "1.2.20240531"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240530/setup.py` & `iam_actions-1.2.20240531/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240530',
+    'version': '1.2.20240531',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240530/PKG-INFO` & `iam_actions-1.2.20240531/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240530
+Version: 1.2.20240531
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

