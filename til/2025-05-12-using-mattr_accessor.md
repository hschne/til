---
title: Using mattr_accessor
date: 2025-05-12
tags: ruby, rails
---

ActiveSupport provides the `mattr_accessor` method, which defines both class and instance accessors for class attributes.

```ruby
module HairColors
  mattr_accessor :hair_colors, default: [:brown, :black, :blonde, :red]
end

class Person
  include HairColors
end

HairColors.hair_colors = [:brown, :black, :blonde, :red]
Person.new.hair_colors # => [:brown, :black, :blonde, :red]
Person.new.hair_colors = [:pink]
HairColors.hair_colors # => [:pink]
Person.new.hair_colors # => [:pink]
```

Source: [APIDock Rails](https://apidock.com/rails/Module/mattr_accessor)
