# Comparing `tmp/slpkg-5.0.8.tar.gz` & `tmp/slpkg-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slpkg-5.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "slpkg-5.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `slpkg-5.0.8.tar` & `slpkg-5.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1945 2024-05-10 20:55:25.000000 slpkg-5.0.8/README.md
--rw-r--r--   0        0        0     1693 2024-05-10 20:55:25.000000 slpkg-5.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/binaries/__init__.py
--rw-r--r--   0        0        0     9746 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/binaries/install.py
--rw-r--r--   0        0        0     2202 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/binaries/required.py
--rw-r--r--   0        0        0     1117 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/blacklist.py
--rw-r--r--   0        0        0     7545 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/check_updates.py
--rw-r--r--   0        0        0     1558 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/checks.py
--rw-r--r--   0        0        0     1856 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/checksum.py
--rw-r--r--   0        0        0     4548 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/choose_packages.py
--rw-r--r--   0        0        0      948 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/cleanings.py
--rw-r--r--   0        0        0     5637 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/configs.py
--rw-r--r--   0        0        0     4783 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/dependees.py
--rw-r--r--   0        0        0     2080 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/dialog_box.py
--rw-r--r--   0        0        0     5220 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/dialog_configs.py
--rw-r--r--   0        0        0     4699 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/download_only.py
--rw-r--r--   0        0        0     4283 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/downloader.py
--rw-r--r--   0        0        0      667 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/error_messages.py
--rw-r--r--   0        0        0     2284 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/find_installed.py
--rw-r--r--   0        0        0     1558 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/gpg_verify.py
--rw-r--r--   0        0        0    10030 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/install_data.py
--rw-r--r--   0        0        0     4211 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/load_data.py
--rw-r--r--   0        0        0    29927 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/main.py
--rw-r--r--   0        0        0     6630 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/multi_process.py
--rw-r--r--   0        0        0    12003 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/new_configs.py
--rw-r--r--   0        0        0     3207 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/progress_bar.py
--rw-r--r--   0        0        0     6881 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/remove_packages.py
--rw-r--r--   0        0        0     5389 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/repo_info.py
--rw-r--r--   0        0        0    17569 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/repositories.py
--rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/__init__.py
--rw-r--r--   0        0        0     1419 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/dependencies.py
--rw-r--r--   0        0        0     5192 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/sbo_generate.py
--rw-r--r--   0        0        0    13345 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/slackbuild.py
--rw-r--r--   0        0        0     3684 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/search.py
--rw-r--r--   0        0        0      712 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/toml_errors.py
--rw-r--r--   0        0        0     5529 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/tracking.py
--rw-r--r--   0        0        0     6878 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/update_repositories.py
--rw-r--r--   0        0        0    11373 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/upgrade.py
--rw-r--r--   0        0        0     9832 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/utilities.py
--rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/__init__.py
--rw-r--r--   0        0        0     6757 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/asciibox.py
--rw-r--r--   0        0        0     6696 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/cli_menu.py
--rw-r--r--   0        0        0      690 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/version.py
--rw-r--r--   0        0        0     8072 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/view_package.py
--rw-r--r--   0        0        0     1942 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/view_process.py
--rw-r--r--   0        0        0    13487 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/views.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1945 2024-05-23 17:39:38.000000 slpkg-5.0.9/README.md
+-rw-r--r--   0        0        0     1693 2024-05-23 17:39:38.000000 slpkg-5.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/binaries/__init__.py
+-rw-r--r--   0        0        0     9663 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/binaries/install.py
+-rw-r--r--   0        0        0     2176 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/binaries/required.py
+-rw-r--r--   0        0        0     1146 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/blacklist.py
+-rw-r--r--   0        0        0     7482 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/check_updates.py
+-rw-r--r--   0        0        0     1543 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/checks.py
+-rw-r--r--   0        0        0     1846 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/checksum.py
+-rw-r--r--   0        0        0     4505 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/choose_packages.py
+-rw-r--r--   0        0        0      932 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/cleanings.py
+-rw-r--r--   0        0        0     5781 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/configs.py
+-rw-r--r--   0        0        0     4749 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/dependees.py
+-rw-r--r--   0        0        0     2040 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/dialog_box.py
+-rw-r--r--   0        0        0     5225 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/dialog_configs.py
+-rw-r--r--   0        0        0     4713 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/download_only.py
+-rw-r--r--   0        0        0     4247 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/downloader.py
+-rw-r--r--   0        0        0      654 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/error_messages.py
+-rw-r--r--   0        0        0     2217 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/find_installed.py
+-rw-r--r--   0        0        0     1550 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/gpg_verify.py
+-rw-r--r--   0        0        0    10098 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/install_data.py
+-rw-r--r--   0        0        0     4572 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/load_data.py
+-rw-r--r--   0        0        0    29739 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/main.py
+-rw-r--r--   0        0        0     6569 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/multi_process.py
+-rw-r--r--   0        0        0    11817 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/new_configs.py
+-rw-r--r--   0        0        0     3101 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/progress_bar.py
+-rw-r--r--   0        0        0     6766 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/remove_packages.py
+-rw-r--r--   0        0        0     5296 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/repo_info.py
+-rw-r--r--   0        0        0    17558 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/repositories.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/sbos/__init__.py
+-rw-r--r--   0        0        0     1456 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/sbos/dependencies.py
+-rw-r--r--   0        0        0     5203 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0        0        0    13321 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/sbos/slackbuild.py
+-rw-r--r--   0        0        0     3640 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/search.py
+-rw-r--r--   0        0        0      696 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/toml_errors.py
+-rw-r--r--   0        0        0     5451 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/tracking.py
+-rw-r--r--   0        0        0     6796 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/update_repositories.py
+-rw-r--r--   0        0        0    11100 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/upgrade.py
+-rw-r--r--   0        0        0     9797 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/utilities.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/views/__init__.py
+-rw-r--r--   0        0        0     6626 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/views/asciibox.py
+-rw-r--r--   0        0        0     6681 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/views/cli_menu.py
+-rw-r--r--   0        0        0      685 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/views/version.py
+-rw-r--r--   0        0        0     8032 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/views/view_package.py
+-rw-r--r--   0        0        0     1901 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/views/view_process.py
+-rw-r--r--   0        0        0    14016 2024-05-23 17:39:38.000000 slpkg-5.0.9/slpkg/views/views.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.9/PKG-INFO
```

### Comparing `slpkg-5.0.8/README.md` & `slpkg-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.8/pyproject.toml` & `slpkg-5.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "slpkg"
-version = "5.0.8"
+version = "5.0.9"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 maintainers = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Package manager utility for Slackware Linux"
```

### Comparing `slpkg-5.0.8/slpkg/binaries/install.py` & `slpkg-5.0.9/slpkg/binaries/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 from slpkg.progress_bar import ProgressBar
 from slpkg.multi_process import MultiProcess
 from slpkg.binaries.required import Required
 from slpkg.views.view_process import ViewProcess
 
 
 class Packages(Configs):  # pylint: disable=[R0902]
-
-    """
-    Download and install packages with dependencies.
-    """
+    """Download and install packages with dependencies."""
 
     def __init__(self, repository: str, data: dict, packages: list, flags: list, mode: str):  # pylint: disable=[R0913]
         super(Configs, self).__init__()
         self.repository = repository
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
@@ -61,81 +58,74 @@
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ('-k', '--skip-installed'), flags)
 
         self.packages: list = self.utils.apply_package_pattern(data, packages)
 
     def execute(self) -> None:
-        """ Calls methods in order.
-        """
+        """Call methods in order."""
         self.view_process.message('Resolving dependencies')
         self.creating_dependencies_list()
         self.choose_package_dependencies()
         self.add_dependencies_to_install_order()
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
         self.check_for_skipped()
 
         self.view.install_upgrade_packages(self.packages, self.dependencies, self.mode)
         self.view.missing_dependencies(self.install_order)
         self.view.question()
 
         start: float = time.time()
         self.view.skipping_packages(self.skipped_packages)
-        self.crating_the_package_urls_list()
+        self.creating_the_package_urls_list()
         self.checksum_binary_packages()
         self.set_progress_message()
         self.install_packages()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
-        """ Creating the full list o f dependencies.
-        """
+        """Create the full list of dependencies."""
         for package in self.packages:
             dependencies: tuple = Required(self.data, package, self.flags).resolve()
 
             for dependency in dependencies:
                 self.dependencies.append(dependency)
 
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
-        """ Adds dependencies in order to install.
-        """
+        """Add dependencies in order to install."""
         self.install_order.extend(self.dependencies)
 
     def clean_the_main_slackbuilds(self) -> None:
-        """ Removes packages that already listed in dependencies.
-        """
+        """Remove packages that already listed in dependencies."""
         for dependency in self.dependencies:
             if dependency in self.packages:
                 self.packages.remove(dependency)
 
     def add_main_packages_to_install_order(self) -> None:
-        """ Adds main packages in order to install.
-        """
+        """Add main packages in order to install."""
         self.install_order.extend(self.packages)
 
     def check_for_skipped(self) -> None:
-        """ Skip packages by user.
-        """
+        """Skip packages by user."""
         if self.option_for_skip_installed:
             for name in self.install_order:
                 installed: str = self.utils.is_package_installed(name)
                 if installed:
                     self.skipped_packages.append(name)
 
         # Remove packages from skipped packages.
         self.install_order: list = [pkg for pkg in self.install_order if pkg not in self.skipped_packages]
 
-    def crating_the_package_urls_list(self) -> None:
-        """ Prepare package urls for downloading.
-        """
+    def creating_the_package_urls_list(self) -> None:
+        """Prepare package urls for downloading."""
         packages: dict = {}
         asc_files: list = []
         if self.install_order:
             self.view_process.message('Prepare sources for downloading')
             for pkg in self.install_order:
                 package: str = self.data[pkg]['package']
                 mirror: str = self.data[pkg]['mirror']
@@ -146,43 +136,40 @@
 
                 packages[pkg] = (url, self.tmp_slpkg)
                 if self.gpg_verification:
                     packages[f'{pkg}.asc'] = (asc_url, self.tmp_slpkg)
                     asc_files.append(asc_file)
 
                 self.binary_packages.append(package)
-                self.utils.remove_file_if_exists(self.tmp_slpkg, package)
 
             self.view_process.done()
             self.download_the_binary_packages(packages)
             if self.gpg_verification:
                 self.gpg.verify(asc_files)
 
     def download_the_binary_packages(self, packages: dict) -> None:
-        """ Download the packages.
+        """Download the packages.
 
         Args:
             packages (dict): Packages for downloading.
         """
         if packages:
             print(f'Started to download total ({self.cyan}{len(packages)}{self.endc}) packages:\n')
             self.download.download(packages)
             print()
 
     def checksum_binary_packages(self) -> None:
-        """ Checksum packages.
-        """
+        """Checksum packages."""
         for package in self.binary_packages:
             name: str = self.utils.split_package(Path(package).stem)['name']
             pkg_checksum: str = self.data[name]['checksum']
             self.check_md5.md5sum(self.tmp_slpkg, package, pkg_checksum)
 
     def install_packages(self) -> None:
-        """ Install the packages.
-        """
+        """Install the packages."""
         # Remove old slpkg.log file.
         if self.slpkg_log_file.is_file():
             self.slpkg_log_file.unlink()
 
         if self.binary_packages:
             print(f'Started the processing of ({self.cyan}{len(self.binary_packages)}{self.endc}) packages:\n')
 
@@ -191,16 +178,19 @@
                 if self.option_for_reinstall:
                     command: str = f'{self.reinstall} {self.tmp_slpkg}/{package}'
 
                 self.multi_proc.process_and_log(command, package, self.progress_message)
                 name: str = self.utils.split_package(package)['name']
                 self.write_deps_log(name)
 
+                if self.delete_sources:
+                    self.utils.remove_file_if_exists(self.tmp_slpkg, package)
+
     def write_deps_log(self, name: str) -> None:
-        """ Create log file with installed packages with dependencies.
+        """Create log file with installed packages with dependencies.
 
         Args:
             name (str): Package name.
         """
         deps: dict = {}
         deps_logs: dict = {}
         installed_requires: list = []
@@ -213,22 +203,20 @@
         deps[name] = installed_requires
         if self.deps_log_file.is_file():
             deps_logs: dict = self.utils.read_json_file(self.deps_log_file)
             deps_logs.update(deps)
         self.deps_log_file.write_text(json.dumps(deps_logs, indent=4), encoding='utf-8')
 
     def set_progress_message(self) -> None:
-        """ Set message for upgrade method.
-        """
+        """Set message for upgrade method."""
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.progress_message: str = f'{self.violet}Upgrading{self.endc}'
 
     def choose_package_dependencies(self) -> None:
-        """ Choose dependencies for install with dialog tool.
-        """
+        """Choose dependencies for install with dialog tool."""
         if self.dependencies and self.dialog:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = ' Choose dependencies you want to install '
```

### Comparing `slpkg-5.0.8/slpkg/binaries/required.py` & `slpkg-5.0.9/slpkg/binaries/required.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 
 
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
 class Required:
-
-    """
-    Creates a tuple of dependencies with
-    the right order to install.
-    """
+    """Create a tuple of dependencies with the right order to install."""
 
     __slots__ = ('data', 'name', 'flags', 'repos', 'utils',
                  'full_requires', 'repository_packages',
                  'option_for_resolve_off')
 
     def __init__(self, data: dict, name: str, flags: list):
         self.data: dict = data
@@ -32,16 +28,15 @@
             if info.get(repo_name):
                 self.full_requires: bool = info[repo_name].get('full_requires', False)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
             ('-O', '--resolve-off'), flags)
 
     def resolve(self) -> tuple:
-        """ Resolve the dependencies.
-        """
+        """Resolve the dependencies."""
         dependencies: tuple = ()
         if not self.option_for_resolve_off:
             requires: list[str] = self.remove_deps(self.data[self.name]['requires'])
 
             # Resolve dependencies for some special repos.
             if not self.full_requires:
                 for require in requires:
```

### Comparing `slpkg-5.0.8/slpkg/check_updates.py` & `slpkg-5.0.9/slpkg/check_updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 from slpkg.repo_info import RepoInfo
 from slpkg.utilities import Utilities
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 
 
 class CheckUpdates(Configs):  # pylint: disable=[R0902]
-
-    """
-    Checks for changes in the ChangeLog files.
-    """
+    """Checks for changes in the ChangeLog files."""
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repository: str = repository
 
         self.utils = Utilities()
@@ -44,15 +41,15 @@
         self.option_for_check: bool = self.utils.is_option(
             ('-c', '--check'), flags)
 
         self.option_for_progress_bar: bool = self.utils.is_option(
             ('-B', '--progress-bar'), flags)
 
     def check_the_repositories(self, queue: str = None) -> None:
-        """ Saves checks to a dictionary.
+        """Save checks to a dictionary.
 
         Args:
             queue (str, optional): Puts attributes to the queue.
         """
         if self.option_for_repository:
             self.save_the_compares(self.repository)
         else:
@@ -61,15 +58,15 @@
                     self.save_the_compares(repo)
 
         if queue is not None:
             queue.put(self.compare)
             queue.put(self.error_connected)
 
     def save_the_compares(self, repo: str) -> None:
-        """ Saves compares to a dictionary.
+        """Save compares to a dictionary.
 
         Args:
             repo (str): Repository name.
         """
         local_chg_txt: Path = Path(
             self.repos.repositories[repo]['path'],
             self.repos.repositories[repo]['changelog_txt']
@@ -85,15 +82,15 @@
         if not repo_data_file.is_file():
             self.compare[repo] = True
         else:
             self.compare[repo] = self.compare_the_changelogs(
                 local_chg_txt, repo_chg_txt)
 
     def compare_the_changelogs(self, local_chg_txt: Path, repo_chg_txt: str) -> bool:
-        """ Compares the two ChangeLog files for changes.
+        """Compare the two ChangeLog files for changes.
 
         Args:
             local_chg_txt (Path): Path to local ChangeLog file.
             repo_chg_txt (str): Mirror or remote ChangeLog file.
 
         Returns:
             bool: True of False.
@@ -127,39 +124,35 @@
 
         if repo_size == 0:
             return False
 
         return local_size != repo_size
 
     def check_for_error_connected(self) -> None:
-        """ Checks for error connected and prints a message.
-        """
+        """Check for error connected and prints a message."""
         if self.error_connected:
             print(f'\n{self.endc}Failed connected to the mirrors:\n')
             for repo in self.error_connected:
                 print(f'{self.red}>{self.endc} {repo}')
 
     def set_http_proxy_server(self) -> None:
-        """ Sets for HTTP proxy server.
-        """
+        """Set for HTTP proxy server."""
         self.http = ProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
 
     def set_socks_proxy_server(self) -> None:
-        """ Sets for proxy server.
-        """
+        """Set for proxy server."""
         try:  # Try to import PySocks if it's installed.
             from urllib3.contrib.socks import SOCKSProxyManager  # pylint: disable=[W0621,C0415]
         except (ModuleNotFoundError, ImportError) as error:
             print(error)
         # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
         self.http = SOCKSProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
 
     def view_messages(self) -> None:
-        """ Prints for update messages.
-        """
+        """Print for update messages."""
         repo_for_update: list = []
         for repo, comp in self.compare.items():
             if comp:
                 repo_for_update.append(repo)
 
         if repo_for_update:
             last_updates: dict = self.repo_info.repo_information()
@@ -180,15 +173,15 @@
         else:
             print(f'\n{self.endc}{self.yellow}No updated packages since the last check.{self.endc}')
 
         if self.option_for_check:
             print()
 
     def updates(self) -> dict:
-        """ Calls methods in parallel with progress tool or single.
+        """Call methods in parallel with progress tool or single.
 
         Returns:
             dict: Description
         """
         message: str = 'Checking for news, please wait'
         if self.progress_bar_conf or self.option_for_progress_bar:
             queue: Queue = Queue()
```

### Comparing `slpkg-5.0.8/slpkg/checks.py` & `slpkg-5.0.9/slpkg/checks.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 
 
 class Check(Configs):
-
-    """
-    Some checks before proceed.
-    """
+    """Some checks before proceed."""
 
     def __init__(self, repository: str):
         super(Configs, self).__init__()
         self.repository = repository
 
         self.errors = Errors()
         self.utils = Utilities()
 
     def package_exists_in_the_database(self, packages: list, data: dict) -> None:
-        """ Check if the package exist if not prints a message.
+        """Check if the package exist if not prints a message.
 
         Args:
             packages (list): List of packages.
             data (dict): Repository data.
         """
         not_packages: list = []
 
@@ -34,15 +31,15 @@
                 not_packages.append(pkg)
 
         if not_packages:
             self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists",
                                             exit_status=1)
 
     def is_package_installed(self, packages: list) -> None:
