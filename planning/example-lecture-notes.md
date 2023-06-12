# Example Lecture Notes

This is a quick example doc for how Lecture Notes _could_ be used for our course.

## Lecture - Arrays

Arrays are a powerful data structure that allow us to store multiple values in a single variable. They are a core concept in programming and are used in almost every program you will write.

### Creating Arrays

Arrays are created using square brackets `[]` and can be assigned to a variable like any other value.

```js
const myArray = [];
```

Arrays can also be created with values already in them by placing the values inside the square brackets, separated by commas.

```js
const myArray = [1, 2, 3];
```

### Accessing Array Values

Values in an array can be accessed by their index. The index of an array starts at 0, so the first value in an array is at index 0, the second value is at index 1, and so on.

```js
const myArray = [1, 2, 3];
console.log(myArray[0]); // 1
console.log(myArray[1]); // 2
console.log(myArray[2]); // 3
```

### Array Methods

Arrays have many built-in methods that allow us to manipulate the values in the array. Some of the most common methods are: `push`, `pop`, `shift`, `unshift`, `slice`, `splice`, `concat`, `join`, `indexOf`, `includes`, `reverse`, `sort`, and `forEach`.

#### `push`

The `push` method adds a value to the end of an array.

```js
const myArray = [1, 2, 3];
myArray.push(4);
console.log(myArray); // [1, 2, 3, 4]
```

#### `pop`

The `pop` method removes the last value from an array and returns it.

```js
const myArray = [1, 2, 3];
const lastValue = myArray.pop();
console.log(myArray); // [1, 2]
console.log(lastValue); // 3
```

#### `shift`

The `shift` method removes the first value from an array and returns it.

```js
const myArray = [1, 2, 3];
const firstValue = myArray.shift();
console.log(myArray); // [2, 3]
console.log(firstValue); // 1
```
