# 

# *Arrays*



## Arrays are just regular objects

1. the items in the array are nothing more than properties of that objects

2. An array has, alongside its elements, a special property named `length` and a generous **collection of methods for manipulating** the elements. They represent the real power of arrays. You can search, sort, delete, insert, etc.
   
   # 

## Declaring an Array

```javascript
var arr = [1, 2, 3, 4, 5]
```

    or

```javascript
var arr = new Array(1, 2, 3, 4, 5)
```

Remember:

- use array literals instead of the Array constructor

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

The `length` property can also be set externally. We can truncate an array by setting `length`

```javascript
var arr = [1, 2, 3, 4];
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
