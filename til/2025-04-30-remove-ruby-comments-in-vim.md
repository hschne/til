---
title: Remove Ruby Comments in Vim
date: 2025-04-30
tags:
---

# Remove Ruby Comments in Vim

AI likes to add a lot of comments. In case you forget to tell it not to, here's how you can quickly remove Ruby comments using normal mode in Vim.

```vim
g/^\s.*#/norm dd
```

This also works nicely for visual selections.
