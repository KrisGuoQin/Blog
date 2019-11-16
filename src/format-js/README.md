当我们和后端对接的时候可能会碰到这种情况，后端给了我们接口的注释，可能是下面这种形式的。

```javascript
{
    'foo': '注释1',
    'bar': '注释2',
    ...
}
```

我们可能需要转化成下面这种形式

```javascript
[
    {
        label: '注释1',
        prop: 'foo'
    },
    {
        label: '注释1',
        prop: 'foo'
    },
]
```
这样我们就可以循环显示了。