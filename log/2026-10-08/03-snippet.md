# Snippet — 2026-10-08

Flatten a nested list in one line:

```python
nested = [[1, 2], [3, 4], [5]]
flat = [x for sub in nested for x in sub]
print(flat)  # [1, 2, 3, 4, 5]
```
