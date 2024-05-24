# Comparing `tmp/gtodo_sprokkel78-1.0.1.tar.gz` & `tmp/gtodo_sprokkel78-1.0.3.tar.gz`

## Comparing `gtodo_sprokkel78-1.0.1.tar` & `gtodo_sprokkel78-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/.DS_Store
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/MANIFEST.in
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/CHANGELOG
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/LICENSE
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/__init__
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/gtodo.desktop
--rw-r--r--   0        0        0    16441 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/gtodo.py
--rwxr-xr-x   0        0        0    20671 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/gtodo.svg
--rwxr-xr-x   0        0        0      666 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/install.sh
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/uninstall.sh
--rw-r--r--   0        0        0    27730 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/screenshots/gTodo-1.png
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/LICENSE
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/MANIFEST.in
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/CHANGELOG
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/LICENSE
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/__init__
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/gtodo.desktop
+-rw-r--r--   0        0        0    13712 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/gtodo.png
+-rw-r--r--   0        0        0    19261 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/gtodo.py
+-rwxr-xr-x   0        0        0    20671 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/gtodo.svg
+-rwxr-xr-x   0        0        0      666 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/install.sh
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/uninstall.sh
+-rw-r--r--   0        0        0    27730 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/screenshots/gTodo-1.png
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 gtodo_sprokkel78-1.0.3/PKG-INFO
```

### Comparing `gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/LICENSE` & `gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/LICENSE`

 * *Files identical despite different names*

### Comparing `gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/README.md` & `gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/README.md`

 * *Files identical despite different names*

### Comparing `gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/gtodo.py` & `gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/gtodo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,119 @@
 import os.path
 import subprocess
 import gi
+import sys
 
 gi.require_version('Gtk', '4.0')
 gi.require_version('Adw', '1')
 from gi.repository import Gtk, Adw
 from time import sleep
 
-# VERSION = 1.0.1
-ver = "1.0.1"
-
+# VERSION = 1.0.4
+ver = "1.0.4"
 
+#=====================================================================================================
 # GLOBAL VARIABLES
+#=====================================================================================================
 global thread
 global thread_started
 thread_started = False
 
 global homedir
 global topic
 topic = "Main"
 remove = 0
+topic_edit = 0
+old_topic = ""
 
 entry_todo = Gtk.Entry()
 entry_priority = Gtk.Entry()
 listbox_todo = Gtk.ListBox()
 hbox_topic = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=6)
 label_title = Gtk.Label()
 listbox_topic = Gtk.ListBox()
 box0 = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL, spacing=6)
 box_00a = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=6)
+statusbar = Gtk.Statusbar()
+entry_topic_1 = Gtk.Entry()
 
+#=====================================================================================================
 # STARTUP CHECKS
-
+#=====================================================================================================
 if not os.path.exists(os.path.expanduser("~") + "/.gtodo"):
     command = "mkdir " + os.path.expanduser("~") + "/.gtodo"
     result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
     out = result.communicate()
 if not os.path.exists(os.path.expanduser("~") + "/.gtodo/Main.txt"):
     command = "touch " + os.path.expanduser("~") + "/.gtodo/Main.txt"
     result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
     out = result.communicate()
 
-# ACCOUNT FOR DARK MODE.
-def is_dark_mode_enabled():
-    command = 'osascript -e "tell app \\"System Events\\" to tell appearance preferences to get dark mode"'
-    result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    out, err = result.communicate()
-    out = out.strip()
-    if out == "true":
-        Gtk.Settings.get_default().set_property("gtk-application-prefer-dark-theme", True)
-    else:
-        Gtk.Settings.get_default().set_property("gtk-application-prefer-dark-theme", False)
-
-is_dark_mode_enabled()
 
+#=====================================================================================================
+# ACCOUNT FOR DARK MODE ON MACOSX.
+#=====================================================================================================
+#def is_dark_mode_enabled():
+#    command = 'osascript -e "tell app \\"System Events\\" to tell appearance preferences to get dark mode"'
+#    result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+#    out, err = result.communicate()
+#    out = out.strip()
+#    if out == "true":
+#        Gtk.Settings.get_default().set_property("gtk-application-prefer-dark-theme", True)
+#    else:
+#        Gtk.Settings.get_default().set_property("gtk-application-prefer-dark-theme", False)
+
+#is_dark_mode_enabled()
+
+
+#=====================================================================================================
+# USER INTERFACE FUNCTIONS
+#=====================================================================================================
 def button_done_clicked(obj, listbox, row, label):
     global homedir
     global topic
     #print(str(obj))
     entry = label.get_text()
     #print(entry)
     listbox.remove(row)
