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

    - Parameter: 
    - Return: returns value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase(); //
      ```

3. `toLowerCase`
   
    - Parameter: 
    - Return: returns the value of the string converted to lower case.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toLowerCase(); // 
      let name = 'VINEET';
      name.toLowerCase(); //
      let carName = 'COROLLA';
      carName.toLowerCase(); //
      ```
    
4. `trim`

    - Parameter: 
    - Return: A new string representing str stripped of whitespace from both its beginning and end.
    - Example: 
      ```js
      const sentence = '   Welcome to ALtcampus.  ';
      sentence.trim(); // 
      let greeting  = '  hello world! ';
      name.trim(); //
      let carName = '   altis  ';
      carName.trim(); //
      ```
5. `trimEnd`

    - Parameter: 
    - Return: whitespace from its end (right side).
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.   ';
      sentence.trimEnd(); // 
      let name = 'Vineet  ';
      name.trimEnd(); //
      let carName = 'altis  ';
      carName.trimEnd(); //
      ```
6. `trimStart`
   
    - Parameter: 
    - Return: whitespace from its end (left side)..
    - Example: 
      ```js
      const sentence = '   Welcome to ALtcampus.';
      sentence.trimStart(); // 
      let name = '  Vineet';
      name.trimStart(); //
      let carName = '  altis';
      carName.trimStart(); // 
      ```
7. `concat`

    - Parameter: One or more strings to concatenate.
    - Return: New string containing the combined text of the strings provided..
    - Example: 
      ```js
      let  sentence = 'Welcome to ALtcampus.';
      let  word = 'System';
      sentence.concat('', word); // 

      let firstName = 'Vineet';
      let lastName = 'kumar';
      firstName.concat('', lastName); //

      let carCompany = 'corolla';
      let carList = ['corolla', ' ', 'Altis'];
      carCompany.concat('...carList');
      
      ```

8. `endsWith`

    - Parameter: searchSring: - character to be searched for at the end of str
                 length: - it is used as the length of str
    - Return: true if the given characters are found at the end of the string; otherwise, false.
    - Example: 
      ```js
      let str = 'To be, or not to be, that is the question.'
      str.endsWith('question'); // 

      let name = 'Vineet is the best';
      name.endsWith('bad'); //

      let carName = 'Altis, the superfical is car';
      carName.endsWith('car');

      ```

9. `includes`

    - Parameter: searchSring: - A string to be searched for within str.
                 position - The position within the string at which to begin searching for searchString
    - Return: true if the search string is found anywhere within the given string; otherwise, false if not.
    - Example: 
      ```js
      const sent = 'Welcome to ALtcampus.';
      sent.includes('ALtcampus'); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
10. `indexOf`

    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
11. `lastIndexOf`

    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
12. `padEnd`

    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
13. `padStart`
    
    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
14. `repeat`

    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
15. `replace`

    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
16. `slice`
    
    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
    
17. `split`

    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
18. `substring`

    - Parameter: 
    - Return: value of the String converted into uppercase.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toUpperCase(); // 
      let name = 'Vineet';
      name.toUpperCase(); //
      let carName = 'altis';
      carName.toUpperCase();
      ```
