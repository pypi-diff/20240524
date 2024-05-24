# Comparing `tmp/hukudo-ingress-2.1.2.tar.gz` & `tmp/hukudo-ingress-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hukudo-ingress-2.1.2.tar", last modified: Mon Dec  4 08:01:41 2023, max compression
+gzip compressed data, was "hukudo-ingress-2.2.0.tar", last modified: Fri May 24 09:18:18 2024, max compression
```

## Comparing `hukudo-ingress-2.1.2.tar` & `hukudo-ingress-2.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-12-04 08:01:41.530681 hukudo-ingress-2.1.2/
--rw-rw-r--   0 felix     (1337) felix     (1337)      163 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/.bumpversion.cfg
--rw-r--r--   0 felix     (1337) felix     (1337)    53248 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/.coverage
--rw-rw-r--   0 felix     (1337) felix     (1337)      245 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/.editorconfig
--rw-rw-r--   0 felix     (1337) felix     (1337)       72 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/.gitignore
--rw-rw-r--   0 felix     (1337) felix     (1337)       15 2023-06-01 14:00:13.000000 hukudo-ingress-2.1.2/.python-version
--rw-rw-r--   0 felix     (1337) felix     (1337)      340 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/CHANGELOG.md
--rw-rw-r--   0 felix     (1337) felix     (1337)     1823 2023-12-04 07:29:57.000000 hukudo-ingress-2.1.2/Caddyfile
--rw-rw-r--   0 felix     (1337) felix     (1337)      427 2023-06-01 14:02:21.000000 hukudo-ingress-2.1.2/Dockerfile
--rw-rw-r--   0 felix     (1337) felix     (1337)     1073 2023-11-23 14:26:21.000000 hukudo-ingress-2.1.2/LICENSE
--rw-rw-r--   0 felix     (1337) felix     (1337)       62 2023-11-23 14:25:58.000000 hukudo-ingress-2.1.2/MANIFEST.in
--rw-rw-r--   0 felix     (1337) felix     (1337)      760 2023-11-23 14:55:17.000000 hukudo-ingress-2.1.2/Makefile
--rw-rw-r--   0 felix     (1337) felix     (1337)      803 2023-12-04 08:01:41.530681 hukudo-ingress-2.1.2/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      473 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/README.md
--rw-rw-r--   0 felix     (1337) felix     (1337)    15819 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/coverage.xml
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-12-04 08:01:41.530681 hukudo-ingress-2.1.2/hukudo_ingress.egg-info/
--rw-r--r--   0 felix     (1337) felix     (1337)      803 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/hukudo_ingress.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      660 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/hukudo_ingress.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        1 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/hukudo_ingress.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)       45 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/hukudo_ingress.egg-info/entry_points.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)      163 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/hukudo_ingress.egg-info/requires.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        8 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/hukudo_ingress.egg-info/top_level.txt
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-12-04 08:01:41.530681 hukudo-ingress-2.1.2/ingress/
--rw-rw-r--   0 felix     (1337) felix     (1337)       22 2023-12-04 08:01:41.000000 hukudo-ingress-2.1.2/ingress/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1258 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/ingress/caddy.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2168 2023-11-23 14:51:31.000000 hukudo-ingress-2.1.2/ingress/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2116 2023-06-01 13:53:02.000000 hukudo-ingress-2.1.2/ingress/config.py
--rw-rw-r--   0 felix     (1337) felix     (1337)       38 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/ingress/exceptions.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     3888 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/ingress/main.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1991 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/ingress/models.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      659 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/ingress/repo.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      511 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/ingress/utils.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1736 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/requirements.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)      707 2023-12-04 08:01:41.530681 hukudo-ingress-2.1.2/setup.cfg
--rw-rw-r--   0 felix     (1337) felix     (1337)      348 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/setup.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-12-04 08:01:41.530681 hukudo-ingress-2.1.2/tests/
--rw-rw-r--   0 felix     (1337) felix     (1337)      317 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/tests/test_caddy.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      319 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/tests/test_logging.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      594 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/tests/test_models.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      317 2023-06-01 13:48:21.000000 hukudo-ingress-2.1.2/tests/test_repo.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2024-05-24 09:18:18.830778 hukudo-ingress-2.2.0/
+-rw-rw-r--   0 felix     (1337) felix     (1337)      163 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/.bumpversion.cfg
+-rw-r--r--   0 felix     (1337) felix     (1337)    53248 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/.coverage
+-rw-rw-r--   0 felix     (1337) felix     (1337)      245 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/.editorconfig
+-rw-rw-r--   0 felix     (1337) felix     (1337)       72 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/.gitignore
+-rw-rw-r--   0 felix     (1337) felix     (1337)       15 2023-06-01 14:00:13.000000 hukudo-ingress-2.2.0/.python-version
+-rw-rw-r--   0 felix     (1337) felix     (1337)      340 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/CHANGELOG.md
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1829 2024-05-24 09:02:13.000000 hukudo-ingress-2.2.0/Caddyfile
+-rw-rw-r--   0 felix     (1337) felix     (1337)      427 2023-06-01 14:02:21.000000 hukudo-ingress-2.2.0/Dockerfile
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1073 2023-11-23 14:26:21.000000 hukudo-ingress-2.2.0/LICENSE
+-rw-rw-r--   0 felix     (1337) felix     (1337)       62 2023-11-23 14:25:58.000000 hukudo-ingress-2.2.0/MANIFEST.in
+-rw-rw-r--   0 felix     (1337) felix     (1337)      760 2023-11-23 14:55:17.000000 hukudo-ingress-2.2.0/Makefile
+-rw-rw-r--   0 felix     (1337) felix     (1337)      803 2024-05-24 09:18:18.830778 hukudo-ingress-2.2.0/PKG-INFO
+-rw-rw-r--   0 felix     (1337) felix     (1337)      473 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/README.md
+-rw-rw-r--   0 felix     (1337) felix     (1337)    15998 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/coverage.xml
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2024-05-24 09:18:18.830778 hukudo-ingress-2.2.0/hukudo_ingress.egg-info/
+-rw-r--r--   0 felix     (1337) felix     (1337)      803 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/hukudo_ingress.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1337) felix     (1337)      660 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/hukudo_ingress.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)        1 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/hukudo_ingress.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)       45 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/hukudo_ingress.egg-info/entry_points.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)      163 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/hukudo_ingress.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)        8 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/hukudo_ingress.egg-info/top_level.txt
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2024-05-24 09:18:18.830778 hukudo-ingress-2.2.0/ingress/
+-rw-rw-r--   0 felix     (1337) felix     (1337)       22 2024-05-24 09:18:18.000000 hukudo-ingress-2.2.0/ingress/__init__.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1258 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/ingress/caddy.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2168 2023-11-23 14:51:31.000000 hukudo-ingress-2.2.0/ingress/cli.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2116 2023-06-01 13:53:02.000000 hukudo-ingress-2.2.0/ingress/config.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)       38 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/ingress/exceptions.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     4126 2024-05-24 09:13:12.000000 hukudo-ingress-2.2.0/ingress/main.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1991 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/ingress/models.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      659 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/ingress/repo.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      511 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/ingress/utils.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1736 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/requirements.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)      707 2024-05-24 09:18:18.830778 hukudo-ingress-2.2.0/setup.cfg
+-rw-rw-r--   0 felix     (1337) felix     (1337)      348 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/setup.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2024-05-24 09:18:18.830778 hukudo-ingress-2.2.0/tests/
+-rw-rw-r--   0 felix     (1337) felix     (1337)      317 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/tests/test_caddy.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      319 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/tests/test_logging.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      594 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/tests/test_models.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      317 2023-06-01 13:48:21.000000 hukudo-ingress-2.2.0/tests/test_repo.py
```

### Comparing `hukudo-ingress-2.1.2/.coverage` & `hukudo-ingress-2.2.0/.coverage`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/Caddyfile` & `hukudo-ingress-2.2.0/Caddyfile`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {
-  debug
 	admin 0.0.0.0:2019
 	local_certs
 	ocsp_stapling off
 	auto_https disable_redirects
 }
 (_proxy) {
 	handle_errors {
@@ -40,50 +39,51 @@
 		import authelia {args.0}
 		tls internal
 		import _proxy {args.1}
 	}
 }
 # ----------------------------------------------------------------------------
 
