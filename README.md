## **CodeWars**
* task 1
```javascript
let y = -11 < 0 ? true : false;
console.log(y);
```
* task 2
```javascript
### Holiday VIII - Duty Free

function dutyFree(normPrice, discount, hol){
  return(Math.floor(hol / normPrice / discount * 100))
}
```
* task 3
```javascript
const smash = words => words.join(' ');  
```
* task 4
```javascript
### Convert to Binary.

const toBinary = n => +n.toString(2)
```
* task 5
* Formatting decimal places #0
```javascript
function twoDecimalPlaces(n) {
return Math.round(100 * n)/100;
}
```
* task 6
```javascript
function excludingVatPrice(price){
  if(price === null){
  return -1;
}
else return +(price/1.15).toFixed(2)
}
```
* task 7
* Remove the minimum
```javascript
function removeSmallest(numbers) {
let newArray = [];
let index = numbers.indexOf(Math.min(...numbers));
console.log(index)
for(let i = 0; i < numbers.length; i++){
if(i !== index)
newArray.push(numbers[i]);
}
return newArray;
}
```

























