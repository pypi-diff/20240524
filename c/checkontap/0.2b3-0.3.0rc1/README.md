# Comparing `tmp/checkontap-0.2b3.tar.gz` & `tmp/checkontap-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkontap-0.2b3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "checkontap-0.3.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `checkontap-0.2b3.tar` & `checkontap-0.3.0rc1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.2b3/README.md
--rw-r--r--   0        0        0      931 2023-08-09 12:23:12.826155 checkontap-0.2b3/checkontap/__init__.py
--rw-r--r--   0        0        0     3818 2023-09-20 09:10:46.289460 checkontap-0.2b3/checkontap/cli.py
--rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.2b3/checkontap/ontapcmd/__init__.py
--rw-r--r--   0        0        0     2196 2023-08-09 13:14:56.124632 checkontap-0.2b3/checkontap/ontapcmd/about.py
--rw-r--r--   0        0        0     6378 2023-10-30 10:32:44.960200 checkontap-0.2b3/checkontap/ontapcmd/aggregateusage.py
--rw-r--r--   0        0        0     4610 2023-08-09 13:20:15.708654 checkontap-0.2b3/checkontap/ontapcmd/clusterhealth.py
--rw-r--r--   0        0        0     9441 2023-09-22 12:47:02.510254 checkontap-0.2b3/checkontap/ontapcmd/diskhealth.py
--rw-r--r--   0        0        0     8073 2023-09-19 06:20:16.166441 checkontap-0.2b3/checkontap/ontapcmd/hardwarehealth.py
--rw-r--r--   0        0        0     3834 2023-09-20 09:25:13.415579 checkontap-0.2b3/checkontap/ontapcmd/interfacehealth.py
--rw-r--r--   0        0        0     5059 2023-08-14 07:05:28.595099 checkontap-0.2b3/checkontap/ontapcmd/lunusage.py
--rw-r--r--   0        0        0     4297 2023-10-18 12:59:54.038751 checkontap-0.2b3/checkontap/ontapcmd/porthealth.py
--rw-r--r--   0        0        0     5522 2023-09-18 12:44:21.536553 checkontap-0.2b3/checkontap/ontapcmd/volumehealth.py
--rw-r--r--   0        0        0    10532 2023-09-18 12:42:24.354614 checkontap-0.2b3/checkontap/ontapcmd/volumeusage.py
--rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.2b3/checkontap/tools/__init__.py
--rw-r--r--   0        0        0    10314 2023-09-14 06:43:44.958496 checkontap-0.2b3/checkontap/tools/cli.py
--rw-r--r--   0        0        0     4217 2023-08-09 13:09:23.880171 checkontap-0.2b3/checkontap/tools/helper.py
--rw-r--r--   0        0        0      856 2023-10-30 10:35:45.686926 checkontap-0.2b3/pyproject.toml
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 checkontap-0.2b3/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.3.0rc1/README.md
+-rw-r--r--   0        0        0      936 2024-05-24 13:59:45.745899 checkontap-0.3.0rc1/checkontap/__init__.py
+-rw-r--r--   0        0        0     3820 2024-05-24 13:50:24.031583 checkontap-0.3.0rc1/checkontap/cli.py
+-rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.3.0rc1/checkontap/ontapcmd/__init__.py
+-rw-r--r--   0        0        0     2196 2023-08-09 13:14:56.124632 checkontap-0.3.0rc1/checkontap/ontapcmd/about.py
+-rw-r--r--   0        0        0     6378 2024-04-16 08:21:49.194100 checkontap-0.3.0rc1/checkontap/ontapcmd/aggregateusage.py
+-rw-r--r--   0        0        0     6936 2023-12-04 08:53:26.351468 checkontap-0.3.0rc1/checkontap/ontapcmd/clusterhealth.py
+-rw-r--r--   0        0        0     9228 2024-05-24 13:59:39.418483 checkontap-0.3.0rc1/checkontap/ontapcmd/diskhealth.py
+-rw-r--r--   0        0        0     8653 2024-03-13 15:06:57.126587 checkontap-0.3.0rc1/checkontap/ontapcmd/hardwarehealth.py
+-rw-r--r--   0        0        0     4764 2023-12-04 08:53:26.360822 checkontap-0.3.0rc1/checkontap/ontapcmd/interfacehealth.py
+-rw-r--r--   0        0        0     5059 2023-08-14 07:05:28.595099 checkontap-0.3.0rc1/checkontap/ontapcmd/lunusage.py
+-rw-r--r--   0        0        0     4297 2023-10-18 12:59:54.038751 checkontap-0.3.0rc1/checkontap/ontapcmd/porthealth.py
+-rw-r--r--   0        0        0     3748 2024-05-24 13:59:39.419486 checkontap-0.3.0rc1/checkontap/ontapcmd/snapmirrorhealth.py
+-rw-r--r--   0        0        0     5617 2024-05-24 13:59:45.746300 checkontap-0.3.0rc1/checkontap/ontapcmd/snapshothealth.py
+-rw-r--r--   0        0        0     5522 2023-09-18 12:44:21.536553 checkontap-0.3.0rc1/checkontap/ontapcmd/volumehealth.py
+-rw-r--r--   0        0        0    12382 2024-01-22 10:06:12.075231 checkontap-0.3.0rc1/checkontap/ontapcmd/volumeusage.py
+-rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.3.0rc1/checkontap/tools/__init__.py
+-rw-r--r--   0        0        0    10505 2024-05-24 13:59:45.757723 checkontap-0.3.0rc1/checkontap/tools/cli.py
+-rw-r--r--   0        0        0     4875 2024-05-24 13:59:45.758316 checkontap-0.3.0rc1/checkontap/tools/helper.py
+-rw-r--r--   0        0        0      874 2024-05-24 13:59:45.759323 checkontap-0.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 checkontap-0.3.0rc1/PKG-INFO
```

### Comparing `checkontap-0.2b3/checkontap/__init__.py` & `checkontap-0.3.0rc1/checkontap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = "0.1"
+__version__ = "0.3.0rc1"
 
 class CheckOntapException(Exception):
     pass
 
 class CheckOntapTimeout(BaseException):
     pass
