---
title: Attach TTY to Editor
date: 2025-04-18
tags: bash, scripts
---

# Attach TTY to Editor

When opening a command line editor (such as Nvim) in a script, attach TTY
to the editor in order to be able to edit the file.

```bash
$EDITOR "$filepath" <$(tty) >$(tty)
```
