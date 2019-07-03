# Javascript Tips & Tricks
JS tips and tricks I found along the way. &lt;3

### Filter array for falsy values
Using the Boolean constructor
```
['foo', 'bar', undefined, null, 42, '', false, true].filter(Boolean);
// returns ['foo', 'bar', 42, true];
```

### Get first array value using ES6 destructuring
```
const arr = ['foo', 'bar', 'boo', 'far'];
const [firstElement,] = arr; // firstElement === 'foo';
const [first, ...next] = arr // next = ['bar', 'boo', 'far'];
```

### Reassign destructured object property
```
const foo = {
  bar: {
    boo: 'far',
  },
};

const { bar: { boo }} = foo; // boo === 'far';
const { bar: { boo : newBoo }} = foo; // newBoo === 'far';
```
