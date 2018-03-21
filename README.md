# CamelCase JS

> String to CamelCase or CamelCase to string: `foo-bar` ⇄ `fooBar`


## Install

```
$ npm install --save camelcasejs
```

## CamelCase
### Strings
```js
const { CamelCase } = require('camelcasejs');

CamelCase('foo-bar');
// Response = 'fooBar'

CamelCase('foo_bar');
// Response = 'fooBar'

CamelCase('Foo-Bar');
// Response = 'fooBar'

CamelCase('--foo.bar');
// Response = 'fooBar'

CamelCase('__foo__bar__');
// Response = 'fooBar'

CamelCase('foo bar');
// Response = 'fooBar'
```
### Array
```js
const { CamelCase } = require('camelcasejs');

CamelCase(['foo', 'bar']);
// Response = 'fooBar'
```

## DeCamelize
```js
const { DeCamelize } = require('camelcasejs');

DeCamelize('fooBar');
// Response = 'foo_bar'

DeCamelize('fooBarV9_2');
// Response = 'foo_bar_v9.2'

/* Custom separator */
DeCamelize('fooBar', '=');
// Response = 'foo=bar'

DeCamelize('fooBarV9_2', '-');
// Response = 'foo-bar-v9.2'
```

## License

MIT © [Julio Sansossio](https://github.com/Sansossio)