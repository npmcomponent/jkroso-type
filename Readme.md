*This repository is a mirror of the [component](http://component.io) module [jkroso/type](http://github.com/jkroso/type). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/jkroso-type`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# type

  Type assertions aka less-broken `typeof`.

## API

```js
var type = require('type')
type(new Date) // => 'date'
type({}) // => 'object'
type(null) // => 'null'
type(undefined) // => 'undefined'
type("hey") // => 'string'
type(true) // => 'boolean'
type(false) // => 'boolean'
type(12) // => 'number'
type(type) // => 'function'
type(/asdf/) // => 'regexp'
type((function(){ return arguments })()) // => 'arguments'
type([]) // => 'array'
type(new Uint8Array) // => 'bit-array'
type(document.createElement('div')) // => 'element'
```
