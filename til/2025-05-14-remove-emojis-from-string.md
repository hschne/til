---
title: Remove Emojis From String
date: 2025-05-14
tags: ruby
---

# Remove Emojis From String

You can remove Emojis from a Ruby string using regex character properties. There is the `\p{Emoji}` property, which unfortunately behaves strangely. Alternatively, use the undocumented `\p{Emoji_Presentation}` or `\p{So}` to remove any Unicode symbols.

```ruby
p "Germany 🇩🇪".gsub(/\p{Emoji}/, '')
p "Austria 🇦🇹".gsub(/\p{Emoji_Presentation}/, '')
p "Switzerland 🇨🇭".gsub(/\p{So}/, '')
```

Source: [StackOverflow](https://stackoverflow.com/a/64997179), [Ruby Doc](https://ruby-doc.org/3.2.0/Regexp.html#class-Regexp-label-Character+Properties)