```

### Comparing `checkontap-0.2b3/checkontap/cli.py` & `checkontap-0.3.0rc1/checkontap/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,16 @@
         else:
             sys.exit(e.code)
     except urllib3.exceptions.NewConnectionError as e:
         print(f"UNKNOWN - connection issue {e}")
         sys.exit(3)
     except CheckOntapTimeout as e:
         print("UNKNOWN - Timeout reached")
-        traceback.print_exc(file=sys.stdout)
+        #traceback.print_exc(file=sys.stdout)
         sys.exit(3)
     except Exception as e:
         print(f"UNKNOWN - Unhandled exception: {e}")
-        traceback.print_exc()
+        #traceback.print_exc()
         sys.exit(3)
 
 if __name__ == "__main__":
     main()
```

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/__init__.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/about.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/aggregateusage.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/aggregateusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/clusterhealth.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/interfacehealth.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,103 +13,109 @@
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from monplugin import Check,Status
-from netapp_ontap.resources import Cluster, Node, IpInterface
+from netapp_ontap.resources import IpInterface,Svm
 from netapp_ontap.error import NetAppRestError
 from ..tools import cli
-from ..tools.helper import setup_connection,severity,item_filter
+from ..tools.helper import setup_connection,item_filter,severity
+import re
 
-__cmd__ = "cluster-health"
+__cmd__ = "interface-health"
+description = f"check interface status and home location"
 
 """
 """
+
 def run():
     parser = cli.Parser()
-    parser.add_optional_arguments(cli.Argument.EXCLUDE,cli.Argument.INCLUDE)
-    parser.add_optional_arguments({
-        'name_or_flags': ['--mode'],
+    parser.set_description(description)
+    parser.add_optional_arguments(cli.Argument.EXCLUDE,
+                                  cli.Argument.INCLUDE)
+    parser.add_optional_arguments( {
+        'name_or_flags': ['--exclude-svm'],
         'options': {
             'action': 'store',
-            'choices': ['health', 'connect'],
-            'default': 'health',
-        'help': 'check health state or interconnect of a cluster',
+            'help': 'regexp to exclude interfaces from svm',
         }
     })
     args = parser.get_args()
+    
     # Setup module logging
     logger = logging.getLogger(__name__)
-    logger.disabled=True
+    logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
-    setup_connection(args.host, args.api_user, args.api_pass)
-
     check = Check()
 
-    # Get data
+    setup_connection(args.host, args.api_user, args.api_pass)
+
+    SvmInt = []
+    # check for running svm's
     try:
-        cluster = Cluster()
-        cluster.get(fields="name,metric,version")
-        logger.debug(f"Cluster info \n{cluster.__dict__}")
-        nodes_count = Node.count_collection()
-        logger.debug(f"found {nodes_count} nodes")
-        nodes = list(Node.get_collection(fields="name,state,membership,ha,cluster_interfaces"))
-        logger.debug(f"{nodes}")
-        if args.mode == "connect":
-            interfaces = []
-            for node in nodes:
-                # fetch cluster interfaces
-                for ipint in node.cluster_interfaces:
-                    Interface = IpInterface(uuid=ipint.uuid)
-                    Interface.get()
-                    interfaces.append(Interface)
+        svm = Svm.get_collection(fields="name,state,ip_interfaces")
+        for s in svm:
+            if hasattr(s, 'ip_interfaces') and 'stopped' in s.state:
+                for int in s.ip_interfaces:
+                    logger.info(f"found int {int.name} on stopped svm {s.name}")
+                    SvmInt.append(int.name)
     except NetAppRestError as error:
-        check.exit(Status.UNKNOWN, "Error => {}".format(error))
-    #
-    # Cluster health check
-    #
-    if args.mode == "health":
-        # Cluster global health
-        if 'ok' not in cluster.metric.status.lower():
-            check.add_message(Status.CRITICAL,"Cluster global status is {}".format(cluster.metric.status))
-        # Cluster node states
-        for node in nodes:
-            logger.debug(f"Node info \n{node.__dict__}")
-            m = "{} state {} as {}; giveback: {}; takeover: {}".format(node.name,node.state,node.membership,node.ha.giveback.state,node.ha.takeover.state)
-            if 'up' in node.state:
-                check.add_message(Status.OK, m)
-            elif 'down' in node.state:
-                check.add_message(Status.CRITICAL, m)
-            else:
-                check.add_message(Status.WARNING, m)
-        short = f"Checked {len(nodes)} Nodes"
-
-    #
-    # Cluster connect check
-    #
-    count = 0
-    if args.mode == "connect":
-        for IpInt in interfaces:
-            logger.debug(f"Interface info {IpInt.name}\n{IpInt.__dict__}")
+        check.exit(Status.UNKNOWN, f"Error => {error}")
+    except Exception as error:
+        check.exit(Status.UNKNOWN, f"{error}")
+    
+    IpInts = []
+    try:
+        interface_count = IpInterface.count_collection()
+        logger.info(f"found {interface_count} interfaces")
+        if interface_count == 0:
+            check.exit(Status.UNKNOWN, "no interfaces found")
+
+        for IpInt in IpInterface.get_collection(fields="*"):
             if (args.exclude or args.include) and item_filter(args,IpInt.name):
-                logger.debug(f"ex-/include interface {IpInt.name}")
+                logger.info(f"exclude interface {IpInt.name} due to include / exclude")
                 continue
-            count += 1
-            if 'down' in IpInt.state:
-                check.add_message(Status.CRITICAL, f"Int {IpInt.name} is {IpInt.state}")
-            elif not IpInt.location.is_home:
-                check.add_message(Status.CRITICAL, f"Int {IpInt.name} is on {IpInt.location.node.name} but should be on {IpInt.location.home_node.name}")
-            else:
-                check.add_message(Status.OK, f"Int {IpInt.name} on {IpInt.location.node.name} port {IpInt.location.port.name} is {IpInt.state}")
-        short = f"Checked {count} Interfaces"
+            if args.exclude_svm and hasattr(IpInt, 'svm'):
+                if re.search(args.exclude_svm, IpInt.svm.name):
+                    logger.info(f"exclude interface {IpInt.name} due to SVM exclude. SVM {IpInt.svm.name}")
+                    continue
+            logger.debug(f"INTERFACE {IpInt.name}\n{IpInt}")
+            IpInts.append(IpInt)
+
+    except NetAppRestError as error:
+        check.exit(Status.UNKNOWN, f"Error => {error}")
+    except Exception as error:
+        check.exit(Status.UNKNOWN, f"{error}")
+
+    count = 0
 
-    (code, message) = check.check_messages(separator="\n")
-    check.exit(code=code,message=f"{short}\n{message}")
+    for Int in IpInts:
+        if not Int.enabled:
+            logger.info(f"Interface {Int.name} is not enabled, ignore")
+            continue
+        count += 1
+        if 'down' in Int.state and Int.name in SvmInt:
+            logger.info(f"Interface {Int.name} for stopped svm {Int.svm.name}")
+        elif 'down' in Int.state:
+            check.add_message(Status.CRITICAL, f"int {Int.name} is {Int.state}")
+        if not Int.location.is_home:
+            check.add_message(Status.CRITICAL, f"Int {Int.name} is on {Int.location.node.name} but should be on {Int.location.home_node.name}")
+
+    check.add_message(Status.OK, f"{count} of {len(IpInts)} Interfaces are up")
+    
+    for Int in IpInts:
+        if hasattr(Int, 'svm'):
+            check.add_message(Status.OK, f"Int {Int.name:40}{Int.state:5}{Int.ip.address:16}/{Int.ip.netmask:3} is homed {Int.location.is_home} and belongs to SVM {Int.svm.name}")
+        else:
+            check.add_message(Status.OK, f"Int {Int.name:40}{Int.state:5}{Int.ip.address:16}/{Int.ip.netmask:3} is homed {Int.location.is_home}")
+        
+    (code, message) = check.check_messages(separator='\n  ')
+    check.exit(code=code,message=message)
 
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/diskhealth.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/diskhealth.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import logging
 from monplugin import Check,Status
 from netapp_ontap.resources import Disk,Software
 from netapp_ontap.error import NetAppRestError
 from ..tools import cli
 from ..tools.helper import setup_connection,item_filter,severity,compareVersion
 import re
-from pprint import pprint as pp
 
 __cmd__ = "disk-health"
 """
 Disk({
     'rpm': 7200,
     'node': {
         'uuid': 'f3a35903-68ae-11e8-8898-4b3d2df62ccf',
@@ -168,19 +167,17 @@
         #Shared = Disk is partitioned or in a storage pool.
         #Spare = Disk is a spare disk.
         #Unassigned = Disk ownership has not been assigned.
         #Unknown = Container is currently unknown. This is the default setting.
         #Unsupported = Disk is not supported.
 
         if not hasattr(disk, 'bay'):
-            pp("ADD BAY")
             disk.bay = " - "
 
         if not hasattr(disk, 'state'):
-            pp(f"ADD STATE : {disk.container_type}")
             m = f"Disk {disk.name:7} on bay {disk.bay:3} is {disk.type:6} {disk.container_type}"
             if hasattr(disk, 'outage'):
                 if disk.outage.persistently_failed:
                     m = f"Disk {disk.name} on bay {disk.bay:3} is persistently failed {disk.outage.reason.message}"
                     check.add_message(Status.CRITICAL, m)
                 else:
                     check.add_message(Status.OK, m)
@@ -198,29 +195,26 @@
         cType[disk.container_type] += 1
 
         out[disk.name] = {}
         out[disk.name]['name'] = disk.name
         out[disk.name]['state'] = disk.state
         out[disk.name]['bay'] = disk.bay if hasattr(disk, 'bay') else " - "
         out[disk.name]['node'] = disk.home_node.name if hasattr(disk, 'home_node') else "unknown"
-        pp("#########")
-        pp(f"State: {disk.state} cType: {disk.container_type}")
         if disk.container_type in ["unassigned","unsupported","unknown"]:
             m = f"Disk {disk.name:7} on bay {disk.bay:3} is {disk.container_type}"
             check.add_message(Status.WARNING,m)
         elif disk.container_type != "remote":
             if disk.node.name != disk.home_node.name:
                 check.add_message(Status.WARNING, f"Disk {disk.name} is on node {disk.node.name} instead of {disk.home_node.name}")
             m = f"Disk {disk.name:7} on bay {disk.bay:3} of node {disk.home_node.name} is {disk.state}"
             if stateWarn:
                 check.add_message(Status.WARNING,m)
             elif stateCrit:
                 check.add_message(Status.CRITICAL,m)
 
-    pp(cType)
     for c in cType.keys():
         check.add_perfdata(label=c,value=int(cType[c]))
     check.add_perfdata(label=f"total",value=int(disk_count))
     check.add_message(Status.OK, f"found {disk_count} disks at all while { ' - '.join({ f'{v} {k}' for (k,v) in cType.items()}) } ")
     for d in sorted(out.keys()):
         check.add_message(Status.OK, f"Disk {out[d]['name']:7} on bay {out[d]['bay']:2} of node {out[d]['node']} is {out[d]['state']}")
```

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/hardwarehealth.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/hardwarehealth.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,22 @@
         'name_or_flags': ['--type'],
         'options': {
             'action': 'store',
             'nargs': '+',
             'help': 'List of available sensor types (separated by space):\nfan thermal voltage current battery-life discrete fru nvmem counter minutes percent agent unknown',
         }
     })
