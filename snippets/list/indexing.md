# Indexing
Use the syntax `some_list[n]` to index into a list. Under the hood, the `__getitem__` method is called.
Lists in Python are zero-indexed.


```python
fruits = [
    "apple", "banana", "guava"
]

print(fruits[0])  # "apple"
print(fruits[2])  # "guava"
```
