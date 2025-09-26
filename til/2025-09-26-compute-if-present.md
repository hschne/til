---
title: Compute If Present 
date: 2025-09-26
tags: ruby
---

# Compute If Present 

`Concurrent::Map` provides a `compute_if_present` method that can be used to recalculate a value if it's key is present, as seen in the SolidCable source.

```ruby
map.compute_if_present(key) do |old_value|
  calculate_new_value
end
```

Source: [RubyDocs](https://ruby-concurrency.github.io/concurrent-ruby/1.1.7/Concurrent/Map.html#compute_if_present-instance_method)