+    parser.add_optional_arguments({
+        'name_or_flags': ['-s', '--sensor-details'],
+        'options': {
+            'action': 'store_true',
+            'help': 'Rather than using global status information from the node, check each sensor individually'
+        }
+    })
+    
     args = parser.get_args()
     # Setup module logging
     logger = logging.getLogger(__name__)
     logger.disabled=True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
@@ -62,27 +70,29 @@
     [-type {fan|thermal|voltage|current|battery-life|discrete|fru|nvmem|counter|minutes|percent|agent|unknown}] - Sensor Type
     [-state {normal|warn-low|warn-high|crit-low|crit-high|disabled|uninitialized|init-failed|not-available|invalid|retry|bad|not-present|failed|ignored|fault|unknown}]
     """
     if not args.type:
         sType = ['fan','thermal','voltage','current','battery-life','discrete','fru','nvmem','counter','minutes','percent','agent']
     else:
         sType = args.type
+        
+    if args.perfdata:
+        args.sensor_details = True
 
     mapWarn = ['warn-low','warn-high','ok-with-suppressed']
     mapCrit = ['crit-low','crit-high','bad','failed','fault','degraded','unreachable']
     mapUnknown = ['unknown','not-present','ignored','uninitialized','init-failed','not-available','invalid']
     nvramOk = ['battery_ok','battery_partially_discharged','battery_fully_charged']
     nvramWarn = ['battery_near_end_of_life','battery_over_charged']
     nvramCrit = ['battery_full_discharged','battery_not_present','battery_at_end_of_life']
     nvramUnknown = ['battery_unknown']
 
     logger.info(f"checking sensors: {sType}")
     try:
         # Node info
-        nodes_count = Node.count_collection()
         nodes = Node.get_collection(fields="*")
         for node in nodes:
             logger.info(f"{node.name}")
             logger.debug(f"{node}")
             if 'thermal' in sType:
                 logger.info(f"Thermal {node.controller.over_temperature}")
                 msg = f"Temperature on {node.name} is {node.controller.over_temperature}"
@@ -125,43 +135,48 @@
                         check.add_message(Status.CRITICAL, msg)
                     elif fru.state in mapUnknown:
                         check.add_message(Status.UNKNOWN, msg)
                     else:
                         check.add_message(Status.OK, msg)
 
         # Sensor environment
-        response = CLI().execute("system node environment sensors show",fields="fru,state,name,type,value,units,discrete-state",type=f"{','.join(str(x) for x in sType)}")
-        if response.http_response.json()['num_records'] == 0:
-            check.exit(Status.UNKNOWN,f"no sensors found")
-        for sensor in response.http_response.json()['records']:
-            logger.debug(f"{sensor}")
-            if (args.exclude or args.include) and item_filter(args,sensor['name']):
-                continue
-
-            msg = f"{sensor['type']} {sensor['name']} on node {sensor['node']} is {sensor['state']}"
-
-            if args.perfdata:
-                if 'value' in sensor and 'units' in sensor:
-                    perfData = {'label': f"{sensor['node']}_{sensor['name']}",
-                                'value': f"{sensor['value']}",
-                                'uom': f"{sensor['units'].replace('mA*hr','mAh')}"}
-                    check.add_perfdata(**perfData)
-
-            if sensor['state'] in mapCrit:
-                check.add_message(Status.CRITICAL,msg)
-            elif sensor['state'] in mapWarn:
-                check.add_message(Status.WARNING,msg)
-            elif sensor['state'] in mapUnknown:
-                check.add_message(Status.UNKNOWN,msg)
-
+        if args.sensor_details:
+            response = CLI().execute("system node environment sensors show",fields="fru,state,name,type,value,units,discrete-state",type=f"{','.join(str(x) for x in sType)}")
+            sensorCount = response.http_response.json()['num_records']
+            if sensorCount == 0:
+                check.exit(Status.UNKNOWN,f"no sensors found")
+            for sensor in response.http_response.json()['records']:
+                logger.debug(f"{sensor}")
+                if (args.exclude or args.include) and item_filter(args,sensor['name']):
+                    continue
+    
+                msg = f"{sensor['type']} {sensor['name']} on node {sensor['node']} is {sensor['state']}"
+    
+                if args.perfdata:
+                    if 'value' in sensor and 'units' in sensor:
+                        perfData = {'label': f"{sensor['node']}_{sensor['name']}",
+                                    'value': f"{sensor['value']}",
+                                    'uom': f"{sensor['units'].replace('mA*hr','mAh')}"}
+                        check.add_perfdata(**perfData)
+    
+                if sensor['state'] in mapCrit:
+                    check.add_message(Status.CRITICAL,msg)
+                elif sensor['state'] in mapWarn:
+                    check.add_message(Status.WARNING,msg)
+                elif sensor['state'] in mapUnknown:
+                    check.add_message(Status.UNKNOWN,msg)
+    
         (code, message) = check.check_messages(separator="\n")
         if code != Status.OK:
             check.exit(code=code,message=message)
         else:
-            check.exit(code=code,message=f"all {response.http_response.json()['num_records']} checked sensors are fine\n{message}")
+            if args.sensor_details:
+                check.exit(code=code,message=f"all {sensorCount} checked sensors are fine\n{message}")
+            else:
+                check.exit(code=code,message=f"all checked sensors are fine\n{message}")
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, f"Error => {error}")
     except Exception as error:
         logger.exception(error)
 
 if __name__ == "__main__":
```

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/interfacehealth.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/porthealth.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,90 +13,103 @@
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from monplugin import Check,Status
-from netapp_ontap.resources import IpInterface
+from netapp_ontap.resources import Port
 from netapp_ontap.error import NetAppRestError
 from ..tools import cli
 from ..tools.helper import setup_connection,item_filter,severity
-import re
 
-__cmd__ = "interface-health"
-description = f"check interface status and home location"
+__cmd__ = "port-health"
+description = f"check port status"
 
 """
