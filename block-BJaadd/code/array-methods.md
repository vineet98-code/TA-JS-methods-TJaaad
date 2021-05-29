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

   - Parameter: n (any) number of values (number, string)
   - Return: A string with all array elements joined. If arr.length is 0, the empty string is returned.
   - Example:
     ```js
     var a  = ['Wind', 'Water', 'Fire'];
     a.join(); // "Wind,Water,Fire"

     a.join('-'); // "Wind-Water-Fire"

     a.join('+'); // "Wind+Water+Fire"
     ```
   - `join` accepts n number of values and a new string by concatenating all of the elements in an array
   - it does mutate the original array

3. `flat`

   - Parameter: n (any) number of values (number)
   - Return: A new array with the sub-array elements concatenated into it..
   - Example:
     ```js
     
     const arr1 = [0, 1, 2, [3, 4]];
     arr1.flat(); // [0, 1, 2, 3, 4];

     const arr4 = [1, 2, [3, 4, [5, 6, [7, 8, [9, 10]]]]];
     arr4.flat(Infinity); //  [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

     const arr5 = [1,2, , 4, 5];
     arr5.flat(); // [1, 2, 4, 5];

     ```
   - `flat` accepts n number of values and creates a new array with all sub-array elements concatenated into it recursively up to the specified depth..
   - It does mutate the original array

   
4. `push`
 
   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: The new length property of the object upon which the method was called..
   - Example:
     ```js
     const animals = ['pigs', 'goats', 'sheep'];

     animals.push('cows'); // ["pigs", "goats", "sheep", "cows"];

     let sports = ['soccer', 'baseball'];

     sports.push('football', 'swimming'); // ['soccer', 'baseball', 'football', 'swimming']

     animals.push('chickens', 'cats', 'dogs'); // ["pigs", "goats", "sheep", "cows", "chickens", "cats", "dogs"]

     ```
   - `push` method adds one or more elements to the end of an array and returns the new length of the array.
   - It mutate the original array

5. `indexOf`
  
   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.indexOf(3); // 2
     
     let colors = ['red', 'green', 'blue', 'white', 'black', 'pink'];
     colors.indexOf(7); // -1

     const beasts = ['ant', 'bison', 'camel', 'duck', 'bison'];
     beasts.indexOf('bison', 2);

     ```
   - `indexOf` method returns the first index at which a given element can be found in the array, or -1 if it is not present.
   - No it does not mutate the original array

6. `lastIndexOf`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: The last index of the element in the array; -1 if not found..
   - Example:
     ```js

     const animals = ['Dodo', 'Tiger', 'Penguin', 'Dodo'];
     animals.lastIndexOf('Penguin'); // 2

     var numbers = [2, 5, 9, 2];

     numbers.lastIndexOf(2); // 3

    
     let colors = ['red', 'green', 'blue', 'black', 'red'];
     colors.lastIndexOf('black'); // 
     ```
   - `lastIndexOf` accepts n number of values and returns the last index at which a given element can be found in the array, or -1 if it is not present. The array is searched backwards, starting at fromIndex
   - No it does not mutate the original array

7. `includes`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: if the value searchElement is found within the array.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.includes(4); // false
     
     const pets = ['cat', 'dog', 'bat'];
     pets.includes('cat')); // true
     let colors = ['red', 'green', 'blue'];
     colors.includes('red'); //  true
     ```
   - `includes` accepts n number of values and method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
   - No it does not mutate the original array

