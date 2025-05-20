---
title: Activesupport Inflections 
date: 2025-05-20
tags: 
---

# Activesupport Inflections 

You may configure how ActiveSupport pluralizes some words. This is needed when you're dealing with irregular words - such as Bonus.

```ruby
# config/initializers/inflections.rb
ActiveSupport::Inflector.inflections do |inflect|
  inflect.irregular 'bonus', 'bonuses'
end
```

Without adding the above, generating classes with that name results in interesting behaviour.

```ruby
# Generating a model 'bonus' yields unexpected results
# rails g model bonus

# ???
class Bonu < ApplicationRecord
  # ...
end
```