+Port({
+    'mtu': 1500,
+    'uuid': 'e5b8287b-b111-11ed-975c-d039ea958568',
+    '_links': {'self': {'href': '/api/network/ethernet/ports/e5b8287b-b111-11ed-975c-d039ea958568'}},
+    'reachability': 'not_repairable',
+    'state': 'down',
+    'mac_address': 'd0:39:ev:95:x5:5e',
+    'type': 'physical',
+    'node': {
+        'uuid': '12c08d1a-e131-11ec-9572-d039ea958568',
+        '_links': {'self': {'href': '/api/cluster/nodes/12c08d1a-e131-11ec-9572-d039ea958568'}},
+        'name': 'Cluster01-Node02'},
+    'enabled': False,
+    'name': 'e0e'})
 """
 
 def run():
     parser = cli.Parser()
     parser.set_description(description)
     parser.add_optional_arguments(cli.Argument.EXCLUDE,
                                   cli.Argument.INCLUDE)
-    parser.add_optional_arguments( {
-        'name_or_flags': ['--exclude-svm'],
-        'options': {
-            'action': 'store',
-            'help': 'regexp to exclude interfaces from svm',
-        }
-    })
     args = parser.get_args()
-    
+
     # Setup module logging
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
     check = Check()
 
     setup_connection(args.host, args.api_user, args.api_pass)
 
-    IpInts = []
     try:
-        interface_count = IpInterface.count_collection()
-        logger.info(f"found {interface_count} interfaces")
-        if interface_count == 0:
-            check.exit(Status.UNKNOWN, "no interfaces found")
-
-        for IpInt in IpInterface.get_collection(fields="*"):
-            if (args.exclude or args.include) and item_filter(args,IpInt.name):
-                logger.info(f"exclude interface {IpInt.name} due to include / exclude")
+        port_count = Port.count_collection()
+        
+        if port_count == 0:
+            check.exit(Status.UNKNOWN,"no ports found on device")
+            
+        disabled = 0
+        
+        Ports = Port.get_collection(fields="*")
+        
+        for p in Ports:
+            if not hasattr(p, "enabled") or not p.enabled:
+                logger.info(f"Port isn't enabled {p.name}")
+                disabled += 1
                 continue
-            if args.exclude_svm and hasattr(IpInt, 'svm'):
-                if re.search(args.exclude_svm, IpInt.svm.name):
-                    logger.info(f"exclude interface {IpInt.name} due to SVM exclude. SVM {IpInt.svm.name}")
-                    continue
-            logger.debug(f"INTERFACE {IpInt.name}\n{IpInt}")
-            IpInts.append(IpInt)
+
+            if (args.exclude or args.include) and item_filter(args,p.name):
+                logger.info(f"exclude port  {p.name}")
+                port_count -= 1
+                continue
+
+            logger.info(f"checking {p.node.name} - {p.name} - {p.type}")
+            logger.debug(f"{p}")
+            out = f"{p.type} {p.name} on node {p.node.name} is {p.state}"
+            # check for type lag
+            if 'lag' in p.type:
+                active = [a.name for a  in p.lag.active_ports]
+                activePorts = set(active)
+                logger.info(f"LAG port {p.name} has {activePorts} as active ports")
+                missing = [ m.name for m in p.lag.member_ports if m.name not in activePorts ]
+                if len(missing) > 0:
+                    check.add_message(Status.CRITICAL,f"{out}, port {missing} is missing on lag")
+                else:
+                    check.add_message(Status.OK,f"{out}, with members {active}")
+            # check for type vlan and physical
+            else:
+                if not 'up' in p.state:
+                    check.add_message(Status.CRITICAL, out)
+                else:
+                    check.add_message(Status.OK,out)
 
     except NetAppRestError as error:
-        check.exit(Status.UNKNOWN, f"Error => {error}")
+        check.exit(Status.UNKNOWN, "Error => {}".format(error))
     except Exception as error:
-        check.exit(Status.UNKNOWN, f"{error}")
+        logger.exception(error)
 
-    count = 0
-
-    for Int in IpInts:
-        if not Int.enabled:
-            logger.info(f"Interface {Int.name} is not enabled, ignore")
-            continue
-        count += 1
-        if 'down' in Int.state:
-            check.add_message(Status.CRITICAL, f"int {Int.name} is {Int.state}")
-        if not Int.location.is_home:
-            check.add_message(Status.CRITICAL, f"Int {Int.name} is on {Int.location.node.name} but should be on {Int.location.home_node.name}")
-
-    check.add_message(Status.OK, f"{count} of {len(IpInts)} Interfaces are up")
-    
-    for Int in IpInts:
-        check.add_message(Status.OK, f"Int {Int.name:40}{Int.state:5}{Int.ip.address:16}/{Int.ip.netmask:3} is homed {Int.location.is_home}")
-        
-    (code, message) = check.check_messages(separator='\n  ')
-    check.exit(code=code,message=message)
+    short = f"checked {port_count} Ports; ({port_count- disabled} enabled, {disabled} disabled)"
+    (code, message) = check.check_messages(separator='\n')
+    check.exit(code=code,message=f"{short}\n{message}")
 
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/lunusage.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/lunusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/porthealth.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/volumehealth.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,103 +13,115 @@
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from monplugin import Check,Status
-from netapp_ontap.resources import Port
+from netapp_ontap.resources import Volume
 from netapp_ontap.error import NetAppRestError
 from ..tools import cli
-from ..tools.helper import setup_connection,item_filter,severity
-
-__cmd__ = "port-health"
-description = f"check port status"
+from ..tools.helper import setup_connection,severity,item_filter
 
+__cmd__ = "volume-health"
+description = "Check state of volumes online,offline,error or mixed"
 """
