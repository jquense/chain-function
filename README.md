# chain-function
chain a bunch of functions

```sh
npm i chain-function
```

```js
 function foo() {
   console.log('foo')
 }
 
 function baz() {
   console.log('bar')
 }
 
 var barfoo = chain(bar, foo)
 
 barfoo() // "bar" "foo"
 
 //handles falsely values just fine
 barfoo = chain(bar, null, foo, undefined, false)
 
 barfoo() // "bar" "foo"
```
