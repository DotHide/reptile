# Reptile

[![Travis](https://img.shields.io/travis/DotHide/reptile.svg?maxAge=2592000)](https://travis-ci.org/DotHide/reptile) 

Reptile is a web spider framework using Ruby.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'reptile'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install reptile

## Usage

```ruby
require('reptile')

Reptile.url("http://www.jd.com/allSort.aspx") do |reptile|
    puts reptile.grab(".category-items .category-item .items dt a")
end
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/DotHide/reptile.

