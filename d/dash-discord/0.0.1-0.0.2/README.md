# Comparing `tmp/dash_discord-0.0.1.tar.gz` & `tmp/dash_discord-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_discord-0.0.1.tar", last modified: Fri May 31 21:46:20 2024, max compression
+gzip compressed data, was "dash_discord-0.0.2.tar", last modified: Fri May 31 22:17:24 2024, max compression
```

## Comparing `dash_discord-0.0.1.tar` & `dash_discord-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 21:46:20.787019 dash_discord-0.0.1/
--rw-r--r--   0 pip        (501) staff       (20)        0 2024-05-31 21:22:21.000000 dash_discord-0.0.1/LICENSE
--rw-r--r--   0 pip        (501) staff       (20)      353 2024-05-31 21:22:21.000000 dash_discord-0.0.1/MANIFEST.in
--rw-r--r--   0 pip        (501) staff       (20)     3979 2024-05-31 21:46:20.786814 dash_discord-0.0.1/PKG-INFO
--rw-r--r--   0 pip        (501) staff       (20)     3711 2024-05-31 21:22:21.000000 dash_discord-0.0.1/README.md
-drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 21:46:20.785577 dash_discord-0.0.1/dash_discord/
--rw-r--r--   0 pip        (501) staff       (20)     1075 2024-05-31 21:39:52.000000 dash_discord-0.0.1/dash_discord/DiscordCrate.py
--rw-r--r--   0 pip        (501) staff       (20)     1401 2024-05-31 21:39:52.000000 dash_discord-0.0.1/dash_discord/DiscordWidget.py
--rw-r--r--   0 pip        (501) staff       (20)     2253 2024-05-31 21:22:21.000000 dash_discord-0.0.1/dash_discord/__init__.py
--rw-r--r--   0 pip        (501) staff       (20)      134 2024-05-31 21:39:52.000000 dash_discord-0.0.1/dash_discord/_imports_.py
--rw-r--r--   0 pip        (501) staff       (20)     8050 2024-05-31 21:39:51.000000 dash_discord-0.0.1/dash_discord/dash_discord.min.js
--rw-r--r--   0 pip        (501) staff       (20)    24333 2024-05-31 21:39:51.000000 dash_discord-0.0.1/dash_discord/dash_discord.min.js.map
--rw-r--r--   0 pip        (501) staff       (20)     2460 2024-05-31 21:39:52.000000 dash_discord-0.0.1/dash_discord/metadata.json
--rw-r--r--   0 pip        (501) staff       (20)     2141 2024-05-31 21:39:52.000000 dash_discord-0.0.1/dash_discord/package-info.json
-drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 21:46:20.786620 dash_discord-0.0.1/dash_discord.egg-info/
--rw-r--r--   0 pip        (501) staff       (20)     3979 2024-05-31 21:46:20.000000 dash_discord-0.0.1/dash_discord.egg-info/PKG-INFO
--rw-r--r--   0 pip        (501) staff       (20)      453 2024-05-31 21:46:20.000000 dash_discord-0.0.1/dash_discord.egg-info/SOURCES.txt
--rw-r--r--   0 pip        (501) staff       (20)        1 2024-05-31 21:46:20.000000 dash_discord-0.0.1/dash_discord.egg-info/dependency_links.txt
--rw-r--r--   0 pip        (501) staff       (20)       13 2024-05-31 21:46:20.000000 dash_discord-0.0.1/dash_discord.egg-info/top_level.txt
--rw-r--r--   0 pip        (501) staff       (20)     2141 2024-05-31 21:32:30.000000 dash_discord-0.0.1/package.json
--rw-r--r--   0 pip        (501) staff       (20)       38 2024-05-31 21:46:20.787063 dash_discord-0.0.1/setup.cfg
--rw-r--r--   0 pip        (501) staff       (20)      695 2024-05-31 21:22:21.000000 dash_discord-0.0.1/setup.py
-drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 21:46:20.786196 dash_discord-0.0.1/tests/
--rw-r--r--   0 pip        (501) staff       (20)      920 2024-05-31 21:22:21.000000 dash_discord-0.0.1/tests/test_usage.py
+drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 22:17:24.893972 dash_discord-0.0.2/
+-rw-r--r--   0 pip        (501) staff       (20)        0 2024-05-31 21:22:21.000000 dash_discord-0.0.2/LICENSE
+-rw-r--r--   0 pip        (501) staff       (20)      353 2024-05-31 21:22:21.000000 dash_discord-0.0.2/MANIFEST.in
+-rw-r--r--   0 pip        (501) staff       (20)     3979 2024-05-31 22:17:24.893720 dash_discord-0.0.2/PKG-INFO
+-rw-r--r--   0 pip        (501) staff       (20)     3711 2024-05-31 21:22:21.000000 dash_discord-0.0.2/README.md
+drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 22:17:24.892436 dash_discord-0.0.2/dash_discord/
+-rw-r--r--   0 pip        (501) staff       (20)     1077 2024-05-31 22:16:12.000000 dash_discord-0.0.2/dash_discord/DiscordCrate.py
+-rw-r--r--   0 pip        (501) staff       (20)     1494 2024-05-31 22:16:12.000000 dash_discord-0.0.2/dash_discord/DiscordWidget.py
+-rw-r--r--   0 pip        (501) staff       (20)     2253 2024-05-31 21:22:21.000000 dash_discord-0.0.2/dash_discord/__init__.py
+-rw-r--r--   0 pip        (501) staff       (20)      134 2024-05-31 22:16:12.000000 dash_discord-0.0.2/dash_discord/_imports_.py
+-rw-r--r--   0 pip        (501) staff       (20)     6861 2024-05-31 22:16:11.000000 dash_discord-0.0.2/dash_discord/dash_discord.min.js
+-rw-r--r--   0 pip        (501) staff       (20)    24411 2024-05-31 22:16:11.000000 dash_discord-0.0.2/dash_discord/dash_discord.min.js.map
+-rw-r--r--   0 pip        (501) staff       (20)     2698 2024-05-31 22:16:12.000000 dash_discord-0.0.2/dash_discord/metadata.json
+-rw-r--r--   0 pip        (501) staff       (20)     2141 2024-05-31 22:16:12.000000 dash_discord-0.0.2/dash_discord/package-info.json
+drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 22:17:24.893400 dash_discord-0.0.2/dash_discord.egg-info/
+-rw-r--r--   0 pip        (501) staff       (20)     3979 2024-05-31 22:17:24.000000 dash_discord-0.0.2/dash_discord.egg-info/PKG-INFO
+-rw-r--r--   0 pip        (501) staff       (20)      453 2024-05-31 22:17:24.000000 dash_discord-0.0.2/dash_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 pip        (501) staff       (20)        1 2024-05-31 22:17:24.000000 dash_discord-0.0.2/dash_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 pip        (501) staff       (20)       13 2024-05-31 22:17:24.000000 dash_discord-0.0.2/dash_discord.egg-info/top_level.txt
+-rw-r--r--   0 pip        (501) staff       (20)     2141 2024-05-31 22:17:03.000000 dash_discord-0.0.2/package.json
+-rw-r--r--   0 pip        (501) staff       (20)       38 2024-05-31 22:17:24.894017 dash_discord-0.0.2/setup.cfg
+-rw-r--r--   0 pip        (501) staff       (20)      695 2024-05-31 21:22:21.000000 dash_discord-0.0.2/setup.py
+drwxr-xr-x   0 pip        (501) staff       (20)        0 2024-05-31 22:17:24.893063 dash_discord-0.0.2/tests/
+-rw-r--r--   0 pip        (501) staff       (20)      920 2024-05-31 21:22:21.000000 dash_discord-0.0.2/tests/test_usage.py
```

### Comparing `dash_discord-0.0.1/PKG-INFO` & `dash_discord-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_discord
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discord Component for the Dash Framework
 Author: Pip Install Python <pipinstallpython@gmail.com>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_discord-0.0.1/README.md` & `dash_discord-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dash_discord-0.0.1/dash_discord/DiscordCrate.py` & `dash_discord-0.0.2/dash_discord/DiscordCrate.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     """A DiscordCrate component.
 
 
 Keyword arguments:
 
 - id (string; optional)
 
-- channel (string; default '355719584830980096')
+- channel (string; default '1246197743781810332')
 
-- server (string; default '299881420891881473')"""
+- server (string; default '1246197743307980940')"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_discord'
     _type = 'DiscordCrate'
     @_explicitize_args
     def __init__(self, id=Component.UNDEFINED, server=Component.UNDEFINED, channel=Component.UNDEFINED, **kwargs):
         self._prop_names = ['id', 'channel', 'server']
