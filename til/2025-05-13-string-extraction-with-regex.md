---
title: String Extraction With Regex
date: 2025-05-13
tags: ruby
---

# String Extraction With Regex

You may use a Regex expression with capture groups to extract parts of a string in Ruby.

```ruby
# Extract the event name
url = "www.meetup.com/vienna-rb/events/307283556/"
group = url[%r{meetup\.com/([^/]+)/events}, 1]
```
