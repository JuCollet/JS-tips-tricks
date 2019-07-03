# Javascript Tips & Tricks
JS tips and tricks I found along the way. &lt;3

### Filter array for falsy values
Using the Boolean constructor
```
['foo', 'bar', undefined, null, 42, '', false, true].filter(Boolean) // returns ['foo', 'bar', 42, true]
```
