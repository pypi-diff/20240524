# Comparing `tmp/iipyper-0.1.3.tar.gz` & `tmp/iipyper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iipyper-0.1.3.tar", max compression
+gzip compressed data, was "iipyper-0.1.4.tar", max compression
```

## Comparing `iipyper-0.1.3.tar` & `iipyper-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.521024 iipyper-0.1.3/LICENSE
--rw-r--r--   0        0        0     2212 2024-05-17 00:13:01.654594 iipyper-0.1.3/README.md
--rw-r--r--   0        0        0      984 2024-05-17 00:14:36.756461 iipyper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4057 2024-05-17 00:13:01.655539 iipyper-0.1.3/src/iipyper/__init__.py
--rw-r--r--   0        0        0     1011 2024-05-17 00:13:01.655924 iipyper-0.1.3/src/iipyper/audio.py
--rw-r--r--   0        0        0     9580 2024-05-17 00:13:01.656183 iipyper-0.1.3/src/iipyper/midi.py
--rw-r--r--   0        0        0    32977 2024-05-17 00:13:01.656770 iipyper-0.1.3/src/iipyper/osc.py
--rw-r--r--   0        0        0      213 2023-11-28 17:22:02.524007 iipyper-0.1.3/src/iipyper/state.py
--rw-r--r--   0        0        0     1311 2024-05-17 00:13:01.657191 iipyper-0.1.3/src/iipyper/timing.py
--rw-r--r--   0        0        0     5108 2024-05-17 00:13:01.657648 iipyper-0.1.3/src/iipyper/tui.py
--rw-r--r--   0        0        0     1795 2024-05-17 00:13:01.658088 iipyper-0.1.3/src/iipyper/types.py
--rw-r--r--   0        0        0      937 2024-05-17 00:13:01.658421 iipyper-0.1.3/src/iipyper/util.py
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 iipyper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.521024 iipyper-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2212 2024-05-17 00:13:01.654594 iipyper-0.1.4/README.md
+-rw-r--r--   0        0        0     1002 2024-05-24 01:05:13.995739 iipyper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4057 2024-05-17 00:13:01.655539 iipyper-0.1.4/src/iipyper/__init__.py
+-rw-r--r--   0        0        0     1011 2024-05-17 00:13:01.655924 iipyper-0.1.4/src/iipyper/audio.py
+-rw-r--r--   0        0        0     9604 2024-05-24 01:04:41.692438 iipyper-0.1.4/src/iipyper/midi.py
+-rw-r--r--   0        0        0    33030 2024-05-24 01:04:41.692864 iipyper-0.1.4/src/iipyper/osc.py
+-rw-r--r--   0        0        0      213 2023-11-28 17:22:02.524007 iipyper-0.1.4/src/iipyper/state.py
+-rw-r--r--   0        0        0     1311 2024-05-17 00:13:01.657191 iipyper-0.1.4/src/iipyper/timing.py
+-rw-r--r--   0        0        0     5339 2024-05-24 01:04:41.693238 iipyper-0.1.4/src/iipyper/tui.py
+-rw-r--r--   0        0        0     1795 2024-05-17 00:13:01.658088 iipyper-0.1.4/src/iipyper/types.py
+-rw-r--r--   0        0        0      937 2024-05-17 00:13:01.658421 iipyper-0.1.4/src/iipyper/util.py
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 iipyper-0.1.4/PKG-INFO
```

### Comparing `iipyper-0.1.3/LICENSE` & `iipyper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.3/README.md` & `iipyper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.3/src/iipyper/__init__.py` & `iipyper-0.1.4/src/iipyper/__init__.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.3/src/iipyper/audio.py` & `iipyper-0.1.4/src/iipyper/audio.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.3/src/iipyper/midi.py` & `iipyper-0.1.4/src/iipyper/midi.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,24 +92,25 @@
         # for port in in_ports:
         #     try:
         #         self.in_ports[port] = mido.open_input(
         #             port, callback=self.get_callback(port))
         #     except Exception:
         #         print(f"""WARNING: MIDI input {port} not found""")
         for port in in_ports:
