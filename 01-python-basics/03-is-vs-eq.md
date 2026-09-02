# `is`、`==` 与 `id()`

> `is` 判断是否为同一个对象，`==` 判断值是否相等，`id()` 是观察对象身份的工具。

```python
a = [1, 2]
b = [1, 2]
c = a

assert a == b
assert a is not b
assert a == c
assert a is c
```

`None` 是单例对象，因此推荐这样判断：

```python
if value is None:
    ...
```

