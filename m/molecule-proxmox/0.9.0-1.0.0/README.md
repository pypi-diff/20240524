# Comparing `tmp/molecule-proxmox-0.9.0.tar.gz` & `tmp/molecule_proxmox-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-proxmox-0.9.0.tar", last modified: Tue Jan  2 21:30:50 2024, max compression
+gzip compressed data, was "molecule_proxmox-1.0.0.tar", last modified: Fri May 24 13:46:18 2024, max compression
```

## Comparing `molecule-proxmox-0.9.0.tar` & `molecule_proxmox-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1122 2022-01-25 16:08:55.000000 molecule-proxmox-0.9.0/LICENSE
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       77 2022-01-25 16:05:10.000000 molecule-proxmox-0.9.0/MANIFEST.in
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     6071 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/PKG-INFO
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     5599 2024-01-02 20:16:10.000000 molecule-proxmox-0.9.0/README.rst
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       38 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/setup.cfg
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1220 2024-01-02 20:50:42.000000 molecule-proxmox-0.9.0/setup.py
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/molecule_proxmox/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       22 2024-01-02 21:02:30.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/__init__.py
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/molecule_proxmox/cookiecutter/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      107 2022-01-25 16:07:10.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/cookiecutter/cookiecutter.json
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      110 2022-01-25 22:32:46.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     3876 2024-01-02 17:45:01.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/driver.py
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/molecule_proxmox/modules/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        0 2022-01-29 05:50:49.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/modules/__init__.py
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     6893 2022-05-20 13:00:17.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/molecule_proxmox/playbooks/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     4207 2023-04-17 19:56:35.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/playbooks/create.yml
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1666 2022-05-20 13:00:17.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/playbooks/destroy.yml
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      851 2023-04-17 19:15:49.000000 molecule-proxmox-0.9.0/src/molecule_proxmox/playbooks/prepare.yml
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/
--rw-r--r--   0 mmeffie   (1001) mmeffie   (1001)     6071 2024-01-02 21:30:50.000000 molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/PKG-INFO
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      783 2024-01-02 21:30:50.000000 molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/SOURCES.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        1 2024-01-02 21:30:50.000000 molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/dependency_links.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       60 2024-01-02 21:30:50.000000 molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/entry_points.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       40 2024-01-02 21:30:50.000000 molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/requires.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       17 2024-01-02 21:30:50.000000 molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/top_level.txt
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-01-02 21:30:50.165315 molecule-proxmox-0.9.0/tests/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1176 2024-01-02 19:02:16.000000 molecule-proxmox-0.9.0/tests/test_proxmox_driver.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1122 2022-01-25 16:08:55.000000 molecule_proxmox-1.0.0/LICENSE
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       77 2022-01-25 16:05:10.000000 molecule_proxmox-1.0.0/MANIFEST.in
+-rw-r--r--   0 mmeffie   (1001) mmeffie   (1001)     6577 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/PKG-INFO
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     5866 2024-05-03 12:15:40.000000 molecule_proxmox-1.0.0/README.rst
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       38 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/setup.cfg
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1371 2024-05-03 12:21:29.000000 molecule_proxmox-1.0.0/setup.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.720567 molecule_proxmox-1.0.0/src/
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/src/molecule_proxmox/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       22 2024-05-24 11:43:36.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/__init__.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/src/molecule_proxmox/cookiecutter/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      107 2022-01-25 16:07:10.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/cookiecutter/cookiecutter.json
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.720567 molecule_proxmox-1.0.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      110 2022-01-25 22:32:46.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     3919 2024-05-02 15:23:06.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/driver.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/src/molecule_proxmox/modules/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        0 2022-01-29 05:50:49.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/modules/__init__.py
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     7054 2024-05-02 15:23:06.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/src/molecule_proxmox/playbooks/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     4440 2024-05-02 15:23:06.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/playbooks/create.yml
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1714 2024-05-02 15:23:06.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/playbooks/destroy.yml
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      960 2024-05-02 15:23:06.000000 molecule_proxmox-1.0.0/src/molecule_proxmox/playbooks/prepare.yml
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/
+-rw-r--r--   0 mmeffie   (1001) mmeffie   (1001)     6577 2024-05-24 13:46:18.000000 molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/PKG-INFO
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      783 2024-05-24 13:46:18.000000 molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        1 2024-05-24 13:46:18.000000 molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       60 2024-05-24 13:46:18.000000 molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/entry_points.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       40 2024-05-24 13:46:18.000000 molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/requires.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       17 2024-05-24 13:46:18.000000 molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/top_level.txt
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2024-05-24 13:46:18.724567 molecule_proxmox-1.0.0/tests/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1205 2024-05-02 15:23:06.000000 molecule_proxmox-1.0.0/tests/test_proxmox_driver.py
```

### Comparing `molecule-proxmox-0.9.0/LICENSE` & `molecule_proxmox-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-proxmox-0.9.0/PKG-INFO` & `molecule_proxmox-1.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,14 @@
-Metadata-Version: 2.1
-Name: molecule-proxmox
-Version: 0.9.0
-Summary: Proxmox Molecule Plugin :: run molecule tests using proxmox
-Home-page: https://github.com/meffie/molecule-proxmox
-Author: Michael Meffie
-Author-email: mmeffie@sinenomine.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ***********************
 Molecule Proxmox Plugin
 ***********************
 
