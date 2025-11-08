# List
An array.

**Type**: `list[T]` or `typing.List[T]`.

```python
items: list[str] = [
    "apple",
    "banana",
    "pickles"
]
print(items[0])  # "apple"
print(items[2])  # "pickles"
```

```python
# You can have multiple types.
combined: list[str | int] = [
    1,
    2,
    "hello",
    "world",
    -10
]
```
