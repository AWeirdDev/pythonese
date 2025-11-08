# Slicing
You can take a part of a list. This is called "slicing."

**Syntax**: `some_list[start?:stop?:step?]`

- `start`: The index to start.
- `stop`: When reached/over this index number, immediately stops. In other words, this is not inclusive. Can be assigned with a negative value.
- `step`: The step. If assigned `2`, it only yields every 2 items; if assigned `-1`, it starts from the end.

If none of the above (`start`, `stop`, or `step`) is given, the list is copied.

**`[:]` (`[::]`) - Copying behavior**

```python
a = [1, 2, 3, 4, 5]
copied_a = a[:]

print(a is copied_a)  # False
print(id(a) == id(copied_a))  # False

a[0] = -10
print(copied_a[0])  # 1
```

<br />

**`[start:]` - Starts from `start` until the end**

```python
a = [1, 2, 3, 4, 5]
slice = a[2:]  # starts at index 2

print(slice)  # [3, 4, 5]
```

<br />

**`[:end]` - Starts from `0` until reaches/over `end`**

```python
a = [1, 2, 3, 4, 5]
slice = a[:3]  # halts at index 3

print(slice)  # [1, 2, 3]
```

<br />

**`[start::step]` - Starts from `start` until the end, stepping by `step`**

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
slice = a[2::2]  # starts at index 2

print(slice)  # [3, 5, 7, 9]
```

<br />

**`[:end:step]` - Starts from `0` until reaches/over `end`, stepping by `step`**

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
slice = a[:7:2]  # halts when reached or over `end`

print(slice)  # [1, 3, 5, 7]
```

**`[start:end:step]` - Starts from `start` until reaches/over `end`, stepping by `step`**

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
slice = a[1:2:3]

print(slice)  # [2]
```
