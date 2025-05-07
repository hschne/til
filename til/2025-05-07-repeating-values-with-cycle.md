---
title: Repeating Values With Cycle
date: 2025-05-07
tags:
---

# Repeating Values With Cycle

You can generate a looping set of values easily with the `cycle` method. Cycle returns a new enumerator that you can call `next` on

```ruby
@cycle = %w[first second third].cycle
@cycle.next
# => first
@cycle.next
# => second
@cycle.next
# => third
@cycle.next
# => first
```

Source: [APIDock](https://apidock.com/ruby/v2_5_5/Enumerable/cycle)