+            cb = self.get_callback(port)
             try:
-                self.in_ports[port] = mido.open_input(
-                    port, callback=self.get_callback(port))
+                self.in_ports[port] = mido.open_input(port, callback=cb)
             except Exception:
-                print(f"""WARNING: MIDI input {port} not found""")
+                print(f"""WARNING: failed to open MIDI input {port}""")
         for i in range(virtual_in_ports):
             port = f'To iipyper {i+1}'
+            cb = self.get_callback(port)
             try:
                 self.in_ports[port] = mido.open_input(
-                    port, virtual=True, callback=self.get_callback(port))
+                    port, virtual=True, callback=cb)
             except Exception: print(
                 f'WARNING: iipyper: failed to open virtual MIDI port {port}')
 
         if self.verbose:
             print(f"""opened MIDI input ports: {list(self.in_ports)}""")
 
         ##### WIP
```

### Comparing `iipyper-0.1.3/src/iipyper/osc.py` & `iipyper-0.1.4/src/iipyper/osc.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,15 +587,16 @@
                             value returned from OSC handler should start with route
                             """)
                         else:
                             client = (
                                 client[0] if return_host is None else return_host,
                                 client[1] if return_port is None else return_port
                             )
-                            print('iipyper OSC return', client, r)
+                            if self.verbose > 0:
+                                print('iipyper OSC return', client, r)
                             try:
                                 self.get_client_by_sender(client).send_message(
                                     r[0], r[1:])
                             except ValueError:
                                 rt = [type(item) for item in r]
                                 print(
                                     f'iipyper OSC return to {r[0]} failed,'
```

### Comparing `iipyper-0.1.3/src/iipyper/timing.py` & `iipyper-0.1.4/src/iipyper/timing.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.3/src/iipyper/tui.py` & `iipyper-0.1.4/src/iipyper/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,31 @@
     from rich.panel import Panel
     from rich.pretty import Pretty
 
     from textual.app import App, ComposeResult
     from textual.reactive import reactive
     from textual.widgets import Header, Footer, Static, Button, Log, RichLog, Label
     from textual.css.query import NoMatches, TooManyMatches
+    from textual.screen import Screen
 
     class TUI(App):
         """Base Textual app for iipyper programs."""
         ## e.g.
         # CSS_PATH = 'my_tui.css'
         # BINDINGS = [
         #     ("a", "my_a_action", "Do something when A is pressed"),
-        #     ("b", "my_b_action", "Do somethign when B is pressed")]
+        #     ("b", "my_b_action", "Do something when B is pressed")]
 
         def __init__(self):
             super().__init__()
             # self.std_log = RichLog(id='std_log')
             self.std_log = Log(id='std_log')
             self.buffered_writes = []
 
-        def compose(self) -> ComposeResult:
+        def compose(self):
             """Create child widgets for the Textual App.
             
             override this to build the TUI for your iipyper app.
             """
             yield Header()
             yield self.std_log
             yield Footer()
@@ -66,15 +67,17 @@
                 pass
         
         def set_mouse_move(self, f):
             self.on_mouse_move = f
             return f
 
         def on_button_pressed(self, event: Button.Pressed) -> None:
-            getattr(self, f'action_{event.button.id}')()
+            k = f'action_{event.button.id}'
+            if hasattr(self, k):
+                getattr(self, k)()
 
         def flush(self): pass
         def write(self, s):
             """for redirecting stdout to a file-like"""
             if self.is_running:
                 if len(self.buffered_writes):
                     s = '\n'.join(self.buffered_writes)
@@ -122,18 +125,21 @@
             with a reactive `value` attribute, which updates the node when set.
             then calling my_tui(my_node_id=my_value) will update the node.
             """
             if not self.is_running:
                 return
             for k in kw:
                 try:
