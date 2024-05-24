# Comparing `tmp/pyavd_cli-0.1.3.tar.gz` & `tmp/pyavd_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyavd_cli-0.1.3.tar", max compression
+gzip compressed data, was "pyavd_cli-0.1.4.tar", max compression
```

## Comparing `pyavd_cli-0.1.3.tar` & `pyavd_cli-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      376 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0    11344 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/LICENSE
--rw-r--r--   0        0        0       18 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/README.md
--rw-r--r--   0        0        0      148 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/pyavd_cli/__init__.py
--rwxr-xr-x   0        0        0     8758 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/pyavd_cli/build.py
--rw-r--r--   0        0        0      898 2024-04-02 14:48:43.889116 pyavd_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pyavd_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      466 2024-05-24 09:44:59.654646 pyavd_cli-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0    11344 2024-05-24 09:44:59.654646 pyavd_cli-0.1.4/LICENSE
+-rw-r--r--   0        0        0       18 2024-05-24 09:44:59.654646 pyavd_cli-0.1.4/README.md
+-rw-r--r--   0        0        0      148 2024-05-24 09:44:59.654646 pyavd_cli-0.1.4/pyavd_cli/__init__.py
+-rwxr-xr-x   0        0        0     9855 2024-05-24 09:44:59.654646 pyavd_cli-0.1.4/pyavd_cli/build.py
+-rw-r--r--   0        0        0      898 2024-05-24 09:45:06.682691 pyavd_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pyavd_cli-0.1.4/PKG-INFO
```

### Comparing `pyavd_cli-0.1.3/LICENSE` & `pyavd_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyavd_cli-0.1.3/pyavd_cli/build.py` & `pyavd_cli-0.1.4/pyavd_cli/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 @log_execution_time(log_prefix="Total build time")
 def build(  # pylint: disable=too-many-arguments,too-many-locals
     inventory_path: Path,
     fabric_name: str,
     limit: str,
     intended_configs_path: Path,
     structured_configs_path: Path,
+    avd_facts_path: Optional[Path] = None,
     max_workers: int = 10,
     strict: bool = False,
 ):
     init_plugin_loader()
 
     loader = DataLoader()
     inventory = InventoryManager(loader=loader, sources=[inventory_path.as_posix()])
@@ -171,33 +172,54 @@
 
     with ProcessPoolExecutor(max_workers=max_workers) as executor:
         # Validate inputs
         all_hostvars = validate_all_inputs(all_hostvars, strict, executor)
 
         # Generate facts
         avd_facts = log_execution_time(log_prefix="Generate facts time")(get_avd_facts)(all_hostvars)
+        if avd_facts_path is not None:
+            avd_facts_path.parent.mkdir(parents=True, exist_ok=True)
+            with open(avd_facts_path, mode="w", encoding="utf8") as fd:
+                yaml.dump(
+                    avd_facts,
+                    fd,
+                    Dumper=AnsibleDumper,
+                    indent=2,
+                    sort_keys=False,
+                    width=130,
+                )
 
         limit_hostvars = {hostname: hostvars for hostname, hostvars in all_hostvars.items() if hostname in limit_hostnames}
 
         # Build structured config
         structured_configs = build_and_write_all_structured_configs(
             limit_hostvars, avd_facts, structured_configs_path, templar, executor
         )
 
         # Generate device config
         build_and_write_all_device_configs(intended_configs_path, structured_configs, strict, executor)
 
 
 def main():
     parser = argparse.ArgumentParser(description="Build AVD fabric.")
-    parser.add_argument("-i", "--inventory-path", required=True, type=Path)
-    parser.add_argument("-o", "--config-output-path", default=Path("intended"), type=Path)
-    parser.add_argument("-f", "--fabric-group-name", required=True, type=str)
-    parser.add_argument("-l", "--limit", default="all,!cvp", type=str)
-    parser.add_argument("-m", "--max-workers", default=os.cpu_count(), type=int)
+    parser.add_argument("-i", "--inventory-path", required=True, type=Path, help="Path to the inventory file.")
+    parser.add_argument("-o", "--config-output-path", default=Path("intended"), type=Path, help="Path to the output directory.")
+    parser.add_argument("--avd-facts-path", type=Path, help="If provided AVD facts will be written to this path.")
+    parser.add_argument("-f", "--fabric-group-name", required=True, type=str, help="Name of the fabric group.")
+    parser.add_argument(
+        "-l",
+        "--limit",
+        default="all,!cvp",
+        type=str,
+        help=(
+            "Limit filter for inventory. See https://docs.ansible.com/ansible/latest/inventory_guide/intro_patterns.html"
+            "#patterns-and-ad-hoc-commands."
+        ),
+    )
+    parser.add_argument("-m", "--max-workers", default=os.cpu_count(), type=int, help="Maximum number of parallel workers.")
     parser.add_argument(
         "--strict",
         action="store_true",
         help="Use strict mode and fail if there is validation errors",
     )
     parser.add_argument("-v", "--verbose", action="store_true")
 
@@ -205,34 +227,37 @@
 
     logging.basicConfig(level=logging.DEBUG if args.verbose else logging.INFO)
 
     inventory_path = args.inventory_path
     config_output_path = args.config_output_path
     intended_configs_path = config_output_path / "configs"
     structured_configs_path = config_output_path / "structured_configs"
+    avd_facts_path = args.avd_facts_path
     max_workers = args.max_workers
     strict = args.strict
     fabric_group_name = args.fabric_group_name
     limit = args.limit
 
     logger.debug("pyavd version: %s", pyavd_version)
     logger.debug("inventory_path: %s", inventory_path)
     logger.debug("intended_configs_path: %s", intended_configs_path)
     logger.debug("structured_configs_path: %s", structured_configs_path)
+    logger.debug("avd_facts_path: %s", avd_facts_path)
     logger.debug("max_workers: %s", max_workers)
     logger.debug("strict: %s", strict)
     logger.debug("fabric_group_name: %s", fabric_group_name)
     logger.debug("limit: %s", limit)
 
     build(
         inventory_path=inventory_path,
         fabric_name=fabric_group_name,
         limit=limit,
         intended_configs_path=intended_configs_path,
         structured_configs_path=structured_configs_path,
+        avd_facts_path=avd_facts_path,
         max_workers=max_workers,
         strict=strict,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyavd_cli-0.1.3/pyproject.toml` & `pyavd_cli-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyavd-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = "A collection of cli scripts to use pyavd"
 authors = ["Arista Networks <eosplus-dev@arista.com>"]
 readme = "README.md"
 include = ["CHANGELOG.md", "LICENSE"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `pyavd_cli-0.1.3/PKG-INFO` & `pyavd_cli-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyavd-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of cli scripts to use pyavd
 Author: Arista Networks
 Author-email: eosplus-dev@arista.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