-This is an experimental Ansible Molecule Driver plugin to manage instances on a
+This is an Ansible Molecule Driver plugin to manage instances on a
 `Proxmox VE`_ hypervisor cluster.  Only virtual machines are supported at this
-time.  Proxmox containers will be supported in a future release.
+time.
 
 Requirements
 ============
 
 * Access to a `Proxmox VE`_ cluster
 * One or more virtual machine templates with required setup
 * Python package `proxmoxer`_
@@ -60,57 +46,63 @@
 The ``molecule-proxmox`` plugin may be installed with Python ``pip``. A virtualenv
 is recommended.  The following commands install Ansible, Molecule, and the
 Molecule Proxmox plugin in a virtualenv called ``venv``.
 
 .. code-block:: bash
 
     $ python3 -m venv venv
-    $ source venv/bin/activate
-    $ pip3 install molecule[ansible] molecule-proxmox
-
+    $ . venv/bin/activate
+    $ pip3 install ansible-core molecule molecule-proxmox
 
-Example
-=======
+Examples
+========
 
 .. code-block:: yaml
 
    driver:
      name: molecule-proxmox
      options:
-        api_host: pve01.example.com
-        api_user: molecule
+        api_host: <hostname>        # e.g. pve01.example.com
+        api_user: <name>@<realm>    # e.g. root@pam
         api_password: "********"
         node: pve01
         ssh_user: tester
         ssh_identity_file: /path/to/id_rsa
-        template_name: debian11
-        sethostname: yes
    platforms:
      - name: test01
        template_name: debian11
      - name: test02
        template_name: alma8
 
 .. code-block:: yaml
 
    driver:
      name: molecule-proxmox
      options:
-        api_host: pve01.example.com
-        api_user: molecule
+        api_host: <hostname>        # e.g. pve01.example.com
+        api_user: <name>@<realm>    # e.g. root@pam
+        # Optional: Use an API token for Proxmox authentication.
         api_token_id: "********"
         api_token_secret: "*******************************"
         node: pve01
         ssh_user: tester
         ssh_identity_file: /path/to/id_rsa
+        # Optional: The default template name.
         template_name: debian11
+        # Optional: Set the hostname after cloning.
+        sethostname: yes
+        # Optional: Create the VMs in the pool.
+        pool: test
    platforms:
      - name: test01
+       # Optional: Specify the VM id of the clone.
+       newid: 216
      - name: test02
-       sethostname: no
+       # Optional: Specify the VM id of the clone.
+       newid: 217
 
 .. code-block:: yaml
 
    driver:
      name: molecule-proxmox
      options:
         # Secrets file may be encrypted with ansible-vault.
@@ -152,39 +144,40 @@
 To checkout the source code:
 
 .. code-block:: bash
 
     $ git clone https://github.com/meffie/molecule-proxmox
     $ cd molecule-proxmox
 
