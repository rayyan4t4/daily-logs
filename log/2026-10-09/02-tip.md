# Tech tip — grep with context

Stop re-running `grep` to see the lines around a match. The `-C` flag shows
context in both directions:

```bash
grep -C 3 "error" app.log
```

`-A 3` for lines after, `-B 3` for lines before. Small flag, saves a lot of
scrolling when debugging logs.
