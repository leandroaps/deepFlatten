# deepFlatten
This snippet flattens an array recursively.

```
const deepFlatten = arr => [].concat(...arr.map(v => (Array.isArray(v) ? deepFlatten(v) : v)));
```

**Usage:**
```
deepFlatten([1, [2], [[3], 4], 5]); // [1,2,3,4,5]
```