-                    node = self.query_one('#'+k)
+                    # TODO: search later screens?
+                    node = self.screen_stack[0].query_one('#'+k)
                     node.value = kw[k]
-                except (NoMatches, TooManyMatches):
+                except NoMatches:
                     self.print(f'TUI: node "{k}" not found')
+                except TooManyMatches:
+                    self.print(f'TUI: node "{k}" multiply defined')
                 except AttributeError:
                     self.print(f'TUI: node "{k}" lacks value "reactive"')
 
 
 except ImportError as e:
     print(e.msg)
     print('install package `textual` for terminal user interface')
```

### Comparing `iipyper-0.1.3/src/iipyper/types.py` & `iipyper-0.1.4/src/iipyper/types.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.3/src/iipyper/util.py` & `iipyper-0.1.4/src/iipyper/util.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.3/PKG-INFO` & `iipyper-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: iipyper
-Version: 0.1.3
-Summary: python package for easy MIDI, OSC, event loops
+Version: 0.1.4
+Summary: A Ppython package for rapid prototyping with MIDI and OSC
 Home-page: https://github.com/Intelligent-Instruments-Lab/iipyper
 License: MIT
 Author: Victor Shepardson
 Author-email: victor.shepardson@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: fire (>=0.6.0,<0.7.0)
 Requires-Dist: mido (>=1.3.0,<2.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pydantic-numpy (>=4.1.0,<5.0.0)
 Requires-Dist: python-osc (>=1.8.3,<2.0.0)
 Requires-Dist: python-rtmidi (>=1.5.7,<2.0.0)
 Requires-Dist: sounddevice (>=0.4.6,<0.5.0)
-Requires-Dist: textual (>=0.41.0,<0.42.0)
+Requires-Dist: textual (>=0.63.0,<0.64.0)
 Project-URL: Documentation, https://intelligent-instruments-lab.github.io/iipyper/
 Project-URL: Repository, https://github.com/Intelligent-Instruments-Lab/iipyper
 Description-Content-Type: text/markdown
 
 # iipyper ([Documentation](https://intelligent-instruments-lab.github.io/iipyper/))
 
 `iipyper` is a Python package for fast creation of [Open Sound Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC) and [MIDI](https://en.wikipedia.org/wiki/MIDI)-based event loops.
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: iipyper Version: 0.1.3 Summary: python package for
-easy MIDI, OSC, event loops Home-page: https://github.com/Intelligent-
-Instruments-Lab/iipyper License: MIT Author: Victor Shepardson Author-email:
-victor.shepardson@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: mido (>=1.3.0,<2.0.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0) Requires-Dist: pydantic-numpy
-(>=4.1.0,<5.0.0) Requires-Dist: python-osc (>=1.8.3,<2.0.0) Requires-Dist:
-python-rtmidi (>=1.5.7,<2.0.0) Requires-Dist: sounddevice (>=0.4.6,<0.5.0)
-Requires-Dist: textual (>=0.41.0,<0.42.0) Project-URL: Documentation, https://
-intelligent-instruments-lab.github.io/iipyper/ Project-URL: Repository, https:/
-/github.com/Intelligent-Instruments-Lab/iipyper Description-Content-Type: text/
-markdown # iipyper ([Documentation](https://intelligent-instruments-
-lab.github.io/iipyper/)) `iipyper` is a Python package for fast creation of
-[Open Sound Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC)
-and [MIDI](https://en.wikipedia.org/wiki/MIDI)-based event loops. It is
-designed for creatives who want to explore the Python ecosystem and experiment
-with music and, for example, machine learning. For examples and tutorials of
-how to use `iipyper`, see our [examples repo](https://github.com/intelligent-
-instruments-lab/iil-examples) (TBC). ## Install `iipyper` can be installed via
-[PyPI](https://pypi.org/project/iipyper): ```sh pip install iipyper ``` ##
-Develop ```sh git clone git@github.com:Intelligent-Instruments-Lab/iipyper.git
-cd iipyper poetry install iipyper ``` ## Contact `iipyper` is developed by the
-[Intelligent Instruments Lab](https://iil.is/about). Get in touch to
-[collaborate](https://iil.is/collaborate): â¦ _i_i_l_._i_s â¦ _F_a_c_e_b_o_o_k â¦
-_I_n_s_t_a_g_r_a_m â¦ _X_ _(_T_w_i_t_t_e_r_) â¦ _Y_o_u_T_u_b_e â¦ _D_i_s_c_o_r_d â¦ _G_i_t_H_u_b â¦ _L_i_n_k_e_d_I_n â¦
-_E_m_a_i_l â¦ ## Funding The Intelligent Instruments project (INTENT) is funded by
-the European Research Council (ERC) under the European Unionâs Horizon 2020
-research and innovation programme (Grant agreement No. 101001848).
+Metadata-Version: 2.1 Name: iipyper Version: 0.1.4 Summary: A Ppython package
+for rapid prototyping with MIDI and OSC Home-page: https://github.com/
+Intelligent-Instruments-Lab/iipyper License: MIT Author: Victor Shepardson
+Author-email: victor.shepardson@gmail.com Requires-Python: >=3.10,<3.13
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: fire (>=0.6.0,<0.7.0) Requires-Dist:
+mido (>=1.3.0,<2.0.0) Requires-Dist: pydantic (>=2.5.2,<3.0.0) Requires-Dist:
+pydantic-numpy (>=4.1.0,<5.0.0) Requires-Dist: python-osc (>=1.8.3,<2.0.0)
+Requires-Dist: python-rtmidi (>=1.5.7,<2.0.0) Requires-Dist: sounddevice
+(>=0.4.6,<0.5.0) Requires-Dist: textual (>=0.63.0,<0.64.0) Project-URL:
+Documentation, https://intelligent-instruments-lab.github.io/iipyper/ Project-
+URL: Repository, https://github.com/Intelligent-Instruments-Lab/iipyper
+Description-Content-Type: text/markdown # iipyper ([Documentation](https://
+intelligent-instruments-lab.github.io/iipyper/)) `iipyper` is a Python package
+for fast creation of [Open Sound Control](https://en.wikipedia.org/wiki/
+Open_Sound_Control) (OSC) and [MIDI](https://en.wikipedia.org/wiki/MIDI)-based
+event loops. It is designed for creatives who want to explore the Python
+ecosystem and experiment with music and, for example, machine learning. For
+examples and tutorials of how to use `iipyper`, see our [examples repo](https:/
+/github.com/intelligent-instruments-lab/iil-examples) (TBC). ## Install
+`iipyper` can be installed via [PyPI](https://pypi.org/project/iipyper): ```sh
+pip install iipyper ``` ## Develop ```sh git clone git@github.com:Intelligent-
+Instruments-Lab/iipyper.git cd iipyper poetry install iipyper ``` ## Contact
+`iipyper` is developed by the [Intelligent Instruments Lab](https://iil.is/
+about). Get in touch to [collaborate](https://iil.is/collaborate): â¦ _i_i_l_._i_s
+â¦ _F_a_c_e_b_o_o_k â¦ _I_n_s_t_a_g_r_a_m â¦ _X_ _(_T_w_i_t_t_e_r_) â¦ _Y_o_u_T_u_b_e â¦ _D_i_s_c_o_r_d â¦ _G_i_t_H_u_b
+â¦ _L_i_n_k_e_d_I_n â¦ _E_m_a_i_l â¦ ## Funding The Intelligent Instruments project
+(INTENT) is funded by the European Research Council (ERC) under the European
+Unionâs Horizon 2020 research and innovation programme (Grant agreement No.
+101001848).
```

