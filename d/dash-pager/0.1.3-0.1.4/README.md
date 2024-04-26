# Comparing `tmp/dash_pager-0.1.3.tar.gz` & `tmp/dash_pager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pager-0.1.3.tar", last modified: Thu Apr 18 18:47:51 2024, max compression
+gzip compressed data, was "dash_pager-0.1.4.tar", last modified: Fri Apr 26 17:05:35 2024, max compression
```

## Comparing `dash_pager-0.1.3.tar` & `dash_pager-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 18:47:51.099397 dash_pager-0.1.3/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2024-04-18 01:01:07.000000 dash_pager-0.1.3/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.1.3/MANIFEST.in
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 18:47:51.099268 dash_pager-0.1.3/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3952 2024-04-18 01:10:30.000000 dash_pager-0.1.3/README.md
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 18:47:51.098411 dash_pager-0.1.3/dash_pager/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1912 2024-04-18 18:46:23.000000 dash_pager-0.1.3/dash_pager/Pager.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.1.3/dash_pager/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-18 18:46:23.000000 dash_pager-0.1.3/dash_pager/_imports_.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4616 2024-04-18 18:42:46.000000 dash_pager-0.1.3/dash_pager/async-Pager.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)     8238 2024-04-18 18:42:46.000000 dash_pager-0.1.3/dash_pager/async-Pager.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3942 2024-04-18 18:46:22.000000 dash_pager-0.1.3/dash_pager/dash_pager.min.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)    19383 2024-04-18 18:46:22.000000 dash_pager-0.1.3/dash_pager/dash_pager.min.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3956 2024-04-18 18:46:23.000000 dash_pager-0.1.3/dash_pager/metadata.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 18:46:23.000000 dash_pager-0.1.3/dash_pager/package-info.json
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 18:47:51.098927 dash_pager-0.1.3/dash_pager.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 18:47:51.000000 dash_pager-0.1.3/dash_pager.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-18 18:47:51.000000 dash_pager-0.1.3/dash_pager.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-18 18:47:51.000000 dash_pager-0.1.3/dash_pager.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-18 18:47:51.000000 dash_pager-0.1.3/dash_pager.egg-info/top_level.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 18:42:35.000000 dash_pager-0.1.3/package.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-18 18:47:51.099433 dash_pager-0.1.3/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.1.3/setup.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 18:47:51.099094 dash_pager-0.1.3/tests/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.1.3/tests/test_usage.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-26 17:05:35.637962 dash_pager-0.1.4/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2024-04-18 01:01:07.000000 dash_pager-0.1.4/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.1.4/MANIFEST.in
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-26 17:05:35.637770 dash_pager-0.1.4/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3952 2024-04-18 01:10:30.000000 dash_pager-0.1.4/README.md
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-26 17:05:35.636594 dash_pager-0.1.4/dash_pager/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1912 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/Pager.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.1.4/dash_pager/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/_imports_.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5213 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/async-Pager.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     9443 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/async-Pager.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3942 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/dash_pager.min.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    19383 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/dash_pager.min.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3956 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/metadata.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-26 17:04:39.000000 dash_pager-0.1.4/dash_pager/package-info.json
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-26 17:05:35.637582 dash_pager-0.1.4/dash_pager.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-26 17:05:35.000000 dash_pager-0.1.4/dash_pager.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-26 17:05:35.000000 dash_pager-0.1.4/dash_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-26 17:05:35.000000 dash_pager-0.1.4/dash_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-26 17:05:35.000000 dash_pager-0.1.4/dash_pager.egg-info/top_level.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-26 15:39:04.000000 dash_pager-0.1.4/package.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-26 17:05:35.637998 dash_pager-0.1.4/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.1.4/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-26 17:05:35.637251 dash_pager-0.1.4/tests/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.1.4/tests/test_usage.py
```

### Comparing `dash_pager-0.1.3/LICENSE` & `dash_pager-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.3/PKG-INFO` & `dash_pager-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_pager
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_pager-0.1.3/README.md` & `dash_pager-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.3/dash_pager/Pager.py` & `dash_pager-0.1.4/dash_pager/Pager.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.3/dash_pager/__init__.py` & `dash_pager-0.1.4/dash_pager/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.3/dash_pager/async-Pager.js` & `dash_pager-0.1.4/dash_pager/async-Pager.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,220 +1,239 @@
 "use strict";
 (self.webpackChunkdash_pager = self.webpackChunkdash_pager || []).push([
     [119], {
-        993: (e, t, n) => {
-            n.r(t), n.d(t, {
-                default: () => b
+        993: (e, t, r) => {
+            r.r(t), r.d(t, {
+                default: () => y
             });
-            var r = n(609),
-                o = n.n(r),
-                i = n(120),
-                a = n.n(i);
+            var n = r(609),
+                a = r.n(n),
+                o = r(120),
+                i = r.n(o);
 
             function l(e) {
                 return l = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                 }, l(e)
             }
 
             function u(e, t) {
-                for (var n = 0; n < t.length; n++) {
-                    var r = t[n];
-                    r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, c(r.key), r)
+                for (var r = 0; r < t.length; r++) {
+                    var n = t[r];
+                    n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, b(n.key), n)
                 }
             }
 
-            function c(e) {
-                var t = function(e, t) {
-                    if ("object" != l(e) || !e) return e;
-                    var n = e[Symbol.toPrimitive];
-                    if (void 0 !== n) {
-                        var r = n.call(e, "string");
-                        if ("object" != l(r)) return r;
-                        throw new TypeError("@@toPrimitive must return a primitive value.")
-                    }
-                    return String(e)
-                }(e);
-                return "symbol" == l(t) ? t : t + ""
-            }
-
-            function s(e, t, n) {
-                return t = m(t),
+            function c(e, t, r) {
+                return t = p(t),
                     function(e, t) {
                         if (t && ("object" === l(t) || "function" == typeof t)) return t;
                         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
                         return function(e) {
                             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return e
                         }(e)
-                    }(e, p() ? Reflect.construct(t, n || [], m(e).constructor) : t.apply(e, n))
+                    }(e, s() ? Reflect.construct(t, r || [], p(e).constructor) : t.apply(e, r))
             }
 
-            function p() {
+            function s() {
                 try {
                     var e = !Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {})))
                 } catch (e) {}
-                return (p = function() {
+                return (s = function() {
                     return !!e
                 })()
             }
 
-            function m(e) {
-                return m = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+            function p(e) {
+                return p = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                     return e.__proto__ || Object.getPrototypeOf(e)
-                }, m(e)
+                }, p(e)
             }
 
-            function f(e, t) {
-                return f = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+            function m(e, t) {
+                return m = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                     return e.__proto__ = t, e
-                }, f(e, t)
+                }, m(e, t)
             }
-            var b = function(e) {
+
+            function f(e, t, r) {
+                return (t = b(t)) in e ? Object.defineProperty(e, t, {
+                    value: r,
+                    enumerable: !0,
+                    configurable: !0,
+                    writable: !0
+                }) : e[t] = r, e
+            }
+
+            function b(e) {
+                var t = function(e, t) {
+                    if ("object" != l(e) || !e) return e;
+                    var r = e[Symbol.toPrimitive];
+                    if (void 0 !== r) {
+                        var n = r.call(e, "string");
+                        if ("object" != l(n)) return n;
+                        throw new TypeError("@@toPrimitive must return a primitive value.")
+                    }
+                    return String(e)
+                }(e);
+                return "symbol" == l(t) ? t : t + ""
+            }
+            var y = function(e) {
                 function t() {
-                    return function(e, t) {
+                    var e;
+                    ! function(e, t) {
                         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                    }(this, t), s(this, t, arguments)
+                    }(this, t);
+                    for (var r = arguments.length, n = new Array(r), a = 0; a < r; a++) n[a] = arguments[a];
+                    return f(e = c(this, t, [].concat(n)), "visibleVal", null), f(e, "updateInterval", (function(t) {
+                        var r = t.tempVal,
+                            n = e.visibleVal[0],
+                            a = e.visibleVal[1];
+                        if (r) {
+                            "MM" === r ? n = e.props.minValue : "M" === r ? n -= 1 : "PP" === r ? a = e.props.maxValue : "P" === r ? a += 1 : r.startsWith("F") && isNaN(n = parseInt(r.replace("F", ""))) ? n = r.replace("F", "") : r.startsWith("T") && isNaN(a = parseInt(r.replace("T", ""))) && (a = r.replace("T", ""));
+                            var o = [n, a];
+                            "number" == typeof n && e.props.value[0] != n && n >= 1 && n <= e.props.maxValue ? (o = [n, e.props.value[1]], e.props.setProps({
+                                value: o
+                            })) : "number" == typeof a && e.props.value[1] != a && a >= e.props.value[0] && a <= e.props.maxValue && (o = [e.props.value[0], a], e.props.setProps({
+                                value: o
+                            })), e.visibleVal = o
+                        }
+                        e.forceUpdate()
+                    })), e
                 }
                 return function(e, t) {
                     if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                     e.prototype = Object.create(t && t.prototype, {
                         constructor: {
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
                     }), Object.defineProperty(e, "prototype", {
                         writable: !1
-                    }), t && f(e, t)
-                }(t, e), n = t, (r = [{
+                    }), t && m(e, t)
+                }(t, e), r = t, (n = [{
                     key: "render",
                     value: function() {
-                        var e = this.props,
-                            t = e.id,
-                            n = e.value,
-                            r = e.maxValue,
-                            i = e.minValue,
-                            a = e.symbols,
-                            l = e.tempVal,
-                            u = e.style,
-                            c = e.setProps,
-                            s = n[0],
-                            p = n[1];
-                        return l && ("MM" === l ? s = i : "M" === l ? s -= 1 : "PP" === l ? p = r : "P" === l ? p += 1 : l.startsWith("F") && isNaN(s = parseInt(l.replace("F", ""))) ? s = l.replace("F", "") : l.startsWith("T") && isNaN(p = parseInt(l.replace("T", ""))) && (p = l.replace("T", "")), "number" == typeof s && n[0] != s && s >= 1 && s <= r && this.props.setProps({
-                            value: [s, n[1]],
-                            tempVal: null
-                        }), "number" == typeof p && n[1] != p && p >= n[0] && p <= r && this.props.setProps({
-                            value: [n[0], p],
-                            tempVal: null
-                        })), o().createElement("div", {
-                            id: t + "-container",
+                        var e = this,
+                            t = this.props,
+                            r = t.id,
+                            n = t.value,
+                            o = t.maxValue,
+                            i = t.minValue,
+                            l = t.symbols,
+                            u = t.style;
+                        t.setProps, this.visibleVal || (this.visibleVal = n);
+                        var c = this.visibleVal[0],
+                            s = this.visibleVal[1];
+                        return a().createElement("div", {
+                            id: r + "-container",
                             className: "form-row",
                             style: u
-                        }, o().createElement("button", {
-                            id: t + "-mm",
+                        }, a().createElement("button", {
+                            id: r + "-mm",
                             className: "btn btn-outline-primary me-2",
                             type: "button",
-                            onClick: function(e) {
-                                return c({
+                            onClick: function(t) {
+                                return e.updateInterval({
                                     tempVal: "MM"
                                 })
                             }
-                        }, o().createElement("i", {
+                        }, a().createElement("i", {
                             className: "bi bi-chevron-double-left"
-                        }), a[0]), o().createElement("button", {
-                            id: t + "-m",
+                        }), l[0]), a().createElement("button", {
+                            id: r + "-m",
                             className: "btn btn-outline-primary me-2",
                             type: "button",
-                            onClick: function(e) {
-                                return c({
+                            onClick: function(t) {
+                                return e.updateInterval({
                                     tempVal: "M"
                                 })
                             }
-                        }, o().createElement("i", {
+                        }, a().createElement("i", {
                             className: "bi bi-chevron-left"
-                        }), a[1]), o().createElement("span", {
+                        }), l[1]), a().createElement("span", {
                             className: "me-2"
-                        }, " From "), o().createElement("input", {
-                            id: t + "-ip-from",
-                            value: s,
-                            onChange: function(e) {
-                                return c({
-                                    tempVal: "F" + e.target.value
+                        }, " From "), a().createElement("input", {
+                            id: r + "-ip-from",
+                            value: c,
+                            onChange: function(t) {
+                                return e.updateInterval({
+                                    tempVal: "F" + t.target.value
                                 })
                             },
                             type: "number",
                             style: {
                                 width: "10ch",
                                 display: "inline"
                             },
-                            className: "form-control" + (s != n[0] || s < i || s > p ? " is-invalid" : "")
-                        }), o().createElement("span", {
+                            className: "form-control" + (c != n[0] || c < i || c > s ? " is-invalid" : "")
+                        }), a().createElement("span", {
                             className: "me-2"
-                        }, " to "), o().createElement("input", {
-                            id: t + "-ip-to",
-                            value: p,
-                            onChange: function(e) {
-                                return c({
-                                    tempVal: "T" + e.target.value
+                        }, " to "), a().createElement("input", {
+                            id: r + "-ip-to",
+                            value: s,
+                            onChange: function(t) {
+                                return e.updateInterval({
+                                    tempVal: "T" + t.target.value
                                 })
                             },
                             type: "number",
                             style: {
                                 width: "10ch",
                                 display: "inline"
                             },
-                            className: "form-control" + (p != n[1] || p > r || p < s ? " is-invalid" : "")
-                        }), o().createElement("span", {
+                            className: "form-control" + (s != n[1] || s > o || s < c ? " is-invalid" : "")
+                        }), a().createElement("span", {
                             className: "me-2"
-                        }, " of ", r, " "), o().createElement("button", {
-                            id: t + "-p",
+                        }, " of ", o, " "), a().createElement("button", {
+                            id: r + "-p",
                             className: "btn btn-outline-primary me-2",
                             type: "button",
-                            onClick: function(e) {
-                                return c({
+                            onClick: function(t) {
+                                return e.updateInterval({
                                     tempVal: "P"
                                 })
                             }
-                        }, o().createElement("i", {
+                        }, a().createElement("i", {
                             className: "bi bi-chevron-right"
-                        }), a[2]), o().createElement("button", {
-                            id: t + "-pp",
+                        }), l[2]), a().createElement("button", {
+                            id: r + "-pp",
                             className: "btn btn-outline-primary me-2",
                             type: "button",
-                            onClick: function(e) {
-                                return c({
+                            onClick: function(t) {
+                                return e.updateInterval({
                                     tempVal: "PP"
                                 })
                             }
-                        }, o().createElement("i", {
+                        }, a().createElement("i", {
                             className: "bi bi-chevron-double-right"
-                        }), a[3]), o().createElement("input", {
-                            id: t,
+                        }), l[3]), a().createElement("input", {
+                            id: r,
                             value: n,
                             type: "hidden"
                         }))
                     }
-                }]) && u(n.prototype, r), Object.defineProperty(n, "prototype", {
+                }]) && u(r.prototype, n), Object.defineProperty(r, "prototype", {
                     writable: !1
-                }), n;
-                var n, r
-            }(r.Component);
-            b.defaultProps = {
+                }), r;
+                var r, n
+            }(n.Component);
+            y.defaultProps = {
                 minValue: 1,
                 symbols: ["", "", "", ""]
-            }, b.propTypes = {
-                id: a().string,
-                value: a().arrayOf(a().number),
-                maxValue: a().number.isRequired,
-                minValue: a().number,
-                symbols: a().arrayOf(a().string),
-                style: a().object,
-                tempVal: a().string,
-                setProps: a().func
+            }, y.propTypes = {
+                id: i().string,
+                value: i().arrayOf(i().number),
+                maxValue: i().number.isRequired,
+                minValue: i().number,
+                symbols: i().arrayOf(i().string),
+                style: i().object,
+                setProps: i().func
             }
         }
     }
 ]);
 //# sourceMappingURL=async-Pager.js.map
```

### Comparing `dash_pager-0.1.3/dash_pager/async-Pager.js.map` & `dash_pager-0.1.4/dash_pager/async-Pager.js.map`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8120879120879121%*

 * *Differences: {"'mappings'": "'wuDAGA,IAGqBA,EAAK,SAAAC,GAAA,SAAAD,IAAA,IAAAE,G,4FAAAC,CAAA,KAAAH,GAAA,QAAAI,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAyCrB,OAzCqBC,EAAAR,EAAAS,EAAA,KAAAX,EAAA,GAAAY,OAAAL,IAAA,aAET,MAAIG,EAAAR,EAAA,kBAEA,SAACW,GACd,IAAIC,EAAUD,EAAEC,QAEZC,EAAOb,EAAKc,WAAW,GACvBC,EAAOf,EAAKc,WAAW,GAE3B,GAAIF,EAAS,CACO,OAAZA,EACAC,EAAOb,EAAKgB,MAAMC,SACC,MAAZL,EACPC,GAAY,EACO,OAAZD,EACPG,EAAKf,EAAKgB,MAAME,SACG,MAAZN,EACPG,GAAQ,EACDH,EAAQO,WAAW,MAC1BC,MAAOP,EA […]*

```diff
@@ -1,40 +1,53 @@
 {
     "file": "async-Pager.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "Pager",
         "_Component",
+        "_this",
         "_classCallCheck",
-        "_callSuper",
+        "_len",
         "arguments",
-        "_inherits",
-        "key",
-        "value",
-        "_this$props",
-        "this",
-        "props",
-        "id",
-        "maxValue",
-        "minValue",
-        "symbols",
+        "length",
+        "args",
+        "Array",
+        "_key",
+        "_defineProperty",
+        "_callSuper",
+        "concat",
+        "e",
         "tempVal",
-        "style",
-        "setProps",
         "from",
+        "visibleVal",
         "to",
+        "props",
+        "minValue",
+        "maxValue",
         "startsWith",
         "isNaN",
         "parseInt",
         "replace",
+        "newVal",
+        "value",
+        "setProps",
+        "forceUpdate",
+        "_inherits",
+        "key",
+        "_this2",
+        "_this$props",
+        "this",
+        "id",
+        "symbols",
+        "style",
         "React",
         "className",
         "type",
         "onClick",
-        "e",
+        "updateInterval",
         "onChange",
         "target",
         "width",
         "display",
         "Component",
         "defaultProps",
         "propTypes",
@@ -42,11 +55,11 @@
         "isRequired"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/lib/fragments/Pager.react.js"
     ],
     "sourcesContent": [
-        "import React, {Component} from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * Generic pagination component.\n */\nexport default class Pager extends Component {\n    render() {\n        const {id, value, maxValue, minValue, symbols, tempVal, style, setProps} = this.props;\n        \n        var from = value[0];\n        var to   = value[1];\n\n        if (tempVal) {\n            if (tempVal === 'MM'){\n                from = minValue\n            } else if (tempVal === 'M'){\n                from = from-1\n            } else if (tempVal === 'PP'){\n                to = maxValue\n            } else if (tempVal === 'P'){\n                to = to+1\n            } else if (tempVal.startsWith(\"F\") && \n                isNaN( from = parseInt(tempVal.replace(\"F\", \"\")) )\n               ) {\n                from = tempVal.replace(\"F\", \"\");\n            } else if (tempVal.startsWith(\"T\") && \n                isNaN( to = parseInt(tempVal.replace(\"T\", \"\")) ) \n               ) {\n                to = tempVal.replace(\"T\", \"\");\n            } \n        \n            if (typeof from === \"number\" && value[0] != from && from >= 1 && from <= maxValue)\n                this.props.setProps({ 'value': [from, value[1]], 'tempVal': null });\n            if (typeof to === \"number\" && value[1] != to && to >= value[0] && to <= maxValue)\n                this.props.setProps({ 'value': [value[0], to], 'tempVal': null });\n        }\n        \n        return (\n            <div id={id+\"-container\"} className=\"form-row\" style={style}>\n                <button id={id+\"-mm\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'MM' })\n                    }>\n                    <i className=\"bi bi-chevron-double-left\"></i>{symbols[0]}\n                </button>\n                <button id={id+\"-m\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'M' })\n                    }>\n                    <i className=\"bi bi-chevron-left\"></i>{symbols[1]}\n                </button>\n                <span className=\"me-2\"> From </span>\n                <input\n                    id={id+\"-ip-from\"}\n                    value={from}\n                    onChange={\n                        e => setProps({ tempVal: 'F'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((from != value[0] || from < minValue || from > to) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> to </span>\n                <input\n                    id={id+\"-ip-to\"}\n                    value={to}\n                    onChange={\n                        e => setProps({ tempVal: 'T'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((to != value[1] || to > maxValue || to < from) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> of {maxValue} </span>\n                <button id={id+\"-p\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'P' })\n                    }>\n                    <i className=\"bi bi-chevron-right\"></i>{symbols[2]}\n                </button>\n                <button id={id+\"-pp\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'PP' })\n                    }>\n                    <i className=\"bi bi-chevron-double-right\"></i>{symbols[3]}\n                </button>\n                <input\n                    id={id}\n                    value={value}\n                    type=\"hidden\"\n                />\n            </div>\n        );\n    }\n}\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n    \n    /**\n     * The style of the container (div)\n     */\n    style: PropTypes.object,\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    tempVal: PropTypes.string,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n"
+        "import React, {Component} from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * Generic pagination component.\n */\nexport default class Pager extends Component {\n    \n    visibleVal = null;\n    \n    updateInterval = (e) => {\n        let tempVal = e.tempVal;\n        \n        var from = this.visibleVal[0];\n        var to   = this.visibleVal[1];\n\n        if (tempVal) {\n            if (tempVal === 'MM'){\n                from = this.props.minValue;\n            } else if (tempVal === 'M'){\n                from = from-1;\n            } else if (tempVal === 'PP'){\n                to = this.props.maxValue;\n            } else if (tempVal === 'P'){\n                to = to+1;\n            } else if (tempVal.startsWith(\"F\") && \n                isNaN( from = parseInt(tempVal.replace(\"F\", \"\")) )\n               ) {\n                from = tempVal.replace(\"F\", \"\");\n            } else if (tempVal.startsWith(\"T\") && \n                isNaN( to = parseInt(tempVal.replace(\"T\", \"\")) ) \n               ) {\n                to = tempVal.replace(\"T\", \"\");\n            } \n            \n            let newVal = [from, to];\n            if (typeof from === \"number\" && this.props.value[0] != from && from >= 1 && from <= this.props.maxValue) {\n                newVal = [from, this.props.value[1]];\n                this.props.setProps({ 'value': newVal });\n            } else if (typeof to === \"number\" && this.props.value[1] != to && to >= this.props.value[0] && to <= this.props.maxValue) {\n                newVal = [this.props.value[0], to];\n                this.props.setProps({ 'value': newVal });\n            }\n            this.visibleVal = newVal;\n        }\n\n        this.forceUpdate();\n    };\n    \n    render() {\n        const {id, value, maxValue, minValue, symbols, style, setProps} = this.props;\n        \n        if (!this.visibleVal)\n            this.visibleVal = value\n        \n        let from = this.visibleVal[0];\n        let to   = this.visibleVal[1];\n        \n        return (\n            <div id={id+\"-container\"} className=\"form-row\" style={style}>\n                <button id={id+\"-mm\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => this.updateInterval({ tempVal: 'MM' })\n                    }>\n                    <i className=\"bi bi-chevron-double-left\"></i>{symbols[0]}\n                </button>\n                <button id={id+\"-m\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => this.updateInterval({ tempVal: 'M' })\n                    }>\n                    <i className=\"bi bi-chevron-left\"></i>{symbols[1]}\n                </button>\n                <span className=\"me-2\"> From </span>\n                <input\n                    id={id+\"-ip-from\"}\n                    value={from}\n                    onChange={\n                        e => this.updateInterval({ tempVal: 'F'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((from != value[0] || from < minValue || from > to) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> to </span>\n                <input\n                    id={id+\"-ip-to\"}\n                    value={to}\n                    onChange={\n                        e => this.updateInterval({ tempVal: 'T'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((to != value[1] || to > maxValue || to < from) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> of {maxValue} </span>\n                <button id={id+\"-p\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => this.updateInterval({ tempVal: 'P' })\n                    }>\n                    <i className=\"bi bi-chevron-right\"></i>{symbols[2]}\n                </button>\n                <button id={id+\"-pp\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => this.updateInterval({ tempVal: 'PP' })\n                    }>\n                    <i className=\"bi bi-chevron-double-right\"></i>{symbols[3]}\n                </button>\n                <input\n                    id={id}\n                    value={value}\n                    type=\"hidden\"\n                />\n            </div>\n        );\n    }\n}\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n    \n    /**\n     * The style of the container (div)\n     */\n    style: PropTypes.object,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func,\n};\n"
     ],
     "version": 3
 }
```

### Comparing `dash_pager-0.1.3/dash_pager/dash_pager.min.js` & `dash_pager-0.1.4/dash_pager/dash_pager.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -95,15 +95,15 @@
         var s = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var r, t = (r = i(), /\/_dash-component-suites\//.test(r.src)),
                 n = s(e);
             if (!t) return n;
             var o = n.split("/"),
                 a = o.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_1_3m1713465983"), o.splice(-1, 1, a.join(".")), o.join("/")
+            return a.splice(1, 0, "v0_1_4m1714151079"), o.splice(-1, 1, a.join(".")), o.join("/")
         }
     }(() => {
         var e = {
             792: 0
         };
         o.f.j = (r, t) => {
             var n = o.o(e, r) ? e[r] : void 0;
```

### Comparing `dash_pager-0.1.3/dash_pager/dash_pager.min.js.map` & `dash_pager-0.1.4/dash_pager/dash_pager.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915966386554622%*

 * *Differences: {"'sourcesContent'": "{insert: [(12, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc […]*

```diff
@@ -173,14 +173,14 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + \"async-Pager\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_3m1713465983\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_4m1714151079\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t792: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkdash_pager\"] = self[\"webpackChunkdash_pager\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "export const Pager = React.lazy(() => import(/* webpackChunkName: \"Pager\" */ './fragments/Pager.react'));",
         "import React from 'react';\nimport PropTypes from 'prop-types';\nimport { Pager as RealComponent } from '../LazyLoader';\n\n/**\n * ExampleComponent is an example component.\n * It takes a property, `label`, and\n * displays it.\n * It renders an input with the property `value`\n * which is editable by the user.\n */\nconst Pager = (props) => {\n    return (\n        <React.Suspense fallback={null}>\n            <RealComponent {...props}/>\n        </React.Suspense>\n    );\n};\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * A label that will be printed when this component is rendered.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n    \n    /**\n     * The style of the container (div)\n     */\n    style: PropTypes.object,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n\nexport default Pager;\n\nexport const defaultProps = Pager.defaultProps;\nexport const propTypes = Pager.propTypes;\n"
     ],
     "version": 3
 }
```

### Comparing `dash_pager-0.1.3/dash_pager/metadata.json` & `dash_pager-0.1.4/dash_pager/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.3/dash_pager/package-info.json` & `dash_pager-0.1.4/dash_pager/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.4'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `dash_pager-0.1.3/dash_pager.egg-info/PKG-INFO` & `dash_pager-0.1.4/dash_pager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dash-pager
-Version: 0.1.3
+Name: dash_pager
+Version: 0.1.4
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_pager-0.1.3/package.json` & `dash_pager-0.1.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.4'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `dash_pager-0.1.3/setup.py` & `dash_pager-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.3/tests/test_usage.py` & `dash_pager-0.1.4/tests/test_usage.py`

 * *Files identical despite different names*

