---
title: Ruby Shellsplit 
date: 2025-06-02
tags: ruby
---

# Shellsplit 

You can split any string into an array using the same splitting rules as a Unix Bourne shell. 

```ruby
argv = 'here are "two words"'.shellsplit
argv #=> ["here", "are", "two words"]
```