-    command = "cat " + homedir + "/.gtodo/" + topic + ".txt | grep -v \"" + entry + "\" > " + homedir + "/.gtodo/" + topic + ".txt.new"
-    result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    out = result.communicate()
+
+    todo_list = ""
+    with open(homedir + "/.gtodo/" + topic + ".txt") as f:
+        content = f.readlines()
+        for x in content:
+            line = x.strip()
+            line_split = line.split(";")
+            if line_split[0]:
+                if line_split[1] != entry:
+                    todo_list = todo_list + line + "\n"
+
+    output = homedir + "/.gtodo/" + topic + ".txt"
+    new_topic_file = open(output, "w")
+    new_topic_file.write(todo_list)
+    new_topic_file.close()
+
     sleep(0.5)
-    command = "cp " + homedir + "/.gtodo/" + topic + ".txt.new " + homedir + "/.gtodo/" + topic + ".txt; rm " + homedir + "/.gtodo/" + topic + ".txt.new"
-    result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    out = result.communicate()
 
     reload_lists()
-
+    statusbar.push(0, "Todo item removed > " + entry)
 
 def reload_lists():
     print("Reloading the todo lists.")
     listbox_todo.remove_all()
     sleep(0.5)
     hbox_todo = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL)
     listbox_todo.append(hbox_todo)
 
     label_todo_1 = Gtk.Button(label="Todo Items")
     # label_todo_1.set_xalign(0.0)
     label_todo_1.set_size_request(500, 25)
     hbox_todo.append(label_todo_1)
 
     label_todo_2 = Gtk.Button(label="Priority")
-    label_todo_2.set_size_request(89, -1)
+    label_todo_2.set_size_request(120, -1)
     # label_todo_2.set_xalign(0.0)
     hbox_todo.append(label_todo_2)
 
     label_todo_3 = Gtk.Button(label="Done")
     label_todo_3.set_size_request(106, -1)
     hbox_todo.append(label_todo_3)
 
@@ -180,14 +204,16 @@
     command = "cp " + homedir + "/.gtodo/" + topic + ".txt.new " + homedir + "/.gtodo/" + topic + ".txt; rm " + homedir + "/.gtodo/" + topic + ".txt.new"
     result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
     out = result.communicate()
     sleep(0.5)
 
     reload_lists()
 
+    statusbar.push(0, "Todo item priority changed > " + prio + " > "+ todo)
+
 
 def button_todo_clicked(obj):
     global topic
     todo = entry_todo.get_text()
     prio = entry_priority.get_text()
 
     if entry_todo.get_text() != "" and ";" not in entry_todo.get_text() and "\"" not in entry_todo.get_text():
@@ -230,33 +256,47 @@
         sleep(0.5)
         command = "cp " + homedir + "/.gtodo/" + topic + ".txt.new " + homedir + "/.gtodo/" + topic + ".txt; rm " + homedir + "/.gtodo/" + topic + ".txt.new"
         result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         out = result.communicate()
         sleep(0.5)
         reload_lists()
 
+        statusbar.push(0, "Todo item added > " + todo)
+
 
 def new_topic(obj, entry):
     global topic
+    global topic_edit
+    global old_topic
     topic = entry.get_text()
-    if topic != "" and ";" not in topic and "." not in topic:
+    if topic != "" and ";" not in topic and "." not in topic and topic_edit == 0:
         if not os.path.exists(os.path.expanduser("~") + "/.gtodo/" + topic + ".txt"):
             command = "touch " + os.path.expanduser("~") + "/.gtodo/" + topic + ".txt"
             result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
             out = result.communicate()
 
             row = Gtk.ListBoxRow()
             label_topic = Gtk.Label(label=topic)
             row.set_child(label_topic)
             listbox_topic.append(row)
