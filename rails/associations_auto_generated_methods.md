# associations
```ruby
class Project < ActiveRecord::Base
  belongs_to              :portfolio
  has_one                 :project_manager
  has_many                :milestones
  has_and_belongs_to_many :categories
end
```

### Singular associations (one-to-one)

|generated methods|belongs_to|belongs_to:polymorphic|has_one|
|:----    |:---|:----- |-----   |
other                             |     X      |      X       |    X
other=(other)                     |     X      |      X       |    X
build_other(attributes={})        |     X      |              |    X
create_other(attributes={})       |     X      |              |    X
create_other!(attributes={})      |     X      |              |    X
reload_other                      |     X      |      X       |    X


### Collection associations (one-to-many / many-to-many)

|generated methods|habtm|has_many|has_many:through|
|:----    |:---|:----- |-----   |
others                            |   X   |    X     |    X
others=(other,other,...)          |   X   |    X     |    X
other_ids                         |   X   |    X     |    X
other_ids=(id,id,...)             |   X   |    X     |    X
others<<                          |   X   |    X     |    X
others.push                       |   X   |    X     |    X
others.concat                     |   X   |    X     |    X
others.build(attributes={})       |   X   |    X     |    X
others.create(attributes={})      |   X   |    X     |    X
others.create!(attributes={})     |   X   |    X     |    X
others.size                       |   X   |    X     |    X
others.length                     |   X   |    X     |    X
others.count                      |   X   |    X     |    X
others.sum(*args)                 |   X   |    X     |    X
others.empty?                     |   X   |    X     |    X
others.clear                      |   X   |    X     |    X
others.delete(other,other,...)    |   X   |    X     |    X
others.delete_all                 |   X   |    X     |    X
others.destroy(other,other,...)   |   X   |    X     |    X
others.destroy_all                |   X   |    X     |    X
others.find(*args)                |   X   |    X     |    X
others.exists?                    |   X   |    X     |    X
others.distinct                   |   X   |    X     |    X
others.reset                      |   X   |    X     |    X
others.reload                     |   X   |    X     |    X

### links
* https://stackoverflow.com/questions/2472982/using-build-with-a-has-one-association-in-rails
* https://api.rubyonrails.org/classes/ActiveRecord/Associations/ClassMethods.html#M001834