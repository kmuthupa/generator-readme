# <%= name %>
<% if (isNodeModule) { -%>

[![Build Status][travis-image]][travis-url]
[![npm version][npm-image]][npm-url]
[![License][license-image]][license-url]

[travis-url]: https://travis-ci.org/<%= githubUser %>/<%= name %>
[travis-image]: https://img.shields.io/travis/<%= githubUser %>/<%= name %>.svg
[npm-url]: https://www.npmjs.com/package/<%= name %>
[npm-image]: https://img.shields.io/npm/v/<%= name %>.svg
[license-url]: https://opensource.org/licenses/<%= license %>
[license-image]: https://img.shields.io/npm/l/<%= name %>.svg
<% } -%>

> <%= description %>

<% if (isNodeModule) { -%>
## Installation

```shell
npm install --save <%= name %>
```

## Usage

```js
var <%= camelCaseName %> = require('<%= name %>')
```

<% } -%>
## Author

© <%= year %> <%= author %> <<%= email %>> (<%= website %>)

## License

<% if (license === 'MIT') { -%>
Released under the [MIT license](http://<%= githubUser %>.mit-license.org).
<% } else { -%>
Released under the <%= license %> license.
<% } -%>
