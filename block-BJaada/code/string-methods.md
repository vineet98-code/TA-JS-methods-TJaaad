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
      sentence.toUpperCase(); // "WELCOME TO ALTCAMPUS."
      let name = 'Vineet';
      name.toUpperCase(); // "VINEET"
      let carName = 'altis';
      carName.toUpperCase(); // "ALTIS"
      ```

3. `toLowerCase`
   
    - Parameter: 
    - Return: returns the value of the string converted to lower case.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.toLowerCase(); // "welcome to altcampus."
      let name = 'VINEET';
      name.toLowerCase(); // "vineet"
      let carName = 'COROLLA';
      carName.toLowerCase(); // "corolla"
      ```
    
4. `trim`

    - Parameter: 
    - Return: A new string representing str stripped of whitespace from both its beginning and end.
    - Example: 
      ```js
      const sentence = '   Welcome to ALtcampus.  ';
      sentence.trim(); // "Welcome to ALtcampus."
      let greeting  = '  hello world! ';
      greeting.trim(); // "hello world!"
      let carName = '   altis  ';
      carName.trim(); //  "altis"
      ```
5. `trimEnd`

    - Parameter: 
    - Return: whitespace from its end (right side).
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.   ';
      sentence.trimEnd(); //  "Welcome to ALtcampus."
      let name = 'Vineet  ';
      name.trimEnd(); //   "Vineet"
      let carName = 'altis  ';
      carName.trimEnd(); // "altis"
      ```
6. `trimStart`
   
    - Parameter: 
    - Return: whitespace from its end (left side)..
    - Example: 
      ```js
      const sentence = '   Welcome to ALtcampus.';
      sentence.trimStart(); // "Welcome to ALtcampus."
      let name = '  Vineet';
      name.trimStart(); //   "Vineet"
      let carName = '  altis';
      carName.trimStart(); // "altis"
      ```
7. `concat`

    - Parameter: One or more strings to concatenate.
    - Return: New string containing the combined text of the strings provided..
    - Example: 
      ```js
      let  sentence = 'Welcome to ALtcampus.';
      let  word = 'System';
      sentence.concat('', word); // "Welcome to ALtcampus.System"

      let firstName = 'Vineet';
      let lastName = 'kumar';
      firstName.concat(' ', lastName); // "Vineet kumar"

      let carCompany = 'corolla';
      let carList = ['corolla', ' ', 'Altis'];
      carCompany.concat('...carList');  // "corolla...carList"
      
      ```

8. `endsWith`

    - Parameter: searchSring: - character to be searched for at the end of str
                 length: - it is used as the length of str
    - Return: true if the given characters are found at the end of the string; otherwise, false.
    - Example: 
      ```js
      let str = 'To be, or not to be, that is the question.'
      str.endsWith('question'); // false

      let name = 'Vineet is the best';
      name.endsWith('bad'); // false

      let carName = 'Altis, the superfical is car';
      carName.endsWith('car'); // true

      ```

9. `includes`

    - Parameter: searchSring: - A string to be searched for within str.
                 position - The position within the string at which to begin searching for searchString
    - Return: true if the search string is found anywhere within the given string; otherwise, false if not.

    - Example: 
      ```js
      const sent = 'Welcome to ALtcampus.';
      sent.includes('ALtcampus'); // true

      let name = 'Vineet';
      name.includes('or not to be, that is the question.'); // false

      let carName = 'altis is a nice car';
      carName.includes('is'); // true
      ```
10. `indexOf`

    - Parameter:  If no string is explicitly provided, searchValue will be undefined
    - Return: The index of the first occurrence of searchValue, or -1 if not found. An integer     representing the index at which to start the search. Defaults to 0
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.indexOf('c'); // 3
      let name = 'Vineet';
      name.indexOf(); //-1

      let carName = 'altis';
      carName.indexOf(''); // 0
      ```
11. `lastIndexOf`

    - Parameter: A string representing the value to search for. If searchValue is an empty string, then fromIndex is returned.
    - Return: The index of the last occurrence of searchValue; -1 if not found.
    - Example: 
      ```js
      let para = 'The index of the last occurrence of searchValue; -1 if not found.';
      const searchTerm = 'not';
      para.lastIndexOf(searchTerm); // 55

      let name = 'Vineet';
      name.lastIndexOf(); // -1

      let carName = 'altis';
      carName.lastIndexOf(); // -1
      ```