-A `Makefile` is provided to facilitate development and testing. A Python
-virtualenv environment may be created with the `init` target.
+A `Makefile` and `tox.ini` are provided to facilitate development and testing.
+A Python virtualenv environment may be created with the `init` target.
 
 .. code-block:: bash
 
     $ make init
     $ source .venv/bin/activate
 
 Export the following shell environment variables to run the unit tests.
 
 .. code-block:: bash
 
-    export PROXMOX_SECRETS=<proxmox secrets yaml file path>
+    # Connection info:
+    export PROXMOX_HOST=<proxmox hostname>
+    export PROXMOX_USER=<username@realm>   # e.g. root@pam
+    export PROXMOX_PASSWORD=<password>
+    export PROXMOX_TOKEN_ID=<id>
+    export PROXMOX_TOKEN_SECRET=<secret>
     export PROXMOX_NODE=<proxmox node name>
     export PROXMOX_SSH_USER=<username>
     export PROXMOX_SSH_IDENTITY_FILE=<ssh key file for username>
+
+    # Template id and names for unit tests:
     export PROXMOX_TEMPLATE_VMID=<template vmid to be cloned in by-vmid scenario>
     export PROXMOX_TEMPLATE_NAME=<template name to be cloned in by-name scenario>
 
-The secrets file should contain the proxmox login credentials, either the
-username and password, or a Proxmox API token id and value.  This file should
-be encrypted with `ansible-vault`. The ssh user and identity file should match
-the user and public key installed when the virtual machine template was
-created.
-
 To run the unit tests in verbose mode:
 
 .. code-block:: bash
 
     $ make test
 
 To run the unit tests in quiet mode:
```

### Comparing `molecule-proxmox-0.9.0/setup.py` & `molecule_proxmox-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,18 +23,21 @@
     entry_points={
         'molecule.driver': [
             'proxmox = molecule_proxmox.driver:Proxmox',
         ],
     },
     install_requires=[
         # molecule plugins are not allowed to mention Ansible as a direct dependency
-        'molecule>=4.0.1',
-        'pyyaml',
+        'molecule>=6.0.0',
+        'PyYAML',
         'proxmoxer>=1.3.1',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.10',
 )
```

### Comparing `molecule-proxmox-0.9.0/src/molecule_proxmox/driver.py` & `molecule_proxmox-1.0.0/src/molecule_proxmox/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,27 +88,27 @@
             d = self._get_instance_config(instance_name)
             return {
                 "ansible_user": d["user"],
                 "ansible_host": d["address"],
                 "ansible_port": d["port"],
                 "ansible_private_key_file": d["identity_file"],
                 "connection": "ssh",
-                "ansible_ssh_common_args": " ".join(self.ssh_connection_options),
+                "ansible_ssh_common_args": " ".join(self.ssh_connection_options),  # noqa: E501
             }
         except StopIteration:
             return {}
         except IOError:
             # Instance has yet to be provisioned, therefore the
             # instance_config is not on disk.
             return {}
 
     def _get_instance_config(self, instance_name):
-        instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
+        instance_config_dict = util.safe_load_file(self._config.driver.instance_config)  # noqa: E501
         return next(
-            item for item in instance_config_dict if item["instance"] == instance_name
+            item for item in instance_config_dict if item["instance"] == instance_name   # noqa: E501
         )
 
     def sanity_checks(self):
         pass
 
     def template_dir(self):
         """Return path to its own cookiecutterm templates. It is used by init
```

### Comparing `molecule-proxmox-0.9.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py` & `molecule_proxmox-1.0.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     'supported_by': 'community',
 }
 
 DOCUMENTATION = r"""
 ---
 module: proxmox_qemu_agent
 
-short_description: Query the QEMU guest agent to find the IP addresses of a running vm.
+short_description: Query the QEMU guest agent to find the IP addresses
+                   of a running vm.
 
 description:
-  - Start the vm if it is currently not running and wait until at least one non-loopback
-    IP address is detected.
+  - Start the vm if it is currently not running and wait until at least
+    one non-loopback IP address is detected.
 
   - Fails when an IP address is not found within the timeout value.
 
 author:
   - Michael Meffie (@meffie)
 """
 
@@ -45,31 +46,31 @@
 addresses:
   decription: list of one or more IPv4 addresses
   returned: always
   type: list
   sample: ['192.168.136.123']
 """
 
