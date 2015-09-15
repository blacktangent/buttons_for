[travis]: https://travis-ci.org/blacktangent/buttons_for
[codeclimate]: https://codeclimate.com/github/blacktangent/buttons_for
[fontawesome]: https://fortawesome.github.io/Font-Awesome
[fontawesomerails]: https://github.com/bokmann/font-awesome-rails
[coveralls]: https://coveralls.io/r/blacktangent/buttons_for

# ButtonsFor

[![Build Status](https://travis-ci.org/blacktangent/buttons_for.svg?branch=master)][travis]
[![Code Climate](https://codeclimate.com/github/blacktangent/buttons_for/badges/gpa.svg)][codeclimate]
[![Test Coverage](http://img.shields.io/coveralls/blacktangent/buttons_for/master.svg)][coveralls]

ActiveView helper to generate Bootstrap buttons and dropdown-buttons.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'buttons_for'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install buttons_for

Run generator to add I18n locales:

    $ rails generate buttons_for:install

The gem depends on [Bootstrap 3](http://getbootstrap.com/) to create buttons and dropdown-buttons. Bring bootstrap into
your project by using [Bootstrap for Sass](https://github.com/twbs/bootstrap-sass) or you preferred method.

`buttons_for` depends on [Font Awesome][fontawesome] icon and CSS
framework, bring [Font Awesome][fontawesome] into your project using
[font-awesome-rails][fontawesomerails] or your preferred method.

## Sample Application

Sample Application using `buttons_for` can be found
[here](https://github.com/blacktangent/rails-buttons_for)

## Usage

```erb
<%= buttons_for @project do |b| %>
  <%= b.button :complete, new_project_complete_path(@project), icon: "check" %>
  <%= b.new %>
  <%= b.edit %>
  <%= b.delete %>
<% end %>
```

## Options

Available options:

* __:label__ - Override standard label

## Sample

Sample applicaiton using `buttons_for` can be found
[here](https://github.com/blacktangent/buttons_for).

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake rspec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/blacktangent/buttons_for. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