-Port({
-    'mtu': 1500,
-    'uuid': 'e5b8287b-b111-11ed-975c-d039ea958568',
-    '_links': {'self': {'href': '/api/network/ethernet/ports/e5b8287b-b111-11ed-975c-d039ea958568'}},
-    'reachability': 'not_repairable',
-    'state': 'down',
-    'mac_address': 'd0:39:ev:95:x5:5e',
-    'type': 'physical',
-    'node': {
-        'uuid': '12c08d1a-e131-11ec-9572-d039ea958568',
-        '_links': {'self': {'href': '/api/cluster/nodes/12c08d1a-e131-11ec-9572-d039ea958568'}},
-        'name': 'Cluster01-Node02'},
-    'enabled': False,
-    'name': 'e0e'})
+Volume({
+    'snapshot_policy': {'name': 'none'},
+    'analytics': {'state': 'off'},
+    'space': {'size': 27487790694400, 'available': 13976673030144, 'used': 13511117664256},
+    'type': 'rw',
+    'size': 27487790694400,
+    'cloud_retrieval_policy': 'default',
+    'name': 'eald_p',
+    'svm': {
+        'name': 'acme01',
+        'uuid': '21a63386-5483-11ea-8c65-00a098ef551e',
+        '_links': {'self': {'href': '/api/svm/svms/21a63386-5483-11ea-8c65-00a098ef551e'}}},
+    'aggregates': [{'uuid': '01d71c4b-88d8-43c3-ae33-afa2b64a629d', 'name': 'acme01_data'}],
+    'snapmirror': {'is_protected': True},
+    'style': 'flexvol',
+    'uuid': '42b7ee25-a342-11eb-b488-00a098c53056',
+    '_links': {'self': {'href': '/api/storage/volumes/42b7ee25-a342-11eb-b488-00a098c53056'}},
+    'state': 'online',
+    'nas': {'export_policy': {'name': 'default'}},
+    'tiering': {'policy': 'none'},
+    'clone': {'is_flexclone': False},
+    'language': 'c.utf_8',
+    'metric': {
+        'status': 'ok',
+        'timestamp': '2022-08-03T11:22:00+00:00',
+        'latency': {'other': 214, 'write': 259, 'read': 173, 'total': 205},
+        'duration': 'PT15S',
+        'iops': {'other': 7, 'write': 2, 'read': 5, 'total': 15},
+        'throughput': {'other': 0, 'write': 6967, 'read': 25478, 'total': 32445}},
+    'comment': '',
+    'create_time': '2021-04-22T10:10:54+02:00'})
 """
-
 def run():
     parser = cli.Parser()
     parser.set_description(description)
-    parser.add_optional_arguments(cli.Argument.EXCLUDE,
-                                  cli.Argument.INCLUDE)
+    parser.set_epilog("")
+    parser.add_optional_arguments(cli.Argument.WARNING,
+                                  cli.Argument.CRITICAL,
+                                  cli.Argument.EXCLUDE,
+                                  cli.Argument.INCLUDE,
+                                  cli.Argument.NAME)
     args = parser.get_args()
-
     # Setup module logging
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
-    check = Check()
-
     setup_connection(args.host, args.api_user, args.api_pass)
 
+    check = Check()
+
     try:
-        port_count = Port.count_collection()
-        
-        if port_count == 0:
-            check.exit(Status.UNKNOWN,"no ports found on device")
-            
-        disabled = 0
-        
-        Ports = Port.get_collection(fields="*")
-        
-        for p in Ports:
-            if not hasattr(p, "enabled") or not p.enabled:
-                logger.info(f"Port isn't enabled {p.name}")
-                disabled += 1
-                continue
-
-            if (args.exclude or args.include) and item_filter(args,p.name):
-                logger.info(f"exclude port  {p.name}")
-                port_count -= 1
-                continue
-
-            logger.info(f"checking {p.node.name} - {p.name} - {p.type}")
-            logger.debug(f"{p}")
-            out = f"{p.type} {p.name} on node {p.node.name} is {p.state}"
-            # check for type lag
-            if 'lag' in p.type:
-                active = [a.name for a  in p.lag.active_ports]
-                activePorts = set(active)
-                logger.info(f"LAG port {p.name} has {activePorts} as active ports")
-                missing = [ m.name for m in p.lag.member_ports if m.name not in activePorts ]
-                if len(missing) > 0:
-                    check.add_message(Status.CRITICAL,f"{out}, port {missing} is missing on lag")
+        volumes_count = Volume.count_collection()
+        logger.info(f"found {volumes_count} volumes")
+        if volumes_count == 0:
+            check.exit(Status.UNKNOWN, "no vols found")
+
+        if args.name:
+            volumes_count = len(args.name[0])
+            for n in args.name[0]:
+                vol = Volume.find(name=n)
+                logger.info(f"find volume {n}")
+                logger.debug(f"{vol}")
+                if args.warning and vol.state in args.warning:
+                    check.add_message(Status.WARNING, f"Vol: {vol.name} has state {vol.state}")
+                elif args.critical and vol.state in args.critical:
+                    check.add_message(Status.CRITICAL, f"Vol: {vol.name} has state {vol.state}")
                 else:
-                    check.add_message(Status.OK,f"{out}, with members {active}")
-            # check for type vlan and physical
-            else:
-                if not 'up' in p.state:
-                    check.add_message(Status.CRITICAL, out)
+                    check.add_message(Status.OK, f"Vol: {vol.name} has state {vol.state}")
+        else:
+            for vol in Volume.get_collection(fields="name,state,style,comment"):
+                logger.info(f"get volume {vol.name}")
+                logger.debug(f"{vol}")
+                if not hasattr(vol,'state'):
+                    volumes_count -= 1
+                    continue
+                if (args.exclude or args.include) and item_filter(args,vol.name):
+                    volumes_count -= 1
+                    continue
+                logger.info(f"state: {vol.state}\tname: {vol.name}\tstyle: {vol.style}\tcomment: {vol.comment}")
+                if args.warning and vol.state in args.warning:
+                    check.add_message(Status.WARNING, f"Vol: {vol.name} has state {vol.state}")
+                elif args.critical and vol.state in args.critical:
+                    check.add_message(Status.CRITICAL, f"Vol: {vol.name} has state {vol.state}")
                 else:
-                    check.add_message(Status.OK,out)
+                    check.add_message(Status.OK, f"Vol: {vol.name} has state {vol.state}")
+        short = f"checked {volumes_count} volumes"
+        (code, message) = check.check_messages(separator='\n')
+        check.exit(code=code,message=f"{short}\n{message}")
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error))
     except Exception as error:
         logger.exception(error)
 
-    short = f"checked {port_count} Ports; ({port_count- disabled} enabled, {disabled} disabled)"
-    (code, message) = check.check_messages(separator='\n')
-    check.exit(code=code,message=f"{short}\n{message}")
-
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.2b3/checkontap/ontapcmd/volumeusage.py` & `checkontap-0.3.0rc1/checkontap/ontapcmd/volumeusage.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from monplugin import Check,Status,Threshold, Range
 from netapp_ontap.resources import Volume
 from netapp_ontap.error import NetAppRestError
 from ..tools import cli
-from ..tools.helper import setup_connection,item_filter,severity,bytes_to_uom,range_in_bytes
+from ..tools.helper import setup_connection,item_filter,severity,bytes_to_uom,range_in_bytes,uom_to_bytes
 
 __cmd__ = "volume-usage"
 description = f"Mode {__cmd__} with -m / --metric usage or size description like used_GB. Inodes thresholds are alway given in %"
 """
 space.used + space.available + snapshot.reserve_available = space.size
 Volume({
     'files': {'maximum': 31122, 'used': 102},
@@ -71,14 +71,15 @@
     parser.set_epilog("Name of SVM will be prepended automaticaly to the volume name")
     parser.add_required_arguments(cli.Argument.WARNING, cli.Argument.CRITICAL)
     parser.add_optional_arguments(cli.Argument.EXCLUDE,
                                   cli.Argument.INCLUDE,
                                   cli.Argument.NAME,
                                   cli.Argument.METRIC,
                                   cli.Argument.INODE_WARN, cli.Argument.INODE_CRIT,
+                                  cli.Argument.SNAP_WARN, cli.Argument.SNAP_CRIT,
                                   )
     args = parser.get_args()
 
     # Setup module logging
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
@@ -140,26 +141,37 @@
                 
             if hasattr(vol.space.snapshot, 'reserve_size') and vol.space.snapshot.reserve_size > 0:
                 v['snapshot'] = {
                     'max': vol.space.snapshot.reserve_size,
                     'used': vol.space.snapshot.used,
                     'usage': bytes_to_uom(vol.space.snapshot.used, '%' ,vol.space.snapshot.reserve_size)
                 }
-            elif vol.space.snapshot.used > 0:
+                logger.info(f"{v['name']} hast {vol.space.snapshot.reserve_size}B snapshot reserved")
+            elif hasattr(vol.space.snapshot, 'reserve_percent') and vol.space.snapshot.reserve_percent > 0:
+                reserved_size = uom_to_bytes(vol.space.snapshot.reserve_percent, '%', v['space']['max'])
                 v['snapshot'] = {
-                    'max': 0,
+                    'max': reserved_size,
+                    'used': vol.space.snapshot.used,
+                    'usage': bytes_to_uom(vol.space.snapshot.used, '%', reserved_size)
+                }
+                logger.info(f"{v['name']} hast {vol.space.snapshot.reserve_percent}% snapshot reserved")
+            elif hasattr(vol.space.snapshot, 'reserve_percent') and vol.space.snapshot.reserve_percent == 0:
+                v['snapshot'] = {
+                    'max': vol.space.size,
                     'used': vol.space.snapshot.used,
                     'usage': bytes_to_uom(vol.space.snapshot.used, '%', vol.space.size)
                 }
+                logger.info(f"{v['name']} hast 0% snapshot reserved")
             else:
                 v['snapshot'] = {
                     'max': 0,
                     'used': vol.space.snapshot.used,
                     'usage': 0
                 }
+                logger.info(f"{v['name']} could'nt find snapshot settings")
 
             # Space
             usage = Threshold(args.warning or None, args.critical or None)
 
             for metric in ['usage', 'used', 'free']:
                 opts = {}
                 typ, uom, *_ = (args.metric.split('_') + ['%' if 'usage' in args.metric else 'B'])
@@ -215,15 +227,30 @@
                 if s != Status.OK:
                     check.add_message(s, f"Inodes usage on {v['name']} is {v['inodes']['usage']}%")
                 check.add_perfdata(label=f"{v['name']} inodes usage", value=v['inodes']['usage'], uom="%", **opts)
             else:
                 check.add_perfdata(label=f"{v['name']} inodes usage", value=v['inodes']['usage'], uom="%")
 
             # Snapshot usage just as perfdata
-            check.add_perfdata(label=f"{v['name']} snapshot usage" ,value=v['snapshot']['usage'], uom='%')
+            if args.snapshot_warning or args.snapshot_critical:
+                snapshot = Threshold(args.snapshot_warning or None, args.snapshot_critical or None)
+                opts = {}
+                opts['threshold'] = {}
+                threshold = {}
+                s = snapshot.get_status(v['snapshot']['usage'])
+                if args.snapshot_warning:
+                    threshold['warning'] = args.snapshot_warning
+                if args.snapshot_critical:
+                    threshold['critical'] = args.snapshot_critical
+                opts['threshold'] = Threshold(**threshold)
+                if s != Status.OK:
+                    check.add_message(s,f"Snapshot usage on {v['name']} id {v['snapshot']['usage']}%")
+                check.add_perfdata(label=f"{v['name']} snapshot usage" ,value=v['snapshot']['usage'], uom='%', **opts)
+            else:
+                check.add_perfdata(label=f"{v['name']} snapshot usage" ,value=v['snapshot']['usage'], uom='%')
 
         (code, message) = check.check_messages(separator='\n  ',allok=f"all {volumes_count} volumes are ok")
         check.exit(code=code,message=f"{message}")
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error))
     except Exception as error:
