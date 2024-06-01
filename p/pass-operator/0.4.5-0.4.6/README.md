# Comparing `tmp/pass_operator-0.4.5.tar.gz` & `tmp/pass_operator-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass_operator-0.4.5.tar", max compression
+gzip compressed data, was "pass_operator-0.4.6.tar", max compression
```

## Comparing `pass_operator-0.4.5.tar` & `pass_operator-0.4.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35140 2024-05-30 20:15:41.585211 pass_operator-0.4.5/LICENSE
--rw-r--r--   0        0        0     3727 2024-05-30 20:15:41.585211 pass_operator-0.4.5/README.md
--rw-r--r--   0        0        0     1612 2024-05-30 20:15:59.485250 pass_operator-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1670 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/__init__.py
--rw-r--r--   0        0        0    18470 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/daemon.py
--rw-r--r--   0        0        0     2017 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/git.py
--rw-r--r--   0        0        0     1213 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/gpg.py
--rw-r--r--   0        0        0     9217 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/secret.py
--rw-r--r--   0        0        0     1313 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/utils.py
--rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 pass_operator-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    35140 2024-05-31 18:17:28.384762 pass_operator-0.4.6/LICENSE
+-rw-r--r--   0        0        0     3496 2024-05-31 18:17:28.388762 pass_operator-0.4.6/README.md
+-rw-r--r--   0        0        0     1612 2024-05-31 18:17:45.820851 pass_operator-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1670 2024-05-31 18:17:28.392762 pass_operator-0.4.6/src/passoperator/__init__.py
+-rw-r--r--   0        0        0    15234 2024-05-31 18:17:28.392762 pass_operator-0.4.6/src/passoperator/daemon.py
+-rw-r--r--   0        0        0     2017 2024-05-31 18:17:28.392762 pass_operator-0.4.6/src/passoperator/git.py
+-rw-r--r--   0        0        0     1213 2024-05-31 18:17:28.392762 pass_operator-0.4.6/src/passoperator/gpg.py
+-rw-r--r--   0        0        0     3691 2024-05-31 18:17:28.392762 pass_operator-0.4.6/src/passoperator/locks.py
+-rw-r--r--   0        0        0     9217 2024-05-31 18:17:28.392762 pass_operator-0.4.6/src/passoperator/secret.py
+-rw-r--r--   0        0        0     1313 2024-05-31 18:17:28.392762 pass_operator-0.4.6/src/passoperator/utils.py
+-rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 pass_operator-0.4.6/PKG-INFO
```

### Comparing `pass_operator-0.4.5/LICENSE` & `pass_operator-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.5/README.md` & `pass_operator-0.4.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # `pass` secrets operator
 
 ![GitHub Release](https://img.shields.io/github/v/release/premiscale/pass-operator)
 ![PyPI - License](https://img.shields.io/pypi/l/pass-operator)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pass-operator)
-![Docker Pulls](https://img.shields.io/docker/pulls/premiscale/pass-operator)
-![CircleCI](https://img.shields.io/circleci/build/github/premiscale/pass-operator)
-
 
 A Kubernetes operator to sync and decrypt secrets from a password store ([pass](https://www.passwordstore.org/)) Git repository. This operator is proposed as a proof-of-concept and shouldn't be used in any production capacity.
 
 While this approach to secrets management on Kubernetes is more technically challenging, the advantage is that we don't have to rely on a 3rd party SaaS platform, such as Vault or Doppler, to hold our secrets (the obvious benefits these platforms do provide, however, are better user and access management). We may also use this operator in an airgapped environment with a self-hosted git repository.
 
 <!--
 I also acknowledge that this approach swims against the DevSecOps tide in that it requires you to store your secrets (albeit encrypted)
@@ -21,15 +17,15 @@
 The following flowchart outlines how this operator reacts to `PassSecret`-related events and pass store updates.
 
 <p align="center" width="100%">
   <img width="100%" src="img/pass-operator-flow.png" alt="pass operator flow diagram">
 </p>
 
 From a high level, this operator runs `git pull` on an interval to grab updates from a git repository populated with encrypted
-secrets by `pass`. It maps secrets' paths to data values through the application of a [`PassSecret`](helm/operator/crds/PassSecret.yaml), a [custom resource](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/), such as the following.
+secrets by `pass`. It maps secrets' paths to data values through the application of a [`PassSecret`](helm/operator-crds/templates/PassSecret.yaml), a [custom resource](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/), such as the following.
 
 ```yaml
 apiVersion: secrets.premiscale.com/v1alpha1
 kind: PassSecret
 metadata:
   name: mysecret
   namespace: pass-operator-test
```

### Comparing `pass_operator-0.4.5/pyproject.toml` & `pass_operator-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pass-operator"
-version = "v0.4.5"
+version = "v0.4.6"
 description = "A Kubernetes operator that syncs and decrypts secrets from pass store git repositories"
 authors = ["Emma Doyle <emma@premiscale.com>"]
 maintainers = ["Emma Doyle <emma@premiscale.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
   { include = "passoperator", from = "src" }
```

### Comparing `pass_operator-0.4.5/src/passoperator/__init__.py` & `pass_operator-0.4.6/src/passoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.5/src/passoperator/daemon.py` & `pass_operator-0.4.6/src/passoperator/daemon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,37 @@
 """
 A kubernetes operator that syncs and decrypts secrets from Linux password store (https://www.passwordstore.org/) git repositories.
 """
 
 
-from typing import Any, List, Tuple
+from typing import Any
 from pathlib import Path
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from importlib import metadata
 from kubernetes import client, config
 from http import HTTPStatus
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
-from time import sleep
 
 from passoperator.git import pull, clone
 from passoperator.utils import LogLevel
 from passoperator.secret import PassSecret, ManagedSecret
+from passoperator.locks import lock_passsecret
 from passoperator import env
 
 import asyncio
 import logging
 import sys
 import kopf
 
 
 __version__ = metadata.version('pass-operator')
 
 log = logging.getLogger(__name__)
 
-__in_progress_queue: List[Tuple[Any, Any]] = []
-
-
-def _passsecret_block(body: kopf.Body) -> None:
-    """
-    Block handlers' progress on a PassSecret until it's safe to modify the managed secret.
-    Decryption takes time, so we want to be sure to queue up any changes.
-
-    Args:
-        body [kopf.Body]: raw body of the PassSecret.
-    """
-    log.debug(f'Blocking PassSecret "{body["metadata"]["name"]}" in namespace "{body["metadata"]["namespace"]}')
-    __in_progress_queue.append(
-        (
-            body['metadata']['name'],
-            body['metadata']['namespace']
-        )
-    )
-
-
-def _is_passsecret_blocked(body: kopf.Body) -> bool:
-    """
-    Check if a PassSecret is blocked from modification.
-
-    Args:
-        body [kopf.Body]: raw body of the PassSecret.
-
-    Returns:
-        bool: True if the PassSecret is blocked, else False.
-    """
-    return (
-        body['metadata']['name'],
-        body['metadata']['namespace']
-    ) in __in_progress_queue
-
-
-def _block_passsecret_block(body: kopf.Body) -> None:
-    """
-    Block handlers' progress on a PassSecret until it's safe to modify the managed secret.
-    This should only ever be called by event handlers, not by the reconciliation loop.
-
-    Args:
-        body (kopf.Body): raw body of the PassSecret.
-    """
-    while True:
-        if not _is_passsecret_blocked(body):
-            _passsecret_block(body)
-            break
-        else:
-            log.debug(f'PassSecret "{body["metadata"]["name"]}" in namespace "{body["metadata"]["namespace"]}" is already blocked.')
-            sleep(0.5)
-
-
-def _lift_passsecret_block(body: kopf.Body) -> None:
-    """
-    Unblock handlers' progress to modify the managed secret.
-
-    Args:
-        body [kopf.Body]: raw body of the PassSecret.
-    """
-    log.debug(f'Lifting block on PassSecret "{body["metadata"]["name"]}" in namespace "{body["metadata"]["namespace"]}"')
-    __in_progress_queue.remove(
-        (
-            body['metadata']['name'],
-            body['metadata']['namespace']
-        )
-    )
-
 
 @kopf.on.startup()
 def start(settings: kopf.OperatorSettings, **_: Any) -> None:
     """
     Set up operator runtime.
     """
     log.info(f'Starting operator version {__version__}')
@@ -112,38 +44,33 @@
     'secrets.premiscale.com', 'v1alpha1', 'passsecret',
     # Interval to check every instance of a PassSecret.
     interval=float(env['OPERATOR_INTERVAL']),
     # Initial delay in seconds before reviewing managed PassSecrets.
     initial_delay=float(env['OPERATOR_INITIAL_DELAY']),
     # Don't delay if the prior reconciliation hasn't completed.
     sharp=True)
+@lock_passsecret(exit_early=True)
 def reconciliation(body: kopf.Body, **_: Any) -> None:
     """
     Reconcile state of a managed secret against the pass store. Update secrets' data if a mismatch
     is found. Kopf timers are triggered on an object-by-object basis, so this method will
     automatically revisit every PassSecret, iff it resides in the same namespace as the operator.
 
     Args:
         body [kopf.Body]: raw body of the PassSecret.
     """
 
-    # Before we parse and decrypt anything, which is more expensive, check if this PassSecret is already in progress.
-    if _is_passsecret_blocked(body):
-        log.info(f'PassSecret "{body["metadata"]["name"]}" is still in progress. Skipping.')
-        return None
-
     # Ensure the GPG key ID in ~/.password-store/${PASS_DIRECTORY}/.gpg-id did not change with the git update.
     check_gpg_id(
         path=f'{env["PASS_DIRECTORY"]}/.gpg-id'
     )
 
     v1 = client.CoreV1Api()
 
     # Create a new PassSecret object with an up-to-date managedSecret decrypted value from the pass store.
-    _passsecret_block(body)
     passSecretObj = PassSecret.from_kopf(body)
 
     log.info(
         f'Reconciling PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}" against password store.'
     )
 
     try:
@@ -155,15 +82,14 @@
         log.debug(secret)
         _managedSecret = ManagedSecret.from_kopf(secret.to_dict())
 
         # If the managed secret data does not match what's in the newly-generated ManagedSecret object,
         # submit a patch request to update it.
         if not _managedSecret.data_equals(passSecretObj.spec.managedSecret):
             if _managedSecret.immutable:
-                _lift_passsecret_block(body)
                 raise kopf.TemporaryError(
                     f'PassSecret "{passSecretObj.metadata.name}" managed secret "{passSecretObj.spec.managedSecret.metadata.name}" is immutable. Ignoring data patch.'
                 )
 
             v1.patch_namespaced_secret(
                 name=passSecretObj.spec.managedSecret.metadata.name,
                 namespace=passSecretObj.spec.managedSecret.metadata.namespace,
@@ -182,18 +108,15 @@
             v1.create_namespaced_secret(
                 namespace=passSecretObj.spec.managedSecret.metadata.namespace,
                 body=client.V1Secret(
                     **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
                 )
             )
         else:
-            _lift_passsecret_block(body)
             raise kopf.PermanentError(e)
-    finally:
-        _lift_passsecret_block(body)
 
 
 # @kopf.on.cleanup()
 # def cleanup(**kwargs) -> None:
 #     pass
 
 # @kopf.on.resume()
@@ -227,14 +150,15 @@
         else:
             return None
     except client.ApiException as e:
         raise kopf.PermanentError(e)
 
 
 @kopf.on.update('secrets.premiscale.com', 'v1alpha1', 'passsecret')
+@lock_passsecret()
 def update(old: kopf.BodyEssence | Any, new: kopf.BodyEssence | Any, meta: kopf.Meta, body: kopf.Body, **_: Any) -> None:
     """
     An update was received on the PassSecret object, so attempt to update the corresponding Secret.
 
     This method is pretty much identical to 'create'-type events.
 
     Args:
@@ -246,40 +170,34 @@
     metadata = {
         'metadata': {
             'name': meta['name'],
             'namespace': meta['namespace']
         }
     }
 
-    # If a reconciliation is already in progress for the triggered PassSecret, block this event handler
-    # until it's safe to modify the managed secret.
-    _block_passsecret_block(body)
-
     # Parse the old PassSecret manifest.
     try:
         oldPassSecret = PassSecret.from_kopf(
             {
                 **metadata,
                 **old
             }
         )
     except (ValueError, KeyError) as e:
-        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     # Parse the new PassSecret manifest.
     try:
         newPassSecret = PassSecret.from_kopf(
             {
                 **metadata,
                 **new
             }
         )
     except (ValueError, KeyError) as e:
-        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     v1 = client.CoreV1Api()
 
     # Handle typically immutable field changes separately from the rest of the manifest on Secrets.
     try:
         if newPassSecret.spec.managedSecret.metadata.namespace != oldPassSecret.spec.managedSecret.metadata.namespace or newPassSecret.spec.managedSecret.metadata.name != oldPassSecret.spec.managedSecret.metadata.name:
@@ -306,35 +224,29 @@
             )
 
         log.info(
             f'Successfully updated PassSecret "{newPassSecret.metadata.name}" managed Secret "{newPassSecret.spec.managedSecret.metadata.name}".'
         )
     except client.ApiException as e:
         raise kopf.PermanentError(e)
-    finally:
-        _lift_passsecret_block(body)
 
 
 @kopf.on.create('secrets.premiscale.com', 'v1alpha1', 'passsecret')
+@lock_passsecret()
 def create(body: kopf.Body, **_: Any) -> None:
     """
     Create a new Secret with the spec of the newly-created PassSecret.
 
     Args:
         body [kopf.Body]: raw body of the created PassSecret.
     """
 
-    # If a reconciliation is already in progress for the triggered PassSecret, block this event handler
-    # until it's safe to modify the managed secret.
-    _block_passsecret_block(body)
-
     try:
         passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
-        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     log.info(f'PassSecret "{passSecretObj.metadata.name}" created')
 
     v1 = client.CoreV1Api()
 
     try:
@@ -349,35 +261,29 @@
             f'Created PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}"'
         )
     except client.ApiException as e:
         if e.status == HTTPStatus.CONFLICT:
             raise kopf.TemporaryError(f'Duplicate PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}". Skipping.')
 
         raise kopf.PermanentError(e)
-    finally:
-        _lift_passsecret_block(body)
 
 
 @kopf.on.delete('secrets.premiscale.com', 'v1alpha1', 'passsecret')
+@lock_passsecret()
 def delete(body: kopf.Body, **_: Any) -> None:
     """
     Remove a managed secret, as the managing PassSecret has been deleted.
 
     Args:
         body [kopf.Body]: raw body of the deleted PassSecret.
     """
 
-    # If a reconciliation is already in progress for the triggered PassSecret, block this event handler
-    # until it's safe to modify the managed secret.
-    _block_passsecret_block(body)
-
     try:
         passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
-        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     log.info(f'PassSecret "{passSecretObj.metadata.name}" deleted')
 
     v1 = client.CoreV1Api()
 
     try:
@@ -386,16 +292,14 @@
             namespace=passSecretObj.spec.managedSecret.metadata.namespace
         )
         log.info(f'Deleted PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}"')
     except client.ApiException as e:
         if e.status == HTTPStatus.NOT_FOUND:
             log.warning(f'PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" was not found. Skipping.')
         raise kopf.PermanentError(e)
-    finally:
-        _lift_passsecret_block(body)
 
 
 def check_gpg_id(path: Path | str, remove: bool =False) -> None:
     """
     Ensure the gpg ID exists (leftover from 'pass init' in the entrypoint, or a git clone) and its contents match PASS_GPG_KEY_ID.
 
     Args:
```

### Comparing `pass_operator-0.4.5/src/passoperator/git.py` & `pass_operator-0.4.6/src/passoperator/git.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.5/src/passoperator/gpg.py` & `pass_operator-0.4.6/src/passoperator/gpg.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.5/src/passoperator/secret.py` & `pass_operator-0.4.6/src/passoperator/secret.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.5/src/passoperator/utils.py` & `pass_operator-0.4.6/src/passoperator/utils.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.5/PKG-INFO` & `pass_operator-0.4.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pass-operator
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Kubernetes operator that syncs and decrypts secrets from pass store git repositories
 License: GPL-3.0-or-later
 Keywords: python,kubernetes,secrets,operator,pass
 Author: Emma Doyle
 Author-email: emma@premiscale.com
 Maintainer: Emma Doyle
 Maintainer-email: emma@premiscale.com
@@ -23,18 +23,14 @@
 Requires-Dist: python-gnupg (>=0.5.2,<0.6.0)
 Description-Content-Type: text/markdown
 
 # `pass` secrets operator
 
 ![GitHub Release](https://img.shields.io/github/v/release/premiscale/pass-operator)
 ![PyPI - License](https://img.shields.io/pypi/l/pass-operator)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pass-operator)
-![Docker Pulls](https://img.shields.io/docker/pulls/premiscale/pass-operator)
-![CircleCI](https://img.shields.io/circleci/build/github/premiscale/pass-operator)
-
 
 A Kubernetes operator to sync and decrypt secrets from a password store ([pass](https://www.passwordstore.org/)) Git repository. This operator is proposed as a proof-of-concept and shouldn't be used in any production capacity.
 
 While this approach to secrets management on Kubernetes is more technically challenging, the advantage is that we don't have to rely on a 3rd party SaaS platform, such as Vault or Doppler, to hold our secrets (the obvious benefits these platforms do provide, however, are better user and access management). We may also use this operator in an airgapped environment with a self-hosted git repository.
 
 <!--
 I also acknowledge that this approach swims against the DevSecOps tide in that it requires you to store your secrets (albeit encrypted)
@@ -46,15 +42,15 @@
 The following flowchart outlines how this operator reacts to `PassSecret`-related events and pass store updates.
 
 <p align="center" width="100%">
   <img width="100%" src="img/pass-operator-flow.png" alt="pass operator flow diagram">
 </p>
 
 From a high level, this operator runs `git pull` on an interval to grab updates from a git repository populated with encrypted
-secrets by `pass`. It maps secrets' paths to data values through the application of a [`PassSecret`](helm/operator/crds/PassSecret.yaml), a [custom resource](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/), such as the following.
+secrets by `pass`. It maps secrets' paths to data values through the application of a [`PassSecret`](helm/operator-crds/templates/PassSecret.yaml), a [custom resource](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/), such as the following.
 
 ```yaml
 apiVersion: secrets.premiscale.com/v1alpha1
 kind: PassSecret
 metadata:
   name: mysecret
   namespace: pass-operator-test
```

