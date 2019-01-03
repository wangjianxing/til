## intro
  `require ::File.expand_path('../config/environment',  __FILE__)`
  
  It means that you're referring to the constant File from the toplevel namespace. 

## sample

```ruby
class MyClass #1
end

module MyNameSpace
  class MyClass #2
  end

  def foo # Creates an instance of MyClass #1
    ::MyClass.new # If I left out the ::, it would refer to
                  # MyNameSpace::MyClass instead.
  end
end
```

## link
* https://stackoverflow.com/questions/4819312/double-colons-before-class-names-in-ruby