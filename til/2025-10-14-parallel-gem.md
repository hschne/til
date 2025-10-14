---
title: Parallel Gem 
date: 2025-10-14
tags: ruby
---

TIL you can use the parallel gem to easily parallelize work into separate threads. Very handy for IO bound scripts and such.

```ruby
Parallel.each(events_to_geocode, in_threads: 5) do |event|
  process_event(event, api_key, options[:overwrite])
end
```
