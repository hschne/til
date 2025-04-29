---
title: Difference Between Turbo Replace and Turbo Update
date: 2025-04-29
tags: hotwire, rails
---

# Difference Between Turbo Replace and Turbo Update

Turbo/Hotwire provides `broadcast_update` and `broadcast_replace`. The difference between those methods is that `update` replaces the content _inside_ the turbo-frame, while `replace` replaces the _entire_ turbo-frame.

Essentially, `update` replaces the inner HTML of the frame, `replace` the outer HTML.
