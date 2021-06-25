###### 1. What's the output?
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
<details><summary><b>why I ask</b></summary>
<p>
 
  The last execute code wins, the last one overrides previous one.
  Checkout [this article](https://jakearchibald.com/2021/last-return-wins/).
  
  And finally statement makes it posibble to return many times from a single function call.

</p>
</details>
