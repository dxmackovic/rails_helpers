# rails_helpers
Solutions to common problems and some edge cases

# fetch values from Hash and set default_value in case key doesn't exist
hash = {a: 4, b: 2}
pp hash.fetch(:c, 0)

