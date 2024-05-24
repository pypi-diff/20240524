# Comparing `tmp/dash_websocket_component-0.0.7.tar.gz` & `tmp/dash_websocket_component-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_websocket_component-0.0.7.tar", last modified: Tue Apr 30 11:46:12 2024, max compression
+gzip compressed data, was "dash_websocket_component-1.0.0.tar", last modified: Fri May 24 10:41:22 2024, max compression
```

## Comparing `dash_websocket_component-0.0.7.tar` & `dash_websocket_component-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 11:46:12.478563 dash_websocket_component-0.0.7/
--rw-rw-rw-   0        0        0        0 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      484 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4137 2024-04-30 11:46:12.477563 dash_websocket_component-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3837 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 11:46:12.462561 dash_websocket_component-0.0.7/dash_websocket_component/
--rw-rw-rw-   0        0        0     2109 2024-04-30 11:46:08.000000 dash_websocket_component-0.0.7/dash_websocket_component/DashWebsocketComponent.py
--rw-rw-rw-   0        0        0     2389 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.7/dash_websocket_component/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-30 11:46:08.000000 dash_websocket_component-0.0.7/dash_websocket_component/_imports_.py
--rw-rw-rw-   0        0        0     4947 2024-04-30 11:46:06.000000 dash_websocket_component-0.0.7/dash_websocket_component/async-DashWebsocketComponent.js
--rw-rw-rw-   0        0        0     7418 2024-04-30 11:46:06.000000 dash_websocket_component-0.0.7/dash_websocket_component/async-DashWebsocketComponent.js.map
--rw-rw-rw-   0        0        0     4113 2024-04-30 11:46:06.000000 dash_websocket_component-0.0.7/dash_websocket_component/dash_websocket_component.min.js
--rw-rw-rw-   0        0        0    20188 2024-04-30 11:46:06.000000 dash_websocket_component-0.0.7/dash_websocket_component/dash_websocket_component.min.js.map
--rw-rw-rw-   0        0        0     2747 2024-04-30 11:46:08.000000 dash_websocket_component-0.0.7/dash_websocket_component/metadata.json
--rw-rw-rw-   0        0        0     2118 2024-04-30 11:46:08.000000 dash_websocket_component-0.0.7/dash_websocket_component/package-info.json
-drwxrwxrwx   0        0        0        0 2024-04-30 11:46:12.473562 dash_websocket_component-0.0.7/dash_websocket_component.egg-info/
--rw-rw-rw-   0        0        0     4137 2024-04-30 11:46:12.000000 dash_websocket_component-0.0.7/dash_websocket_component.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-04-30 11:46:12.000000 dash_websocket_component-0.0.7/dash_websocket_component.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 11:46:12.000000 dash_websocket_component-0.0.7/dash_websocket_component.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-30 11:46:12.000000 dash_websocket_component-0.0.7/dash_websocket_component.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2118 2024-04-30 11:46:00.000000 dash_websocket_component-0.0.7/package.json
--rw-rw-rw-   0        0        0       42 2024-04-30 11:46:12.479565 dash_websocket_component-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      721 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 11:46:12.475562 dash_websocket_component-0.0.7/tests/
--rw-rw-rw-   0        0        0      945 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.7/tests/test_usage.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:41:22.977751 dash_websocket_component-1.0.0/
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:35:19.000000 dash_websocket_component-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      484 2024-02-23 09:35:19.000000 dash_websocket_component-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4094 2024-05-24 10:41:22.975750 dash_websocket_component-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3837 2024-02-23 09:35:19.000000 dash_websocket_component-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 10:41:22.956748 dash_websocket_component-1.0.0/dash_websocket_component/
+-rw-rw-rw-   0        0        0     2517 2024-05-24 10:41:20.000000 dash_websocket_component-1.0.0/dash_websocket_component/DashWebsocketComponent.py
+-rw-rw-rw-   0        0        0     2389 2024-02-23 09:35:19.000000 dash_websocket_component-1.0.0/dash_websocket_component/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-05-24 10:41:20.000000 dash_websocket_component-1.0.0/dash_websocket_component/_imports_.py
+-rw-rw-rw-   0        0        0     4659 2024-05-24 10:38:26.000000 dash_websocket_component-1.0.0/dash_websocket_component/async-DashWebsocketComponent.js
+-rw-rw-rw-   0        0        0     8741 2024-05-24 10:38:26.000000 dash_websocket_component-1.0.0/dash_websocket_component/async-DashWebsocketComponent.js.map
+-rw-rw-rw-   0        0        0     4176 2024-05-24 10:41:17.000000 dash_websocket_component-1.0.0/dash_websocket_component/dash_websocket_component.min.js
+-rw-rw-rw-   0        0        0    20575 2024-05-24 10:41:17.000000 dash_websocket_component-1.0.0/dash_websocket_component/dash_websocket_component.min.js.map
+-rw-rw-rw-   0        0        0     3188 2024-05-24 10:41:20.000000 dash_websocket_component-1.0.0/dash_websocket_component/metadata.json
+-rw-rw-rw-   0        0        0     2118 2024-05-24 10:41:19.000000 dash_websocket_component-1.0.0/dash_websocket_component/package-info.json
+drwxrwxrwx   0        0        0        0 2024-05-24 10:41:22.973749 dash_websocket_component-1.0.0/dash_websocket_component.egg-info/
+-rw-rw-rw-   0        0        0     4094 2024-05-24 10:41:22.000000 dash_websocket_component-1.0.0/dash_websocket_component.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-05-24 10:41:22.000000 dash_websocket_component-1.0.0/dash_websocket_component.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 10:41:22.000000 dash_websocket_component-1.0.0/dash_websocket_component.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-24 10:41:22.000000 dash_websocket_component-1.0.0/dash_websocket_component.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2118 2024-05-23 11:33:30.000000 dash_websocket_component-1.0.0/package.json
+-rw-rw-rw-   0        0        0       42 2024-05-24 10:41:22.978751 dash_websocket_component-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-02-23 09:35:19.000000 dash_websocket_component-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:41:22.970752 dash_websocket_component-1.0.0/tests/
+-rw-rw-rw-   0        0        0      945 2024-02-23 09:35:19.000000 dash_websocket_component-1.0.0/tests/test_usage.py
```

### Comparing `dash_websocket_component-0.0.7/PKG-INFO` & `dash_websocket_component-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: dash_websocket_component
-Version: 0.0.7
+Version: 1.0.0
 Summary: Project Description
