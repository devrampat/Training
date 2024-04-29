### 1. Swap two integers present in variables num1 and num2 without using temporary variable

Hint 1: simple destructuring assignment using array
Hint 2: Traditional approach of swapping by using the given variables is also achievable


### 2. Write a program to reverse a string

Hint 1: String can be reversed by iterating it and storing it in reverse order
Hint 2: String can also be reversed by converting it to array, then joining it after reversing


### 3. Write a program to reverse a string by words. Also show the reverse of each words in place


### 4. Write a code to replace all the spaces of the string with underscores

Hint 1: `replaceAll` is the inbuilt String function on prototype which can be used to replace a string with another string


### 5. Write a function which accepts a string argument and returns the count of characters between the first and last character 'X'

```js copy
// Example
getTheGapX("XeroX"); // 4
getTheGapX("Xamarin"); // -1       (If there is only single character 'X')
getTheGapX("JavaScript"); // -1       (If there is no character 'X')
getTheGapX("F(X) !== G(X) !== F(X)"); // 18
```

Hint 1:  `indexOf` and `lastIndexOf` are the methods on String which returns the position of the given string in the input string from start and end respectively



### 6. Write a code to truncate a string to a certain number of words

Hint: `slice` method of array can be used to get the number of words.

```js copy
const str = "JavaScript is simple but not easy to master";
const wordLimit = 3;

Exptected output: "JavaScript is simple"
```


### Objects ###

### 7. Display all the keys and values of a nested object

Hint 1: `typeof` operator on value gives the type of value
Hint 2: Recursive solution can be used to iterate over all the nested objects


### 8. Write a program which can empty a given object

Hint 1: Object can be emptied by removing all the keys present on it
HInt 2: Alternatively, a new object can be created and the prototype of the new object can be set as prototype of old object


### 9. Show how a deep copy of an object can be done

Hint:  Deep copy is done by copying all the properties of the object to another object


### 10. Create an object which has a property 'userid' which can only be set once and will be a read only property

Hint: Property accessor `writable`;


### 11. Create an object 'obj' with functions assigned to keys. Show how can we achieve 'obj.func1().func2().func3()' considering func1, func2, func3 are object keys

Hint: For achieving chaining functionality, each function can return the calling context itself so that context is retained


### 12. Write a program which can return a boolean if value is present in the range with given start and end values in an object


### Functions ###

### 13. Design a Calulator interface function for 2 number inputs which can perform sum, difference, product and dividend whenever invoked on the same interface

```js copy
// Example
const calc12And5 = Calculator(12, 5);
calc12And5.sum(); // 17
calc12And5.difference(); // 7
calc12And5.product(); // 60
calc12And5.dividend(); // 2
```

### 14. Design a private counter function which exposes increment and retrive functionalities

### 15. Write a function which helps to achieve multiply(a)(b) and returns product of a and b

```js copy
// Example
multiply(2)(4); // 8
multiply(5)(3); // 15
```


### 16. Design a function which helps to do debouncing

Hint: The `debounce` function forces a function to wait a certain amount of time before running again
- The function is built to limit the number of function calls to improve the performance
- Debounce function design can take function (to be debounced), delay and the optional context


### 17. Design a function which can keep recieving the arguments on each function call and returns the sum when no argument is passed

- The function can be designed to return another function which maintains the closure over the previous sum value
- The check for breaking condition can be added using the argument check for `undefined`
- 3rd solution uses the property on function to store the total which will be updated on each call hence the same function can be returned

```js copy
// Example
sum(2)(4)(6)(1)(); // 13
sum(2)(4)(); // 6
sum(3)(); // 3
```