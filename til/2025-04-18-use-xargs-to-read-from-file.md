---
title: Use Xargs to Read From File
date: 2025-04-18
tags:
---

# Use Xargs to Read From File

When one script returns a file path, and you need to use the contents of that file
in some other script, you can use some `xargs` magic.

```bash
# til returns a file path, but we want to append the contents of that file
# to some other file
til -d ~/Source/til/til | xargs -I{} cat {} >> ~/Documents/other-file.md"
```