-Home-page: UNKNOWN
 Author: Dominik Tkacik <tkacik38@gmail.com>
 License: MIT
-Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dash WebSocket Component
 
 Dash WebSocket Component is a Dash component library.
@@ -104,9 +102,7 @@
         ```
         _Publishing your component to NPM will make the JavaScript bundles available on the unpkg CDN. By default, Dash serves the component library's CSS and JS locally, but if you choose to publish the package to NPM you can set `serve_locally` to `False` and you may see faster load times._
 
 5. Share your component with the community! https://community.plotly.com/c/dash
     1. Publish this repository to GitHub
     2. Tag your GitHub repository with the plotly-dash tag so that it appears here: https://github.com/topics/plotly-dash
     3. Create a post in the Dash community forum: https://community.plotly.com/c/dash
-
-
```

### Comparing `dash_websocket_component-0.0.7/README.md` & `dash_websocket_component-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component/DashWebsocketComponent.py` & `dash_websocket_component-1.0.0/dash_websocket_component/DashWebsocketComponent.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,39 +15,45 @@
 
 - id (string; optional):
     The ID used to identify this component in Dash callbacks.
 
 - error (dict | string; optional):
     This property is set with the content of the onerror event.
 
+- maxReconnectAttempts (number; optional):
+    Max count of the reconnect attempts. Default = -1 -> Unlimited.
+
 - message (dict | string; optional):
     When messages are received, this property is updated with the
     message content.
 
 - protocols (list of strings; optional):
     Supported websocket protocols (optional).
 