12. `padEnd`

    - Parameter: targetLength - The length of the resulting string once the current str has been padded. If the value is lower than str.length, the current string will be returned as-is.

                padString - The string to pad the current str with. If padString is too long to stay within targetLength, it will be truncated: for left-to-right languages the left-most part and for right-to-left languages the right-most will be applied.

    - Return: A String of the specified targetLength with the padString applied at the end of the current str.
    - Example: 
      ```js

      const str1 = 'Breaded Mushrooms';
      str1.padEnd(25, '.'); // "Breaded Mushrooms........"
      
      'abc'.padEnd(6, "123456"); // "abc123"
      'abc'.padEnd(1);           // "abc"

      let name = 'Vineet';
      name.padEnd(7, "kumar"); // "Vineetk"
      
      ```
13. `padStart`
    
    - Parameter: targetLength - The length of the resulting string once the current str has been padded. If the value is less than str.length, then str is returned as-is.
                 padString -  The string to pad the current str with. If padString is too long to stay within the targetLength, it will be truncated from the end.

    - Return: A String of the specified targetLength with padString applied from the start
    - Example: 
      ```js
      const str1 = 'Breaded Mushrooms';
      str1.padStart(25, '.');  // "........Breaded Mushrooms"
      
      'abc'.padStart(6, "123456"); // "123abc"
      'abc'.padStart(1);           //  "abc"

      let name = 'Vineet';
      name.padStart(7, "kumar"); // "kVineet"
      ```
14. `repeat`

    - Parameter:  count - An integer between 0 and +Infinity, indicating the number of times to repeat the string.
    - Return: A new string containing the specified number of copies of the given string.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.repeat(3); //  "Welcome to ALtcampus.Welcome to ALtcampus.Welcome to ALtcampus."
      
      let name = 'Vineet';
      name.repeat(5); // "VineetVineetVineetVineetVineet"
      let carName = 'altis';
      carName.repeat(2); // "altisaltis"
      ```
15. `replace`

    - Parameter: regexp - A RegExp object or literal. The match or matches are replaced with newSubstr or the value returned by the specified replacerFunction.
                 substr - A String that is to be replaced by newSubstr.
                 newSubstr - The String that replaces the substring specified by the specified regexp or substr parameter.
                 replacerFunction - A function to be invoked to create the new substring to be used to replace the matches to the given regexp or substr

    - Return: A new string, with some or all matches of a pattern replaced by a replacement.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.replace('Welcome', 'Hello'); // "Hello to ALtcampus."
      let name = 'Vineet';
      name.replace('Vineet', 'Hello'); // "Hello"
      let carName = 'altis';
      carName.replace('altis', 'Hello'); // "Hello"
      ```
16. `slice`
    
    - Parameter:  beginIndex - The zero-based index at which to begin extraction. If negative, it is treated as str.length + beginIndex.
      
      endIndex - The zero-based index before which to end extraction. The character at this index will not be included.

    - Return: A new string containing the extracted section of the string.
    - Example: 
      ```js
      const sentence = 'The quick brown fox jumps over the lazy dog.';;
      sentence.slice(6, 9); // "ick"
      
      sentence.slice(-10, -8); // " l"
      
      sentence.slice( 30); //  " the lazy dog."
      ```
    
17. `split`

    - Parameter: separator - The pattern describing where each split should occur.  The separator can be a simple string or it can be a regular expression.
        If separator contains multiple characters, that entire character sequence must be found in order to split.
          
    - Return: An Array of strings, split at each point where the separator occurs in the given string.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus brown fox jumps over the lazy dog.';
      sentence.split(' ', 7); //  ["Welcome", "to", "ALtcampus", "brown", "fox", "jumps", "over"]

      
      sentence.split(' '); // ["Welcome", "to", "ALtcampus", "brown", "fox", "jumps", "over", "the", "lazy", "dog."]
      
      sentence.split('-'); // ["W", "e", "l", "c", "o", "m", "e", " ", "t", "o", " ", "A", "L", "t", "c", "a", "m", "p", "u", "s", " ", "b", "r", "o", "w", "n", " ", "f", "o", "x", " ", "j", "u", "m", "p", "s", " ", "o", "v", "e", "r", " ", "t", "h", "e", " ", "l", "a", "z", "y", " ", "d", "o", "g", "."]
      ```
18. `substring`

    - Parameter:  indexStart - The index of the first character to include in the returned substring.
                  indexEnd - The index of the first character to exclude from the returned substring.

    - Return: A new string containing the specified part of the given string.
    - Example: 
      ```js
      const sentence = 'Welcome to ALtcampus.';
      sentence.substring(1,7); //   "elcome"
      let name = 'Vineet';
      name.substring(0,0); // ""
      let carName = 'altis';
      carName.substring(0); // "altis"
      ``` 