-import proxy docs.imx.0-main.de 0859b12ecd38:80
+import proxy docs.imx.0-main.de 2699bcf22f3d:80
 
-import proxy flower.imx.0-main.de 1ea597e4fd00:443
+import proxy flower.imx.0-main.de 59d9b2db71f2:443
 
-import proxy node-exporter.imx.0-main.de f27f1e23932e:9100
+import proxy node-exporter.imx.0-main.de 3ae299bcd6a3:9100
 
-import proxy service.imx.0-main.de 148929d0f0e0:5000
+import proxy service.imx.0-main.de c7d2876676fe:80
 
-import proxy solr.imx.0-main.de 4f3b6f4f321c:8983
+import proxy sfdc.imx.0-main.de 2d9a3eab4faa:80
 
-import proxy app.imx.0-main.de 638b5eca8a07:80
+import proxy solr.imx.0-main.de da220ac9ca33:8983
 
-import proxy a.0-main.de 57014948484d:8080
-
-import authed b.0-main.de 8df0ca7f1170:7331
+import proxy app.imx.0-main.de 845e788ebfc4:80
 
 import proxy fog.0-main.de e046513e7a50:8000
 
-import proxy auth.0-main.de f11e888fde8a:9091
+import proxy grafana.local.0-main.de 865f1ff0e120:3000
+
+import proxy auth.0-main.de f5d81a7d3718:9091
 
 import proxy grafana.dev.0-main.de e941a9969c60:3000
 
