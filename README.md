!function() {
    try {
        var e = "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {}
          , t = (new Error).stack;
        t && (e._sentryDebugIds = e._sentryDebugIds || {},
        e._sentryDebugIds[t] = "96c23dce-27ea-406e-8c31-f85ca084fd04",
        e._sentryDebugIdIdentifier = "sentry-dbid-96c23dce-27ea-406e-8c31-f85ca084fd04")
    } catch (e) {}
}();
var _global = "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
_global.SENTRY_RELEASE = {
    id: "4.7.0"
},
( () => {
    function e(e, n) {
        var r = "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
        if (!r) {
            if (Array.isArray(e) || (r = function(e, n) {
                if (e) {
                    if ("string" == typeof e)
                        return t(e, n);
                    var r = {}.toString.call(e).slice(8, -1);
                    return "Object" === r && e.constructor && (r = e.constructor.name),
                    "Map" === r || "Set" === r ? Array.from(e) : "Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r) ? t(e, n) : void 0
                }
            }(e)) || n && e && "number" == typeof e.length) {
                r && (e = r);
                var o = 0
                  , i = function() {};
                return {
                    s: i,
                    n: function() {
                        return o >= e.length ? {
                            done: !0
                        } : {
                            done: !1,
                            value: e[o++]
                        }
                    },
                    e: function(e) {
                        throw e
                    },
                    f: i
                }
            }
            throw new TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
        }
        var l, c = !0, a = !1;
        return {
            s: function() {
                r = r.call(e)
            },
            n: function() {
                var e = r.next();
                return c = e.done,
                e
            },
            e: function(e) {
                a = !0,
                l = e
            },
            f: function() {
                try {
                    c || null == r.return || r.return()
                } finally {
                    if (a)
                        throw l
                }
            }
        }
    }
    function t(e, t) {
        (null == t || t > e.length) && (t = e.length);
        for (var n = 0, r = Array(t); n < t; n++)
            r[n] = e[n];
        return r
    }
    !function(t) {
        var n = null;
        function r(e) {
            var t, r, o;
            e && e.detail && e.detail.code && (e.stopImmediatePropagation(),
            t = e.detail.code,
            r = document.createElement("script"),
            (o = document.querySelector("link[nonce], style[nonce], script[nonce]")) && o.nonce && r.setAttribute("nonce", o.nonce),
            r.textContent = n ? n.createScript(t) : t,
            (document.head || document.documentElement).append(r),
            r.remove())
        }
        function o() {
            var t, n = e(document.querySelectorAll("lt-mirror:not([data-lt-linked]), lt-highlighter:not([data-lt-linked])"));
            try {
                var r = function() {
                    var e = t.value;
                    if (!e.nextElementSibling || !e.nextElementSibling.hasAttribute("data-lt-tmp-id"))
                        return 1;
                    var n = e.nextElementSibling;
                    e.setAttribute("data-lt-linked", "1");
                    for (var r = function() {
                        var t = i[o];
                        try {
                            Object.defineProperty(e, t, {
                                get: function() {
                                    return n[t]
                                },
                                set: function(e) {
                                    n[t] = e
                                }
                            })
                        } catch (e) {}
                    }, o = 0, i = ["selectionStart", "selectionEnd", "value", "textContent", "innerHTML", "innerText", "required", "maxLength", "disabled", "readOnly", "contentEditable", "isContentEditable"]; o < i.length; o++)
                        r()
                };
                for (n.s(); !(t = n.n()).done; )
                    r()
            } catch (e) {
                n.e(e)
            } finally {
                n.f()
            }
        }
        null !== (t = self.trustedTypes) && void 0 !== t && t.createPolicy && (n = self.trustedTypes.createPolicy("QB_Executor_Policy", {
            createScript: function(e) {
                return e
            }
        })),
        document.addEventListener("lt-execute-link-properties", o),
        document.addEventListener("lt-execute-code", r),
        document.addEventListener("lt-execute-destroy", (function e() {
            document.removeEventListener("lt-execute-destroy", e),
            document.removeEventListener("lt-execute-link-properties", o),
            document.removeEventListener("lt-execute-code", r)
        }
        ))
    }()
}
)();
//# sourceMappingURL=sourceMap/executor.js.map
# news