```

### Comparing `checkontap-0.2b3/checkontap/tools/__init__.py` & `checkontap-0.3.0rc1/checkontap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.2b3/checkontap/tools/cli.py` & `checkontap-0.3.0rc1/checkontap/tools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,8 +265,16 @@
     }
     SNAP_CRIT = {
         'name_or_flags': ['--snapshot-critical'],
         'options': {
             'action': 'store',
             'help': 'Snapshot used space critical threshold in percent'
         }
+    }
+    COUNT = {
+        'name_or_flags': ['-C','--count'] ,
+        'options': {
+            'action': 'store',
+            'help': 'count of whatever',
+            'type': int
+        }
     }
```

### Comparing `checkontap-0.2b3/checkontap/tools/helper.py` & `checkontap-0.3.0rc1/checkontap/tools/helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -122,8 +122,33 @@
     for i in range(max(len(versions1),len(versions2))):
        v1 = versions1[i] if i < len(versions1) else 0
        v2 = versions2[i] if i < len(versions2) else 0
        if v1 < v2:
            return 1
        elif v1 > v2:
            return 0
-    return -1
+    return -1
+
+# Convert time into secons
+# 1d / 1 W / 1.5h
+def to_seconds(value) -> None:
+    if not value:
+        return None
+    t = re.search('([0-9.]+)\s*([smhdw]*)', value.lower())
+    time = float(t.group(1))
+    if not t.group(2) or "s" in t.group(2):
+        # assuming seconds
+        return time
+    elif "m" in t.group(2):
+        # assuming minutes
+        return time * 60
+    elif "h" in t.group(2):
+        # assuming hours
+        return time * 3600
+    elif "d" in t.group(2):
+        # assuming hours
+        return time * 3600 * 24
+    elif "w" in t.group(2):
+        # assuming hours
+        return time * 3600 * 24 * 7
+    else:
+        return None
```

### Comparing `checkontap-0.2b3/pyproject.toml` & `checkontap-0.3.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkontap"
 readme = "README.md"
 description = "check_ontap monitoring plugin"