-import proxy odoo.0-main.de eefbb5df54f8:8069
+import proxy odoo.0-main.de a9eda13651f6:8069
 
 import proxy grafana.puddl.x dabc85de2f7d:3000
 
 import proxy pgadmin.puddl.x cefef6f092b0:80
 
-import proxy grafana.apm.x f1faacec6dd0:3000
+import proxy grafana.apm.x a504055533a2:3000
+
 
 # ----------------------------------------------------------------------------
 # ----------------------------------------------------------------------------
 # default server
 :443 {
 	tls internal {
 		on_demand
 	}
 	respond 502 {
 		body "502 Bad Gateway
 "
 		close
 	}
-}
+}
```

### Comparing `hukudo-ingress-2.1.2/LICENSE` & `hukudo-ingress-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/Makefile` & `hukudo-ingress-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/PKG-INFO` & `hukudo-ingress-2.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hukudo-ingress
-Version: 2.1.2
+Version: 2.2.0
 Home-page: https://gitlab.com/hukudo/ingress
 Author: hukudo GmbH
 Author-email: hukudo-ingress@hukudo.de
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: include_package_data
@@ -13,15 +13,15 @@
 # Ingress
 Configure Caddy as an ingress for your Docker containers.
 
 See https://gitlab.com/hukudo/ingress for example usage.
 
 ## Usage
 ```
-pip install hukudo-ingress==2.1.2
+pip install hukudo-ingress==2.2.0
 ingress --help
 ```
 
 ## Development
 Initial
 ```
 make dev-setup
```

### Comparing `hukudo-ingress-2.1.2/coverage.xml` & `hukudo-ingress-2.2.0/coverage.xml`

 * *Files 1% similar despite different names*

#### Comparing `hukudo-ingress-2.1.2/coverage.xml` & `hukudo-ingress-2.2.0/coverage.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1701676901192" lines-valid="353" lines-covered="164" line-rate="0.4646" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
+<coverage version="7.2.7" timestamp="1716542298529" lines-valid="358" lines-covered="164" line-rate="0.4581" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/felix/ingress/controller</source>
   </sources>
   <packages>
     <package name="." line-rate="0" branch-rate="0" complexity="0">
@@ -16,15 +16,15 @@
             <line number="7" hits="0"/>
             <line number="8" hits="0"/>
             <line number="11" hits="0"/>
           </lines>
         </class>
       </classes>
     </package>
-    <package name="ingress" line-rate="0.3907" branch-rate="0" complexity="0">
+    <package name="ingress" line-rate="0.3844" branch-rate="0" complexity="0">
       <classes>
         <class name="__init__.py" filename="ingress/__init__.py" complexity="0" line-rate="1" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
           </lines>
         </class>
@@ -211,66 +211,71 @@
             <line number="32" hits="0"/>
             <line number="33" hits="0"/>
             <line number="34" hits="0"/>
             <line number="35" hits="0"/>
             <line number="36" hits="0"/>
             <line number="37" hits="0"/>
             <line number="38" hits="0"/>
-            <line number="46" hits="0"/>
-            <line number="47" hits="0"/>
-            <line number="48" hits="0"/>
-            <line number="49" hits="0"/>
-            <line number="50" hits="0"/>
+            <line number="39" hits="0"/>
+            <line number="40" hits="0"/>
+            <line number="41" hits="0"/>
+            <line number="42" hits="0"/>
+            <line number="43" hits="0"/>
             <line number="51" hits="0"/>
             <line number="52" hits="0"/>
             <line number="53" hits="0"/>
             <line number="54" hits="0"/>
             <line number="55" hits="0"/>
