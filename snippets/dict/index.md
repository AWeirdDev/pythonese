# Dict
Dictionaries serve as an efficient in-memory key-value store in Python.
Dictionary lookups are O(1), while O(N) for lists.

However, it doesn't mean it's always necessary to build a dictionary.
For simple lookups (say, only ~10 items), it's highly recommended to use a list
(array) instead, as arrays are the core building blocks of a hashmap (dictionary).
Using a list for simple scenarios can reduce overhead.

**Type**: `dict[K, V]` or `typing.Dict[K, V]`.

```python
profile: dict[str, str] = {
    "name": "Walter White",
    "description": "The chemist. The teacher.",
    "companion": "Jesse Pinkman"
}
```

## References
- [Update](./update.md)
- [Indexing](./indexing.md)
