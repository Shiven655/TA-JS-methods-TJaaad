Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

#### Getting To Know String Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (4-5 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your own words and one sentence explain what this method does.

Example:

1. `charAt`

   - Parameter: (index) defaults to 0 - (number data type)
   - Return: character at specific index in the string (string data type)
   - Example:
     ```js
     let name = 'Arya Stark';
     name.charAt(2); //"y"
     let sentance = 'A quick brown fox jumped over a lazy dog';
     sentance(4); // "i"
     let houseName = 'Starks';
     houseName.charAt(0); // "S"
     ```
   - `charAt` accepts a index (number data type) and return the character on that index in the string.

2. `toUpperCase`

  - Parameter: toUpperCase
  - Return:  converted string in uppercase (string data type) 
  -Example:
  ```js
  let name =`Arya Stark`
  name.toUpperCase(); // "ARYA STARK"
  let sentance = 'A quick brown fox jumped over a lazy dog'; 
  sentance.toUpperCase();// "A QUICK BROWN FOX JUMPED OVER A LAZY DOG"
  let houseName = 'Starks'
  housName.toUpperCase(); // "STARKS"
  ```
  `toUpperCase` this method convert the return value to uppercase.

3. `toLowerCase`
- Parameter:toLowerCase
  - Return: converted string in lowercase (string data type)
  -Example:
  ```js
  let name =`Arya Stark`
  name.toLowerCase(); // "arya stark"
  let sentance = 'A quick brown fox jumped over a lazy dog'; 
  sentance.toLowerCase();// "a quick brown fox jumped over a lazy dog"
  let houseName = 'Starks'
  housName.tolowerCase(); // "starks"

  ```
4. `trim`
- Parameter:trim
  - Return:converted string stripped out of space from start and end.
  -Example:
  ```js
  let name = "  Arya Stark  "
  name.trim(); // "Arya Stark"
  let sentance = '  A quick brown fox jumped over a lazy dog  ';   
  sentance.trim(); //'A quick brown fox jumped over a lazy dog'
  let houseName = '  Starks  '
  houseName.trim(); //"Starks"
  ```
5. `trimEnd`
- Parameter:trimEnd
  - Return: converted string stripped out of whitespace from the end.
  -Example:
  ```js
  let name = "Arya Stark  "
  name.trimEnd(); // "Arya Stark"
  let sentance = 'A quick brown fox jumped over a lazy dog  ';   
  sentance.trimEnd(); //'A quick brown fox jumped over a lazy dog'
  let houseName = 'Starks  '
  houseName.trimEnd(); //"Starks"
  ```
6. `trimStart`
- Parameter:trimStart
  - Return:converted string stripped out of whitespace from the start.
  -Example:
  ```js
  let name = "  Arya Stark"
  name.trimStart(); // "Arya Stark"
  let sentance = '  A quick brown fox jumped over a lazy dog';   
  sentance.trimStart(); //'A quick brown fox jumped over a lazy dog'
  let houseName = '  Starks'
  houseName.trimStart(); //"Starks"
  ```
7. `concat`
- Parameter:strN
  - Return:new string containing or combining of string provided.
  -Example:
  ```js
let str1 = "Hello"
let str2 = "World!"
str1.concat(' ', str2);
  ```

8. `endsWith`
- Parameter:searchString , length optional
  - Return:true if searched value is found else false
  -Example:
  ```js
  let name = "Arya Stark"
  name.endsWith('Stark'); // True
  let name = "  Arya Stark"
  name.endsWith('Arya'); // False
  ```
9. `includes`
- Parameter:searchString, position optional
  - Return:true if the searchString is found else false.
  -Example:
  ```js
let sentance = 'A quick brown fox jumped over a lazy dog';
sentance.includes('fox') // true
  ```
10. `indexOf`
- Parameter:searchValue, fromIndex-optional
  - Return:return index of the first occurance else return -1.
  -Example:
  ```js
let sentance = 'A quick brown fox jumped over a lazy dog';
sentance.indexOf('fox'); // The index of the fox from the beginning is 12
  ```
11. `lastIndexOf`
- Parameter:searchValue, fromIndex-optional
  - Return:The index of the last search value else -1
  -Example:
  ```js
let sentance = 'A quick brown fox jumped over a lazy dog if the dog barked '; // The index of the first dog from the end is 15.
  ```
12. `padEnd`
- Parameter:targetLength, padString-optional
  - Return:String of specified targetLength with the padString at the end of the current string
  -Example:
  ```js
 let Name ="Hello"
 Name.padEnd(10, '.')  // "Hello....."
  ```
13. `padStart`
- Parameter:targetLength, padString- optional
  - Return:String of specified target with the padString at the start of the current String
  -Example:
  ```js
let value = 25
value.padStart(5, '00') // 00025
  ```
14. `repeat`
- Parameter:count
  - Return:A new string containing specified no of copies of the string
  -Example:
  ```js
hello.repeat(3) // hellohellohello
  ```
15. `replace`
- Parameter:regexp, substr,newsubstr-replacement, replaceFunction-replacement
  - Return:A new string with some or all match or a pattern replaced by replacement.
  -Example:
  ```js
let sentance = 'A quick brown fox jumped over a lazy dog'; 
sentance.replace('dog', monkey); // 'A quick brown fox jumped over a lazy monkey'; 
  ```
16. `slice`
- Parameter:beginIndex, endIndex- optional
  - Return:a new string containing the extracted string
  -Example:
  ```js
 let sentance = 'A quick brown fox jumped over a lazy dog'; 
 sentance.slice(31); "the lazy dog"
  ```
17. `split`
- Parameter:separator, limit
  - Return: An array of strings, split at which point where the separator occur at point
  -Example:
  ```js
let sentance = 'A quick brown fox jumped over a lazy dog'; 
sentance.split(words[3]); // fox
  ```
18. `substring`
- Parameter:separator, limit
  - Return:An array of strings , split at which point where the separator occur at point
  -Example:
  ```js
```js
let sentance = 'A quick brown fox jumped over a lazy dog'; 
sentance
  ```