+            <line number="56" hits="0"/>
+            <line number="57" hits="0"/>
             <line number="58" hits="0"/>
             <line number="59" hits="0"/>
-            <line number="62" hits="0"/>
-            <line number="69" hits="0"/>
-            <line number="70" hits="0"/>
-            <line number="71" hits="0"/>
-            <line number="72" hits="0"/>
-            <line number="73" hits="0"/>
+            <line number="60" hits="0"/>
+            <line number="63" hits="0"/>
+            <line number="64" hits="0"/>
+            <line number="67" hits="0"/>
             <line number="74" hits="0"/>
             <line number="75" hits="0"/>
+            <line number="76" hits="0"/>
             <line number="77" hits="0"/>
             <line number="78" hits="0"/>
             <line number="79" hits="0"/>
+            <line number="80" hits="0"/>
             <line number="82" hits="0"/>
             <line number="83" hits="0"/>
             <line number="84" hits="0"/>
-            <line number="85" hits="0"/>
-            <line number="86" hits="0"/>
             <line number="87" hits="0"/>
+            <line number="88" hits="0"/>
             <line number="89" hits="0"/>
             <line number="90" hits="0"/>
             <line number="91" hits="0"/>
             <line number="92" hits="0"/>
             <line number="94" hits="0"/>
             <line number="95" hits="0"/>
             <line number="96" hits="0"/>
-            <line number="98" hits="0"/>
+            <line number="97" hits="0"/>
             <line number="99" hits="0"/>
-            <line number="102" hits="0"/>
-            <line number="114" hits="0"/>
-            <line number="115" hits="0"/>
-            <line number="116" hits="0"/>
-            <line number="117" hits="0"/>
-            <line number="118" hits="0"/>
+            <line number="100" hits="0"/>
+            <line number="101" hits="0"/>
+            <line number="103" hits="0"/>
+            <line number="104" hits="0"/>
+            <line number="107" hits="0"/>
             <line number="119" hits="0"/>
             <line number="120" hits="0"/>
             <line number="121" hits="0"/>
             <line number="122" hits="0"/>
             <line number="123" hits="0"/>
             <line number="124" hits="0"/>
             <line number="125" hits="0"/>
             <line number="126" hits="0"/>
+            <line number="127" hits="0"/>
+            <line number="128" hits="0"/>
+            <line number="129" hits="0"/>
+            <line number="130" hits="0"/>
+            <line number="131" hits="0"/>
           </lines>
         </class>
         <class name="models.py" filename="ingress/models.py" complexity="0" line-rate="0.8571" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
```

### Comparing `hukudo-ingress-2.1.2/hukudo_ingress.egg-info/PKG-INFO` & `hukudo-ingress-2.2.0/hukudo_ingress.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hukudo-ingress
-Version: 2.1.2
+Version: 2.2.0
 Home-page: https://gitlab.com/hukudo/ingress
 Author: hukudo GmbH
 Author-email: hukudo-ingress@hukudo.de
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: include_package_data
@@ -13,15 +13,15 @@
 # Ingress
 Configure Caddy as an ingress for your Docker containers.
 
 See https://gitlab.com/hukudo/ingress for example usage.
 
 ## Usage
 ```
-pip install hukudo-ingress==2.1.2
+pip install hukudo-ingress==2.2.0
 ingress --help
 ```
 
 ## Development
 Initial
 ```
 make dev-setup
```

### Comparing `hukudo-ingress-2.1.2/hukudo_ingress.egg-info/SOURCES.txt` & `hukudo-ingress-2.2.0/hukudo_ingress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/ingress/caddy.py` & `hukudo-ingress-2.2.0/ingress/caddy.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/ingress/cli.py` & `hukudo-ingress-2.2.0/ingress/cli.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/ingress/config.py` & `hukudo-ingress-2.2.0/ingress/config.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/ingress/main.py` & `hukudo-ingress-2.2.0/ingress/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,57 +25,62 @@
 
 class ContainerParseError(Exception):
     def __init__(self, msg, container: Container):
         self.msg = msg
         self.container = container
 
 
-def container2proxy(container: Container):
+def iter_container2proxies(container: Container):
     container_network_alias = container.short_id