-        """Checking for installed packages and prints message if not.
+        """Check for installed packages and prints message if not.
 
         Args:
             packages (list): List of packages.
         """
         not_found: list = []
 
         for pkg in packages:
```

### Comparing `slpkg-5.0.8/slpkg/checksum.py` & `slpkg-5.0.9/slpkg/checksum.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,25 @@
 from slpkg.configs import Configs
 from slpkg.views.views import View
 from slpkg.error_messages import Errors
 from slpkg.views.asciibox import AsciiBox
 
 
 class Md5sum(Configs):
-
-    """ Checksum the file sources.
-    """
+    """Checksum the file sources."""
 
     def __init__(self, flags: list):
         super(Configs, self).__init__()
 
         self.ascii = AsciiBox()
         self.errors = Errors()
         self.view = View(flags)
 
     def md5sum(self, path: Union[str, Path], source: str, checksum: str) -> None:
-        """ Checksum the source file.
+        """Checksum the source file.
 
         Args:
             path (Union[str, Path]): Path to source file.
             source (str): Source file.
             checksum (str): Expected checksum.
         """
         if self.checksum_md5:
@@ -45,15 +43,15 @@
             checksum: str = "".join(checksum)
 
             if file_check != checksum:
                 self.ascii.draw_checksum_error_box(filename, checksum, file_check)
                 self.view.question()
 
     def read_binary_file(self, filename: Union[str, Path]) -> bytes | None:
-        """ Reads the file source.
+        """Read the file source.
 
         Args:
             filename (Union[str, Path]): File name.
 
         Returns:
             bytes: Binary bytes.
         """
```

### Comparing `slpkg-5.0.8/slpkg/choose_packages.py` & `slpkg-5.0.9/slpkg/choose_packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,30 @@
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 
 
 class Choose(Configs):
-
-    """
-    Choose packages with dialog utility and -S, --search flag.
-    """
+    """Choose packages with dialog utility and -S, --search flag."""
 
     def __init__(self, repository: str):
         super(Configs, self).__init__()
         self.repository: str = repository
 
         self.utils = Utilities()
         self.dialogbox = DialogBox()
 
         self.choices: list = []
         self.height: int = 10
         self.width: int = 70
         self.list_height: int = 0
 
     def packages(self, data: dict, packages: list, method: str) -> list:
-        """ Calls methods to choosing packages via dialog tool.
+        """Call methods to choosing packages via dialog tool.
 
         Args:
             data (dict): Repository data.
             packages (list): List of packages.
             method (str): Type of method.
 
         Returns:
@@ -63,26 +60,24 @@
                 raise SystemExit(0)
 
             os.system('clear')
 
         return packages
 
     def choose_from_installed(self, packages: list) -> None:
-        """ Choose installed packages for remove or find.
-        """
+        """Choose installed packages for remove or find."""
         for name, package in self.utils.all_installed().items():
             version: str = self.utils.split_package(package)['version']
 
             for pkg in sorted(packages):
                 if pkg in name or pkg == '*':
                     self.choices.extend([(name, version, False, f'Package: {package}')])
 
     def choose_for_upgraded(self, data: dict, packages: list) -> None:
-        """ Choose packages that they will going to upgrade.
-        """
+        """Choose packages that they will going to upgrade."""
         for package in sorted(packages):
 
             inst_package: str = self.utils.is_package_installed(package)
             inst_package_version: str = self.utils.split_package(inst_package)['version']
             inst_package_build: str = self.utils.split_package(inst_package)['build']
 
             repo_ver: str = data[package]['version']
@@ -95,16 +90,15 @@
             else:
                 self.choices.extend(
                     [(package, f'{inst_package_version} -> {repo_ver}', True,
                         f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
                         f'Available: {repo_ver} Build: {repo_build_tag}')])
 
     def choose_for_others(self, data: dict, packages: list) -> None:
-        """ Choose packages for others methods like install, tracking etc.
-        """
+        """Choose packages for others methods like install, tracking etc."""
         if self.repository == '*':
             for pkg in sorted(packages):
                 for repo_name, repo_data in data.items():
                     for package in repo_data.keys():
                         if pkg in package or pkg == '*':
                             version: str = repo_data[package]['version']
                             self.choices.extend([(package, version, False, f'Package: {package}-{version} '
```

### Comparing `slpkg-5.0.8/slpkg/cleanings.py` & `slpkg-5.0.9/slpkg/cleanings.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.views import View
 
 
 class Cleanings(Configs):  # pylint: disable=[R0903]
-    """ Cleans the logs from packages.
-    """
+    """Cleans the logs from packages."""
 
     def __init__(self):
         super(Configs, self).__init__()
 
         self.view = View()
         self.utils = Utilities()
 
     def tmp(self) -> None:
-        """ Delete files and folders in /tmp/slpkg/ folder.
-        """
+        """Delete files and folders in /tmp/slpkg/ folder."""
         print('Deleting of local data:\n')
 
         for file in self.tmp_slpkg.rglob('*'):
             print(f"  {self.bred}>{self.endc} {file}")
 
         print(f"\n{self.prog_name}: {self.bold}{self.bred}WARNING{self.endc}: All the files and "
               f"folders will delete!")
```

### Comparing `slpkg-5.0.8/slpkg/configs.py` & `slpkg-5.0.9/slpkg/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,47 +13,50 @@
 from dataclasses import dataclass
 
 from slpkg.toml_errors import TomlErrors
 
 
 @dataclass
 class Configs:  # pylint: disable=[R0902]
-    """ Default configurations. """
+    """Default configurations."""
+
     toml_errors = TomlErrors()
 
     prog_name: str = 'slpkg'
-    os_arch: str = platform.machine()
     tmp_path: Path = Path('/tmp')
     tmp_slpkg: Path = Path(tmp_path, prog_name)
     build_path: Path = Path(tmp_path, prog_name, 'build')
-    download_only_path: Path = Path(tmp_slpkg, '')
     etc_path: Path = Path('/etc', prog_name)
     lib_path: Path = Path('/var/lib', prog_name)
     log_path: Path = Path('/var/log/', prog_name)
     log_packages: Path = Path('/var', 'log', 'packages')
 
     deps_log_file: Path = Path(log_path, 'deps.log')
     slpkg_log_file: Path = Path(log_path, 'slpkg.log')
     upgrade_log_file: Path = Path(log_path, 'upgrade.log')
 
+    os_arch: str = platform.machine()
     file_list_suffix: str = '.pkgs'
     installpkg: str = 'upgradepkg --install-new'
     reinstall: str = 'upgradepkg --reinstall'
     removepkg: str = 'removepkg'
+    kernel_version: str = True
     colors: bool = True
     makeflags: str = '-j4'
     gpg_verification: bool = False
     checksum_md5: bool = True
     dialog: bool = True
     view_missing_deps: bool = True
+    delete_sources: bool = False
     downloader: str = 'wget'
     wget_options: str = '--c -q --progress=bar:force:noscroll --show-progress'
     curl_options: str = ''
     lftp_get_options: str = '-c get -e'
     lftp_mirror_options: str = '-c mirror --parallel=100 --only-newer --delete'
+    download_only_path: Path = Path(tmp_slpkg, '')
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     maximum_parallel: int = 5
     progress_bar_conf: bool = False
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
@@ -66,42 +69,44 @@
 
     proxy_address: str = ''
     proxy_username: str = ''
     proxy_password: str = ''
 
     try:
         # Load user configuration.
+        configs = {}
         config_path_file = Path(etc_path, f'{prog_name}.toml')
         if config_path_file.exists():
             with open(config_path_file, 'rb') as conf:
                 configs = {k.lower(): v for k, v in tomli.load(conf).items()}
 
         if configs:
             config = {k.lower(): v for k, v in configs['configs'].items()}
 
             os_arch: str = config['os_arch']
-            download_only_path: Path = Path(config['download_only_path'])
-            ask_question: bool = config['ask_question']
-            kernel_version: str = config['kernel_version']
+            file_list_suffix: str = config['file_list_suffix']
             installpkg: str = config['installpkg']
             reinstall: str = config['reinstall']
             removepkg: str = config['removepkg']
+            kernel_version: str = config['kernel_version']
             colors: bool = config['colors']
             makeflags: str = config['makeflags']
             gpg_verification: bool = config['gpg_verification']
             checksum_md5: bool = config['checksum_md5']
             dialog: bool = config['dialog']
             view_missing_deps: bool = config['view_missing_deps']
+            delete_sources: bool = config['delete_sources']
             downloader: str = config['downloader']
             wget_options: str = config['wget_options']
             curl_options: str = config['curl_options']
             lftp_get_options: str = config['lftp_get_options']
             lftp_mirror_options: str = config['lftp_mirror_options']
+            download_only_path: Path = Path(config['download_only_path'])
             ascii_characters: bool = config['ascii_characters']
-            file_list_suffix: str = config['file_list_suffix']
+            ask_question: bool = config['ask_question']
             parallel_downloads: bool = config['parallel_downloads']
             maximum_parallel: int = config['maximum_parallel']
             progress_bar_conf: bool = config['progress_bar']
             progress_spinner: str = config['progress_spinner']
             spinner_color: str = config['spinner_color']
             border_color: str = config['border_color']
             process_log: bool = config['process_log']
```

### Comparing `slpkg-5.0.8/slpkg/dependees.py` & `slpkg-5.0.9/slpkg/dependees.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 from typing import Generator
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
 
 
 class Dependees(Configs):  # pylint: disable=[R0902]
-
-    """
-    Prints the packages that depend on.
-    """
+    """Prints the packages that depend on."""
 
     def __init__(self, data: dict, packages: list, flags: list):
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
 
@@ -31,28 +28,27 @@
         self.option_for_full_reverse: bool = self.utils.is_option(
             ('-E', '--full-reverse'), flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def find(self) -> None:
-        """ Calls the methods.
-        """
+        """Call the methods."""
         print('The list below shows the packages that dependees on:\n')
         self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
 
         for package in self.packages:
             dependees: dict = dict(self.find_requires(package))
             self.view_the_main_package(package)
             self.view_no_dependees(dependees)
             self.view_dependees(dependees)
             self.view_summary_of_dependees(dependees, package)
 
     def set_the_package_version(self, package: str) -> None:
-        """ Set the version of the package.
+        """Set the version of the package.
 
         Args:
             package (str): Package name.
         """
         self.package_version: str = self.data[package]['version']
 
     def find_requires(self, package: str) -> Generator:
@@ -65,46 +61,46 @@
             Generator: List of names with requires.
         """
         for name, data in self.data.items():
             if package in data['requires']:
                 yield name, data['requires']
 
     def view_no_dependees(self, dependees: dict) -> None:
-        """ Prints for no dependees.
+        """Print for no dependees.
 
         Args:
             dependees (dict): Packages data.
         """
         if not dependees:
             print(f"{'':>1}{self.cyan}No dependees{self.endc}")
 
     def view_the_main_package(self, package: str) -> None:
-        """ Prints the main package.
+        """Print the main package.
 
         Args:
             package (str): Package name.
         """
         print(f'{self.byellow}{package}{self.endc}')
         print(f"{'':>1}{self.llc}{self.hl}", end='')
 
     @staticmethod
     def view_dependency_line(n: int, dependency: str) -> None:
-        """ Prints the dependency line.
+        """Print the dependency line.
 
         Args:
             n (int): Line number.
             dependency (str): Name of dependency.
         """
         str_dependency: str = f"{'':>4}{dependency}"
         if n == 1:
             str_dependency: str = f"{'':>1}{dependency}"
         print(str_dependency)
 
     def view_dependees(self, dependees: dict) -> None:
-        """ View packages that depend on.
+        """View packages that depend on.
 
         Args:
             dependees (dict): Packages data.
         """
         name_length: int = 0
         if dependees:
             name_length: int = max(len(name) for name in dependees.keys())
@@ -117,27 +113,27 @@
 
             self.view_dependency_line(n, dependency)
 
             if self.option_for_full_reverse:
                 self.view_full_reverse(n, dependees, requires)
 
     def view_full_reverse(self, n: int, dependees: dict, requires: str) -> None:
-        """ Prints all packages.
+        """Print all packages.
 
         Args:
             n (int): Number of line.
             dependees (dict): Packages data.
             requires (str): Package requires.
         """
         line_requires: str = f"{'':>5}{self.var}{self.hl} {self.violet}{','.join(requires)}{self.endc}"
         if n == len(dependees):
             line_requires: str = f"{'':>5}{self.llc}{self.hl} {self.violet}{','.join(requires)}{self.endc}"
         print(line_requires)
 
     def view_summary_of_dependees(self, dependees: dict, package: str) -> None:
-        """ Prints the summary.
+        """Print the summary.
 
         Args:
             dependees (dict): Packages data.
             package (str): Package name.
         """
         print(f'\n{self.grey}{len(dependees)} dependees for {package}{self.endc}\n')
```

### Comparing `slpkg-5.0.8/slpkg/dialog_box.py` & `slpkg-5.0.9/slpkg/dialog_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,52 +10,48 @@
 from slpkg.configs import Configs
 from slpkg.views.version import Version
 
 locale.setlocale(locale.LC_ALL, '')
 
 
 class DialogBox(Configs):
-    """ Class for dialog box"""
+    """Class for dialog box."""
 
     def __init__(self):
         super(Configs).__init__()
         self.more_kwargs: dict = {}
 
         self.d = Dialog(dialog="dialog")
         self.d.set_background_title(f'{self.prog_name} {Version().version} - Software Package Manager')
 
     def checklist(self, text: str, title: str, height: int, width: int,  # pylint: disable=[R0913]
                   list_height: int, choices: list) -> Tuple[bool, list]:
-        """ Display a checklist box.
-        """
+        """Display a checklist box."""
         self.more_kwargs.update(
             {"item_help": True}
         )
 
         code, tags = self.d.checklist(text=text, choices=choices, title=title, height=height, width=width,  # pylint: disable=[R0913]
                                       list_height=list_height, help_status=True, **self.more_kwargs)
 
         return code, tags
 
     def mixedform(self, text: str, title: str, elements: list, height: int, width: int,  # pylint: disable=[R0913]
                   form_height: int) -> Tuple[bool, list]:
-        """ Display a mixedform box.
-        """
+        """Display a mixedform box."""
         self.more_kwargs.update(
             {"item_help": True,
              "help_tags": True}
         )
         code, tags = self.d.mixedform(text=text, title=title, elements=elements,  # type: ignore
                                       height=height, width=width, form_height=form_height, help_button=True,
                                       help_status=True, **self.more_kwargs)
 
         return code, tags
 
     def msgbox(self, text: str, height: int, width: int) -> None:
-        """ Display a message box.
-        """
+        """Display a message box."""
         self.d.msgbox(text, height, width)
 
     def textbox(self, text: Union[str, Path], height: int, width: int) -> None:
-        """ Display a text box.
-        """
+        """Display a text box."""
         self.d.textbox(text, height, width)
```

### Comparing `slpkg-5.0.8/slpkg/dialog_configs.py` & `slpkg-5.0.9/slpkg/dialog_configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,38 +8,33 @@
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.error_messages import Errors
 
 
 class FormConfigs(Configs):
-
-    """
-    Edit slpkg.toml config file with dialog utility.
-    """
+    """Edit slpkg.toml config file with dialog utility."""
 
     def __init__(self):
         super(Configs).__init__()
         self.dialogbox = DialogBox()
         self.errors = Errors()
         self.utils = Utilities()
 
         self.orig_configs: list = []
         self.config_file: Path = Path(self.etc_path, f'{self.prog_name}.toml')
 
     def is_dialog_enabled(self) -> None:
-        """ Checking if the dialog box is enabled by the user.
-        """
+        """Check if the dialog box is enabled by the user."""
         if not self.dialog:
             self.errors.raise_error_message(f"You should enable the dialog in the "
                                             f"'{self.etc_path}/{self.prog_name}.toml' file", exit_status=1)
 
     def edit(self) -> None:
-        """ Read and write the configuration file.
-        """
+        """Read and write the configuration file."""
         self.is_dialog_enabled()
         elements: list = []
         height: int = 9
         width: int = 0
         form_height: int = 0
         text: str = f'Edit the configuration file: {self.config_file}'
         title: str = ' Configuration File '
@@ -67,26 +62,25 @@
         if code == 'ok' and check:
             self.write_file(tags)
 
         elif not check:
             self.edit()
 
     def help(self) -> None:
-        """ Load the configuration file on a text box.
-        """
+        """Load the configuration file on a text box."""
         self.dialogbox.textbox(str(self.config_file), 40, 60)
         self.edit()
 
     def check_configs(self, tags: list) -> bool:
-        """ Check for true of false values.
-        """
+        """Check for true of false values."""
         keys: list = [
             'COLORS',
             'DIALOG',
             'VIEW_MISSING_DEPS',
+            'DELETE_SOURCES',
             'SILENT_MODE',
             'ASCII_CHARACTERS',
             'ASK_QUESTION',
             'KERNEL_VERSION',
             'PARALLEL_DOWNLOADS',
             'PROGRESS_BAR',
             'SPINNING_BAR',
@@ -110,36 +104,35 @@
                 self.dialogbox.msgbox(f"\nError: Value for '{key}' not supported.\n",
                                       height=7, width=60)
                 return False
 
         return True
 
     def read_configs(self) -> None:
-        """ Read the original config file.
-        """
+        """Read the original config file."""
         with open(self.config_file, 'r', encoding='utf-8') as toml_file:
             self.orig_configs: list = toml_file.readlines()
 
     def write_file(self, tags: list) -> None:
-        """ Write the new values to the config file.
-        """
+        """Write the new values to the config file."""
         self.read_configs()
 
         with open(self.config_file, 'w', encoding='utf-8') as patch_toml:
             for line in self.orig_configs:
                 for key, value in zip(self.configs['configs'].keys(), tags):
 
                     if line.lstrip().startswith(f'{key} ='):
                         line = f'  {key} = "{value}"\n'
 
                     if line.lstrip().startswith(
 
                             ('COLORS =',
                              'DIALOG =',
                              'VIEW_MISSING_DEPS =',
+                             'DELETE_SOURCES =',
                              'SILENT_MODE =',
                              'ASCII_CHARACTERS =',
                              'ASK_QUESTION =',
                              'KERNEL_VERSION =',
                              'PARALLEL_DOWNLOADS =',
                              'MAXIMUM_PARALLEL = ',
                              'PROGRESS_BAR =',
```

### Comparing `slpkg-5.0.8/slpkg/download_only.py` & `slpkg-5.0.9/slpkg/download_only.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,15 @@
 from slpkg.downloader import Downloader
 from slpkg.error_messages import Errors
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 
 
 class DownloadOnly(Configs):  # pylint: disable=[R0902]
-
-    """
-    Download only the sources and the slackbuilds or the packages
-    for binary repositories.
-    """
+    """Download only the sources or packages."""
 
     def __init__(self, directory: str, flags: list, data: dict, repository: str):
         super(Configs, self).__init__()
         self.directory: Path = Path(directory)
         self.flags: list = flags
         self.data: dict = data
         self.repository: str = repository
@@ -41,15 +37,15 @@
         self.urls: dict = {}
         self.asc_files: list = []
 
         self.option_for_directory: bool = self.utils.is_option(
             ('-z', '--directory'), flags)
 
     def packages(self, packages: list) -> None:
-        """ Download the packages.
+        """Download the packages.
 
         Args:
             packages (list): List of packages.
         """
         if not self.directory.is_dir():
             self.errors.raise_error_message(f"Path '{self.directory}' does not exist", 1)
 
