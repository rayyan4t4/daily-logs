# Tech fact — Git stores snapshots, not diffs

Popular belief: Git stores the diff between versions. Reality: each commit
stores full snapshots of every file, and diffs are computed on demand when
you run `git log -p` or `git show`.

That's why `git checkout` is so fast — it's just restoring a tree, not
replaying patches.