8. `reverse`
  
   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: The reversed array..
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.reverse(); //[3, 2, 1]

     const array1 = ['one', 'two', 'three'];
     array1.reverse(); // ["three", "two", "one"]
     
     let colors = ['red', 'green', 'blue'];
     colors.reverse(); // ["blue", "green", "red"]
     ```
   - `reverse` accepts n number of values and method reverses an array in place. The first array element becomes the last, and the last array element becomes the first.
   - It mutate the original array

9. `every`
  
   - Parameter: n (any) number of values (number, string,  array, object and function etc)
   - Return: true if the callbackFn function returns a truthy value for every array element. Otherwise, false..
   - Example:
     ```js
     
     function isBigEnough(element, index, array){
       return element >= 10;
     }
     [12, 5, 8, 130, 44].every(isBigEnough); // false

     [12, 5, 8, 130, 44].every(x => x >= 10); // false

     ['red', 'green', 'blue'].every(x => x = 'blue'); // true
     
     ```
   - `every` accepts n number of values and tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.
   - No it does not mutate the original array

10. `shift`

    - Parameter: n (any) number of values (number, string, array, object etc)
   - Return: The removed element from the array; undefined if the array is empty..
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.shift(); // 1

     var myFish = ['angel', 'clown', 'mandarin', 'surgeon'];

     var shifted = myFish.shift(); // 'angel'

     let colors = ['red', 'green', 'blue'];
     colors.shift('black', 'red', 21, true); // 'red';
     ```
   - `shift` accepts n number of values and removes the first element from an array and returns that removed element. This method changes the length of the array.
   - It mutate the original array

11. `splice`

    - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: A new array containing the extracted elements.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.splice(4); //[1,2,3,4]
     
     let fruits = ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango'];
     let citrus = fruits.slice(1,2); // "Orange"]

     let colors = ['red', 'green', 'blue'];
     colors.splice(); // 
     ```
   - `splice`returns a shallow copy of a portion of an array into a new array object selected from start to end (end not included) where start and end represent the index of items in that array. 
   - No it does not mutate the original array

12. `find`

    - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: The value of the first element in the array that satisfies the provided testing function. Otherwise, undefined is returned.
   - Example:
     ```js
     let numbers = [1, 2, 3, 140, 44];
     numbers.find(elements => elements > 10); // 140

     let colors = ['red', 'green', 'blue'];
     colors.find(color => color === 'green'); // 'green'

     colors.find(color => color === ' ');  // undefined
     ```
   - `find` accepts n number of values and returns one array with all the values in same order. It does not change the original array.returns the value of the first element in the provided array that satisfies the provided testing function

   - No it does not mutate the original array

13. `unshift`
   
   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: The new length property of the object upon which the method was called..
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.unshift(4); // [4, 1, 2, 3]
    
     let colors = ['red', 'green', 'blue'];
     colors.unshift('black'); // ["black", "red", "green", "blue"]
     ```
   - `unshift` accepts n number of values and method adds one or more elements to the beginning of an array and returns the new length of the array. The unshift method inserts the given values to the beginning of an array-like object.

   - It mutate the original array

