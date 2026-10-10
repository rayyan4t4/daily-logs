# Sat, Oct 10 2026 — tech tip

**Tip: `git log` with `--oneline --graph` for a quick repo overview**

When you land in an unfamiliar repo, run:

```bash
git log --oneline --graph -n 20 --all
```

It shows the last 20 commits across all branches as a compact tree — the
fastest way to see what changed recently and how branches relate. Add
`--decorate` to also show branch and tag names next to commits.