-version = "0.2b3"
-requires-python = ">= 3.6"
+version = "0.3.0rc1"
+requires-python = ">= 3.8"
 authors = [
     { name = "Matthias Gallinger", email = "matthias.gallinger@consol.de" }
 ]
 dependencies = [
-    "netapp-ontap >= 9.11.1.0",
-    "monplugin >= 0.6",
+    "netapp-ontap >= 9.14.1.0",
+    "monplugin >= 0.6.2",
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
 ]
 
 [project.scripts]
 check_ontap = "checkontap.cli:main"
```

### Comparing `checkontap-0.2b3/PKG-INFO` & `checkontap-0.3.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: checkontap
-Version: 0.2b3
+Version: 0.3.0rc1
 Summary: check_ontap monitoring plugin
 Author-email: Matthias Gallinger <matthias.gallinger@consol.de>
-Requires-Python: >= 3.6
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Requires-Dist: netapp-ontap >= 9.11.1.0
-Requires-Dist: monplugin >= 0.6
+Requires-Dist: netapp-ontap >= 9.14.1.0
+Requires-Dist: monplugin >= 0.6.2
 Project-URL: homepage, https://github.com/consol/check_ontap
 Project-URL: issues, https://github.com/consol/check_ontap/issues
 Project-URL: repository, https://github.com/consol/check_ontap.git
 
 # check_ontap
 
 Plugin for Naemon / Nagios like monitoring systems.
```

