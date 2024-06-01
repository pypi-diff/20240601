# Comparing `tmp/jaynes-0.9.8-py3-none-any.whl.zip` & `tmp/jaynes-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 40143 bytes, number of entries: 28
+Zip file size: 40690 bytes, number of entries: 28
 -rw-r--r--  2.0 unx      138 b- defN 21-Dec-28 04:17 jaynes/__init__.py
 -rw-r--r--  2.0 unx     3197 b- defN 21-Dec-28 04:17 jaynes/client.py
 -rw-r--r--  2.0 unx       40 b- defN 21-Dec-28 04:17 jaynes/constants.py
 -rw-r--r--  2.0 unx      721 b- defN 21-Dec-28 04:17 jaynes/daemon.py
 -rw-r--r--  2.0 unx      376 b- defN 21-Dec-28 04:17 jaynes/entry.py
 -rw-r--r--  2.0 unx     5180 b- defN 22-Sep-10 18:42 jaynes/gce_utils.py
 -rw-r--r--  2.0 unx     2767 b- defN 21-Dec-28 21:38 jaynes/helpers.py
 -rw-r--r--  2.0 unx    10791 b- defN 22-Sep-10 18:42 jaynes/jaynes.py
--rw-r--r--  2.0 unx    24723 b- defN 23-Apr-03 02:01 jaynes/mounts.py
+-rw-r--r--  2.0 unx    25214 b- defN 24-Jun-01 20:13 jaynes/mounts.py
 -rw-r--r--  2.0 unx      664 b- defN 21-Dec-28 04:17 jaynes/param_codec.py
--rw-r--r--  2.0 unx    20607 b- defN 23-Oct-19 19:14 jaynes/runners.py
+-rw-r--r--  2.0 unx    24080 b- defN 24-Jun-01 21:14 jaynes/runners.py
 -rw-r--r--  2.0 unx     4290 b- defN 22-Sep-10 18:42 jaynes/server.py
 -rw-r--r--  2.0 unx     1617 b- defN 23-Apr-08 16:31 jaynes/shell.py
--rw-r--r--  2.0 unx     5387 b- defN 21-Dec-28 04:17 jaynes/templates.py
+-rw-r--r--  2.0 unx     5488 b- defN 24-Jun-01 21:24 jaynes/templates.py
 -rw-r--r--  2.0 unx      211 b- defN 22-May-10 04:01 jaynes/launchers/__init__.py
--rw-r--r--  2.0 unx     5220 b- defN 23-Oct-17 01:46 jaynes/launchers/base_launcher.py
+-rw-r--r--  2.0 unx     4903 b- defN 24-Jun-01 21:23 jaynes/launchers/base_launcher.py
 -rw-r--r--  2.0 unx     3735 b- defN 22-Jan-12 15:01 jaynes/launchers/ec2_launch.py
 -rw-r--r--  2.0 unx     6997 b- defN 22-Jan-21 18:58 jaynes/launchers/gcp_launch.py
 -rw-r--r--  2.0 unx     2024 b- defN 22-Jun-17 15:54 jaynes/launchers/kube_launch.py
--rw-r--r--  2.0 unx     1387 b- defN 21-Dec-28 21:46 jaynes/launchers/local_launcher.py
+-rw-r--r--  2.0 unx     1227 b- defN 24-Jun-01 21:23 jaynes/launchers/local_launcher.py
 -rw-r--r--  2.0 unx     2104 b- defN 22-Jan-12 15:03 jaynes/launchers/manager_launch.py
--rw-r--r--  2.0 unx     4939 b- defN 21-Dec-28 22:16 jaynes/launchers/ssh_launch.py
+-rw-r--r--  2.0 unx     4837 b- defN 24-Jun-01 20:51 jaynes/launchers/ssh_launch.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Dec-28 04:17 jaynes/stale/__init__.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Oct-19 19:15 jaynes-0.9.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     8328 b- defN 23-Oct-19 19:15 jaynes-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-19 19:15 jaynes-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Oct-19 19:15 jaynes-0.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2198 b- defN 23-Oct-19 19:15 jaynes-0.9.8.dist-info/RECORD
-28 files, 118787 bytes uncompressed, 36657 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx     1047 b- defN 24-Jun-01 21:28 jaynes-0.9.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8329 b- defN 24-Jun-01 21:28 jaynes-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 21:28 jaynes-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Jun-01 21:28 jaynes-0.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2198 b- defN 24-Jun-01 21:28 jaynes-0.9.9.dist-info/RECORD
+28 files, 122274 bytes uncompressed, 37204 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -63,23 +63,23 @@
 
 Filename: jaynes/launchers/ssh_launch.py
 Comment: 
 
 Filename: jaynes/stale/__init__.py
 Comment: 
 
-Filename: jaynes-0.9.8.dist-info/LICENSE
+Filename: jaynes-0.9.9.dist-info/LICENSE
 Comment: 
 
-Filename: jaynes-0.9.8.dist-info/METADATA
+Filename: jaynes-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: jaynes-0.9.8.dist-info/WHEEL
+Filename: jaynes-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: jaynes-0.9.8.dist-info/top_level.txt
+Filename: jaynes-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: jaynes-0.9.8.dist-info/RECORD
+Filename: jaynes-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jaynes/mounts.py

