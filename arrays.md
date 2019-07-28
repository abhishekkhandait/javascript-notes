# *Arrays*

## Arrays are just regular objects

1. the items in the array are nothing more than properties of that objects

2. An array has, alongside its elements, a special property named `length` and a generous **collection of methods for manipulating** the elements. They represent the real power of arrays. You can search, sort, delete, insert, etc.

## Declaring an Array

```javascript
let arr = [1, 2, 3, 4, 5]
```

    or

```javascript
let arr = new Array(1, 2, 3, 4, 5)
```

An array can store elements of any type. For ex:

```javascript
let arr = [1, 2, 'apple', true, { total: 1 }, function(){console.log('hey')}, undefined, null]
```

> always try to use array literals instead of the Array constructor

## Accesing array elements

JavaScript arrays are zero-indexed: the first element of an array is at index `0`, and the last element is at the index equal to the value of the array's `length` property minus 1. Using an invalid index number returns `undefined`.

```javascript
let arr = ['apple', 'mango', 'cherty'];
console.log(arr[0]); // apple
console.log(arr[1]); // mango
console.log(arr[arr.length - 1]); // cherry
console.log(arr[100]); // undefined
```

> trying to access an element of an array as follows throws a syntax error because the property name is not valid: 
> 
> ```javascript
> console.log(arr.0); //syntax error
> ```

## Detecting an Array

The `Array.isArray()` method determines whether the passed value is an [`Array`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array "The JavaScript Array object is a global object that is used in the construction of arrays; which are high-level, list-like objects.").

Syntax:      `Array.isArray(value)`

`Array.isArray` method return a `true` if the value is an `Array` ; othewise `false`

```javascript
Array.isArray([1, 2, 3]);  // true
Array.isArray({foo: 123}); // false
Array.isArray('foobar');   // false
Array.isArray(undefined);  // false
```

## The `length` Property

- An `Array` has a special property `length` which simply returns the length of an `Array`

- Whenever you add a new element, the value of length will be updated

>  The `length` property can also be set externally. We can truncate an array by setting `length`

```javascript
let arr = [1, 2, 3, 4];
console.log(arr.length); // 4
arr[20] = 2; 
console.log(arr.length); // 21 - even though there are no elements between index 5 and 19
```

> Remember
> 
> - its a bad practice to add elements to array at random indexs
> 
> - Dont change the property of an array like a regular object.
> 
> - Always use the array methods to modify an array

## Array Methods

- #### `push()` :   `push`  appends one or more element to the end of an array.
  
  ```javascript
  let days = ['Monday'];
  days.push('Tuesday');
  days.push('Wednesday', 'Thursday', 'Friday');
  console.log(days); // ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"]
  ```

- #### `pop()` :  `pop`  takes an element from the end of an array
  
  ```javascript
  let days = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"];
  days.pop();
  console.log(days); // ["Monday", "Tuesday", "Wednesday", "Thursday"]
  ```

- #### `shift()` : Extracts the first element of the array and returns it
  
  ```javascript
  let days = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"];
  let removedDay = days.shift(); // removes Monday and assigns it to removedDay;
  console.log(days); // ["Tuesday", "Wednesday", "Thursday", "Friday"]
  ```

- #### `unshift()` : Add the element to the beginning of the array
  
  ```javascript
  let days = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"];
  days.unshift("Sunday");
  console.log(days); // ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday"];
  ```
  
  > - Methods `push/pop` run fast, while `shift/unshift` are slow.
  > 
  > - Methods `push` and `unshift` can add multiple elements at once:
  >   
  >   ```javascript
  >   var days = ["Tuesday"];
  >   days.push("Wednesday", "Thursday");
  >   days.unshift("Sunday", "Monday");
  >   console.log(days); // ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday"]
  >   ```



##### 


