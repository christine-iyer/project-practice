This is my code so far for the luhn algo. 
4 4 0 8 0 4 1 2 3 4 5 6 7 89 3

```js
const array = [4, 4, 0, 8, 0, 4, 1, 2, 3, 4, 5, 6, 7, 8, 9, 3]
let even = [];
let odd = [];
let evenLess = [];
let evenMore = [];
const sumArray = (array) => {
     let total = 0;
     for (let i = 0; i < array.length; i++) {
          total += array[i];
     }
     return total
}
reversed = array.reverse()

for (var i = 0; i < reversed.length; i++) {
     if (i % 2 !== 0 || i == 0) {
          even.push(reversed[i]);
     } else {
          odd.push(reversed[i])
     }
}
for (var i = 0; i < reversed.length; i++) {
     if (i % 2 !== 0 || i == 0) {
          evenLess.push(even[i]);
     } else {
          evenMore.push(even[i])
     }
}
console.log("odd: ", odd," ",sumArray(odd))
console.log(reversed)
console.log("even: ",sumArray(even))
console.log("evenMore is: ", evenMore)
console.log("evenLess is: ", evenLess)
```

![](./public/images/Screen%20Shot%202022-12-14%20at%202.14.31%20PM.png)


