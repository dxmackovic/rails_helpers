# rails_helpers
Solutions to common problems and some edge cases

# fetch values from Hash and set default_value in case key doesn't exist
hash = {a: 4, b: 2}
pp hash.fetch(:c, 0)

# check hash has value
person = { name: "John", age: 30 }
hash.value?(30) # true
hash.value?(45) # false


# list all TODO and FIXME Rails tasks
bin/rails notes
bin/rails notes --help


# search JSONB object
# () are important to include the array
Account.where("metadata ->> 'reffered_by' IN (?)", ['Social Media']).count


# start rails jobs
rake jobs:work