```diff
@@ -1,13 +1,14 @@
 import os
 from os.path import join as pathJoin
 from textwrap import dedent
 from uuid import uuid4
 
 from jaynes.shell import check_call
+
 from .helpers import get_temp_dir
 
 
 class Mount:
     local_script = None
 
     # used by kubernetes
@@ -77,30 +78,48 @@
     :param acl: The ACL to set on the s3 object. When set to "public-read", the object will be publicly accessible.
                 This is needed for aws s3 download without credentials.
     :param no_sign: Whether to sign the s3 url. When set to true, the aws s3 download does not require credientials.
                     This needs to be used with the [acl: "public-read"] option.
     :return: self
     """
 
-    def __init__(self, *, prefix, local_path, host_path=None,
-                 volume=None, mount_path=None, sub_path=None,
-                 init_image="alpine:latest",
-                 init_image_pull_policy="IfNotPresent",
-                 init_image_pull_secret=None,
-                 remote_tar=None, container_path=None,
-                 docker_mount_type="bind",
-                 pypath=False, excludes=None, file_mask=None,
-                 name=None, compress=True, no_signin=False, acl=None, region=None,
-                 exclude_vcs=True, exclude_from=None, **tar_options):
+    def __init__(
+        self,
+        *,
+        prefix,
+        local_path,
+        host_path=None,
+        volume=None,
+        mount_path=None,
+        sub_path=None,
+        init_image="alpine:latest",
+        init_image_pull_policy="IfNotPresent",
+        init_image_pull_secret=None,
+        remote_tar=None,
+        container_path=None,
+        docker_mount_type="bind",
+        pypath=False,
+        excludes=None,
+        file_mask=None,
+        name=None,
+        compress=True,
+        no_signin=False,
+        acl=None,
+        region=None,
+        exclude_vcs=True,
+        exclude_from=None,
+        **tar_options,
+    ):
         # I fucking hate the behavior of python defaults. -- GY
         from .jaynes import RUN
+
         local_path = os.path.expandvars(local_path)
         local_abs = os.path.join(RUN.config_root, local_path)
 
-        tar_options = ' '.join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
+        tar_options = " ".join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
         if exclude_vcs:
             tar_options += " --exclude-vcs"
         if exclude_from:
             ignore_file_path = os.path.join(RUN.config_root, exclude_from)
             tar_options += f" --exclude-from='{ignore_file_path}'"
 
         name = name or str(uuid4())
@@ -155,23 +174,24 @@
         init_script = self.host_setup.strip()
         self.init_container = {
             "image": init_image,
             # fixme: hard-coded for now
             "imagePullPolicy": init_image_pull_policy,
             "name": name,
             "command": ["/bin/bash"],
-            "args": ['-c'] + [init_script],
+            "args": ["-c"] + [init_script],
             "volumeMounts": [
-                {"name": volume, "mountPath": mount_path, }
-            ]}
+                {
+                    "name": volume,
+                    "mountPath": mount_path,
+                }
+            ],
+        }
 
-        self.volume_mount = {
-            "name": volume,
-            "mountPath": self.container_path,
-            "subPath": sub_path}
+        self.volume_mount = {"name": volume, "mountPath": self.container_path, "subPath": sub_path}
 
 
 class GSCode(Mount):
     """
     Tars a local folder, uploads the content to Google Cloud Storage (GCS), downloads the tar ball
     on the remote instance and mounts it in docker.
 
@@ -204,27 +224,44 @@
     :param container_path: The path for the docker instance. Can be something like /Users/ge/project-folder/blah
     :param pypath (bool): Whether this directory should be added to the python path
     :param excludes: The files paths to exclude, default to "--exclude='*__pycache__'"
     :param file_mask: The file mask for files to include. Default to "."
     :return: self
     """
 
-    def __init__(self, *, prefix, local_path, host_path=None,
-                 volume=None, mount_path=None, sub_path=None, init_image="alpine:latest",
-                 init_image_pull_policy="IfNotPresent",
-                 remote_tar=None, container_path=None,
-                 docker_mount_type="bind",
-                 pypath=False, excludes=None, file_mask=None,
-                 name=None, compress=True, exclude_vcs=True, exclude_from=None, **tar_options):
+    def __init__(
+        self,
+        *,
+        prefix,
+        local_path,
+        host_path=None,
+        volume=None,
+        mount_path=None,
+        sub_path=None,
+        init_image="alpine:latest",
+        init_image_pull_policy="IfNotPresent",
+        remote_tar=None,
+        container_path=None,
+        docker_mount_type="bind",
+        pypath=False,
+        excludes=None,
+        file_mask=None,
+        name=None,
+        compress=True,
+        exclude_vcs=True,
+        exclude_from=None,
+        **tar_options,
+    ):
         # I fucking hate the behavior of python defaults. -- GY
         from .jaynes import RUN
+
         local_path = os.path.expandvars(local_path)
         local_abs = os.path.join(RUN.config_root, local_path)
 
-        tar_options = ' '.join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
+        tar_options = " ".join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
         if exclude_vcs:
             tar_options += " --exclude-vcs"
         if exclude_from:
             ignore_file_path = os.path.join(RUN.config_root, exclude_from)
             tar_options += f" --exclude-from='{ignore_file_path}'"
 
         name = name or str(uuid4())
@@ -279,23 +316,24 @@
 
         init_script = self.host_setup.strip()
         self.init_container = {
             "image": init_image,
             "imagePullPolicy": init_image_pull_policy,
             "name": name,
             "command": ["/bin/bash"],
-            "args": ['-c'] + [init_script],
+            "args": ["-c"] + [init_script],
             "volumeMounts": [
-                {"name": volume, "mountPath": mount_path, }
-            ]}
+                {
+                    "name": volume,
+                    "mountPath": mount_path,
+                }
+            ],
+        }
 
-        self.volume_mount = {
-            "name": volume,
-            "mountPath": self.container_path,
-            "subPath": sub_path}
+        self.volume_mount = {"name": volume, "mountPath": self.container_path, "subPath": sub_path}
 
 
 class S3Output(Mount):
     """
     Mounting a remote directory to docker, and upload it's content periodically to s3.
 
     **To Avoid downloading to local during startup**: set local to None
@@ -313,51 +351,54 @@
     :param local_path: When None, do not download those files
     :param interval:
     :param pypath:
     :param sync_s3:
     :return:
     """
 
-    def __init__(self, *, container_path, prefix, host_path=None, name=None, local_path=None, interval=15,
-                 pypath=False, sync_s3=True):
-
+    def __init__(self, *, container_path, prefix, host_path=None, name=None, local_path=None, interval=15, pypath=False, sync_s3=True):
         if host_path is None:
             host_path = f"/tmp/jaynes_mounts/{uuid4() if name is None else name}"
         else:
             assert os.path.isabs(host_path), "ATTENTION: host_path path has to be an absolute path."
 
         # used for getting the container log path
         self.host_path = host_path
 
-        assert os.path.isabs(container_path), \
-            "ATTENTION: docker path has to be absolute, to make sure your code knows where it is writing to."
+        assert os.path.isabs(
+            container_path
+        ), "ATTENTION: docker path has to be absolute, to make sure your code knows where it is writing to."
 
         if local_path:
             from .jaynes import RUN
+
             local_path = os.path.expandvars(local_path)
             local_abs = os.path.join(RUN.config_root, local_path)
 
             download_script = f"""
                 aws s3 cp --recursive {prefix} {local_path} || echo "s3 bucket is EMPTY" """
             self.local_script = f"""
                 mkdir -p {local_abs}
                 while true; do
                     echo "downloading..." {download_script}
                     {f"sleep {interval}" if interval else ""}
                 done & echo 'sync {local_path} initiated'
             """
         else:
-            print('S3UploadMount(**{}) generated no local_script.'.format(locals()))
+            print("S3UploadMount(**{}) generated no local_script.".format(locals()))
             # pass
         self.upload_script = f"""
                 aws s3 cp --recursive {host_path} {prefix} """  # --only-show-errors"""
         self.host_setup = f"""
                 echo 'making main_log directory {host_path}'
                 mkdir -p {host_path}
-                echo "made main_log directory" """ + ("" if not sync_s3 else f"""
+                echo "made main_log directory" """ + (
+            ""
+            if not sync_s3
+            else f"""
                 while true; do
                     echo "uploading..." {self.upload_script}
                     {f"sleep {interval}" if interval else ""}
                 done & echo "sync {host_path} initiated" 
                 while true; do
                     if [ -z $(curl -Is http://169.254.169.254/latest/meta-data/spot/termination-time | head -1 | grep 404 | cut -d \  -f 2) ]
                     then
@@ -365,15 +406,16 @@
                         break
                     else
                         # Spot instance not yet marked for termination. This is hoping that there's at least 3 seconds
                         # between when the spot instance gets marked for termination and when it actually terminates.
                         sleep 3
                     fi
                 done & echo main_log sync initiated
-                """)
+                """
+        )
         self.docker_mount = f"-v {host_path}:{container_path}"
         self.container_path = container_path
         self.pypath = pypath
 
 
 # New
 class SSHCode(Mount):
@@ -390,36 +432,50 @@
     :param container_path: The path for the docker instance. Can be something like /Users/ge/project-folder/blah
     :param pypath (bool): Whether this directory should be added to the python path
     :param excludes: The files paths to exclude, default to "--exclude='*__pycache__'"
     :param file_mask: The file mask for files to include. Default to "."
     :return: self
     """
 
-    def __init__(self, *, local_path, local_tar=None, host_path=None, remote_tar=None,
-                 container_path=None, pypath=False, excludes=None, file_mask=None, name=None,
-                 compress=True, exclude_vcs=True, exclude_from=None, **tar_options):
-
+    def __init__(
+        self,
+        *,
+        local_path,
+        local_tar=None,
+        host_path=None,
+        remote_tar=None,
+        container_path=None,
+        pypath=False,
+        excludes=None,
+        file_mask=None,
+        name=None,
+        compress=True,
+        exclude_vcs=True,
+        exclude_from=None,
+        **tar_options,
+    ):
         # I fucking hate the behavior of python defaults. -- GY
         self.local_path = local_path
         self.host_path = host_path
         self.container_path = container_path or host_path
         self.pypath = pypath
         name = name or str(uuid4())
         self.name = name
         self.compress = compress
 
         self.excludes = excludes or "--exclude='*__pycache__' --exclude='*.git' --exclude='*.idea' --exclude='*.egg-info'"
         self.file_mask = file_mask or "."  # file_mask can Not be None or "".
 
         from .jaynes import RUN
+
         local_path = os.path.expandvars(local_path)
         local_abs = os.path.join(RUN.config_root, local_path)
         self.container_path = os.path.join(RUN.config_root, container_path) if container_path else local_abs
 
-        tar_options = ' '.join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
+        tar_options = " ".join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
         if exclude_vcs:
             tar_options += " --exclude-vcs"
         if exclude_from:
             ignore_file_path = os.path.join(RUN.config_root, exclude_from)
             tar_options += f" --exclude-from='{ignore_file_path}'"
 
         if local_tar is None:
@@ -429,33 +485,33 @@
         else:
             tar_name = os.path.basename(local_tar)
             self.temp_dir = os.path.dirname(local_tar)
             self.local_tar = local_tar
 
         self.remote_tar = remote_tar or f"/tmp/{tar_name}"
 
-        self.tar_script = f"""
+        self.tar_script = dedent(f"""
                 type gtar >/dev/null 2>&1 && alias tar=`which gtar`
                 mkdir -p {self.temp_dir}
                 # Do not use absolute path in tar.
                 tar {self.excludes} {tar_options} -c{"z" if self.compress else ""}f {self.local_tar} -C {local_abs} {self.file_mask}
-                """
+                """)
 
-        self.host_setup = f"""
+        self.host_setup = dedent(f"""
                 mkdir -p {self.host_path}
                 tar -{"z" if self.compress else ""}xf {self.remote_tar}{tar_name if self.remote_tar.endswith('/') else ''} -C {self.host_path}
-                """
+                """)
         # used by the docker runner
         self.docker_mount = f"-v {self.host_path}:{self.container_path}"
 
     def upload(self, verbose=None, *, username, ip, pem=None, port=None, password=None, profile=None, **_):
         _port = "" if port is None else f"-p {port}"
         _pem = "" if pem is None else f"-i {pem}"
 
-        ssh_string = f"ssh {_port} {_pem}" if _port or _pem else 'ssh'
+        ssh_string = f"ssh {_port} {_pem}" if _port or _pem else "ssh"
         mkdir_script = f"{ssh_string} {username}@{ip} mkdir -p {os.path.dirname(self.remote_tar)}"
         rsync_script = f"rsync -az -e '{ssh_string}' --info=progress2 {self.local_tar} {username}@{ip}:{self.remote_tar}"
         if password is not None:  # note: now supports password log in!
             # rsync_script = f'expect <<EOF\nspawn {rsync_script};expect \"password:\";send \"{password}\\r\"\nEOF'
             # need to install sshpass from:
             # https://gist.github.com/arunoda/7790979
             mkdir_script = f"sshpass -p '{password}' {mkdir_script}"
@@ -470,33 +526,48 @@
         return super().upload(verbose=verbose)
 
 
 class TarMount(Mount):
     tar_path = None
     host_path = None
 
-    def __init__(self, *_, local_path, local_tar=None, remote_tar=None, host_path=None,
-                 container_path=None, pypath=False, name=None, excludes=None, file_mask=None,
-                 compress=True, exclude_vcs=True, exclude_from=None, **tar_options):
+    def __init__(
+        self,
+        *_,
+        local_path,
+        local_tar=None,
+        remote_tar=None,
+        host_path=None,
+        container_path=None,
+        pypath=False,
+        name=None,
+        excludes=None,
+        file_mask=None,
+        compress=True,
+        exclude_vcs=True,
+        exclude_from=None,
+        **tar_options,
+    ):
         self.local_path = local_path
         self.host_path = host_path
         self.container_path = container_path or host_path
         self.pypath = pypath
         name = name or str(uuid4())
         self.name = name
         self.compress = compress
 
         self.file_mask = file_mask or "."  # file_mask can Not be None or "".
         self.excludes = excludes or "--exclude='*__pycache__' --exclude='*.git' --exclude='*.idea' --exclude='*.egg-info'"
 
         from .jaynes import RUN
+
         local_path = os.path.expandvars(local_path)
         local_abs = os.path.join(RUN.config_root, local_path)
 
-        tar_options = ' '.join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
+        tar_options = " ".join([f"--{key.replace('_', '-')}={value}" for key, value in tar_options.items()])
         if exclude_vcs:
             tar_options += " --exclude-vcs"
         if exclude_from:
             ignore_file_path = os.path.join(RUN.config_root, exclude_from)
             tar_options += f" --exclude-from='{ignore_file_path}'"
 
         if local_tar is None:
@@ -521,32 +592,36 @@
                 tar -{"z" if compress else ""}xf {self.remote_tar} -C {host_path}
                 """
 
     def upload(self, verbose=None, *, host, user=None, token=None, **_):
         from jaynes.client import JaynesClient
 
         if os.path.exists(self.local_tar):
-            print('local tar already exists', self.local_tar)
+            print("local tar already exists", self.local_tar)
         else:
             script = dedent(self.local_script)
             check_call(script, verbose=verbose, shell=True)
 
         parent_dir = os.path.dirname(self.remote_tar)
         tar_name = os.path.basename(self.remote_tar)
 
         client = JaynesClient(host, token=token)
 
         # grep to speed up transmission
         stdout, stderr, error = client.execute(f"ls {parent_dir} | grep {tar_name}")
 
         if tar_name in stdout:
-            print('remote tar already exists', self.remote_tar)
+            print("remote tar already exists", self.remote_tar)
             return
 
         client.execute(f"mkdir -p {parent_dir}")
         client.upload_file(self.local_tar, self.remote_tar)
 
         stdout, *_ = client.execute(f"echo {parent_dir}")
         if verbose:
-            print(stdout, parent_dir, self.remote_tar, )
+            print(
+                stdout,
+                parent_dir,
+                self.remote_tar,
+            )
         stdout, *_ = client.execute(f"ls {parent_dir} | grep {tar_name}")
         assert tar_name in stdout, "file upload failed" + stdout
```

