## Install

  `gem install thor`

## Sample
```ruby
# my_app.rb
require "thor"

class MyApp < Thor
  desc "hello", "Say hello"
  def hello(name)
    puts "Hello #{name}"
  end

  desc "gogo", "gogo"
  def gogo
    puts "gogo"
  end
end

MyApp.start(ARGV)
```

* Usage 

  `ruby my_app.rb hello abc123`

## Links
  https://github.com/erikhuda/thor/wiki

  https://www.sitepoint.com/ruby-command-line-interface-gems/