@@ -70,15 +66,15 @@
         print(f'{self.bgreen}{self.ascii.done}{self.endc}')
         self.download_the_sources()
 
         elapsed_time: float = time.time() - start
         self.utils.finished_time(elapsed_time)
 
     def save_binary_sources(self, name: str) -> None:
-        """ Assign for binary repositories.
+        """Assign for binary repositories.
 
         Args:
             name (str): Package name.
         """
         package: str = self.data[name]['package']
         mirror: str = self.data[name]['mirror']
         location: str = self.data[name]['location']
@@ -88,15 +84,15 @@
         asc_file: Path = Path(self.directory, f'{package}.asc')
 
         if self.gpg_verification:
             self.urls[f'{name}.asc'] = (asc_url, self.directory)
             self.asc_files.append(asc_file)
 
     def save_slackbuild_sources(self, name: str) -> None:
-        """ Assign for sbo repositories.
+        """Assign for sbo repositories.
 
         Args:
             name (str): SBo name.
         """
         if self.os_arch == 'x86_64' and self.data[name]['download64']:
             sources: tuple = self.data[name]['download64']
         else:
@@ -106,27 +102,29 @@
         if self.gpg_verification and self.repository == self.repos.sbo_repo_name:
             location: str = self.data[name]['location']
             asc_file: Path = Path(self.repos.repositories_path, self.repos.sbo_repo_name,
                                   location, f'{name}{self.repos.sbo_repo_tar_suffix}.asc')
             self.asc_files.append(asc_file)
 
     def copy_slackbuild_scripts(self, name: str) -> None:
-        """ Copy slackbuilds from local repository to download path.
+        """Copy slackbuilds from local repository to download path.
 
         Args:
             name (str): SBo name.
         """
         repo_path_package: Path = Path(self.repos.repositories[self.repository]['path'],
                                        self.data[name]['location'], name)
         if not Path(self.directory, name).is_dir():
             shutil.copytree(repo_path_package, Path(self.directory, name))
 
     def download_the_sources(self) -> None:
-        """ Starts to download the sources.
-        """
+        """Download the sources."""
         if self.urls:
             print(f'\nStarted to download total ({self.cyan}{len(self.urls)}{self.endc}) sources:\n')
             self.download.download(self.urls)
             print()
+            self.gpg_verify()
 
+    def gpg_verify(self) -> None:
+        """Verify files with GPG."""
         if self.gpg_verification and self.repository != self.repos.ponce_repo_name:
             self.gpg.verify(self.asc_files)
```

### Comparing `slpkg-5.0.8/slpkg/downloader.py` & `slpkg-5.0.9/slpkg/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 from slpkg.multi_process import MultiProcess
 from slpkg.views.views import View
 
 
 class Downloader(Configs):  # pylint: disable=[R0902]
-
-    """
-    Downloads the sources using external tools.
-    """
+    """Download the sources using external tools."""
 
     def __init__(self, flags: list):
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.errors = Errors()
         self.utils = Utilities()
@@ -40,40 +37,40 @@
 
         self.semaphore = Semaphore(self.maximum_parallel)
 
         self.option_for_parallel: bool = self.utils.is_option(
             ('-P', '--parallel'), flags)
 
     def download(self, sources: dict) -> None:
-        """ Starting the processing for downloading. """
+        """Start the process for downloading."""
         if self.parallel_downloads or self.option_for_parallel:
             self.parallel_download(sources)
         else:
             self.normal_download(sources)
 
     def parallel_download(self, sources: dict) -> None:
-        """ Download sources with parallel mode. """
+        """Download sources with parallel mode."""
         processes: list = []
         for urls, path in sources.values():
             for url in urls:
                 proc = Process(target=self.tools, args=(url, path))
                 processes.append(proc)
                 proc.start()
 
         for process in processes:
             process.join()
 
     def normal_download(self, sources: dict) -> None:
-        """ Download sources with normal mode. """
+        """Download sources with normal mode."""
         for urls, path in sources.values():
             for url in urls:
                 self.tools(url, path)
 
     def tools(self, url: str, path: Path) -> None:
-        """ Run the tool to downloading.
+        """Run the tool to downloading.
 
         Args:
             url (str): The URL link.
             path (Path): Path to save.
         """
         self.semaphore.acquire()
         url_parse: str = urlparse(url).path
@@ -85,43 +82,43 @@
             self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported", exit_status=1)
 
         self.multi_process.process(self.downloader_command)
         self.check_if_downloaded(url, path)
         self.semaphore.release()
 
     def set_wget_downloader(self, url: str, path: Path) -> None:
-        """ Set for wget tool.
+        """Set for wget tool.
 
         Args:
             url (str): URL link.
             path (Path): Path to save.
         """
         self.downloader_command: str = f'{self.downloader} {self.wget_options} --directory-prefix={path} "{url}"'
 
     def set_curl_downloader(self, url: str, path: Path) -> None:
-        """ Set for curl tool.
+        """Set for curl tool.
 
         Args:
             url (str): URL link.
             path (Path): Path to save.
         """
         self.downloader_command: str = (f'{self.downloader} {self.curl_options} "{url}" '
                                         f'--output {path}/{self.filename}')
 
     def set_lftp_downloader(self, url: str, path: Path) -> None:
-        """ Set for lftp tool.
+        """Set for lftp tool.
 
         Args:
             url (str): URL link.
             path (Path): Path to save.
         """
         self.downloader_command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {path}'
 
     def check_if_downloaded(self, url: str, path: Path) -> None:
-        """ Checking if file downloaded.
+        """Check for downloaded.
 
         Args:
             url (str): URL link.
             path (Path): Path to check the file.
         """
         path_file: Path = Path(path, self.filename)
         if not path_file.exists():
```

### Comparing `slpkg-5.0.8/slpkg/error_messages.py` & `slpkg-5.0.9/slpkg/error_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 # -*- coding: utf-8 -*-
 
 
 from slpkg.configs import Configs
 
 
 class Errors(Configs):  # pylint: disable=[R0903]
-
-    """
-    Raise an error message.
-    """
+    """Raise an error message."""
 
     def __init__(self):
         super(Configs, self).__init__()
 
     def raise_error_message(self, message: str, exit_status: int) -> None:
-        """A general method to raise an error message and exit.
+        """General method to raise an error message and exit.
 
         Args:
             message (str): Str message.
             exit_status (int): Exit status code.
 
         Raises:
             SystemExit: Description
```

### Comparing `slpkg-5.0.8/slpkg/find_installed.py` & `slpkg-5.0.9/slpkg/find_installed.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,69 +3,62 @@
 
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 
 
 class FindInstalled(Configs):
-
-    """
-    Find installed packages.
-    """
+    """Find the installed packages."""
 
     def __init__(self, flags: list, packages: list):
         super(Configs, self).__init__()
         self.packages: list = packages
 
         self.utils = Utilities()
         self.matching: list = []
         self.total_size: int = 0
 
         self.option_for_no_case: bool = self.utils.is_option(
             ('-m', '--no-case'), flags)
 
     def find(self) -> None:
-        """ Find packages installed packages.
-        """
+        """Find the packages."""
         self.view_title()
         for package in self.packages:
             for name in self.utils.all_installed().values():
 
                 if package in name or package == '*' or self.is_not_case_sensitive(package, name):
                     self.matching.append(name)
         self.view_matched_packages()
 
     @staticmethod
     def view_title() -> None:
-        """ Prints the title.
-        """
+        """Print the title."""
         print('The list below shows the installed packages:\n')
 
     def view_matched_packages(self) -> None:
-        """ Prints the matching packages.
-        """
+        """Print the matching packages."""
         if self.matching:
             for package in self.matching:
                 name: str = self.utils.split_package(package)['name']
                 pkg_size: int = self.utils.count_file_size(name)
                 size: str = self.utils.convert_file_sizes(pkg_size)
                 self.total_size += pkg_size
                 print(f'{self.cyan}{package}{self.endc} ({size})')
             self.view_summary()
         else:
             print('\nDoes not match any package.\n')
 
     def view_summary(self) -> None:
-        """ Prints the summary.
-        """
+        """Print the summary."""
         print(f'\n{self.grey}Total found {len(self.matching)} packages with '
               f'{self.utils.convert_file_sizes(self.total_size)} size.{self.endc}')
 
     def is_not_case_sensitive(self, package: str, name: str) -> bool:
-        """ Checks for case sensitive.
+        """Check for case sensitive.
 
         Args:
             package (str): Package file.
             name (str): Name of package.
 
         Returns:
             bool: True or False.
```

### Comparing `slpkg-5.0.8/slpkg/gpg_verify.py` & `slpkg-5.0.9/slpkg/gpg_verify.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,24 @@
 from slpkg.configs import Configs
 from slpkg.views.asciibox import AsciiBox
 from slpkg.views.views import View
 from slpkg.views.view_process import ViewProcess
 
 
 class GPGVerify(Configs):  # pylint: disable=[R0903]
-
-    """ GPG verify files.
-    """
+    """GPG verify files."""
 
     def __init__(self, flags: list):
         super(Configs, self).__init__()
         self.ascii = AsciiBox()
         self.view = View()
         self.view_process = ViewProcess(flags)
 
     def verify(self, asc_files: list) -> None:
