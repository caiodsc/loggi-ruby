# [Loggi](https://github.com/petlove/loggi-ruby)

[![Build Status](https://travis-ci.org/petlove/loggi-ruby.svg?branch=master)](https://travis-ci.org/petlove/loggi-ruby)

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'loggi', github: 'petlove/loggi-ruby'
```

And then execute:U

    $ bundle

## Usage

#### Authentication
You should use the model `Loggi::Crendetial` to generate your `api_key`.
```ruby
credential = Loggi::Credential.new(email: email, password: password)
credential.authenticate!
credential.api_key
# => 14651f0f-8888-4100-9ab7-cf4b2dffb31e
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

## Contributing

Bug reports and pull requests are welcome!

### Remaining Loggi's features
- [~Authentication~](https://docs.api.loggi.com/reference/autorizacao#consultar-api-key)
- [List shops](https://docs.api.loggi.com/reference/lojas#listagem-de-lojas)
- [List packages](https://docs.api.loggi.com/reference/pacotes#listagem-de-pacotes)
- [Package's history](https://docs.api.loggi.com/reference/pacotes#historico-de-pacote)
- [Package's status](https://docs.api.loggi.com/reference/pacotes#status-dos-pacotes)
- [Create an order](https://docs.api.loggi.com/reference/pedidos#criacao-de-pedido)
- [Estimate an order by geolocation](https://docs.api.loggi.com/reference/pedidos#estimar-precos-de-pedido)
- [Estimate an order by package and pickups](https://docs.api.loggi.com/reference/pedidos#estimativa-com-endereco)
- [Remake an order](https://docs.api.loggi.com/reference/pedidos#refazer-um-pedido)
- [Tracking an order](https://docs.api.loggi.com/reference/pedidos#buscar-um-pedido)
- [Edit an order](https://docs.api.loggi.com/reference/pedidos#edi%C3%A7%C3%A3o-de-pedido)

### Other remaining features
- ~Config Travis as a CI~

### Some references
- [Loggi's getting started](https://docs.api.loggi.com/docs/getting-started)
- [Loggi's API Reference](https://docs.api.loggi.com/reference/autorizacao)

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