+- reconnectIntervalMs (number; optional):
+    Duration between attempts to reconnect. Default = 2000ms -> 2sec.
+
 - send (dict | string; optional):
     When this property is set, a message is sent with its content.
 
 - state (dict | string; optional):
     This websocket state (in the readyState prop) and associated
     information.
 
 - url (string; optional):
     The websocket endpoint (e.g. wss://echo.websocket.org)."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_websocket_component'
     _type = 'DashWebsocketComponent'
     @_explicitize_args
-    def __init__(self, state=Component.UNDEFINED, message=Component.UNDEFINED, error=Component.UNDEFINED, send=Component.UNDEFINED, url=Component.UNDEFINED, protocols=Component.UNDEFINED, id=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'error', 'message', 'protocols', 'send', 'state', 'url']
+    def __init__(self, state=Component.UNDEFINED, message=Component.UNDEFINED, error=Component.UNDEFINED, send=Component.UNDEFINED, protocols=Component.UNDEFINED, reconnectIntervalMs=Component.UNDEFINED, maxReconnectAttempts=Component.UNDEFINED, url=Component.UNDEFINED, id=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'error', 'maxReconnectAttempts', 'message', 'protocols', 'reconnectIntervalMs', 'send', 'state', 'url']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'error', 'message', 'protocols', 'send', 'state', 'url']
+        self.available_properties = ['id', 'error', 'maxReconnectAttempts', 'message', 'protocols', 'reconnectIntervalMs', 'send', 'state', 'url']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(DashWebsocketComponent, self).__init__(**args)
```

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component/__init__.py` & `dash_websocket_component-1.0.0/dash_websocket_component/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component/async-DashWebsocketComponent.js` & `dash_websocket_component-1.0.0/dash_websocket_component/async-DashWebsocketComponent.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,220 +1,194 @@
 "use strict";
 (self.webpackChunkdash_websocket_component = self.webpackChunkdash_websocket_component || []).push([
     [12], {
         368: (t, e, n) => {
             n.r(e), n.d(e, {
-                default: () => m
+                default: () => b
             });
             var o = n(609),
                 r = n(120),
-                i = n.n(r);
+                c = n.n(r);
 
-            function c(t) {
-                return c = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+            function s(t) {
+                return s = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
                     return typeof t
                 } : function(t) {
                     return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
-                }, c(t)
+                }, s(t)
             }
 
-            function s(t, e) {
-                var n = Object.keys(t);
-                if (Object.getOwnPropertySymbols) {
-                    var o = Object.getOwnPropertySymbols(t);
-                    e && (o = o.filter((function(e) {
-                        return Object.getOwnPropertyDescriptor(t, e).enumerable
-                    }))), n.push.apply(n, o)
-                }
-                return n
-            }
-
-            function u(t) {
-                for (var e = 1; e < arguments.length; e++) {
-                    var n = null != arguments[e] ? arguments[e] : {};
-                    e % 2 ? s(Object(n), !0).forEach((function(e) {
-                        var o, r, i;
-                        o = t, r = e, i = n[e], (r = p(r)) in o ? Object.defineProperty(o, r, {
-                            value: i,
-                            enumerable: !0,
-                            configurable: !0,
-                            writable: !0
-                        }) : o[r] = i
-                    })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : s(Object(n)).forEach((function(e) {
-                        Object.defineProperty(t, e, Object.getOwnPropertyDescriptor(n, e))
-                    }))
-                }
-                return t
-            }
-
-            function a(t, e) {
+            function i(t, e) {
                 for (var n = 0; n < e.length; n++) {
                     var o = e[n];
-                    o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(t, p(o.key), o)
+                    o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(t, u(o.key), o)
                 }
             }
 
-            function p(t) {
+            function u(t) {
                 var e = function(t, e) {
-                    if ("object" != c(t) || !t) return t;
+                    if ("object" != s(t) || !t) return t;
                     var n = t[Symbol.toPrimitive];
                     if (void 0 !== n) {
                         var o = n.call(t, "string");
-                        if ("object" != c(o)) return o;
+                        if ("object" != s(o)) return o;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }
                     return String(t)
                 }(t);
-                return "symbol" == c(e) ? e : String(e)
+                return "symbol" == s(e) ? e : String(e)
             }
 
-            function l(t, e, n) {
-                return e = y(e),
+            function a(t, e, n) {
+                return e = l(e),
                     function(t, e) {
-                        if (e && ("object" === c(e) || "function" == typeof e)) return e;
+                        if (e && ("object" === s(e) || "function" == typeof e)) return e;
                         if (void 0 !== e) throw new TypeError("Derived constructors may only return object or undefined");
                         return function(t) {
                             if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return t
                         }(t)
-                    }(t, f() ? Reflect.construct(e, n || [], y(t).constructor) : e.apply(t, n))
+                    }(t, p() ? Reflect.construct(e, n || [], l(t).constructor) : e.apply(t, n))
             }
 
-            function f() {
+            function p() {
                 try {
                     var t = !Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {})))
                 } catch (t) {}
-                return (f = function() {
+                return (p = function() {
                     return !!t
                 })()
             }
 
-            function y(t) {
-                return y = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
+            function l(t) {
+                return l = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
                     return t.__proto__ || Object.getPrototypeOf(t)
-                }, y(t)
+                }, l(t)
             }
 
-            function b(t, e) {
-                return b = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(t, e) {
+            function f(t, e) {
+                return f = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(t, e) {
                     return t.__proto__ = e, t
-                }, b(t, e)
+                }, f(t, e)
             }
-            var m = function(t) {
-                function e() {
+            var b = function(t) {
+                function e(t) {
+                    var n;
                     return function(t, e) {
                         if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
-                    }(this, e), l(this, e, arguments)
+                    }(this, e), (n = a(this, e, [t])).state = {
+                        isConnected: !1,
+                        reconnectAttempts: 0
+                    }, n
                 }
                 var n, o;
                 return function(t, e) {
                     if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function");
                     t.prototype = Object.create(e && e.prototype, {
                         constructor: {
                             value: t,
                             writable: !0,
                             configurable: !0
                         }
                     }), Object.defineProperty(t, "prototype", {
                         writable: !1
-                    }), e && b(t, e)
-                }(e, t), n = e, o = [{
-                    key: "_init_client",
+                    }), e && f(t, e)
+                }(e, t), n = e, (o = [{
+                    key: "componentDidMount",
+                    value: function() {
+                        this.props.url && this.connectWebSocket()
+                    }
+                }, {
+                    key: "componentDidUpdate",
                     value: function(t) {
-                        function e() {
-                            return t.apply(this, arguments)
+                        var e = this.props,
+                            n = e.send,
+                            o = e.url;
+                        if (null == this.ws) {
+                            if (null == o) return;
+                            this.connectWebSocket()
                         }
-                        return e.toString = function() {
-                            return t.toString()
-                        }, e
-                    }((function() {
+                        n && n !== t.send && (this.ws.readyState === WebSocket.OPEN ? this.ws.send(n) : console.error("Trying to send data -> ".concat(n, " over closed websocket connection.")))
+                    }
+                }, {
+                    key: "componentWillUnmount",
+                    value: function() {
+                        this.disconnectWebSocket()
+                    }
+                }, {
+                    key: "attemptReconnect",
+                    value: function() {
+                        var t = this; - 1 === this.props.maxReconnectAttempts || this.state.reconnectAttempts < this.props.maxReconnectAttempts ? setTimeout((function() {
+                            t.setState({
+                                reconnectAttempts: t.state.reconnectAttempts += 1
+                            });
+                            var e = -1 == t.props.maxReconnectAttempts ? "Unlimited" : t.props.maxReconnectAttempts;
+                            console.log("Attempting to reconnect... Attempt (".concat(t.state.reconnectAttempts, "/").concat(e, ")")), t.connectWebSocket()
+                        }), this.props.reconnectIntervalMs) : console.error("Max reconnect attempts reached.")
+                    }
+                }, {
+                    key: "connectWebSocket",
+                    value: function() {
                         var t = this,
-                            e = this.props.url,
-                            n = this.props.protocols;
-                        e = e || "ws://" + location.host + location.pathname + "ws", this.client = new WebSocket(e, n), this.client.onopen = function(e) {
-                            t.props.setProps({
-                                state: {
-                                    readyState: WebSocket.OPEN,
-                                    isTrusted: e.isTrusted,
-                                    timeStamp: e.timeStamp,
-                                    origin: e.origin,
-                                    lastConnected: Number(new Date)
-                                }
+                            e = this.props,
+                            n = e.url,
+                            o = e.protocols;
+                        this.ws = new WebSocket(n, o), this.ws.onopen = function() {
+                            console.log("WebSocket connected"), t.setState({
+                                isConnected: !0,
+                                reconnectAttempts: 0
                             })
-                        }, this.client.onmessage = function(e) {
+                        }, this.ws.onmessage = function(e) {
                             t.props.setProps({
-                                state: u(u({}, t.props.state), {}, {
-                                    lastConnected: Number(new Date)
-                                }),
                                 message: {
                                     data: e.data,
                                     isTrusted: e.isTrusted,
                                     origin: e.origin,
                                     timeStamp: e.timeStamp
                                 }
                             })
-                        }, this.client.onerror = function(e) {
-                            console.log("ON ERROR ".concat(location.host)), t.props.setProps({
+                        }, this.ws.onclose = function() {
+                            console.log("WebSocket disconnected"), t.setState({
+                                isConnected: !1
+                            }), t.disconnectWebSocket(), t.attemptReconnect()
+                        }, this.ws.onerror = function(e) {
+                            var n;
+                            t.props.setProps({
                                 error: JSON.stringify(e)
-                            })
-                        }, this.client.onclose = function(e) {
-                            console.log("ON CLOSE ".concat(location.host)), t.props.setProps({
-                                error: JSON.stringify(e),
-                                state: {
-                                    readyState: WebSocket.CLOSED,
-                                    isTrusted: e.isTrusted,
-                                    timeStamp: e.timeStamp,
-                                    code: e.code,
-                                    reason: e.reason,
-                                    wasClean: e.wasClean,
-                                    lastConnected: Number(new Date)
-                                }
-                            }), setTimeout(_init_client, 1e3)
+                            }), (null === (n = t.ws) || void 0 === n ? void 0 : n.readyState) == WebSocket.OPEN && t.ws.close()
                         }
-                    }))
-                }, {
-                    key: "componentDidMount",
-                    value: function() {
-                        console.log("Try to load web socket component"), this.props.setProps({
-                            state: u(u({}, this.props.state), {}, {
-                                lastConnected: 0
-                            })
-                        }), this._init_client()
-                    }
-                }, {
-                    key: "componentDidUpdate",
-                    value: function(t) {
-                        var e = this.props.send;
-                        e && e !== t.send && this.props.state.readyState === WebSocket.OPEN && this.client.send(e)
                     }
                 }, {
-                    key: "componentWillUnmount",
+                    key: "disconnectWebSocket",
                     value: function() {
-                        this.client.onopen = null, this.client.onclose = null, this.client.onerror = null, this.client.onmessage = null, this.client.close()
+                        var t, e;
+                        (null === (t = this.ws) || void 0 === t ? void 0 : t.readyState) != WebSocket.OPEN && (null === (e = this.ws) || void 0 === e ? void 0 : e.readyState) != WebSocket.CONNECTING || (this.ws.close(), delete this.ws)
                     }
                 }, {
                     key: "render",
                     value: function() {
                         return null
                     }
-                }], o && a(n.prototype, o), Object.defineProperty(n, "prototype", {
+                }]) && i(n.prototype, o), Object.defineProperty(n, "prototype", {
                     writable: !1
                 }), e
             }(o.Component);
-            m.defaultProps = {
-                state: {
-                    readyState: WebSocket.CONNECTING
-                }
-            }, m.propTypes = {
-                state: i().oneOfType([i().object, i().string]),
-                message: i().oneOfType([i().object, i().string]),
-                error: i().oneOfType([i().object, i().string]),
-                send: i().oneOfType([i().object, i().string]),
-                url: i().string,
-                protocols: i().arrayOf(i().string),
-                id: i().string,
-                setProps: i().func
+            b.defaultProps = {
+                state: {},
+                maxReconnectAttempts: -1,
+                reconnectIntervalMs: 2e3
+            }, b.propTypes = {
+                state: c().oneOfType([c().object, c().string]),
+                message: c().oneOfType([c().object, c().string]),
+                error: c().oneOfType([c().object, c().string]),
+                send: c().oneOfType([c().object, c().string]),
+                protocols: c().arrayOf(c().string),
+                reconnectIntervalMs: c().number,
+                maxReconnectAttempts: c().number,
+                url: c().string,
+                id: c().string,
+                setProps: c().func
             }
         }
     }
 ]);
 //# sourceMappingURL=async-DashWebsocketComponent.js.map
```

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component/dash_websocket_component.min.js` & `dash_websocket_component-1.0.0/dash_websocket_component/dash_websocket_component.min.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -95,15 +95,15 @@
         var a = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var t, r = (t = s(), /\/_dash-component-suites\//.test(t.src)),
                 n = a(e);
             if (!r) return n;
             var o = n.split("/"),
                 i = o.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_0_7m1714477566"), o.splice(-1, 1, i.join(".")), o.join("/")
+            return i.splice(1, 0, "v1_0_0m1716547278"), o.splice(-1, 1, i.join(".")), o.join("/")
         }
     }(() => {
         var e = {
             792: 0
         };
         o.f.j = (t, r) => {
             var n = o.o(e, t) ? e[t] : void 0;
@@ -153,16 +153,18 @@
                 }, t().createElement(i, e))
             };
         s.defaultProps = {}, s.propTypes = {
             state: n().oneOfType([n().object, n().string]),
             message: n().oneOfType([n().object, n().string]),
             error: n().oneOfType([n().object, n().string]),
             send: n().oneOfType([n().object, n().string]),
-            url: n().string,
             protocols: n().arrayOf(n().string),
+            reconnectIntervalMs: n().number,
+            maxReconnectAttempts: n().number,
+            url: n().string,
             id: n().string,
             setProps: n().func
         };
         const a = s
     })(), window.dash_websocket_component = c
 })();
 //# sourceMappingURL=dash_websocket_component.min.js.map
