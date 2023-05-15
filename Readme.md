# Rest and Spread Exercises

###



```
function filterOutOdds() {
  var nums = Array.prototype.slice.call(arguments);
  return nums.filter(function(num) {
    return num % 2 === 0
  });
}

```


### refactor

```

const filterOutOdd = (...numbers) => numbers.filter(number => number % 2  === 0);


```

### Write a function called findMin that accepts a variable number of arguments and returns the smallest argument.


```

const findMin = (...min) => Mat.min(...min);


```

### Write a function called mergeObjects that accepts two objects and returns a new object which contains all the keys and values of the first object and second object.


```
const mergeObjects = (firtsObejct, secondObejct) => ( {...firtsObejct, ...secondObejct} );
```

### Write a function called doubleAndReturnArgs which accepts an array and a variable number of arguments. The function should return a new array with the original array values and all of additional arguments doubled.

```
const doubleAndReturnArgs = (numbers, ...doubles) => [...numbers, ...doubles.map(double => double *2)];
```

### Slice and Dice

```
const removeRandom = items => {
  const idx = Math.floor(Math.random() * items.length);
  const newItems = [...items];    
  newItems.splice(idx, 1);

  return newItems
}
```

```
const extend = (array1, array2) => [...array1, ...array2];
```

```
const addKeyVal = (obj, key, val) => ( {...obj, [key]: val } );
```

```
const combine = (obj1, obj2) => ( ...obj1, ...obj2 );
```

```
const removeKey = (obj, key) => {
 ({ [key]: undefined, ...obj } = obj);
  return obj;
}

```