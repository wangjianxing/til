# infinity
## code
```ruby
# >=201
201..Float::INFINITY

# rails5
3.days.ago..DateTime::Infinity.new

# >=201 with ruby 2.6
201..

```

## links
* https://stackoverflow.com/questions/11317662/rails-using-greater-than-less-than-with-a-where-statement

# &.(ampersand dot)
## code
  It is called the Safe Navigation Operator. Introduced in Ruby 2.3.0, it lets you call methods on objects without worrying that the object may be nil(Avoiding an undefined method for nil:NilClass error), similar to the [try method in Rails](https://api.rubyonrails.org/classes/Object.html#method-i-try).
```ruby
@person&.spouse&.name

means

@person.spouse.name if @person && @person.spouse
```

## links
* https://stackoverflow.com/questions/36812647/what-does-ampersand-dot-mean-in-ruby
* https://api.rubyonrails.org/classes/Object.html#method-i-try