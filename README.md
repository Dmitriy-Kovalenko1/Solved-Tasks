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
* task 20
* Formatting decimal places #0
```javascript
function twoDecimalPlaces(n) {
return Math.round(100 * n)/100;
}
```
task 21
* Total of amount points
```javascript
function points(games) {
 let count = 0;
 for(i = 0;i < games.length; i++){
 let arr = games[i].split(':');
 let x = +arr[0];
 let y = +arr[1];
 if(x > y) count +=3;
 else if(x === y) count +=1;
}
return count;
}
```
* task 22
* Sum of differences in array
```javascript
function sumOfDifferences(arr) {
if(arr.length === 0) return 0;
arr.sort((a, b) => b - a);
return arr[0] - arr[arr.length - 1];
}
```
* task 23
* Find Maximum and Minimum Values of a List
```javascript
const min = list =>list.sort((a, b) => a - b)[0];
const max = list =>list.sort((a, b) => b - a)[0];
```
* task 24
* Sum of two lowest positive integers
```javascript
function sumTwoSmallestNumbers(n) {  
n.sort((a, b) => a - b)
return n[0] + n[1];
}
```
* task 25
* Sum of Odd Cubed Numbers
```javascript
function cubeOdd(arr) {
let sum = 0;                           
for (let i = 0; i < arr.length;i++){  
  if (arr[i] % 2 !== 0 ){
  sum = sum + arr[i]**3;
  } 
 if (typeof(arr[i]) !== 'number'){ return undefined;
 }
}
return sum;
}
```
* task 26
* Odd or Even?
```javascript
function oddOrEven(array) {
  let result = 0;
  for (let i = 0; i < array.length; i++)
  {result + = array[i];}
  if (result % 2 === 0)
  {return "even";}
  else{return "odd";}
}
```
* task 27
* Sum without highest and lowest number
```javascript
function sumArray(array){
  if (array === null || array.length <= 1) return 0;
  let sum = 0;
  for (let i = 0; i < array.length; i++){
    
    if (typeof array[i] == 'object') return 0;
    sum += array[i];
    
  }
  return sum - Math.max(...array) - Math.min(...array);
}
```
* task 28
* Find the divisors!
```javascript
function divisors(integer) {
  let a = [];
  for (i=2;i<integer-1;i++) {
    (integer % i == 0) ? a.push(i) : null
  }
  return a.length > 0 ? a : integer + " is prime" 
};
```
* task 29
* Count by X
```javascript
function countBy(x, n) {
  var z = []
  for (var i = 1; i <= n; i++) {
    z.push(x* i);
  }
  return z
}
```
* task 30
* Generate range of integers
```javascript
function generateRange(min, max, step){
  let arr = [];
  for (let i=min; i<=max; i += step) {
    arr.push(i);
  }
  return arr;
}
```
* task 31
* Training JS #10: loop statement --for
```javascript
function pickIt(arr) {
  let odd  = [];
  let even = [];
  
  for (let i = 0; i < arr.length; i++) {
    let num = arr[i];
    (num % 2 === 0) ? even.push(num) : odd.push(num);
  }
  
  return [odd,even];
}
```
* task 32
* 

















