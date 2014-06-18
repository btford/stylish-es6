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

## license
MIT