-import time
-import syslog
+import time  # noqa: E402
+import syslog  # noqa: E402
 
-from proxmoxer import ProxmoxAPI
-from proxmoxer.core import ResourceException
-from ansible.module_utils.basic import AnsibleModule
+from proxmoxer import ProxmoxAPI  # noqa: E402
+from proxmoxer.core import ResourceException  # noqa: E402
+from ansible.module_utils.basic import AnsibleModule  # noqa: E402
 
 
 def get_vm(module, proxmox, vmid):
     """
     Look up a vm by id, and fail if not found.
     """
-    vm_list = [vm for vm in proxmox.cluster.resources.get(type='vm') if vm['vmid'] == int(vmid)]
+    vm_list = [vm for vm in proxmox.cluster.resources.get(type='vm') if vm['vmid'] == int(vmid)]  # noqa: E501
     if len(vm_list) == 0:
         module.fail_json(vmid=vmid, msg='VM with vmid = %s not found' % vmid)
     if len(vm_list) > 1:
-        module.fail_json(vmid=vmid, msg='Multiple VMs with vmid = %s found' % vmid)
+        module.fail_json(vmid=vmid, msg='Multiple VMs with vmid = %s found' % vmid)  # noqa: E501
     return vm_list[0]
 
 
 def start_vm(module, proxmox, vm):
     """
     Start the vm and wait until the start task completes.
     """
@@ -102,20 +103,20 @@
     proxmox_node = proxmox.nodes(vm['node'])
     timeout = module.params['timeout']
 
     syslog.syslog('Waiting for vmid {0} IP address'.format(vmid))
     while timeout:
         reply = None
         try:
-            reply = proxmox_node.qemu(vmid).agent.get('network-get-interfaces')
+            reply = proxmox_node.qemu(vmid).agent.get('network-get-interfaces')  # noqa: E501
             # syslog.syslog('network-get-interfaces: {0}'.format(reply))
         except ResourceException as e:
-            if e.status_code == 500 and 'VM {0} is not running'.format(vmid) in e.content:
+            if e.status_code == 500 and 'VM {0} is not running'.format(vmid) in e.content:  # noqa: 501
                 start_vm(module, proxmox, vm)
-            elif e.status_code == 500 and 'QEMU guest agent is not running' in e.content:
+            elif e.status_code == 500 and 'QEMU guest agent is not running' in e.content:  # noqa: 501
                 pass  # Waiting for guest agent to start.
             else:
                 module.fail_json(msg=str(e))
         if reply and 'result' in reply:
             addresses = i2a(reply['result'])
             if len(addresses) > 0:
                 return addresses   # Found at least one address.