+    port = c2port(container)
+    has_authelia = container.labels.get("ingress.authelia", "").lower() == "true"
     try:
-        host = container.labels['ingress.host']
+        ingress_host = container.labels["ingress.host"]
     except KeyError:
-        raise ContainerParseError('no ingress.host', container)
-    return Proxy(
-        host=host,
-        port=c2port(container),
-        target=container_network_alias,
-        authelia=container.labels.get('ingress.authelia', '').lower() == 'true',
-    )
+        raise ContainerParseError("no ingress.host", container)
+    extra_hosts = container.labels.get("ingress.extra_hosts", "").split()
+    _hosts = [ingress_host] + extra_hosts
+    for host in _hosts:
+        yield Proxy(
+            host=host,
+            port=port,
+            target=container_network_alias,
+            authelia=has_authelia,
+        )
 
 
 def iter_proxies():
     client = get_docker_client()
-    containers: [Container] = client.containers.list(filters={'label': 'ingress.host'})
+    containers: [Container] = client.containers.list(filters={"label": "ingress.host"})
     for container in sorted(containers, key=lambda c: c.name):
-        extra = {'name': container.name, 'id': container.id}
-        log.debug('found container', **extra)
+        extra = {"name": container.name, "id": container.id}
+        log.debug("found container", **extra)
         try:
-            yield container2proxy(container)
+            yield from iter_container2proxies(container)
         except ContainerParseError as e:
-            log.debug(msg='skip', reason=e.msg, **extra)
+            log.debug(msg="skip", reason=e.msg, **extra)
 
 
 def get_proxy_map() -> ProxyMap:
     return ProxyMap(list(iter_proxies()))
 
 
 def set_network_aliases(net: Network, caddy_container_name: str, pm: ProxyMap):
     """
     Caddy should be reachable as the proxies' names, so other containers on the ingress network can reach services at
     their FQDN.
     For example: opening "https://foo.0-main.de" in your browser should result in the same result as "curl'ing" from
     another container.
     """
     aliases = [u.host for u in pm]
-    log.debug({'aliases': aliases})
+    log.debug({"aliases": aliases})
     try:
         net.disconnect(caddy_container_name)
     except docker.errors.APIError as e:
-        if 'is not connected to network' in str(e):
+        if "is not connected to network" in str(e):
             pass
         else:
             raise
     net.connect(caddy_container_name, aliases=aliases)
     return aliases
 
 
@@ -84,15 +89,15 @@
     network = client.networks.get(get_network_name())
     caddy_hostname = get_caddy_hostname()
     caddy_container_name = get_caddy_container_name()
     set_network_aliases(network, caddy_container_name, pm)
 
     caddyfile = get_caddyfile()
     caddyfile.write_text(caddy.render(pm))
-    log.debug('wrote Caddyfile', path=caddyfile)
+    log.debug("wrote Caddyfile", path=caddyfile)
     caddy.reformat(caddyfile)
 
     @backoff.on_exception(backoff.expo, CaddyError, max_time=30)
     def load_with_timeout():
         post_caddyfile(caddyfile, caddy_hostname)
 
     load_with_timeout()
@@ -113,14 +118,14 @@
     """
     repo = InMemoryRepo()
     try:
         while True:
             new = get_proxy_map()
             old = repo.load()
             if new != old:
-                log.info('changes detected', extra={'diff': len(new) - len(old)})
+                log.info("changes detected", extra={"diff": len(new) - len(old)})
                 repo.save(new)
                 reconfigure(new)
             time.sleep(tick_s)
     except KeyboardInterrupt:
-        log.debug('caught SIGINT. exiting.')
+        log.debug("caught SIGINT. exiting.")
         raise SystemExit(0)
```

### Comparing `hukudo-ingress-2.1.2/ingress/models.py` & `hukudo-ingress-2.2.0/ingress/models.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/ingress/repo.py` & `hukudo-ingress-2.2.0/ingress/repo.py`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/requirements.txt` & `hukudo-ingress-2.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `hukudo-ingress-2.1.2/setup.cfg` & `hukudo-ingress-2.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hukudo-ingress
-version = 2.1.2
+version = 2.2.0
 url = https://gitlab.com/hukudo/ingress
 author = hukudo GmbH
 author_email = hukudo-ingress@hukudo.de
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
```

### Comparing `hukudo-ingress-2.1.2/tests/test_models.py` & `hukudo-ingress-2.2.0/tests/test_models.py`

 * *Files identical despite different names*