14. `findIndex`
 
    - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];

     const index = numbers.findIndex(num => num === 3); // 2

     const fruits = ["apple", "banana", "cantaloupe", "blueberries", "grapefruit"];

     const index = fruits.findIndex(fruit => fruit === 'mango'); // -1
     
     let colors = ['red', 'green', 'blue'];
     colors.findIndex(color => color === 'red'); // 0
     ```
   - `findIndex` accepts n number of values and eturns the index of the first element in the array that satisfies the provided testing function. Otherwise, it returns -1, indicating that no element passed the test.
   - No it does not mutate the original array

15. `filter`
  
   - Parameter: n (any) number of values (number, string,  array, object and function etc)

   - Return: A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.

   - Example:
     ```js
     let numbers = [1,4,5,6,7,8,9,12,14,156,265];

     function isEven(num){
       return num % 2 === 0;
     }
     let evenNumber = numbers.filter(isEven);

     
     const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
     const result = words.filter(word => word.length > 6); // ["exuberant", "destruction", "present"]

     let colors = ['red', 'green', 'blue'];

     const result = colors.filter(color => color.length > 3);

     
     ```
   - `filter` accepts n number of values and method creates a new array with all elements that pass the test implemented by the provided function.

   - It mutate the original array

16. `flat`

    - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: A new array with the sub-array elements concatenated into it..
   - Example:
     ```js
     let numbers = [0, 1, 2, [3, 4]];
     numbers.flat(); //[0, 1, 2, 3, 4]

     const arr2 = [0, 1, 2, [[[3, 4]]]];
     arr2.flat(); //  [0, 1, 2, Array(1)]
     
     let colors = ['red', 'green', 'black','blue'];
     colors.flat(); //   ["red", "green", "black", "blue"]
     ```
   - `flat` accepts n number of values and method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.
  
   - It mutate the original array.

17. `forEach`
  
    - Parameter: n (any) number of values (number, index, , array, null, undefined, object and function etc)
   - Return: undefined.
   - Example:
     ```js

     const array1 = ['a', 'b', 'c'];

     array1.forEach(element => console.log(element)); // ["a", "b", "c"]

     let numbers = [1, 2, 3];
     numbers.forEach(num => num); // [1, 2, 3]
     
     let colors = ['red', 'green', 'blue'];
     colors.forEach(color => color ); // ["red", "green", "blue"]
     ```
   - `forEach` accepts n number of values and method executes a provided function once for each array element. forEach() calls a provided callbackFn function once for each element in an array in ascending index order. It is not invoked for index properties that have been deleted or are uninitialized.
   - No it does not mutate the original array

18. `map`

    - Parameter: n (any) number of values (number, string, element, thisArg, array, object and function etc)
   - Return: A new array with each element being the result of the callback function..
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.map(x => x * 2); // [2, 4, 6]

     numbers.map(x => x / 2); // [0.5, 1, 1.5]

     numbers.map(x => x + 2); // [3, 4, 5]
     ```
   - `map` accepts n number of values and method creates a new array populated with the results of calling a provided function on every element in the calling array.
   - It mutate the original array

19. `pop`

    - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: The removed element from the array; undefined if the array is empty..
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.pop(); // 2
     
     let fruits = [];
     fruits.pop(); //  undefined
     let colors = ['red', 'green', 'blue'];
     colors.pop();  // 'blue'
     ```
   - `pop` accepts n number of values and method removes the last element from an array and returns that element. This method changes the length of the array. The pop method removes the last element from an array and returns that value to the caller.
   - It mutate the original array

20. `reduce`

    - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: The single value that results from the reduction..
   - Example:
     ```js

     let numbers = [1, 2, 3];
     
     let number = [undefined];

     const reducer = (accumulator, currentValue) => accumulator + currentValue;
     numbers.reduce(reducer); // 6
     
     number.reduce(reducer) // undefined 

     let colors = ['red', 'green', 'blue'];
     colors.reduce(reducer); // "redgreenblue"
     ```
   - `reduce` accepts n number of values and method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.
   - No it does not mutate the original array

21. `slice`

    - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: A new array containing the extracted elements..
   - Example:
     ```js

     const flowers = ['rose', 'lilly', 'sunflower', 'tulip', 'lotus'];
     
     flowers.slice(2,4); // ["sunflower", "tulip"]

     let colors = ['red', 'green', 'blue'];
     colors.slice(); // ["red", "green", "blue"]
     ```
   - `slice` accepts n number of values and returns a shallow copy of a portion of an array into a new array object selected from start to end (end not included) where start and end represent the index of items in that array. 
   - No it does not mutate the original array

22. `some`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: true if the callback function returns a truthy value for at least one element in the array. Otherwise, false..
   - Example:
     ```js
     let numbers = [1, 2, 3];
     const even = (element) => element % 2 === 0;
     numbers.some(even);  // true


     const odd = (element) => element % 2 !== 0;
     numbers.some(odd); //  true
 
     [2, 5, 8, 1, 4].some(x => x > 10); // false
     
     ```
   - `some` accepts n number of values and method tests whether at least one element in the array passes the test implemented by the provided function. It returns true if, in the array, it finds an element for which the provided function returns true; otherwise it returns false.

   - No it does not mutate the original array