+    if topic != "" and ";" not in topic and "." not in topic and topic_edit == 1 and topic != "Main":
+        command = "mv " + os.path.expanduser("~") + "/.gtodo/" + old_topic + ".txt " + os.path.expanduser(
+            "~") + "/.gtodo/" + topic + ".txt"
+        result = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        out = result.communicate()
+        topic_edit = 0
+        label_topic = Gtk.Label(label=topic)
+
+    entry.set_text("")
+    listbox_topic.remove_all()
+    load_topics()
+    topic_changed(0, 0, 0, 0, label_topic)
+    statusbar.push(0, "Created new topic.")
+
 
-        entry.set_text("")
-        listbox_topic.remove_all()
-        load_topics()
-        topic_changed(0, 0, 0, 0, label_topic)
 
 def load_topics():
     print("Loading topics.")
     global homedir
     global listbox_topic
     global hbox_topic
     global topic
@@ -308,14 +348,15 @@
         else:
             if remove == 1:
                 listbox_topic.select_row(listbox_topic.get_row_at_index(0))
                 remove = 0
 
         x = x + 1
 
+
 def button_topic_delete_clicked(obj):
     global topic
     global topic_title
     global remove
     remove = 1
     if topic != "Main":
         if os.path.exists(os.path.expanduser("~") + "/.gtodo/" + topic + ".txt"):
@@ -326,87 +367,103 @@
         topic = "Main"
         label = Gtk.Label(label=topic)
         row = Gtk.ListBoxRow()
         row.set_child(label)
         listbox_topic.append(row)
         topic_changed(0, 0, 0, 0, label)
         load_topics()
+        statusbar.push(0, "Topic removed.")
 
 
 def topic_changed(obj, obj1, obj2, obj3, label):
     print("Topic changed.")
     global topic
     global label_title
     topic = label.get_text()
     label_title.set_text(" -> " + topic)
     reload_lists()
+    statusbar.push(0, "Topic changed to: " + topic)
 
 
+def button_topic_edit_clicked(obj):
+    global topic
+    global old_topic
+    global topic_edit
+    print("edit topic: " + topic)
+    topic_edit = 1
+    old_topic = topic
+    entry_topic_1.set_text(topic)
 
 
+#=====================================================================================================
 # CREATE THE USER INTERFACE
+#=====================================================================================================
 class MainWindow(Gtk.ApplicationWindow):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # Things will go here
 
 class MyApp(Adw.Application):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.connect('activate', self.on_activate)
 
     def on_activate(self, app):
 
         win = MainWindow(application=app)
         win.set_title("gTodo " + ver)
-        win.set_default_size(800, 500)
+        win.set_default_size(960, 1100)
         win.set_resizable(False)
         global box0
         win.set_child(box0)
 
         seperator_5 = Gtk.Separator()
         box0.append(seperator_5)
 
         scrolled_window_1 = Gtk.ScrolledWindow()
-        scrolled_window_1.set_size_request(100, 400)
+        scrolled_window_1.set_size_request(200, 700)
 
         box0.append(scrolled_window_1)
 
         global box_00a
         scrolled_window_1.set_child(box_00a)
 
         label_spacer_3 = Gtk.Label()
         label_spacer_3.set_size_request(-1, 17)
         box_00a.append(label_spacer_3)
 
-        label_topic = Gtk.Button(label="TOPICS")
+        label_topic = Gtk.Button(label="TOPICS LIST")
         label_topic.set_size_request(100, -1)
         box_00a.append(label_topic)
 
         # Create listbox columns
 
-        entry_topic_1 = Gtk.Entry()
-        entry_topic_1.set_max_length(12)
+        global entry_topic_1
+        entry_topic_1.set_max_length(20)
         entry_topic_1.set_editable(True)
-        entry_topic_1.set_placeholder_text("Add Topic")
+        entry_topic_1.set_placeholder_text("Add New Topic")
         entry_topic_1.connect("activate", new_topic, entry_topic_1)
         box_00a.append(entry_topic_1)
 
         label_topic_empty = Gtk.Label()
         label_topic_empty.set_size_request(100, 15)
         box_00a.append(label_topic_empty)
 
         box_00a.append(listbox_topic)
 
         load_topics()
 
         label_topic_delete_empty = Gtk.Label()
         box_00a.append(label_topic_delete_empty)
 