```

### Comparing `dash_discord-0.0.1/dash_discord/DiscordWidget.py` & `dash_discord-0.0.2/dash_discord/DiscordWidget.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,32 +9,34 @@
 
 Keyword arguments:
 
 - id (string; optional)
 
 - avatar (string; optional)
 
-- channel (string; default '355719584830980096')
+- channel (string; default '1246197743781810332')
 
 - className (string; optional)
 
-- server (string; default '299881420891881473')
+- height (string; default '100%')
 
-- style (dict; optional)
+- server (string; default '1246197743307980940')
 
-- username (string; optional)"""
+- username (string; optional)
+
+- width (string; default '100%')"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_discord'
     _type = 'DiscordWidget'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, server=Component.UNDEFINED, channel=Component.UNDEFINED, username=Component.UNDEFINED, avatar=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'avatar', 'channel', 'className', 'server', 'style', 'username']
+    def __init__(self, id=Component.UNDEFINED, server=Component.UNDEFINED, channel=Component.UNDEFINED, username=Component.UNDEFINED, avatar=Component.UNDEFINED, className=Component.UNDEFINED, width=Component.UNDEFINED, height=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'avatar', 'channel', 'className', 'height', 'server', 'username', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'avatar', 'channel', 'className', 'server', 'style', 'username']
+        self.available_properties = ['id', 'avatar', 'channel', 'className', 'height', 'server', 'username', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(DiscordWidget, self).__init__(**args)
```

### Comparing `dash_discord-0.0.1/dash_discord/__init__.py` & `dash_discord-0.0.2/dash_discord/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_discord-0.0.1/dash_discord/dash_discord.min.js` & `dash_discord-0.0.2/dash_discord/dash_discord.min.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -136,73 +136,73 @@
                     border: "none"
                 }
             },
             953: (e, t, r) => {
                 const n = r(16),
                     i = r(609),
                     s = r(264),
-                    o = r(769);
-                class a extends i.PureComponent {
+                    a = r(769);
+                class o extends i.PureComponent {
                     constructor() {
                         super(...arguments), this.state = {
                             url: null,
-                            id: (0, o.generateUUID)()
+                            id: (0, a.generateUUID)()
                         }, this.api = new n.Client({
                             id: this.state.id,
                             iframe: null
                         })
                     }
                     static getDerivedStateFromProps(e, t) {
                         let r = e.shard;
                         r.startsWith("http") || (r = `https://${r}`), r.endsWith("/") && (r = r.substring(0, r.length - 1));
                         let n = Object.assign(Object.assign({}, e.options), {
                             api: t.id
                         });
                         return e.thread && (n.thread = e.thread), e.username && (n.username = e.username), e.avatar && (n.avatar = e.avatar), e.token && (n.token = e.token), e.notifications && (n.notifications = e.notifications), e.notificationTimeout && (n.notificationtimeout = e.notificationTimeout), e.accessibility && (n.accessibility = e.accessibility.join()), e.settingsGroup && (n["settings-group"] = e.settingsGroup), {
-                            url: `${r}/channels/${e.server}${e.channel?`/${e.channel}`:""}/${(0,o.searchParams)(n)}`
+                            url: `${r}/channels/${e.server}${e.channel?`/${e.channel}`:""}/${(0,a.searchParams)(n)}`
                         }
                     }
                     componentDidMount() {
                         const {
                             onAPI: e
                         } = this.props;
                         e && e(this.api)
                     }
                     render() {
                         const {
                             defer: e,
                             className: t,
                             style: r,
                             height: n,
-                            width: o,
-                            focusable: a
+                            width: a,
+                            focusable: o
                         } = this.props;
                         return i.createElement("div", {
                             className: t,
                             style: Object.assign(Object.assign({}, (0, s.Root)({
-                                width: o,
+                                width: a,
                                 height: n
                             })), r)
                         }, i.createElement("iframe", {
                             src: e ? "" : this.state.url,
                             ref: e => this.api.iframe = e,
                             style: s.Embed,
-                            tabIndex: a ? null : -1,
+                            tabIndex: o ? null : -1,
                             allow: "clipboard-write; fullscreen",
                             title: "Discord chat embed"
                         }))
                     }
                 }
-                a.defaultProps = {
+                o.defaultProps = {
                     server: "299881420891881473",
                     shard: "https://e.widgetbot.io",
                     options: {},
                     defer: !1,
                     focusable: !0
-                }, t.A = a
+                }, t.A = o
             },
             769: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.searchParams = t.generateUUID = void 0, t.generateUUID = function() {
                     let e = (new Date).getTime();
                     return "undefined" != typeof performance && "function" == typeof performance.now && (e += performance.now()), "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g, (t => {
@@ -258,122 +258,71 @@
             })
         }), "undefined" != typeof jsonpScriptSrc) {
         var s = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var t, r = (t = i(), /\/_dash-component-suites\//.test(t.src)),
                 n = s(e);
             if (!r) return n;
-            var o = n.split("/"),
-                a = o.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_1m1717191591"), o.splice(-1, 1, a.join(".")), o.join("/")
+            var a = n.split("/"),
+                o = a.slice(-1)[0].split(".");
+            return o.splice(1, 0, "v0_0_1m1717193772"), a.splice(-1, 1, o.join(".")), a.join("/")
         }
     }
-    var o = {};
+    var a = {};
     (() => {
-        r.r(o), r.d(o, {
-            DiscordCrate: () => h,
-            DiscordWidget: () => p
+        r.r(a), r.d(a, {
+            DiscordCrate: () => l,
+            DiscordWidget: () => c
         });
         var e = r(609),
             t = r.n(e);
         const n = window.PropTypes;
         var i = r.n(n),
-            s = r(953);
-
-        function a(e) {
-            return a = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                return typeof e
-            } : function(e) {
-                return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-            }, a(e)
-        }
-
-        function c(e, t) {
-            var r = Object.keys(e);
-            if (Object.getOwnPropertySymbols) {
-                var n = Object.getOwnPropertySymbols(e);
-                t && (n = n.filter((function(t) {
-                    return Object.getOwnPropertyDescriptor(e, t).enumerable
-                }))), r.push.apply(r, n)
-            }
-            return r
-        }
-
-        function l(e) {
-            for (var t = 1; t < arguments.length; t++) {
-                var r = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? c(Object(r), !0).forEach((function(t) {
-                    d(e, t, r[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : c(Object(r)).forEach((function(t) {
-                    Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(r, t))
+            s = r(953),
+            o = function(e) {
+                var r = e.id,
+                    n = e.server,
+                    i = e.channel,
+                    a = e.avatar,
+                    o = e.username,
+                    c = e.className,
+                    d = e.width,
+                    l = e.height;
+                return t().createElement("div", {
+                    id: r,
+                    className: c
+                }, t().createElement(s.A, {
+                    server: n,
+                    channel: i,
+                    username: o,
+                    avatar: a,
+                    width: d,
+                    height: l
                 }))
-            }
-            return e
-        }
-
-        function d(e, t, r) {
-            return (t = function(e) {
-                var t = function(e, t) {
-                    if ("object" != a(e) || !e) return e;
-                    var r = e[Symbol.toPrimitive];
-                    if (void 0 !== r) {
-                        var n = r.call(e, "string");
-                        if ("object" != a(n)) return n;
-                        throw new TypeError("@@toPrimitive must return a primitive value.")
-                    }
-                    return String(e)
-                }(e);
-                return "symbol" == a(t) ? t : t + ""
-            }(t)) in e ? Object.defineProperty(e, t, {
-                value: r,
-                enumerable: !0,
-                configurable: !0,
-                writable: !0
-            }) : e[t] = r, e
-        }
-        var u = function(e) {
-            var r = e.id,
-                n = e.server,
-                i = e.channel,
-                o = e.avatar,
-                a = e.username,
-                c = e.className,
-                d = e.style;
-            return t().createElement("div", {
-                id: r,
-                className: c,
-                style: l(l({}, d), {}, {
-                    height: "50vh",
-                    width: "50vw"
-                })
-            }, t().createElement(s.A, {
-                server: n,
-                channel: i,
-                username: a,
-                avatar: o
-            }))
-        };
-        u.defaultProps = {
-            server: "299881420891881473",
-            channel: "355719584830980096",
+            };
+        o.defaultProps = {
+            server: "1246197743307980940",
+            channel: "1246197743781810332",
             username: null,
             avatar: null,
             className: null,
-            style: {}
-        }, u.propTypes = {
+            width: "100%",
+            height: "100%"
+        }, o.propTypes = {
             id: i().string,
             server: i().string.isRequired,
             channel: i().string.isRequired,
             username: i().string,
             avatar: i().string,
             className: i().string,
-            style: i().object
+            width: i().string,
+            height: i().string
         };
-        const p = u;
-        var f = function(r) {
+        const c = o;
+        var d = function(r) {
             var n = r.id,
                 i = r.server,
                 s = r.channel;
             return (0, e.useEffect)((function() {
                 var e = document.createElement("script");
                 return e.src = "https://cdn.jsdelivr.net/npm/@widgetbot/crate@3", e.async = !0, e.onload = function() {
                         window.Crate = new window.Crate({
@@ -384,19 +333,19 @@
                     function() {
                         document.body.removeChild(e)
                     }
             }), [i, s]), t().createElement("div", {
                 id: n
             })
         };
-        f.defaultProps = {
-            server: "299881420891881473",
-            channel: "355719584830980096"
-        }, f.propTypes = {
+        d.defaultProps = {
+            server: "1246197743307980940",
+            channel: "1246197743781810332"
+        }, d.propTypes = {
             id: i().string,
             server: i().string.isRequired,
             channel: i().string.isRequired
         };
-        const h = f
-    })(), window.dash_discord = o
+        const l = d
+    })(), window.dash_discord = a
 })();
 //# sourceMappingURL=dash_discord.min.js.map
```

### Comparing `dash_discord-0.0.1/dash_discord/dash_discord.min.js.map` & `dash_discord-0.0.2/dash_discord/dash_discord.min.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9067415730337078%*

 * *Differences: {"'mappings'": "'sCACAA,OAAOC,eAAeC,EAAS,aAAc,CAAEC,OAAO,IA8CtDD,EAAA,QA7CA,MACI,WAAAE,GACIC,KAAKC,UAAY,CAAC,CACtB,CACA,WAAAC,CAAYC,GACR,IACI,IAAIC,EAAUC,KAAKC,MAAMH,EAC7B,CACA,MAAOI,GACH,MACJ,CACA,GAAIH,aAAmBT,SACG,IAAtBS,EAAQI,WACRJ,EAAQK,KAAOT,KAAKS,GAAI,CACxB,MAAM,MAAEC,EAAK,KAAEC,GAASP,EAClBH,EAAYD,KAAKC,UAAUS,GAC7BT,GACAA,EAAUW,SAAQC,GAAYA,EAASF,IAE/C,CACJ,CAMA,EAAAG,CAAGJ,EAAOK,GACDf,KAAKC,UAAUS,KAChBV,KAAKC,UAAUS,GAAS,IACVV,KAAKC,UAAUS,GACvBM,KAAKD,GACfE,QAAQC,MAAM,mBAAmBC,OAAOT,MAAWK,EACvD,CAMA,cAA […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_discord.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "Object",
         "defineProperty",
         "exports",
         "value",
         "constructor",
         "this",
@@ -165,15 +165,14 @@
         "chunkId",
         "isLocal",
         "test",
         "srcFragments",
         "fileFragments",
         "splice",
         "DiscordWidget",
-        "_objectSpread",
         "propTypes",
         "PropTypes",
         "isRequired",
         "DiscordCrate",
         "useEffect",
         "onload",
         "Crate",
@@ -211,14 +210,14 @@
         "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.searchParams = exports.generateUUID = void 0;\nfunction generateUUID() {\n    let d = new Date().getTime();\n    if (typeof performance !== 'undefined' &&\n        typeof performance.now === 'function') {\n        d += performance.now(); // use high-precision timer if available\n    }\n    return 'xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx'.replace(/[xy]/g, c => {\n        let r = (d + Math.random() * 16) % 16 | 0;\n        d = Math.floor(d / 16);\n        return (c === 'x' ? r : (r & 0x3) | 0x8).toString(16);\n    });\n}\nexports.generateUUID = generateUUID;\nconst searchParams = (obj = {}) => '?' +\n    Object.keys(obj)\n        .map(k => `${encodeURIComponent(k)}=${encodeURIComponent(obj[k])}`)\n        .join('&');\nexports.searchParams = searchParams;\n//# sourceMappingURL=util.js.map",
         "module.exports = window[\"React\"];",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_1m1717191591\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_1m1717193772\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
-        "import React from 'react';\nimport PropTypes from 'prop-types';\nimport WidgetBot from '@widgetbot/react-embed'\n\nconst DiscordWidget = (props) => {\n    const {id, server, channel, avatar, username, className, style} = props;\n\n    return (\n        <div id={id} className={className} style={{...style, height: '50vh', width: '50vw'}}>\n            <WidgetBot\n                server={server}\n                channel={channel}\n                username={username}\n                avatar={avatar}\n              />\n        </div>\n    );\n}\n\nDiscordWidget.defaultProps = {\n    server: '299881420891881473',\n    channel: '355719584830980096',\n    username: null,\n    avatar: null,\n    className: null,\n    style: {}\n};\n\nDiscordWidget.propTypes = {\n    id: PropTypes.string,\n    server: PropTypes.string.isRequired,\n    channel: PropTypes.string.isRequired,\n    username: PropTypes.string,\n    avatar: PropTypes.string,\n    className: PropTypes.string,\n    style: PropTypes.object\n};\n\nexport default DiscordWidget;\n",
-        "import React, { useEffect } from 'react';\nimport PropTypes from 'prop-types';\n\nconst DiscordCrate = (props) => {\n    const {id, server, channel} = props;\n\n    useEffect(() => {\n        const script = document.createElement('script');\n\n        script.src = \"https://cdn.jsdelivr.net/npm/@widgetbot/crate@3\";\n        script.async = true;\n\n        script.onload = () => {\n            window.Crate = new window.Crate({\n                server: server,\n                channel: channel,\n            });\n        };\n\n        document.body.appendChild(script);\n\n        return () => {\n            document.body.removeChild(script);\n        };\n    }, [server, channel]);\n\n    return <div id={id} />;\n}\n\nDiscordCrate.defaultProps = {\n    server: '299881420891881473',\n    channel: '355719584830980096',\n};\n\nDiscordCrate.propTypes = {\n    id: PropTypes.string,\n    server: PropTypes.string.isRequired,\n    channel: PropTypes.string.isRequired,\n};\n\nexport default DiscordCrate;"
+        "import React from 'react';\nimport PropTypes from 'prop-types';\nimport WidgetBot from '@widgetbot/react-embed'\n\nconst DiscordWidget = (props) => {\n    const {id, server, channel, avatar, username, className, width, height} = props;\n\n    return (\n        <div id={id} className={className}>\n            <WidgetBot\n                server={server}\n                channel={channel}\n                username={username}\n                avatar={avatar}\n                width={width}\n                height={height}\n              />\n        </div>\n    );\n}\n\nDiscordWidget.defaultProps = {\n    server: '1246197743307980940',\n    channel: '1246197743781810332',\n    username: null,\n    avatar: null,\n    className: null,\n    width: '100%',\n    height: '100%',\n};\n\nDiscordWidget.propTypes = {\n    id: PropTypes.string,\n    server: PropTypes.string.isRequired,\n    channel: PropTypes.string.isRequired,\n    username: PropTypes.string,\n    avatar: PropTypes.string,\n    className: PropTypes.string,\n    width: PropTypes.string,\n    height: PropTypes.string,\n};\n\nexport default DiscordWidget;\n",
+        "import React, { useEffect } from 'react';\nimport PropTypes from 'prop-types';\n\nconst DiscordCrate = (props) => {\n    const {id, server, channel} = props;\n\n    useEffect(() => {\n        const script = document.createElement('script');\n\n        script.src = \"https://cdn.jsdelivr.net/npm/@widgetbot/crate@3\";\n        script.async = true;\n\n        script.onload = () => {\n            window.Crate = new window.Crate({\n                server: server,\n                channel: channel,\n            });\n        };\n\n        document.body.appendChild(script);\n\n        return () => {\n            document.body.removeChild(script);\n        };\n    }, [server, channel]);\n\n    return <div id={id} />;\n}\n\nDiscordCrate.defaultProps = {\n    server: '1246197743307980940',\n    channel: '1246197743781810332',\n};\n\nDiscordCrate.propTypes = {\n    id: PropTypes.string,\n    server: PropTypes.string.isRequired,\n    channel: PropTypes.string.isRequired,\n};\n\nexport default DiscordCrate;"
     ],
     "version": 3
 }
```

### Comparing `dash_discord-0.0.1/dash_discord/metadata.json` & `dash_discord-0.0.2/dash_discord/metadata.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891493055555556%*

 * *Differences: {"'src/lib/components/DiscordCrate.react.js'": "{'props': {'server': {'defaultValue': {'value': "*

 * *                                               '"\'1246197743307980940\'"}}, \'channel\': '*

 * *                                               "{'defaultValue': {'value': "*

 * *                                               '"\'1246197743781810332\'"}}}}',*

 * * "'src/lib/components/DiscordWidget.react.js'": "{'props': {'server': {'defaultValue': {'value': "*

 * *                                                '"\'12461977433079 […]*

```diff
@@ -3,15 +3,15 @@
         "description": "",
         "displayName": "DiscordCrate",
         "methods": [],
         "props": {
             "channel": {
                 "defaultValue": {
                     "computed": false,
-                    "value": "'355719584830980096'"
+                    "value": "'1246197743781810332'"
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
@@ -21,15 +21,15 @@
                 "type": {
                     "name": "string"
                 }
             },
             "server": {
                 "defaultValue": {
                     "computed": false,
-                    "value": "'299881420891881473'"
+                    "value": "'1246197743307980940'"
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             }
@@ -50,15 +50,15 @@
                 "type": {
                     "name": "string"
                 }
             },
             "channel": {
                 "defaultValue": {
                     "computed": false,
-                    "value": "'355719584830980096'"
+                    "value": "'1246197743781810332'"
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
@@ -69,47 +69,58 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
+            "height": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'100%'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
             "id": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
             "server": {
                 "defaultValue": {
                     "computed": false,
-                    "value": "'299881420891881473'"
+                    "value": "'1246197743307980940'"
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
-            "style": {
+            "username": {
                 "defaultValue": {
                     "computed": false,
-                    "value": "{}"
+                    "value": "null"
                 },
                 "description": "",
                 "required": false,
                 "type": {
-                    "name": "object"
+                    "name": "string"
                 }
             },
-            "username": {
+            "width": {
                 "defaultValue": {
                     "computed": false,
-                    "value": "null"
+                    "value": "'100%'"
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             }
```

### Comparing `dash_discord-0.0.1/dash_discord/package-info.json` & `dash_discord-0.0.2/dash_discord/package-info.json`

 * *Files identical despite different names*

### Comparing `dash_discord-0.0.1/dash_discord.egg-info/PKG-INFO` & `dash_discord-0.0.2/dash_discord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_discord
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discord Component for the Dash Framework
 Author: Pip Install Python <pipinstallpython@gmail.com>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_discord-0.0.1/package.json` & `dash_discord-0.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.2'"}*

```diff
@@ -51,9 +51,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_discord -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.0.2"
 }
```

### Comparing `dash_discord-0.0.1/setup.py` & `dash_discord-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `dash_discord-0.0.1/tests/test_usage.py` & `dash_discord-0.0.2/tests/test_usage.py`

 * *Files identical despite different names*

