---
title: Undo File Changes in Branch 
date: 2025-06-18
tags: git
---

# Undo File Changes in Branch 

I often end up making changes to files in a branch that I want to get rid of before opening a PR. This is a simple command to undo all changes to a specific file.

```bash
git checkout main -- path/to/file.rb
```
