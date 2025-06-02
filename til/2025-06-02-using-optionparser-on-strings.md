---
title: Using Optionparser On Strings 
date: 2025-06-02
tags: ruby
---

# Using Optionparser On Strings 

OptionsParser is generally used to parse options for command line scripts. However, you can also use it to parse arbitrary strings. 

```ruby
def parse_arguments_from_string(arg)
  args = arg.to_s.shellsplit

  options = {}
  OptionParser.new do |opts|
    opts.on("-e", "--email EMAIL", "User email") do |email|
      options[:email] = email
    end
    opts.on("-a", "--admin", "Make user admin") do |admin|
      options[:admin] = true
    end
  end.parse!(args)
end

parse_arguments_from_string "-e hello@hansschnedlitz.com --admin"
# => {email: "hello@test.com", admin: true}
```
