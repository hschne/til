---
title: Use Entr to Watch Files
date: 2025-05-13
tags:
---

# Use Entr to Watch Files

[Entr](https://github.com/eradman/entr) is a small command line utility to run arbitrary commands when files change. Useful to rebuild various artifacts.

```bash
ls stylesheet.css resume.md | entr -s ./build.sh
```
