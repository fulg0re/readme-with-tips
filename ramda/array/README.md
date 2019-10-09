[Tips](../../README.md) > [Ramda](../README.md) > Array

# Work with array by ramda

- Remove object from array by object key:
```
const R = require('ramda');

const arr = [
  { key: 'someKey_1' },
  { key: 'someKey_2' },
  { key: 'someKey_3' },
];

const result = R.reject(
    R.propEq('key', 'someKey_2'),
    arr,
);

console.log(result);
// result = [ { key: 'someKey_1' }, { key: 'someKey_3' } ];
```
