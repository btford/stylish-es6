# stylish es6

This is me thinking out loud on writing good lookin' ES6.

## Anonymous functions that return an object

```javascript
// note that you need extra parens around the
// implicitly returned object
(bar) => ({ foo: bar })

// es5
function (bar) {
  return {
    foo: bar
  }
}
```

## Reduce + anonymous function + comma operator

[teach the controversy](https://twitter.com/briantford/status/479353642676662272)

```javascript
// again note the parens around the function body
[1,2,3].reduce((obj, prop) => (obj[prop] = prop, obj), {})
// -> { 1: 1, 2: 2, 3: 3 }

// es5
// way less cute imho
[1, 2, 3].reduce(function (obj, prop) {
  obj[prop] = prop;
  return obj;
}, {});
```


## license
MIT
