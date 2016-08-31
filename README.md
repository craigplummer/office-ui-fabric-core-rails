# office-ui-fabric-core-rails

[![Gem Version](https://badge.fury.io/rb/office-ui-fabric-core-rails.svg)](https://badge.fury.io/rb/office-ui-fabric-core-rails)

office-ui-fabric-core-rails integrates the [Office UI Fabric Core](https://github.com/OfficeDev/office-ui-fabric-core) framework from Microsoft into the Rails Asset Pipeline.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'office-ui-fabric-core-rails'
```
If you want to include the [Fabric JS components](http://dev.office.com/fabric/components) from the [Office UI Fabric JS](https://github.com/OfficeDev/office-ui-fabric-js) framework. You should also include:

```ruby
gem 'office-ui-fabric-js-rails'
```

And then execute:

    bundle

## Usage

### Add Office UI Fabric to your CSS

#### CSS

Add the following line to the end of your `app/assets/stylesheets/application.css` file:

```
*= require fabric
```

#### Sass

If you are using Sass then you can add the following to your application.scss instead:

```
@import "Fabric";
```

### Using Office UI JS Components

For instructions on how to use the Office UI Fabric JS Components see: https://github.com/craigplummer/office-ui-fabric-js-rails

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/craigplummer/office-ui-fabric-core-rails.

For issues with Office UI Fabric itself please use https://github.com/OfficeDev/office-ui-fabric-core

## License

The [Office UI Fabric](https://github.com/OfficeDev/Office-UI-Fabric) framework and the rest of the office-ui-fabric-core-rails project are licenced under the [MIT License](https://opensource.org/licenses/mit-license.html)
