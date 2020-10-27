# FastWhile

### clean code
This gem extends the Array and Hash classes by adding a while method for arrays.
The method repeats the loop while most of it is used while remaining inside the given method, which allows for cleaner code using the capabilities of a regular while loop.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'fast_while'

or

gem 'fast_while', '0.1.1.beta', git: "https://github.com/rubywarlock/fast_while"
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install fast_while
    or
    $ gem install rubywarlock-fast_while, -s "https://github.com"

## Usage
```
["one", "two"].while do |el, index|
  puts "#{el}, #{index}"
end
```

#### for a hash, it is currently required to specify two parameters, if you need not only a key but also a value
```
{one: "VALUE"}.while do |key, value|
  puts "#{key}, #{value}"
end
```
## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake test` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/rubywarlock/fast_while.


## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
