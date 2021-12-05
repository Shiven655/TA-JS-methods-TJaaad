Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

## Getting To Know Array Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (2-3 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your words what this method does.
6. Does it mutate the original value or not (check https://doesitmutate.xyz)

Example:

1. `concat`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');
     sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.concat('black', 'red', 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `concat` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

2. `join`

  -Parameter:separator - optional
  -Return: A string with all array elements joined. If arr.length is 0, the empty string is returned. 
  -Example:
  ```js
  var a = ['Wind', 'Water', 'Fire'];
  a.join();      // 'Wind,Water,Fire'
  ```
3. `flat`
  -Parameter:depth - optional
  -Return:A new array with the sub-array elements concatenated into it.
  -Example:
  ```js
  const arr = [1, 2, [3, 4]];
  arr.flat();  // [1, 2, 3, 4]
  ```
4. `push`
-Parameter:elementN
  -Return:The new length property of the object upon which the method was called. 
  -Example:
  ```js
  let sports = ['soccer', 'baseball']
  let total = sports.push('football', 'swimming')
  ```
5. `indexOf`
  -Parameter:searchElement
  -Return:The first index of the element in the array; -1 if not found.
  -Example:
  ```js
  var array = [2, 9, 9];
  array.indexOf(2);     // 0
  ```
6. `lastIndexOf`
  -Parameter:searchElement
  -Return:The last index of the element in the array; -1 if not found.
  -Example:
  ```js
  var numbers = [2, 5, 9, 2];
  numbers.lastIndexOf(2);     // 3
  ```
7. `includes`
-Parameter:searchElement, fromIndex-optional
  -Return: A boolean value which is true if the value searchElement is found within the array 
  -Example:
  ```js
  [1, 2, 3].includes(2)         // true
  ``` 
8. `reverse`
-Parameter:
  -Return:the reversed array
  -Example:
  ```js
  const a = [1, 2, 3];

  console.log(a); // [1, 2, 3]
  ```
9. `every`
-Parameter:callBackFn, element, index-optional, array-optional, thisArg-optional
  -Return:true if the callbackFn function returns a truthy value for every array element. Otherwise, false
  -Example:
  ```js
  
console.log(isSubset([1, 2, 3, 4, 5, 6, 7], [5, 7, 6])); // true
console.log(isSubset([1, 2, 3, 4, 5, 6, 7], [5, 8, 7])); // false
  ```
10. `shift`
-Parameter:
  -Return:The removed element from the array; undefined if the array is empty.
  -Example:
  ```js
  var shifted = myFish.shift();

console.log('myFish after:', myFish);// myFish after: ['clown', 'mandarin', 'surgeon']

console.log('Removed this element:', shifted);// Removed this element: angel

  ```
11. `splice`
-Parameter:start, deleteCount, item1, item2-optional
  -Return:An array containing the deleted elements,If only one element is removed, an array of one element is returned,If no elements are removed, an empty array is returned.
  -Example:
  ```js
  let myFish = ['angel', 'clown', 'mandarin', 'sturgeon']
  let removed = myFish.splice(2, 0, 'drum')

// myFish is ["angel", "clown", "drum", "mandarin", "sturgeon"]
// removed is [], no elements removed

  ```
12. `find`
-Parameter:callbackfn, element,  index, array-optional, thisArg-optional
  -Return:The value of the first element in the array that satisfies the provided testing function. Otherwise, undefined is returned. 
  -Example:
  ```js
  const inventory = [
  {name: 'apples', quantity: 2},
  {name: 'bananas', quantity: 0},
  {name: 'cherries', quantity: 5}
];

function isCherries(fruit) {
  return fruit.name === 'cherries';
}

console.log(inventory.find(isCherries));
// { name: 'cherries', quantity: 5 }

  ```
13. `unshift`
-Parameter:elementN
  -Return: The new length property of the object upon which the method was called.
  -Example:
  ```js
  let arr = [4, 5, 6]

arr.unshift(1, 2, 3)
console.log(arr);// [1, 2, 3, 4, 5, 6]
  ```
14. `findIndex`
-Parameter:callbackFn, element, array-optional, index-optional
  -Return:The index of the first element in the array that passes the test. Otherwise, -1. 
  -Example:
  ```js
  function isPrime(num) {
  for (let i = 2; num > i; i++) {
    if (num % i == 0) {
      return false;
    }
  }
  return num > 1;
}

console.log([4, 6, 8, 9, 12].findIndex(isPrime)); // -1, not found
console.log([4, 6, 7, 9, 12].findIndex(isPrime)); // 2 (array[2] is 7)

  ```
15. `filter`
-Parameter:callbackFn, element, index-optional, array-optional
  -Return:A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.
  -Example:
  ```js
  function isBigEnough(value) {
  return value >= 10
}

let filtered = [12, 5, 8, 130, 44].filter(isBigEnough)// filtered is [12, 130, 44]

  ```
16. `flat`
  -Parameter:depth - optional
  -Return:A new array with the sub-array elements concatenated into it.
  -Example:
  ```js
  const arr = [1, 2, [3, 4]];
  arr.flat();  // [1, 2, 3, 4]
  ```
17. `forEach`
-Parameter:callbackFn, element, array, index-optional
  -Return:undefined
  -Example:
  ```js
  let ratings = [5, 4, 5];
let sum = 0;

let sumFunction = async function (a, b)
{
  return a + b
}

ratings.forEach(async function(rating) {
  sum = await sumFunction(sum, rating)
})

console.log(sum)
// Naively expected output: 14
// Actual output: 0

  ```
18. `map`
-Parameter:callbackFn, element, array, index-optional
  -Return:A new array with each element being the result of the callback function.
  -Example:
  ```js
  let numbers = [1, 4, 9]
let roots = numbers.map(function(num) {
    return Math.sqrt(num)
})
// roots is now     [1, 2, 3]
// numbers is still [1, 4, 9]

  ```
19. `pop`
-Parameter:
  -Return:The removed element from the array; undefined if the array is empty.
  -Example:
  ```js
  var myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];

var popped = myFish.pop();

console.log(myFish); // ['angel', 'clown', 'mandarin' ]
  ```
20. `reduce`
-Parameter:callbackFn, initialValue
  -Return:The value that results from running the “reducer” callback function to completion over the entire array.
  -Example:
  ```js
  let sum = [0, 1, 2, 3].reduce(function (previousValue, currentValue) {
  return previousValue + currentValue
}, 0)
// sum is 6

  ```
21. `slice`
-Parameter:start, end -optional
  -Return:A new array containing the extracted elements.
  -Example:
  ```js
  let fruits = ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango']
let citrus = fruits.slice(1, 3)

// fruits contains ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango']
// citrus contains ['Orange','Lemon']

  ```
22. `some`
-Parameter:callbackfn, element,  index, array-optional, thisArg-optional
  -Return:true if the callback function returns a truthy value for at least one element in the array. Otherwise, false. 
  -Example:
  ```js
  function isBiggerThan10(element, index, array) {
  return element > 10;
}

[2, 5, 8, 1, 4].some(isBiggerThan10);  // false
[12, 5, 8, 1, 4].some(isBiggerThan10); // true

  ```