-        button_topic_delete = Gtk.Button(label="Remove")
+        button_topic_edit = Gtk.Button(label="Change Topic")
+        button_topic_edit.connect("clicked", button_topic_edit_clicked)
+        box_00a.append(button_topic_edit)
+
+        button_topic_delete = Gtk.Button(label="Remove Topic")
         button_topic_delete.connect("clicked", button_topic_delete_clicked)
         box_00a.append(button_topic_delete)
 
         seperator_1 = Gtk.Separator()
         box0.append(seperator_1)
 
         box1 = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=6)
@@ -420,15 +477,15 @@
         label_spacer = Gtk.Label()
         box_11a.append(label_spacer)
 
         box_11b = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL, spacing=6)
         box_11a.append(box_11b)
 
         global entry_todo
-        entry_todo.set_placeholder_text("New Todo")
+        entry_todo.set_placeholder_text("New Todo Item")
         entry_todo.set_size_request(500, -1)
         entry_todo.set_max_length(80)
         box_11b.append(entry_todo)
 
         global entry_priority
         entry_priority.set_placeholder_text("Priority")
         entry_priority.set_size_request(1, -1)
@@ -439,38 +496,46 @@
         button_todo = Gtk.Button(label="Add")
         button_todo.set_size_request(110, -1)
         button_todo.connect("clicked", button_todo_clicked)
         box_11b.append(button_todo)
 
         box_title = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL, spacing=6)
         box_11a.append(box_title)
+        box_statusbar = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL, spacing=6)
+        box_11a.append(box_statusbar)
 
         label_title.set_text(" -> " + topic)
         label_title.set_size_request(100, 35)
         label_title.set_xalign(0.0)
         box_title.append(label_title)
 
         label_spacer_2 = Gtk.Label()
         box_11a.append(label_spacer_2)
 
         scrolled_window = Gtk.ScrolledWindow()
-        scrolled_window.set_size_request(700, 400)
+        scrolled_window.set_size_request(700, 850)
         global listbox_todo
         box_11a.append(scrolled_window)
         scrolled_window.set_child(listbox_todo)
 
         # Create listbox columns
 
         reload_lists()
 
         seperator_3 = Gtk.Separator()
         box0.append(seperator_3)
 
         listbox_topic.select_row(listbox_topic.get_row_at_index(0))
 
+        global statusbar
+        statusbar.set_size_request(500, 30)
+        box_statusbar.append(statusbar)
+        statusbar.push(0, "Ready for input.")
+
         win.present()
 
 
+#=====================================================================================================
 # START THE APP
-
+#=====================================================================================================
 app = MyApp(application_id="com.sprokkel78.gtodo")
 app.run(None)
```

### Comparing `gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/gtodo.svg` & `gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/gtodo.svg`

 * *Files identical despite different names*

### Comparing `gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/install.sh` & `gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/install.sh`

 * *Files identical despite different names*

### Comparing `gtodo_sprokkel78-1.0.1/src/gtodo_sprokkel78/screenshots/gTodo-1.png` & `gtodo_sprokkel78-1.0.3/src/gtodo_sprokkel78/screenshots/gTodo-1.png`

 * *Files identical despite different names*

### Comparing `gtodo_sprokkel78-1.0.1/LICENSE` & `gtodo_sprokkel78-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gtodo_sprokkel78-1.0.1/README.md` & `gtodo_sprokkel78-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gtodo_sprokkel78-1.0.1/pyproject.toml` & `gtodo_sprokkel78-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gtodo_sprokkel78"
-version = "1.0.1"
+version = "1.0.3"
 authors = [
   { name="Sprokkel78", email="sprokkel78.bart@gmail.com" },
 ]
 description = "A graphical user interface in PyGTK4 for performing TODO list items on Ubuntu and other Linux distro's."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `gtodo_sprokkel78-1.0.1/PKG-INFO` & `gtodo_sprokkel78-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gtodo_sprokkel78
-Version: 1.0.1
+Version: 1.0.3
 Summary: A graphical user interface in PyGTK4 for performing TODO list items on Ubuntu and other Linux distro's.
 Author-email: Sprokkel78 <sprokkel78.bart@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