## jaynes/runners.py

```diff
@@ -1,16 +1,19 @@
 import os
 from copy import deepcopy
 from datetime import datetime
+from textwrap import dedent
 
 import jaynes
+
 from .constants import JAYNES_PARAMS_KEY
 from .param_codec import serialize
 
 
+# fmt: off
 def inline(script: str) -> str:
     script = script.strip()
     if not script:
         return ""
     return script if script.endswith(';') else f'{script};'
 
 
@@ -40,15 +43,15 @@
         self.entry_script = entry_script
         self.post_script = post_script
 
     @property
     def main_script_thunk(self):
         entry_env = f"{JAYNES_PARAMS_KEY}={{JYNS_encoded_thunk}}"
 
-        cmd = f"""printf "\\e[1;34m%-6s\\e[m\\n" "Running inside worker `hostname`" 1>&2;"""
+        cmd = """printf "\\e[1;34m%-6s\\e[m\\n" "Running inside worker `hostname`" 1>&2;"""
         if self.startup:
             cmd += inline(self.startup)
         if self.work_dir:
             cmd += f"""cd {self.work_dir};"""
         if self.pypath:
             cmd += f"PYTHONPATH=$PYTHONPATH:{self.pypath}"
         return f"{cmd} {entry_env} {self.entry_script}"
@@ -128,15 +131,15 @@
                  n_gpu=None, shell="/bin/sh", entry_script="python -u -m jaynes.entry",
                  partition=None, interactive=True, n_seq_jobs=1, time_limit: str = None, n_cpu=4, name=None,
                  comment=None, label=False, args=None,
                  post_script="", **options):
         super().__init__(mounts, work_dir, pypath, startup, entry_script, post_script)
 
         # --get-user-env
-        setup_cmd = f"""printf "\\e[1;34m%-6s\\e[m\\n" "Running on login-node `hostname`"\n"""
+        setup_cmd = """printf "\\e[1;34m%-6s\\e[m\\n" "Running on login-node `hostname`"\n"""
         setup_cmd += (setup.strip() + '\n') if setup else ''
         # remove
         # if pypath:
         #     setup_cmd += f"export PYTHONPATH=$PYTHONPATH:{pypath}"
 
         # some cluster only allows --gres=gpu:[1-]
         option_str = ""
@@ -147,15 +150,15 @@
         if n_cpu is not None:
             option_str += f" --cpus-per-task={n_cpu}"
         if n_gpu:
             option_str += f" --gres=gpu:{n_gpu}"
         if name:
             option_str += f' --job-name="{name}"'
         if label:
-            option_str += f" --label"
+            option_str += " --label"
         if comment:
             option_str += f' --comment="{comment}"'
 
         extra_options = " ".join([f'--{k.replace("_", "-")}="{v}"' for k, v in options.items()])
         if args:
             extra_options = "".join([f"--{a} " for a in args]) + extra_options
 
@@ -257,14 +260,105 @@
         self.run_script_thunk = f"""
             {setup or ""}
             {envs if envs else ""} {shell} -c '{{JYNS_main_script}}{pipe}'
             {cleanup}
             """
 
 
+# fmt: on
+class Tmux(Runner):
+    """
+    Tmux Runner
+
+    Example
+    -------
+
+    to configure the Docker runner in :code:`jaynes.yml`, you can do
+
+    .. code:: yaml
+
+        # ⬇️ this is a yaml syntax to select the class
+        runner: !runners.Docker
+            name: "some-job"  # only for docker
+            image: "episodeyang/super-expert"
+            startup: yes | pip install jaynes ml-logger -q
+            envs: "LANG=utf-8"
+            pypath: "{mounts[0].container_path}"
+            work_dir: "{mounts[0].container_path}"
+            ipc: host
+            use_gpu: false
+
+    :param mounts: list, reserved by jaynes to pass in the mount objects.
+    :param work_dir: this is the current work directory for the bash script.
+    :param setup: the script you want to run outside, before the tmux session
+    :param mounts:
+    :param pypath:
+    :param startup: the script you want to run first INSIDE tmux session
+    :param envs: Set of environment key and variables, a string
+    :param entry_script: "python -u -m jaynes.entry"
+    :param name: Name of the tmux session container instance, use uuid if is None
+                ssh/bash session is not going to be tty.
+    :param tmux_cmd: The tmux new-session command to use.
+    :param daemon: Default to True, run in the background when set.
+                Note: The Non-daemon mode is not supported, because I can't figure out ssh -t (tty) with this.
+
+    :param post_script: a script attached to after run_script
+    :param exit_session_when_done: exits the tmux session in daemon mode when it is done. Not used in interactive mode.
+    :param **kwargs: passed in as parameters to tmux session command.
+                memory="4g" gets translated into `--memory 4g`
+    """
+
+    def __init__(
+        self,
+        *,
+        mounts=None,
+        work_dir=None,
+        setup="",
+        startup=None,
+        pypath=None,
+        envs=None,
+        entry_script="python -u -m jaynes.entry",
+        name=None,
+        tmux_cmd="tmux new-session",
+        daemon=True,
+        # The Non-daemon mode is not supported, because I can't figure out ssh -t (tty) with this.
+        post_script="",
+        exit_session_when_done=False,
+        **options,
+    ):
+        super().__init__(mounts, work_dir, pypath, startup, entry_script, post_script)
+
+        self.setup_script = setup
+
+        # dynamically generate the job name to avoid conflict
+        job_name = name or f"jaynes-job-{datetime.utcnow():%H%M%S}-{jaynes.RUN.count}"
+
+        config = ""
+        for env_string in envs.strip().split(" "):
+            config += f"-e {env_string} "
+
+        rest_config = " ".join(f"--{k.replace('_', '-')}={v}" for k, v in options.items())
+
+        # note: there can not be end of line characters.
+        # fmt: off
+        self.run_script_thunk = dedent(f"""
+            printf "\e[1;34m%-6s\e[m\\n" "Launching tmux inside `hostname`"
+            {tmux_cmd}{' -d' if daemon else ''} -s '{job_name}' {config} {rest_config} bash -c '{{JYNS_main_script}}{" && exit" if exit_session_when_done else ""}'
+            printf "\e[1;34m%-6s\e[m\\n" "Launched session {job_name}"
+            """).strip()
+
+    chain = None
+    # def chain(self, fn, *args, __sep=" &\n", **kwargs):
+    #     encoded_thunk = serialize(fn, args, kwargs)
+    #     self.main_script = self.main_script_thunk.format(JYNS_encoded_thunk=encoded_thunk)
+    #     self.run_script += __sep + self.run_script_thunk.format(JYNS_main_script=self.main_script).strip()
+
+
+# fmt: off
+
 class Docker(Runner):
     """
     Docker Runner
 
     Example
     -------
 
@@ -308,15 +402,15 @@
                  pypath=None, envs=None, shell="/bin/sh", entry_script="python -u -m jaynes.entry", name=None,
                  docker_cmd="docker", ipc=None, tty=False, post_script="", net=None, **options):
         super().__init__(mounts, work_dir, pypath, startup, entry_script, post_script)
 
         mount_string = " ".join([m.docker_mount for m in mounts])
         self.setup_script = setup
 
-        is_gpu = options.get('gpus', None) or "nvidia" in docker_cmd
+        # is_gpu = options.get('gpus', None) or "nvidia" in docker_cmd
 
         # dynamically generate the job name to avoid conflict
         docker_container_name = name or f"jaynes-job-{datetime.utcnow():%H%M%S}-{jaynes.RUN.count}"
 
         remove_by_name = f"""
 echo -ne 'kill running instances '
 {docker_cmd} kill {docker_container_name}
@@ -332,32 +426,35 @@
         if net:
             options['net'] = net
         if ipc:
             options['ipc'] = ipc
 
         rest_config = " ".join(f"--{k.replace('_', '-')}={v}" for k, v in options.items())
 
-        test_gpu = f"""
-            echo 'Testing nvidia-smi inside docker'
-            {docker_cmd} run --rm {rest_config} {image} nvidia-smi
-            """
+        # test_gpu = f"""
+        #     echo 'Testing nvidia-smi inside docker'
+        #     {docker_cmd} run --rm {rest_config} {image} nvidia-smi
+        #     """
+
         # note: always connect the docker to stdin and stdout.
-        self.run_script_thunk = f"""
-{remove_by_name if name else ""}
-echo 'running {image} on' `hostname`
-{docker_cmd} run -i{"t" if tty else ""} {config} {rest_config} {mount_string} --name '{docker_container_name}' \\
-{image} {shell} -c '{{JYNS_main_script}} & wait' """
+        self.run_script_thunk = dedent(f"""
+            {remove_by_name if name else ""}
+            echo 'running {image} on' `hostname`
+            {docker_cmd} run -i{"t" if tty else ""} {config} {rest_config} {mount_string} --name '{docker_container_name}' \\
+            {image} {shell} -c '{{JYNS_main_script}} & wait' 
+            """).strip() # add strip to make this more robust, and dedent.
 
     chain = None
     # def chain(self, fn, *args, __sep=" &\n", **kwargs):
     #     encoded_thunk = serialize(fn, args, kwargs)
     #     self.main_script = self.main_script_thunk.format(JYNS_encoded_thunk=encoded_thunk)
     #     self.run_script += __sep + self.run_script_thunk.format(JYNS_main_script=self.main_script).strip()
 
 
+# fmt: on
 class Container(Runner):
     """
     Container Runner for Kubernetes
 
     Example
     -------
 
@@ -391,51 +488,59 @@
     :param ipc: specify ipc for multiprocessing. Typically 'host'
     :param net: for ec2, `--net host` allows docker to use the host's IAM for ec2 services
     :param tty: almost never used. This is because when this script is ran, it is almost guaranteed that the
                 ssh/bash session is not going to be tty.
     :param post_script: a script attached to after run_script
     :param **kwargs: Not used
     """
+
     job = None
 
-    def __init__(self, *, image,
-                 image_pull_policy="IfNotPresent",
-                 image_pull_secret=None,
-                 mounts=None,
-                 work_dir=None,
-                 workdir=None,
-                 setup="",
-                 startup=None,
-                 namespace=None,
-                 pypath=None,
-                 envs=None,
-                 shell="/bin/sh",
-                 entry_script="python -u -m jaynes.entry", name=None,
-                 docker_cmd="docker",
-                 ipc=None,
-                 tty=False,
-                 gpu=0,
-                 gpu_types=None,
-                 gpu_limit=0,
-                 post_script="",
-                 net=None,
-                 volumes=None,
-                 cpu="50m", mem="50Mi",
-                 cpu_limit=None, mem_limit=None,
-                 restart_policy="Never",
-                 backoff_limit=1,
-                 ttl_seconds_after_finished=3600,
-                 **options):
+    def __init__(
+        self,
+        *,
+        image,
+        image_pull_policy="IfNotPresent",
+        image_pull_secret=None,
+        mounts=None,
+        work_dir=None,
+        workdir=None,
+        setup="",
+        startup=None,
+        namespace=None,
+        pypath=None,
+        envs=None,
+        shell="/bin/sh",
+        entry_script="python -u -m jaynes.entry",
+        name=None,
+        docker_cmd="docker",
+        ipc=None,
+        tty=False,
+        gpu=0,
+        gpu_types=None,
+        gpu_limit=0,
+        post_script="",
+        net=None,
+        volumes=None,
+        cpu="50m",
+        mem="50Mi",
+        cpu_limit=None,
+        mem_limit=None,
+        restart_policy="Never",
+        backoff_limit=1,
+        ttl_seconds_after_finished=3600,
+        **options,
+    ):
         super().__init__(mounts, work_dir, pypath, startup, entry_script, post_script)
 
         # self.mounts reuses the mounts from the Runner class
         init_containers = [m.init_container for m in self.mounts]
         volume_mounts = [m.volume_mount for m in self.mounts]
 
-        self.is_gpu = options.get('gpus', None) or "nvidia" in docker_cmd
+        self.is_gpu = options.get("gpus", None) or "nvidia" in docker_cmd
 
         if not gpu_limit:
             gpu_limit = gpu
         if not cpu_limit:
             cpu_limit = cpu
         if not mem_limit:
             mem_limit = mem
@@ -468,53 +573,52 @@
                 "template": {
                     "spec": {
                         "volumes": volumes,
                         "initContainers": init_containers,
                         "containers": [],
                         "restartPolicy": restart_policy,
                     },
-
                 },
                 "backoffLimit": backoff_limit,
-                "ttlSecondsAfterFinished": ttl_seconds_after_finished
+                "ttlSecondsAfterFinished": ttl_seconds_after_finished,
             },
         }
         if image_pull_secret:
-            self.job_template['spec']['template']['spec']["imagePullSecrets"] = [{"name": image_pull_secret}]
+            self.job_template["spec"]["template"]["spec"]["imagePullSecrets"] = [{"name": image_pull_secret}]
 
         if gpu_types is not None:
-            affinity = {"nodeAffinity": {
-                "requiredDuringSchedulingIgnoredDuringExecution": {
-                    "nodeSelectorTerms": [{
-                        "matchExpressions": [{
-                            "key": "nvidia.com/gpu.product",
-                            "operator": "In",
-                            "values": gpu_types.split(',')
-                        }]
-                    }]
+            affinity = {
+                "nodeAffinity": {
+                    "requiredDuringSchedulingIgnoredDuringExecution": {
+                        "nodeSelectorTerms": [
+                            {"matchExpressions": [{"key": "nvidia.com/gpu.product", "operator": "In", "values": gpu_types.split(",")}]}
+                        ]
+                    }
                 }
-            }}
+            }
             self.job_template["spec"]["template"]["spec"]["affinity"] = affinity
 
     def build(self, fn, *args, __sep="\n", **kwargs):
         encoded_thunk = serialize(fn, args, kwargs)
         self.main_script = self.main_script_thunk.format(JYNS_encoded_thunk=encoded_thunk)
 
         if self.job is None:
             self.job = deepcopy(self.job_template)
 
         container = deepcopy(self.container_template)
-        container['command'].append(self.main_script)
-        self.job['spec']['template']['spec']['containers'].append(container)
+        container["command"].append(self.main_script)
+        self.job["spec"]["template"]["spec"]["containers"].append(container)
 
     def chain(self, fn, *args, __sep=" &\n", **kwargs):
         encoded_thunk = serialize(fn, args, kwargs)
         self.main_script = self.main_script_thunk.format(JYNS_encoded_thunk=encoded_thunk)
 
         assert self.job is not None
 
-        command_list = self.job['spec']['template']['spec']['containers'][-1]['command']
+        command_list = self.job["spec"]["template"]["spec"]["containers"][-1]["command"]
 
         if command_list[-1].endswith("& wait"):
             command_list[-1] = command_list[-1][:-6]
 
         command_list[-1] += "&\n" + self.main_script + "& wait"
+
+    # fmt: off
```