@@ -127,15 +128,16 @@
     msg = 'Timeout while waiting for vmid {0} IP address'.format(vmid)
     syslog.syslog(msg)
     module.fail_json(msg=msg)
 
 
 def i2a(interfaces):
     """
-    Extract the non-loopback IPv4 addresses from network-get-interfaces results.
+    Extract the non-loopback IPv4 addresses from
+    network-get-interfaces results.
 
     Example:
 
         reply = {'results': [
           {
             'name': 'ens18',
             'hardware-address': '6e:25:bb:c7:4b:76',
```

### Comparing `molecule-proxmox-0.9.0/src/molecule_proxmox/playbooks/create.yml` & `molecule_proxmox-1.0.0/src/molecule_proxmox/playbooks/create.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 ---
 - name: Create
   hosts: localhost
   connection: local
   gather_facts: false
-  collections:
-    - community.general
   vars:
       options: "{{ molecule_yml.driver.options }}"
   tasks:
     - name: "Load proxmox secrets."
-      include_vars: "{{ options.proxmox_secrets }}"
+      ansible.builtin.include_vars: "{{ options.proxmox_secrets }}"
       when: options.proxmox_secrets is defined
       no_log: true
 
     - name: "Create molecule instance(s)."
-      proxmox_kvm:
+      community.general.proxmox_kvm:
         state: present
         api_host: "{{ api_host | d(options.api_host) | d(omit) }}"
         api_user: "{{ api_user | d(options.api_user) | d(omit) }}"
         api_password: "{{ api_password | d(options.api_password) | d(omit) }}"
         api_token_id: "{{ api_token_id | d(options.api_token_id) | d(omit) }}"
         api_token_secret: "{{ api_token_secret | d(options.api_token_secret) | d(omit) }}"
         vmid: "{{ p.proxmox_template_vmid | d(p.template_vmid, true) | d(omit, true) }}"
         clone: "{{ p.proxmox_template_name | d(p.template_name, true) | d(options.template_name, true) | d(p.box, true) | d('molecule', true) }}"
         name: "{{ p.name }}"
         node: "{{ options.node }}"
         timeout: "{{ options.timeout | d(omit) }}"
+        pool: "{{ options.pool | d(omit) }}"
+        newid: "{{ p.newid | d(p.newid, true) | d(omit, true) }}"
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         loop_var: p
         label: "{{ p.name }}"
       register: proxmox_clone
 
     - name: "Update molecule instance config(s)"
-      proxmox_kvm:
+      community.general.proxmox_kvm:
         state: present
         update: true
         api_host: "{{ api_host | d(options.api_host) | d(omit) }}"
         api_user: "{{ api_user | d(options.api_user) | d(omit) }}"
         api_password: "{{ api_password | d(options.api_password) | d(omit) }}"
         api_token_id: "{{ api_token_id | d(options.api_token_id) | d(omit) }}"
         api_token_secret: "{{ api_token_secret | d(options.api_token_secret) | d(omit) }}"
@@ -76,28 +76,30 @@
       loop: "{{ proxmox_clone.results }}"
       loop_control:
         loop_var: rc
         label: "{{ rc.p.name, rc.vmid }}"
       register: proxmox_qemu_agent
 
     - name: "Populate instance configs."
-      set_fact:
+      ansible.builtin.set_fact:
         instance_config:
           instance: "{{ ra.rc.p.name }}"
           address: "{{ ra.addresses[0] }}"
           user: "{{ options.ssh_user | d('molecule') }}"
           port: 22
           identity_file: "{{ options.ssh_identity_file }}"
           vmid: "{{ ra.vmid }}"
       loop: "{{ proxmox_qemu_agent.results }}"
       loop_control:
         loop_var: ra
         label: "{{ ra.rc.p.name, ra.vmid, ra.addresses[0] }}"
       register: instance_configs
 
-    - set_fact:
+    - name: "Set instance_config fact."
+      ansible.builtin.set_fact:
         instance_configs: "{{ instance_configs.results | map(attribute='ansible_facts.instance_config') | list }}"
 
     - name: "Write instance configs."
-      copy:
+      ansible.builtin.copy:
         content: "{{ instance_configs | to_nice_yaml }}"
         dest: "{{ molecule_instance_config }}"
+        mode: '0644'
```

### Comparing `molecule-proxmox-0.9.0/src/molecule_proxmox/playbooks/destroy.yml` & `molecule_proxmox-1.0.0/src/molecule_proxmox/playbooks/destroy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 ---
 - name: Destroy
   hosts: localhost
   connection: local
   gather_facts: false
-  collections:
-    - community.general
   vars:
       options: "{{ molecule_yml.driver.options }}"
   tasks:
     - name: "Load proxmox secrets."
-      include_vars: "{{ options.proxmox_secrets }}"
+      ansible.builtin.include_vars: "{{ options.proxmox_secrets }}"
       when: options.proxmox_secrets is defined
       no_log: true
 
     # Remove instances by numeric vmid instead of by name, which seems
     # safer and more reliable. Since the Ansible lookup() plugin complains
     # even when error=ingore is set, just create an empty file to ignore
     # a missing instance_configs.
     - name: "Check for instance configs."
-      stat:
+      ansible.builtin.stat:
         path: "{{ molecule_instance_config }}"
       register: instance_config_stat
 
     - name: "Write empty instance configs."
-      copy:
+      ansible.builtin.copy:
         content: "[]"
         dest: "{{ molecule_instance_config }}"
+        mode: '0644'
       when: not instance_config_stat.stat.exists
 
     - name: "Remove molecule instance(s)."
-      proxmox_kvm:
+      community.general.proxmox_kvm:
         api_host: "{{ api_host | d(options.api_host) | d(omit) }}"
         api_user: "{{ api_user | d(options.api_user) | d(omit) }}"
         api_password: "{{ api_password | d(options.api_password) | d(omit) }}"
         api_token_id: "{{ api_token_id | d(options.api_token_id) | d(omit) }}"
         api_token_secret: "{{ api_token_secret | d(options.api_token_secret) | d(omit) }}"
         state: absent
         vmid: "{{ i.vmid }}"
```

### Comparing `molecule-proxmox-0.9.0/src/molecule_proxmox/playbooks/prepare.yml` & `molecule_proxmox-1.0.0/src/molecule_proxmox/playbooks/prepare.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 ---
 - name: Prepare
   hosts: all
   gather_facts: no
   tasks:
     - name: "Waiting for instance ssh connection."
-      wait_for_connection:
+      ansible.builtin.wait_for_connection:
 
-    - when: molecule_yml.driver.options.sethostname | d('yes') | bool
+    - name: "Set host name."
+      when: molecule_yml.driver.options.sethostname | d('yes') | bool
       block:
         - name: "Set instance hostname."
           become: yes
-          hostname:
+          ansible.builtin.hostname:
             name: "{{ inventory_hostname }}"
 
         - name: "Gather facts."
-          setup:
+          ansible.builtin.setup:
 
         - name: "Remove workaround loopback from /etc/hosts file."
           become: yes
-          lineinfile:
+          ansible.builtin.lineinfile:
             state: absent
             path: /etc/hosts
             regex: '^127\.0\.1\.1\s+\S+'
 
         - name: "Add address and hostname to /etc/hosts file."
           become: yes
-          lineinfile:
+          ansible.builtin.lineinfile:
             state: present
             path: /etc/hosts
             line: "{{ ansible_default_ipv4.address }} {{ ansible_hostname }}"
```

### Comparing `molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/PKG-INFO` & `molecule_proxmox-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: molecule-proxmox
-Version: 0.9.0
+Version: 1.0.0
 Summary: Proxmox Molecule Plugin :: run molecule tests using proxmox
 Home-page: https://github.com/meffie/molecule-proxmox
 Author: Michael Meffie
 Author-email: mmeffie@sinenomine.net
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: molecule>=6.0.0
+Requires-Dist: PyYAML
+Requires-Dist: proxmoxer>=1.3.1
 
 ***********************
 Molecule Proxmox Plugin
 ***********************
 
-This is an experimental Ansible Molecule Driver plugin to manage instances on a
+This is an Ansible Molecule Driver plugin to manage instances on a
 `Proxmox VE`_ hypervisor cluster.  Only virtual machines are supported at this
-time.  Proxmox containers will be supported in a future release.
+time.
 
 Requirements
 ============
 
 * Access to a `Proxmox VE`_ cluster
 * One or more virtual machine templates with required setup
 * Python package `proxmoxer`_
@@ -60,57 +66,63 @@
 The ``molecule-proxmox`` plugin may be installed with Python ``pip``. A virtualenv
 is recommended.  The following commands install Ansible, Molecule, and the
 Molecule Proxmox plugin in a virtualenv called ``venv``.
 
 .. code-block:: bash
 
     $ python3 -m venv venv
-    $ source venv/bin/activate
-    $ pip3 install molecule[ansible] molecule-proxmox
+    $ . venv/bin/activate
+    $ pip3 install ansible-core molecule molecule-proxmox
 
-
-Example
-=======
+Examples
+========
 
 .. code-block:: yaml
 
    driver:
      name: molecule-proxmox
      options:
-        api_host: pve01.example.com
-        api_user: molecule
+        api_host: <hostname>        # e.g. pve01.example.com
+        api_user: <name>@<realm>    # e.g. root@pam
         api_password: "********"
         node: pve01
         ssh_user: tester
         ssh_identity_file: /path/to/id_rsa
-        template_name: debian11
-        sethostname: yes
    platforms:
      - name: test01
        template_name: debian11
      - name: test02
        template_name: alma8
 
 .. code-block:: yaml
 
    driver:
      name: molecule-proxmox
      options:
-        api_host: pve01.example.com
-        api_user: molecule
+        api_host: <hostname>        # e.g. pve01.example.com
+        api_user: <name>@<realm>    # e.g. root@pam
+        # Optional: Use an API token for Proxmox authentication.
         api_token_id: "********"
         api_token_secret: "*******************************"
         node: pve01
         ssh_user: tester
         ssh_identity_file: /path/to/id_rsa
+        # Optional: The default template name.
         template_name: debian11
+        # Optional: Set the hostname after cloning.
+        sethostname: yes
+        # Optional: Create the VMs in the pool.
+        pool: test
    platforms:
      - name: test01
+       # Optional: Specify the VM id of the clone.
+       newid: 216
      - name: test02
-       sethostname: no
+       # Optional: Specify the VM id of the clone.
+       newid: 217
 
 .. code-block:: yaml
 
    driver:
      name: molecule-proxmox
      options:
         # Secrets file may be encrypted with ansible-vault.
@@ -152,39 +164,40 @@
 To checkout the source code:
 
 .. code-block:: bash
 
     $ git clone https://github.com/meffie/molecule-proxmox
     $ cd molecule-proxmox
 
-A `Makefile` is provided to facilitate development and testing. A Python
-virtualenv environment may be created with the `init` target.
+A `Makefile` and `tox.ini` are provided to facilitate development and testing.
+A Python virtualenv environment may be created with the `init` target.
 
 .. code-block:: bash
 
     $ make init
     $ source .venv/bin/activate
 
 Export the following shell environment variables to run the unit tests.
 
 .. code-block:: bash
 
-    export PROXMOX_SECRETS=<proxmox secrets yaml file path>
+    # Connection info:
+    export PROXMOX_HOST=<proxmox hostname>
+    export PROXMOX_USER=<username@realm>   # e.g. root@pam
+    export PROXMOX_PASSWORD=<password>
+    export PROXMOX_TOKEN_ID=<id>
+    export PROXMOX_TOKEN_SECRET=<secret>
     export PROXMOX_NODE=<proxmox node name>
     export PROXMOX_SSH_USER=<username>
     export PROXMOX_SSH_IDENTITY_FILE=<ssh key file for username>
+
+    # Template id and names for unit tests:
     export PROXMOX_TEMPLATE_VMID=<template vmid to be cloned in by-vmid scenario>
     export PROXMOX_TEMPLATE_NAME=<template name to be cloned in by-name scenario>
 
-The secrets file should contain the proxmox login credentials, either the
-username and password, or a Proxmox API token id and value.  This file should
-be encrypted with `ansible-vault`. The ssh user and identity file should match
-the user and public key installed when the virtual machine template was
-created.
-
 To run the unit tests in verbose mode:
 
 .. code-block:: bash
 
     $ make test
 
 To run the unit tests in quiet mode:
```

### Comparing `molecule-proxmox-0.9.0/src/molecule_proxmox.egg-info/SOURCES.txt` & `molecule_proxmox-1.0.0/src/molecule_proxmox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-proxmox-0.9.0/tests/test_proxmox_driver.py` & `molecule_proxmox-1.0.0/tests/test_proxmox_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     with chdir(tmpdir):
         molecule('init', 'scenario', '--driver-name', 'molecule-proxmox')
         assert pathlib.Path('molecule/default/converge.yml').exists()
         assert pathlib.Path('molecule/default/create.yml').exists()
         assert pathlib.Path('molecule/default/destroy.yml').exists()
         assert pathlib.Path('molecule/default/molecule.yml').exists()
 
-@pytest.mark.parametrize('scenario', ['default', 'by-name', 'by-vmid', 'cloud-init'])
+
+@pytest.mark.parametrize('scenario', [
+                           'default', 'by-name', 'by-vmid', 'cloud-init'])
 def test_molecule_test(scenario):
     print('')
     testdir = pathlib.Path(__file__).resolve().parent
     projectdir = testdir / 'proxmox_driver'
     with chdir(projectdir):
         molecule('test', '--scenario-name', scenario)
         molecule('reset')
```