-        """ Verify files with gpg tool.
+        """Verify files with gpg tool.
 
         Args:
             asc_files (list): List of files.
         """
         if self.gpg_verification:
             output: dict = {}
             gpg_command: str = 'gpg --verify'
```

### Comparing `slpkg-5.0.8/slpkg/install_data.py` & `slpkg-5.0.9/slpkg/install_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
 from slpkg.views.view_process import ViewProcess
 
 
 class InstallData(Configs):
-
-    """ Installs data to the repositories path.
-    """
+    """Installs data to the repositories path."""
 
     def __init__(self, flags: list):
         super(Configs, self).__init__()
         self.utils = Utilities()
         self.repos = Repositories()
         self.ascii = AsciiBox()
         self.multi_process = MultiProcess()
         self.view_process = ViewProcess(flags)
 
     def write_repo_info(self, changelog_file: Path, info: dict) -> None:
-        """ Reads the first date of the changelog file."""
+        """Read the first date of the changelog file.
+
+        Args:
+            changelog_file: Respository ChangeLog.txt path.
+            info: Repository information.
+        """
         repo_name: str = info['repo_name']
         full_requires: bool = info['full_requires']
         last_date: str = ''
         repo_info: dict = {}
         lines: list = self.utils.read_text_file(changelog_file)
         days = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
         for line in lines:
@@ -47,21 +50,18 @@
             'last_updated': last_date,
             'full_requires': full_requires
         }
 
         self.repos.repos_information.write_text(json.dumps(repo_info, indent=4), encoding='utf-8')
 
     def install_sbo_data(self, repo: str) -> None:  # pylint: disable=[R0914]
-        """ Reads the SLACKBUILDS.TXT FILE and creates a json data file.
+        """Read the SLACKBUILDS.TXT FILE and creates a json data file.
 
         Args:
             repo (str): repository name.
-
-        No Longer Returned:
-            None.
         """
         self.view_process.message(f'Updating the database for {repo}')
 
         data: dict = {}
         cache: list = []
         sbo_tags: list = [
             'SLACKBUILD NAME:',
@@ -133,15 +133,16 @@
         data_file: Path = Path(self.repos.repositories[repo]['path'], self.repos.data_json)
         data_file.write_text(json.dumps(data, indent=4), encoding='utf-8')
 
         self.view_process.done()
         print()
 
     def install_binary_data(self, repo: str) -> None:  # pylint: disable=[R0912,R0914,R0915]
-        """ Installs the data for binary repositories.
+        """Installs the data for binary repositories.
+
         Args:
             repo (str): Description
         """
         print()
         self.view_process.message(f'Updating the database for {repo}')
 
         slack_repos: list = [self.repos.slack_patches_repo_name, self.repos.slack_extra_repo_name]
```

### Comparing `slpkg-5.0.8/slpkg/load_data.py` & `slpkg-5.0.9/slpkg/load_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,32 +10,30 @@
 from slpkg.blacklist import Blacklist
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 from slpkg.views.view_process import ViewProcess
 
 
 class LoadData(Configs):
-
-    """ Reads data form json file and load to dictionary.
-    """
+    """Reads data form json file and load to dictionary."""
 
     def __init__(self, flags: list = None):
         super(Configs, self).__init__()
 
         if flags is None:
             flags = []
 
         self.repos = Repositories()
         self.utils = Utilities()
         self.black = Blacklist()
         self.ascii = AsciiBox()
         self.view_process = ViewProcess(flags)
 
     def load(self, repository: str, message: bool = True) -> dict:
-        """ Load data to the dictionary.
+        """Load data to the dictionary.
 
         Args:
             repository (str): Repository name.
             message (bool, optional): Prints or not progress message.
 
         Returns:
             dict: Dictionary data.
@@ -63,16 +61,16 @@
 
         if message:
             self.view_process.done()
 
         return data
 
     def read_data_file(self, file: Path) -> dict:
-        """
-        Read JSON data from the file.
+        """Read JSON data from the file.
+
         Args:
             file: Path file for reading.
         Returns:
             Dictionary with data.
         """
         json_data: dict = {}
         try:
@@ -84,14 +82,21 @@
             print(f"{'':>2} $ {self.green}slpkg update{self.endc}\n")
             raise SystemExit(1) from e
         except json.decoder.JSONDecodeError:
             pass
         return json_data
 
     def _remove_blacklist_from_all_repos(self, data: dict) -> dict:
+        """Remove blacklist packages from all repositories.
+
+        Args:
+            data: Repository data.
+        Returns:
+            Repository data without the blackpackages.
+        """
         # Remove blacklist packages from keys.
         for name, repo in data.items():
             blacklist_packages: list = self.utils.ignore_packages(list(data[name].keys()))
             for pkg in blacklist_packages:
                 if pkg in data[name].keys():
                     del data[name][pkg]
 
@@ -103,14 +108,21 @@
                 for blk in blacklist_packages:
                     if blk in deps:
                         deps.remove(blk)
                         data[name][pkg]['requires'] = deps
         return data
 
     def _remove_blacklist_from_a_repo(self, data: dict) -> dict:
+        """Remove blacklist from a repository.
+
+        Args:
+            data: Repository data.
+        Returns:
+            Repositories data without the blackpackages.
+        """
         blacklist_packages: list = self.utils.ignore_packages(list(data.keys()))
         # Remove blacklist packages from keys.
         for pkg in blacklist_packages:
             if pkg in data.keys():
                 del data[pkg]
 
         # Remove blacklist packages from dependencies (values).
```

### Comparing `slpkg-5.0.8/slpkg/main.py` & `slpkg-5.0.9/slpkg/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,15 @@
 from slpkg.remove_packages import RemovePackages
 from slpkg.update_repositories import UpdateRepositories
 
 signal(SIGPIPE, SIG_DFL)
 
 
 class Menu(Configs):  # pylint: disable=[R0902]
-
-    """
-    Control cli options
-    """
+    """Control cli options."""
 
     def __init__(self, args: list):  # pylint: disable=[R0915]
         super(Configs, self).__init__()
 
         self.args: list = args
         self.flags: list = []
         self.directory: str = str(self.tmp_slpkg)
@@ -300,16 +297,15 @@
         self.check_for_repositories()
         self.load_data = LoadData(self.flags)
 
         self.check = Check(self.repository)
         self.choose = Choose(self.repository)
 
     def check_for_repositories(self) -> None:
-        """ Checks a combination for binaries use repositories only and if repository exists.
-        """
+        """Check a combination for binaries use repositories only and if repository exists."""
         except_options: tuple = (
             '-s', 'search',
             '-U', 'upgrade'
         )
         if self.repository == '*' and not self.utils.is_option(except_options, self.args):
             self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
@@ -317,16 +313,15 @@
             self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
         if self.repository != '*':
             if not self.repos.repositories[self.repository]['enable']:
                 self.usage.help_minimal(f"{self.prog_name}: repository '{self.repository}' is disabled")
 
     def invalid_options(self) -> None:
-        """ Checks for invalid options.
-        """
+        """Check for invalid options."""
         invalid, commands, repeat = [], [], []
 
         for arg in self.args:
             if arg[0] == '-' and arg in self.commands:
                 commands.append(arg)
             elif arg[0] == '-' and arg not in self.options:
                 invalid.append(arg)
@@ -354,38 +349,34 @@
             self.usage.help_short(1)
 
         # Prints error for invalid options.
         if invalid:
             self.usage.help_minimal(f"{self.prog_name}: invalid options '{','.join(invalid)}'")
 
     def split_options(self) -> None:
-        """ Split options and commands, like: -iyjR
-
-            slpkg -jyiR package
+        """Split options and commands.
 
-            Put the command first and options after.
-            Result: ['-i', '-y', '-j', '-R']
+        Put the command first and options after.
         """
         for args in self.args:
             if args[0] == '-' and args[:2] != '--' and len(args) >= 3 and '=' not in args:
                 self.args.remove(args)
 
                 for opt in map(lambda x: f'-{x}', list(args[1:])):
                     if opt in self.commands:
                         self.args.insert(0, opt)
                         continue
 
                     self.args.append(opt)
 
     def split_options_from_args(self) -> None:
-        """ Split options from arguments.
+        """Split options from arguments.
 
-            slpkg -d package --directory=/path/to/download
-
-            Split the option ['--directory'] and ['/path/to/download/'].
+        slpkg -d package --directory=/path/to/download
+        Split the option ['--directory'] and ['/path/to/download/'].
         """
         remove_args: list = []
 
         for arg in self.args:
             split_arg: list = arg.split('=')
 
             if len(split_arg) > 1:
@@ -415,39 +406,37 @@
                 self.repository: str = ''
 
         for arg in remove_args:
             if arg in self.args:
                 self.args.remove(arg)
 
     def move_options(self) -> None:
-        """ Move options to the flags and removes from the arguments.
-        """
+        """Move options to the flags and removes from the arguments."""
         new_args: list = []
 
         for arg in self.args:
             if arg in self.options:
                 self.flags.append(arg)
             else:
                 new_args.append(arg)
 
         self.args: list = new_args
 
     def is_file_list_packages(self) -> list:
-        """ Checks if the arg is filelist.pkgs.
-        """
+        """Check if the arg is filelist.pkgs."""
         if self.args[1].endswith(self.file_list_suffix):
             file = Path(self.args[1])
             packages: list = list(self.utils.read_packages_from_file(file))
         else:
             packages: list = list(set(self.args[1:]))
 
         return packages
 
     def update(self) -> None:
-        """ Update the local repositories.
+        """Update the local repositories.
 
         Raises:
             SystemExit: Exit code 0.
         """
         if len(self.args) == 1:
             if self.utils.is_option((self.flag_check, self.flag_short_check), self.flags):
                 check = CheckUpdates(self.flags, self.repository)
@@ -455,15 +444,15 @@
             else:
                 update = UpdateRepositories(self.flags, self.repository)
                 update.repositories()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def upgrade(self) -> None:
-        """ Upgrade the installed packages.
+        """Upgrade the installed packages.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.upgrade.__name__
         removed: list = []
 
@@ -505,27 +494,27 @@
             else:
                 self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def repo_info(self) -> None:
-        """ Prints repositories information.
+        """Print repositories information.
 
         Raises:
             SystemExit: Exit code 0.
         """
         if len(self.args) == 1:
             repo = RepoInfo(self.flags, self.repository)
             repo.info()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def build(self) -> None:
-        """ Builds slackbuilds with dependencies without install.
+        """Build slackbuilds with dependencies without install.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.build.__name__
 
         if len(self.args) >= 2:
@@ -546,15 +535,15 @@
             else:
                 self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def install(self) -> None:
-        """ Builds and install packages with dependencies.
+        """Build and install packages with dependencies.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.install.__name__
 
         if len(self.args) >= 2:
@@ -573,15 +562,15 @@
             else:
                 install_sbo = Slackbuilds(self.repository, self.data, packages, self.flags, mode=command)
                 install_sbo.execute()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def download(self) -> None:
-        """ Download only packages.
+        """Download only packages.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.download.__name__
 
         if len(self.args) >= 2:
@@ -595,15 +584,15 @@
             self.check.package_exists_in_the_database(packages, self.data)
             down_only = DownloadOnly(self.directory, self.flags, self.data, self.repository)
             down_only.packages(packages)
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def remove(self) -> None:
-        """ Remove packages with dependencies.
+        """Remove packages with dependencies.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.remove.__name__
 
         if len(self.args) >= 2:
@@ -616,15 +605,15 @@
 
             remove = RemovePackages(packages, self.flags)
             remove.remove()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def find(self) -> None:
-        """ Find installed packages.
+        """Find installed packages.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.find.__name__
 
         if len(self.args) >= 2:
@@ -637,15 +626,15 @@
 
             find = FindInstalled(self.flags, packages)
             find.find()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def view(self) -> None:
-        """ View package information.
+        """View package information.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.view.__name__
 
         if len(self.args) >= 2:
@@ -664,15 +653,15 @@
                 view.package(self.data, packages)
             else:
                 view.slackbuild(self.data, packages)
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def search(self) -> None:
-        """ Searching packages to the repositories.
+        """Search packages from the repositories.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.search.__name__
         self.data: dict = self.load_data.load(self.repository)
 
@@ -684,15 +673,15 @@
 
             pkgs = SearchPackage(self.flags, packages, self.data, self.repository)
             pkgs.search()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def dependees(self) -> None:
-        """ View packages that depend on other packages.
+        """View packages that depend on other packages.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.dependees.__name__
 
         if len(self.args) >= 2:
@@ -707,15 +696,15 @@
 
             dependees = Dependees(self.data, packages, self.flags)
             dependees.find()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def tracking(self) -> None:
-        """ Tracking package dependencies.
+        """Tracking package dependencies.
 
         Raises:
             SystemExit: Exit code 0.
         """
         command: str = Menu.tracking.__name__
 
         if len(self.args) >= 2:
@@ -731,68 +720,68 @@
             tracking = Tracking(self.data, packages, self.flags, self.repository)
             tracking.package()
             raise SystemExit(0)
         self.usage.help_short(1)
 
 
 class SubMenu:
-    """ Submenu that separate from the main menu because of
-    have no options to manage here.
+    """Submenu that separate from the main menu.
+
+    Because of have no options to manage here.
     """
 
     def __init__(self, args: list):
         self.args: list = args
         self.usage = Usage()
         self.form_configs = FormConfigs()
         self.clean = Cleanings()
 
     def help(self) -> None:
-        """ Prints help menu and exit.
-        """
+        """Print help menu and exit."""
         if len(self.args) == 1:
             self.usage.help(0)
         self.usage.help_short(1)
 
     def version(self) -> None:
-        """ Print program version and exit.
+        """Print program version and exit.
 
         Raises:
             SystemExit: Exit code 0.
         """
         if len(self.args) == 1:
             version = Version()
             version.view()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def edit_configs(self) -> None:
-        """ Edit configurations via dialog box.
+        """Edit configurations via dialog box.
 
         Raises:
             SystemExit: Exit code 0.
         """
         if len(self.args) == 1:
             self.form_configs.edit()
             raise SystemExit(0)
         self.usage.help_short(1)
 
     def clean_tmp(self) -> None:
-        """ Remove all files and directories from tmp.
+        """Remove all files and directories from tmp.
 
         Raises:
             SystemExit: Exit code 0.
         """
         if len(self.args) == 1:
             self.clean.tmp()
             raise SystemExit(0)
         self.usage.help_short(1)
 
 
 def main() -> None:
-    """ Call options and commands.
+    """Call options and commands.
 
     Raises:
         SystemExit: Exit code 0.
     """
     args: list = sys.argv
     args.pop(0)
     usage = Usage()
```

### Comparing `slpkg-5.0.8/slpkg/multi_process.py` & `slpkg-5.0.9/slpkg/multi_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 from slpkg.views.asciibox import AsciiBox
 from slpkg.progress_bar import ProgressBar
 
 
 class MultiProcess(Configs):  # pylint: disable=[R0902]
-
-    """
-    Creates parallel process between progress bar and process.
-    """
+    """Create parallel process between progress bar and process."""
 
     def __init__(self, flags: list = None):
         super(Configs, self).__init__()
 
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.ascii = AsciiBox()
@@ -37,15 +34,16 @@
             self.option_for_progress_bar: bool = self.utils.is_option(
                 ('-B', '--progress-bar'), flags)
 
             self.option_for_reinstall: bool = self.utils.is_option(
                 ('-r', '--reinstall'), flags)
 
     def process_and_log(self, command: str, filename: str, progress_message: str) -> None:
-        """ Starting a multiprocessing process.
+        """Start a multiprocessing process.
+
         Args:
             command: The command of process
             filename: The filename of process.
             progress_message: The message of progress.
         Returns:
             None.
         """
@@ -84,16 +82,16 @@
 
             # Restore the terminal cursor
             print('\x1b[?25h', self.endc)
         else:
             self._run(command)
 
     def _run(self, command: str, stdout: subprocess = subprocess.PIPE, stderr: subprocess = subprocess.STDOUT) -> None:
-        """
-        Build the package and write a log file.
+        """Build the package and write a log file.
+
         Args:
             command: The command of process
             stdout: Captured stdout from the child process.
             stderr: Captured stderr from the child process.
         Returns:
             None.
         """
@@ -116,54 +114,51 @@
 
             # If the process failed, return exit code.
             if process.returncode != 0:
                 self._error_process()
                 raise SystemExit(process.returncode)
 
     def _error_process(self) -> None:
-        """ Prints error message for a process.
-        """
+        """Print error message for a process."""
         if not self.progress_bar_conf and not self.option_for_progress_bar:
             message: str = 'Error occurred with process. Please check the log file.'
             print()
             print(len(message) * '=')
             print(f'{self.bred}{message}{self.endc}')
             print(len(message) * '=')
             print()
 
     def _write_log_head(self) -> None:
-        """ Write the timestamp at the head of the log file.
-        """
+        """Write the timestamp at the head of the log file."""
         if self.process_log:
             with open(self.slpkg_log_file, 'a', encoding='utf-8') as log:
                 log.write(f"{len(self.head_message) * '='}\n")
                 log.write(f'{self.head_message}\n')
                 log.write(f"{len(self.head_message) * '='}\n")
 
     def _write_log_eof(self) -> None:
-        """ Write the bottom of the log file.
-        """
+        """Write the bottom of the log file."""
         if self.process_log:
             with open(self.slpkg_log_file, 'a', encoding='utf-8') as log:
                 log.write(f"\n{len(self.bottom_message) * '='}\n")
                 log.write(f'{self.bottom_message}\n')
                 log.write(f"{len(self.bottom_message) * '='}\n\n")
 
     @staticmethod
     def process(command: str, stderr: subprocess = None, stdout: subprocess = None) -> None:
-        """
-        Build the package and write a log file.
+        """Build the package and write a log file.
+
         Args:
             command: The command of process
             stdout: Captured stdout from the child process.
             stderr: Captured stderr from the child process.
         Returns:
             None.
         """
         try:
-            output = subprocess.run(f'{command}', shell=True, stderr=stderr, stdout=stdout, check=True)
+            output = subprocess.run(f'{command}', shell=True, stderr=stderr, stdout=stdout, check=False)
         except KeyboardInterrupt as e:
             raise SystemExit(1) from e
 
         if output.returncode != 0:
             if not command.startswith(('wget', 'wget2', 'curl', 'lftp')):
                 raise SystemExit(output.returncode)
```

### Comparing `slpkg-5.0.8/slpkg/new_configs.py` & `slpkg-5.0.9/slpkg/new_configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 import shutil
 import difflib
 import subprocess
 from pathlib import Path
 
 
 class NewConfigs:  # pylint: disable=[R0902]
-
-    """
-    Tool that manage the config files.
-    """
+    """Tool that manage the config files."""
 
     def __init__(self, options: list):
         self.options: list = options
         self.etc_path: Path = Path('/etc/slpkg')
         self.slpkg_config: Path = Path(self.etc_path, 'slpkg.toml')
         self.repositories_config: Path = Path(self.etc_path, 'repositories.toml')
         self.blacklist_config: Path = Path(self.etc_path, 'blacklist.toml')
@@ -34,31 +31,29 @@
         self.endc: str = '\x1b[0m'
 
         self.set_no_colors()
 
         self.choice = None
 
     def set_no_colors(self) -> None:
-        """ Switch off colors.
-        """
+        """Switch off colors."""
         if '--no-colors' in self.options:
             self.bold: str = ''
             self.red: str = ''
             self.green: str = ''
             self.bgreen: str = ''
             self.yellow: str = ''
             self.byellow: str = ''
             self.endc: str = ''
 
     def check(self) -> None:
-        """ Checks for .new files.
-        """
+        """Check for .new files."""
         print('Checking for NEW configuration files...\n')
-        if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
-                or self.repositories_config_new.is_file()):
+        if (self.slpkg_config_new.is_file()
+                or self.blacklist_config_new.is_file() or self.repositories_config_new.is_file()):
             print('There are NEW files:\n')
 
             if self.slpkg_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.slpkg_config_new}{self.endc}")
 
             if self.repositories_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.repositories_config_new}{self.endc}")
@@ -77,16 +72,15 @@
 
             self.menu()
 
         else:
             print(f"\n{'No .new files found.':>23}\n")
 
     def menu(self) -> None:
-        """ Menu of choices.
-        """
+        """Menu of choices."""
         choice: str = input('Choice: ')
 
         choice: str = choice.lower()
 
         arguments: dict = {
             'k': self.keep,
             'o': self.overwrite,
@@ -97,111 +91,100 @@
         try:
             arguments[choice]()
         except KeyError:
             self.keep()
 
     @staticmethod
     def keep() -> None:
-        """ Prints a message.
-        """
+        """Print a message."""
         print("\nNo changes were made.\n")
 
     def overwrite(self) -> None:
-        """ Copy tne .new files and rename the olds to .orig.
-        """
+        """Copy tne .new files and rename the olds to .orig."""
         if self.slpkg_config_new.is_file():
             self.overwrite_config_file()
 
         if self.repositories_config_new.is_file():
             self.overwrite_repositories_file()
 
         if self.blacklist_config_new.is_file():
             self.overwrite_blacklist_file()
 
         print()  # new line
 
     def overwrite_config_file(self) -> None:
-        """ Copy the slpkg.toml.new file and rename the old to .orig.
-        """
+        """Copy the slpkg.toml.new file and rename the old to .orig."""
         if self.slpkg_config.is_file():
             shutil.copy(self.slpkg_config, f"{self.slpkg_config}.orig")
             print(f"\ncp {self.green}{self.slpkg_config}{self.endc} -> {self.slpkg_config}.orig")
 
         shutil.move(self.slpkg_config_new, self.slpkg_config)
         print(f"mv {self.slpkg_config_new} -> {self.green}{self.slpkg_config}{self.endc}")
 
     def overwrite_repositories_file(self) -> None:
-        """ Copy the repositories.toml.new file and rename the old to .orig.
-        """
+        """Copy the repositories.toml.new file and rename the old to .orig."""
         if self.slpkg_config.is_file():
             shutil.copy(self.repositories_config, f"{self.repositories_config}.orig")
             print(f"\ncp {self.green}{self.repositories_config}{self.endc} -> {self.repositories_config}.orig")
 
         shutil.move(self.repositories_config_new, self.repositories_config)
         print(f"mv {self.repositories_config_new} -> {self.green}{self.repositories_config}{self.endc}")
 
     def overwrite_blacklist_file(self) -> None:
-        """ Copy the blacklist.toml.new file and rename the old to .orig.
-        """
+        """Copy the blacklist.toml.new file and rename the old to .orig."""
         if self.blacklist_config.is_file():
             shutil.copy(self.blacklist_config, f"{self.blacklist_config}.orig")
             print(f"\ncp {self.green}{self.blacklist_config}{self.endc} -> {self.blacklist_config}.orig")
 
         shutil.move(self.blacklist_config_new, self.blacklist_config)
         print(f"mv {self.blacklist_config_new} -> {self.green}{self.blacklist_config}{self.endc}")
 
     def remove(self) -> None:
-        """ Removes the .new files.
-        """
+        """Remove the .new files."""
         print()  # new line
         self.remove_config_new_file()
         self.remove_repositories_new_file()
         self.remove_blacklist_new_file()
         print()  # new line
 
     def remove_config_new_file(self) -> None:
-        """ Remove slpkg.toml.new file.
-        """
+        """Remove slpkg.toml.new file."""
         if self.slpkg_config_new.is_file():
             self.slpkg_config_new.unlink()
             print(f"rm {self.red}{self.slpkg_config_new}{self.endc}")
 
     def remove_repositories_new_file(self) -> None:
-        """ Remove repositories.toml.new file.
-        """
+        """Remove repositories.toml.new file."""
         if self.repositories_config_new.is_file():
             self.repositories_config_new.unlink()
             print(f"rm {self.red}{self.repositories_config_new}{self.endc}")
 
     def remove_blacklist_new_file(self) -> None:
-        """ Remove blacklist.toml.new file.
-        """
+        """Remove blacklist.toml.new file."""
         if self.blacklist_config_new.is_file():
             self.blacklist_config_new.unlink()
             print(f"rm {self.red}{self.blacklist_config_new}{self.endc}")
 
     def prompt(self) -> None:
-        """ Prompt K, O, R selection for every single file.
-        """
+        """Prompt K, O, R selection for every single file."""
         print(f"\n{'':>2}({self.byellow}K{self.endc})eep, ({self.byellow}O{self.endc})verwrite, "
               f"({self.byellow}R{self.endc})emove, ({self.byellow}D{self.endc})iff, "
               f"({self.byellow}V{self.endc})imdiff\n")
 
         if self.slpkg_config_new.is_file():
             self.prompt_slpkg_config()
 
         if self.repositories_config_new.is_file():
             self.prompt_repositories_config()
 
         if self.blacklist_config_new.is_file():
             self.prompt_blacklist_config()
 
     def prompt_slpkg_config(self) -> None:
-        """ Prompt for slpkg.toml file.
-        """
+        """Prompt for slpkg.toml file."""
         make: str = input(f'{self.bgreen}{self.slpkg_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -215,16 +198,15 @@
         if make.lower() == 'd':
             self.diff_files(self.slpkg_config_new, self.slpkg_config)
             self.prompt_slpkg_config()
         if make.lower() == 'v':
             self.vimdiff(self.slpkg_config_new, self.slpkg_config)
 
     def prompt_repositories_config(self) -> None:
-        """ Prompt for repositories.toml file.
-        """
+        """Prompt for repositories.toml file."""
         make: str = input(f'{self.bgreen}{self.repositories_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -238,16 +220,15 @@
         if make.lower() == 'd':
             self.diff_files(self.repositories_config_new, self.repositories_config)
             self.prompt_repositories_config()
         if make.lower() == 'v':
             self.vimdiff(self.repositories_config_new, self.repositories_config)
 
     def prompt_blacklist_config(self) -> None:
-        """ Prompt for blacklist.toml file.
-        """
+        """Prompt for blacklist.toml file."""
         make: str = input(f'{self.bgreen}{self.blacklist_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -262,45 +243,44 @@
             self.diff_files(self.blacklist_config_new, self.blacklist_config)
             self.prompt_blacklist_config()
         if make.lower() == 'v':
             self.vimdiff(self.blacklist_config_new, self.blacklist_config)
 
     @staticmethod
     def diff_files(file2: Path, file1: Path) -> None:
-        """ Diff the .new and the current file.
-        """
+        """Diff the .new and the current file."""
         with open(file1, 'r', encoding='utf-8') as f1:
             with open(file2, 'r', encoding='utf-8') as f2:
                 diff = difflib.context_diff(
                     f1.readlines(),
                     f2.readlines(),
                     fromfile=str(file1),
                     tofile=str(file2)
                 )
                 for line in diff:
                     print(line, end='')
 
     @staticmethod
     def vimdiff(file1: Path, file2: Path) -> None:
-        """ Show vimdiff command.
+        """Show vimdiff command.
 
         Args:
             file1 (Any): First file.
             file2 (Any): Second file.
 
         Raises:
             SystemExit: Raise exit code.
         """
         output = subprocess.call(f'vimdiff {file1} {file2}', shell=True)
         if output != 0:
             raise SystemExit(output)
 
 
 def main() -> None:
-    """ Manage arguments.
+    """Manage arguments.
 
     Raises:
         SystemExit: Description
     """
     args: list = sys.argv
     args.pop(0)
```

### Comparing `slpkg-5.0.8/slpkg/progress_bar.py` & `slpkg-5.0.9/slpkg/progress_bar.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,32 +5,28 @@
 import time
 
 from slpkg.configs import Configs
 from slpkg.views.asciibox import AsciiBox
 
 
 class ProgressBar(Configs):
-
-    """
-    Progress bar that show spinner instead of the
-    of the file progress.
-    """
+    """Progress spinner bar."""
 
     def __init__(self):
         super(Configs, self).__init__()
         self.ascii = AsciiBox()
 
         self.color: str = self.endc
         self.spinners: dict = {}
         self.spinners_color: dict = {}
         self.spinner: str = ''
         self.bar_message: str = ''
 
     def progress_bar(self, message: str, filename: str = None) -> None:
-        """ Creating progress bar. """
+        """Create the progress bar."""
         self.assign_spinner_chars()
         self.set_spinner()
         self.assign_spinner_colors()
         self.set_color()
         self.set_the_spinner_message(filename, message)
         print('\x1b[?25l', end='')  # Hide cursor before starting
 
@@ -41,60 +37,56 @@
                 time.sleep(0.1)
                 current_state = (current_state + 1) % len(self.spinner)
         except KeyboardInterrupt as e:
             print('\x1b[?25h', end='')
             raise SystemExit(1) from e
 
     def assign_spinner_colors(self) -> None:
-        """ Assign spinner colors.
-        """
+        """Assign spinner colors."""
         self.spinners_color: dict = {
             'green': self.green,
             'violet': self.violet,
             'yellow': self.yellow,
             'blue': self.blue,
             'cyan': self.cyan,
             'grey': self.grey,
             'red': self.red,
             'white': self.endc
         }
 
     def assign_spinner_chars(self) -> None:
-        """ Assign for characters.
-        """
+        """Assign for characters."""
         self.spinners: dict = {
             'spinner': ('-', '\\', '|', '/'),
             'pie': ('◷', '◶', '◵', '◴'),
             'moon': ('◑', '◒', '◐', '◓'),
             'line': ('⎺', '⎻', '⎼', '⎽', '⎼', '⎻'),
             'pixel': ('⣾', '⣷', '⣯', '⣟', '⡿', '⢿', '⣻', '⣽'),
             'ball': ('_', '.', '|', 'o'),
             'clock': ('🕛', '🕑', '🕒', '🕔', '🕧', '🕗', '🕘', '🕚')
         }
 
     def set_the_spinner_message(self, filename: str, message: str) -> None:
-        """ Set message to the spinner.
+        """Set message to the spinner.
 
         Args:
             filename (str): Name of file.
             message (str): The progress bar message.
         """
         self.bar_message: str = f'{message}... '
         if filename:
             self.bar_message: str = (f"{'':>2}{self.yellow}{self.ascii.bullet}{self.endc} {filename}: "
                                      f"{message}... ")
 
     def set_spinner(self) -> None:
-        """ Spinners characters.
-        """
+        """Spanners characters."""
         try:
             self.spinner: tuple = self.spinners[self.progress_spinner]
         except KeyError:
             self.spinner: tuple = self.spinners['spinner']
 
     def set_color(self) -> None:
-        """ Setting the spinner color.
-        """
+        """Set the spinner color."""
         try:
             self.color: str = self.spinners_color[self.spinner_color]
         except KeyError:
             self.color: str = self.endc
```

### Comparing `slpkg-5.0.8/slpkg/remove_packages.py` & `slpkg-5.0.9/slpkg/remove_packages.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,15 @@
 from slpkg.views.views import View
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.multi_process import MultiProcess
 
 
 class RemovePackages(Configs):  # pylint: disable=[R0902]
-
-    """
-    Removes installed packages with dependencies if they installed with
-    slpkg install command.
-    """
+    """Remove installed packages with dependencies."""
 
     def __init__(self, packages: list, flags: list):
         super(Configs, self).__init__()
         self.packages: list = packages
 
         self.dialogbox = DialogBox()
         self.utils = Utilities()
@@ -39,15 +35,15 @@
         self.option_for_yes: bool = self.utils.is_option(
             ('-y', '--yes'), flags)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
             ('-O', '--resolve-off'), flags)
 
     def remove(self, upgrade: bool = False) -> None:
