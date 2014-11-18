# Linkify

Linkify urls in an Ember app with a helper and/or component. This uses a tested
[url-regex](https://github.com/kevva/url-regex) and Handlebars `Utils.escapeExpression`
to ensure links are safe.

Integrates with [ember-cli](http://ember-cli.com).

## Installation

```
npm i --save-dev ember-linkify
ember g ember-linkify
```

## Usage

Use the helper:

```hbs
{{linkify 'Here is a link: https://google.com and some attempted XSS <script>alert("xss!");</script>'}}
```

The proposed usage of the component, which is coming soon:

```hbs
{{linkify-component text=descriptionText}}
```

## Development

### Installation

* `git clone` this repository
* `npm install`
* `bower install`

### Running

* `ember server`
* Visit your app at http://localhost:4200.

### Running Tests

* `ember test`
* `ember test --server`

### Building

* `ember build`

For more information on using ember-cli, visit [http://www.ember-cli.com/](http://www.ember-cli.com/).

## License

MIT

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

Crafted with <3 by [John Otander](http://johnotander.com)([@4lpine](https://twitter.com/4lpine)).