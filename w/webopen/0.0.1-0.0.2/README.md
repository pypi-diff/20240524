# Comparing `tmp/webopen-0.0.1.tar.gz` & `tmp/webopen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webopen-0.0.1.tar", last modified: Thu May 23 20:55:35 2024, max compression
+gzip compressed data, was "webopen-0.0.2.tar", last modified: Fri May 24 07:44:43 2024, max compression
```

## Comparing `webopen-0.0.1.tar` & `webopen-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 20:55:35.247506 webopen-0.0.1/
--rw-rw-rw-   0        0        0     1096 2024-05-21 18:16:50.000000 webopen-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1650 2024-05-23 20:55:35.245289 webopen-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      977 2024-05-23 20:31:11.000000 webopen-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 20:55:35.248619 webopen-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1080 2024-05-23 20:46:32.000000 webopen-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:55:35.143133 webopen-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 20:55:35.154576 webopen-0.0.1/src/webopen/
--rw-rw-rw-   0        0        0       19 2024-05-21 17:26:47.000000 webopen-0.0.1/src/webopen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:55:35.241609 webopen-0.0.1/src/webopen/db/
--rw-rw-rw-   0        0        0      188 2024-05-23 20:31:11.000000 webopen-0.0.1/src/webopen/db/__init__.py
--rw-rw-rw-   0        0        0       46 2024-05-23 20:31:11.000000 webopen-0.0.1/src/webopen/db/config.py
--rw-rw-rw-   0        0        0      241 2024-05-23 20:31:11.000000 webopen-0.0.1/src/webopen/db/connection.py
--rw-rw-rw-   0        0        0      452 2024-05-23 20:31:11.000000 webopen-0.0.1/src/webopen/db/models.py
--rw-rw-rw-   0        0        0     2148 2024-05-23 20:31:11.000000 webopen-0.0.1/src/webopen/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:55:35.243777 webopen-0.0.1/src/webopen.egg-info/
--rw-rw-rw-   0        0        0     1650 2024-05-23 20:55:35.000000 webopen-0.0.1/src/webopen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-05-23 20:55:35.000000 webopen-0.0.1/src/webopen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 20:55:35.000000 webopen-0.0.1/src/webopen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-23 20:55:35.000000 webopen-0.0.1/src/webopen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 20:55:35.000000 webopen-0.0.1/src/webopen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 20:55:35.000000 webopen-0.0.1/src/webopen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 07:44:43.808744 webopen-0.0.2/
+-rw-rw-rw-   0        0        0     1096 2024-05-21 18:16:50.000000 webopen-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1657 2024-05-24 07:44:43.805701 webopen-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2024-05-23 20:31:11.000000 webopen-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:44:43.808744 webopen-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2024-05-24 07:44:29.000000 webopen-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:44:43.691811 webopen-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 07:44:43.716138 webopen-0.0.2/src/webopen/
+-rw-rw-rw-   0        0        0       19 2024-05-21 17:26:47.000000 webopen-0.0.2/src/webopen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:44:43.796681 webopen-0.0.2/src/webopen/db/
+-rw-rw-rw-   0        0        0      188 2024-05-23 20:31:11.000000 webopen-0.0.2/src/webopen/db/__init__.py
+-rw-rw-rw-   0        0        0       46 2024-05-23 20:31:11.000000 webopen-0.0.2/src/webopen/db/config.py
+-rw-rw-rw-   0        0        0      241 2024-05-23 20:31:11.000000 webopen-0.0.2/src/webopen/db/connection.py
+-rw-rw-rw-   0        0        0      452 2024-05-23 20:31:11.000000 webopen-0.0.2/src/webopen/db/models.py
+-rw-rw-rw-   0        0        0     2986 2024-05-24 07:42:55.000000 webopen-0.0.2/src/webopen/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:44:43.802165 webopen-0.0.2/src/webopen.egg-info/
+-rw-rw-rw-   0        0        0     1657 2024-05-24 07:44:43.000000 webopen-0.0.2/src/webopen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2024-05-24 07:44:43.000000 webopen-0.0.2/src/webopen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:44:43.000000 webopen-0.0.2/src/webopen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-24 07:44:43.000000 webopen-0.0.2/src/webopen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-05-24 07:44:43.000000 webopen-0.0.2/src/webopen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 07:44:43.000000 webopen-0.0.2/src/webopen.egg-info/top_level.txt
```

### Comparing `webopen-0.0.1/LICENSE.txt` & `webopen-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webopen-0.0.1/PKG-INFO` & `webopen-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: webopen
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/BhuvaneshwarMarri/webopen
 Author: Bhuvaneshwar_Marri
 Author-email: bhuvaneshwarmarri@gmail.com
 Project-URL: Homepage, https://github.com/BhuvaneshwarMarri/webopen
 Project-URL: Issues, https://github.com/BhuvaneshwarMarri/webopen/issues
