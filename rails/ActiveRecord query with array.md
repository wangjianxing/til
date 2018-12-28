## ways
* return Relation
```ruby
Model.where('id IN (?)', [array of values])

Model.where(id: [array of values])
```

* return Array
```ruby
results = Model.find([1,2,3], :order => "id") # ascending order

results = Model.find([1,2,3], :order => "id desc") # descending order
```

## links

https://stackoverflow.com/questions/28954500/activerecord-where-field-array-of-possible-values

https://stackoverflow.com/questions/2129824/rails-activerecord-return-order-with-activerecordfindarray