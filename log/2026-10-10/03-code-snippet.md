# Sat, Oct 10 2026 — code snippet

**Small Python: count lines of code in a directory**

```python
from pathlib import Path

def count_lines(root, exts=(".py", ".md", ".js")):
    total = 0
    for p in Path(root).rglob("*"):
        if p.suffix in exts and p.is_file():
            total += sum(1 for _ in p.open(errors="ignore"))
    return total

print("lines:", count_lines("."))
```

Handy before refactoring — gives you a quick sense of how big a
codebase (or folder) actually is.