-Keywords: add,search
+Keywords: add,search,delete
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: argparse
```

### Comparing `webopen-0.0.1/README.md` & `webopen-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `webopen-0.0.1/setup.py` & `webopen-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webopen',
-    version='0.0.1',
+    version='0.0.2',
     author='Bhuvaneshwar_Marri',
     author_email='bhuvaneshwarmarri@gmail.com',
     description='A small example package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BhuvaneshwarMarri/webopen',
     project_urls={
@@ -17,15 +17,15 @@
     package_dir={'': 'src'},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    keywords=["add", "search"],
+    keywords=["add", "search","delete"],
     python_requires=">=3.8",
     install_requires=[
         "argparse",
         "click",
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `webopen-0.0.1/src/webopen/main.py` & `webopen-0.0.2/src/webopen/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,39 +28,65 @@
         WHERE website=?
         ''', (website,))
         data = cursor.fetchone()
         if data:
             labels = ["Website", "Username", "Password"]
             for i in range(3):
                 click.echo(f"{labels[i]} : {data[i]}")
+            return True
         else:
             click.echo("No data found for the specified website.")
+            return False
 
 def credential_search():
     website = click.prompt("Enter website name to search")
     search_data(website)
 
+def delete_data(website):
+    create_tables()
+    with get_db() as conn:
+        cursor = conn.cursor()
+        cursor.execute('''
+        DELETE FROM creds
+        WHERE website=?
+        ''', (website,))
+        conn.commit()
+        click.echo("Data deleted successfully")
+
+def credential_delete():
+    website = click.prompt("Enter website name to delete")
+    x=search_data(website)
+    if x:
+        choice = click.prompt("Enter yes to delete this credential else type no")
+        if choice == "yes":
+            delete_data(website)
+        else:
+            click.echo("Successfully exited from delete process")
+    
 def open_link(website):
     webbrowser.open(f"http://{website}")
         
 def main():
     
     parser = argparse.ArgumentParser(description="Manage credentials and open links.")
     subparsers = parser.add_subparsers(dest="command", help="Commands")
     
     parser.add_argument("-link", dest="link_name", help="The name of the link to open")
     subparsers.add_parser("add", help="Add a new credential")
     subparsers.add_parser("search", help="Search for a credential")
+    subparsers.add_parser("delete",help="Delete a particular credential")
     args = parser.parse_args()
     
     if args.link_name:
         open_link(args.link_name)
     elif args.command == "add":
         credential_add()
     elif args.command == "search":
         credential_search()
+    elif args.command == "delete":
+        credential_delete()
     else:
         parser.print_help()
 
 if __name__ == "__main__":
     create_tables()
     main()
```

### Comparing `webopen-0.0.1/src/webopen.egg-info/PKG-INFO` & `webopen-0.0.2/src/webopen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: webopen
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/BhuvaneshwarMarri/webopen
 Author: Bhuvaneshwar_Marri
 Author-email: bhuvaneshwarmarri@gmail.com
 Project-URL: Homepage, https://github.com/BhuvaneshwarMarri/webopen
 Project-URL: Issues, https://github.com/BhuvaneshwarMarri/webopen/issues
-Keywords: add,search
+Keywords: add,search,delete
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: argparse
```