-        """ Remove packages
+        """Remove packages.
 
         Args:
             upgrade (bool, optional): Is packages comes from upgrade method.
         """
         if not self.option_for_resolve_off:
             self.deps_log: dict = self.utils.read_json_file(self.deps_log_file)
 
@@ -72,30 +68,28 @@
             if answer in ['y', 'Y']:
                 start: float = time.time()
                 self.remove_packages()
                 elapsed_time: float = time.time() - start
                 self.utils.finished_time(elapsed_time)
 
     def add_packages_for_remove(self) -> None:
-        """ Add packages for remove.
-        """
+        """Add packages for remove."""
         for package in self.packages:
             installed: str = self.utils.is_package_installed(package)
             if installed:
                 self.packages_for_remove.append(installed)
 
             if self.deps_log.get(package):
                 dependencies: list = self.deps_log[package]
                 for dep in dependencies:
                     if self.utils.is_package_installed(dep) and dep not in self.packages:
                         self.dependencies.append(dep)
 
     def find_dependent(self) -> None:
-        """ Find packages that depend on other packages.
-        """
+        """Find packages that depend on other packages."""
         for package in self.packages_for_remove:
             name: str = self.utils.split_package(package)['name']
             for pkg, deps in self.deps_log.items():
                 if name in deps and pkg not in self.packages + self.dependencies:
                     version: str = ''
                     installed: str = self.utils.is_package_installed(pkg)
                     if installed:
@@ -105,29 +99,26 @@
         if self.found_dependent_packages:
             dependent_packages: list = list(set(self.found_dependent_packages))
             print(f'\n{self.bred}Warning: {self.endc}found extra ({len(dependent_packages)}) dependent packages:')
             for pkg, ver in self.found_dependent_packages.items():
                 print(f"{'':>2}{pkg} {self.grey}{ver}{self.endc}")
 
     def remove_doubles_dependencies(self) -> None:
-        """ Removes doubles packages.
-        """
+        """Remove doubles packages."""
         self.dependencies: list = list(set(self.dependencies))
 
     def add_installed_dependencies_to_remove(self) -> None:
-        """ Adds dependencies for remove.
-        """
+        """Add dependencies for remove."""
         for dep in self.dependencies:
             installed: str = self.utils.is_package_installed(dep)
             if installed:
                 self.packages_for_remove.append(installed)
 
     def remove_packages(self) -> None:
-        """ Remove packages.
-        """
+        """Remove packages."""
         # Remove old slpkg.log file.
         if self.slpkg_log_file.is_file():
             self.slpkg_log_file.unlink()
 
         print(f'Started of removing total ({self.cyan}{len(self.packages_for_remove)}{self.endc}) packages:\n')
         for package in self.packages_for_remove:
             command: str = f'{self.removepkg} {package}'
@@ -137,15 +128,15 @@
             name: str = self.utils.split_package(package)['name']
             if name in self.deps_log.keys():
                 self.deps_log.pop(name)
 
         self.deps_log_file.write_text(json.dumps(self.deps_log, indent=4), encoding='utf-8')
 
     def choose_packages_for_remove(self, packages: list, upgrade: bool = False) -> list:
-        """ Choose packages via dialog utility.
+        """Choose packages via dialog utility.
 
         Args:
             packages (list): Description
             upgrade (bool, optional): Description
 
         Returns:
             list: List of package names.
@@ -169,15 +160,15 @@
                 text: str = f'There are {len(choices)} packages:'
             code, packages = self.dialogbox.checklist(text, title, height, width, list_height, choices)  # pylint: disable=[W0612]
             os.system('clear')
             return packages
         return packages
 
     def remove_question(self) -> str | None:
-        """ Question about remove packages.
+        """Question about remove packages.
 
         Returns:
             str | None: Answer.
         """
         if not self.option_for_yes and self.ask_question:
             answer: str = input('\nDo you want to remove these packages? [y/N] ')
             return answer
```

### Comparing `slpkg-5.0.8/slpkg/repo_info.py` & `slpkg-5.0.9/slpkg/repo_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 from slpkg.configs import Configs
 from slpkg.load_data import LoadData
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
 class RepoInfo(Configs):  # pylint: disable=[R0902]
-
-    """
-    View information about repositories.
-    """
+    """View information about repositories."""
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repository: str = repository
 
         self.load_data = LoadData(flags)
@@ -35,60 +32,56 @@
         self.repo_data: dict = {}
         self.dates: dict = {}
 
         self.option_for_repository: bool = self.utils.is_option(
             ('-o', '--repository'), flags)
 
     def info(self) -> None:
-        """ Prints information about repositories.
-        """
+        """Print information about repositories."""
         self.load_repo_data()
 
         self.view_the_title()
 
         if self.option_for_repository:
             self.view_the_repository_information()
         else:
             self.view_the_repositories_information()
 
     def load_repo_data(self) -> None:
-        """ Loads repository data.
-        """
+        """Load repository data."""
         self.dates: dict = self.repo_information()
         if self.option_for_repository:
             self.repo_data: dict = self.load_data.load(self.repository)
         else:
             self.repo_data: dict = self.load_data.load('*')
 
     def repo_information(self) -> dict:
-        """ Loads repository information.
+        """Load repository information.
 
         Returns:
             dict: Description
         """
         repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
         if repo_info_json.is_file():
             repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
             return self.utils.read_json_file(repo_info_json)
         return {}
 
     def view_the_title(self) -> None:
-        """ Prints the title.
-        """
+        """Print the title."""
         title: str = 'repositories information:'.title()
         if self.option_for_repository:
             title: str = 'repository information:'.title()
         print(f'\n{title}')
         print('=' * (self.columns - 1))
         print(f"{'Name:':<{self.name_alignment}}{'Status:':<14}{'Last Updated:':<34}{'Packages:':>12}")
         print('=' * (self.columns - 1))
 
     def view_the_repository_information(self) -> None:
-        """ Prints the repository information.
-        # """
+        """Print the repository information."""
         args: dict = {
             'repo': self.repository,
             'date': 'None',
             'count': 0,
             'color': self.red,
             'status': 'Disable'
         }
@@ -102,16 +95,15 @@
             args['color'] = self.green
             args['count'] = len(self.repo_data)
 
         self.view_the_line_information(args)
         self.view_summary_of_all_repositories()
 
     def view_the_repositories_information(self) -> None:
