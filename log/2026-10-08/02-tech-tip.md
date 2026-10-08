# Tech tip — 2026-10-08

`git log --oneline --graph --all` gives you a compact visual history of every branch.

Add it as an alias and you will never type the long form again:

```bash
git config --global alias.lg "log --oneline --graph --all"
```
