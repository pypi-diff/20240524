# Comparing `tmp/gradio_clickabletextbox-0.0.3.tar.gz` & `tmp/gradio_clickabletextbox-0.0.4.tar.gz`

## Comparing `gradio_clickabletextbox-0.0.3.tar` & `gradio_clickabletextbox-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/__init__.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.py
--rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.pyi
--rw-r--r--   0        0        0    97610 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/index.js
--rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/css.css
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/requirements.txt
--rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/Example.svelte
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/Index.svelte
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/gradio.config.js
--rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/package-lock.json
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/package.json
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/shared/Textbox.svelte
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/shared/transitions.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/.gitignore
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/README.md
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/__init__.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/clickabletextbox.py
+-rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/clickabletextbox.pyi
+-rw-r--r--   0        0        0    97402 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/templates/component/index.js
+-rw-r--r--   0        0        0    16061 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/demo/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/demo/app.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/demo/app2.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/demo/css.css
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/demo/requirements.txt
+-rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/frontend/Example.svelte
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/frontend/Index.svelte
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/frontend/gradio.config.js
+-rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/frontend/package-lock.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/frontend/package.json
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/frontend/shared/Textbox.svelte
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/frontend/shared/transitions.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/.gitignore
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/README.md
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.4/PKG-INFO
```

### Comparing `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.py` & `gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/clickabletextbox.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.pyi` & `gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/clickabletextbox.pyi`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/index.js` & `gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/templates/component/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
 const {
-    SvelteComponent: Sl,
-    assign: zl,
-    create_slot: El,
-    detach: Tl,
-    element: Bl,
-    get_all_dirty_from_scope: Nl,
-    get_slot_changes: Dl,
-    get_spread_update: Il,
-    init: jl,
-    insert: Al,
-    safe_not_equal: Pl,
-    set_dynamic_element_data: Mt,
+    SvelteComponent: Zl,
+    assign: Sl,
+    create_slot: zl,
+    detach: El,
+    element: Tl,
+    get_all_dirty_from_scope: Bl,
+    get_slot_changes: Nl,
+    get_spread_update: Dl,
+    init: Il,
+    insert: jl,
+    safe_not_equal: Al,
+    set_dynamic_element_data: Lt,
     set_style: K,
-    toggle_class: ie,
-    transition_in: dl,
-    transition_out: ml,
-    update_slot_base: Yl
+    toggle_class: se,
+    transition_in: cl,
+    transition_out: dl,
+    update_slot_base: Pl
 } = window.__gradio__svelte__internal;
 
-function Kl(l) {
+function Yl(l) {
     let e, t, n;
     const s = (
             /*#slots*/
             l[18].default
         ),
-        o = El(
+        f = zl(
             s,
             l,
             /*$$scope*/
             l[17],
             null
         );
     let i = [{
@@ -41,46 +41,46 @@
                 /*elem_id*/
                 l[2]
             )
         }, {
             class: t = "block " + /*elem_classes*/
                 l[3].join(" ") + " svelte-nl1om8"
         }],
-        f = {};
-    for (let r = 0; r < i.length; r += 1)
-        f = zl(f, i[r]);
+        o = {};
+    for (let u = 0; u < i.length; u += 1)
+        o = Sl(o, i[u]);
     return {
         c() {
-            e = Bl(
+            e = Tl(
                 /*tag*/
                 l[14]
-            ), o && o.c(), Mt(
+            ), f && f.c(), Lt(
                 /*tag*/
                 l[14]
-            )(e, f), ie(
+            )(e, o), se(
                 e,
                 "hidden",
                 /*visible*/
                 l[10] === !1
-            ), ie(
+            ), se(
                 e,
                 "padded",
                 /*padding*/
                 l[6]
-            ), ie(
+            ), se(
                 e,
                 "border_focus",
                 /*border_mode*/
                 l[5] === "focus"
-            ), ie(
+            ), se(
                 e,
                 "border_contrast",
                 /*border_mode*/
                 l[5] === "contrast"
-            ), ie(e, "hide-container", ! /*explicit_call*/
+            ), se(e, "hide-container", ! /*explicit_call*/
                 l[8] && ! /*container*/
                 l[9]), K(
                 e,
                 "height",
                 /*get_dimension*/
                 l[15](
                     /*height*/
@@ -107,230 +107,230 @@
                 e,
                 "flex-grow",
                 /*scale*/
                 l[12]
             ), K(e, "min-width", `calc(min(${/*min_width*/
       l[13]}px, 100%))`), K(e, "border-width", "var(--block-border-width)");
         },
-        m(r, a) {
-            Al(r, e, a), o && o.m(e, null), n = !0;
+        m(u, a) {
+            jl(u, e, a), f && f.m(e, null), n = !0;
         },
-        p(r, a) {
-            o && o.p && (!n || a & /*$$scope*/
-                    131072) && Yl(
-                    o,
+        p(u, a) {
+            f && f.p && (!n || a & /*$$scope*/
+                    131072) && Pl(
+                    f,
                     s,
-                    r,
+                    u,
                     /*$$scope*/
-                    r[17],
-                    n ? Dl(
+                    u[17],
+                    n ? Nl(
                         s,
                         /*$$scope*/
-                        r[17],
+                        u[17],
                         a,
                         null
-                    ) : Nl(
+                    ) : Bl(
                         /*$$scope*/
-                        r[17]
+                        u[17]
                     ),
                     null
-                ), Mt(
+                ), Lt(
                     /*tag*/
-                    r[14]
-                )(e, f = Il(i, [
+                    u[14]
+                )(e, o = Dl(i, [
                     (!n || a & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
-                            r[7]
+                            u[7]
                         )
                     },
                     (!n || a & /*elem_id*/
                         4) && {
                         id: (
                             /*elem_id*/
-                            r[2]
+                            u[2]
                         )
                     },
                     (!n || a & /*elem_classes*/
                         8 && t !== (t = "block " + /*elem_classes*/
-                            r[3].join(" ") + " svelte-nl1om8")) && {
+                            u[3].join(" ") + " svelte-nl1om8")) && {
                         class: t
                     }
-                ])), ie(
+                ])), se(
                     e,
                     "hidden",
                     /*visible*/
-                    r[10] === !1
-                ), ie(
+                    u[10] === !1
+                ), se(
                     e,
                     "padded",
                     /*padding*/
-                    r[6]
-                ), ie(
+                    u[6]
+                ), se(
                     e,
                     "border_focus",
                     /*border_mode*/
-                    r[5] === "focus"
-                ), ie(
+                    u[5] === "focus"
+                ), se(
                     e,
                     "border_contrast",
                     /*border_mode*/
-                    r[5] === "contrast"
-                ), ie(e, "hide-container", ! /*explicit_call*/
-                    r[8] && ! /*container*/
-                    r[9]), a & /*height*/
+                    u[5] === "contrast"
+                ), se(e, "hide-container", ! /*explicit_call*/
+                    u[8] && ! /*container*/
+                    u[9]), a & /*height*/
                 1 && K(
                     e,
                     "height",
                     /*get_dimension*/
-                    r[15](
+                    u[15](
                         /*height*/
-                        r[0]
+                        u[0]
                     )
                 ), a & /*width*/
-                2 && K(e, "width", typeof /*width*/ r[1] == "number" ? `calc(min(${/*width*/
-      r[1]}px, 100%))` : (
+                2 && K(e, "width", typeof /*width*/ u[1] == "number" ? `calc(min(${/*width*/
+      u[1]}px, 100%))` : (
                     /*get_dimension*/
-                    r[15](
+                    u[15](
                         /*width*/
-                        r[1]
+                        u[1]
                     )
                 )), a & /*variant*/
                 16 && K(
                     e,
                     "border-style",
                     /*variant*/
-                    r[4]
+                    u[4]
                 ), a & /*allow_overflow*/
                 2048 && K(
                     e,
                     "overflow",
                     /*allow_overflow*/
-                    r[11] ? "visible" : "hidden"
+                    u[11] ? "visible" : "hidden"
                 ), a & /*scale*/
                 4096 && K(
                     e,
                     "flex-grow",
                     /*scale*/
-                    r[12]
+                    u[12]
                 ), a & /*min_width*/
                 8192 && K(e, "min-width", `calc(min(${/*min_width*/
-      r[13]}px, 100%))`);
+      u[13]}px, 100%))`);
         },
