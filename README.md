# Standard Ruby Styleguide

We've started writing our Ruby code in the same way we do our JavaScript code and we've never been happier. We call this approach `srs`, because we're totally serious.

#### Semicolons
End all your statements with semicolons. Semicolons are optional, but you should always put them in for consistency. Semicolons are fine in Ruby. All Ruby interpreters like MRI, Rubinius and JRuby will be able to parse your code correctly.

```rb
def create_user(name)
  user = User.create({ name: name });
  user.validate!();
  user.save();
end
```

### Use parentheses
Although parentheses are optional in Ruby, prefer to always put them so that your code will be consistent.

```rb
# ✓ OK
if model.valid?()
  return false
end
  ```

```rb
# ✓ Avoid
if model.valid?
  return false
end
```

----

> This document is satire, in case you haven't picked up on that yet. If you want a real styleguide, look at [bbatsov/ruby-style-guide](https://github.com/bbatsov/ruby-style-guide).