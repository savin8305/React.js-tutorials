![Screenshot (12971)](https://github.com/savin8305/React.js-tutorials/assets/118232727/3c054ecb-d5a3-491d-a173-92c6308f76c7)
![Screenshot (12973)](https://github.com/savin8305/React.js-tutorials/assets/118232727/015cc1aa-7487-4168-8877-764f3ede6450)
```
##  In the context of function calls, the spread operator can be used to pass the elements of an array as argument values to a function. For example:
function myFunction(x, y, z) {
  console.log(`x=${x}, y=${y}, z=${z}`);
}

const myArray = [1, 2, 3];
myFunction(...myArray); // logs "x=1, y=2, z=3".

## In the context of array literals, the spread operator can be used to concatenate arrays or create a shallow copy of an array. 
const array1 = [1, 2, 3];
const array2 = [4, 5, 6];

const concatenatedArray = [...array1, ...array2]; // [1, 2, 3, 4, 5, 6]
const copiedArray = [...array1]; // [1, 2, 3]
## In the context of object literals, the spread operator can be used to merge multiple objects into a single object. For example:

const obj1 = { name: 'Alice', age: 30 };
const obj2 = { city: 'New York' };

const mergedObject = { ...obj1, ...obj2 }; // { name: 'Alice', age: 30, city: 'New York' }

