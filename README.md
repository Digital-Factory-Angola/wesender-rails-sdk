# Wesender - RubyOnRails application integration library
## Installation

[Oficial doc](https://rubygems.org/gems/wesender).
Add this line to your application's Gemfile:

```ruby
gem 'wesender'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install wesender

## Setup and Usage
Make sure you setup the environment variables WESENDER_API_KEY:

```ruby
WESENDER_API_KEY='your_api_key' 
our
WesenderSMS.new(api_key)

test = WesenderSMS.new

numbers: Array
message: String
hasSpecialCharacter: Boolean // opcional, by default is false

test.send(numbers, message, hasSpecialCharacter)
```

```ruby
Eg: test.send(["913000111"], "Hello Angola")
```

```js
# response
{
 "Exito" : Boolean ,
 "Mensagem" : String,
 "Objeto" :
   {
     // quantity of message that you can send
     "SMS" : Number,
     "WhatsApp" : Number,
     "FacebookMesseger" : Number,
     "Integracoes" : Number,
   }
}
```

## License
[MIT License](https://opensource.org/licenses/MIT).

## Author

[JM Cabanga](https://github.com/cabanga).
