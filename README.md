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
* task 8
* Remove the minimum
```javascript
function removeSmallest(numbers) {
  numbers = numbers.slice(0);
  const min = Math.min(...numbers);
  numbers.splice(numbers.indexOf(min),1);
  return numbers;
}
```
* task 9
* Binary Addition
```javascript
function addBinary(a,b) {
return (a + b).toString(2);
}
```
* task 10
* Convert to Binary
```javascript
function toBinary(n){
  return Number(n.toString(2));
}
```
* task 11
* Convert to Binary
```javascript
function toBinary(n){
  return Number(n.toString(2));
}
```
* task 12
* Lario and Muigi Pipe Problem
```javascript
function pipeFix(numbers){
let a = Math.max(...numbers); 
let b = Math.min(...numbers);
let arr = [];
for(i = b; i <= a; i++){
arr.push(i);
}
return arr
}
```
* task 13
* Bin to Decimal
```javascript
const binToDec = bin => parseInt(bin, 2);
```
* task 14
* Hex to Decimal
```javascript
function hexToDec(hexString){
return parseInt(hexString,16);
}
```
* task 15
* Is every value in the array an array?
```javascript
const arrCheck = value => value.every(Array.isArray);
```
* task 16
* Parse nice int from char problem
```javascript
function getAge(inputString) {
  return parseInt(inputString.match(/\d/).join(''))
}
```
* task 17
* No zeros for heros
```javascript
function noBoringZeros(n) {
  if (n === 0) return 0
  const number = String(n)
  let result = number
  for (let i = 0; i < number.length; i++) {
    if (result.endsWith('0')) {
      result = result.substring(0, result.length - 1)
    }
  }
  return Number(result)
}
```
* task 18
* Remove the minimum
```javascript
function removeSmallest(numbers) {
  numbers = numbers.slice(0);
  const min = Math.min(...numbers);
  numbers.splice(numbers.indexOf(min),1);
  return numbers;
}
```
* task 19
* Simple Fun #74: Growing Plant
```javascript
function growingPlant(upSpeed, downSpeed, desiredHeight) {
  if (upSpeed > desiredHeight) downSpeed = 0;
  return x = Math.ceil( (desiredHeight - downSpeed) / (upSpeed - downSpeed) );
}
```