-        """ Prints the repositories information.
-        """
+        """Print the repositories information."""
         args: dict = {}
         for repo, conf in self.repos.repositories.items():
             args: dict = {
                 'repo': repo,
                 'date': 'None',
                 'count': 0,
                 'color': self.red,
@@ -127,33 +119,31 @@
                 args['color'] = self.green
                 args['count'] = len(self.repo_data[repo])
 
             self.view_the_line_information(args)
         self.view_summary_of_all_repositories()
 
     def view_the_line_information(self, args: dict) -> None:
-        """Prints the row of information.
+        """Print the row of information.
 
         Args:
             args (dict): Arguments for print.
         """
         repository: str = args['repo']
         repo_color: str = self.cyan
         if args['repo'] == self.repos.default_repository:
             repo_color: str = self.byellow
             repository: str = f"{args['repo']} (default)"
 
         print(f"{repo_color}{repository:<{self.name_alignment}}{self.endc}{args['color']}{args['status']:<14}"
               f"{self.endc}{args['date']:<34}{self.yellow}{args['count']:>12}{self.endc}")
 
     def view_summary_of_repository(self) -> None:
-        """ Prints the repository summary.
-        """
+        """Print the repository summary."""
         print('=' * (self.columns - 1))
         print(f"{self.grey}Total {self.total_packages} packages available from the '{self.repository}' repository.\n")
 
     def view_summary_of_all_repositories(self) -> None:
-        """ Prints the total summary of repositories.
-        """
+        """Print the total summary of repositories."""
         print('=' * (self.columns - 1))
         print(f"{self.grey}Total of {self.enabled}/{len(self.repos.repositories)} "
               f"repositories are enabled with {self.total_packages} packages available.\n")
```

### Comparing `slpkg-5.0.8/slpkg/repositories.py` & `slpkg-5.0.9/slpkg/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.toml_errors import TomlErrors
 
 
 @dataclass
 class Repositories:  # pylint: disable=[R0902]
-
-    """
-    Repositories configurations.
-    """
+    """Repositories configurations."""
 
     toml_errors = TomlErrors()
     utils = Utilities()
 
     repositories_toml_file: Path = Path(Configs.etc_path, 'repositories.toml')
     repositories_path: Path = Path(Configs.lib_path, 'repos')
```

### Comparing `slpkg-5.0.8/slpkg/sbos/dependencies.py` & `slpkg-5.0.9/slpkg/sbos/dependencies.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 # -*- coding: utf-8 -*-
 
 
 from slpkg.utilities import Utilities
 
 
 class Requires:
-    """ Creates a tuple of dependencies with
-    the right order to install. """
+    """Create a tuple with package dependencies."""
+
     __slots__ = (
         'data', 'name', 'flags', 'utils', 'option_for_resolve_off'
     )
 
     def __init__(self, data: dict, name: str, flags: list):
         self.data: dict = data
         self.name: str = name
         self.utils = Utilities()
 
         self.option_for_resolve_off: bool = self.utils.is_option(
             ('-O', '--resolve-off'), flags)
 
     def resolve(self) -> tuple:
-        """ Resolve the dependencies. """
+        """Resolve the dependencies.
+
+        Return package dependencies in the right order.
+        """
         dependencies: tuple = ()
 
         if not self.option_for_resolve_off:
             requires: list[str] = self.remove_deps(self.data[self.name]['requires'])
 
             for require in requires:
                 sub_requires: list[str] = self.remove_deps(self.data[require]['requires'])
@@ -36,14 +39,15 @@
             requires.reverse()
             dependencies: tuple = tuple(dict.fromkeys(requires))
 
         return dependencies
 
     def remove_deps(self, requires: list) -> list:
         """Remove requirements that not in the repository.
+
         Args:
             requires (list): List of requires.
 
         Returns:
             list: List of packages name.
         """
         return [req for req in requires if req in self.data]
```

### Comparing `slpkg-5.0.8/slpkg/sbos/sbo_generate.py` & `slpkg-5.0.9/slpkg/sbos/sbo_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 
 from pathlib import Path
 from slpkg.configs import Configs
 from slpkg.views.asciibox import AsciiBox
 
 
 class SBoGenerate(Configs):
-
-    """
-    Generating the SLACKBUILDS.TXT file.
-    """
+    """Generating the SLACKBUILDS.TXT file."""
 
     def __init__(self):
         super(Configs, self).__init__()
         self.ascii = AsciiBox()
 
     def slackbuild_file(self, repo_path: Path, repo_slackbuild_txt: str) -> None:  # pylint: disable=[R0914]
-        """ Creates a SLACKBUILDS.TXT file.
+        """Create a SLACKBUILDS.TXT file.
 
         Args:
             repo_path (Path): Path to file.
             repo_slackbuild_txt (str): Name of file to create.
         """
         print(f'Generating the {repo_slackbuild_txt} file... ', end='', flush=True)
 
@@ -86,37 +83,37 @@
                     sbo.write(f'SLACKBUILD SHORT DESCRIPTION: {short_description}\n')
                     sbo.write('\n')
 
         print(f'{self.bgreen}{self.ascii.done}{self.endc}\n')
 
     @staticmethod
     def read_short_description(path: Path, name: str) -> str:
-        """ Returns the short description.
+        """Return the short description from slack-desc file.
 
         Args:
             path (Path): Path to file.
             name (str): Slackbuild name.
 
         Returns:
-            str: Description
+            str: Short description
         """
         slack_desc: Path = Path(path, 'slack-desc')
         if slack_desc.is_file():
             with open(slack_desc, 'r', encoding='utf-8') as f:
                 slack = f.readlines()
 
             for line in slack:
                 pattern: str = f'{name}: {name}'
                 if line.startswith(pattern):
                     return line[len(name) + 1:].strip()
         return ''
 
     @staticmethod
     def read_info_file(info_file: Path, start: str, stop: str) -> list:
-        """Reads the .info file and return the line between to variables.
+        """Read the .info file and return the line between to variables.
 
         Args:
             info_file (Path): Slackbuild file name.
             start (str): Variable name to start.
             stop (str): Variable name to stop.
 
         Returns:
```

### Comparing `slpkg-5.0.8/slpkg/sbos/slackbuild.py` & `slpkg-5.0.9/slpkg/sbos/slackbuild.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
 from slpkg.views.view_process import ViewProcess
 from slpkg.sbos.dependencies import Requires
 
 
 class Slackbuilds(Configs):  # pylint: disable=[R0902,R0904]
-
-    """
-    Download build and install the SlackBuilds.
-    """
+    """Download, build and install the SlackBuilds."""
 
     def __init__(self, repository: str, data: dict, slackbuilds: list, flags: list, mode: str):  # pylint: disable=[R0913]
         super(Configs, self).__init__()
 
         self.repository: str = repository
         self.data: dict = data
         self.flags: list = flags
@@ -51,15 +48,15 @@
         self.download = Downloader(flags)
         self.upgrade = Upgrade(repository, data)
         self.gpg = GPGVerify(flags)
         self.errors = Errors()
 
         self.bar_process = None
         self.sources: dict = {}
-        self.install_order: list = []
+        self.build_order: list = []
         self.dependencies: list = []
         self.skipped_packages: list = []
         self.asc_files: list = []
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
@@ -69,166 +66,159 @@
 
         self.slackbuilds: list = self.utils.apply_package_pattern(data, slackbuilds)
 
         self.repo_tag: str = self.repos.repositories[repository]['repo_tag']
         self.tar_suffix: str = self.repos.repositories[repository]['tar_suffix']
 
     def execute(self) -> None:
-        """ Calls the methods in order.
-        """
+        """Call the methods in order."""
         self.view_process.message('Resolving dependencies')
         self.creating_dependencies_list()
         self.choose_package_dependencies()
         self.add_dependencies_to_install_order()
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
         self.check_for_skipped()
 
         self.view_slackbuilds_before_build()
-        self.view.missing_dependencies(self.install_order)
+        self.view.missing_dependencies(self.build_order)
         self.view.question()
 
         start: float = time.time()
         self.view.skipping_packages(self.skipped_packages)
         self.prepare_slackbuilds_for_build()
         self.download_the_sources()
         self.set_progress_message()
         self.build_and_install_the_slackbuilds()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
-        """ Creates the package dependencies list.
-        """
+        """Create the package dependencies list."""
         for slackbuild in self.slackbuilds:
             dependencies: tuple = Requires(self.data, slackbuild, self.flags).resolve()
 
             for dependency in dependencies:
                 self.dependencies.append(dependency)
 
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
-        """ Adds the dependency list in order for install.
-        """
-        self.install_order.extend(self.dependencies)
+        """Add the dependency list in order for install."""
+        self.build_order.extend(self.dependencies)
 
     def clean_the_main_slackbuilds(self) -> None:
-        """ Removes main packages if they already added as dependency.
-        """
+        """Remove main packages if they already added as dependency."""
         for dep in self.dependencies:
             if dep in self.slackbuilds:
                 self.slackbuilds.remove(dep)
 
     def add_main_packages_to_install_order(self) -> None:
-        """ Adds the main packages to order for install.
-        """
-        self.install_order.extend(self.slackbuilds)
+        """Add the main packages to order for install."""
+        self.build_order.extend(self.slackbuilds)
 
     def check_for_skipped(self) -> None:
-        """ Checks packages for skipped.
-        """
+        """Check packages for skipped."""
         if self.option_for_skip_installed:
-            for name in self.install_order:
+            for name in self.build_order:
                 installed: str = self.utils.is_package_installed(name)
                 if installed:
                     self.skipped_packages.append(name)
 
         # Remove packages from skipped packages.
-        self.install_order: list = [pkg for pkg in self.install_order if pkg not in self.skipped_packages]
+        self.build_order: list = [pkg for pkg in self.build_order if pkg not in self.skipped_packages]
 
     def view_slackbuilds_before_build(self) -> None:
-        """ View packages before build.
-        """
+        """View packages before build."""
         if self.mode == 'build':
             self.view.build_packages(self.slackbuilds, self.dependencies)
         else:
             self.view.install_upgrade_packages(self.slackbuilds, self.dependencies, self.mode)
 
     def prepare_slackbuilds_for_build(self) -> None:
-        """ Prepare slackbuilds for build.
-        """
-        if self.install_order:
+        """Prepare slackbuilds for build."""
+        if self.build_order:
             self.view_process.message('Prepare sources for downloading')
-            for sbo in self.install_order:
+            for sbo in self.build_order:
                 build_path: Path = Path(self.build_path, sbo)
 
-                self.utils.remove_folder_if_exists(build_path)
+                # self.utils.remove_folder_if_exists(build_path)
                 location: str = self.data[sbo]['location']
                 slackbuild: Path = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
 
                 # Copy slackbuilds to the build folder.
-                path_repo_package: Path = Path(self.repos.repositories[self.repository]['path'], location, sbo)
-                shutil.copytree(path_repo_package, build_path)
+                repo_package: Path = Path(self.repos.repositories[self.repository]['path'], location, sbo)
+
+                shutil.copytree(repo_package, build_path, dirs_exist_ok=True)
 
                 os.chmod(slackbuild, 0o775)
 
                 if self.os_arch == 'x86_64' and self.data[sbo]['download64']:
                     sources: tuple = self.data[sbo]['download64']
                 else:
-                    sources: tuple = self.data[sbo]['download']  # type: ignore[no-redef]
+                    sources: tuple = self.data[sbo]['download']
 
                 if self.gpg_verification and self.repository == self.repos.sbo_repo_name:
                     asc_file: Path = Path(self.repos.repositories_path, self.repos.sbo_repo_name,
                                           location, f'{sbo}{self.tar_suffix}.asc')
                     self.asc_files.append(asc_file)
 
                 self.sources[sbo] = (sources, Path(self.build_path, sbo))
 
             self.view_process.done()
 
     def download_the_sources(self) -> None:
-        """ Download the sources.
-        """
+        """Download the sources."""
         if self.sources:
             print(f'Started to download total ({self.cyan}{len(self.sources)}{self.endc}) sources:\n')
             self.download.download(self.sources)
             print()
 
             self.checksum_downloaded_sources()
 
     def checksum_downloaded_sources(self) -> None:
-        """ Checksum the sources.
-        """
-        for sbo in self.install_order:
+        """Checksum the sources."""
+        for sbo in self.build_order:
             path: Path = Path(self.build_path, sbo)
 
             if self.os_arch == 'x86_64' and self.data[sbo]['md5sum64']:
                 checksums: list = self.data[sbo]['md5sum64']
                 sources: list = self.data[sbo]['download64']
             else:
                 checksums: list = self.data[sbo]['md5sum']
                 sources: list = self.data[sbo]['download']
 
             for source, checksum in zip(sources, checksums):
                 self.check_md5.md5sum(path, source, checksum)
 
     def build_and_install_the_slackbuilds(self) -> None:
-        """ Builds an install the slackbuilds.
-        """
-        # Remove old slpkg.log file.
-        if self.slpkg_log_file.is_file():
+        """Build or install the slackbuilds."""
+        if self.slpkg_log_file.is_file():  # Remove old slpkg.log file.
             self.slpkg_log_file.unlink()
 
         if self.gpg_verification and self.repository == self.repos.sbo_repo_name:
             self.gpg.verify(self.asc_files)
 
-        if self.install_order:
-            print(f'Started the processing of ({self.cyan}{len(self.install_order)}{self.endc}) packages:\n')
+        if self.build_order:
+            print(f'Started the processing of ({self.cyan}{len(self.build_order)}{self.endc}) packages:\n')
 
-            for sbo in self.install_order:
+            for sbo in self.build_order:
                 self.patch_slackbuild_tag(sbo)
                 self.build_the_script(self.build_path, sbo)
 
                 if self.mode in ('install', 'upgrade'):
                     self.install_package(sbo)
 
+                if self.delete_sources:
+                    sbo_build_folder: Path = Path(self.build_path, sbo)
+                    self.utils.remove_folder_if_exists(sbo_build_folder)
+
     def patch_slackbuild_tag(self, sbo: str) -> None:
-        """ Patch the slackbuild tag.
+        """Patch the slackbuild tag.
 
         Args:
             sbo (str): Slackbuild name.
         """
         sbo_script: Path = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
         if sbo_script.is_file() and self.repo_tag:
             lines: list = self.utils.read_text_file(sbo_script)
@@ -236,30 +226,30 @@
             with open(sbo_script, 'w', encoding='utf-8') as script:
                 for line in lines:
                     if line.startswith('TAG=$'):
                         line: str = f'TAG=${{TAG:-{self.repo_tag}}}\n'
                     script.write(line)
 
     def install_package(self, name: str) -> None:
-        """ Install the slackbuild.
+        """Install the slackbuild.
 
         Args:
             name (str): Slackbuild name.
         """
         package: str = self.find_package_for_install(name)
 
         command: str = f'{self.installpkg} {self.tmp_path}/{package}'
         if self.option_for_reinstall:
             command: str = f'{self.reinstall} {self.tmp_path}/{package}'
 
         self.multi_proc.process_and_log(command, package, self.progress_message)
         self.write_deps_log(name)
 
     def write_deps_log(self, name: str) -> None:
-        """ Creates a log file with Slackbuild dependencies.
+        """Create a log file with Slackbuild dependencies.
 
         Args:
             name (str): Slackbuild name.
         """
         deps: dict = {}
         deps_logs: dict = {}
         installed_requires: list = []
@@ -272,15 +262,15 @@
         deps[name] = installed_requires
         if self.deps_log_file.is_file():
             deps_logs: dict = self.utils.read_json_file(self.deps_log_file)
             deps_logs.update(deps)
         self.deps_log_file.write_text(json.dumps(deps_logs, indent=4), encoding='utf-8')
 
     def find_package_for_install(self, name: str) -> str:
-        """ Find build slackbuilds for install.
+        """Find build slackbuilds for install.
 
         Args:
             name (str): Package name.
 
         Returns:
             str: Package file.
         """
@@ -291,42 +281,39 @@
             return max(packages)
         except ValueError:
             self.errors.raise_error_message(f"Package '{name}' not found for install", exit_status=20)
 
         return None
 
     def build_the_script(self, path: Path, name: str) -> None:
-        """ Builds the slackbuild script.
+        """Build the slackbuild script.
 
         Args:
             path (Path): Path to build the script.
             name (str): Slackbuild name.
         """
         self.set_makeflags()
         folder: Path = Path(path, name)
         filename: str = f'{name}.SlackBuild'
         command: str = f'{folder}/./{filename}'
         self.utils.change_owner_privileges(folder)
         progress_message: str = f'{self.red}Building{self.endc}'
         self.multi_proc.process_and_log(command, filename, progress_message)
 
     def set_progress_message(self) -> None:
-        """ Set progress message for upgrade.
-        """
+        """Set progress message for upgrade."""
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.progress_message: str = f'{self.violet}Upgrading{self.endc}'
 
     def set_makeflags(self) -> None:
-        """ Set makeflags.
-        """
+        """Set makeflags."""
         os.environ['MAKEFLAGS'] = f'-j {self.makeflags}'
 
     def choose_package_dependencies(self) -> None:
-        """ Choose dependencies for install with dialog tool.
-        """
+        """Choose dependencies for install with dialog tool."""
         if self.dependencies and self.dialog:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = ' Choose dependencies you want to install '
```

### Comparing `slpkg-5.0.8/slpkg/search.py` & `slpkg-5.0.9/slpkg/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
 class SearchPackage(Configs):  # pylint: disable=[R0902]
-
-    """
-    Search packages from the repositories.
-    """
+    """Search packages from the repositories."""
 
     def __init__(self, flags: list, packages: list, data: dict, repository: str):
         super(Configs, self).__init__()
         self.packages: list = packages
         self.data: dict = data
         self.repository: str = repository
 
@@ -29,35 +26,33 @@
         self.option_for_no_case: bool = self.utils.is_option(
             ('-m', '--no-case'), flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def search(self) -> None:
-        """ Choose between all and one repository.
-        """
+        """Choose between all and one repository."""
         if self.repository == '*':
             self.search_to_all_repositories()
         else:
             self.repo_data: dict = self.data
             self.search_for_the_packages(self.repository)
 
         print('The list below shows the repository packages:\n')
         self.summary_of_searching()
 
     def search_to_all_repositories(self) -> None:
-        """ Search package name to all enabled repositories.
-        """
+        """Search package name to all enabled repositories."""
         all_data: dict = self.data
         for name, repo in all_data.items():
             self.repo_data: dict = repo
             self.search_for_the_packages(name)
 
     def search_for_the_packages(self, repo: str) -> None:
-        """ Search for packages and save in a dictionary.
+        """Search for packages and save in a dictionary.
 
         Args:
             repo (str): repository name.
         """
         for package in self.packages:
             for name, data_pkg in sorted(self.repo_data.items()):
 
@@ -67,16 +62,15 @@
                     self.data_dict[self.matching] = {
                         'repository': repo,
                         'name': name,
                         'version': data_pkg['version']
                     }
 
     def summary_of_searching(self) -> None:
-        """ Prints the result.
-        """
+        """Print the result."""
         try:
             repo_length: int = max(len(repo['repository']) for repo in self.data_dict.values())
         except ValueError:
             repo_length: int = 1
 
         try:
             name_length: int = max(len(name['name']) for name in self.data_dict.values())
@@ -96,15 +90,15 @@
                       f"{self.yellow}{version}{self.endc}")
 
             print(f'\n{self.grey}Total found {self.matching} packages.{self.endc}')
         else:
             print('\nDoes not match any package.\n')
 
     def is_not_case_sensitive(self, package: str, name: str) -> bool:
-        """ Check for case sensitive.
+        """Check for case sensitive.
 
         Args:
             package (str): Package file.
             name (str): Package name.
 
         Returns:
             bool: True or False.
```

### Comparing `slpkg-5.0.8/slpkg/tracking.py` & `slpkg-5.0.9/slpkg/tracking.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 from slpkg.sbos.dependencies import Requires
 from slpkg.binaries.required import Required
 
 
 class Tracking(Configs):  # pylint: disable=[R0902]
-
-    """
-    Tracking of the package dependencies.
-    """
+    """Tracking of the package dependencies."""
 
     def __init__(self, data: dict, packages: list, flags: list, repository: str):
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
         self.repository: str = repository
@@ -37,16 +34,15 @@
         self.count_requires: int = 0
         self.require_length: int = 0
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def package(self) -> None:
-        """ Call methods and prints the results.
-        """
+        """Call methods and prints the results."""
         self.view_the_title()
 
         for package in self.packages:
             self.count_requires: int = 0
 
             self.set_the_package_line(package)
             self.set_package_requires(package)
@@ -58,52 +54,48 @@
 
                 self.set_the_package_require_line(require)
                 self.view_requires()
 
             self.view_summary_of_tracking(package)
 
     def view_the_title(self) -> None:
-        """ Prints the title.
-        """
+        """Print the title."""
         print("The list below shows the packages with dependencies:\n")
         self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
 
     def view_the_main_package(self) -> None:
-        """ Prints the main package.
-        """
+        """Print the main package."""
         print(self.package_line)
         print(f"{'':>1}{self.llc}{self.hl}", end='')
 
     def view_requires(self) -> None:
-        """ Prints the requires.
-        """
+        """Print the requires."""
         if self.count_requires == 1:
             print(f"{'':>1}{self.require_line}")
         else:
             print(f"{'':>4}{self.require_line}")
 
     def view_no_dependencies(self) -> None:
-        """ Prints the message 'No dependencies'.
-        """
+        """Print the message 'No dependencies'."""
         if not self.package_requires:
             print(f"{'':>1}{self.cyan}No dependencies{self.endc}")
 
     def set_the_package_line(self, package: str) -> None:
-        """ Sets for package line.
+        """Set for package line.
 
         Args:
             package (str): Package name.
         """
         self.package_line: str = f'{self.yellow}{package}{self.endc}'
         if self.option_for_pkg_version:
             self.set_package_version(package)
             self.package_line: str = f'{self.yellow}{package} {self.package_version}{self.endc}'
 
     def set_the_package_require_line(self, require: str) -> None:
-        """ Sets the requires.
+        """Set the requires.
 
         Args:
             require (str): Require name.
         """
         color: str = self.cyan
         if require not in self.data:
             color: str = self.red
@@ -112,53 +104,52 @@
 
         if self.option_for_pkg_version:
             self.set_package_dependency_version(require)
             self.require_line: str = (f'{color}{require:<{self.require_length}}{self.endc}'
                                       f'{self.package_dependency_version}')
 
     def set_package_dependency_version(self, require: str) -> None:
-        """ Sets the dependency version.
+        """Set the dependency version.
 
         Args:
             require (str): Description
         """
         self.package_dependency_version: str = f"{'':>1}(not included)"
         if self.data.get(require):
             self.package_dependency_version: str = (
                 f"{'':>1}{self.yellow}{self.data[require]['version']}{self.endc}"
             )
 
     def set_package_version(self, package: str) -> None:
-        """ Sets the main package version.
+        """Set the main package version.
 
         Args:
             package (str): Package name.
         """
         self.package_version: str = self.data[package]['version']
 
     def set_package_requires(self, package: str) -> None:
-        """ Sets for the package require.
+        """Set for the package require.
 
         Args:
             package (str): Package name.
         """
-
         if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
             self.package_requires: list = list(Required(self.data, package, self.flags).resolve())
         else:
             self.package_requires: list = list(Requires(self.data, package, self.flags).resolve())
 
         if self.package_requires:
             if self.view_missing_deps:
                 requires: list = self.data[package]['requires']
                 for req in requires:
                     if req not in self.data:
                         self.package_requires.append(req)
             self.require_length: int = max(len(name) for name in self.package_requires)
 
     def view_summary_of_tracking(self, package: str) -> None:
-        """ Prints the summary.
+        """Print the summary.
 
         Args:
             package (str): Package name.
         """
         print(f'\n{self.grey}{self.count_requires} dependencies for {package}{self.endc}\n')
```

### Comparing `slpkg-5.0.8/slpkg/update_repositories.py` & `slpkg-5.0.9/slpkg/update_repositories.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,15 @@
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
 from slpkg.check_updates import CheckUpdates
 from slpkg.sbos.sbo_generate import SBoGenerate
 
 
 class UpdateRepositories(Configs):  # pylint: disable=[R0902]
-
-    """
-    Updates the local repositories and install the data
-    into the database.
-    """
+    """Update the local repositories."""
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
 
         self.view = View(flags)
         self.multi_process = MultiProcess(flags)
         self.repos = Repositories()
@@ -38,28 +34,27 @@
 
         self.repos_for_update: dict = {}
 
         self.option_for_yes: bool = self.utils.is_option(
             ('-y', '--yes'), flags)
 
     def repositories(self) -> None:
-        """ Checks and call the repositories for update.
-        """
+        """Check and call the repositories for update."""
         self.repos_for_update: dict = self.check_updates.updates()
 
         if not any(list(self.repos_for_update.values())):
             self.view.question(message='Do you want to force update?')
             # Force update the repositories.
             for repo in self.repos_for_update:
                 self.repos_for_update[repo] = True
 
         self.run_update()
 
     def import_gpg_key(self, repo: str) -> None:
-        """ Imports the GPG KEY.
+        """Import the GPG KEY.
 
         Args:
             mirror (str): Repository GPG mirror key.
         """
         if self.gpg_verification:
             mirror: str = self.repos.repositories[repo]['mirror_changelog']
 
@@ -87,35 +82,34 @@
                         return
 
             output: str = re.split(r"/|\s", process.stdout)
             if process.returncode == 0 and 'imported:' in output:
                 print(f'Getting GPG key from: {mirror}\n')
 
     def run_update(self) -> None:
-        """ Update the repositories by category.
-        """
+        """Update the repositories by category."""
         for repo, update in self.repos_for_update.items():
             if update:
 
                 self.view_downloading_message(repo)
                 if repo in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
                     self.update_slackbuild_repos(repo)
                 else:
                     self.update_binary_repos(repo)
 
     def view_downloading_message(self, repo: str) -> None:
-        """ Prints the syncing message.
+        """Print the syncing message.
 
         Args:
             repo (str): Repository name.
         """
         print(f"Syncing with the repository '{self.green}{repo}{self.endc}', please wait...\n")
 
     def update_binary_repos(self, repo: str) -> None:
-        """Updates the binary repositories.
+        """Update the binary repositories.
 
         Args:
             repo (str): Repository name.
         """
         urls: dict = {}
 
         self.import_gpg_key(repo)
@@ -139,15 +133,15 @@
         self.utils.create_directory(self.repos.repositories[repo]['path'])
 
         self.download.download(urls)
 
         self.data.install_binary_data(repo)
 
     def update_slackbuild_repos(self, repo: str) -> None:
-        """Updates the slackbuild repositories.
+        """Update the slackbuild repositories.
 
         Args:
             repo (str): Repository name.
         """
         # self.import_gpg_key(mirror='https://www.slackbuilds.org/')
         self.import_gpg_key(repo)
```

### Comparing `slpkg-5.0.8/slpkg/upgrade.py` & `slpkg-5.0.9/slpkg/upgrade.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 from slpkg.load_data import LoadData
 
 
 class Upgrade(Configs):  # pylint: disable=[R0902]
-
-    """
-    Upgrade the installed packages.
-    """
+    """Upgrade the installed packages."""
 
     def __init__(self, repository: str, data: dict):
         super(Configs, self).__init__()
         self.repository: str = repository
         self.data: dict = data
 
         self.utils = Utilities()
@@ -35,16 +32,18 @@
         self.sum_added: int = 0
         self.installed_names: list = []
         self.installed_packages: list = []
 
         self.kernel_ver: str = platform.uname()[2]
         self.columns, self.rows = shutil.get_terminal_size()
 
+        self.check_run: bool = False
+
     def load_installed_packages(self, repository: str) -> None:
-        """Summary
+        """Load installed packages.
 
         Args:
             repository (str): Repository name.
         """
         if repository == self.repos.slack_repo_name:
             extra_repo: dict = {}
 
@@ -68,16 +67,15 @@
                         self.installed_packages.append(Path(package))
                         self.installed_names.append(name)
         else:
             repo_tag: str = self.repos.repositories[repository]['repo_tag']
             self.installed_packages: list = list(self.log_packages.glob(f'*{repo_tag}'))
 
     def packages(self) -> Generator:
-        """ Returns the upgradeable packages.
-        """
+        """Return the upgradeable packages."""
         # Delete log file before starts.
         if self.upgrade_log_file.is_file():
             self.upgrade_log_file.unlink()
 
         self.load_installed_packages(self.repository)
 
         for inst in self.installed_packages:
@@ -92,15 +90,15 @@
         if self.repository in self.repos.new_packages:
             for name in self.data.keys():
                 # if not self.utils.is_package_installed(name):
                 if name not in self.installed_names:
                     yield name
 
     def is_package_upgradeable(self, installed: str) -> bool:  # pylint: disable=[R0911]
-        """Returns True for upgradeable packages.
+        """Return True for upgradeable packages.
 
         Args:
             installed (str): Installed package.
 
         Returns:
             bool: True if the package is upgradeable.
         """
@@ -119,45 +117,40 @@
             try:
                 if parse(repo_version) > parse(inst_version):
                     return True
 
                 if parse(repo_version) == parse(inst_version) and int(repo_build) > int(inst_build):
                     return True
             except InvalidVersion as err:
-                # Different options to compare packages.
-                repo_package: str = self.data[inst_name]['package']
                 if repo_version > inst_version:  # Try to compare the strings.
                     return True
                 if repo_version == inst_version and int(repo_build) > int(inst_build):
                     return True
-                if installed != repo_package[:-4]:  # Add the package if a new one on the repository.
-                    return True
-                if installed == repo_package[:-4]:  # Not new packages in the repository.
-                    return False
                 self._write_log_file(installed, inst_name, err)
 
         return False
 
     def _write_log_file(self, installed: str, name: str, err: InvalidVersion) -> None:
-        """Writes a log file for invalid versions.
+        """Write a log file for invalid versions.
 
         Args:
             installed (str): Installed package.
             name (str): Package name.
             err (InvalidVersion): InvalidVersion error.
         """
         if self.log_path.is_dir():
             with self.upgrade_log_file.open('a', encoding='utf-8') as log:
                 log.write(f"Installed: {installed}, "
                           f"Repository: {self.data[name]['package']}, "
-                          f"Error: {err}\n")
+                          f"Error: {err}, "
+                          f"Repo: {self.repository}\n")
 
     def check_packages(self) -> None:
-        """ Checks only which packages are upgradeable.
-        """
+        """Check only which packages are upgradeable."""
+        self.check_run: bool = True
         repo_data: dict = {}
         found_packages: dict = {}
 
         if self.repository == '*':
             repo_data: dict = self.data
         else:
             repo_data[self.repository] = self.data
@@ -225,15 +218,15 @@
                             'repo_build': repo_build,
                             'repo': self.repos.slack_repo_name,
                             'type': 'add'
                         }
         self._results(found_packages)
 
     def _results(self, found_packages: dict) -> None:
-        """ Prints the results of checking.
+        """Print the results of checking.
 
         Args:
             found_packages (dict): Data of packages.
 
         Raises:
             SystemExit: Exit code 0.
         """
```

### Comparing `slpkg-5.0.8/slpkg/utilities.py` & `slpkg-5.0.9/slpkg/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,27 +14,24 @@
 
 from slpkg.configs import Configs
 from slpkg.blacklist import Blacklist
 from slpkg.error_messages import Errors
 
 
 class Utilities(Configs):
-
-    """
-    List of utilities.
-    """
+    """List of utilities."""
 
     def __init__(self):
         super(Configs, self).__init__()
 
         self.black = Blacklist()
         self.errors = Errors()
 
     def is_package_installed(self, name: str) -> str:
-        """Returns the installed package binary.
+        """Return the installed package binary.
 
         Args:
             name (str): Package name.
 
         Returns:
             str: Full package name.
         """
@@ -77,35 +74,35 @@
         """
         archive: Path = Path(path, file)
         if archive.is_file():
             archive.unlink()
 
     @staticmethod
     def remove_folder_if_exists(folder: Path) -> None:
-        """Removes the folder if exist.
+        """Remove the folder if exist.
 
         Args:
             folder (Path): Path to the folder.
         """
         if folder.exists():
             shutil.rmtree(folder)
 
     @staticmethod
     def create_directory(directory: Path) -> None:
-        """Creates folder like mkdir -p.
+        """Create folder like mkdir -p.
 
         Args:
             directory (Path): Path to folder.
         """
         if not directory.is_dir():
             directory.mkdir(parents=True, exist_ok=True)
 
     @staticmethod
     def split_package(package: str) -> dict:
-        """Splits the binary package name in name, version, arch, build and tag.
+        """Split the binary package name in name, version, arch, build and tag.
 
         Args:
             package (str): Full package name for spliting.
 
         Returns:
             dict: Splitted package by name, version, arch, build and package tag.
         """
@@ -122,39 +119,39 @@
             'arch': arch,
             'build': build,
             'tag': pkg_tag
         }
 
     @staticmethod
     def finished_time(elapsed_time: float) -> None:
-        """Printing the elapsed time.
+        """Print the elapsed time.
 
         Args:
             elapsed_time (float): Unformatted time.
         """
         print('\nFinished:', time.strftime('%H:%M:%S', time.gmtime(elapsed_time)))
 
     @staticmethod
     def is_option(options: tuple, flags: list) -> bool:
-        """Returns True if option applied.
+        """Return True if option applied.
 
         Args:
             options (tuple): Options for checking.
             flags (list): The flags applied by the user.
 
         Returns:
             bool: True if match or False, if not matched.
         """
         for option in options:
             if option in flags:
                 return True
         return False
 
     def read_packages_from_file(self, file: Path) -> Generator:
-        """Reads name packages from file.
+        """Read packages from file.
 
         Args:
             file (Path): Path to the file.
 
         Yields:
             Generator: Package names.
         """
@@ -167,15 +164,15 @@
                     if '#' in package:
                         package: str = package.split('#')[0].strip()
                     yield package
         except FileNotFoundError:
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
     def read_text_file(self, file: Path) -> list:
-        """Reads a text file.
+        """Read a text file.
 
         Args:
             file (Path): Path to the file.
 
         Returns:
             list: The lines in the list.
         """
@@ -183,17 +180,18 @@
             with open(file, 'r', encoding='utf-8', errors='replace') as text_file:
                 return text_file.readlines()
         except FileNotFoundError:
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
         return []
 
     def count_file_size(self, name: str) -> int:
-        """
-        Read the contents files from the package file list and count
-        the total installation file size in bytes.
+        """Count the file size.
+
+        Read the contents files from the package file list
+        and count the total installation file size in bytes.
         Args:
             name: The name of the package.
 
         Returns:
             The total package installation file size.
         """
         count_files: int = 0
@@ -204,16 +202,16 @@
                 file: Path = Path('/', line)
                 if file.is_file():
                     count_files += file.stat().st_size
         return count_files
 
     @staticmethod
     def convert_file_sizes(byte_size: float) -> str:
-        """
-        Convert bytes to kb, mb and gb.
+        """Convert bytes to kb, mb and gb.
+
         Args:
             byte_size: The file size in bytes.
         Returns:
             The size converted.
         """
         kb_size: float = byte_size / 1024
         mb_size: float = kb_size / 1024
@@ -243,15 +241,15 @@
             if pkg == '*':
                 packages.remove('*')
                 packages.extend(list(data.keys()))
         return packages
 
     @staticmethod
     def change_owner_privileges(folder: Path) -> None:
-        """Changes the owner privileges.
+        """Change the owner privileges.
 
         Args:
             folder (Path): Path to the folder.
         """
         os.chown(folder, 0, 0)
         for file in os.listdir(folder):
             os.chown(Path(folder, file), 0, 0)
@@ -274,16 +272,16 @@
                     if package.lower() == pkg.lower():
                         packages.append(pkg)
                         packages.remove(package)
                         break
         return packages
 
     def read_json_file(self, file: Path) -> dict:
-        """
-        Read JSON data from the file.
+        """Read JSON data from the file.
+
         Args:
             file: Path file for reading.
         Returns:
             Dictionary with data.
         """
         json_data: dict = {}
         try:
@@ -291,30 +289,30 @@
         except FileNotFoundError:
             self.errors.raise_error_message(f'{file} not found.', exit_status=1)
         except json.decoder.JSONDecodeError:
             pass
         return json_data
 
     def ignore_packages(self, packages: list) -> list:
-        """
-        Matching packages using regular expression.
+        """Match packages using regular expression.
+
         Args:
             packages: The packages to apply the pattern.
         Returns:
             The matching packages.
         """
         matching_packages: list = []
         blacklist: tuple = self.black.packages()
         if blacklist:
             pattern: str = '|'.join(blacklist)
             matching_packages: list = [pkg for pkg in packages if re.search(pattern, pkg)]
         return matching_packages
 
     def convert_dict_keys_to_lower(self, d: dict) -> dict:
-        """ Converts dictionary keys to lower.
+        """Convert dictionary keys to lower.
 
         Args:
             d (dict): Dictionary data.
 
         Returns:
             dict: Dictionary in lower case.
         """
```

### Comparing `slpkg-5.0.8/slpkg/views/asciibox.py` & `slpkg-5.0.9/slpkg/views/asciibox.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,24 @@
 
 import shutil
 
 from slpkg.configs import Configs
 
 
 class AsciiBox(Configs):  # pylint: disable=[R0902]
-
-    """
-    Managing the ASCII characters.
-    """
+    """Managing the ASCII characters."""
 
     def __init__(self):
         super(Configs, self).__init__()
         self.columns, self.rows = shutil.get_terminal_size()
         self.package_alignment: int = self.columns - 56
         self.version_alignment: int = 29
         self.size_alignment: int = 9
         self.repo_alignment: int = 14
 
-        # if self.package_alignment < 1:
-        #     self.package_alignment = 1
-
         self.package_alignment = max(self.package_alignment, 1)
 
         self.bd_color: str = self.endc
         self.border_colors: dict = {}
         self.assign_border_color()
 
         self.bullet: str = '-'
@@ -46,31 +40,30 @@
         self.horizontal_and_down: str = '+'
         self.vertical_and_right: str = '+'
         self.vertical_and_left: str = '+'
 
         if self.ascii_characters:
             self.bullet: str = '•'
             self.done: str = '✔️'
-            self.failed: str = 'X'
+            self.failed: str = '✖️'
             self.skipped: str = '↪'
             self.vertical_line: str = '│'
             self.horizontal_line: str = '─'
             self.horizontal_vertical: str = '┼'
             self.upper_right_corner: str = '┐'
             self.lower_left_corner: str = '└'
             self.lower_right_corner: str = '┘'
             self.upper_left_corner: str = '┌'
             self.horizontal_and_up: str = '┴'
             self.horizontal_and_down: str = '┬'
             self.vertical_and_right: str = '├'
             self.vertical_and_left: str = '┤'
 
     def assign_border_color(self) -> None:
-        """ Assign the colors.
-        """
+        """Assign the colors."""
         self.border_colors: dict = {
             'red': self.red,
             'blue': self.blue,
             'cyan': self.cyan,
             'white': self.endc,
             'green': self.green,
             'yellow': self.yellow,
@@ -82,15 +75,15 @@
         }
         try:
             self.bd_color: str = self.border_colors[self.border_color]
         except KeyError:
             self.bd_color: str = self.endc
 
     def draw_package_title(self, message: str, title: str) -> None:
-        """ Draw the package title.
+        """Draw the package title.
 
         Args:
             message (str): Message about the action.
             title (str): Slpkg title.
         """
         title = title.title()
         print(f"{self.bd_color}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
@@ -101,15 +94,15 @@
               f"{self.bd_color}{self.vertical_line}")
         self.draw_middle_line()
         print(f"{self.bd_color}{self.vertical_line}{self.endc} {'Package:':<{self.package_alignment}}"
               f"{'Version:':<{self.version_alignment}}{'Size:':<{self.size_alignment}}{'Repo:':>{self.repo_alignment}} "
               f"{self.bd_color}{self.vertical_line}{self.endc}")
 
     def draw_package_line(self, package: str, version: str, size: str, color: str, repo: str) -> None:  # pylint: disable=[R0913]
-        """ Draw the package line.
+        """Draw the package line.
 
         Args:
             package (str): Package name.
             version (str): Package version.
             size (str): Package size.
             color (str): Package highlight.
             repo (str): Repository name.
@@ -120,33 +113,30 @@
             package: str = f'{package[:self.package_alignment - 4]}...'
 
         print(f"{self.bd_color}{self.vertical_line} {self.bold}{color}{package:<{self.package_alignment}}{self.endc}"
               f"{self.bd_color}{version:<{self.version_alignment}}{self.endc}{size:<{self.size_alignment}}{self.blue}"
               f"{repo:>{self.repo_alignment}}{self.bd_color} {self.vertical_line}{self.endc}")
 
     def draw_middle_line(self) -> None:
-        """ Draw the middle line
-        """
+        """Draw the middle line."""
         print(f"{self.bd_color}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
               f"{self.vertical_and_left}")
 
     def draw_dependency_line(self) -> None:
-        """ Draw the dependency line.
-        """
+        """Draw the dependency line."""
         print(f"{self.bd_color}{self.vertical_line}{self.endc} Dependencies:{' ' * (self.columns - 16)}"
               f"{self.bd_color}{self.vertical_line}{self.endc}")
 
     def draw_bottom_line(self) -> None:
-        """ Draw the bottom line.
-        """
+        """Draw the bottom line."""
         print(f"{self.bd_color}{self.lower_left_corner}{self.horizontal_line * (self.columns - 2)}"
               f"{self.lower_right_corner}{self.endc}")
 
     def draw_checksum_error_box(self, name: str, checksum: str, file_check: str) -> None:
-        """ Draw a checksum error box.
+        """Draw a checksum error box.
 
         Args:
             name (str): Package name.
             checksum (str): Expected checksum.
             file_check (str): Found checksum.
         """
         print(f"{self.bred}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
```

### Comparing `slpkg-5.0.8/slpkg/views/cli_menu.py` & `slpkg-5.0.9/slpkg/views/cli_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 
 from typing import NoReturn
 from slpkg.configs import Configs
 from slpkg.views.version import Version
 
 
 class Usage(Configs):
-
-    """
-    CLI Usage menu.
-    """
+    """CLI Usage menu."""
 
     def __init__(self):
         super(Configs, self).__init__()
 
     def help_minimal(self, message: str) -> NoReturn:
-        """ Prints the minimal help menu.
+        """Print the minimal help menu.
 
         Args:
             message (str): Message of error.
 
         Raises:
             SystemExit: Raises an exit code 1.
         """
@@ -31,15 +28,15 @@
             f'<packages>\n'
             f"\nTry '{self.prog_name} --help' for more options.")
 
         print(args)
         raise SystemExit(1)
 
     def help_short(self, status: int) -> NoReturn:
-        """Prints the short menu.
+        """Print the short menu.
 
         Args:
             status (int): Status exit code.
 
         Raises:
             SystemExit: Raises the status code.
         """
@@ -58,15 +55,15 @@
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-o, --repository=NAME, -z, --directory=PATH]\n'
             "  \nIf you need more information please try 'slpkg --help'.")
 
         print(args)
         raise SystemExit(status)
 
     def help(self, status: int) -> NoReturn:
