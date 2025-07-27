---
title: Git Blame Ignore Revs 
date: 2025-07-27
tags: git
---

# Git Blame Ignore Revs 

When making bulk formatting changes (e.g. with RuboCop) you generally don't want those changes to show up in git blame/change sets in PR reviews. A `.git-blame-ignore-revs` tells git to ignore changes from specific revisions.

```bash
touch .git-blame-ignore-revs
echo "<commit-hash>" >> .git-blame-ignore-revs
git config blame.ignoreRevsFile .git-blame-ignore-revs
```

