# Logging

If we are using ActiveModel::Serializers on Rails app by default the `Rails.logger` will be used.

On a non Rails enviroment by default the `ActiveSupport::TaggedLogging` will be
used.

If we need to customize the logger we can define this in an initializer:

```ruby
ActiveModelSerializers.logger = Logger.new(STDOUT)
```
