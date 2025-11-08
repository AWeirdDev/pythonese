# Drain
Drain items in a list without preserving the order.

```python
items: list[int] = [1, 2, 3]

while len(items):
    drained = items.pop()
    print(drained)
```

> [!NOTE]
> It's not recommended to use `.pop(0)` as this operation requires reordering the list.
> You could use a `deque()` instead, but draining is not a common operation in Python.
