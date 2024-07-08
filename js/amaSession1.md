# Ama Session 1 - Javascript Basics

## Questions

**1. Difference Between == and === Operator?**

- "==" : Checks equality after converting both the values to a common type.
- "===" : Checks equality without type conversion

**2. Console.log(typeof []) is equals to 'object' why?**

- Array is a special type of object.

**3. Whats are the disadvantages of using closure**

- Memory leaks and debugging issues

**4. Why using global variables are bad in js ?**

- Name conflicts
- Difficult to debug

**5. How to extract certain properties from an array of objects to create a new array ?**

- Using map() method

**6. Difference between charAt() and at() method in js ?**

- At() allows negative indexing
- charAt() does not allow negative indexing

**7. How to reset initial or 1st commit in git, if it's possible ?**
  ```bash
git update-ref -d HEAD
 ``` 
**9. If console.log(typeof []) returns 'object', then why can not we use (.) operator in array to access its values just like objects,where we use (.) operator in objects for accessing key and values**

- Array uses different way of indexing.
 
**10. Why 'forEach' loop skips 'not defined' whereas 'for' loop gives 'undefined' ?**
- forEach operates only on defined values.

**11. How can we mimic the action Array.splice and 'Array.slice' on objects**
- Traverse through the object using for..in loop and delete or insert properties.

**12. What is "Callback Hell" problem and how to avoid it ?**

- Callback Hell occurs where callbacks are nested within other callbacks.
- It can be solved using promises.

**13. Why "Hello" is also printing ? when we have exported array('ar') only!**  

   ```javascript
    //file1.js
   
    let ar = [1,2,3];
    console.log("Hello");
    module.exports.ar = ar;
    
    //file2.js

  
    const {ar} = require('file1.js');
    let print = ar;
    console.log(print);
    
    Output: 
    "Hello" 
    [1,2,3]
  ```

  - When we import the module using require, it executes the whole file.