```

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component/dash_websocket_component.min.js.map` & `dash_websocket_component-1.0.0/dash_websocket_component/dash_websocket_component.min.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9116923764811089%*

 * *Differences: {"'mappings'": "'uBAAIA,EACAC,E,WCDJC,EAAOC,QAAUC,OAAkB,S,UCAnCF,EAAOC,QAAUC,OAAc,K,GCC3BC,EAA2B,CAAC,EAGhC,SAASC,EAAoBC,GAE5B,IAAIC,EAAeH,EAAyBE,GAC5C,QAAqBE,IAAjBD,EACH,OAAOA,EAAaL,QAGrB,IAAID,EAASG,EAAyBE,GAAY,CAGjDJ,QAAS,CAAC,GAOX,OAHAO,EAAoBH,GAAUL,EAAQA,EAAOC,QAASG,GAG/CJ,EAAOC,OACf,CAGAG,EAAoBK,EAAID,ECxBxBJ,EAAoBM,EAAKV,IACxB,IAAIW,EAASX,GAAUA,EAAOY,WAC7B,IAAOZ,EAAiB,QACxB,IAAM,EAEP,OADAI,EAAoBS,EAAEF,EAAQ,CAAEG,EAAGH,IAC5BA,CAAM,ECLdP,EAAoBS,EAAI,CAACZ,EAASc,KACjC,IAAI,IAAIC,KAAOD,EACXX,EAAoBa,EAAE […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_websocket_component.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "inProgress",
         "dataWebpackPrefix",
         "module",
         "exports",
         "window",
         "__webpack_module_cache__",
@@ -137,14 +137,16 @@
         "RealComponent",
         "defaultProps",
         "propTypes",
         "state",
         "PropTypes",
         "send",
         "protocols",
+        "reconnectIntervalMs",
+        "maxReconnectAttempts",
         "setProps"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///webpack/runtime/load script",
         "webpack:///external window \"PropTypes\"",
         "webpack:///external window \"React\"",
@@ -171,14 +173,14 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + \"async-DashWebsocketComponent\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_7m1714477566\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v1_0_0m1716547278\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t792: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkdash_websocket_component\"] = self[\"webpackChunkdash_websocket_component\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "export const DashWebsocketComponent = React.lazy(() =>\r\n    import(\r\n        /* webpackChunkName: \"DashWebsocketComponent\" */ './fragments/DashWebsocketComponent.react'\r\n    )\r\n);\r\n",
-        "import React from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport {DashWebsocketComponent as RealComponent} from '../LazyLoader';\r\n\r\n/**\r\n * ExampleComponent is an example component.\r\n * It takes a property, `label`, and\r\n * displays it.\r\n * It renders an input with the property `value`\r\n * which is editable by the user.\r\n */\r\nconst DashWebsocketComponent = (props) => {\r\n    return (\r\n        <React.Suspense fallback={null}>\r\n            <RealComponent {...props} />\r\n        </React.Suspense>\r\n    );\r\n};\r\n\r\nDashWebsocketComponent.defaultProps = {};\r\n\r\nDashWebsocketComponent.propTypes = {\r\n    /**\r\n     * This websocket state (in the readyState prop) and associated information.\r\n     */\r\n    state: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When messages are received, this property is updated with the message content.\r\n     */\r\n    message: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * This property is set with the content of the onerror event.\r\n     */\r\n    error: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When this property is set, a message is sent with its content.\r\n     */\r\n    send: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * The websocket endpoint (e.g. wss://echo.websocket.org).\r\n     */\r\n    url: PropTypes.string,\r\n\r\n    /**\r\n     * Supported websocket protocols (optional).\r\n     */\r\n    protocols: PropTypes.arrayOf(PropTypes.string),\r\n\r\n    /**\r\n     * The ID used to identify this component in Dash callbacks.\r\n     */\r\n    id: PropTypes.string,\r\n\r\n    /**\r\n     * Dash-assigned callback that should be called to report property changes\r\n     * to Dash, to make them available for callbacks.\r\n     */\r\n    setProps: PropTypes.func,\r\n};\r\n\r\nexport default DashWebsocketComponent;\r\n\r\nexport const defaultProps = DashWebsocketComponent.defaultProps;\r\nexport const propTypes = DashWebsocketComponent.propTypes;\r\n"
+        "import React from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport {DashWebsocketComponent as RealComponent} from '../LazyLoader';\r\n\r\n/**\r\n * ExampleComponent is an example component.\r\n * It takes a property, `label`, and\r\n * displays it.\r\n * It renders an input with the property `value`\r\n * which is editable by the user.\r\n */\r\nconst DashWebsocketComponent = (props) => {\r\n    return (\r\n        <React.Suspense fallback={null}>\r\n            <RealComponent {...props} />\r\n        </React.Suspense>\r\n    );\r\n};\r\n\r\nDashWebsocketComponent.defaultProps = {};\r\n\r\nDashWebsocketComponent.propTypes = {\r\n    /**\r\n     * This websocket state (in the readyState prop) and associated information.\r\n     */\r\n    state: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When messages are received, this property is updated with the message content.\r\n     */\r\n    message: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * This property is set with the content of the onerror event.\r\n     */\r\n    error: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When this property is set, a message is sent with its content.\r\n     */\r\n    send: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * Supported websocket protocols (optional).\r\n     */\r\n    protocols: PropTypes.arrayOf(PropTypes.string),\r\n\r\n    /**\r\n     * Duration between attempts to reconnect. Default = 2000ms -> 2sec.\r\n     */\r\n    reconnectIntervalMs: PropTypes.number,\r\n    \r\n    /**\r\n     * Max count of the reconnect attempts. Default = -1 -> Unlimited. \r\n     */\r\n    maxReconnectAttempts: PropTypes.number,\r\n\r\n    /**\r\n     * The websocket endpoint (e.g. wss://echo.websocket.org).\r\n     */\r\n    url: PropTypes.string,\r\n\r\n    /**\r\n     * The ID used to identify this component in Dash callbacks.\r\n     */\r\n    id: PropTypes.string,\r\n\r\n    /**\r\n     * Dash-assigned callback that should be called to report property changes\r\n     * to Dash, to make them available for callbacks.\r\n     */\r\n    setProps: PropTypes.func,\r\n};\r\n\r\nexport default DashWebsocketComponent;\r\n\r\nexport const defaultProps = DashWebsocketComponent.defaultProps;\r\nexport const propTypes = DashWebsocketComponent.propTypes;\r\n"
     ],
     "version": 3
 }
```

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component/metadata.json` & `dash_websocket_component-1.0.0/dash_websocket_component/metadata.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'src/lib/components/DashWebsocketComponent.react.js'": "{'props': {'reconnectIntervalMs': "*

 * *                                                         "OrderedDict([('type', "*

 * *                                                         "OrderedDict([('name', 'number')])), "*

 * *                                                         "('required', False), ('description', "*

 * *                                                         "'Duration between attempts to reconnect. "*

 * *                                           […]*

```diff
@@ -22,14 +22,21 @@
             "id": {
                 "description": "The ID used to identify this component in Dash callbacks.",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
+            "maxReconnectAttempts": {
+                "description": "Max count of the reconnect attempts. Default = -1 -> Unlimited.",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
             "message": {
                 "description": "When messages are received, this property is updated with the message content.",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
@@ -47,14 +54,21 @@
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "string"
                     }
                 }
             },
+            "reconnectIntervalMs": {
+                "description": "Duration between attempts to reconnect. Default = 2000ms -> 2sec.",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
             "send": {
                 "description": "When this property is set, a message is sent with its content.",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
```

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component/package-info.json` & `dash_websocket_component-1.0.0/dash_websocket_component/package-info.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.0.0'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_websocket_component -p package-info.json --r-prefix 'dwc' --jl-prefix 'dwc' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.7"
+    "version": "1.0.0"
 }
```

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component.egg-info/PKG-INFO` & `dash_websocket_component-1.0.0/dash_websocket_component.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: dash-websocket-component
-Version: 0.0.7
+Version: 1.0.0
 Summary: Project Description
-Home-page: UNKNOWN
 Author: Dominik Tkacik <tkacik38@gmail.com>
 License: MIT
-Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dash WebSocket Component
 
 Dash WebSocket Component is a Dash component library.
@@ -104,9 +102,7 @@
         ```
         _Publishing your component to NPM will make the JavaScript bundles available on the unpkg CDN. By default, Dash serves the component library's CSS and JS locally, but if you choose to publish the package to NPM you can set `serve_locally` to `False` and you may see faster load times._
 
 5. Share your component with the community! https://community.plotly.com/c/dash
     1. Publish this repository to GitHub
     2. Tag your GitHub repository with the plotly-dash tag so that it appears here: https://github.com/topics/plotly-dash
     3. Create a post in the Dash community forum: https://community.plotly.com/c/dash
-
-
```

### Comparing `dash_websocket_component-0.0.7/dash_websocket_component.egg-info/SOURCES.txt` & `dash_websocket_component-1.0.0/dash_websocket_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.7/package.json` & `dash_websocket_component-1.0.0/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.0.0'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_websocket_component -p package-info.json --r-prefix 'dwc' --jl-prefix 'dwc' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.7"
+    "version": "1.0.0"
 }
```

### Comparing `dash_websocket_component-0.0.7/setup.py` & `dash_websocket_component-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.7/tests/test_usage.py` & `dash_websocket_component-1.0.0/tests/test_usage.py`

 * *Files identical despite different names*

