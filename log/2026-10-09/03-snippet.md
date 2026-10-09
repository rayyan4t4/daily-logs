# Snippet — safe markdown file counter

Counts markdown files in a directory tree without tripping on odd names:

```python
from pathlib import Path

def count_markdown(root: str) -> int:
    return sum(1 for p in Path(root).rglob("*.md") if p.is_file())

if __name__ == "__main__":
    print(count_markdown("."))
```
