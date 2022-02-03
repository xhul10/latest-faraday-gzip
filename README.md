# Faraday Gzip

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/lostisland/faraday-gzip/ci)](https://github.com/lostisland/faraday-gzip/actions?query=branch%3Amain)
[![Gem](https://img.shields.io/gem/v/faraday-gzip.svg?style=flat-square)](https://rubygems.org/gems/faraday-gzip)
[![License](https://img.shields.io/github/license/lostisland/faraday-gzip.svg?style=flat-square)](LICENSE.md)

The `Gzip` middleware adds the necessary `Accept-Encoding` headers and automatically decompresses the response.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'faraday-gzip'
```

And then execute:

```shell
bundle install
```

Or install it yourself as:

```shell
gem install faraday-gzip
```

## Usage

```ruby
require 'faraday/gzip'

conn = Faraday.new(...) do |f|
  f.request :gzip
  #...
end
```

## Development

After checking out the repo, run `bin/setup` to install dependencies.

Then, run `bin/test` to run the tests.

To install this gem onto your local machine, run `rake build`.

To release a new version, make a commit with a message such as "Bumped to 0.0.2" and then run `rake release`.
See how it works [here](https://bundler.io/guides/creating_gem.html#releasing-the-gem).

## Contributing

Bug reports and pull requests are welcome on GitHub.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).