## jaynes/templates.py

```diff
@@ -1,40 +1,58 @@
+from textwrap import dedent
 import os
 from os.path import join as pathJoin
 
-ec2_tag_instance = lambda name: f"""
+
+def ec2_tag_instance(name):
+    return dedent(f"""
         if [ `cat /sys/devices/virtual/dmi/id/bios_version` == 1.0 ] || [[ -f /sys/hypervisor/uuid && `head -c 3 /sys/hypervisor/uuid` == ec2 ]]; then
             export REGION="$(wget -q -O - http://169.254.169.254/latest/meta-data/placement/region)"
             EC2_INSTANCE_ID="`wget -q -O - http://169.254.169.254/latest/meta-data/instance-id`"
             aws ec2 create-tags --resources $EC2_INSTANCE_ID --tags 'Key=Name,Value={name}' --region $REGION
         fi
-        """
-
-ec2_terminate = lambda delay=30: f"""
-            {f"sleep {delay}" if delay else ""}
-            die() {{ status=$1; shift; echo "FATAL: $*"; exit $status; }}
-            echo "Now terminate this instance"
-            export REGION="$(wget -q -O - http://169.254.169.254/latest/meta-data/placement/region)"
-            export EC2_INSTANCE_ID="`wget -q -O - http://169.254.169.254/latest/meta-data/instance-id || die "wget instance-id has failed: $?"`"
-            aws ec2 terminate-instances --instance-ids $EC2_INSTANCE_ID --region $REGION
-            """
-
-gce_terminate = lambda delay=30: f"""
-            {f"sleep {delay}" if delay else ""}
-            echo "Now terminate this instance"
-            export NAME=$(curl -X GET http://metadata.google.internal/computeMetadata/v1/instance/name -H 'Metadata-Flavor: Google')
-            export ZONE=$(curl -X GET http://metadata.google.internal/computeMetadata/v1/instance/zone -H 'Metadata-Flavor: Google')
-            gcloud --quiet compute instances delete $NAME --zone=$ZONE
-            """
+        """)
 
 
-def ssh_remote_exec(user, ip_address, script_path, port=None, pem=None,
-                    profile=None, password=None, require_password=False, sudo=True, remote_script_dir=None):
+def ec2_terminate(delay=30):
+    return dedent(f"""
+        {f"sleep {delay}" if delay else ""}
+        die() {{ status=$1; shift; echo "FATAL: $*"; exit $status; }}
+        echo "Now terminate this instance"
+        export REGION="$(wget -q -O - http://169.254.169.254/latest/meta-data/placement/region)"
+        export EC2_INSTANCE_ID="`wget -q -O - http://169.254.169.254/latest/meta-data/instance-id || die "wget instance-id has failed: $?"`"
+        aws ec2 terminate-instances --instance-ids $EC2_INSTANCE_ID --region $REGION
+        """)
+
+
+def gce_terminate(delay=30):
+    return dedent(f"""
+        {f"sleep {delay}" if delay else ""}
+        echo "Now terminate this instance"
+        export NAME=$(curl -X GET http://metadata.google.internal/computeMetadata/v1/instance/name -H 'Metadata-Flavor: Google')
+        export ZONE=$(curl -X GET http://metadata.google.internal/computeMetadata/v1/instance/zone -H 'Metadata-Flavor: Google')
+        gcloud --quiet compute instances delete $NAME --zone=$ZONE
+        """)
+
+
+def ssh_remote_exec(
+    user,
+    ip_address,
+    script_path,
+    port=None,
+    pem=None,
+    profile=None,
+    password=None,
+    require_password=False,
+    sudo=True,
+    remote_script_dir=None,
+    options="",
+):
     """
-    run script remotely via ssh agent. 
+    run script remotely via ssh agent.
 
     :param password: password, if the *ssh session* requires a password
     :param require_password: if the bash script that needs to be ran requires password
     :param user: username for the ssh login
     :param ip_address: address for the host
     :param pem: path to the public key for this login
 
@@ -72,26 +90,29 @@
                 for this.
 
                 question: what script name does this use?
 
     :return:
     """
 
-    options = "" if password is None else "-T "
-    options += "-o 'StrictHostKeyChecking=no'"
+    options = options or ""
+    options = options if password else f"{options} -T"
+    options += " -o 'StrictHostKeyChecking=no'"
 
     port_ = "" if port is None else f"-p {port}"
-    pem_ = f'-i {pem}' if pem else ''
-    sudo_ = 'sudo -n -s' if sudo else ""
+    pem_ = f"-i {pem}" if pem else ""
+    sudo_ = "sudo -n -s" if sudo else ""
     if remote_script_dir:  # `upload` mode
         assert os.path.isabs(remote_script_dir), "remote_script_dir need to be absolute"
         remote_path = pathJoin(remote_script_dir, os.path.basename(script_path))
         # this should be factorized out.
-        send_file = f"""ssh {options} {user}@{ip_address} {port_} {pem_} 'mkdir -p {remote_script_dir}'\n""" \
-                    f"""scp {port_.upper()} {pem_} {script_path} {user}@{ip_address}:{remote_script_dir}"""
+        send_file = dedent(f"""
+        ssh {options} {user}@{ip_address} {port_} {pem_} 'mkdir -p {remote_script_dir}'
+        scp {port_.upper()} {pem_} {script_path} {user}@{ip_address}:{remote_script_dir}
+        """)
         if profile:
             launch = f'''ssh {options} {user}@{ip_address} {port_} {pem_} "sudo {"-kS " if require_password else ""}su - {profile}; {sudo_} bash {remote_path}"'''
         else:
             launch = f"""ssh {options} {user}@{ip_address} {port_} {pem_} '{sudo_} bash {remote_path}'"""
         if password is not None:
             send_file = f"sshpass -p '{password}' {send_file}"
             launch = f"sshpass -p '{password}' {launch}"
```

## jaynes/launchers/base_launcher.py

```diff
@@ -50,45 +50,46 @@
     :param _:
     :return:
     """
     # the log_dir is primarily used for the run script. Therefore it should use ued here instead.
     log_path = os.path.join(launch_dir, "jaynes-launch.log")
     error_path = os.path.join(launch_dir, "jaynes-launch.err.log")
 
-    all_setup = "\n".join(
-        [m.host_setup for m in mounts if hasattr(m, "host_setup") and m.host_setup]
-    )
+    all_setup = "\n".join([m.host_setup for m in mounts if hasattr(m, "host_setup") and m.host_setup])
 
     host_unpack_script = dedent(f"""
-        #!/bin/bash
-        # to allow process substitution
-        set +o posix
-        {root_config or ""}
-        mkdir -p {launch_dir}
-        {{
-            {all_setup}
-            {f"sleep {delay}" if delay else ""}
-        }} > >(tee -a {log_path}) 2> >(tee -a {error_path} >&2)
-        """).strip()
+#!/bin/bash
+# to allow process substitution
+set +o posix
+{root_config or ""}
+mkdir -p {launch_dir}
+{{
+    {all_setup}
+    {f"sleep {delay}" if delay else ""}
+}} > >(tee -a {log_path}) 2> >(tee -a {error_path} >&2)
+""").strip()
 
     return host_unpack_script
 
 
 # noinspection PyShadowingBuiltins
