# Comparing `tmp/firefly_client-2.9.0.tar.gz` & `tmp/firefly_client-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_client-2.9.0.tar", last modified: Mon Oct  9 20:32:54 2023, max compression
+gzip compressed data, was "firefly_client-3.0.0.tar", last modified: Fri May 24 20:03:25 2024, max compression
```

## Comparing `firefly_client-2.9.0.tar` & `firefly_client-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2023-10-09 20:32:54.207385 firefly_client-2.9.0/
--rw-r--r--   0 jsinghal  (5826) staff       (20)      442 2023-10-09 20:32:54.207481 firefly_client-2.9.0/PKG-INFO
--rw-r--r--   0 jsinghal  (5826) staff       (20)      938 2023-10-09 20:27:18.000000 firefly_client-2.9.0/README.md
-drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2023-10-09 20:32:54.205260 firefly_client-2.9.0/firefly_client/
--rw-r--r--   0 jsinghal  (5826) staff       (20)      217 2023-08-17 00:26:14.000000 firefly_client-2.9.0/firefly_client/__init__.py
--rw-r--r--   0 jsinghal  (5826) staff       (20)     4287 2023-09-14 22:13:57.000000 firefly_client-2.9.0/firefly_client/env.py
--rw-r--r--   0 jsinghal  (5826) staff       (20)     3647 2023-10-09 20:27:27.000000 firefly_client-2.9.0/firefly_client/fc_utils.py
--rw-r--r--   0 jsinghal  (5826) staff       (20)     8069 2023-08-17 00:26:14.000000 firefly_client-2.9.0/firefly_client/ffws.py
--rw-r--r--   0 jsinghal  (5826) staff       (20)    73140 2023-10-09 20:27:27.000000 firefly_client-2.9.0/firefly_client/firefly_client.py
--rw-r--r--   0 jsinghal  (5826) staff       (20)    10468 2023-08-17 00:26:14.000000 firefly_client-2.9.0/firefly_client/plot.py
--rw-r--r--   0 jsinghal  (5826) staff       (20)     8310 2023-08-17 00:26:14.000000 firefly_client-2.9.0/firefly_client/range_values.py
-drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2023-10-09 20:32:54.206572 firefly_client-2.9.0/firefly_client.egg-info/
--rw-r--r--   0 jsinghal  (5826) staff       (20)      442 2023-10-09 20:32:54.000000 firefly_client-2.9.0/firefly_client.egg-info/PKG-INFO
--rw-r--r--   0 jsinghal  (5826) staff       (20)      477 2023-10-09 20:32:54.000000 firefly_client-2.9.0/firefly_client.egg-info/SOURCES.txt
--rw-r--r--   0 jsinghal  (5826) staff       (20)        1 2023-10-09 20:32:54.000000 firefly_client-2.9.0/firefly_client.egg-info/dependency_links.txt
--rw-r--r--   0 jsinghal  (5826) staff       (20)       26 2023-10-09 20:32:54.000000 firefly_client-2.9.0/firefly_client.egg-info/requires.txt
--rw-r--r--   0 jsinghal  (5826) staff       (20)       15 2023-10-09 20:32:54.000000 firefly_client-2.9.0/firefly_client.egg-info/top_level.txt
--rw-r--r--   0 jsinghal  (5826) staff       (20)       67 2023-10-09 20:32:54.207776 firefly_client-2.9.0/setup.cfg
--rwxr-xr-x   0 jsinghal  (5826) staff       (20)      605 2023-10-09 20:26:22.000000 firefly_client-2.9.0/setup.py
-drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2023-10-09 20:32:54.207057 firefly_client-2.9.0/test/
--rw-r--r--   0 jsinghal  (5826) staff       (20)     2499 2023-08-17 00:26:14.000000 firefly_client-2.9.0/test/test-5-instances-3-channels.py
--rw-r--r--   0 jsinghal  (5826) staff       (20)     2196 2023-08-17 00:26:14.000000 firefly_client-2.9.0/test/test-simple-callback-response.py
+drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2024-05-24 20:03:25.620240 firefly_client-3.0.0/
+-rw-r--r--   0 jsinghal  (5826) staff       (20)     1758 2023-08-17 00:26:14.000000 firefly_client-3.0.0/License.txt
+-rw-r--r--   0 jsinghal  (5826) staff       (20)       20 2024-03-26 00:35:42.000000 firefly_client-3.0.0/MANIFEST.in
+-rw-r--r--   0 jsinghal  (5826) staff       (20)      381 2024-05-24 20:03:25.620315 firefly_client-3.0.0/PKG-INFO
+-rw-r--r--   0 jsinghal  (5826) staff       (20)      902 2024-04-16 01:02:10.000000 firefly_client-3.0.0/README.md
+drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2024-05-24 20:03:25.618481 firefly_client-3.0.0/firefly_client/
+-rw-r--r--   0 jsinghal  (5826) staff       (20)      217 2023-08-17 00:26:14.000000 firefly_client-3.0.0/firefly_client/__init__.py
+-rw-r--r--   0 jsinghal  (5826) staff       (20)     4277 2024-05-24 20:02:15.000000 firefly_client-3.0.0/firefly_client/env.py
+-rw-r--r--   0 jsinghal  (5826) staff       (20)     3780 2024-05-24 20:02:15.000000 firefly_client-3.0.0/firefly_client/fc_utils.py
+-rw-r--r--   0 jsinghal  (5826) staff       (20)     8069 2023-08-17 00:26:14.000000 firefly_client-3.0.0/firefly_client/ffws.py
+-rw-r--r--   0 jsinghal  (5826) staff       (20)    79151 2024-05-24 20:02:37.000000 firefly_client-3.0.0/firefly_client/firefly_client.py
+-rw-r--r--   0 jsinghal  (5826) staff       (20)    10468 2023-08-17 00:26:14.000000 firefly_client-3.0.0/firefly_client/plot.py
+-rw-r--r--   0 jsinghal  (5826) staff       (20)     8310 2023-08-17 00:26:14.000000 firefly_client-3.0.0/firefly_client/range_values.py
+drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2024-05-24 20:03:25.619529 firefly_client-3.0.0/firefly_client.egg-info/
+-rw-r--r--   0 jsinghal  (5826) staff       (20)      381 2024-05-24 20:03:25.000000 firefly_client-3.0.0/firefly_client.egg-info/PKG-INFO
+-rw-r--r--   0 jsinghal  (5826) staff       (20)      501 2024-05-24 20:03:25.000000 firefly_client-3.0.0/firefly_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jsinghal  (5826) staff       (20)        1 2024-05-24 20:03:25.000000 firefly_client-3.0.0/firefly_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jsinghal  (5826) staff       (20)       26 2024-05-24 20:03:25.000000 firefly_client-3.0.0/firefly_client.egg-info/requires.txt
+-rw-r--r--   0 jsinghal  (5826) staff       (20)       15 2024-05-24 20:03:25.000000 firefly_client-3.0.0/firefly_client.egg-info/top_level.txt
+-rw-r--r--   0 jsinghal  (5826) staff       (20)       67 2024-05-24 20:03:25.620566 firefly_client-3.0.0/setup.cfg
+-rwxr-xr-x   0 jsinghal  (5826) staff       (20)      605 2024-05-24 20:02:15.000000 firefly_client-3.0.0/setup.py
+drwxr-xr-x   0 jsinghal  (5826) staff       (20)        0 2024-05-24 20:03:25.620069 firefly_client-3.0.0/test/
+-rw-r--r--   0 jsinghal  (5826) staff       (20)     2499 2023-08-17 00:26:14.000000 firefly_client-3.0.0/test/test-5-instances-3-channels.py
+-rw-r--r--   0 jsinghal  (5826) staff       (20)     2196 2023-08-17 00:26:14.000000 firefly_client-3.0.0/test/test-simple-callback-response.py
```

### Comparing `firefly_client-2.9.0/README.md` & `firefly_client-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 ## Usage
 
 The client must be connected to a Firefly server. The Firefly
 repository is located at http://github.com/Caltech-IPAC/firefly.
 Standalone Firefly servers may be obtained from
 [this Dockerhub repository](https://hub.docker.com/r/ipac/firefly/).
 
-For detailed explanation on the usage, see [the online documentation](https://firefly-client.lsst.io),
-or [the documentation source file](doc/index.rst). Following is a very simple example:
+For detailed explanation on the usage, see [the online documentation](https://caltech-ipac.github.io/firefly_client). Following is a very simple example:
 
 ```
 from firefly_client import FireflyClient
 fc = FireflyClient.make_client()  # can also explictly pass url of a firefly server; default is http://localhost:8080/firefly
 ```
 
 A FITS image may be uploaded and displayed:
```

### Comparing `firefly_client-2.9.0/firefly_client/env.py` & `firefly_client-3.0.0/firefly_client/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class Env:
     # all os environment access here
     firefly_lab_extension = str_2_bool(os.environ.get(ENV_FF_LAB_EXT, ''))
     firefly_channel_lab = os.environ.get(ENV_FF_CHANNEL_LAB)
     firefly_url_lab = os.environ.get(ENV_FF_URL_LAB)
     firefly_url = os.environ.get(ENV_FF_URL)
     firefly_channel_from_env = os.environ.get(ENV_FF_CHANNEL)
-    firefly_html = os.environ.get(ENV_FF_HTML, 'slate.html')
+    firefly_html = os.environ.get(ENV_FF_HTML, '')
     user = os.environ.get(ENV_USER, '')
 
     @classmethod
     def validate_lab_client(cls, generate_lab_ext_channel):
         """ return the url and channel or raise an Error """
         not cls.lab_ext_valid() and cls.raise_invalid_lab_error()
         return cls.firefly_url_lab, cls.resolve_lab_channel(generate_lab_ext_channel)
```

### Comparing `firefly_client-2.9.0/firefly_client/fc_utils.py` & `firefly_client-3.0.0/firefly_client/fc_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,17 @@
     'CreateRegionLayer': 'DrawLayerCntlr.RegionPlot.createLayer',
     'DeleteRegionLayer': 'DrawLayerCntlr.RegionPlot.deleteLayer',
     'AddRegionData': 'DrawLayerCntlr.RegionPlot.addRegion',
     'RemoveRegionData': 'DrawLayerCntlr.RegionPlot.removeRegion',
     'PlotMask': 'ImagePlotCntlr.plotMask',
     'DeleteOverlayMask': 'ImagePlotCntlr.deleteOverlayPlot',
     'AddCell': 'layout.addCell',
+    'SetLayoutMode': 'layout.setLayoutMode',
+    'UpdateLayout': 'layout.updateLayout',
+    'TriviewLayout': 'layout.triviewLayout',
     'ShowCoverage': 'layout.enableSpecialViewer',
     'ShowImageMetaData': 'layout.enableSpecialViewer',
     'ReinitViewer': 'app_data.reinitApp',
     'ShowHiPS': 'ImagePlotCntlr.PlotHiPS',
     'ShowImageOrHiPS': 'ImagePlotCntlr.plotHiPSOrImage',
     'ImagelineBasedFootprint': 'DrawLayerCntlr.ImageLineBasedFP.imagelineBasedFPCreate',
     'StartLabWindow': 'StartLabWindow',
```

### Comparing `firefly_client-2.9.0/firefly_client/ffws.py` & `firefly_client-3.0.0/firefly_client/ffws.py`

 * *Files identical despite different names*

### Comparing `firefly_client-2.9.0/firefly_client/firefly_client.py` & `firefly_client-3.0.0/firefly_client/firefly_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         URL for Firefly server, e.g. https://lsst-demo.ncsa.illinois.edu/firefly.
         Defaults to the value of the environment variable FIREFLY_URL, if defined;
         or to 'http://localhost:8080/firefly' if FIREFLY_URL is not defined.
     channel : `str`
         WebSocket channel ID. Default is None which auto-generates a unique string.
     html_file : `str`
         HTML file that is the 'landing page' for users, appended to the URL.
-        Defaults to 'slate.html'.
+        Defaults to ''. If the landing page in 'slate.html' it puts FireflyClient into slate mode.
     make_default : `bool`
         If True, make this the default FireflyClient instance. Default False.
     use_lab_env : `bool`
         If True, try to use environment variables for Jupyterlab. This can only be True in the
         Jupyter lab environment, otherwise there is an error. Default False.
     start_tab: `bool`
         If True, bring up a Jupyterlab or a browser tab for Firefly. Default False.
@@ -70,14 +70,49 @@
     token: `str` or None
         A token for connecting to a Firefly server that requires
         authentication. The provided token will be appended to the
         string "Bearer " to form the value of the "Authorization" header
         in the sessions attribute.
     """
 
+    TAB_ID = 'firefly-viewer-tab-id'
+    TRIVIEW_ICov_Ch_T = 'TRIVIEW_ICov_Ch_T'
+    TRIVIEW_I_ChCov_T = 'TRIVIEW_I_ChCov_T'
+    BIVIEW_ICov_Ch = 'BIVIEW_ICov_Ch'
+    BIVIEW_I_ChCov = 'BIVIEW_I_ChCov'
+    BIVIEW_T_IChCov = 'BIVIEW_T_IChCov'
+    BIVIEW_IChCov_T = 'BIVIEW_IChCov_T'
+    tri_view_types_list = [
+        TRIVIEW_ICov_Ch_T,
+        TRIVIEW_I_ChCov_T,
+        BIVIEW_ICov_Ch,
+        BIVIEW_I_ChCov,
+        BIVIEW_T_IChCov,
+        BIVIEW_IChCov_T
+    ]
+
+    tri_view_layout_desc = {
+        TRIVIEW_ICov_Ch_T: 'top left: image/cov, top right: charts, bottom: tables',
+        TRIVIEW_I_ChCov_T: 'top left: image, top right: charts/cov, bottom: tables',
+        BIVIEW_ICov_Ch: 'left: image/cov, right: charts',
+        BIVIEW_I_ChCov: 'left: image, right: charts/cov',
+        BIVIEW_T_IChCov: 'left: tables, right: image/charts/cov',
+        BIVIEW_IChCov_T: 'left: image/charts/cov, right: tables',
+    }
+
+    # viewer modes
+    TRIVIEW_VIEWER = 'FireflyViewer'
+    SLATE_VIEWER = 'FireflySlate'
+    NO_VIEWER = 'NO_VIEWER'
+    _viewer_modes = [TRIVIEW_VIEWER,SLATE_VIEWER,NO_VIEWER]
+
+    # viewer ids
+    PINNED_CHART_VIEWER_ID = 'PINNED_CHART_VIEWER_ID'
+    PINNED_IMAGE_VIEWER_ID = 'DEFAULT_FITS_VIEWER_ID'
+
     _debug = False
     # Keep track of instances.
     instances = []
 
     """All events are enabled for the listener (`str`)."""
 
     # id for table, region layer, extension
@@ -98,20 +133,20 @@
         start_browser_tab : `bool`
             If True start a browser tab, if False start a lab tab. start_tab must
             also be True.
             To start a new tab you will have to disable popup blocking for the Jupyterlab site.
                 Chrome: look at the right side of the address bar
                 Firefox: a preference bar appears at the top
                 Safari: shows an animation to follow on the left side bar
-        html_file : `str`, optional
+        html_file: `str`, optional
             HTML file that is the 'landing page' for users, appended to the URL.
-            You should almost always take the default, e.g. 'slate.html'.
             Defaults to the value of the environment variable 'FIREFLY_URL' if
-            it is defined: otherwise defaults to None.
-        start_tab : `bool`, optional
+            it is defined: otherwise defaults to ''.
+            If the landing page in 'slate.html' it puts FireflyClient into slate mode.
+        start_tab: `bool`, optional
             If True, bring up a Jupyterlab or a browser tab for Firefly. You should almost always take the default.
         token: `str` or None
             A token for connecting to a Firefly server that requires
             authentication. The provided token will be appended to the
             string "Bearer " to form the value of the "Authorization" header
             in the sessions attribute.
         verbose: `boolean`
@@ -123,37 +158,38 @@
             A FireflyClient that works in the lab environment
         """
         tab_type = BROWSER if (start_browser_tab and start_tab) else (LAB if start_tab else None)
         url, channel = Env.validate_lab_client(tab_type == BROWSER)
         fc = cls(url, channel, html_file, token)
         if tab_type:
             verbose and tab_type == BROWSER and Env.show_start_browser_tab_msg(fc.get_firefly_url())
-            fc._lab_env_tab_start(tab_type)
-        return fc
+            fc._lab_env_tab_start(tab_type, html_file)
+        return fcse
 
     @classmethod
     def make_client(cls, url=_default_url, html_file=_def_html_file, launch_browser=True,
-                    channel_override=None, verbose=False, token=None):
+                    channel_override=None, verbose=False, token=None, viewer_override=None):
         """
         Factory method to create a Firefly client in a plain Python, IPython, or
         notebook session, and attempt to open a display.  If a display cannot be
         opened, a link will be displayed.
 
         Parameters
         ----------
-        url : `str`, optional
+        url: `str`, optional
             URL of the Firefly server. The default is determined by checking
             environment variables 'fireflyURLLab' and 'FIREFLY_URL'; if these
             are undefined, then the default is 'http://localhost:8080/firefly'
             for the case of a user running a Firefly server on their desktop.
-        html_file : `str`, optional
+        html_file: `str`, optional
             HTML file that is the 'landing page' for users, appended to the URL.
-            The default is the value of the environment variable 'FIREFLY_HTML'
-            if it is defined; otherwise 'slate.html'.
-        launch_browser : `bool`, optional
+            Defaults to the value of the environment variable 'FIREFLY_URL' if
+            it is defined: otherwise defaults to ''.
+            If the landing page in 'slate.html' it puts FireflyClient into slate mode.
+        launch_browser: `bool`, optional
             If True, attempt to launch a browser tab for the Firefly viewer.
             If that attempt is unsuccessful, a link for the Firefly viewer is
             displayed.
         channel_override: `str` or None
             If channel_override is None, the value of the environment variable
             'FIREFLY_CHANNEL' is checked. If unset, then a URL-safe channel
             string is generated.
@@ -162,26 +198,31 @@
         verbose: `bool`
             If True, print instructions if web browser is not opened (default *false*)
         token: `str` or None
             A token for connecting to a Firefly server that requires
             authentication. The provided token will be appended to the
             string "Bearer " to form the value of the "Authorization" header
             in the sessions attribute.
+        viewer_override: `str`
+            This parameter is almost never used, default to None.
+            It is only for those special circumstances that you would use
+            firefly_client to control a custom created interface that is not a triview ora slate view.
+            maybe one of FireflyClient.TRIVIEW_VIEWER, FireflyClient.SLATE_VIEWER, FireflyClient.NO_VIEWER,
 
         Returns
         -------
         fc : `FireflyClient`
             A FireflyClient that works in the lab environment
         """
-        fc = cls(url, Env.resolve_client_channel(channel_override), html_file, token)
+        fc = cls(url, Env.resolve_client_channel(channel_override), html_file, token, viewer_override)
         verbose and Env.show_start_browser_tab_msg(fc.get_firefly_url())
         launch_browser and fc.launch_browser()
         return fc
 
-    def __init__(self, url, channel, html_file=_def_html_file, token=None):
+    def __init__(self, url, channel, html_file=_def_html_file, token=None, viewer_override=None):
         DebugMarker.firefly_client_debug = FireflyClient._debug
         FireflyClient.instances.append(weakref.ref(self))
 
         ssl = url.startswith('https://')
         self.wsproto = 'wss' if ssl else 'ws'
         self.location = url[8:] if ssl else url[7:]
         self.location = self.location[:-1] if self.location.endswith('/') else self.location
@@ -195,38 +236,54 @@
         protocol = 'https' if ssl else 'http'
         self.url_cmd_service = urljoin('{}://{}/'.format(protocol, self.location), 'sticky/CmdSrv')
         self.url_browser = urljoin(urljoin('{}://{}/'.format(protocol, self.location), html_file), '?__wsch=')
         self.url_bw = self.url_browser  # keep around for backward compatibility
         self.session = requests.Session()
         token and ssl and self.session.headers.update(self.auth_headers)
         not ssl and token and warn('token ignored: should be None when url starts with http://')
+        self.firefly_viewer = FireflyClient.get_viewer_mode(html_file,viewer_override)
         debug('new instance: %s' % url)
 
-    def _lab_env_tab_start(self, tab_type):
+    def _lab_env_tab_start(self, tab_type, html_file):
         """start a tab in the lab environment, tab_type must be 'lab' or 'browser' """
         self.lab_env_tab_type = tab_type
         if tab_type == BROWSER:
             idx = self.channel.find('__viewer')
             c = self.channel[0:idx] if idx > -1 else self.channel  # the ext will add '__viewer' so I have to remove it
-            self.dispatch(ACTION_DICT['StartBrowserTab'], {'channel': c}, Env.firefly_channel_lab)
+            self.dispatch(ACTION_DICT['StartBrowserTab'],
+                          {'channel': c, 'fireflyHtmlFile': _def_html_file}, Env.firefly_channel_lab)
         elif tab_type == LAB:
             if not self.render_tree_id:
-                self.render_tree_id = 'slateClient-%s-%s' % (len(self.instances), round(time.time()))
-            self.show_lab_tab()
+                self.render_tree_id = FireflyClient.TAB_ID  # no longer generating redner_tree_id
+                # self.render_tree_id = 'slateClient-%s-%s' % (len(self.instances), round(time.time()))
+            self.show_lab_tab(html_file)
 
-    def show_lab_tab(self):
+    def show_lab_tab(self, html_file):
         """If using a jupyter lab tab- show it or reopen it. If not using a lab tab then noop"""
-        self.lab_env_tab_type = LAB and self.dispatch(ACTION_DICT['StartLabWindow'], {})
+        self.lab_env_tab_type = (LAB and
+                                 self.dispatch(ACTION_DICT['StartLabWindow'],
+                                               {'fireflyHtmlFile': html_file}))
+
+    @staticmethod
+    def get_viewer_mode(html_file, viewer_override):
+        if viewer_override:
+            if viewer_override in _viewer_modes:
+                return viewer_override
+            else:
+                warn('viewer_override mode: {} is not a recognized mode, using {}'.format(viewer_override, UNKNOWN))
+                return UNKNOWN
+        else:
+            return FireflyClient.SLATE_VIEWER if html_file == 'slate.html' else FireflyClient.TRIVIEW_VIEWER
 
     def _send_url_as_get(self, url):
         return self.call_response(self.session.get(url, headers=self.header_from_ws))
 
     def _send_url_as_post(self, data):
         return self.call_response(self.session.post(self.url_cmd_service, data=data, headers=self.header_from_ws))
-    
+
     def call_response(self, response):
         if response.status_code != 200:
             raise ValueError(Env.failed_net_message(self.url, response.status_code))
         try:
             status = json.loads(response.text)
             return status[0]
         except ValueError as err:
@@ -243,14 +300,18 @@
         """Check if the page is connected.
         """
         ip = socket.gethostbyname(socket.gethostname())
         url = self.url_cmd_service + '?cmd=pushAliveCheck&ipAddress=%s' % ip
         retval = self._send_url_as_get(url)
         return retval['active']
 
+    def is_triview(self): return self.firefly_viewer == FireflyClient.TRIVIEW_VIEWER
+
+    def is_slate(self): return self.firefly_viewer == FireflyClient.SLATE_VIEWER
+
     @staticmethod
     def _make_pid_param(plot_id):
         return ','.join(plot_id) if isinstance(plot_id, list) else plot_id
 
 # -----------------------------------------------------------------
 # -----------------------------------------------------------------
 # Public API Begins
@@ -290,15 +351,15 @@
             The name of the event to be removed from the callback listener
             (the default is `ALL`, all events).
 
         Returns
         -------
         out : none
 
-        .. note:: `callback` in listener list is removed if all events are removed from the callback.
+        .. note:: `callback` in the listener list is removed if all events are removed from the callback.
         """
         FFWs.remove_listener(self.channel, self.location, callback, name)
 
     def wait_for_events(self):
         """
         Wait over events from the server.
 
@@ -344,15 +405,15 @@
             url = self.get_firefly_url()
         try:
             ipy_str = str(type(get_ipython()))
         except NameError:
             ipy_str = ''
         if 'zmqshell' in ipy_str:
             from IPython.display import display, HTML
-            display( HTML('Open your web browser to <a href="{}"" target="_blank">this link</a>'.format(url)))
+            display(HTML('Open your web browser to <a href="{}"" target="_blank">this link</a>'.format(url)))
         else:
             print('Open your web browser to {}'.format(url))
 
     def launch_browser(self, channel=None, force=False, verbose=True):
         """
         Launch a browser with the Firefly Tools viewer and the channel set.
 
@@ -513,24 +574,24 @@
     def dispatch(self, action_type, payload, override_channel=None):
         """
         Dispatch the action to the server by using 'POST' request.
 
         Parameters
         ----------
         action_type : `str`
-            Action type, one of actions from FireflyClient's attribute, `ACTION_DICT`.
+            Action type, one of the actions from FireflyClient's attribute, `ACTION_DICT`.
         payload : `dict`
             Payload, the content varies based on the value of `action_type`.
         override_channel : `str`
             overrides the default channel
 
         Returns
         -------
         out : `dict`
-            Status of remotely dispatch, like {'success': True}.
+            Status of the remote dispatch, like {'success': True}.
         """
 
         if payload is None:
             payload = {}
         if self.render_tree_id:
             payload['renderTreeId'] = self.render_tree_id
         channel = self.channel if override_channel is None else override_channel
@@ -545,14 +606,39 @@
     # -------------------------
 
     # --------------------------------------------------------------------------
     # action on adding cell for slate viewer,
     #           showing fits, tables, XYPlot, adding extension, and adding mask
     # -------------------------------------------------------------------------
 
+    def change_triview_layout(self, layout):
+        """
+        Change the tri view layout
+
+        Parameters
+        ----------
+        layout : `str`
+            should be one of
+            FireflyClient.TRIVIEW_ICov_Ch_T - top left: image/cov, top right: charts, bottom: tables
+            FireflyClient.TRIVIEW_I_ChCov_T - top left: image, top right: charts/cov, bottom: tables
+            FireflyClient.BIVIEW_ICov_Ch - left: image/cov, right: charts
+            FireflyClient.BIVIEW_I_ChCov - left: image, right: charts/cov
+            FireflyClient.BIVIEW_T_IChCov- left: tables, right: image/charts/cov
+            FireflyClient.BIVIEW_IChCov_T- left: image/charts/cov, right: tables
+        """
+
+        if not self.is_triview():
+            return {'success': True, 'warning': 'change_triview_layout ignored when not in triview mode'}
+        if layout not in FireflyClient.tri_view_types_list:
+            warning = '{} is an unknown layout type, valid types: {}'.format(layout, FireflyClient.tri_view_types_list)
+            return {'success': False, 'warning': warning}
+
+        self.dispatch(ACTION_DICT['TriviewLayout'], {'triviewLayout': layout})
+        return {'success': True, 'description': FireflyClient.tri_view_layout_desc[layout]}
+
     def add_cell(self, row, col, width, height, element_type, cell_id=None):
         """
         Add a slate viewer cell.
 
         Parameters
         ----------
         row : `int`
@@ -569,14 +655,17 @@
             Cell Id.
 
         Returns
         -------
         out : `dict`
             Status of the request, like {'success': True, 'cell_id': 'Cell-1'}.
         """
+        if not self.is_slate():
+            return {'success': True, 'cell_id': cell_id if cell_id else 'noop',
+                    'warning': 'add_cell ignored when not in slate mode'}
 
         # force the cell_id to be 'main' for table's case
         if element_type == LO_VIEW_DICT['table']:
             if not cell_id or cell_id != 'main':
                 cell_id = 'main'
         else:
             if not cell_id:
@@ -643,25 +732,27 @@
         """
 
         wp_request = {'plotGroupId': 'groupFromPython',
                       'GroupLocked': False}
         payload = {'wpRequest': wp_request,
                    'useContextModifications': True}
 
-        if not viewer_id:
-            viewer_id = 'DEFAULT_FITS_VIEWER_ID'
-            if self.render_tree_id:
-                viewer_id += '_' + self.render_tree_id
+        warning = None
+        if not viewer_id or self.is_triview():
+            warning = 'viewer_id unnecessary and ignored in triview mode' if self.is_triview() and viewer_id else None
+            viewer_id = FireflyClient.PINNED_IMAGE_VIEWER_ID
 
         payload.update({'viewerId': viewer_id})
         plot_id and payload['wpRequest'].update({'plotId': plot_id})
         file_on_server and payload['wpRequest'].update({'file': file_on_server})
         additional_params and payload['wpRequest'].update(additional_params)
 
-        return self.dispatch(ACTION_DICT['ShowFits'], payload)
+        r = self.dispatch(ACTION_DICT['ShowFits'], payload)
+        warning and r.update({'warning': warning})
+        return r
 
     def show_fits_3color(self, three_color_params, plot_id=None, viewer_id=None):
         """
         Show a 3-color image constructed from the three color parameters
 
         Parameters
         ----------
@@ -687,21 +778,23 @@
             item.update({'GroupLocked': item.get('GroupLocked') if 'GroupLocked' in item else False})
             item.update({'plotGroupId': item.get('plotGroupId') if 'plotGroupId' in item else 'groupFromPython'})
             item.update({'Title': item.get('Title') if 'Title' in item else '3 Color'})
             if 'plotId' not in item and plot_id:
                 item.update({'plotId': plot_id})
 
         payload = {'wpRequest': three_color, 'threeColor': True, 'useContextModifications': True}
-        if not viewer_id:
-            viewer_id = 'DEFAULT_FITS_VIEWER_ID'
-            if self.render_tree_id:
-                viewer_id += '_' + self.render_tree_id
+        warning = None
+        if not viewer_id or self.is_triview():
+            warning = 'viewer_id unnecessary and ignored in triview mode' if self.is_triview() and viewer_id else None
+            viewer_id = FireflyClient.PINNED_IMAGE_VIEWER_ID
         payload.update({'viewerId': viewer_id})
 
-        return self.dispatch(ACTION_DICT['ShowFits'], payload)
+        r = self.dispatch(ACTION_DICT['ShowFits'], payload)
+        warning and r.update({'warning': warning})
+        return r
 
     def show_table(self, file_on_server=None, tbl_id=None, title=None, page_size=100, is_catalog=True,
                    meta=None, target_search_info=None, options=None, table_index=None,
                    column_spec=None, filters=None, visible=True):
         """
         Show a table.
 
@@ -908,24 +1001,30 @@
 
         .. note:: For the chart parameters, `xCol` and `yCol` are required, then all other
                   parameters are valid.
         """
 
         cid = gen_item_id('XYPlot')
 
-        if not group_id:
+        warning = None
+        if self.is_triview():
+            warning = 'group_id unnecessary and ignored in triview mode' if group_id else None
+            group_id = FireflyClient.PINNED_CHART_VIEWER_ID
+        elif not group_id:
             group_id = 'default' if standalone else tbl_id
 
         payload = {'chartId': cid, 'chartType': 'scatter',
                    'groupId': group_id, 'viewerId': group_id,
                    'params': {'tbl_id': tbl_id, **chart_params}}
 
-        return self.dispatch(ACTION_DICT['ShowXYPlot'], payload)
+        r = self.dispatch(ACTION_DICT['ShowXYPlot'], payload)
+        warning and r.update({'warning': warning})
+        return r
 
-    def show_histogram(self, tbl_id, group_id='default', **histogram_params):
+    def show_histogram(self, tbl_id, group_id=PINNED_CHART_VIEWER_ID, **histogram_params):
         """
         Show a histogram
 
         Parameters
         ----------
         tbl_id : `str`
             A table ID of the data to be plotted.
@@ -953,23 +1052,30 @@
         -------
         out : `dict`
             Status of the request, like {'success': True}.
 
         .. note:: For the histogram parameters, `col` is required.
         """
 
+        warning = None
+        if self.is_triview():
+            warning = 'group_id unnecessary and ignored in triview mode' if group_id else None
+            group_id = FireflyClient.PINNED_CHART_VIEWER_ID
+
         cid = gen_item_id('Histogram')
         payload = {'chartId': cid, 'chartType': 'histogram',
                    'groupId': group_id,
                    'viewerId': group_id,
                    'params': {'tbl_id': tbl_id, **histogram_params}}
 
-        return self.dispatch(ACTION_DICT['ShowXYPlot'], payload)
+        r = self.dispatch(ACTION_DICT['ShowXYPlot'], payload)
+        warning and r.update({'warning': warning})
+        return r
 
-    def show_chart(self, group_id='default', **chart_params):
+    def show_chart(self, group_id=PINNED_CHART_VIEWER_ID, **chart_params):
         """
         Show a plot.ly chart
 
         Plotly chart is described by a list of trace data and a layout. Any list in trace data can come from a table.
 
         For example, if a trace is defined by *{'tbl_id': 'wise', 'x': 'tables::w1pro', 'y': 'tables::w2mpro' }*,
         *x* and *y* points of the trace will come from *w1mpro* and *w2mpro* columns of the table with the id *wise*.
@@ -997,24 +1103,30 @@
         Returns
         -------
         out : `dict`
             Status of the request, like {'success': True}.
 
         """
         chart_id = chart_params.get('chartId') if 'chartId' in chart_params else gen_item_id('Plotly')
+        warning = None
+        if self.is_triview():
+            warning = 'group_id unnecessary and ignored in triview mode' if group_id else None
+            group_id = FireflyClient.PINNED_CHART_VIEWER_ID
         payload = {'chartId': chart_id,
                    'groupId': group_id,
                    'viewerId': group_id,
                    'chartType': 'plot.ly',
                    'closable': True}
 
         for item in ['data', 'layout']:
             (item in chart_params) and payload.update({item: chart_params.get(item)})
 
-        return self.dispatch(ACTION_DICT['ShowPlot'], payload)
+        r = self.dispatch(ACTION_DICT['ShowPlot'], payload)
+        warning and r.update({'warning': warning})
+        return r
 
     def show_coverage(self, viewer_id=None, table_group='main'):
         """
         Show image coverage associated with the active table in the specified table group
 
         Parameters
         ----------
@@ -1024,14 +1136,16 @@
             Table group which the image coverage associated table belongs to.
 
         Returns
         -------
         out : `dict`
             Status of the request, like {'success': True}
         """
+        if self.is_triview():
+            return {'success': True, 'warning': 'show_coverage ignored in triview mode'}
 
         view_type = 'coverImage'
         cid = viewer_id if viewer_id else ("%s-%s" % (LO_VIEW_DICT[view_type], table_group))
         payload = {'viewerType': LO_VIEW_DICT[view_type], 'cellId': cid}
         return self.dispatch(ACTION_DICT['ShowCoverage'], payload)
 
     def show_image_metadata(self, viewer_id=None, table_group='main'):
@@ -1046,14 +1160,17 @@
             Table group which the image metadata table belongs to.
 
         Returns
         -------
         out : `dict`
             Status of the request, like {'success': True}
         """
+        if self.is_triview():
+            return {'success': True, 'warning': 'show_image_metadata ignored in triview mode'}
+
         view_type = 'imageMeta'
         cid = viewer_id if viewer_id else ("%s-%s" % (LO_VIEW_DICT[view_type], table_group))
         payload = {'viewerType': LO_VIEW_DICT[view_type], 'cellId': cid}
 
         return self.dispatch(ACTION_DICT['ShowImageMetaData'], payload)
 
     def add_extension(self, ext_type, plot_id=None, title='', tool_tip='',
@@ -1186,25 +1303,27 @@
 
         if not plot_id:
             plot_id = gen_item_id('Image')
 
         payload.update({'plotId': plot_id})
         wp_request.update({'plotId': plot_id})
 
-        if not viewer_id:
-            viewer_id = 'DEFAULT_FITS_VIEWER_ID'
-            if self.render_tree_id:
-                viewer_id += '_' + self.render_tree_id
+        warning = None
+        if not viewer_id or self.is_triview():
+            warning = 'viewer_id unnecessary and ignored in triview mode' if self.is_triview() and viewer_id else None
+            viewer_id = FireflyClient.PINNED_IMAGE_VIEWER_ID
 
         payload.update({'viewerId': viewer_id})
 
         if hips_image_conversion and type(hips_image_conversion) is dict:
             payload.update({'hipsImageConversion': hips_image_conversion})
 
-        return self.dispatch(ACTION_DICT['ShowHiPS'], payload)
+        r = self.dispatch(ACTION_DICT['ShowHiPS'], payload)
+        warning and r.update({'warning': warning})
+        return r
 
     def show_image_or_hips(self, plot_id=None, viewer_id=None, image_request=None, hips_request=None,
                            fov_deg_fallover=0.12, allsky_request=None, plot_allsky_first=False):
         """
         Show a FiTS or HiPS image.
 
         Parameters
@@ -1233,18 +1352,18 @@
         """
 
         if not image_request and not hips_request:
             return
 
         if not plot_id:
             plot_id = gen_item_id('Image')
-        if not viewer_id:
-            viewer_id = 'DEFAULT_FITS_VIEWER_ID'
-            if self.render_tree_id:
-                viewer_id += '_' + self.render_tree_id
+        warning = None
+        if not viewer_id or self.is_triview():
+            warning = 'viewer_id unnecessary and ignored in triview mode' if self.is_triview() and viewer_id else None
+            viewer_id = FireflyClient.PINNED_IMAGE_VIEWER_ID
 
         payload = {'fovDegFallOver': fov_deg_fallover, 'plotAllSkyFirst': plot_allsky_first,
                    'plotId': plot_id, 'viewerId': viewer_id}
 
         pg_key = 'plotGroupId'
         if not ((hips_request and hips_request.get(pg_key)) or (image_request and image_request.get(pg_key))):
             if hips_request:
@@ -1252,15 +1371,17 @@
             elif image_request:
                 image_request.update({pg_key: 'groupFromPython'})
 
         image_request and payload.update({'imageRequest': image_request})
         hips_request and payload.update({'hipsRequest': hips_request})
         allsky_request and payload.update({'allSkyRequest': allsky_request})
 
-        return self.dispatch(ACTION_DICT['ShowImageOrHiPS'], payload)
+        r = self.dispatch(ACTION_DICT['ShowImageOrHiPS'], payload)
+        warning and r.update({'warning': warning})
+        return r
 
     # ----------------------------
     # actions on image
     # ----------------------------
 
     def set_zoom(self, plot_id, factor=1.0):
         """
```

### Comparing `firefly_client-2.9.0/firefly_client/plot.py` & `firefly_client-3.0.0/firefly_client/plot.py`

 * *Files identical despite different names*

### Comparing `firefly_client-2.9.0/firefly_client/range_values.py` & `firefly_client-3.0.0/firefly_client/range_values.py`

 * *Files identical despite different names*

### Comparing `firefly_client-2.9.0/setup.py` & `firefly_client-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Licensed under a 3-clause BSD style license - see License.txt
 
 from setuptools import setup
 
 setup(
     name='firefly_client',
-    version='2.9.0',
+    version='3.0.0',
     description='Python API for Firefly',
     author='IPAC LSST SUIT',
     license='BSD',
     url='http://github.com/Caltech-IPAC/firefly_client',
     packages=['firefly_client'],
     install_requires=['websocket-client', 'requests'],
     classifiers=[
```

### Comparing `firefly_client-2.9.0/test/test-5-instances-3-channels.py` & `firefly_client-3.0.0/test/test-5-instances-3-channels.py`

 * *Files identical despite different names*

### Comparing `firefly_client-2.9.0/test/test-simple-callback-response.py` & `firefly_client-3.0.0/test/test-simple-callback-response.py`

 * *Files identical despite different names*

