# test
```html
<body>
    <script>
        Object.defineProperties(Object.prototype, {
            _: {
                value: function (f) {
                    return f instanceof Function ? this instanceof Promise ? this.then(f).then(v => v ?? this) : f(this) ?? this : f instanceof Array ? f.length > 0 ? [...f, ...this] : this instanceof Array ? this.slice(1) : [] : f
                }
            }
        })
            ._([])
            ._([document.createElement('input')])
            ._(([_]) => (_.placeholder = 'TYPE ENTER TO BASE64 ENCODE')._())
            ._([document.createElement('code')])
            ._(([_]) => (_.style.wordBreak = 'break-all')._())
            ._(([_, $]) => ($.style.width = _.style.width = '100%')._())
            ._(([$, _]) => (_.onchange = _ => _._(_ => _.target.value)._(_ => btoa(_))._(_ => $.innerText = _))._())
            ._(([_, $]) => document.body.replaceChildren($, _))
            ._([])
            ._([])
    </script>
</body>
```