-def make_launch_script(runners: Tuple[Runner],
-                       mounts: Sequence[Mount],
-                       unpack_on_host: Union[bool, None],
-                       type: str,
-                       launch_dir="~/jaynes-launch",
-                       pipe_out: bool = None,
-                       setup: str = None,
-                       terminate_after=False,
-                       delay: float = None,
-                       instance_name: str = None,
-                       root_config: dict = None, **_):
+def make_launch_script(
+    runners: Tuple[Runner],
+    mounts: Sequence[Mount],
+    unpack_on_host: Union[bool, None],
+    type: str,
+    launch_dir="~/jaynes-launch",
+    pipe_out: bool = None,
+    setup: str = None,
+    terminate_after=False,
+    delay: float = None,
+    instance_name: str = None,
+    root_config: dict = None,
+    **_,
+):
     """
     function to make the host script
 
     :param type:
     :param root_config:
     :param setup:
     :param pipe_out:
@@ -100,31 +101,27 @@
     :param launch_dir:
     :param terminate_after:
     :param delay:
     :param instance_name: less than 128 ascii characters
     :return:
     """
     log_setup = dedent(f"""
-        mkdir -p {launch_dir}
-        JAYNES_LAUNCH_DIR={launch_dir}
-        """)
+mkdir -p {launch_dir}
+JAYNES_LAUNCH_DIR={launch_dir}
+""").strip()
 
     if not pipe_out:
         log_path = os.path.join(launch_dir, "jaynes-launch.log")
         error_path = os.path.join(launch_dir, "jaynes-launch.err.log")
         pipe_out = pipe_out or f""" > >(tee -a {log_path}) 2> >(tee -a {error_path} >&2)"""
 
-    upload_script = '\n'.join(
-        [m.upload_script for m in mounts if hasattr(m, "upload_script") and m.upload_script]
-    )
+    upload_script = "\n".join([m.upload_script for m in mounts if hasattr(m, "upload_script") and m.upload_script])
     # does not unpack if the self.host_unpack_script has already been generated.
     if unpack_on_host:
-        host_unpack_script = "\n".join(
-            [m.host_setup for m in mounts if hasattr(m, "host_setup") and m.host_setup]
-        )
+        host_unpack_script = "\n".join([m.host_setup for m in mounts if hasattr(m, "host_setup") and m.host_setup])
     else:
         host_unpack_script = ""
     if instance_name:
         assert len(instance_name) <= 128, "Error: ws limits instance tag to 128 unicode characters."
 
     # NOTE: path.join is running on local computer, so it might not be quite right if remote is say windows.
     # NOTE: dedent is required by aws EC2.
@@ -142,15 +139,15 @@
     if len(runners) == 1:
         run_scripts = runners[0].run_script.strip()
     else:
         # todo: does not return the correct exit code.
         run_scripts = " & \n".join([r.run_script.strip() for r in runners] + ["wait"])
     post_scripts = "\n".join([r.post_script for r in runners])
 
-    return f"""
+    return dedent(f"""
 #!/bin/bash
 # to allow process substitution
 set +o posix
 {root_config or ''}
 {log_setup or ''}
 {{
 # launch.setup script
@@ -163,8 +160,8 @@
 {setup_scripts}
 # run script
 {run_scripts}
 # post script
 {post_scripts}
 {terminate_commands}
 }} {pipe_out or ""}
-""".strip()
+""").strip()
```

## jaynes/launchers/local_launcher.py

```diff
@@ -14,30 +14,30 @@
         [m.upload_script for m in mounts if hasattr(m, "upload_script") and m.upload_script]
     )
     host_setup = "" if not unpack_host else "\n".join(
         [m.host_setup for m in mounts if hasattr(m, "host_setup") and m.host_setup]
     )
 
     remote_script = dedent(f"""
-        #!/bin/bash
-        # to allow process substitution
-        set +o posix
-        {root_config or ""}
-        mkdir -p {log_dir}
-        {{
-            {host_setup}
+#!/bin/bash
+# to allow process substitution
+set +o posix
+{root_config or ""}
+mkdir -p {log_dir}
+{{
+{host_setup}
 
-            # upload_script
-            {upload_script}
+# upload_script
+{upload_script}
 
-            {runners[0].setup_script}
-            {runners[0].run_script}
-            {runners[0].post_script}
-            
-            {f"sleep {delay}" if delay else ""}
-        }} > >(tee -a {log_path}) 2> >(tee -a {error_path} >&2)
-        """).strip()
+{runners[0].setup_script}
+{runners[0].run_script}
+{runners[0].post_script}
+
+{f"sleep {delay}" if delay else ""}
+}} > >(tee -a {log_path}) 2> >(tee -a {error_path} >&2)
+""").strip()
     if verbose:
         print(remote_script)
     if not dry:
         return check_call(remote_script, shell=True)
     return
```

## jaynes/launchers/ssh_launch.py

```diff
@@ -5,17 +5,31 @@
 
 from jaynes.helpers import omit
 from jaynes.launchers.base_launcher import Launcher, make_host_unpack_script, make_launch_script
 from jaynes.shell import check_call
 from jaynes.templates import ssh_remote_exec
 
 
-def ssh(script, ip, port=None, username="ubuntu", pem=None, profile=None,
-        password=None, sudo=False, cleanup=True, block=False, console_mode=False, dry=False,
-        verbose=False, **_):
+def ssh(
+    script,
+    ip,
+    port=None,
+    username="ubuntu",
+    pem=None,
+    profile=None,
+    password=None,
+    sudo=False,
+    cleanup=True,
+    block=False,
+    console_mode=False,
+    dry=False,
+    verbose=False,
+    options="",
+    **_,
+):
     """
     run launch_script remotely by ip_address. First saves the run script locally as a file, then use
     scp to transfer the script to remote instance then run.
 
     :param username:
     :param ip:
     :param port:
@@ -30,33 +44,39 @@
     :param password: The password for the user in case it is needed.
     :param dry:
     :param verbose:
     :return:
     """
     # todo: is this still used?
     tf = tempfile.NamedTemporaryFile(prefix="jaynes_launcher-", suffix=".sh", delete=False)
-    with open(tf.name, 'w') as f:
-        _ = os.path.basename(tf.name)  # fixit: does kill require sudo?
+    with open(tf.name, "w") as f:
+        bname = os.path.basename(tf.name)  # fixit: does kill require sudo?
         cleanup_script = dedent(f"""
-            PROCESSES=$(ps aux | grep '[{_[0]}]{_[1:]}' | awk '{{print $2}}')
+            PROCESSES=$(ps aux | grep '[{bname[0]}]{bname[1:]}' | awk '{{print $2}}')
             if [ $PROCESSES ] 
             then
             {"sudo " if sudo else ""}kill $PROCESSES
-            {f"echo 'cleaned up after {_}" if verbose else ""}
+            {f"echo 'cleaned up after {bname}" if verbose else ""}
             fi 
             """)
         f.write(script + cleanup_script if cleanup else "")
     tf.file.close()
 
-    prelaunch_upload_script, launch = ssh_remote_exec(username, ip, tf.name,
-                                                      port=port, pem=pem,
-                                                      profile=profile,
-                                                      password=password,
-                                                      require_password=(profile is not None),
-                                                      sudo=sudo)
+    prelaunch_upload_script, launch = ssh_remote_exec(
+        username,
+        ip,
+        tf.name,
+        port=port,
+        pem=pem,
+        profile=profile,
+        password=password,
+        require_password=(profile is not None),
+        sudo=sudo,
+        options=options,
+    )
 
     # todo: use pipe back to send binary from RPC calls
     if dry:
         if prelaunch_upload_script:
             print("script upload:\n", prelaunch_upload_script)
         print("launch script:\n", launch)
         return
@@ -69,30 +89,31 @@
             p.communicate(bytes(f"{password}\n"))
 
     pipe_in = "" if profile is None else f"{password}\n"
     if not prelaunch_upload_script:
         pipe_in = pipe_in + script + "\n"
 
     if verbose:
-        print('ssh pipe-in: ')
+        print(">> launch script is")
+        print(launch)
+        print(">> ssh pipe-in: ")
         print(pipe_in)
 
     import subprocess
+
     if block:
         # todo: not supported. stdout, stderr, requires subprocess.PIPE for the two.
-        p = subprocess.Popen(launch, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
-                             stderr=subprocess.PIPE)
-        return p.communicate(bytes(pipe_in, 'utf-8'))
+        p = subprocess.Popen(launch, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        return p.communicate(bytes(pipe_in, "utf-8"))
     elif console_mode:
-        p = subprocess.Popen(launch, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
-                             stderr=subprocess.PIPE)
+        p = subprocess.Popen(launch, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     else:
         p = subprocess.Popen(launch, shell=True, stdin=subprocess.PIPE, stdout=sys.stdout, stderr=sys.stderr)
 
-    p.stdin.write(bytes(pipe_in, 'utf-8'))
+    p.stdin.write(bytes(pipe_in, "utf-8"))
     p.stdin.flush()
 
 
 class SSH(Launcher):
     # Not need in GCP launch or EC2 launcher.
     host_unpacked = False
     launch_script = None
@@ -101,23 +122,23 @@
         if self.host_unpacked:
             return
         self.host_unpacked = True
 
         unpack_script = make_host_unpack_script(mounts=self.all_mounts, **self.config)
 
         if verbose:
-            print('Unpacking On Remote')
-        ssh(script=unpack_script, **omit(self.config, 'block'), block=True,
-            verbose=verbose)
+            print("Unpacking On Remote")
+        ssh(script=unpack_script, **omit(self.config, "launch_dir", "type", "block"), block=True, verbose=verbose)
 
     # SSH does not support planning ahead.
     def plan_instance(self, verbose=None):
         pass
 
     def execute(self, verbose=None):
-        self.launch_script = make_launch_script(runners=self.runners, mounts=self.all_mounts,
-                                                unpack_on_host=self.host_unpacked, **self.config)
+        self.launch_script = make_launch_script(
+            runners=self.runners, mounts=self.all_mounts, unpack_on_host=self.host_unpacked, **self.config
+        )
         self.runners.clear()
         if verbose:
             print(self.launch_script)
 
         return ssh(self.launch_script, **self.config)
```

## Comparing `jaynes-0.9.8.dist-info/LICENSE` & `jaynes-0.9.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jaynes-0.9.8.dist-info/METADATA` & `jaynes-0.9.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaynes
-Version: 0.9.8
+Version: 0.9.9
 Summary: A tool for running python code with runner on aws
 Home-page: https://github.com/episodeyang/jaynes
 Author: Ge Yang
 Author-email: yangge1987@gmail.com
 License: Copyright 2022 Ge Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -23,15 +23,15 @@
 Requires-Dist: functional-notations
 Requires-Dist: params-proto >=2.10.0
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: termcolor
 
 Jaynes, A Utility for training ML models on AWS, GCE, SLURM, with or without docker 
-===================================================================================
+====================================================================================
 
 |Downloads|
 
 Overview
 --------
 
 The reality of ML training in universities is that we use what ever
```

## Comparing `jaynes-0.9.8.dist-info/RECORD` & `jaynes-0.9.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 jaynes/client.py,sha256=phuxy9aGNB2UfUpmtafUz_ielK4U0yWPb7K-dEZsU0Q,3197
 jaynes/constants.py,sha256=FI2l_bI8Zs2ftEB6l5BrG6ly3jhInTlkiYhKam0x_BM,40
 jaynes/daemon.py,sha256=57WWnRYqRnjEmg0K5bdUnt1LDIN2gCrgCZ_agzlkeVg,721
 jaynes/entry.py,sha256=GpK811zV6vMeOVpkhkAnPCBhguTJNc0dnuhDegoQwpo,376
 jaynes/gce_utils.py,sha256=dLdZwPKl123TXZm1rMLfWlEHoefwCJ24-TfuJBPT32g,5180
 jaynes/helpers.py,sha256=K6wxDgXBhvMCCrfgap_nmQF1CEyDByfbVmX9kZNMPuw,2767
 jaynes/jaynes.py,sha256=YNoVh-BfqeWZBvQrXYTHw7bFbDS6_MC75IhQ9eBXw-E,10791
-jaynes/mounts.py,sha256=nwptQ8o0Q-oFEAT7kjoVT1dufn4HY15A2gqgxfRY41Y,24723
+jaynes/mounts.py,sha256=m-58LX9-jEW_tT0nCqt73LIakXvuD7upBTOKmZpKZBE,25214
 jaynes/param_codec.py,sha256=eBG532ixzzcibOx95S98CVy6fZQKUvRXHG45wxsE0vw,664
-jaynes/runners.py,sha256=8KWbC8YB2tQC4ZBgR-mlPDUGvfECwXmDcEKsNhfv76U,20607
+jaynes/runners.py,sha256=TvMAMONsS3VI4XGlJwSQPidejdtlkBxsYM_F19tJR4g,24080
 jaynes/server.py,sha256=k3ZoZcuOpMs6xhR-bA5H2BRv-r-RTNd-uMOWQEGb8co,4290
 jaynes/shell.py,sha256=bU-8biTC09SH4Fn1NFonwKZnCiZhEX-KhePbCW-gwVE,1617
-jaynes/templates.py,sha256=Tb8b_z3p82nl-fBoF-3qvVsWy7TEpXDTh7Qod3e469U,5387
+jaynes/templates.py,sha256=i-zVdTlBhev5l6bSZmgXiEFhme3PWsP60w24Ha-3kHQ,5488
 jaynes/launchers/__init__.py,sha256=VuDftYyG8ue7f8-L9XmDjkizVpomKMat5bonVPmQaxE,211
-jaynes/launchers/base_launcher.py,sha256=3zQy2sZ7Xkl3ye-NV8JDy23VVuxJ2ZMX_UNGIoaDxZ4,5220
+jaynes/launchers/base_launcher.py,sha256=86PoleF2pC9IvWGpDAipXm86pFfb-6YieZLjYY5kiqY,4903
 jaynes/launchers/ec2_launch.py,sha256=kaoDp6SywgkcJYm0uZJTV3UUePXrWxzY3dLzi6m_D1I,3735
 jaynes/launchers/gcp_launch.py,sha256=2tgIkweroSiC9U4LebWqfAkukMSCJe7FnxY69m6EQ-k,6997
 jaynes/launchers/kube_launch.py,sha256=Bvt_cGblAvxWfkglo-TIsKwH8bIt2fuep4OvYgB9Zes,2024
-jaynes/launchers/local_launcher.py,sha256=xO0IHWF2ivfjT41tra5-6QPKB6bXkkwW5QD81w2ZRow,1387
+jaynes/launchers/local_launcher.py,sha256=29FIEHlRvQtvTYt0kDv-x4YHVpJScVtIo9UWgZxyi2Q,1227
 jaynes/launchers/manager_launch.py,sha256=krq6adiHee1DI2iWbahZM9tZkhCHUQBxtS3NYy76QkY,2104
-jaynes/launchers/ssh_launch.py,sha256=GzAIotYD3rWZcz-CzSLMTflZJyuygiaQEw88gPa36ac,4939
+jaynes/launchers/ssh_launch.py,sha256=hiJucE5x3YGpZ6dCuKAZZZgaLT92WGrFISi7_rf33MY,4837
 jaynes/stale/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jaynes-0.9.8.dist-info/LICENSE,sha256=7aeBUFBrKApC7DJHqrnGsPuy6pvZegzaTT-iJERVSW0,1047
-jaynes-0.9.8.dist-info/METADATA,sha256=cRbcUu74Zb7l1R_TW8lOM9xXetnvbDNhaNkwNd_fMDk,8328
-jaynes-0.9.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-jaynes-0.9.8.dist-info/top_level.txt,sha256=BqdlhoNVrrByJ8bJYMoZAavY4mca0lxO15ad4EGWqhY,7
-jaynes-0.9.8.dist-info/RECORD,,
+jaynes-0.9.9.dist-info/LICENSE,sha256=7aeBUFBrKApC7DJHqrnGsPuy6pvZegzaTT-iJERVSW0,1047
+jaynes-0.9.9.dist-info/METADATA,sha256=0ODWzPMhroHS_-Llij99qPj6YS_TK32ukRcRDyqvDq0,8329
+jaynes-0.9.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+jaynes-0.9.9.dist-info/top_level.txt,sha256=BqdlhoNVrrByJ8bJYMoZAavY4mca0lxO15ad4EGWqhY,7
+jaynes-0.9.9.dist-info/RECORD,,
```