-        i(r) {
-            n || (dl(o, r), n = !0);
+        i(u) {
+            n || (cl(f, u), n = !0);
         },
-        o(r) {
-            ml(o, r), n = !1;
+        o(u) {
+            dl(f, u), n = !1;
         },
-        d(r) {
-            r && Tl(e), o && o.d(r);
+        d(u) {
+            u && El(e), f && f.d(u);
         }
     };
 }
 
-function Ol(l) {
+function Kl(l) {
     let e, t = (
         /*tag*/
-        l[14] && Kl(l)
+        l[14] && Yl(l)
     );
     return {
         c() {
             t && t.c();
         },
         m(n, s) {
             t && t.m(n, s), e = !0;
         },
         p(n, [s]) {
             /*tag*/
             n[14] && t.p(n, s);
         },
         i(n) {
-            e || (dl(t, n), e = !0);
+            e || (cl(t, n), e = !0);
         },
         o(n) {
-            ml(t, n), e = !1;
+            dl(t, n), e = !1;
         },
         d(n) {
             t && t.d(n);
         }
     };
 }
 
-function Ul(l, e, t) {
+function Ol(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: s
     } = e, {
-        height: o = void 0
+        height: f = void 0
     } = e, {
         width: i = void 0
     } = e, {
-        elem_id: f = ""
+        elem_id: o = ""
     } = e, {
-        elem_classes: r = []
+        elem_classes: u = []
     } = e, {
         variant: a = "solid"
     } = e, {
-        border_mode: u = "base"
+        border_mode: r = "base"
     } = e, {
         padding: _ = !0
     } = e, {
         type: c = "normal"
     } = e, {
         test_id: h = void 0
     } = e, {
         explicit_call: L = !1
     } = e, {
-        container: H = !0
+        container: M = !0
     } = e, {
-        visible: p = !0
+        visible: k = !0
     } = e, {
         allow_overflow: v = !0
     } = e, {
         scale: m = null
     } = e, {
         min_width: b = 0
     } = e, C = c === "fieldset" ? "fieldset" : "div";
-    const T = (k) => {
-        if (k !== void 0) {
-            if (typeof k == "number")
-                return k + "px";
-            if (typeof k == "string")
-                return k;
+    const T = (p) => {
+        if (p !== void 0) {
+            if (typeof p == "number")
+                return p + "px";
+            if (typeof p == "string")
+                return p;
         }
     };
-    return l.$$set = (k) => {
-        "height" in k && t(0, o = k.height), "width" in k && t(1, i = k.width), "elem_id" in k && t(2, f = k.elem_id), "elem_classes" in k && t(3, r = k.elem_classes), "variant" in k && t(4, a = k.variant), "border_mode" in k && t(5, u = k.border_mode), "padding" in k && t(6, _ = k.padding), "type" in k && t(16, c = k.type), "test_id" in k && t(7, h = k.test_id), "explicit_call" in k && t(8, L = k.explicit_call), "container" in k && t(9, H = k.container), "visible" in k && t(10, p = k.visible), "allow_overflow" in k && t(11, v = k.allow_overflow), "scale" in k && t(12, m = k.scale), "min_width" in k && t(13, b = k.min_width), "$$scope" in k && t(17, s = k.$$scope);
+    return l.$$set = (p) => {
+        "height" in p && t(0, f = p.height), "width" in p && t(1, i = p.width), "elem_id" in p && t(2, o = p.elem_id), "elem_classes" in p && t(3, u = p.elem_classes), "variant" in p && t(4, a = p.variant), "border_mode" in p && t(5, r = p.border_mode), "padding" in p && t(6, _ = p.padding), "type" in p && t(16, c = p.type), "test_id" in p && t(7, h = p.test_id), "explicit_call" in p && t(8, L = p.explicit_call), "container" in p && t(9, M = p.container), "visible" in p && t(10, k = p.visible), "allow_overflow" in p && t(11, v = p.allow_overflow), "scale" in p && t(12, m = p.scale), "min_width" in p && t(13, b = p.min_width), "$$scope" in p && t(17, s = p.$$scope);
     }, [
-        o,
-        i,
         f,
-        r,
-        a,
+        i,
+        o,
         u,
+        a,
+        r,
         _,
         h,
         L,
-        H,
-        p,
+        M,
+        k,
         v,
         m,
         b,
         C,
         T,
         c,
         s,
         n
     ];
 }
-class Xl extends Sl {
+class Ul extends Zl {
     constructor(e) {
-        super(), jl(this, e, Ul, Ol, Pl, {
+        super(), Il(this, e, Ol, Kl, Al, {
             height: 0,
             width: 1,
             elem_id: 2,
             elem_classes: 3,
             variant: 4,
             border_mode: 5,
             padding: 6,
@@ -342,343 +342,343 @@
             allow_overflow: 11,
             scale: 12,
             min_width: 13
         });
     }
 }
 const {
-    SvelteComponent: Gl,
-    attr: Rl,
-    create_slot: Wl,
-    detach: Jl,
-    element: Ql,
-    get_all_dirty_from_scope: xl,
-    get_slot_changes: $l,
-    init: en,
-    insert: tn,
-    safe_not_equal: ln,
-    transition_in: nn,
-    transition_out: sn,
-    update_slot_base: on
+    SvelteComponent: Xl,
+    attr: Gl,
+    create_slot: Rl,
+    detach: Wl,
+    element: Jl,
+    get_all_dirty_from_scope: Ql,
+    get_slot_changes: xl,
+    init: $l,
+    insert: en,
+    safe_not_equal: tn,
+    transition_in: ln,
+    transition_out: nn,
+    update_slot_base: sn
 } = window.__gradio__svelte__internal;
 
 function fn(l) {
     let e, t;
     const n = (
             /*#slots*/
             l[1].default
         ),
-        s = Wl(
+        s = Rl(
             n,
             l,
             /*$$scope*/
             l[0],
             null
         );
     return {
         c() {
-            e = Ql("div"), s && s.c(), Rl(e, "class", "svelte-1hnfib2");
+            e = Jl("div"), s && s.c(), Gl(e, "class", "svelte-1hnfib2");
         },
-        m(o, i) {
-            tn(o, e, i), s && s.m(e, null), t = !0;
+        m(f, i) {
+            en(f, e, i), s && s.m(e, null), t = !0;
         },
-        p(o, [i]) {
+        p(f, [i]) {
             s && s.p && (!t || i & /*$$scope*/
-                1) && on(
+                1) && sn(
                 s,
                 n,
-                o,
+                f,
                 /*$$scope*/
-                o[0],
-                t ? $l(
+                f[0],
+                t ? xl(
                     n,
                     /*$$scope*/
-                    o[0],
+                    f[0],
                     i,
                     null
-                ) : xl(
+                ) : Ql(
                     /*$$scope*/
-                    o[0]
+                    f[0]
                 ),
                 null
             );
         },
-        i(o) {
-            t || (nn(s, o), t = !0);
+        i(f) {
+            t || (ln(s, f), t = !0);
         },
-        o(o) {
-            sn(s, o), t = !1;
+        o(f) {
+            nn(s, f), t = !1;
         },
-        d(o) {
-            o && Jl(e), s && s.d(o);
+        d(f) {
+            f && Wl(e), s && s.d(f);
         }
     };
 }
 
-function an(l, e, t) {
+function on(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: s
     } = e;
-    return l.$$set = (o) => {
-        "$$scope" in o && t(0, s = o.$$scope);
+    return l.$$set = (f) => {
+        "$$scope" in f && t(0, s = f.$$scope);
     }, [s, n];
 }
-class rn extends Gl {
+class an extends Xl {
     constructor(e) {
-        super(), en(this, e, an, fn, ln, {});
+        super(), $l(this, e, on, fn, tn, {});
     }
 }
 const {
     SvelteComponent: un,
-    attr: Vt,
-    check_outros: _n,
-    create_component: cn,
-    create_slot: dn,
-    destroy_component: mn,
+    attr: Mt,
+    check_outros: rn,
+    create_component: _n,
+    create_slot: cn,
+    destroy_component: dn,
     detach: Pe,
-    element: hn,
-    empty: bn,
-    get_all_dirty_from_scope: gn,
-    get_slot_changes: wn,
-    group_outros: vn,
-    init: kn,
+    element: mn,
+    empty: hn,
+    get_all_dirty_from_scope: bn,
+    get_slot_changes: gn,
+    group_outros: wn,
+    init: vn,
     insert: Ye,
     mount_component: pn,
-    safe_not_equal: Cn,
-    set_data: yn,
-    space: Ln,
-    text: Mn,
+    safe_not_equal: kn,
+    set_data: Cn,
+    space: yn,
+    text: Ln,
     toggle_class: Le,
     transition_in: Be,
     transition_out: Ke,
-    update_slot_base: Vn
+    update_slot_base: Mn
 } = window.__gradio__svelte__internal;
 
-function Ht(l) {
+function Vt(l) {
     let e, t;
-    return e = new rn({
+    return e = new an({
         props: {
             $$slots: {
-                default: [Hn]
+                default: [Vn]
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
-            cn(e.$$.fragment);
+            _n(e.$$.fragment);
         },
         m(n, s) {
             pn(e, n, s), t = !0;
         },
         p(n, s) {
-            const o = {};
+            const f = {};
             s & /*$$scope, info*/
-                10 && (o.$$scope = {
+                10 && (f.$$scope = {
                     dirty: s,
                     ctx: n
-                }), e.$set(o);
+                }), e.$set(f);
         },
         i(n) {
             t || (Be(e.$$.fragment, n), t = !0);
         },
         o(n) {
             Ke(e.$$.fragment, n), t = !1;
         },
         d(n) {
-            mn(e, n);
+            dn(e, n);
         }
     };
 }
 
-function Hn(l) {
+function Vn(l) {
     let e;
     return {
         c() {
-            e = Mn(
+            e = Ln(
                 /*info*/
                 l[1]
             );
         },
         m(t, n) {
             Ye(t, e, n);
         },
         p(t, n) {
             n & /*info*/
-                2 && yn(
+                2 && Cn(
                     e,
                     /*info*/
                     t[1]
                 );
         },
         d(t) {
             t && Pe(e);
         }
     };
 }
 
-function qn(l) {
+function Hn(l) {
     let e, t, n, s;
-    const o = (
+    const f = (
             /*#slots*/
             l[2].default
         ),
-        i = dn(
-            o,
+        i = cn(
+            f,
             l,
             /*$$scope*/
             l[3],
             null
         );
-    let f = (
+    let o = (
         /*info*/
-        l[1] && Ht(l)
+        l[1] && Vt(l)
     );
     return {
         c() {
-            e = hn("span"), i && i.c(), t = Ln(), f && f.c(), n = bn(), Vt(e, "data-testid", "block-info"), Vt(e, "class", "svelte-22c38v"), Le(e, "sr-only", ! /*show_label*/
+            e = mn("span"), i && i.c(), t = yn(), o && o.c(), n = hn(), Mt(e, "data-testid", "block-info"), Mt(e, "class", "svelte-22c38v"), Le(e, "sr-only", ! /*show_label*/
                 l[0]), Le(e, "hide", ! /*show_label*/
                 l[0]), Le(
                 e,
                 "has-info",
                 /*info*/
                 l[1] != null
             );
         },
-        m(r, a) {
-            Ye(r, e, a), i && i.m(e, null), Ye(r, t, a), f && f.m(r, a), Ye(r, n, a), s = !0;
+        m(u, a) {
+            Ye(u, e, a), i && i.m(e, null), Ye(u, t, a), o && o.m(u, a), Ye(u, n, a), s = !0;
         },
-        p(r, [a]) {
+        p(u, [a]) {
             i && i.p && (!s || a & /*$$scope*/
-                    8) && Vn(
+                    8) && Mn(
                     i,
-                    o,
-                    r,
+                    f,
+                    u,
                     /*$$scope*/
-                    r[3],
-                    s ? wn(
-                        o,
+                    u[3],
+                    s ? gn(
+                        f,
                         /*$$scope*/
-                        r[3],
+                        u[3],
                         a,
                         null
-                    ) : gn(
+                    ) : bn(
                         /*$$scope*/
-                        r[3]
+                        u[3]
                     ),
                     null
                 ), (!s || a & /*show_label*/
                     1) && Le(e, "sr-only", ! /*show_label*/
-                    r[0]), (!s || a & /*show_label*/
+                    u[0]), (!s || a & /*show_label*/
                     1) && Le(e, "hide", ! /*show_label*/
-                    r[0]), (!s || a & /*info*/
+                    u[0]), (!s || a & /*info*/
                     2) && Le(
                     e,
                     "has-info",
                     /*info*/
-                    r[1] != null
+                    u[1] != null
                 ), /*info*/
-                r[1] ? f ? (f.p(r, a), a & /*info*/
-                    2 && Be(f, 1)) : (f = Ht(r), f.c(), Be(f, 1), f.m(n.parentNode, n)) : f && (vn(), Ke(f, 1, 1, () => {
-                    f = null;
-                }), _n());
+                u[1] ? o ? (o.p(u, a), a & /*info*/
+                    2 && Be(o, 1)) : (o = Vt(u), o.c(), Be(o, 1), o.m(n.parentNode, n)) : o && (wn(), Ke(o, 1, 1, () => {
+                    o = null;
+                }), rn());
         },
-        i(r) {
-            s || (Be(i, r), Be(f), s = !0);
+        i(u) {
+            s || (Be(i, u), Be(o), s = !0);
         },
-        o(r) {
-            Ke(i, r), Ke(f), s = !1;
+        o(u) {
+            Ke(i, u), Ke(o), s = !1;
         },
-        d(r) {
-            r && (Pe(e), Pe(t), Pe(n)), i && i.d(r), f && f.d(r);
+        d(u) {
+            u && (Pe(e), Pe(t), Pe(n)), i && i.d(u), o && o.d(u);
         }
     };
 }
 
-function Fn(l, e, t) {
+function qn(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: s
     } = e, {
-        show_label: o = !0
+        show_label: f = !0
     } = e, {
         info: i = void 0
     } = e;
-    return l.$$set = (f) => {
-        "show_label" in f && t(0, o = f.show_label), "info" in f && t(1, i = f.info), "$$scope" in f && t(3, s = f.$$scope);
-    }, [o, i, n, s];
+    return l.$$set = (o) => {
+        "show_label" in o && t(0, f = o.show_label), "info" in o && t(1, i = o.info), "$$scope" in o && t(3, s = o.$$scope);
+    }, [f, i, n, s];
 }
-class Zn extends un {
+class Fn extends un {
     constructor(e) {
-        super(), kn(this, e, Fn, qn, Cn, {
+        super(), vn(this, e, qn, Hn, kn, {
             show_label: 0,
             info: 1
         });
     }
 }
 const {
-    SvelteComponent: Sn,
-    append: ut,
-    attr: ue,
-    bubble: zn,
-    create_component: En,
-    destroy_component: Tn,
-    detach: hl,
+    SvelteComponent: Zn,
+    append: rt,
+    attr: re,
+    bubble: Sn,
+    create_component: zn,
+    destroy_component: En,
+    detach: ml,
     element: _t,
-    init: Bn,
-    insert: bl,
-    listen: Nn,
-    mount_component: Dn,
-    safe_not_equal: In,
-    set_data: jn,
+    init: Tn,
+    insert: hl,
+    listen: Bn,
+    mount_component: Nn,
+    safe_not_equal: Dn,
+    set_data: In,
     set_style: Me,
-    space: An,
-    text: Pn,
+    space: jn,
+    text: An,
     toggle_class: P,
-    transition_in: Yn,
-    transition_out: Kn
+    transition_in: Pn,
+    transition_out: Yn
 } = window.__gradio__svelte__internal;
 
-function qt(l) {
+function Ht(l) {
     let e, t;
     return {
         c() {
-            e = _t("span"), t = Pn(
+            e = _t("span"), t = An(
                 /*label*/
                 l[1]
-            ), ue(e, "class", "svelte-1lrphxw");
+            ), re(e, "class", "svelte-1lrphxw");
         },
         m(n, s) {
-            bl(n, e, s), ut(e, t);
+            hl(n, e, s), rt(e, t);
         },
         p(n, s) {
             s & /*label*/
-                2 && jn(
+                2 && In(
                     t,
                     /*label*/
                     n[1]
                 );
         },
         d(n) {
-            n && hl(e);
+            n && ml(e);
         }
     };
 }
 
-function On(l) {
-    let e, t, n, s, o, i, f, r = (
+function Kn(l) {
+    let e, t, n, s, f, i, o, u = (
         /*show_label*/
-        l[2] && qt(l)
+        l[2] && Ht(l)
     );
     return s = new /*Icon*/
     l[0]({}), {
         c() {
-            e = _t("button"), r && r.c(), t = An(), n = _t("div"), En(s.$$.fragment), ue(n, "class", "svelte-1lrphxw"), P(
+            e = _t("button"), u && u.c(), t = jn(), n = _t("div"), zn(s.$$.fragment), re(n, "class", "svelte-1lrphxw"), P(
                     n,
                     "small",
                     /*size*/
                     l[4] === "small"
                 ), P(
                     n,
                     "large",
@@ -686,30 +686,30 @@
                     l[4] === "large"
                 ), P(
                     n,
                     "medium",
                     /*size*/
                     l[4] === "medium"
                 ), e.disabled = /*disabled*/
-                l[7], ue(
+                l[7], re(
                     e,
                     "aria-label",
                     /*label*/
                     l[1]
-                ), ue(
+                ), re(
                     e,
                     "aria-haspopup",
                     /*hasPopup*/
                     l[8]
-                ), ue(
+                ), re(
                     e,
                     "title",
                     /*label*/
                     l[1]
-                ), ue(e, "class", "svelte-1lrphxw"), P(
+                ), re(e, "class", "svelte-1lrphxw"), P(
                     e,
                     "pending",
                     /*pending*/
                     l[3]
                 ), P(
                     e,
                     "padded",
@@ -737,187 +737,187 @@
                     )), Me(
                     e,
                     "margin-left",
                     /*offset*/
                     l[11] + "px"
                 );
         },
-        m(a, u) {
-            bl(a, e, u), r && r.m(e, null), ut(e, t), ut(e, n), Dn(s, n, null), o = !0, i || (f = Nn(
+        m(a, r) {
+            hl(a, e, r), u && u.m(e, null), rt(e, t), rt(e, n), Nn(s, n, null), f = !0, i || (o = Bn(
                 e,
                 "click",
                 /*click_handler*/
                 l[14]
             ), i = !0);
         },
-        p(a, [u]) {
+        p(a, [r]) {
             /*show_label*/
-            a[2] ? r ? r.p(a, u) : (r = qt(a), r.c(), r.m(e, t)) : r && (r.d(1), r = null), (!o || u & /*size*/
+            a[2] ? u ? u.p(a, r) : (u = Ht(a), u.c(), u.m(e, t)) : u && (u.d(1), u = null), (!f || r & /*size*/
                     16) && P(
                     n,
                     "small",
                     /*size*/
                     a[4] === "small"
-                ), (!o || u & /*size*/
+                ), (!f || r & /*size*/
                     16) && P(
                     n,
                     "large",
                     /*size*/
                     a[4] === "large"
-                ), (!o || u & /*size*/
+                ), (!f || r & /*size*/
                     16) && P(
                     n,
                     "medium",
                     /*size*/
                     a[4] === "medium"
-                ), (!o || u & /*disabled*/
+                ), (!f || r & /*disabled*/
                     128) && (e.disabled = /*disabled*/
-                    a[7]), (!o || u & /*label*/
-                    2) && ue(
+                    a[7]), (!f || r & /*label*/
+                    2) && re(
                     e,
                     "aria-label",
                     /*label*/
                     a[1]
-                ), (!o || u & /*hasPopup*/
-                    256) && ue(
+                ), (!f || r & /*hasPopup*/
+                    256) && re(
                     e,
                     "aria-haspopup",
                     /*hasPopup*/
                     a[8]
-                ), (!o || u & /*label*/
-                    2) && ue(
+                ), (!f || r & /*label*/
+                    2) && re(
                     e,
                     "title",
                     /*label*/
                     a[1]
-                ), (!o || u & /*pending*/
+                ), (!f || r & /*pending*/
                     8) && P(
                     e,
                     "pending",
                     /*pending*/
                     a[3]
-                ), (!o || u & /*padded*/
+                ), (!f || r & /*padded*/
                     32) && P(
                     e,
                     "padded",
                     /*padded*/
                     a[5]
-                ), (!o || u & /*highlight*/
+                ), (!f || r & /*highlight*/
                     64) && P(
                     e,
                     "highlight",
                     /*highlight*/
                     a[6]
-                ), (!o || u & /*transparent*/
+                ), (!f || r & /*transparent*/
                     512) && P(
                     e,
                     "transparent",
                     /*transparent*/
                     a[9]
-                ), u & /*disabled, _color*/
+                ), r & /*disabled, _color*/
                 4224 && Me(e, "color", ! /*disabled*/
                     a[7] && /*_color*/
                     a[12] ? (
                         /*_color*/
                         a[12]
-                    ) : "var(--block-label-text-color)"), u & /*disabled, background*/
+                    ) : "var(--block-label-text-color)"), r & /*disabled, background*/
                 1152 && Me(e, "--bg-color", /*disabled*/
                     a[7] ? "auto" : (
                         /*background*/
                         a[10]
-                    )), u & /*offset*/
+                    )), r & /*offset*/
                 2048 && Me(
                     e,
                     "margin-left",
                     /*offset*/
                     a[11] + "px"
                 );
         },
         i(a) {
-            o || (Yn(s.$$.fragment, a), o = !0);
+            f || (Pn(s.$$.fragment, a), f = !0);
         },
         o(a) {
-            Kn(s.$$.fragment, a), o = !1;
+            Yn(s.$$.fragment, a), f = !1;
         },
         d(a) {
-            a && hl(e), r && r.d(), Tn(s), i = !1, f();
+            a && ml(e), u && u.d(), En(s), i = !1, o();
         }
     };
 }
 
-function Un(l, e, t) {
+function On(l, e, t) {
     let n, {
             Icon: s
         } = e,
         {
-            label: o = ""
+            label: f = ""
         } = e,
         {
             show_label: i = !1
         } = e,
         {
-            pending: f = !1
+            pending: o = !1
         } = e,
         {
-            size: r = "small"
+            size: u = "small"
         } = e,
         {
             padded: a = !0
         } = e,
         {
-            highlight: u = !1
+            highlight: r = !1
         } = e,
         {
             disabled: _ = !1
         } = e,
         {
             hasPopup: c = !1
         } = e,
         {
             color: h = "var(--block-label-text-color)"
         } = e,
         {
             transparent: L = !1
         } = e,
         {
-            background: H = "var(--background-fill-primary)"
+            background: M = "var(--background-fill-primary)"
         } = e,
         {
-            offset: p = 0
+            offset: k = 0
         } = e;
 
     function v(m) {
-        zn.call(this, l, m);
+        Sn.call(this, l, m);
     }
     return l.$$set = (m) => {
-        "Icon" in m && t(0, s = m.Icon), "label" in m && t(1, o = m.label), "show_label" in m && t(2, i = m.show_label), "pending" in m && t(3, f = m.pending), "size" in m && t(4, r = m.size), "padded" in m && t(5, a = m.padded), "highlight" in m && t(6, u = m.highlight), "disabled" in m && t(7, _ = m.disabled), "hasPopup" in m && t(8, c = m.hasPopup), "color" in m && t(13, h = m.color), "transparent" in m && t(9, L = m.transparent), "background" in m && t(10, H = m.background), "offset" in m && t(11, p = m.offset);
+        "Icon" in m && t(0, s = m.Icon), "label" in m && t(1, f = m.label), "show_label" in m && t(2, i = m.show_label), "pending" in m && t(3, o = m.pending), "size" in m && t(4, u = m.size), "padded" in m && t(5, a = m.padded), "highlight" in m && t(6, r = m.highlight), "disabled" in m && t(7, _ = m.disabled), "hasPopup" in m && t(8, c = m.hasPopup), "color" in m && t(13, h = m.color), "transparent" in m && t(9, L = m.transparent), "background" in m && t(10, M = m.background), "offset" in m && t(11, k = m.offset);
     }, l.$$.update = () => {
         l.$$.dirty & /*highlight, color*/
-            8256 && t(12, n = u ? "var(--color-accent)" : h);
+            8256 && t(12, n = r ? "var(--color-accent)" : h);
     }, [
         s,
-        o,
-        i,
         f,
-        r,
-        a,
+        i,
+        o,
         u,
+        a,
+        r,
         _,
         c,
         L,
-        H,
-        p,
+        M,
+        k,
         n,
         h,
         v
     ];
 }
-class Xn extends Sn {
+class Un extends Zn {
     constructor(e) {
-        super(), Bn(this, e, Un, On, In, {
+        super(), Tn(this, e, On, Kn, Dn, {
             Icon: 0,
             label: 1,
             show_label: 2,
             pending: 3,
             size: 4,
             padded: 5,
             highlight: 6,
@@ -927,49 +927,49 @@
             transparent: 9,
             background: 10,
             offset: 11
         });
     }
 }
 const {
-    SvelteComponent: Gn,
+    SvelteComponent: Xn,
     append: it,
     attr: R,
-    detach: Rn,
-    init: Wn,
-    insert: Jn,
+    detach: Gn,
+    init: Rn,
+    insert: Wn,
     noop: st,
-    safe_not_equal: Qn,
-    set_style: se,
+    safe_not_equal: Jn,
+    set_style: fe,
     svg_element: Ie
 } = window.__gradio__svelte__internal;
 
-function xn(l) {
+function Qn(l) {
     let e, t, n, s;
     return {
         c() {
-            e = Ie("svg"), t = Ie("g"), n = Ie("path"), s = Ie("path"), R(n, "d", "M18,6L6.087,17.913"), se(n, "fill", "none"), se(n, "fill-rule", "nonzero"), se(n, "stroke-width", "2px"), R(t, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), R(s, "d", "M4.364,4.364L19.636,19.636"), se(s, "fill", "none"), se(s, "fill-rule", "nonzero"), se(s, "stroke-width", "2px"), R(e, "width", "100%"), R(e, "height", "100%"), R(e, "viewBox", "0 0 24 24"), R(e, "version", "1.1"), R(e, "xmlns", "http://www.w3.org/2000/svg"), R(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), R(e, "xml:space", "preserve"), R(e, "stroke", "currentColor"), se(e, "fill-rule", "evenodd"), se(e, "clip-rule", "evenodd"), se(e, "stroke-linecap", "round"), se(e, "stroke-linejoin", "round");
+            e = Ie("svg"), t = Ie("g"), n = Ie("path"), s = Ie("path"), R(n, "d", "M18,6L6.087,17.913"), fe(n, "fill", "none"), fe(n, "fill-rule", "nonzero"), fe(n, "stroke-width", "2px"), R(t, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), R(s, "d", "M4.364,4.364L19.636,19.636"), fe(s, "fill", "none"), fe(s, "fill-rule", "nonzero"), fe(s, "stroke-width", "2px"), R(e, "width", "100%"), R(e, "height", "100%"), R(e, "viewBox", "0 0 24 24"), R(e, "version", "1.1"), R(e, "xmlns", "http://www.w3.org/2000/svg"), R(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), R(e, "xml:space", "preserve"), R(e, "stroke", "currentColor"), fe(e, "fill-rule", "evenodd"), fe(e, "clip-rule", "evenodd"), fe(e, "stroke-linecap", "round"), fe(e, "stroke-linejoin", "round");
         },
-        m(o, i) {
-            Jn(o, e, i), it(e, t), it(t, n), it(e, s);
+        m(f, i) {
+            Wn(f, e, i), it(e, t), it(t, n), it(e, s);
         },
         p: st,
         i: st,
         o: st,
-        d(o) {
-            o && Rn(e);
+        d(f) {
+            f && Gn(e);
         }
     };
 }
-class $n extends Gn {
+class xn extends Xn {
     constructor(e) {
-        super(), Wn(this, e, null, xn, Qn, {});
+        super(), Rn(this, e, null, Qn, Jn, {});
     }
 }
-const ei = [{
+const $n = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
         color: "green",
         primary: 600,
         secondary: 100
@@ -1002,15 +1002,15 @@
         primary: 500,
         secondary: 100
     }, {
         color: "pink",
         primary: 600,
         secondary: 100
     }],
-    Ft = {
+    qt = {
         inherit: "inherit",
         current: "currentColor",
         transparent: "transparent",
         black: "#000",
         white: "#fff",
         slate: {
             50: "#f8fafc",
@@ -1295,279 +1295,275 @@
             600: "#e11d48",
             700: "#be123c",
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     };
-ei.reduce(
+$n.reduce(
     (l, {
         color: e,
         primary: t,
         secondary: n
     }) => ({
         ...l,
         [e]: {
-            primary: Ft[e][t],
-            secondary: Ft[e][n]
+            primary: qt[e][t],
+            secondary: qt[e][n]
         }
     }), {}
 );
 
 function Oe() {}
 
-function ti(l, e) {
+function ei(l, e) {
     return l != l ? e == e : l !== e || l && typeof l == "object" || typeof l == "function";
 }
-const gl = typeof window < "u";
-let Zt = gl ? () => window.performance.now() : () => Date.now(),
-    wl = gl ? (l) => requestAnimationFrame(l) : Oe;
+const bl = typeof window < "u";
+let Ft = bl ? () => window.performance.now() : () => Date.now(),
+    gl = bl ? (l) => requestAnimationFrame(l) : Oe;
 const Se = /* @__PURE__ */ new Set();
 
-function vl(l) {
+function wl(l) {
     Se.forEach((e) => {
         e.c(l) || (Se.delete(e), e.f());
-    }), Se.size !== 0 && wl(vl);
+    }), Se.size !== 0 && gl(wl);
 }
 
-function li(l) {
+function ti(l) {
     let e;
-    return Se.size === 0 && wl(vl), {
+    return Se.size === 0 && gl(wl), {
         promise: new Promise((t) => {
             Se.add(e = {
                 c: l,
                 f: t
             });
         }),
         abort() {
             Se.delete(e);
         }
     };
 }
 
-function ni(l) {
+function li(l) {
     const e = l - 1;
     return e * e * e + 1;
 }
 const Ve = [];
 
-function ii(l, e = Oe) {
+function ni(l, e = Oe) {
     let t;
     const n = /* @__PURE__ */ new Set();
 
-    function s(f) {
-        if (ti(l, f) && (l = f, t)) {
-            const r = !Ve.length;
+    function s(o) {
+        if (ei(l, o) && (l = o, t)) {
+            const u = !Ve.length;
             for (const a of n)
                 a[1](), Ve.push(a, l);
-            if (r) {
+            if (u) {
                 for (let a = 0; a < Ve.length; a += 2)
                     Ve[a][0](Ve[a + 1]);
                 Ve.length = 0;
             }
         }
     }
 
-    function o(f) {
-        s(f(l));
+    function f(o) {
+        s(o(l));
     }
 
-    function i(f, r = Oe) {
-        const a = [f, r];
-        return n.add(a), n.size === 1 && (t = e(s, o) || Oe), f(l), () => {
+    function i(o, u = Oe) {
+        const a = [o, u];
+        return n.add(a), n.size === 1 && (t = e(s, f) || Oe), o(l), () => {
             n.delete(a), n.size === 0 && t && (t(), t = null);
         };
     }
     return {
         set: s,
-        update: o,
+        update: f,
         subscribe: i
     };
 }
 
-function St(l) {
+function Zt(l) {
     return Object.prototype.toString.call(l) === "[object Date]";
 }
 
 function ct(l, e, t, n) {
-    if (typeof t == "number" || St(t)) {
+    if (typeof t == "number" || Zt(t)) {
         const s = n - t,
-            o = (t - e) / (l.dt || 1 / 60),
+            f = (t - e) / (l.dt || 1 / 60),
             i = l.opts.stiffness * s,
-            f = l.opts.damping * o,
-            r = (i - f) * l.inv_mass,
-            a = (o + r) * l.dt;
-        return Math.abs(a) < l.opts.precision && Math.abs(s) < l.opts.precision ? n : (l.settled = !1, St(t) ? new Date(t.getTime() + a) : t + a);
+            o = l.opts.damping * f,
+            u = (i - o) * l.inv_mass,
+            a = (f + u) * l.dt;
+        return Math.abs(a) < l.opts.precision && Math.abs(s) < l.opts.precision ? n : (l.settled = !1, Zt(t) ? new Date(t.getTime() + a) : t + a);
     } else {
         if (Array.isArray(t))
             return t.map(
-                (s, o) => ct(l, e[o], t[o], n[o])
+                (s, f) => ct(l, e[f], t[f], n[f])
             );
         if (typeof t == "object") {
             const s = {};
-            for (const o in t)
-                s[o] = ct(l, e[o], t[o], n[o]);
+            for (const f in t)
+                s[f] = ct(l, e[f], t[f], n[f]);
             return s;
         } else
             throw new Error(`Cannot spring ${typeof t} values`);
     }
 }
 
-function zt(l, e = {}) {
-    const t = ii(l),
+function St(l, e = {}) {
+    const t = ni(l),
         {
             stiffness: n = 0.15,
             damping: s = 0.8,
-            precision: o = 0.01
+            precision: f = 0.01
         } = e;
-    let i, f, r, a = l,
-        u = l,
+    let i, o, u, a = l,
+        r = l,
         _ = 1,
         c = 0,
         h = !1;
 
-    function L(p, v = {}) {
-        u = p;
-        const m = r = {};
-        return l == null || v.hard || H.stiffness >= 1 && H.damping >= 1 ? (h = !0, i = Zt(), a = p, t.set(l = u), Promise.resolve()) : (v.soft && (c = 1 / ((v.soft === !0 ? 0.5 : +v.soft) * 60), _ = 0), f || (i = Zt(), h = !1, f = li((b) => {
+    function L(k, v = {}) {
+        r = k;
+        const m = u = {};
+        return l == null || v.hard || M.stiffness >= 1 && M.damping >= 1 ? (h = !0, i = Ft(), a = k, t.set(l = r), Promise.resolve()) : (v.soft && (c = 1 / ((v.soft === !0 ? 0.5 : +v.soft) * 60), _ = 0), o || (i = Ft(), h = !1, o = ti((b) => {
             if (h)
-                return h = !1, f = null, !1;
+                return h = !1, o = null, !1;
             _ = Math.min(_ + c, 1);
             const C = {
                     inv_mass: _,
-                    opts: H,
+                    opts: M,
                     settled: !0,
                     dt: (b - i) * 60 / 1e3
                 },
-                T = ct(C, a, l, u);
-            return i = b, a = l, t.set(l = T), C.settled && (f = null), !C.settled;
+                T = ct(C, a, l, r);
+            return i = b, a = l, t.set(l = T), C.settled && (o = null), !C.settled;
         })), new Promise((b) => {
-            f.promise.then(() => {
-                m === r && b();
+            o.promise.then(() => {
+                m === u && b();
             });
         }));
     }
-    const H = {
+    const M = {
         set: L,
-        update: (p, v) => L(p(u, l), v),
+        update: (k, v) => L(k(r, l), v),
         subscribe: t.subscribe,
         stiffness: n,
         damping: s,
-        precision: o
+        precision: f
     };
-    return H;
+    return M;
 }
 
-function Et(l, {
+function zt(l, {
     delay: e = 0,
     duration: t = 500,
-    easing: n = ni
+    easing: n = li
 } = {}) {
     const s = parseFloat(getComputedStyle(l).height);
     return {
         delay: e,
         duration: t,
         easing: n,
-        css: (o) => {
-            const i = o,
-                f = `translateY(${(1 - o) * -10}px)`,
-                r = o * s;
+        css: (f) => {
+            const i = f,
+                o = `translateY(${(1 - f) * -10}px)`,
+                u = f * s;
             return `
                 opacity: ${i};
-                transform: ${f};
-                height: ${r}px;
+                transform: ${o};
+                height: ${u}px;
             `;
         }
     };
 }
 const {
-    SvelteComponent: si,
+    SvelteComponent: ii,
     action_destroyer: bt,
-    add_render_callback: oi,
+    add_render_callback: si,
     append: F,
     attr: g,
-    binding_callbacks: ot,
+    binding_callbacks: ft,
     bubble: He,
     check_outros: fi,
-    create_bidirectional_transition: Tt,
-    create_component: ai,
-    destroy_component: ri,
-    destroy_each: kl,
+    create_bidirectional_transition: Et,
+    create_component: oi,
+    destroy_component: ai,
+    destroy_each: vl,
     detach: $,
     element: B,
     ensure_array_like: Ue,
     group_outros: ui,
-    init: _i,
+    init: ri,
     insert: ee,
     is_function: gt,
     listen: E,
-    mount_component: ci,
+    mount_component: _i,
     noop: Xe,
-    null_to_empty: wt,
-    run_all: vt,
-    safe_not_equal: di,
-    set_data: kt,
+    run_all: wt,
+    safe_not_equal: ci,
+    set_data: vt,
     set_input_value: ze,
     space: te,
     svg_element: Ge,
     text: pt,
-    toggle_class: Bt,
-    transition_in: ft,
+    toggle_class: Tt,
+    transition_in: ot,
     transition_out: at
 } = window.__gradio__svelte__internal, {
-    beforeUpdate: mi,
-    afterUpdate: hi,
-    createEventDispatcher: bi,
-    tick: Nt
+    beforeUpdate: di,
+    afterUpdate: mi,
+    createEventDispatcher: hi,
+    tick: Bt
 } = window.__gradio__svelte__internal;
 
-function Dt(l, e, t) {
+function Nt(l, e, t) {
     const n = l.slice();
     return n[47] = e[t], n;
 }
 
-function It(l, e, t) {
+function Dt(l, e, t) {
     const n = l.slice();
     return n[47] = e[t], n;
 }
 
-function gi(l) {
+function bi(l) {
     let e;
     return {
         c() {
             e = pt(
                 /*label*/
                 l[3]
             );
         },
         m(t, n) {
             ee(t, e, n);
         },
         p(t, n) {
             n[0] & /*label*/
-                8 && kt(
+                8 && vt(
                     e,
                     /*label*/
                     t[3]
                 );
         },
         d(t) {
             t && $(e);
         }
     };
 }
 
-function wi(l) {
-    let e, t, n, s, o, i;
+function gi(l) {
+    let e, t, n, s, f, i;
     return {
         c() {
-            e = B("textarea"), g(e, "data-testid", "textbox"), g(e, "class", wt(
-                    /*show_magic*/
-                    l[15] ? "scroll_hide_magic" : "scroll-hide"
-                ) + " svelte-82ixrs"), g(e, "dir", t = /*rtl*/
+            e = B("textarea"), g(e, "data-testid", "textbox"), g(e, "class", "scroll-hide svelte-lsxp0u"), g(e, "dir", t = /*rtl*/
                     l[10] ? "rtl" : "ltr"), g(
                     e,
                     "placeholder",
                     /*placeholder*/
                     l[2]
                 ), g(
                     e,
@@ -1576,21 +1572,21 @@
                     l[1]
                 ), e.disabled = /*disabled*/
                 l[5], e.autofocus = /*autofocus*/
                 l[11], g(e, "style", n = /*text_align*/
                     l[12] ? "text-align: " + /*text_align*/
                     l[12] : "");
         },
-        m(f, r) {
-            ee(f, e, r), ze(
+        m(o, u) {
+            ee(o, e, u), ze(
                     e,
                     /*value*/
                     l[0]
                 ), l[38](e), /*autofocus*/
-                l[11] && e.focus(), o || (i = [
+                l[11] && e.focus(), f || (i = [
                     bt(s = /*text_area_resize*/
                         l[21].call(
                             null,
                             e,
                             /*value*/
                             l[0]
                         )),
@@ -1626,90 +1622,87 @@
                     ),
                     E(
                         e,
                         "scroll",
                         /*handle_scroll*/
                         l[20]
                     )
-                ], o = !0);
+                ], f = !0);
         },
-        p(f, r) {
-            r[0] & /*rtl*/
+        p(o, u) {
+            u[0] & /*rtl*/
                 1024 && t !== (t = /*rtl*/
-                    f[10] ? "rtl" : "ltr") && g(e, "dir", t), r[0] & /*placeholder*/
+                    o[10] ? "rtl" : "ltr") && g(e, "dir", t), u[0] & /*placeholder*/
                 4 && g(
                     e,
                     "placeholder",
                     /*placeholder*/
-                    f[2]
-                ), r[0] & /*lines*/
+                    o[2]
+                ), u[0] & /*lines*/
                 2 && g(
                     e,
                     "rows",
                     /*lines*/
-                    f[1]
-                ), r[0] & /*disabled*/
+                    o[1]
+                ), u[0] & /*disabled*/
                 32 && (e.disabled = /*disabled*/
-                    f[5]), r[0] & /*autofocus*/
+                    o[5]), u[0] & /*autofocus*/
                 2048 && (e.autofocus = /*autofocus*/
-                    f[11]), r[0] & /*text_align*/
+                    o[11]), u[0] & /*text_align*/
                 4096 && n !== (n = /*text_align*/
-                    f[12] ? "text-align: " + /*text_align*/
-                    f[12] : "") && g(e, "style", n), s && gt(s.update) && r[0] & /*value*/
+                    o[12] ? "text-align: " + /*text_align*/
+                    o[12] : "") && g(e, "style", n), s && gt(s.update) && u[0] & /*value*/
                 1 && s.update.call(
                     null,
                     /*value*/
-                    f[0]
-                ), r[0] & /*value*/
+                    o[0]
+                ), u[0] & /*value*/
                 1 && ze(
                     e,
                     /*value*/
-                    f[0]
+                    o[0]
                 );
         },
         i: Xe,
         o: Xe,
-        d(f) {
-            f && $(e), l[38](null), o = !1, vt(i);
+        d(o) {
+            o && $(e), l[38](null), f = !1, wt(i);
         }
     };
 }
 
-function vi(l) {
-    let e, t, n, s, o, i, f, r, a;
+function wi(l) {
+    let e, t, n, s, f, i, o, u, a;
     return {
         c() {
-            e = B("div"), t = B("textarea"), i = te(), f = B("button"), f.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-82ixrs"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#CCCCCC" class="svelte-82ixrs"></path></svg>', g(t, "data-testid", "textbox"), g(t, "class", wt(
-                    /*show_magic*/
-                    l[15] ? "scroll_hide_magic" : "scroll-hide"
-                ) + " svelte-82ixrs"), g(t, "dir", n = /*rtl*/
+            e = B("div"), t = B("textarea"), i = te(), o = B("button"), o.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-lsxp0u"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#CCCCCC" class="svelte-lsxp0u"></path></svg>', g(t, "data-testid", "textbox"), g(t, "class", "scroll-hide svelte-lsxp0u"), g(t, "dir", n = /*rtl*/
                     l[10] ? "rtl" : "ltr"), g(
                     t,
                     "placeholder",
                     /*placeholder*/
                     l[2]
                 ), g(
                     t,
                     "rows",
                     /*lines*/
                     l[1]
                 ), t.disabled = /*disabled*/
                 l[5], t.autofocus = /*autofocus*/
                 l[11], g(t, "style", s = /*text_align*/
                     l[12] ? "text-align: " + /*text_align*/
-                    l[12] : ""), g(f, "class", "extend_button svelte-82ixrs"), g(f, "aria-label", "Extend"), g(f, "aria-roledescription", "Extend text"), g(e, "class", "magic_container svelte-82ixrs");
+                    l[12] : ""), g(o, "class", "extend_button svelte-lsxp0u"), g(o, "aria-label", "Extend"), g(o, "aria-roledescription", "Extend text"), g(e, "class", "magic_container svelte-lsxp0u");
         },
-        m(u, _) {
-            ee(u, e, _), F(e, t), ze(
+        m(r, _) {
+            ee(r, e, _), F(e, t), ze(
                     t,
                     /*value*/
                     l[0]
-                ), l[36](t), F(e, i), F(e, f), /*autofocus*/
-                l[11] && t.focus(), r || (a = [
-                    bt(o = /*text_area_resize*/
+                ), l[36](t), F(e, i), F(e, o), /*autofocus*/
+                l[11] && t.focus(), u || (a = [
+                    bt(f = /*text_area_resize*/
                         l[21].call(
                             null,
                             t,
                             /*value*/
                             l[0]
                         )),
                     E(
@@ -1745,102 +1738,99 @@
                     E(
                         t,
                         "scroll",
                         /*handle_scroll*/
                         l[20]
                     ),
                     E(
-                        f,
+                        o,
                         "click",
                         /*handle_extension*/
                         l[16]
                     )
-                ], r = !0);
+                ], u = !0);
         },
-        p(u, _) {
+        p(r, _) {
             _[0] & /*rtl*/
                 1024 && n !== (n = /*rtl*/
-                    u[10] ? "rtl" : "ltr") && g(t, "dir", n), _[0] & /*placeholder*/
+                    r[10] ? "rtl" : "ltr") && g(t, "dir", n), _[0] & /*placeholder*/
                 4 && g(
                     t,
                     "placeholder",
                     /*placeholder*/
-                    u[2]
+                    r[2]
                 ), _[0] & /*lines*/
                 2 && g(
                     t,
                     "rows",
                     /*lines*/
-                    u[1]
+                    r[1]
                 ), _[0] & /*disabled*/
                 32 && (t.disabled = /*disabled*/
-                    u[5]), _[0] & /*autofocus*/
+                    r[5]), _[0] & /*autofocus*/
                 2048 && (t.autofocus = /*autofocus*/
-                    u[11]), _[0] & /*text_align*/
+                    r[11]), _[0] & /*text_align*/
                 4096 && s !== (s = /*text_align*/
-                    u[12] ? "text-align: " + /*text_align*/
-                    u[12] : "") && g(t, "style", s), o && gt(o.update) && _[0] & /*value*/
-                1 && o.update.call(
+                    r[12] ? "text-align: " + /*text_align*/
+                    r[12] : "") && g(t, "style", s), f && gt(f.update) && _[0] & /*value*/
+                1 && f.update.call(
                     null,
                     /*value*/
-                    u[0]
+                    r[0]
                 ), _[0] & /*value*/
                 1 && ze(
                     t,
                     /*value*/
-                    u[0]
+                    r[0]
                 );
         },
         i: Xe,
         o: Xe,
-        d(u) {
-            u && $(e), l[36](null), r = !1, vt(a);
+        d(r) {
+            r && $(e), l[36](null), u = !1, wt(a);
         }
     };
 }
 
-function ki(l) {
-    let e, t, n, s, o, i, f, r, a, u, _, c, h, L, H = (
+function vi(l) {
+    let e, t, n, s, f, i, o, u, a, r, _, c, h, L, M = (
             /*prompts*/
-            l[8].length > 0 && jt(l)
+            l[8].length > 0 && It(l)
         ),
-        p = (
+        k = (
             /*suffixes*/
-            l[9].length > 0 && Pt(l)
+            l[9].length > 0 && At(l)
         );
     return {
         c() {
-            e = B("div"), t = B("textarea"), i = te(), f = B("button"), f.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-82ixrs"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#ff6700" class="svelte-82ixrs"></path></svg>', r = te(), a = B("div"), H && H.c(), u = te(), p && p.c(), g(t, "data-testid", "textbox"), g(t, "class", wt(
-                    /*show_magic*/
-                    l[15] ? "scroll_hide_magic" : "scroll-hide"
-                ) + " svelte-82ixrs"), g(t, "dir", n = /*rtl*/
+            e = B("div"), t = B("textarea"), i = te(), o = B("button"), o.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-lsxp0u"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#ff6700" class="svelte-lsxp0u"></path></svg>', u = te(), a = B("div"), M && M.c(), r = te(), k && k.c(), g(t, "data-testid", "textbox"), g(t, "class", "scroll-hide svelte-lsxp0u"), g(t, "dir", n = /*rtl*/
                     l[10] ? "rtl" : "ltr"), g(
                     t,
                     "placeholder",
                     /*placeholder*/
                     l[2]
                 ), g(
                     t,
                     "rows",
                     /*lines*/
                     l[1]
                 ), t.disabled = /*disabled*/
                 l[5], t.autofocus = /*autofocus*/
                 l[11], g(t, "style", s = /*text_align*/
                     l[12] ? "text-align: " + /*text_align*/
-                    l[12] : ""), g(f, "class", "extend_button svelte-82ixrs"), g(f, "aria-label", "Extend"), g(f, "aria-roledescription", "Extend text"), g(e, "class", "magic_container svelte-82ixrs"), g(a, "class", "menu svelte-82ixrs");
+                    l[12] : ""), g(o, "class", "extend_button svelte-lsxp0u"), g(o, "aria-label", "Extend"), g(o, "aria-roledescription", "Extend text"), g(e, "class", "magic_container svelte-lsxp0u"), g(a, "class", "menu svelte-lsxp0u");
         },
         m(v, m) {
             ee(v, e, m), F(e, t), ze(
                     t,
                     /*value*/
                     l[0]
-                ), l[32](t), F(e, i), F(e, f), ee(v, r, m), ee(v, a, m), H && H.m(a, null), F(a, u), p && p.m(a, null), c = !0, /*autofocus*/
+                ), l[32](t), F(e, i), F(e, o), ee(v, u, m), ee(v, a, m), M && M.m(a, null), F(a, r), k && k.m(a, null), c = !0, /*autofocus*/
                 l[11] && t.focus(), h || (L = [
-                    bt(o = /*text_area_resize*/
+                    bt(f = /*text_area_resize*/
                         l[21].call(
                             null,
                             t,
                             /*value*/
                             l[0]
                         )),
                     E(
@@ -1876,15 +1866,15 @@
                     E(
                         t,
                         "scroll",
                         /*handle_scroll*/
                         l[20]
                     ),
                     E(
-                        f,
+                        o,
                         "click",
                         /*handle_extension*/
                         l[16]
                     )
                 ], h = !0);
         },
         p(v, m) {
@@ -1905,390 +1895,390 @@
                 ), (!c || m[0] & /*disabled*/
                     32) && (t.disabled = /*disabled*/
                     v[5]), (!c || m[0] & /*autofocus*/
                     2048) && (t.autofocus = /*autofocus*/
                     v[11]), (!c || m[0] & /*text_align*/
                     4096 && s !== (s = /*text_align*/
                         v[12] ? "text-align: " + /*text_align*/
-                        v[12] : "")) && g(t, "style", s), o && gt(o.update) && m[0] & /*value*/
-                1 && o.update.call(
+                        v[12] : "")) && g(t, "style", s), f && gt(f.update) && m[0] & /*value*/
+                1 && f.update.call(
                     null,
                     /*value*/
                     v[0]
                 ), m[0] & /*value*/
                 1 && ze(
                     t,
                     /*value*/
                     v[0]
                 ), /*prompts*/
-                v[8].length > 0 ? H ? H.p(v, m) : (H = jt(v), H.c(), H.m(a, u)) : H && (H.d(1), H = null), /*suffixes*/
-                v[9].length > 0 ? p ? p.p(v, m) : (p = Pt(v), p.c(), p.m(a, null)) : p && (p.d(1), p = null);
+                v[8].length > 0 ? M ? M.p(v, m) : (M = It(v), M.c(), M.m(a, r)) : M && (M.d(1), M = null), /*suffixes*/
+                v[9].length > 0 ? k ? k.p(v, m) : (k = At(v), k.c(), k.m(a, null)) : k && (k.d(1), k = null);
         },
         i(v) {
-            c || (v && oi(() => {
-                c && (_ || (_ = Tt(a, Et, {}, !0)), _.run(1));
+            c || (v && si(() => {
+                c && (_ || (_ = Et(a, zt, {}, !0)), _.run(1));
             }), c = !0);
         },
         o(v) {
-            v && (_ || (_ = Tt(a, Et, {}, !1)), _.run(0)), c = !1;
+            v && (_ || (_ = Et(a, zt, {}, !1)), _.run(0)), c = !1;
         },
         d(v) {
-            v && ($(e), $(r), $(a)), l[32](null), H && H.d(), p && p.d(), v && _ && _.end(), h = !1, vt(L);
+            v && ($(e), $(u), $(a)), l[32](null), M && M.d(), k && k.d(), v && _ && _.end(), h = !1, wt(L);
         }
     };
 }
 
-function jt(l) {
-    let e, t, n, s, o = Ue(
+function It(l) {
+    let e, t, n, s, f = Ue(
             /*prompts*/
             l[8]
         ),
         i = [];
-    for (let f = 0; f < o.length; f += 1)
-        i[f] = At(It(l, o, f));
+    for (let o = 0; o < f.length; o += 1)
+        i[o] = jt(Dt(l, f, o));
     return {
         c() {
             e = B("div"), t = B("span"), t.textContent = "Best prompt structures", n = te(), s = B("ul");
-            for (let f = 0; f < i.length; f += 1)
-                i[f].c();
-            g(s, "class", "svelte-82ixrs"), g(e, "class", "menu_section svelte-82ixrs");
+            for (let o = 0; o < i.length; o += 1)
+                i[o].c();
+            g(s, "class", "svelte-lsxp0u"), g(e, "class", "menu_section svelte-lsxp0u");
         },
-        m(f, r) {
-            ee(f, e, r), F(e, t), F(e, n), F(e, s);
+        m(o, u) {
+            ee(o, e, u), F(e, t), F(e, n), F(e, s);
             for (let a = 0; a < i.length; a += 1)
                 i[a] && i[a].m(s, null);
         },
-        p(f, r) {
-            if (r[0] & /*addToTextbox, prompts*/
+        p(o, u) {
+            if (u[0] & /*addToTextbox, prompts*/
                 131328) {
-                o = Ue(
+                f = Ue(
                     /*prompts*/
-                    f[8]
+                    o[8]
                 );
                 let a;
-                for (a = 0; a < o.length; a += 1) {
-                    const u = It(f, o, a);
-                    i[a] ? i[a].p(u, r) : (i[a] = At(u), i[a].c(), i[a].m(s, null));
+                for (a = 0; a < f.length; a += 1) {
+                    const r = Dt(o, f, a);
+                    i[a] ? i[a].p(r, u) : (i[a] = jt(r), i[a].c(), i[a].m(s, null));
                 }
                 for (; a < i.length; a += 1)
                     i[a].d(1);
-                i.length = o.length;
+                i.length = f.length;
             }
         },
-        d(f) {
-            f && $(e), kl(i, f);
+        d(o) {
+            o && $(e), vl(i, o);
         }
     };
 }
 
-function At(l) {
+function jt(l) {
     let e, t, n = (
             /*word*/
             l[47] + ""
         ),
-        s, o, i, f, r, a, u;
+        s, f, i, o, u, a, r;
 
     function _() {
         return (
             /*click_handler*/
             l[33](
                 /*word*/
                 l[47]
             )
         );
     }
     return {
         c() {
-            e = B("li"), t = B("button"), s = pt(n), o = te(), i = Ge("svg"), f = Ge("path"), r = te(), g(f, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), g(f, "fill", "#FF9A57"), g(f, "class", "svelte-82ixrs"), g(i, "xmlns", "http://www.w3.org/2000/svg"), g(i, "width", "11"), g(i, "height", "12"), g(i, "viewBox", "0 0 11 12"), g(i, "fill", "none"), g(i, "class", "svelte-82ixrs"), g(t, "class", "text_extension_button_prompt svelte-82ixrs"), g(e, "class", "svelte-82ixrs");
+            e = B("li"), t = B("button"), s = pt(n), f = te(), i = Ge("svg"), o = Ge("path"), u = te(), g(o, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), g(o, "fill", "#FF9A57"), g(o, "class", "svelte-lsxp0u"), g(i, "xmlns", "http://www.w3.org/2000/svg"), g(i, "width", "11"), g(i, "height", "12"), g(i, "viewBox", "0 0 11 12"), g(i, "fill", "none"), g(i, "class", "svelte-lsxp0u"), g(t, "class", "text_extension_button_prompt svelte-lsxp0u"), g(e, "class", "svelte-lsxp0u");
         },
         m(c, h) {
-            ee(c, e, h), F(e, t), F(t, s), F(t, o), F(t, i), F(i, f), F(e, r), a || (u = E(t, "click", _), a = !0);
+            ee(c, e, h), F(e, t), F(t, s), F(t, f), F(t, i), F(i, o), F(e, u), a || (r = E(t, "click", _), a = !0);
         },
         p(c, h) {
             l = c, h[0] & /*prompts*/
                 256 && n !== (n = /*word*/
-                    l[47] + "") && kt(s, n);
+                    l[47] + "") && vt(s, n);
         },
         d(c) {
-            c && $(e), a = !1, u();
+            c && $(e), a = !1, r();
         }
     };
 }
 
-function Pt(l) {
-    let e, t, n, s, o = Ue(
+function At(l) {
+    let e, t, n, s, f = Ue(
             /*suffixes*/
             l[9]
         ),
         i = [];
-    for (let f = 0; f < o.length; f += 1)
-        i[f] = Yt(Dt(l, o, f));
+    for (let o = 0; o < f.length; o += 1)
+        i[o] = Pt(Nt(l, f, o));
     return {
         c() {
             e = B("div"), t = B("span"), t.textContent = "Best style keywords", n = te(), s = B("ul");
-            for (let f = 0; f < i.length; f += 1)
-                i[f].c();
-            g(s, "class", "svelte-82ixrs"), g(e, "class", "menu_section svelte-82ixrs");
+            for (let o = 0; o < i.length; o += 1)
+                i[o].c();
+            g(s, "class", "svelte-lsxp0u"), g(e, "class", "menu_section svelte-lsxp0u");
         },
-        m(f, r) {
-            ee(f, e, r), F(e, t), F(e, n), F(e, s);
+        m(o, u) {
+            ee(o, e, u), F(e, t), F(e, n), F(e, s);
             for (let a = 0; a < i.length; a += 1)
                 i[a] && i[a].m(s, null);
         },
-        p(f, r) {
-            if (r[0] & /*addToTextbox, suffixes*/
+        p(o, u) {
+            if (u[0] & /*addToTextbox, suffixes*/
                 131584) {
-                o = Ue(
+                f = Ue(
                     /*suffixes*/
-                    f[9]
+                    o[9]
                 );
                 let a;
-                for (a = 0; a < o.length; a += 1) {
-                    const u = Dt(f, o, a);
-                    i[a] ? i[a].p(u, r) : (i[a] = Yt(u), i[a].c(), i[a].m(s, null));
+                for (a = 0; a < f.length; a += 1) {
+                    const r = Nt(o, f, a);
+                    i[a] ? i[a].p(r, u) : (i[a] = Pt(r), i[a].c(), i[a].m(s, null));
                 }
                 for (; a < i.length; a += 1)
                     i[a].d(1);
-                i.length = o.length;
+                i.length = f.length;
             }
         },
-        d(f) {
-            f && $(e), kl(i, f);
+        d(o) {
+            o && $(e), vl(i, o);
         }
     };
 }
 
-function Yt(l) {
+function Pt(l) {
     let e, t, n = (
             /*word*/
             l[47] + ""
         ),
-        s, o, i, f, r, a, u;
+        s, f, i, o, u, a, r;
 
     function _() {
         return (
             /*click_handler_1*/
             l[34](
                 /*word*/
                 l[47]
             )
         );
     }
     return {
         c() {
-            e = B("li"), t = B("button"), s = pt(n), o = te(), i = Ge("svg"), f = Ge("path"), r = te(), g(f, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), g(f, "fill", "#FF9A57"), g(f, "class", "svelte-82ixrs"), g(i, "xmlns", "http://www.w3.org/2000/svg"), g(i, "width", "11"), g(i, "height", "12"), g(i, "viewBox", "0 0 11 12"), g(i, "fill", "none"), g(i, "class", "svelte-82ixrs"), g(t, "class", "text_extension_button svelte-82ixrs"), g(e, "class", "svelte-82ixrs");
+            e = B("li"), t = B("button"), s = pt(n), f = te(), i = Ge("svg"), o = Ge("path"), u = te(), g(o, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), g(o, "fill", "#FF9A57"), g(o, "class", "svelte-lsxp0u"), g(i, "xmlns", "http://www.w3.org/2000/svg"), g(i, "width", "11"), g(i, "height", "12"), g(i, "viewBox", "0 0 11 12"), g(i, "fill", "none"), g(i, "class", "svelte-lsxp0u"), g(t, "class", "text_extension_button svelte-lsxp0u"), g(e, "class", "svelte-lsxp0u");
         },
         m(c, h) {
-            ee(c, e, h), F(e, t), F(t, s), F(t, o), F(t, i), F(i, f), F(e, r), a || (u = E(t, "click", _), a = !0);
+            ee(c, e, h), F(e, t), F(t, s), F(t, f), F(t, i), F(i, o), F(e, u), a || (r = E(t, "click", _), a = !0);
         },
         p(c, h) {
             l = c, h[0] & /*suffixes*/
                 512 && n !== (n = /*word*/
-                    l[47] + "") && kt(s, n);
+                    l[47] + "") && vt(s, n);
         },
         d(c) {
-            c && $(e), a = !1, u();
+            c && $(e), a = !1, r();
         }
     };
 }
 
 function pi(l) {
-    let e, t, n, s, o, i, f;
-    t = new Zn({
+    let e, t, n, s, f, i, o;
+    t = new Fn({
         props: {
             show_label: (
                 /*show_label*/
                 l[6]
             ),
             info: (
                 /*info*/
                 l[4]
             ),
             $$slots: {
-                default: [gi]
+                default: [bi]
             },
             $$scope: {
                 ctx: l
             }
         }
     });
-    const r = [ki, vi, wi],
+    const u = [vi, wi, gi],
         a = [];
 
-    function u(_, c) {
+    function r(_, c) {
         return (
             /*show_menu*/
             _[14] && /*show_magic*/
             _[15] ? 0 : ! /*show_menu*/
             _[14] && /*show_magic*/
             _[15] ? 1 : 2
         );
     }
-    return o = u(l), i = a[o] = r[o](l), {
+    return f = r(l), i = a[f] = u[f](l), {
         c() {
-            e = B("label"), ai(t.$$.fragment), n = te(), s = B("div"), i.c(), g(s, "class", "input-container"), g(e, "class", "svelte-82ixrs"), Bt(
+            e = B("label"), oi(t.$$.fragment), n = te(), s = B("div"), i.c(), g(s, "class", "input-container"), g(e, "class", "svelte-lsxp0u"), Tt(
                 e,
                 "container",
                 /*container*/
                 l[7]
             );
         },
         m(_, c) {
-            ee(_, e, c), ci(t, e, null), F(e, n), F(e, s), a[o].m(s, null), f = !0;
+            ee(_, e, c), _i(t, e, null), F(e, n), F(e, s), a[f].m(s, null), o = !0;
         },
         p(_, c) {
             const h = {};
             c[0] & /*show_label*/
                 64 && (h.show_label = /*show_label*/
                     _[6]), c[0] & /*info*/
                 16 && (h.info = /*info*/
                     _[4]), c[0] & /*label*/
                 8 | c[1] & /*$$scope*/
                 2097152 && (h.$$scope = {
                     dirty: c,
                     ctx: _
                 }), t.$set(h);
-            let L = o;
-            o = u(_), o === L ? a[o].p(_, c) : (ui(), at(a[L], 1, 1, () => {
+            let L = f;
+            f = r(_), f === L ? a[f].p(_, c) : (ui(), at(a[L], 1, 1, () => {
                 a[L] = null;
-            }), fi(), i = a[o], i ? i.p(_, c) : (i = a[o] = r[o](_), i.c()), ft(i, 1), i.m(s, null)), (!f || c[0] & /*container*/
-                128) && Bt(
+            }), fi(), i = a[f], i ? i.p(_, c) : (i = a[f] = u[f](_), i.c()), ot(i, 1), i.m(s, null)), (!o || c[0] & /*container*/
+                128) && Tt(
                 e,
                 "container",
                 /*container*/
                 _[7]
             );
         },
         i(_) {
-            f || (ft(t.$$.fragment, _), ft(i), f = !0);
+            o || (ot(t.$$.fragment, _), ot(i), o = !0);
         },
         o(_) {
-            at(t.$$.fragment, _), at(i), f = !1;
+            at(t.$$.fragment, _), at(i), o = !1;
         },
         d(_) {
-            _ && $(e), ri(t), a[o].d();
+            _ && $(e), ai(t), a[f].d();
         }
     };
 }
 
-function Ci(l, e, t) {
+function ki(l, e, t) {
     var n = this && this.__awaiter || function(d, S, D, A) {
         function me(Te) {
             return Te instanceof D ? Te : new D(function(De) {
                 De(Te);
             });
         }
         return new(D || (D = Promise))(function(Te, De) {
-            function Fl(he) {
+            function ql(he) {
                 try {
                     lt(A.next(he));
                 } catch (nt) {
                     De(nt);
                 }
             }
 
-            function Zl(he) {
+            function Fl(he) {
                 try {
                     lt(A.throw(he));
                 } catch (nt) {
                     De(nt);
                 }
             }
 
             function lt(he) {
-                he.done ? Te(he.value) : me(he.value).then(Fl, Zl);
+                he.done ? Te(he.value) : me(he.value).then(ql, Fl);
             }
             lt((A = A.apply(d, S || [])).next());
         });
     };
     let {
         value: s = ""
     } = e, {
-        value_is_output: o = !1
+        value_is_output: f = !1
     } = e, {
         lines: i = 1
     } = e, {
-        placeholder: f = "Type here..."
+        placeholder: o = "Type here..."
     } = e, {
-        label: r
+        label: u
     } = e, {
         info: a = void 0
     } = e, {
-        disabled: u = !1
+        disabled: r = !1
     } = e, {
         show_label: _ = !0
     } = e, {
         container: c = !0
     } = e, {
         max_lines: h
     } = e, {
         prompts: L = []
     } = e, {
-        suffixes: H = []
+        suffixes: M = []
     } = e, {
-        rtl: p = !1
+        rtl: k = !1
     } = e, {
         autofocus: v = !1
     } = e, {
         text_align: m = void 0
     } = e, {
         autoscroll: b = !0
-    } = e, C, T = !1, k, N = 0, I = !1, ae = L.length > 0 || H.length > 0;
-    const j = bi();
-    mi(() => {
-        k = C && C.offsetHeight + C.scrollTop > C.scrollHeight - 100;
+    } = e, C, T = !1, p, N = 0, I = !1, le = L.length > 0 || M.length > 0;
+    const j = hi();
+    di(() => {
+        p = C && C.offsetHeight + C.scrollTop > C.scrollHeight - 100;
     });
-    const le = () => {
-        k && b && !I && C.scrollTo(0, C.scrollHeight);
+    const ne = () => {
+        p && b && !I && C.scrollTo(0, C.scrollHeight);
     };
 
-    function ne() {
-        j("change", s), o || j("input");
+    function ie() {
+        j("change", s), f || j("input");
     }
-    hi(() => {
-        v && C.focus(), k && b && le(), t(22, o = !1);
+    mi(() => {
+        v && C.focus(), p && b && ne(), t(22, f = !1), t(15, le = L.length > 0 || M.length > 0);
     });
 
     function ge() {
         return n(this, void 0, void 0, function*() {
             t(14, T = !T);
         });
     }
 
     function Y(d) {
         t(0, s += `${d} `);
     }
 
-    function re(d) {
+    function ue(d) {
         const S = d.target,
             D = S.value,
             A = [S.selectionStart, S.selectionEnd];
         j("select", {
             value: D.substring(...A),
             index: A
         });
     }
 
     function O(d) {
         return n(this, void 0, void 0, function*() {
-            yield Nt(), (d.key === "Enter" && d.shiftKey && i > 1 || d.key === "Enter" && !d.shiftKey && i === 1 && h >= 1) && (d.preventDefault(), j("submit"));
+            yield Bt(), (d.key === "Enter" && d.shiftKey && i > 1 || d.key === "Enter" && !d.shiftKey && i === 1 && h >= 1) && (d.preventDefault(), j("submit"));
         });
     }
 
     function we(d) {
         const S = d.target,
             D = S.scrollTop;
         D < N && (I = !0), N = D;
         const A = S.scrollHeight - S.clientHeight;
         D >= A && (I = !1);
     }
 
     function _e(d) {
         return n(this, void 0, void 0, function*() {
-            if (yield Nt(), i === h)
+            if (yield Bt(), i === h)
                 return;
             let S = h === void 0 ? !1 : h === void 0 ? 21 * 11 : 21 * (h + 1),
                 D = 21 * (i + 1);
             const A = d.target;
             A.style.height = "1px";
             let me;
             S && A.scrollHeight > S ? me = S : A.scrollHeight < D ? me = D : me = A.scrollHeight, A.style.height = `${me}px`;
@@ -2304,15 +2294,15 @@
             };
     }
 
     function w(d) {
         He.call(this, l, d);
     }
 
-    function ke(d) {
+    function pe(d) {
         He.call(this, l, d);
     }
 
     function We(d) {
         He.call(this, l, d);
     }
 
@@ -2328,100 +2318,100 @@
         He.call(this, l, d);
     }
 
     function xe() {
         s = this.value, t(0, s);
     }
 
-    function pe(d) {
-        ot[d ? "unshift" : "push"](() => {
+    function ke(d) {
+        ft[d ? "unshift" : "push"](() => {
             C = d, t(13, C);
         });
     }
     const Ce = (d) => Y(d),
         $e = (d) => Y(d);
 
     function de() {
         s = this.value, t(0, s);
     }
 
     function ye(d) {
-        ot[d ? "unshift" : "push"](() => {
+        ft[d ? "unshift" : "push"](() => {
             C = d, t(13, C);
         });
     }
 
     function et() {
         s = this.value, t(0, s);
     }
 
     function tt(d) {
-        ot[d ? "unshift" : "push"](() => {
+        ft[d ? "unshift" : "push"](() => {
             C = d, t(13, C);
         });
     }
     return l.$$set = (d) => {
-        "value" in d && t(0, s = d.value), "value_is_output" in d && t(22, o = d.value_is_output), "lines" in d && t(1, i = d.lines), "placeholder" in d && t(2, f = d.placeholder), "label" in d && t(3, r = d.label), "info" in d && t(4, a = d.info), "disabled" in d && t(5, u = d.disabled), "show_label" in d && t(6, _ = d.show_label), "container" in d && t(7, c = d.container), "max_lines" in d && t(23, h = d.max_lines), "prompts" in d && t(8, L = d.prompts), "suffixes" in d && t(9, H = d.suffixes), "rtl" in d && t(10, p = d.rtl), "autofocus" in d && t(11, v = d.autofocus), "text_align" in d && t(12, m = d.text_align), "autoscroll" in d && t(24, b = d.autoscroll);
+        "value" in d && t(0, s = d.value), "value_is_output" in d && t(22, f = d.value_is_output), "lines" in d && t(1, i = d.lines), "placeholder" in d && t(2, o = d.placeholder), "label" in d && t(3, u = d.label), "info" in d && t(4, a = d.info), "disabled" in d && t(5, r = d.disabled), "show_label" in d && t(6, _ = d.show_label), "container" in d && t(7, c = d.container), "max_lines" in d && t(23, h = d.max_lines), "prompts" in d && t(8, L = d.prompts), "suffixes" in d && t(9, M = d.suffixes), "rtl" in d && t(10, k = d.rtl), "autofocus" in d && t(11, v = d.autofocus), "text_align" in d && t(12, m = d.text_align), "autoscroll" in d && t(24, b = d.autoscroll);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*value*/
             1 && s === null && t(0, s = ""), l.$$.dirty[0] & /*value, el, lines, max_lines*/
             8396803 && C && i !== h && _e({
                 target: C
             }), l.$$.dirty[0] & /*value*/
-            1 && ne();
+            1 && ie();
     }, [
         s,
         i,
-        f,
-        r,
-        a,
+        o,
         u,
+        a,
+        r,
         _,
         c,
         L,
-        H,
-        p,
+        M,
+        k,
         v,
         m,
         C,
         T,
-        ae,
+        le,
         ge,
         Y,
-        re,
+        ue,
         O,
         we,
         ve,
-        o,
+        f,
         h,
         b,
         w,
-        ke,
+        pe,
         We,
         Je,
         Qe,
         y,
         xe,
-        pe,
+        ke,
         Ce,
         $e,
         de,
         ye,
         et,
         tt
     ];
 }
-class yi extends si {
+class Ci extends ii {
     constructor(e) {
-        super(), _i(
+        super(), ri(
             this,
             e,
-            Ci,
+            ki,
             pi,
-            di, {
+            ci, {
                 value: 0,
                 value_is_output: 22,
                 lines: 1,
                 placeholder: 2,
                 label: 3,
                 info: 4,
                 disabled: 5,
@@ -2446,197 +2436,197 @@
         t = 0;
     for (; l > 1e3 && t < e.length - 1;)
         l /= 1e3, t++;
     let n = e[t];
     return (Number.isInteger(l) ? l : l.toFixed(1)) + n;
 }
 const {
-    SvelteComponent: Li,
+    SvelteComponent: yi,
     append: W,
     attr: q,
-    component_subscribe: Kt,
-    detach: Mi,
-    element: Vi,
-    init: Hi,
-    insert: qi,
-    noop: Ot,
-    safe_not_equal: Fi,
+    component_subscribe: Yt,
+    detach: Li,
+    element: Mi,
+    init: Vi,
+    insert: Hi,
+    noop: Kt,
+    safe_not_equal: qi,
     set_style: je,
     svg_element: J,
-    toggle_class: Ut
+    toggle_class: Ot
 } = window.__gradio__svelte__internal, {
-    onMount: Zi
+    onMount: Fi
 } = window.__gradio__svelte__internal;
 
-function Si(l) {
-    let e, t, n, s, o, i, f, r, a, u, _, c;
+function Zi(l) {
+    let e, t, n, s, f, i, o, u, a, r, _, c;
     return {
         c() {
-            e = Vi("div"), t = J("svg"), n = J("g"), s = J("path"), o = J("path"), i = J("path"), f = J("path"), r = J("g"), a = J("path"), u = J("path"), _ = J("path"), c = J("path"), q(s, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(s, "fill", "#FF7C00"), q(s, "fill-opacity", "0.4"), q(s, "class", "svelte-43sxxs"), q(o, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(o, "fill", "#FF7C00"), q(o, "class", "svelte-43sxxs"), q(i, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(f, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(f, "fill", "#FF7C00"), q(f, "class", "svelte-43sxxs"), je(n, "transform", "translate(" + /*$top*/
+            e = Mi("div"), t = J("svg"), n = J("g"), s = J("path"), f = J("path"), i = J("path"), o = J("path"), u = J("g"), a = J("path"), r = J("path"), _ = J("path"), c = J("path"), q(s, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(s, "fill", "#FF7C00"), q(s, "fill-opacity", "0.4"), q(s, "class", "svelte-43sxxs"), q(f, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(f, "fill", "#FF7C00"), q(f, "class", "svelte-43sxxs"), q(i, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(o, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(o, "fill", "#FF7C00"), q(o, "class", "svelte-43sxxs"), je(n, "transform", "translate(" + /*$top*/
                 l[1][0] + "px, " + /*$top*/
-                l[1][1] + "px)"), q(a, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(a, "fill", "#FF7C00"), q(a, "fill-opacity", "0.4"), q(a, "class", "svelte-43sxxs"), q(u, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(u, "fill", "#FF7C00"), q(u, "class", "svelte-43sxxs"), q(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(_, "fill", "#FF7C00"), q(_, "fill-opacity", "0.4"), q(_, "class", "svelte-43sxxs"), q(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(c, "fill", "#FF7C00"), q(c, "class", "svelte-43sxxs"), je(r, "transform", "translate(" + /*$bottom*/
+                l[1][1] + "px)"), q(a, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(a, "fill", "#FF7C00"), q(a, "fill-opacity", "0.4"), q(a, "class", "svelte-43sxxs"), q(r, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(r, "fill", "#FF7C00"), q(r, "class", "svelte-43sxxs"), q(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(_, "fill", "#FF7C00"), q(_, "fill-opacity", "0.4"), q(_, "class", "svelte-43sxxs"), q(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(c, "fill", "#FF7C00"), q(c, "class", "svelte-43sxxs"), je(u, "transform", "translate(" + /*$bottom*/
                 l[2][0] + "px, " + /*$bottom*/
-                l[2][1] + "px)"), q(t, "viewBox", "-1200 -1200 3000 3000"), q(t, "fill", "none"), q(t, "xmlns", "http://www.w3.org/2000/svg"), q(t, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), Ut(
+                l[2][1] + "px)"), q(t, "viewBox", "-1200 -1200 3000 3000"), q(t, "fill", "none"), q(t, "xmlns", "http://www.w3.org/2000/svg"), q(t, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), Ot(
                 e,
                 "margin",
                 /*margin*/
                 l[0]
             );
         },
         m(h, L) {
-            qi(h, e, L), W(e, t), W(t, n), W(n, s), W(n, o), W(n, i), W(n, f), W(t, r), W(r, a), W(r, u), W(r, _), W(r, c);
+            Hi(h, e, L), W(e, t), W(t, n), W(n, s), W(n, f), W(n, i), W(n, o), W(t, u), W(u, a), W(u, r), W(u, _), W(u, c);
         },
         p(h, [L]) {
             L & /*$top*/
                 2 && je(n, "transform", "translate(" + /*$top*/
                     h[1][0] + "px, " + /*$top*/
                     h[1][1] + "px)"), L & /*$bottom*/
-                4 && je(r, "transform", "translate(" + /*$bottom*/
+                4 && je(u, "transform", "translate(" + /*$bottom*/
                     h[2][0] + "px, " + /*$bottom*/
                     h[2][1] + "px)"), L & /*margin*/
-                1 && Ut(
+                1 && Ot(
                     e,
                     "margin",
                     /*margin*/
                     h[0]
                 );
         },
-        i: Ot,
-        o: Ot,
+        i: Kt,
+        o: Kt,
         d(h) {
-            h && Mi(e);
+            h && Li(e);
         }
     };
 }
 
-function zi(l, e, t) {
+function Si(l, e, t) {
     let n, s;
-    var o = this && this.__awaiter || function(h, L, H, p) {
+    var f = this && this.__awaiter || function(h, L, M, k) {
         function v(m) {
-            return m instanceof H ? m : new H(function(b) {
+            return m instanceof M ? m : new M(function(b) {
                 b(m);
             });
         }
-        return new(H || (H = Promise))(function(m, b) {
+        return new(M || (M = Promise))(function(m, b) {
             function C(N) {
                 try {
-                    k(p.next(N));
+                    p(k.next(N));
                 } catch (I) {
                     b(I);
                 }
             }
 
             function T(N) {
                 try {
-                    k(p.throw(N));
+                    p(k.throw(N));
                 } catch (I) {
                     b(I);
                 }
             }
 
-            function k(N) {
+            function p(N) {
                 N.done ? m(N.value) : v(N.value).then(C, T);
             }
-            k((p = p.apply(h, L || [])).next());
+            p((k = k.apply(h, L || [])).next());
         });
     };
     let {
         margin: i = !0
     } = e;
-    const f = zt([0, 0]);
-    Kt(l, f, (h) => t(1, n = h));
-    const r = zt([0, 0]);
-    Kt(l, r, (h) => t(2, s = h));
+    const o = St([0, 0]);
+    Yt(l, o, (h) => t(1, n = h));
+    const u = St([0, 0]);
+    Yt(l, u, (h) => t(2, s = h));
     let a;
 
-    function u() {
-        return o(this, void 0, void 0, function*() {
-            yield Promise.all([f.set([125, 140]), r.set([-125, -140])]), yield Promise.all([f.set([-125, 140]), r.set([125, -140])]), yield Promise.all([f.set([-125, 0]), r.set([125, -0])]), yield Promise.all([f.set([125, 0]), r.set([-125, 0])]);
+    function r() {
+        return f(this, void 0, void 0, function*() {
+            yield Promise.all([o.set([125, 140]), u.set([-125, -140])]), yield Promise.all([o.set([-125, 140]), u.set([125, -140])]), yield Promise.all([o.set([-125, 0]), u.set([125, -0])]), yield Promise.all([o.set([125, 0]), u.set([-125, 0])]);
         });
     }
 
     function _() {
-        return o(this, void 0, void 0, function*() {
-            yield u(), a || _();
+        return f(this, void 0, void 0, function*() {
+            yield r(), a || _();
         });
     }
 
     function c() {
-        return o(this, void 0, void 0, function*() {
-            yield Promise.all([f.set([125, 0]), r.set([-125, 0])]), _();
+        return f(this, void 0, void 0, function*() {
+            yield Promise.all([o.set([125, 0]), u.set([-125, 0])]), _();
         });
     }
-    return Zi(() => (c(), () => a = !0)), l.$$set = (h) => {
+    return Fi(() => (c(), () => a = !0)), l.$$set = (h) => {
         "margin" in h && t(0, i = h.margin);
-    }, [i, n, s, f, r];
+    }, [i, n, s, o, u];
 }
-class Ei extends Li {
+class zi extends yi {
     constructor(e) {
-        super(), Hi(this, e, zi, Si, Fi, {
+        super(), Vi(this, e, Si, Zi, qi, {
             margin: 0
         });
     }
 }
 const {
-    SvelteComponent: Ti,
+    SvelteComponent: Ei,
     append: be,
     attr: x,
-    binding_callbacks: Xt,
+    binding_callbacks: Ut,
     check_outros: dt,
     create_component: pl,
-    create_slot: Cl,
-    destroy_component: yl,
-    destroy_each: Ll,
-    detach: M,
+    create_slot: kl,
+    destroy_component: Cl,
+    destroy_each: yl,
+    detach: V,
     element: oe,
     empty: Ee,
     ensure_array_like: Re,
-    get_all_dirty_from_scope: Ml,
-    get_slot_changes: Vl,
+    get_all_dirty_from_scope: Ll,
+    get_slot_changes: Ml,
     group_outros: mt,
-    init: Bi,
-    insert: V,
-    mount_component: Hl,
+    init: Ti,
+    insert: H,
+    mount_component: Vl,
     noop: ht,
-    safe_not_equal: Ni,
+    safe_not_equal: Bi,
     set_data: G,
     set_style: ce,
     space: X,
     text: z,
     toggle_class: U,
     transition_in: Q,
-    transition_out: fe,
-    update_slot_base: ql
+    transition_out: ae,
+    update_slot_base: Hl
 } = window.__gradio__svelte__internal, {
-    tick: Di
+    tick: Ni
 } = window.__gradio__svelte__internal, {
-    onDestroy: Ii
+    onDestroy: Di
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: ji
-} = window.__gradio__svelte__internal, Ai = (l) => ({}), Gt = (l) => ({}), Pi = (l) => ({}), Rt = (l) => ({});
+    createEventDispatcher: Ii
+} = window.__gradio__svelte__internal, ji = (l) => ({}), Xt = (l) => ({}), Ai = (l) => ({}), Gt = (l) => ({});
 
-function Wt(l, e, t) {
+function Rt(l, e, t) {
     const n = l.slice();
     return n[41] = e[t], n[43] = t, n;
 }
 
-function Jt(l, e, t) {
+function Wt(l, e, t) {
     const n = l.slice();
     return n[41] = e[t], n;
 }
 
-function Yi(l) {
-    let e, t, n, s, o = (
+function Pi(l) {
+    let e, t, n, s, f = (
             /*i18n*/
             l[1]("common.error") + ""
         ),
-        i, f, r;
-    t = new Xn({
+        i, o, u;
+    t = new Un({
         props: {
-            Icon: $n,
+            Icon: xn,
             label: (
                 /*i18n*/
                 l[1]("common.clear")
             ),
             disabled: !1
         }
     }), t.$on(
@@ -2644,771 +2634,771 @@
         /*click_handler*/
         l[32]
     );
     const a = (
             /*#slots*/
             l[30].error
         ),
-        u = Cl(
+        r = kl(
             a,
             l,
             /*$$scope*/
             l[29],
-            Gt
+            Xt
         );
     return {
         c() {
-            e = oe("div"), pl(t.$$.fragment), n = X(), s = oe("span"), i = z(o), f = X(), u && u.c(), x(e, "class", "clear-status svelte-vopvsi"), x(s, "class", "error svelte-vopvsi");
+            e = oe("div"), pl(t.$$.fragment), n = X(), s = oe("span"), i = z(f), o = X(), r && r.c(), x(e, "class", "clear-status svelte-vopvsi"), x(s, "class", "error svelte-vopvsi");
         },
         m(_, c) {
-            V(_, e, c), Hl(t, e, null), V(_, n, c), V(_, s, c), be(s, i), V(_, f, c), u && u.m(_, c), r = !0;
+            H(_, e, c), Vl(t, e, null), H(_, n, c), H(_, s, c), be(s, i), H(_, o, c), r && r.m(_, c), u = !0;
         },
         p(_, c) {
             const h = {};
             c[0] & /*i18n*/
                 2 && (h.label = /*i18n*/
-                    _[1]("common.clear")), t.$set(h), (!r || c[0] & /*i18n*/
-                    2) && o !== (o = /*i18n*/
-                    _[1]("common.error") + "") && G(i, o), u && u.p && (!r || c[0] & /*$$scope*/
-                    536870912) && ql(
-                    u,
+                    _[1]("common.clear")), t.$set(h), (!u || c[0] & /*i18n*/
+                    2) && f !== (f = /*i18n*/
+                    _[1]("common.error") + "") && G(i, f), r && r.p && (!u || c[0] & /*$$scope*/
+                    536870912) && Hl(
+                    r,
                     a,
                     _,
                     /*$$scope*/
                     _[29],
-                    r ? Vl(
+                    u ? Ml(
                         a,
                         /*$$scope*/
                         _[29],
                         c,
-                        Ai
-                    ) : Ml(
+                        ji
+                    ) : Ll(
                         /*$$scope*/
                         _[29]
                     ),
-                    Gt
+                    Xt
                 );
         },
         i(_) {
-            r || (Q(t.$$.fragment, _), Q(u, _), r = !0);
+            u || (Q(t.$$.fragment, _), Q(r, _), u = !0);
         },
         o(_) {
-            fe(t.$$.fragment, _), fe(u, _), r = !1;
+            ae(t.$$.fragment, _), ae(r, _), u = !1;
         },
         d(_) {
-            _ && (M(e), M(n), M(s), M(f)), yl(t), u && u.d(_);
+            _ && (V(e), V(n), V(s), V(o)), Cl(t), r && r.d(_);
         }
     };
 }
 
-function Ki(l) {
-    let e, t, n, s, o, i, f, r, a, u = (
+function Yi(l) {
+    let e, t, n, s, f, i, o, u, a, r = (
         /*variant*/
         l[8] === "default" && /*show_eta_bar*/
         l[18] && /*show_progress*/
-        l[6] === "full" && Qt(l)
+        l[6] === "full" && Jt(l)
     );
 
     function _(b, C) {
         if (
             /*progress*/
             b[7]
         )
-            return Xi;
+            return Ui;
         if (
             /*queue_position*/
             b[2] !== null && /*queue_size*/
             b[3] !== void 0 && /*queue_position*/
             b[2] >= 0
         )
-            return Ui;
+            return Oi;
         if (
             /*queue_position*/
             b[2] === 0
         )
-            return Oi;
+            return Ki;
     }
     let c = _(l),
         h = c && c(l),
         L = (
             /*timer*/
-            l[5] && el(l)
+            l[5] && $t(l)
         );
-    const H = [Ji, Wi],
-        p = [];
+    const M = [Wi, Ri],
+        k = [];
 
     function v(b, C) {
         return (
             /*last_progress_level*/
             b[15] != null ? 0 : (
                 /*show_progress*/
                 b[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(o = v(l)) && (i = p[o] = H[o](l));
+    ~(f = v(l)) && (i = k[f] = M[f](l));
     let m = ! /*timer*/
         l[5] && fl(l);
     return {
         c() {
-            u && u.c(), e = X(), t = oe("div"), h && h.c(), n = X(), L && L.c(), s = X(), i && i.c(), f = X(), m && m.c(), r = Ee(), x(t, "class", "progress-text svelte-vopvsi"), U(
+            r && r.c(), e = X(), t = oe("div"), h && h.c(), n = X(), L && L.c(), s = X(), i && i.c(), o = X(), m && m.c(), u = Ee(), x(t, "class", "progress-text svelte-vopvsi"), U(
                 t,
                 "meta-text-center",
                 /*variant*/
                 l[8] === "center"
             ), U(
                 t,
                 "meta-text",
                 /*variant*/
                 l[8] === "default"
             );
         },
         m(b, C) {
-            u && u.m(b, C), V(b, e, C), V(b, t, C), h && h.m(t, null), be(t, n), L && L.m(t, null), V(b, s, C), ~o && p[o].m(b, C), V(b, f, C), m && m.m(b, C), V(b, r, C), a = !0;
+            r && r.m(b, C), H(b, e, C), H(b, t, C), h && h.m(t, null), be(t, n), L && L.m(t, null), H(b, s, C), ~f && k[f].m(b, C), H(b, o, C), m && m.m(b, C), H(b, u, C), a = !0;
         },
         p(b, C) {
             /*variant*/
             b[8] === "default" && /*show_eta_bar*/
                 b[18] && /*show_progress*/
-                b[6] === "full" ? u ? u.p(b, C) : (u = Qt(b), u.c(), u.m(e.parentNode, e)) : u && (u.d(1), u = null), c === (c = _(b)) && h ? h.p(b, C) : (h && h.d(1), h = c && c(b), h && (h.c(), h.m(t, n))), /*timer*/
-                b[5] ? L ? L.p(b, C) : (L = el(b), L.c(), L.m(t, null)) : L && (L.d(1), L = null), (!a || C[0] & /*variant*/
+                b[6] === "full" ? r ? r.p(b, C) : (r = Jt(b), r.c(), r.m(e.parentNode, e)) : r && (r.d(1), r = null), c === (c = _(b)) && h ? h.p(b, C) : (h && h.d(1), h = c && c(b), h && (h.c(), h.m(t, n))), /*timer*/
+                b[5] ? L ? L.p(b, C) : (L = $t(b), L.c(), L.m(t, null)) : L && (L.d(1), L = null), (!a || C[0] & /*variant*/
                     256) && U(
                     t,
                     "meta-text-center",
                     /*variant*/
                     b[8] === "center"
                 ), (!a || C[0] & /*variant*/
                     256) && U(
                     t,
                     "meta-text",
                     /*variant*/
                     b[8] === "default"
                 );
-            let T = o;
-            o = v(b), o === T ? ~o && p[o].p(b, C) : (i && (mt(), fe(p[T], 1, 1, () => {
-                    p[T] = null;
-                }), dt()), ~o ? (i = p[o], i ? i.p(b, C) : (i = p[o] = H[o](b), i.c()), Q(i, 1), i.m(f.parentNode, f)) : i = null), /*timer*/
-                b[5] ? m && (mt(), fe(m, 1, 1, () => {
+            let T = f;
+            f = v(b), f === T ? ~f && k[f].p(b, C) : (i && (mt(), ae(k[T], 1, 1, () => {
+                    k[T] = null;
+                }), dt()), ~f ? (i = k[f], i ? i.p(b, C) : (i = k[f] = M[f](b), i.c()), Q(i, 1), i.m(o.parentNode, o)) : i = null), /*timer*/
+                b[5] ? m && (mt(), ae(m, 1, 1, () => {
                     m = null;
                 }), dt()) : m ? (m.p(b, C), C[0] & /*timer*/
-                    32 && Q(m, 1)) : (m = fl(b), m.c(), Q(m, 1), m.m(r.parentNode, r));
+                    32 && Q(m, 1)) : (m = fl(b), m.c(), Q(m, 1), m.m(u.parentNode, u));
         },
         i(b) {
             a || (Q(i), Q(m), a = !0);
         },
         o(b) {
-            fe(i), fe(m), a = !1;
+            ae(i), ae(m), a = !1;
         },
         d(b) {
-            b && (M(e), M(t), M(s), M(f), M(r)), u && u.d(b), h && h.d(), L && L.d(), ~o && p[o].d(b), m && m.d(b);
+            b && (V(e), V(t), V(s), V(o), V(u)), r && r.d(b), h && h.d(), L && L.d(), ~f && k[f].d(b), m && m.d(b);
         }
     };
 }
 
-function Qt(l) {
+function Jt(l) {
     let e, t = `translateX(${/*eta_level*/
   (l[17] || 0) * 100 - 100}%)`;
     return {
         c() {
             e = oe("div"), x(e, "class", "eta-bar svelte-vopvsi"), ce(e, "transform", t);
         },
         m(n, s) {
-            V(n, e, s);
+            H(n, e, s);
         },
         p(n, s) {
             s[0] & /*eta_level*/
                 131072 && t !== (t = `translateX(${/*eta_level*/
       (n[17] || 0) * 100 - 100}%)`) && ce(e, "transform", t);
         },
         d(n) {
-            n && M(e);
+            n && V(e);
         }
     };
 }
 
-function Oi(l) {
+function Ki(l) {
     let e;
     return {
         c() {
             e = z("processing |");
         },
         m(t, n) {
-            V(t, e, n);
+            H(t, e, n);
         },
         p: ht,
         d(t) {
-            t && M(e);
+            t && V(e);
         }
     };
 }
 
-function Ui(l) {
+function Oi(l) {
     let e, t = (
             /*queue_position*/
             l[2] + 1 + ""
         ),
-        n, s, o, i;
+        n, s, f, i;
     return {
         c() {
-            e = z("queue: "), n = z(t), s = z("/"), o = z(
+            e = z("queue: "), n = z(t), s = z("/"), f = z(
                 /*queue_size*/
                 l[3]
             ), i = z(" |");
         },
-        m(f, r) {
-            V(f, e, r), V(f, n, r), V(f, s, r), V(f, o, r), V(f, i, r);
+        m(o, u) {
+            H(o, e, u), H(o, n, u), H(o, s, u), H(o, f, u), H(o, i, u);
         },
-        p(f, r) {
-            r[0] & /*queue_position*/
+        p(o, u) {
+            u[0] & /*queue_position*/
                 4 && t !== (t = /*queue_position*/
-                    f[2] + 1 + "") && G(n, t), r[0] & /*queue_size*/
+                    o[2] + 1 + "") && G(n, t), u[0] & /*queue_size*/
                 8 && G(
-                    o,
+                    f,
                     /*queue_size*/
-                    f[3]
+                    o[3]
                 );
         },
-        d(f) {
-            f && (M(e), M(n), M(s), M(o), M(i));
+        d(o) {
+            o && (V(e), V(n), V(s), V(f), V(i));
         }
     };
 }
 
-function Xi(l) {
+function Ui(l) {
     let e, t = Re(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let s = 0; s < t.length; s += 1)
-        n[s] = $t(Jt(l, t, s));
+        n[s] = xt(Wt(l, t, s));
     return {
         c() {
             for (let s = 0; s < n.length; s += 1)
                 n[s].c();
             e = Ee();
         },
-        m(s, o) {
+        m(s, f) {
             for (let i = 0; i < n.length; i += 1)
-                n[i] && n[i].m(s, o);
-            V(s, e, o);
+                n[i] && n[i].m(s, f);
+            H(s, e, f);
         },
-        p(s, o) {
-            if (o[0] & /*progress*/
+        p(s, f) {
+            if (f[0] & /*progress*/
                 128) {
                 t = Re(
                     /*progress*/
                     s[7]
                 );
                 let i;
                 for (i = 0; i < t.length; i += 1) {
-                    const f = Jt(s, t, i);
-                    n[i] ? n[i].p(f, o) : (n[i] = $t(f), n[i].c(), n[i].m(e.parentNode, e));
+                    const o = Wt(s, t, i);
+                    n[i] ? n[i].p(o, f) : (n[i] = xt(o), n[i].c(), n[i].m(e.parentNode, e));
                 }
                 for (; i < n.length; i += 1)
                     n[i].d(1);
                 n.length = t.length;
             }
         },
         d(s) {
-            s && M(e), Ll(n, s);
+            s && V(e), yl(n, s);
         }
     };
 }
 
-function xt(l) {
+function Qt(l) {
     let e, t = (
             /*p*/
             l[41].unit + ""
         ),
-        n, s, o = " ",
+        n, s, f = " ",
         i;
 
-    function f(u, _) {
+    function o(r, _) {
         return (
             /*p*/
-            u[41].length != null ? Ri : Gi
+            r[41].length != null ? Gi : Xi
         );
     }
-    let r = f(l),
-        a = r(l);
+    let u = o(l),
+        a = u(l);
     return {
         c() {
-            a.c(), e = X(), n = z(t), s = z(" | "), i = z(o);
+            a.c(), e = X(), n = z(t), s = z(" | "), i = z(f);
         },
-        m(u, _) {
-            a.m(u, _), V(u, e, _), V(u, n, _), V(u, s, _), V(u, i, _);
+        m(r, _) {
+            a.m(r, _), H(r, e, _), H(r, n, _), H(r, s, _), H(r, i, _);
         },
-        p(u, _) {
-            r === (r = f(u)) && a ? a.p(u, _) : (a.d(1), a = r(u), a && (a.c(), a.m(e.parentNode, e))), _[0] & /*progress*/
+        p(r, _) {
+            u === (u = o(r)) && a ? a.p(r, _) : (a.d(1), a = u(r), a && (a.c(), a.m(e.parentNode, e))), _[0] & /*progress*/
                 128 && t !== (t = /*p*/
-                    u[41].unit + "") && G(n, t);
+                    r[41].unit + "") && G(n, t);
         },
-        d(u) {
-            u && (M(e), M(n), M(s), M(i)), a.d(u);
+        d(r) {
+            r && (V(e), V(n), V(s), V(i)), a.d(r);
         }
     };
 }
 
-function Gi(l) {
+function Xi(l) {
     let e = Fe(
             /*p*/
             l[41].index || 0
         ) + "",
         t;
     return {
         c() {
             t = z(e);
         },
         m(n, s) {
-            V(n, t, s);
+            H(n, t, s);
         },
         p(n, s) {
             s[0] & /*progress*/
                 128 && e !== (e = Fe(
                     /*p*/
                     n[41].index || 0
                 ) + "") && G(t, e);
         },
         d(n) {
-            n && M(t);
+            n && V(t);
         }
     };
 }
 
-function Ri(l) {
+function Gi(l) {
     let e = Fe(
             /*p*/
             l[41].index || 0
         ) + "",
         t, n, s = Fe(
             /*p*/
             l[41].length
         ) + "",
-        o;
+        f;
     return {
         c() {
-            t = z(e), n = z("/"), o = z(s);
+            t = z(e), n = z("/"), f = z(s);
         },
-        m(i, f) {
-            V(i, t, f), V(i, n, f), V(i, o, f);
+        m(i, o) {
+            H(i, t, o), H(i, n, o), H(i, f, o);
         },
-        p(i, f) {
-            f[0] & /*progress*/
+        p(i, o) {
+            o[0] & /*progress*/
                 128 && e !== (e = Fe(
                     /*p*/
                     i[41].index || 0
-                ) + "") && G(t, e), f[0] & /*progress*/
+                ) + "") && G(t, e), o[0] & /*progress*/
                 128 && s !== (s = Fe(
                     /*p*/
                     i[41].length
-                ) + "") && G(o, s);
+                ) + "") && G(f, s);
         },
         d(i) {
-            i && (M(t), M(n), M(o));
+            i && (V(t), V(n), V(f));
         }
     };
 }
 
-function $t(l) {
+function xt(l) {
     let e, t = (
         /*p*/
-        l[41].index != null && xt(l)
+        l[41].index != null && Qt(l)
     );
     return {
         c() {
             t && t.c(), e = Ee();
         },
         m(n, s) {
-            t && t.m(n, s), V(n, e, s);
+            t && t.m(n, s), H(n, e, s);
         },
         p(n, s) {
             /*p*/
-            n[41].index != null ? t ? t.p(n, s) : (t = xt(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+            n[41].index != null ? t ? t.p(n, s) : (t = Qt(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && M(e), t && t.d(n);
+            n && V(e), t && t.d(n);
         }
     };
 }
 
-function el(l) {
+function $t(l) {
     let e, t = (
             /*eta*/
             l[0] ? `/${/*formatted_eta*/
     l[19]}` : ""
         ),
         n, s;
     return {
         c() {
             e = z(
                 /*formatted_timer*/
                 l[20]
             ), n = z(t), s = z("s");
         },
-        m(o, i) {
-            V(o, e, i), V(o, n, i), V(o, s, i);
+        m(f, i) {
+            H(f, e, i), H(f, n, i), H(f, s, i);
         },
-        p(o, i) {
+        p(f, i) {
             i[0] & /*formatted_timer*/
                 1048576 && G(
                     e,
                     /*formatted_timer*/
-                    o[20]
+                    f[20]
                 ), i[0] & /*eta, formatted_eta*/
                 524289 && t !== (t = /*eta*/
-                    o[0] ? `/${/*formatted_eta*/
-      o[19]}` : "") && G(n, t);
+                    f[0] ? `/${/*formatted_eta*/
+      f[19]}` : "") && G(n, t);
         },
-        d(o) {
-            o && (M(e), M(n), M(s));
+        d(f) {
+            f && (V(e), V(n), V(s));
         }
     };
 }
 
-function Wi(l) {
+function Ri(l) {
     let e, t;
-    return e = new Ei({
+    return e = new zi({
         props: {
             margin: (
                 /*variant*/
                 l[8] === "default"
             )
         }
     }), {
         c() {
             pl(e.$$.fragment);
         },
         m(n, s) {
-            Hl(e, n, s), t = !0;
+            Vl(e, n, s), t = !0;
         },
         p(n, s) {
-            const o = {};
+            const f = {};
             s[0] & /*variant*/
-                256 && (o.margin = /*variant*/
-                    n[8] === "default"), e.$set(o);
+                256 && (f.margin = /*variant*/
+                    n[8] === "default"), e.$set(f);
         },
         i(n) {
             t || (Q(e.$$.fragment, n), t = !0);
         },
         o(n) {
-            fe(e.$$.fragment, n), t = !1;
+            ae(e.$$.fragment, n), t = !1;
         },
         d(n) {
-            yl(e, n);
+            Cl(e, n);
         }
     };
 }
 
-function Ji(l) {
-    let e, t, n, s, o, i = `${/*last_progress_level*/
+function Wi(l) {
+    let e, t, n, s, f, i = `${/*last_progress_level*/
   l[15] * 100}%`,
-        f = (
+        o = (
             /*progress*/
-            l[7] != null && tl(l)
+            l[7] != null && el(l)
         );
     return {
         c() {
-            e = oe("div"), t = oe("div"), f && f.c(), n = X(), s = oe("div"), o = oe("div"), x(t, "class", "progress-level-inner svelte-vopvsi"), x(o, "class", "progress-bar svelte-vopvsi"), ce(o, "width", i), x(s, "class", "progress-bar-wrap svelte-vopvsi"), x(e, "class", "progress-level svelte-vopvsi");
+            e = oe("div"), t = oe("div"), o && o.c(), n = X(), s = oe("div"), f = oe("div"), x(t, "class", "progress-level-inner svelte-vopvsi"), x(f, "class", "progress-bar svelte-vopvsi"), ce(f, "width", i), x(s, "class", "progress-bar-wrap svelte-vopvsi"), x(e, "class", "progress-level svelte-vopvsi");
         },
-        m(r, a) {
-            V(r, e, a), be(e, t), f && f.m(t, null), be(e, n), be(e, s), be(s, o), l[31](o);
+        m(u, a) {
+            H(u, e, a), be(e, t), o && o.m(t, null), be(e, n), be(e, s), be(s, f), l[31](f);
         },
-        p(r, a) {
+        p(u, a) {
             /*progress*/
-            r[7] != null ? f ? f.p(r, a) : (f = tl(r), f.c(), f.m(t, null)) : f && (f.d(1), f = null), a[0] & /*last_progress_level*/
+            u[7] != null ? o ? o.p(u, a) : (o = el(u), o.c(), o.m(t, null)) : o && (o.d(1), o = null), a[0] & /*last_progress_level*/
                 32768 && i !== (i = `${/*last_progress_level*/
-      r[15] * 100}%`) && ce(o, "width", i);
+      u[15] * 100}%`) && ce(f, "width", i);
         },
         i: ht,
         o: ht,
-        d(r) {
-            r && M(e), f && f.d(), l[31](null);
+        d(u) {
+            u && V(e), o && o.d(), l[31](null);
         }
     };
 }
 
-function tl(l) {
+function el(l) {
     let e, t = Re(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let s = 0; s < t.length; s += 1)
-        n[s] = ol(Wt(l, t, s));
+        n[s] = sl(Rt(l, t, s));
     return {
         c() {
             for (let s = 0; s < n.length; s += 1)
                 n[s].c();
             e = Ee();
         },
-        m(s, o) {
+        m(s, f) {
             for (let i = 0; i < n.length; i += 1)
-                n[i] && n[i].m(s, o);
-            V(s, e, o);
+                n[i] && n[i].m(s, f);
+            H(s, e, f);
         },
-        p(s, o) {
-            if (o[0] & /*progress_level, progress*/
+        p(s, f) {
+            if (f[0] & /*progress_level, progress*/
                 16512) {
                 t = Re(
                     /*progress*/
                     s[7]
                 );
                 let i;
                 for (i = 0; i < t.length; i += 1) {
-                    const f = Wt(s, t, i);
-                    n[i] ? n[i].p(f, o) : (n[i] = ol(f), n[i].c(), n[i].m(e.parentNode, e));
+                    const o = Rt(s, t, i);
+                    n[i] ? n[i].p(o, f) : (n[i] = sl(o), n[i].c(), n[i].m(e.parentNode, e));
                 }
                 for (; i < n.length; i += 1)
                     n[i].d(1);
                 n.length = t.length;
             }
         },
         d(s) {
-            s && M(e), Ll(n, s);
+            s && V(e), yl(n, s);
         }
     };
 }
 
-function ll(l) {
-    let e, t, n, s, o = (
+function tl(l) {
+    let e, t, n, s, f = (
             /*i*/
-            l[43] !== 0 && Qi()
+            l[43] !== 0 && Ji()
         ),
         i = (
             /*p*/
-            l[41].desc != null && nl(l)
+            l[41].desc != null && ll(l)
         ),
-        f = (
+        o = (
             /*p*/
             l[41].desc != null && /*progress_level*/
             l[14] && /*progress_level*/
             l[14][
                 /*i*/
                 l[43]
-            ] != null && il()
+            ] != null && nl()
         ),
-        r = (
+        u = (
             /*progress_level*/
-            l[14] != null && sl(l)
+            l[14] != null && il(l)
         );
     return {
         c() {
-            o && o.c(), e = X(), i && i.c(), t = X(), f && f.c(), n = X(), r && r.c(), s = Ee();
+            f && f.c(), e = X(), i && i.c(), t = X(), o && o.c(), n = X(), u && u.c(), s = Ee();
         },
-        m(a, u) {
-            o && o.m(a, u), V(a, e, u), i && i.m(a, u), V(a, t, u), f && f.m(a, u), V(a, n, u), r && r.m(a, u), V(a, s, u);
+        m(a, r) {
+            f && f.m(a, r), H(a, e, r), i && i.m(a, r), H(a, t, r), o && o.m(a, r), H(a, n, r), u && u.m(a, r), H(a, s, r);
         },
-        p(a, u) {
+        p(a, r) {
             /*p*/
-            a[41].desc != null ? i ? i.p(a, u) : (i = nl(a), i.c(), i.m(t.parentNode, t)) : i && (i.d(1), i = null), /*p*/
+            a[41].desc != null ? i ? i.p(a, r) : (i = ll(a), i.c(), i.m(t.parentNode, t)) : i && (i.d(1), i = null), /*p*/
                 a[41].desc != null && /*progress_level*/
                 a[14] && /*progress_level*/
                 a[14][
                     /*i*/
                     a[43]
-                ] != null ? f || (f = il(), f.c(), f.m(n.parentNode, n)) : f && (f.d(1), f = null), /*progress_level*/
-                a[14] != null ? r ? r.p(a, u) : (r = sl(a), r.c(), r.m(s.parentNode, s)) : r && (r.d(1), r = null);
+                ] != null ? o || (o = nl(), o.c(), o.m(n.parentNode, n)) : o && (o.d(1), o = null), /*progress_level*/
+                a[14] != null ? u ? u.p(a, r) : (u = il(a), u.c(), u.m(s.parentNode, s)) : u && (u.d(1), u = null);
         },
         d(a) {
-            a && (M(e), M(t), M(n), M(s)), o && o.d(a), i && i.d(a), f && f.d(a), r && r.d(a);
+            a && (V(e), V(t), V(n), V(s)), f && f.d(a), i && i.d(a), o && o.d(a), u && u.d(a);
         }
     };
 }
 
-function Qi(l) {
+function Ji(l) {
     let e;
     return {
         c() {
             e = z(" /");
         },
         m(t, n) {
-            V(t, e, n);
+            H(t, e, n);
         },
         d(t) {
-            t && M(e);
+            t && V(e);
         }
     };
 }
 
-function nl(l) {
+function ll(l) {
     let e = (
             /*p*/
             l[41].desc + ""
         ),
         t;
     return {
         c() {
             t = z(e);
         },
         m(n, s) {
-            V(n, t, s);
+            H(n, t, s);
         },
         p(n, s) {
             s[0] & /*progress*/
                 128 && e !== (e = /*p*/
                     n[41].desc + "") && G(t, e);
         },
         d(n) {
-            n && M(t);
+            n && V(t);
         }
     };
 }
 
-function il(l) {
+function nl(l) {
     let e;
     return {
         c() {
             e = z("-");
         },
         m(t, n) {
-            V(t, e, n);
+            H(t, e, n);
         },
         d(t) {
-            t && M(e);
+            t && V(e);
         }
     };
 }
 
-function sl(l) {
+function il(l) {
     let e = (100 * /*progress_level*/
             (l[14][
                 /*i*/
                 l[43]
             ] || 0)).toFixed(1) + "",
         t, n;
     return {
         c() {
             t = z(e), n = z("%");
         },
-        m(s, o) {
-            V(s, t, o), V(s, n, o);
+        m(s, f) {
+            H(s, t, f), H(s, n, f);
         },
-        p(s, o) {
-            o[0] & /*progress_level*/
+        p(s, f) {
+            f[0] & /*progress_level*/
                 16384 && e !== (e = (100 * /*progress_level*/
                     (s[14][
                         /*i*/
                         s[43]
                     ] || 0)).toFixed(1) + "") && G(t, e);
         },
         d(s) {
-            s && (M(t), M(n));
+            s && (V(t), V(n));
         }
     };
 }
 
-function ol(l) {
+function sl(l) {
     let e, t = (
         /*p*/
         (l[41].desc != null || /*progress_level*/
             l[14] && /*progress_level*/
             l[14][
                 /*i*/
                 l[43]
-            ] != null) && ll(l)
+            ] != null) && tl(l)
     );
     return {
         c() {
             t && t.c(), e = Ee();
         },
         m(n, s) {
-            t && t.m(n, s), V(n, e, s);
+            t && t.m(n, s), H(n, e, s);
         },
         p(n, s) {
             /*p*/
             n[41].desc != null || /*progress_level*/
                 n[14] && /*progress_level*/
                 n[14][
                     /*i*/
                     n[43]
-                ] != null ? t ? t.p(n, s) : (t = ll(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+                ] != null ? t ? t.p(n, s) : (t = tl(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && M(e), t && t.d(n);
+            n && V(e), t && t.d(n);
         }
     };
 }
 
 function fl(l) {
     let e, t, n, s;
-    const o = (
+    const f = (
             /*#slots*/
             l[30]["additional-loading-text"]
         ),
-        i = Cl(
-            o,
+        i = kl(
+            f,
             l,
             /*$$scope*/
             l[29],
-            Rt
+            Gt
         );
     return {
         c() {
             e = oe("p"), t = z(
                 /*loading_text*/
                 l[9]
             ), n = X(), i && i.c(), x(e, "class", "loading svelte-vopvsi");
         },
-        m(f, r) {
-            V(f, e, r), be(e, t), V(f, n, r), i && i.m(f, r), s = !0;
+        m(o, u) {
+            H(o, e, u), be(e, t), H(o, n, u), i && i.m(o, u), s = !0;
         },
-        p(f, r) {
-            (!s || r[0] & /*loading_text*/
+        p(o, u) {
+            (!s || u[0] & /*loading_text*/
                 512) && G(
                 t,
                 /*loading_text*/
-                f[9]
-            ), i && i.p && (!s || r[0] & /*$$scope*/
-                536870912) && ql(
+                o[9]
+            ), i && i.p && (!s || u[0] & /*$$scope*/
+                536870912) && Hl(
                 i,
-                o,
                 f,
+                o,
                 /*$$scope*/
-                f[29],
-                s ? Vl(
-                    o,
+                o[29],
+                s ? Ml(
+                    f,
                     /*$$scope*/
-                    f[29],
-                    r,
-                    Pi
-                ) : Ml(
+                    o[29],
+                    u,
+                    Ai
+                ) : Ll(
                     /*$$scope*/
-                    f[29]
+                    o[29]
                 ),
-                Rt
+                Gt
             );
         },
-        i(f) {
-            s || (Q(i, f), s = !0);
+        i(o) {
+            s || (Q(i, o), s = !0);
         },
-        o(f) {
-            fe(i, f), s = !1;
+        o(o) {
+            ae(i, o), s = !1;
         },
-        d(f) {
-            f && (M(e), M(n)), i && i.d(f);
+        d(o) {
+            o && (V(e), V(n)), i && i.d(o);
         }
     };
 }
 
-function xi(l) {
-    let e, t, n, s, o;
-    const i = [Ki, Yi],
-        f = [];
+function Qi(l) {
+    let e, t, n, s, f;
+    const i = [Yi, Pi],
+        o = [];
 
-    function r(a, u) {
+    function u(a, r) {
         return (
             /*status*/
             a[4] === "pending" ? 0 : (
                 /*status*/
                 a[4] === "error" ? 1 : -1
             )
         );
     }
-    return ~(t = r(l)) && (n = f[t] = i[t](l)), {
+    return ~(t = u(l)) && (n = o[t] = i[t](l)), {
         c() {
             e = oe("div"), n && n.c(), x(e, "class", s = "wrap " + /*variant*/
                 l[8] + " " + /*show_progress*/
                 l[6] + " svelte-vopvsi"), U(e, "hide", ! /*status*/
                 l[4] || /*status*/
                 l[4] === "complete" || /*show_progress*/
                 l[6] === "hidden"), U(
@@ -3438,263 +3428,263 @@
             ), ce(
                 e,
                 "padding",
                 /*absolute*/
                 l[10] ? "0" : "var(--size-8) 0"
             );
         },
-        m(a, u) {
-            V(a, e, u), ~t && f[t].m(e, null), l[33](e), o = !0;
+        m(a, r) {
+            H(a, e, r), ~t && o[t].m(e, null), l[33](e), f = !0;
         },
-        p(a, u) {
+        p(a, r) {
             let _ = t;
-            t = r(a), t === _ ? ~t && f[t].p(a, u) : (n && (mt(), fe(f[_], 1, 1, () => {
-                    f[_] = null;
-                }), dt()), ~t ? (n = f[t], n ? n.p(a, u) : (n = f[t] = i[t](a), n.c()), Q(n, 1), n.m(e, null)) : n = null), (!o || u[0] & /*variant, show_progress*/
+            t = u(a), t === _ ? ~t && o[t].p(a, r) : (n && (mt(), ae(o[_], 1, 1, () => {
+                    o[_] = null;
+                }), dt()), ~t ? (n = o[t], n ? n.p(a, r) : (n = o[t] = i[t](a), n.c()), Q(n, 1), n.m(e, null)) : n = null), (!f || r[0] & /*variant, show_progress*/
                     320 && s !== (s = "wrap " + /*variant*/
                         a[8] + " " + /*show_progress*/
-                        a[6] + " svelte-vopvsi")) && x(e, "class", s), (!o || u[0] & /*variant, show_progress, status, show_progress*/
+                        a[6] + " svelte-vopvsi")) && x(e, "class", s), (!f || r[0] & /*variant, show_progress, status, show_progress*/
                     336) && U(e, "hide", ! /*status*/
                     a[4] || /*status*/
                     a[4] === "complete" || /*show_progress*/
-                    a[6] === "hidden"), (!o || u[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
+                    a[6] === "hidden"), (!f || r[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
                     2384) && U(
                     e,
                     "translucent",
                     /*variant*/
                     a[8] === "center" && /*status*/
                     (a[4] === "pending" || /*status*/
                         a[4] === "error") || /*translucent*/
                     a[11] || /*show_progress*/
                     a[6] === "minimal"
-                ), (!o || u[0] & /*variant, show_progress, status*/
+                ), (!f || r[0] & /*variant, show_progress, status*/
                     336) && U(
                     e,
                     "generating",
                     /*status*/
                     a[4] === "generating"
-                ), (!o || u[0] & /*variant, show_progress, border*/
+                ), (!f || r[0] & /*variant, show_progress, border*/
                     4416) && U(
                     e,
                     "border",
                     /*border*/
                     a[12]
-                ), u[0] & /*absolute*/
+                ), r[0] & /*absolute*/
                 1024 && ce(
                     e,
                     "position",
                     /*absolute*/
                     a[10] ? "absolute" : "static"
-                ), u[0] & /*absolute*/
+                ), r[0] & /*absolute*/
                 1024 && ce(
                     e,
                     "padding",
                     /*absolute*/
                     a[10] ? "0" : "var(--size-8) 0"
                 );
         },
         i(a) {
-            o || (Q(n), o = !0);
+            f || (Q(n), f = !0);
         },
         o(a) {
-            fe(n), o = !1;
+            ae(n), f = !1;
         },
         d(a) {
-            a && M(e), ~t && f[t].d(), l[33](null);
+            a && V(e), ~t && o[t].d(), l[33](null);
         }
     };
 }
-var $i = function(l, e, t, n) {
-    function s(o) {
-        return o instanceof t ? o : new t(function(i) {
-            i(o);
+var xi = function(l, e, t, n) {
+    function s(f) {
+        return f instanceof t ? f : new t(function(i) {
+            i(f);
         });
     }
-    return new(t || (t = Promise))(function(o, i) {
-        function f(u) {
+    return new(t || (t = Promise))(function(f, i) {
+        function o(r) {
             try {
-                a(n.next(u));
+                a(n.next(r));
             } catch (_) {
                 i(_);
             }
         }
 
-        function r(u) {
+        function u(r) {
             try {
-                a(n.throw(u));
+                a(n.throw(r));
             } catch (_) {
                 i(_);
             }
         }
 
-        function a(u) {
-            u.done ? o(u.value) : s(u.value).then(f, r);
+        function a(r) {
+            r.done ? f(r.value) : s(r.value).then(o, u);
         }
         a((n = n.apply(l, e || [])).next());
     });
 };
 let Ae = [],
-    rt = !1;
+    ut = !1;
 
-function es(l) {
-    return $i(this, arguments, void 0, function*(e, t = !0) {
+function $i(l) {
+    return xi(this, arguments, void 0, function*(e, t = !0) {
         if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && t !== !0)) {
-            if (Ae.push(e), !rt)
-                rt = !0;
+            if (Ae.push(e), !ut)
+                ut = !0;
             else
                 return;
-            yield Di(), requestAnimationFrame(() => {
+            yield Ni(), requestAnimationFrame(() => {
                 let n = [0, 0];
                 for (let s = 0; s < Ae.length; s++) {
                     const i = Ae[s].getBoundingClientRect();
                     (s === 0 || i.top + window.scrollY <= n[0]) && (n[0] = i.top + window.scrollY, n[1] = s);
                 }
                 window.scrollTo({
                     top: n[0] - 20,
                     behavior: "smooth"
-                }), rt = !1, Ae = [];
+                }), ut = !1, Ae = [];
             });
         }
     });
 }
 
-function ts(l, e, t) {
+function es(l, e, t) {
     let n, {
         $$slots: s = {},
-        $$scope: o
+        $$scope: f
     } = e;
     this && this.__awaiter;
-    const i = ji();
+    const i = Ii();
     let {
-        i18n: f
+        i18n: o
     } = e, {
-        eta: r = null
+        eta: u = null
     } = e, {
         queue_position: a
     } = e, {
-        queue_size: u
+        queue_size: r
     } = e, {
         status: _
     } = e, {
         scroll_to_output: c = !1
     } = e, {
         timer: h = !0
     } = e, {
         show_progress: L = "full"
     } = e, {
-        message: H = null
+        message: M = null
     } = e, {
-        progress: p = null
+        progress: k = null
     } = e, {
         variant: v = "default"
     } = e, {
         loading_text: m = "Loading..."
     } = e, {
         absolute: b = !0
     } = e, {
         translucent: C = !1
     } = e, {
         border: T = !1
     } = e, {
-        autoscroll: k
-    } = e, N, I = !1, ae = 0, j = 0, le = null, ne = null, ge = 0, Y = null, re, O = null, we = !0;
+        autoscroll: p
+    } = e, N, I = !1, le = 0, j = 0, ne = null, ie = null, ge = 0, Y = null, ue, O = null, we = !0;
     const _e = () => {
-        t(0, r = t(27, le = t(19, ke = null))), t(25, ae = performance.now()), t(26, j = 0), I = !0, ve();
+        t(0, u = t(27, ne = t(19, pe = null))), t(25, le = performance.now()), t(26, j = 0), I = !0, ve();
     };
 
     function ve() {
         requestAnimationFrame(() => {
-            t(26, j = (performance.now() - ae) / 1e3), I && ve();
+            t(26, j = (performance.now() - le) / 1e3), I && ve();
         });
     }
 
     function w() {
-        t(26, j = 0), t(0, r = t(27, le = t(19, ke = null))), I && (I = !1);
+        t(26, j = 0), t(0, u = t(27, ne = t(19, pe = null))), I && (I = !1);
     }
-    Ii(() => {
+    Di(() => {
         I && w();
     });
-    let ke = null;
+    let pe = null;
 
     function We(y) {
-        Xt[y ? "unshift" : "push"](() => {
-            O = y, t(16, O), t(7, p), t(14, Y), t(15, re);
+        Ut[y ? "unshift" : "push"](() => {
+            O = y, t(16, O), t(7, k), t(14, Y), t(15, ue);
         });
     }
     const Je = () => {
         i("clear_status");
     };
 
     function Qe(y) {
-        Xt[y ? "unshift" : "push"](() => {
+        Ut[y ? "unshift" : "push"](() => {
             N = y, t(13, N);
         });
     }
     return l.$$set = (y) => {
-        "i18n" in y && t(1, f = y.i18n), "eta" in y && t(0, r = y.eta), "queue_position" in y && t(2, a = y.queue_position), "queue_size" in y && t(3, u = y.queue_size), "status" in y && t(4, _ = y.status), "scroll_to_output" in y && t(22, c = y.scroll_to_output), "timer" in y && t(5, h = y.timer), "show_progress" in y && t(6, L = y.show_progress), "message" in y && t(23, H = y.message), "progress" in y && t(7, p = y.progress), "variant" in y && t(8, v = y.variant), "loading_text" in y && t(9, m = y.loading_text), "absolute" in y && t(10, b = y.absolute), "translucent" in y && t(11, C = y.translucent), "border" in y && t(12, T = y.border), "autoscroll" in y && t(24, k = y.autoscroll), "$$scope" in y && t(29, o = y.$$scope);
+        "i18n" in y && t(1, o = y.i18n), "eta" in y && t(0, u = y.eta), "queue_position" in y && t(2, a = y.queue_position), "queue_size" in y && t(3, r = y.queue_size), "status" in y && t(4, _ = y.status), "scroll_to_output" in y && t(22, c = y.scroll_to_output), "timer" in y && t(5, h = y.timer), "show_progress" in y && t(6, L = y.show_progress), "message" in y && t(23, M = y.message), "progress" in y && t(7, k = y.progress), "variant" in y && t(8, v = y.variant), "loading_text" in y && t(9, m = y.loading_text), "absolute" in y && t(10, b = y.absolute), "translucent" in y && t(11, C = y.translucent), "border" in y && t(12, T = y.border), "autoscroll" in y && t(24, p = y.autoscroll), "$$scope" in y && t(29, f = y.$$scope);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            436207617 && (r === null && t(0, r = le), r != null && le !== r && (t(28, ne = (performance.now() - ae) / 1e3 + r), t(19, ke = ne.toFixed(1)), t(27, le = r))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
-            335544320 && t(17, ge = ne === null || ne <= 0 || !j ? null : Math.min(j / ne, 1)), l.$$.dirty[0] & /*progress*/
-            128 && p != null && t(18, we = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (p != null ? t(14, Y = p.map((y) => {
+            436207617 && (u === null && t(0, u = ne), u != null && ne !== u && (t(28, ie = (performance.now() - le) / 1e3 + u), t(19, pe = ie.toFixed(1)), t(27, ne = u))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            335544320 && t(17, ge = ie === null || ie <= 0 || !j ? null : Math.min(j / ie, 1)), l.$$.dirty[0] & /*progress*/
+            128 && k != null && t(18, we = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            114816 && (k != null ? t(14, Y = k.map((y) => {
                 if (y.index != null && y.length != null)
                     return y.index / y.length;
                 if (y.progress != null)
                     return y.progress;
-            })) : t(14, Y = null), Y ? (t(15, re = Y[Y.length - 1]), O && (re === 0 ? t(16, O.style.transition = "0", O) : t(16, O.style.transition = "150ms", O))) : t(15, re = void 0)), l.$$.dirty[0] & /*status*/
+            })) : t(14, Y = null), Y ? (t(15, ue = Y[Y.length - 1]), O && (ue === 0 ? t(16, O.style.transition = "0", O) : t(16, O.style.transition = "150ms", O))) : t(15, ue = void 0)), l.$$.dirty[0] & /*status*/
             16 && (_ === "pending" ? _e() : w()), l.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            20979728 && N && c && (_ === "pending" || _ === "complete") && es(N, k), l.$$.dirty[0] & /*status, message*/
+            20979728 && N && c && (_ === "pending" || _ === "complete") && $i(N, p), l.$$.dirty[0] & /*status, message*/
             8388624, l.$$.dirty[0] & /*timer_diff*/
             67108864 && t(20, n = j.toFixed(1));
     }, [
-        r,
-        f,
-        a,
         u,
+        o,
+        a,
+        r,
         _,
         h,
         L,
-        p,
+        k,
         v,
         m,
         b,
         C,
         T,
         N,
         Y,
-        re,
+        ue,
         O,
         ge,
         we,
-        ke,
+        pe,
         n,
         i,
         c,
-        H,
-        k,
-        ae,
-        j,
+        M,
+        p,
         le,
+        j,
         ne,
-        o,
+        ie,
+        f,
         s,
         We,
         Je,
         Qe
     ];
 }
-class ls extends Ti {
+class ts extends Ei {
     constructor(e) {
-        super(), Bi(
+        super(), Ti(
             this,
             e,
-            ts,
-            xi,
-            Ni, {
+            es,
+            Qi,
+            Bi, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 22,
                 timer: 5,
@@ -3710,45 +3700,45 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: ns,
-    add_iframe_resize_listener: is,
-    add_render_callback: ss,
-    append: os,
+    SvelteComponent: ls,
+    add_iframe_resize_listener: ns,
+    add_render_callback: is,
+    append: ss,
     attr: fs,
-    binding_callbacks: as,
-    detach: rs,
+    binding_callbacks: os,
+    detach: as,
     element: us,
-    init: _s,
-    insert: cs,
-    noop: al,
-    safe_not_equal: ds,
-    set_data: ms,
-    text: hs,
+    init: rs,
+    insert: _s,
+    noop: ol,
+    safe_not_equal: cs,
+    set_data: ds,
+    text: ms,
     toggle_class: qe
 } = window.__gradio__svelte__internal, {
-    onMount: bs
+    onMount: hs
 } = window.__gradio__svelte__internal;
 
-function gs(l) {
+function bs(l) {
     let e, t = (
             /*value*/
             (l[0] ? (
                 /*value*/
                 l[0]
             ) : "") + ""
         ),
         n, s;
     return {
         c() {
-            e = us("div"), n = hs(t), fs(e, "class", "svelte-84cxb8"), ss(() => (
+            e = us("div"), n = ms(t), fs(e, "class", "svelte-84cxb8"), is(() => (
                 /*div_elementresize_handler*/
                 l[5].call(e)
             )), qe(
                 e,
                 "table",
                 /*type*/
                 l[1] === "table"
@@ -3760,117 +3750,117 @@
             ), qe(
                 e,
                 "selected",
                 /*selected*/
                 l[2]
             );
         },
-        m(o, i) {
-            cs(o, e, i), os(e, n), s = is(
+        m(f, i) {
+            _s(f, e, i), ss(e, n), s = ns(
                 e,
                 /*div_elementresize_handler*/
                 l[5].bind(e)
             ), l[6](e);
         },
-        p(o, [i]) {
+        p(f, [i]) {
             i & /*value*/
                 1 && t !== (t = /*value*/
-                    (o[0] ? (
+                    (f[0] ? (
                         /*value*/
-                        o[0]
-                    ) : "") + "") && ms(n, t), i & /*type*/
+                        f[0]
+                    ) : "") + "") && ds(n, t), i & /*type*/
                 2 && qe(
                     e,
                     "table",
                     /*type*/
-                    o[1] === "table"
+                    f[1] === "table"
                 ), i & /*type*/
                 2 && qe(
                     e,
                     "gallery",
                     /*type*/
-                    o[1] === "gallery"
+                    f[1] === "gallery"
                 ), i & /*selected*/
                 4 && qe(
                     e,
                     "selected",
                     /*selected*/
-                    o[2]
+                    f[2]
                 );
         },
-        i: al,
-        o: al,
-        d(o) {
-            o && rs(e), s(), l[6](null);
+        i: ol,
+        o: ol,
+        d(f) {
+            f && as(e), s(), l[6](null);
         }
     };
 }
 
-function ws(l, e, t) {
+function gs(l, e, t) {
     let {
         value: n
     } = e, {
         type: s
     } = e, {
-        selected: o = !1
-    } = e, i, f;
+        selected: f = !1
+    } = e, i, o;
 
-    function r(_, c) {
-        !_ || !c || (f.style.setProperty("--local-text-width", `${c < 150 ? c : 200}px`), t(4, f.style.whiteSpace = "unset", f));
+    function u(_, c) {
+        !_ || !c || (o.style.setProperty("--local-text-width", `${c < 150 ? c : 200}px`), t(4, o.style.whiteSpace = "unset", o));
     }
-    bs(() => {
-        r(f, i);
+    hs(() => {
+        u(o, i);
     });
 
     function a() {
         i = this.clientWidth, t(3, i);
     }
 
-    function u(_) {
-        as[_ ? "unshift" : "push"](() => {
-            f = _, t(4, f);
+    function r(_) {
+        os[_ ? "unshift" : "push"](() => {
+            o = _, t(4, o);
         });
     }
     return l.$$set = (_) => {
-        "value" in _ && t(0, n = _.value), "type" in _ && t(1, s = _.type), "selected" in _ && t(2, o = _.selected);
-    }, [n, s, o, i, f, a, u];
+        "value" in _ && t(0, n = _.value), "type" in _ && t(1, s = _.type), "selected" in _ && t(2, f = _.selected);
+    }, [n, s, f, i, o, a, r];
 }
-class Es extends ns {
+class zs extends ls {
     constructor(e) {
-        super(), _s(this, e, ws, gs, ds, {
+        super(), rs(this, e, gs, bs, cs, {
             value: 0,
             type: 1,
             selected: 2
         });
     }
 }
 const {
-    SvelteComponent: vs,
-    add_flush_callback: rl,
-    assign: ks,
+    SvelteComponent: ws,
+    add_flush_callback: al,
+    assign: vs,
     bind: ul,
-    binding_callbacks: _l,
+    binding_callbacks: rl,
     check_outros: ps,
-    create_component: Ct,
-    destroy_component: yt,
-    detach: Cs,
+    create_component: kt,
+    destroy_component: Ct,
+    detach: ks,
     flush: Z,
-    get_spread_object: ys,
-    get_spread_update: Ls,
-    group_outros: Ms,
-    init: Vs,
-    insert: Hs,
-    mount_component: Lt,
-    safe_not_equal: qs,
-    space: Fs,
+    get_spread_object: Cs,
+    get_spread_update: ys,
+    group_outros: Ls,
+    init: Ms,
+    insert: Vs,
+    mount_component: yt,
+    safe_not_equal: Hs,
+    space: qs,
     transition_in: Ze,
     transition_out: Ne
 } = window.__gradio__svelte__internal;
 
-function cl(l) {
+function _l(l) {
     let e, t;
     const n = [{
             autoscroll: (
                 /*gradio*/
                 l[2].autoscroll
             )
         }, {
@@ -3879,78 +3869,78 @@
                 l[2].i18n
             )
         },
         /*loading_status*/
         l[18]
     ];
     let s = {};
-    for (let o = 0; o < n.length; o += 1)
-        s = ks(s, n[o]);
-    return e = new ls({
+    for (let f = 0; f < n.length; f += 1)
+        s = vs(s, n[f]);
+    return e = new ts({
         props: s
     }), e.$on(
         "clear_status",
         /*clear_status_handler*/
         l[24]
     ), {
         c() {
-            Ct(e.$$.fragment);
+            kt(e.$$.fragment);
         },
-        m(o, i) {
-            Lt(e, o, i), t = !0;
+        m(f, i) {
+            yt(e, f, i), t = !0;
         },
-        p(o, i) {
-            const f = i[0] & /*gradio, loading_status*/
-                262148 ? Ls(n, [
+        p(f, i) {
+            const o = i[0] & /*gradio, loading_status*/
+                262148 ? ys(n, [
                     i[0] & /*gradio*/
                     4 && {
                         autoscroll: (
                             /*gradio*/
-                            o[2].autoscroll
+                            f[2].autoscroll
                         )
                     },
                     i[0] & /*gradio*/
                     4 && {
                         i18n: (
                             /*gradio*/
-                            o[2].i18n
+                            f[2].i18n
                         )
                     },
                     i[0] & /*loading_status*/
-                    262144 && ys(
+                    262144 && Cs(
                         /*loading_status*/
-                        o[18]
+                        f[18]
                     )
                 ]) : {};
-            e.$set(f);
+            e.$set(o);
         },
-        i(o) {
-            t || (Ze(e.$$.fragment, o), t = !0);
+        i(f) {
+            t || (Ze(e.$$.fragment, f), t = !0);
         },
-        o(o) {
-            Ne(e.$$.fragment, o), t = !1;
+        o(f) {
+            Ne(e.$$.fragment, f), t = !1;
         },
-        d(o) {
-            yt(e, o);
+        d(f) {
+            Ct(e, f);
         }
     };
 }
 
-function Zs(l) {
-    let e, t, n, s, o, i = (
+function Fs(l) {
+    let e, t, n, s, f, i = (
         /*loading_status*/
-        l[18] && cl(l)
+        l[18] && _l(l)
     );
 
-    function f(u) {
-        l[25](u);
+    function o(r) {
+        l[25](r);
     }
 
-    function r(u) {
-        l[26](u);
+    function u(r) {
+        l[26](r);
     }
     let a = {
         label: (
             /*label*/
             l[3]
         ),
         info: (
@@ -4012,17 +4002,17 @@
             l[23]
     };
     return (
         /*value*/
         l[0] !== void 0 && (a.value = /*value*/
             l[0]), /*value_is_output*/
         l[1] !== void 0 && (a.value_is_output = /*value_is_output*/
-            l[1]), t = new yi({
+            l[1]), t = new Ci({
             props: a
-        }), _l.push(() => ul(t, "value", f)), _l.push(() => ul(t, "value_is_output", r)), t.$on(
+        }), rl.push(() => ul(t, "value", o)), rl.push(() => ul(t, "value_is_output", u)), t.$on(
             "change",
             /*change_handler*/
             l[27]
         ), t.$on(
             "input",
             /*input_handler*/
             l[28]
@@ -4040,84 +4030,84 @@
             l[31]
         ), t.$on(
             "focus",
             /*focus_handler*/
             l[32]
         ), {
             c() {
-                i && i.c(), e = Fs(), Ct(t.$$.fragment);
+                i && i.c(), e = qs(), kt(t.$$.fragment);
             },
-            m(u, _) {
-                i && i.m(u, _), Hs(u, e, _), Lt(t, u, _), o = !0;
+            m(r, _) {
+                i && i.m(r, _), Vs(r, e, _), yt(t, r, _), f = !0;
             },
-            p(u, _) {
+            p(r, _) {
                 /*loading_status*/
-                u[18] ? i ? (i.p(u, _), _[0] & /*loading_status*/
-                    262144 && Ze(i, 1)) : (i = cl(u), i.c(), Ze(i, 1), i.m(e.parentNode, e)) : i && (Ms(), Ne(i, 1, 1, () => {
+                r[18] ? i ? (i.p(r, _), _[0] & /*loading_status*/
+                    262144 && Ze(i, 1)) : (i = _l(r), i.c(), Ze(i, 1), i.m(e.parentNode, e)) : i && (Ls(), Ne(i, 1, 1, () => {
                     i = null;
                 }), ps());
                 const c = {};
                 _[0] & /*label*/
                     8 && (c.label = /*label*/
-                        u[3]), _[0] & /*info*/
+                        r[3]), _[0] & /*info*/
                     16 && (c.info = /*info*/
-                        u[4]), _[0] & /*show_label*/
+                        r[4]), _[0] & /*show_label*/
                     1024 && (c.show_label = /*show_label*/
-                        u[10]), _[0] & /*lines*/
+                        r[10]), _[0] & /*lines*/
                     256 && (c.lines = /*lines*/
-                        u[8]), _[0] & /*type*/
+                        r[8]), _[0] & /*type*/
                     16384 && (c.type = /*type*/
-                        u[14]), _[0] & /*rtl*/
+                        r[14]), _[0] & /*rtl*/
                     524288 && (c.rtl = /*rtl*/
-                        u[19]), _[0] & /*text_align*/
+                        r[19]), _[0] & /*text_align*/
                     1048576 && (c.text_align = /*text_align*/
-                        u[20]), _[0] & /*max_lines, lines*/
+                        r[20]), _[0] & /*max_lines, lines*/
                     2304 && (c.max_lines = /*max_lines*/
-                        u[11] ? (
+                        r[11] ? (
                             /*max_lines*/
-                            u[11]
+                            r[11]
                         ) : (
                             /*lines*/
-                            u[8] + 1
+                            r[8] + 1
                         )), _[0] & /*prompts*/
                     4096 && (c.prompts = /*prompts*/
-                        u[12]), _[0] & /*suffixes*/
+                        r[12]), _[0] & /*suffixes*/
                     8192 && (c.suffixes = /*suffixes*/
-                        u[13]), _[0] & /*placeholder*/
+                        r[13]), _[0] & /*placeholder*/
                     512 && (c.placeholder = /*placeholder*/
-                        u[9]), _[0] & /*autofocus*/
+                        r[9]), _[0] & /*autofocus*/
                     2097152 && (c.autofocus = /*autofocus*/
-                        u[21]), _[0] & /*container*/
+                        r[21]), _[0] & /*container*/
                     32768 && (c.container = /*container*/
-                        u[15]), _[0] & /*autoscroll*/
+                        r[15]), _[0] & /*autoscroll*/
                     4194304 && (c.autoscroll = /*autoscroll*/
-                        u[22]), _[0] & /*interactive*/
+                        r[22]), _[0] & /*interactive*/
                     8388608 && (c.disabled = ! /*interactive*/
-                        u[23]), !n && _[0] & /*value*/
+                        r[23]), !n && _[0] & /*value*/
                     1 && (n = !0, c.value = /*value*/
-                        u[0], rl(() => n = !1)), !s && _[0] & /*value_is_output*/
+                        r[0], al(() => n = !1)), !s && _[0] & /*value_is_output*/
                     2 && (s = !0, c.value_is_output = /*value_is_output*/
-                        u[1], rl(() => s = !1)), t.$set(c);
+                        r[1], al(() => s = !1)), t.$set(c);
             },
-            i(u) {
-                o || (Ze(i), Ze(t.$$.fragment, u), o = !0);
+            i(r) {
+                f || (Ze(i), Ze(t.$$.fragment, r), f = !0);
             },
-            o(u) {
-                Ne(i), Ne(t.$$.fragment, u), o = !1;
+            o(r) {
+                Ne(i), Ne(t.$$.fragment, r), f = !1;
             },
-            d(u) {
-                u && Cs(e), i && i.d(u), yt(t, u);
+            d(r) {
+                r && ks(e), i && i.d(r), Ct(t, r);
             }
         }
     );
 }
 
-function Ss(l) {
+function Zs(l) {
     let e, t;
-    return e = new Xl({
+    return e = new Ul({
         props: {
             visible: (
                 /*visible*/
                 l[7]
             ),
             elem_id: (
                 /*elem_id*/
@@ -4137,171 +4127,171 @@
             ),
             allow_overflow: !1,
             padding: (
                 /*container*/
                 l[15]
             ),
             $$slots: {
-                default: [Zs]
+                default: [Fs]
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
-            Ct(e.$$.fragment);
+            kt(e.$$.fragment);
         },
         m(n, s) {
-            Lt(e, n, s), t = !0;
+            yt(e, n, s), t = !0;
         },
         p(n, s) {
-            const o = {};
+            const f = {};
             s[0] & /*visible*/
-                128 && (o.visible = /*visible*/
+                128 && (f.visible = /*visible*/
                     n[7]), s[0] & /*elem_id*/
-                32 && (o.elem_id = /*elem_id*/
+                32 && (f.elem_id = /*elem_id*/
                     n[5]), s[0] & /*elem_classes*/
-                64 && (o.elem_classes = /*elem_classes*/
+                64 && (f.elem_classes = /*elem_classes*/
                     n[6]), s[0] & /*scale*/
-                65536 && (o.scale = /*scale*/
+                65536 && (f.scale = /*scale*/
                     n[16]), s[0] & /*min_width*/
-                131072 && (o.min_width = /*min_width*/
+                131072 && (f.min_width = /*min_width*/
                     n[17]), s[0] & /*container*/
-                32768 && (o.padding = /*container*/
+                32768 && (f.padding = /*container*/
                     n[15]), s[0] & /*label, info, show_label, lines, type, rtl, text_align, max_lines, prompts, suffixes, placeholder, autofocus, container, autoscroll, interactive, value, value_is_output, gradio, loading_status*/
                 16580383 | s[1] & /*$$scope*/
-                4 && (o.$$scope = {
+                4 && (f.$$scope = {
                     dirty: s,
                     ctx: n
-                }), e.$set(o);
+                }), e.$set(f);
         },
         i(n) {
             t || (Ze(e.$$.fragment, n), t = !0);
         },
         o(n) {
             Ne(e.$$.fragment, n), t = !1;
         },
         d(n) {
-            yt(e, n);
+            Ct(e, n);
         }
     };
 }
 
-function zs(l, e, t) {
+function Ss(l, e, t) {
     let {
         gradio: n
     } = e, {
         label: s = "Textbox"
     } = e, {
-        info: o = void 0
+        info: f = void 0
     } = e, {
         elem_id: i = ""
     } = e, {
-        elem_classes: f = []
+        elem_classes: o = []
     } = e, {
-        visible: r = !0
+        visible: u = !0
     } = e, {
         value: a = ""
     } = e, {
-        lines: u
+        lines: r
     } = e, {
         placeholder: _ = ""
     } = e, {
         show_label: c
     } = e, {
         max_lines: h
     } = e, {
         prompts: L = []
     } = e, {
-        suffixes: H = []
+        suffixes: M = []
     } = e, {
-        type: p = "text"
+        type: k = "text"
     } = e, {
         container: v = !0
     } = e, {
         scale: m = null
     } = e, {
         min_width: b = void 0
     } = e, {
         loading_status: C = void 0
     } = e, {
         value_is_output: T = !1
     } = e, {
-        rtl: k = !1
+        rtl: p = !1
     } = e, {
         text_align: N = void 0
     } = e, {
         autofocus: I = !1
     } = e, {
-        autoscroll: ae = !0
+        autoscroll: le = !0
     } = e, {
-        interactive: j
+        interactive: j = !0
     } = e;
-    const le = () => n.dispatch("clear_status", C);
+    const ne = () => n.dispatch("clear_status", C);
 
-    function ne(w) {
+    function ie(w) {
         a = w, t(0, a);
     }
 
     function ge(w) {
         T = w, t(1, T);
     }
     const Y = () => n.dispatch("change", a),
-        re = () => n.dispatch("input"),
+        ue = () => n.dispatch("input"),
         O = () => n.dispatch("submit"),
         we = () => n.dispatch("blur"),
         _e = (w) => n.dispatch("select", w.detail),
         ve = () => n.dispatch("focus");
     return l.$$set = (w) => {
-        "gradio" in w && t(2, n = w.gradio), "label" in w && t(3, s = w.label), "info" in w && t(4, o = w.info), "elem_id" in w && t(5, i = w.elem_id), "elem_classes" in w && t(6, f = w.elem_classes), "visible" in w && t(7, r = w.visible), "value" in w && t(0, a = w.value), "lines" in w && t(8, u = w.lines), "placeholder" in w && t(9, _ = w.placeholder), "show_label" in w && t(10, c = w.show_label), "max_lines" in w && t(11, h = w.max_lines), "prompts" in w && t(12, L = w.prompts), "suffixes" in w && t(13, H = w.suffixes), "type" in w && t(14, p = w.type), "container" in w && t(15, v = w.container), "scale" in w && t(16, m = w.scale), "min_width" in w && t(17, b = w.min_width), "loading_status" in w && t(18, C = w.loading_status), "value_is_output" in w && t(1, T = w.value_is_output), "rtl" in w && t(19, k = w.rtl), "text_align" in w && t(20, N = w.text_align), "autofocus" in w && t(21, I = w.autofocus), "autoscroll" in w && t(22, ae = w.autoscroll), "interactive" in w && t(23, j = w.interactive);
+        "gradio" in w && t(2, n = w.gradio), "label" in w && t(3, s = w.label), "info" in w && t(4, f = w.info), "elem_id" in w && t(5, i = w.elem_id), "elem_classes" in w && t(6, o = w.elem_classes), "visible" in w && t(7, u = w.visible), "value" in w && t(0, a = w.value), "lines" in w && t(8, r = w.lines), "placeholder" in w && t(9, _ = w.placeholder), "show_label" in w && t(10, c = w.show_label), "max_lines" in w && t(11, h = w.max_lines), "prompts" in w && t(12, L = w.prompts), "suffixes" in w && t(13, M = w.suffixes), "type" in w && t(14, k = w.type), "container" in w && t(15, v = w.container), "scale" in w && t(16, m = w.scale), "min_width" in w && t(17, b = w.min_width), "loading_status" in w && t(18, C = w.loading_status), "value_is_output" in w && t(1, T = w.value_is_output), "rtl" in w && t(19, p = w.rtl), "text_align" in w && t(20, N = w.text_align), "autofocus" in w && t(21, I = w.autofocus), "autoscroll" in w && t(22, le = w.autoscroll), "interactive" in w && t(23, j = w.interactive);
     }, [
         a,
         T,
         n,
         s,
-        o,
-        i,
         f,
-        r,
+        i,
+        o,
         u,
+        r,
         _,
         c,
         h,
         L,
-        H,
-        p,
+        M,
+        k,
         v,
         m,
         b,
         C,
-        k,
+        p,
         N,
         I,
-        ae,
-        j,
         le,
+        j,
         ne,
+        ie,
         ge,
         Y,
-        re,
+        ue,
         O,
         we,
         _e,
         ve
     ];
 }
-class Ts extends vs {
+class Es extends ws {
     constructor(e) {
-        super(), Vs(
+        super(), Ms(
             this,
             e,
-            zs,
             Ss,
-            qs, {
+            Zs,
+            Hs, {
                 gradio: 2,
                 label: 3,
                 info: 4,
                 elem_id: 5,
                 elem_classes: 6,
                 visible: 7,
                 value: 0,
@@ -4517,12 +4507,12 @@
     set interactive(e) {
         this.$$set({
             interactive: e
         }), Z();
     }
 }
 export {
-    Es as BaseExample,
-    yi as BaseTextbox,
-    Ts as
+    zs as BaseExample,
+    Ci as BaseTextbox,
+    Es as
     default
 };
```

### Comparing `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/style.css` & `gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/templates/component/style.css`

 * *Files 15% similar despite different names*

```diff
@@ -1 +1 @@
-.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-1lrphxw{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-1lrphxw{opacity:.5;box-shadow:none}button[disabled].svelte-1lrphxw:hover{cursor:not-allowed}.padded.svelte-1lrphxw{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-1lrphxw:hover,button.highlight.svelte-1lrphxw{cursor:pointer;color:var(--color-accent)}.padded.svelte-1lrphxw:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-1lrphxw{padding:0 1px;font-size:10px}div.svelte-1lrphxw{padding:2px;display:flex;align-items:flex-end}.small.svelte-1lrphxw{width:14px;height:14px}.medium.svelte-1lrphxw{width:20px;height:20px}.large.svelte-1lrphxw{width:22px;height:22px}.pending.svelte-1lrphxw{animation:svelte-1lrphxw-flash .5s infinite}@keyframes svelte-1lrphxw-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-1lrphxw{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-q32hvf{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;align-items:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;color:var(--block-label-text-color);flex-shrink:0}.show_border.svelte-q32hvf{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}label.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:block;width:100%}textarea.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:block;position:relative;outline:none!important;box-shadow:var(--input-shadow);background:var(--input-background-fill);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none}label.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:not(.container){height:100%}textarea.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:disabled{-webkit-text-fill-color:var(--body-text-color);-webkit-opacity:1;opacity:1}textarea.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs::placeholder{color:var(--input-placeholder-color)}.extend_button.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:flex;position:relative;align-items:center;width:20px;height:20px;overflow:hidden;color:var(--block-label-color);font:var(--font-sans);font-size:var(--button-small-text-size)}.extend_button.svelte-82ixrs:hover path.svelte-82ixrs.svelte-82ixrs{--ring-color:var(--color-accent);filter:brightness(1.1);fill:#ff6700}.menu_section.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{padding:12px 0 0;align-items:center;color:#100700;font-family:Inter;font-size:13px;font-style:normal;font-weight:300;line-height:24px;display:flex;flex-direction:column;align-items:flex-start;gap:8px}.menu.svelte-82ixrs ul.svelte-82ixrs.svelte-82ixrs{list-style-type:none;display:flex;align-items:flex-start;align-content:flex-start;gap:4px 12px;flex-wrap:wrap;flex-direction:column;width:100%}.menu.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{border-radius:0 0 15px 15px;background:#cccccc1a;margin:0 16px;padding:0 14px 12px}.menu.svelte-82ixrs li.svelte-82ixrs.svelte-82ixrs{width:100%}.text_extension_button.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{border-radius:15px;border:.5px solid #ff9a57;background:#fff4ea;cursor:pointer;display:flex;padding:4px 12px;align-items:center;gap:4px}.text_extension_button_prompt.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:flex;width:100%;padding:8px 12px;justify-content:space-between;align-items:center;border-radius:10px;border:.5px solid #ff9a57;background:#fff4ea;color:#101111;text-align:left;font-size:13px;font-style:normal;font-weight:300;line-height:normal;gap:4px;flex-wrap:wrap;flex-direction:row}.text_extension_button_prompt.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:hover{color:#fff;fill:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button_prompt.svelte-82ixrs:hover svg.svelte-82ixrs path.svelte-82ixrs{fill:#fff}.text_extension_button.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:hover{color:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button.svelte-82ixrs:hover svg.svelte-82ixrs path.svelte-82ixrs{fill:#fff}.magic_container.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:flex;position:relative;outline:none!important;box-shadow:var(--input-shadow);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none;scrollbar-width:none;resize:none;align-items:center}.scroll_hide_magic.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:block;position:relative;outline:none!important;box-shadow:none;padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none;scrollbar-width:none;resize:none}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden}.wrap.center.svelte-vopvsi.svelte-vopvsi{top:0;right:0;left:0}.wrap.default.svelte-vopvsi.svelte-vopvsi{top:0;right:0;bottom:0;left:0}.hide.svelte-vopvsi.svelte-vopvsi{opacity:0;pointer-events:none}.generating.svelte-vopvsi.svelte-vopvsi{animation:svelte-vopvsi-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1);pointer-events:none}.translucent.svelte-vopvsi.svelte-vopvsi{background:none}@keyframes svelte-vopvsi-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-vopvsi.svelte-vopvsi{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-vopvsi.svelte-vopvsi{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-vopvsi.svelte-vopvsi{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-vopvsi.svelte-vopvsi{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-vopvsi.svelte-vopvsi{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-vopvsi .progress-text.svelte-vopvsi{background:var(--block-background-fill)}.border.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary)}.clear-status.svelte-vopvsi.svelte-vopvsi{position:absolute;display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-84cxb8{padding:var(--size-1) var(--size-2)}div.svelte-84cxb8{overflow:hidden;min-width:var(--local-text-width);white-space:nowrap}
+.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-1lrphxw{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-1lrphxw{opacity:.5;box-shadow:none}button[disabled].svelte-1lrphxw:hover{cursor:not-allowed}.padded.svelte-1lrphxw{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-1lrphxw:hover,button.highlight.svelte-1lrphxw{cursor:pointer;color:var(--color-accent)}.padded.svelte-1lrphxw:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-1lrphxw{padding:0 1px;font-size:10px}div.svelte-1lrphxw{padding:2px;display:flex;align-items:flex-end}.small.svelte-1lrphxw{width:14px;height:14px}.medium.svelte-1lrphxw{width:20px;height:20px}.large.svelte-1lrphxw{width:22px;height:22px}.pending.svelte-1lrphxw{animation:svelte-1lrphxw-flash .5s infinite}@keyframes svelte-1lrphxw-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-1lrphxw{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-q32hvf{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;align-items:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;color:var(--block-label-text-color);flex-shrink:0}.show_border.svelte-q32hvf{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}label.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{display:block;width:100%}textarea.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{display:block;position:relative;outline:none!important;box-shadow:var(--input-shadow);background:var(--input-background-fill);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none}label.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u:not(.container){height:100%}textarea.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u:disabled{-webkit-text-fill-color:var(--body-text-color);-webkit-opacity:1;opacity:1}textarea.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u::placeholder{color:var(--input-placeholder-color)}.extend_button.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{display:flex;position:relative;align-items:center;width:20px;height:20px;overflow:hidden;color:var(--block-label-color);font:var(--font-sans);font-size:var(--button-small-text-size)}.extend_button.svelte-lsxp0u:hover path.svelte-lsxp0u.svelte-lsxp0u{--ring-color:var(--color-accent);filter:brightness(1.1);fill:#ff6700}.menu_section.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{padding:12px 0 0;align-items:center;color:#100700;font-family:Inter;font-size:13px;font-style:normal;font-weight:300;line-height:24px;display:flex;flex-direction:column;align-items:flex-start;gap:8px}.menu.svelte-lsxp0u ul.svelte-lsxp0u.svelte-lsxp0u{list-style-type:none;display:flex;align-items:flex-start;align-content:flex-start;gap:4px 12px;flex-wrap:wrap;flex-direction:column;width:100%}.menu.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{border-radius:0 0 15px 15px;background:#cccccc1a;margin:0 16px;padding:0 14px 12px}.menu.svelte-lsxp0u li.svelte-lsxp0u.svelte-lsxp0u{width:100%}.text_extension_button.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{border-radius:15px;border:.5px solid #ff9a57;background:#fff4ea;cursor:pointer;display:flex;padding:4px 12px;align-items:center;gap:4px}.text_extension_button_prompt.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{display:flex;width:100%;padding:8px 12px;justify-content:space-between;align-items:center;border-radius:10px;border:.5px solid #ff9a57;background:#fff4ea;color:#101111;text-align:left;font-size:13px;font-style:normal;font-weight:300;line-height:normal;gap:4px;flex-wrap:wrap;flex-direction:row}.text_extension_button_prompt.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u:hover{color:#fff;fill:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button_prompt.svelte-lsxp0u:hover svg.svelte-lsxp0u path.svelte-lsxp0u{fill:#fff}.text_extension_button.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u:hover{color:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button.svelte-lsxp0u:hover svg.svelte-lsxp0u path.svelte-lsxp0u{fill:#fff}.magic_container.svelte-lsxp0u.svelte-lsxp0u.svelte-lsxp0u{display:flex;position:relative;outline:none!important;box-shadow:var(--input-shadow);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none;scrollbar-width:none;resize:none;align-items:center}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden}.wrap.center.svelte-vopvsi.svelte-vopvsi{top:0;right:0;left:0}.wrap.default.svelte-vopvsi.svelte-vopvsi{top:0;right:0;bottom:0;left:0}.hide.svelte-vopvsi.svelte-vopvsi{opacity:0;pointer-events:none}.generating.svelte-vopvsi.svelte-vopvsi{animation:svelte-vopvsi-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1);pointer-events:none}.translucent.svelte-vopvsi.svelte-vopvsi{background:none}@keyframes svelte-vopvsi-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-vopvsi.svelte-vopvsi{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-vopvsi.svelte-vopvsi{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-vopvsi.svelte-vopvsi{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-vopvsi.svelte-vopvsi{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-vopvsi.svelte-vopvsi{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-vopvsi .progress-text.svelte-vopvsi{background:var(--block-background-fill)}.border.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary)}.clear-status.svelte-vopvsi.svelte-vopvsi{position:absolute;display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-84cxb8{padding:var(--size-1) var(--size-2)}div.svelte-84cxb8{overflow:hidden;min-width:var(--local-text-width);white-space:nowrap}
```

### Comparing `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/example/index.js` & `gradio_clickabletextbox-0.0.4/backend/gradio_clickabletextbox/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/demo/app.py` & `gradio_clickabletextbox-0.0.4/demo/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1236)
+    demo.launch(server_port=1234)
```

### Comparing `gradio_clickabletextbox-0.0.3/demo/css.css` & `gradio_clickabletextbox-0.0.4/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/demo/space.py` & `gradio_clickabletextbox-0.0.4/demo/space.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1236)
+    demo.launch(server_port=1234)
 
 ```
 """, elem_classes=["md-custom"], header_links=True)
 
 
     gr.Markdown("""
 ## `ClickableTextbox`
```

### Comparing `gradio_clickabletextbox-0.0.3/frontend/Example.svelte` & `gradio_clickabletextbox-0.0.4/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/frontend/Index.svelte` & `gradio_clickabletextbox-0.0.4/frontend/Index.svelte`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 	export let min_width: number | undefined = undefined;
 	export let loading_status: LoadingStatus | undefined = undefined;
 	export let value_is_output = false;
 	export let rtl = false;
 	export let text_align: "left" | "right" | undefined = undefined;
 	export let autofocus = false;
 	export let autoscroll = true;
-	export let interactive: boolean;
+	export let interactive: boolean = true;
 </script>
 
 <Block
 	{visible}
 	{elem_id}
 	{elem_classes}
 	{scale}
```

### Comparing `gradio_clickabletextbox-0.0.3/frontend/package-lock.json` & `gradio_clickabletextbox-0.0.4/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/frontend/package.json` & `gradio_clickabletextbox-0.0.4/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/frontend/shared/Textbox.svelte` & `gradio_clickabletextbox-0.0.4/frontend/shared/Textbox.svelte`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 		if (autofocus) {
 			el.focus();
 		}
 		if (can_scroll && autoscroll) {
 			scroll();
 		}
 		value_is_output = false;
+		show_magic = prompts.length > 0 || suffixes.length > 0;
 	});
 	$: value, handle_change();
 
 	async function handle_extension(): Promise<void> {
 		show_menu = !show_menu;
 	}
 
@@ -178,15 +179,15 @@
 	<BlockTitle {show_label} {info}>{label}</BlockTitle>
 	<div class="input-container">
 		{#if show_menu && show_magic}
 			<div class="magic_container">
 				<textarea
 					data-testid="textbox"
 					use:text_area_resize={value}
-					class={show_magic ? "scroll_hide_magic" : "scroll-hide"}
+					class="scroll-hide"
 					dir={rtl ? "rtl" : "ltr"}
 					bind:value
 					bind:this={el}
 					{placeholder}
 					rows={lines}
 					{disabled}
 					{autofocus}
@@ -277,15 +278,15 @@
 				{/if}
 			</div>
 		{:else if !show_menu && show_magic}
 			<div class="magic_container">
 				<textarea
 					data-testid="textbox"
 					use:text_area_resize={value}
-					class={show_magic ? "scroll_hide_magic" : "scroll-hide"}
+					class="scroll-hide"
 					dir={rtl ? "rtl" : "ltr"}
 					bind:value
 					bind:this={el}
 					{placeholder}
 					rows={lines}
 					{disabled}
 					{autofocus}
@@ -316,15 +317,15 @@
 					</svg>
 				</button>
 			</div>
 		{:else}
 			<textarea
 				data-testid="textbox"
 				use:text_area_resize={value}
-				class={show_magic ? "scroll_hide_magic" : "scroll-hide"}
+				class="scroll-hide"
 				dir={rtl ? "rtl" : "ltr"}
 				bind:value
 				bind:this={el}
 				{placeholder}
 				rows={lines}
 				{disabled}
 				{autofocus}
@@ -497,23 +498,8 @@
 		line-height: var(--line-sm);
 		border: none;
 		scrollbar-width: none;
 		resize: none;
 		align-items: center;
 	}
 
-	.scroll_hide_magic {
-		display: block;
-		position: relative;
-		outline: none !important;
-		box-shadow: none;
-		padding: var(--input-padding);
-		width: 100%;
-		color: var(--body-text-color);
-		font-weight: var(--input-text-weight);
-		font-size: var(--input-text-size);
-		line-height: var(--line-sm);
-		border: none;
-		scrollbar-width: none;
-		resize: none;
-	}
 </style>
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
 show_label} {info}>{label}
 {#if show_menu && show_magic}
-"scroll_hide_magic" : "scroll-hide"} dir={rtl ? "rtl" : "ltr"} bind:value bind:
-this={el} {placeholder} rows={lines} {disabled} {autofocus} on:keypress=
-{handle_keypress} on:blur on:select={handle_select} on:focus on:scroll=
-{handle_scroll} style={text_align ? "text-align: " + text_align : ""} />
+"rtl" : "ltr"} bind:value bind:this={el} {placeholder} rows={lines} {disabled}
+{autofocus} on:keypress={handle_keypress} on:blur on:select={handle_select} on:
+focus on:scroll={handle_scroll} style={text_align ? "text-align: " + text_align
+: ""} />
 {#if prompts.length > 0}
 Best prompt structures
     * {#each prompts as word}
     * > addToTextbox(word)} >{word}
 {/each}
 {/if} {#if suffixes.length > 0}
 Best style keywords
     * {#each suffixes as word}
     * > addToTextbox(word)} >{word}
 {/each}
 {/if}
 {:else if !show_menu && show_magic}
-"scroll_hide_magic" : "scroll-hide"} dir={rtl ? "rtl" : "ltr"} bind:value bind:
-this={el} {placeholder} rows={lines} {disabled} {autofocus} on:keypress=
-{handle_keypress} on:blur on:select={handle_select} on:focus on:scroll=
-{handle_scroll} style={text_align ? "text-align: " + text_align : ""} />
+"rtl" : "ltr"} bind:value bind:this={el} {placeholder} rows={lines} {disabled}
+{autofocus} on:keypress={handle_keypress} on:blur on:select={handle_select} on:
+focus on:scroll={handle_scroll} style={text_align ? "text-align: " + text_align
+: ""} />
 {:else}
-"scroll_hide_magic" : "scroll-hide"} dir={rtl ? "rtl" : "ltr"} bind:value bind:
-this={el} {placeholder} rows={lines} {disabled} {autofocus} on:keypress=
-{handle_keypress} on:blur on:select={handle_select} on:focus on:scroll=
-{handle_scroll} style={text_align ? "text-align: " + text_align : ""} /> {/if}
+"rtl" : "ltr"} bind:value bind:this={el} {placeholder} rows={lines} {disabled}
+{autofocus} on:keypress={handle_keypress} on:blur on:select={handle_select} on:
+focus on:scroll={handle_scroll} style={text_align ? "text-align: " + text_align
+: ""} /> {/if}
```

### Comparing `gradio_clickabletextbox-0.0.3/frontend/shared/transitions.js` & `gradio_clickabletextbox-0.0.4/frontend/shared/transitions.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.3/README.md` & `gradio_clickabletextbox-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1236)
+    demo.launch(server_port=1234)
 
 ```
 
 ## `ClickableTextbox`
 
 ### Initialization
```

### Comparing `gradio_clickabletextbox-0.0.3/pyproject.toml` & `gradio_clickabletextbox-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_clickabletextbox"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library for easily interacting with trained machine learning models"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Textbox"]
 # Add dependencies here
```

### Comparing `gradio_clickabletextbox-0.0.3/PKG-INFO` & `gradio_clickabletextbox-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_clickabletextbox
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for easily interacting with trained machine learning models
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 Keywords: gradio-custom-component,gradio-template-Textbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1236)
+    demo.launch(server_port=1234)
 
 ```
 
 ## `ClickableTextbox`
 
 ### Initialization
```

