# Fill
You can use **generators** to fill a list.

```python
items: list[int] = [
    i * 2 for i in range(5)
]

print(items)  # [0, 2, 4, 6, 8]
```

You can also add **if guards** to generators:

```python
by_two: list[int] = [
    i for i in range(5)
    if i % 2 == 0
]

print(by_two)  # [0, 2, 4]
```