-        """Prints the main menu.
+        """Print the main menu.
 
         Args:
             status (int): Status exit code
 
         Raises:
             SystemExit: Raises the status code.
         """
```

### Comparing `slpkg-5.0.8/slpkg/views/version.py` & `slpkg-5.0.9/slpkg/views/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
 class Version:  # pylint: disable=[R0903]
-    """ Print the version. """
+    """Print the version."""
 
     def __init__(self):
-        self.version: str = "5.0.8"
+        self.version: str = "5.0.9"
         self.license: str = 'GNU General Public License v3 (GPLv3)'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
         self.email: str = 'dslackw@gmail.com'
 
     def view(self) -> None:
-        """ Prints the version. """
+        """Print the version."""
         print(f'Version: {self.version}\n'
               f'Author: {self.author}\n'
               f'License: {self.license}\n'
               f'Homepage: {self.homepage}\n'
               f'Email: {self.email}')
```

### Comparing `slpkg-5.0.8/slpkg/views/view_package.py` & `slpkg-5.0.9/slpkg/views/view_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 
 
 class ViewPackage(Configs):  # pylint: disable=[R0902]
-
-    """
-    View the packages information.
-    """
+    """View the packages information."""
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
 
         self.flags: list = flags
         self.repository: str = repository
 
@@ -68,37 +65,35 @@
                     self.assign_the_sbo_mirror()
                     self.assign_the_info_file_variables()
                     self.assign_dependencies(item)
                     self.assign_dependencies_with_version(item, data)
                     self.view_slackbuild_package(name, item)
 
     def read_the_readme_file(self, path_file: Path) -> None:
-        """ Reads the README file.
+        """Read the README file.
 
         Args:
             path_file (Path): Path to the file.
         """
         self.readme: list = self.utils.read_text_file(path_file)
 
     def read_the_info_file(self, path_info: Path) -> None:
-        """ reads the .info file.
+        """Read the .info file.
 
         Args:
             path_info (Path): Path to the file.
         """
         self.info_file: list = self.utils.read_text_file(path_info)
 
     def assign_the_sbo_mirror(self) -> None:
-        """ Assign the url for the PACKAGES.TXT file.
-        """
+        """Assign the url for the PACKAGES.TXT file."""
         self.mirror: str = self.repos.repositories[self.repository]['mirror_packages']
 
     def assign_the_info_file_variables(self) -> None:
-        """ Assign data from the .info file.
-        """
+        """Assign data from the .info file."""
         for line in self.info_file:
             if line.startswith('HOMEPAGE'):
                 self.homepage: str = line[10:-2].strip()
             if line.startswith('MAINTAINER'):
                 self.maintainer: str = line[12:-2].strip()
             if line.startswith('EMAIL'):
                 self.email: str = line[7:-2].strip()
@@ -108,28 +103,28 @@
 
         Args:
             item (dict): Data value.
         """
         self.dependencies: str = ', '.join([f'{self.cyan}{pkg}' for pkg in item['requires']])
 
     def assign_dependencies_with_version(self, item: dict, data: dict) -> None:
-        """ Assign dependencies with version.
+        """Assign dependencies with version.
 
         Args:
             item (dict): Data value.
             data (dict): Repository data.
         """
         if self.option_for_pkg_version:
             self.dependencies: str = (', '.join(
                 [f"{self.cyan}{pkg}{self.endc}-{self.yellow}{data[pkg]['version']}"
                  f"{self.green}" for pkg in item['requires']
                  if pkg in self.repository_packages]))
 
     def view_slackbuild_package(self, name: str, item: dict) -> None:
-        """ Prints slackbuild information.
+        """Print slackbuild information.
 
         Args:
             name (str): Slackbuild name.
             item (dict): Data value.
         """
         space_align: str = ''
         print(f"{'Repository':<15}: {self.green}{self.repository}{self.endc}\n"
@@ -149,15 +144,15 @@
               f"{'Maintainer':<15}: {self.yellow}{self.maintainer}{self.endc}\n"
               f"{'Email':<15}: {self.yellow}{self.email}{self.endc}\n"
               f"{'Requires':<15}: {self.green}{self.dependencies}{self.endc}\n"
               f"{'Description':<15}: {self.green}{item['description']}{self.endc}\n"
               f"{'README':<15}: {self.cyan}{f'{space_align:>17}'.join(self.readme)}{self.endc}")
 
     def package(self, data: dict, packages: list) -> None:
-        """ View binary packages information.
+        """View binary packages information.
 
         Args:
             data (dict): Repository data.
             packages (list): List of packages.
         """
         print()
         self.repository_packages: tuple = tuple(data.keys())
@@ -166,15 +161,15 @@
                 if package in [name, '*']:
 
                     self.assign_dependencies(item)
                     self.assign_dependencies_with_version(item, data)
                     self.view_binary_package(name, item)
 
     def view_binary_package(self, name: str, item: dict) -> None:
-        """ Print binary packages information.
+        """Print binary packages information.
 
         Args:
             name (str): Package name.
             item (dict): Data values.
         """
         print(f"{'Repository':<15}: {self.green}{self.repository}{self.endc}\n"
               f"{'Name':<15}: {self.green}{name}{self.endc}\n"
```

### Comparing `slpkg-5.0.8/slpkg/views/view_process.py` & `slpkg-5.0.9/slpkg/views/view_process.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,55 +8,49 @@
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.progress_bar import ProgressBar
 from slpkg.views.asciibox import AsciiBox
 
 
 class ViewProcess(Configs):
-
-    """
-    View the process messages.
-    """
+    """View the process messages."""
 
     def __init__(self, flags: list):
         super(Configs, self).__init__()
 
         self.progress = ProgressBar()
         self.utils = Utilities()
         self.ascii = AsciiBox()
 
         self.bar_process = None
 
         self.option_for_progress_bar: bool = self.utils.is_option(
             ('-B', '--progress-bar'), flags)
 
     def message(self, message: str) -> None:
-        """ Show spinner with message or message.
-        """
+        """Show spinner with message or message."""
         if self.progress_bar_conf or self.option_for_progress_bar:
             self.bar_process = Process(target=self.progress.progress_bar, args=(message,))
             self.bar_process.start()
         else:
             print(f'\r{message}... ', end='')
 
     def done(self) -> None:
-        """ Show done message.
-        """
+        """Show done message."""
         if self.progress_bar_conf or self.option_for_progress_bar:
             time.sleep(0.1)
             self.bar_process.terminate()
             self.bar_process.join()
             print(f'\b{self.bgreen}{self.ascii.done}{self.endc}', end='')
             print('\x1b[?25h')  # Reset cursor after hiding.
         else:
             print(f'{self.bgreen}{self.ascii.done}{self.endc}')
 
     def failed(self) -> None:
-        """ Show for failed message.
-        """
+        """Show for failed message."""
         if self.progress_bar_conf or self.option_for_progress_bar:
             time.sleep(0.1)
             self.bar_process.terminate()
             self.bar_process.join()
             print(f'\b{self.bred}{self.ascii.failed}{self.endc}', end='')
             print('\x1b[?25h')  # Reset cursor after hiding.
         else:
```

### Comparing `slpkg-5.0.8/slpkg/views/views.py` & `slpkg-5.0.9/slpkg/views/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 
 
 class View(Configs):  # pylint: disable=[R0902]
-
-    """ Views packages for build, install, remove or download.
-    """
+    """Views packages for build, install, remove or download."""
 
     def __init__(self, flags: list = None, repository: str = None, data: dict = None):
         super(Configs, self).__init__()
 
         if flags is None:
             flags: list = []
 
@@ -38,138 +36,140 @@
         self.sum_size_comp = 0
         self.sum_size_uncomp = 0
         self.sum_size_remove = 0
         self.columns, self.rows = shutil.get_terminal_size()
 
         self.download_only = None
         self.summary_message: str = ''
+        self.mode = None
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
 
         self.option_for_yes: bool = self.utils.is_option(
             ('-y', '--yes'), flags)
 
     def build_packages(self, slackbuilds: list, dependencies: list) -> None:
-        """ View packages for build method.
+        """View packages for build method.
 
         Args:
             slackbuilds (list): Slackbuilds for build.
             dependencies (list): Dependencies for build.
         """
-        mode: str = 'build'
+        self.mode: str = 'build'
         self.ascii.draw_package_title('The following packages will be build:',
                                       'slpkg build packages')
 
         for slackbuild in slackbuilds:
             self.draw_build_package(slackbuild)
-            self.summary(slackbuild, mode)
+            self.summary(slackbuild)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
             for dependency in dependencies:
                 self.draw_build_package(dependency)
-                self.summary(dependency, mode)
+                self.summary(dependency)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_build(slackbuilds + dependencies)
         print(self.summary_message)
 
     def install_upgrade_packages(self, packages: list, dependencies: list, mode: str) -> None:
-        """ View packages for install or upgrade.
+        """View packages for install or upgrade.
 
         Args:
             packages (list): Packages for install.
             dependencies (list): Dependencies for install.
             mode (str): Type of mode.
         """
+        self.mode: str = mode
         title: str = 'slpkg install packages'
         if mode == 'upgrade':
             title: str = 'slpkg upgrade packages'
         self.ascii.draw_package_title('The following packages will be installed or upgraded:', title)
 
         for package in packages:
             self.draw_install_upgrade_package(package)
-            self.summary(package, mode)
+            self.summary(package)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
             for dependency in dependencies:
                 self.draw_install_upgrade_package(dependency)
-                self.summary(dependency, mode)
+                self.summary(dependency)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_install_and_upgrade(self.sum_install, self.sum_upgrade,
                                                  self.sum_size_comp, self.sum_size_uncomp)
         print(self.summary_message)
 
     def download_packages(self, packages: list, directory: Path) -> None:
-        """ View packages for download method.
+        """View packages for download method.
 
         Args:
             packages (list): Packages name for download.
             directory (Path): Path to download.
         """
-        mode: str = 'download'
+        self.mode: str = 'download'
         self.download_only: Path = directory
         self.ascii.draw_package_title('The following packages will be downloaded:',
                                       'slpkg download packages')
 
         for package in packages:
             self.draw_download_package(package)
-            self.summary(package, mode)
+            self.summary(package)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_download(packages, self.sum_size_comp)
         print(self.summary_message)
 
     def remove_packages(self, packages: list, dependencies: list) -> None:
-        """ View packages for remove.
+        """View packages for remove.
 
         Args:
             packages (list): List of packages.
             dependencies (list): List of dependencies.
         """
-        mode: str = 'remove'
+        self.mode: str = 'remove'
         self.ascii.draw_package_title('The following packages will be removed:',
                                       'slpkg remove packages')
         for package in packages:
             self.draw_remove_package(package)
-            self.summary(package, mode)
+            self.summary(package)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
             for dependency in dependencies:
                 self.draw_remove_package(dependency)
-                self.summary(dependency, mode)
+                self.summary(dependency)
 
         self.ascii.draw_bottom_line()
         self.set_summary_for_remove(self.sum_remove, self.sum_size_remove)
         print(self.summary_message)
 
     def draw_build_package(self, package: str) -> None:
-        """ Draw line for build package method.
+        """Draw line for build package method.
 
         Args:
             package (str): Package name.
         """
         size: str = ''
         color: str = self.yellow
         version: str = self.data[package]['version']
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
     def draw_install_upgrade_package(self, package: str) -> None:
-        """ Draw line for install or upgrade package method.
+        """Draw line for install or upgrade package method.
 
         Args:
             package (str): Package name.
         """
         size: str = ''
         color: str = self.cyan
         version: str = self.data[package]['version']
@@ -190,15 +190,15 @@
         if installed and self.option_for_reinstall and not upgradable:
             color: str = self.violet
             package: str = self.build_package_and_version(package)
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
     def draw_download_package(self, package: str) -> None:
-        """ Draw package for download method.
+        """Draw package for download method.
 
         Args:
             package (str): Package name.
         """
         size: str = ''
         color: str = self.cyan
         version: str = self.data[package]['version']
@@ -206,138 +206,145 @@
         if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
             size_comp: float = float(self.data[package]['size_comp']) * 1024
             size: str = self.utils.convert_file_sizes(size_comp)
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
     def draw_remove_package(self, package: str) -> None:
-        """ Draw package for remove method.
+        """Draw package for remove method.
 
         Args:
             package (str): Package name.
         """
         count_size: int = self.utils.count_file_size(package)
         installed: str = self.utils.is_package_installed(package)
         version: str = self.utils.split_package(installed)['version']
         repo_tag: str = self.utils.split_package(installed)['tag']
         size: str = self.utils.convert_file_sizes(count_size)
         repository: str = repo_tag.lower().replace('_', '')
 
         self.ascii.draw_package_line(package, version, size, self.red, repository)
 
-    def summary(self, package: str, method: str) -> None:
-        """ Counts packages per method.
+    def summary(self, package: str) -> None:
+        """Count packages per method.
 
         Args:
             package (str): Package name.
             method (str): Type of method.
         """
         installed: str = self.utils.is_package_installed(package)
 
         if self.repository not in list(self.repos.repositories)[:2] and self.repository is not None:
             self.sum_size_comp += float(self.data[package]['size_comp']) * 1024
             self.sum_size_uncomp += float(self.data[package]['size_uncomp']) * 1024
 
-        if installed and method == 'remove':
+        if installed and self.mode == 'remove':
             self.sum_size_remove += self.utils.count_file_size(package)
 
         upgradeable: bool = False
-        if method != 'remove':
+        if self.mode != 'remove':
             upgradeable: bool = self.upgrade.is_package_upgradeable(installed)
 
         if not installed:
             self.sum_install += 1
         elif installed and self.option_for_reinstall:
             self.sum_upgrade += 1
         elif upgradeable:
             self.sum_upgrade += 1
-        elif installed and method == 'remove':
+        elif installed and self.mode == 'remove':
             self.sum_remove += 1
 
     def set_summary_for_build(self, packages: list) -> None:
-        """ Sets summary message for build.
+        """Set summary message for build.
 
         Args:
             packages (list): List of packages.
         """
         self.summary_message: str = (
             f'{self.grey}Total {len(packages)} packages '
             f'will be build in {self.tmp_path} folder.{self.endc}')
 
     def set_summary_for_install_and_upgrade(self, install: int, upgrade: int, size_comp: int, size_uncomp: int) -> None:
-        """ Sets summary for install or upgrade.
+        """Set summary for install or upgrade.
 
         Args:
             install (int): Counts for installs.
             upgrade (int): Counts for upgrades.
             size_comp (int): Counts of compressed sizes.
             size_uncomp (int): Counts of uncompressed sizes.
         """
+        custom_message: str = ''
+        upgrade_message: str = ''
         split_message: str = '\n'
         if self.columns > 80:
             split_message: str = ''
         total_packages: str = (f'{self.grey}Total {install} packages will be installed and {upgrade} '
                                f'will be upgraded, while a total ')
         total_sizes: str = (f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
                             f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc}')
-        self.summary_message: str = f'{total_packages}{split_message}{total_sizes}'
+        if self.mode == 'upgrade':
+            custom_message: str = (f'\n{self.grey}Note: Packages with custom versions may not '
+                                   f'compare correctly.{self.endc}')
+            if self.upgrade_log_file.is_file():
+                upgrade_message: str = (f'\n{self.red}{self.ascii.failed} Some versions failed, '
+                                        f'check the /var/log/slpkg/upgrade.log file.{self.endc}')
+        self.summary_message: str = f'{total_packages}{split_message}{total_sizes}{custom_message}{upgrade_message}'
 
     def set_summary_for_remove(self, remove: int, size_rmv: int) -> None:
-        """ Sets summary for removes.
+        """Set summary for removes.
 
         Args:
             remove (int): Counts of removes.
             size_rmv (int): Size of removes.
         """
         self.summary_message: str = (
             f'{self.grey}Total {remove} packages '
             f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
             f'of space will be freed up.{self.endc}')
 
     def set_summary_for_download(self, packages: list, size_comp: int) -> None:
-        """ Sets summary for downloads.
+        """Set summary for downloads.
 
         Args:
             packages (list): List of packages.
             size_comp (int): Size of downloads.
         """
         self.summary_message: str = (
             f'{self.grey}Total {len(packages)} packages and {self.utils.convert_file_sizes(size_comp)} '
             f'will be downloaded in {self.download_only} folder.{self.endc}')
 
     def build_package_and_version(self, package: str) -> str:
-        """ Builds package and version.
+        """Build package and version.
 
         Args:
             package (str): Package name.
 
         Returns:
             str: Package with the version.
         """
         installed_package: str = self.utils.is_package_installed(package)
         version: str = self.utils.split_package(installed_package)['version']
         return f'{package}-{version}'
 
     def skipping_packages(self, packages: list) -> None:
-        """ View skipped packages.
+        """View skipped packages.
 
         Args:
             packages (list): List of packages.
         """
         if packages:
             print('Packages skipped by the user:\n')
             for name in packages:
                 failed: str = f'{self.red}{self.ascii.skipped}{self.endc}'
                 print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} "
                       f"{self.data[name]['package']} {failed}{' ' * 17}")
             print()
 
     def missing_dependencies(self, packages: list) -> None:
-        """ View for missing dependencies.
-        """
+        """View for missing dependencies."""
         if self.view_missing_deps:
             missing_deps: dict = {}
             for package in packages:
                 requires: list = self.data[package]['requires']
                 for req in requires:
                     if req not in self.data:
                         missing_deps[package] = [req for req in requires if req not in self.data]
@@ -345,15 +352,15 @@
                 print('\nPackages with missing dependencies:')
                 for pkg, deps in missing_deps.items():
                     if deps and deps != ['']:
                         print(f"> {self.cyan}{pkg}{self.endc}: Requires "
                               f"({len(deps)}) -> {self.red}{', '.join(deps)}{self.endc}")
 
     def question(self, message: str = 'Do you want to continue?') -> None:
-        """ View a question.
+        """View a question.
 
         Args:
             message (str, optional): Message of question.
 
         Raises:
             SystemExit: Raise a exit code 0.
         """
```

### Comparing `slpkg-5.0.8/PKG-INFO` & `slpkg-5.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 5.0.8
+Version: 5.0.9
 Summary: Package manager utility for Slackware Linux
 Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Maintainer-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slpkg Version: 5.0.8 Summary: Package manager
+Metadata-Version: 2.1 Name: slpkg Version: 5.0.9 Summary: Package manager
 utility for Slackware Linux Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis
 gmail.com> Maintainer-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Environment :: Console
 Classifier: Operating System :: POSIX Classifier: Operating System :: POSIX ::
```

