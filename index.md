```javascript
function finallyTest() {
  try {
    console.log('one');
    return 'three';
  } catch (err) {
    console.log('error');
  } finally {
    console.log('two');
  }
}

console.log(finallyTest());
console.log('four');
```
what is the output?
