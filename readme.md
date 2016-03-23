# method-chain

Simple utility function to wrap a value and chain methods against it.

Starts with data and chains function output as input to the next.

Retrieve current value with `.value`

## Installation

```
$ npm install mw-method-chain
```

## Example

```
var chain = require('mw-method-chain')
  , double = function(num) { return num * 2 }

chain(1000)
  (double)
  (double)
  (double)
  .value

// returns 8000
```

## License

MIT
