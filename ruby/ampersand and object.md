# ampersand and object

## code
```ruby
some_objects.each(&:foo)
#It's the same as
some_objects.each { |obj| obj.foo }
```

## intro
- The & calls `to_proc` on the object and passes it as a block to the method, and Ruby implements `to_proc` on `Symbol`.

## links
- https://stackoverflow.com/questions/1961030/ruby-ampersand-colon-shortcut