---
title: Mogrify Images 
date: 2025-05-27
tags: bash
---

# Mogrify Images 

You can use `mogrify` to quickly change a bunch of images. For example, to JPGs to Webp use: 
```bash
mogrify -format webp -quality 80 *.jpg 
```
