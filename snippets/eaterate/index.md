# eaterate
Use the `eaterate` API for a unified Python iterator experience.

```python
from eaterate import eater

ids = eater("hello").map(ord)
print(ids.fold(lambda prev, curr: prev + curr))  # 532
```
