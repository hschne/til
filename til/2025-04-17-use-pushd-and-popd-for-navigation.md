---
title: Use Pushd and Popd for Navigation
date: 2025-04-17
tags: bash
---

# Use Pushd and Popd for Navigation

You can use `pushd` and `popd` for quick navigation in your shell scripts. You can also use the `dirs` command to show what is currently on your directory stack 👀

```bash
pushd "$GIT_REPO" >/dev/null
if git rev-parse --is-inside-work-tree >/dev/null 2>&1; then
  # Do stuff
fi

# Return to original directory
popd >/dev/null
```
