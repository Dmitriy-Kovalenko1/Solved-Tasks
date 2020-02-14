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
* Training JS #4: Basic data types--Array
```javascript
function getLength(arr){
  return arr.length;
}
function getFirst(arr){
  return arr[0];
}
function getLast(arr){
  return arr[arr.length-1];
}
function pushElement(arr){
  arr.push(1);
  return arr;
}
function popElement(arr){
  arr.pop()
  return arr;
}
```
* task 33
* A wolf in sheep's clothing
```javascript
function warnTheSheep(queue) {
if(queue[queue.length - 1] == "wolf")
return "Pls go away and stop eating my sheep";
for(let i =0;i < queue.length -1;i++)
{
if(queue[i] == "wolf")
return  "Oi! Sheep number "+(queue.length - i - 1).toString()+"!"+" You are about to be eaten by a wolf!";
}

}
```
* task 34
* Be Concise IV - Index of an element in an array
```javascript
let find = (a, e) => {
  return a.indexOf(e) >= 0 ? a.indexOf(e) : "Not found";
}
```
* task 35
* Tail Swap
```javascript
function tailSwap(arr) {
  let arr1 = arr[0].split(':');
  let arr2 = arr[1].split(':');
  let temp = arr1[1];
  arr1[1] = arr2[1];
  arr2[1] = temp;
  return [arr1.join(':') , arr2.join(':')]
}
```
* task 36
* Tail Swap
```javascript
function tailSwap(arr) {
let arr0 = arr[0].split(':');
let arr1 = arr[1].split(':');
return [arr0[0] + ':' + arr1[1], arr1[0] + ':' + arr0[1]]
}
```
* task 37
* A Needle in the Haystack
```javascript
function findNeedle(haystack) {
  return "found the needle at position " + haystack.indexOf("needle");
}
```
* task 38
* Grasshopper - Grade book
```javascript
function getGrade (s1, s2, s3) {
let avg = (s1 + s2 + s3) /3;
return avg >= 90 ? 'A' :
       avg >= 80 && avg < 90 ? 'B' :
       avg >= 70 && avg < 80 ? 'C' :
       avg >= 60 && avg < 70 ? 'D' :
       avg < 60 ? 'F' : true
}
```
* task 39
* How good are you really?
```javascript
function betterThanAverage(classPoints, yourPoints){
return classPoints.reduce ((a, b) => a + b) / classPoints.length < yourPoints ? true : false;
}
```
* task 40
* How good are you really?
```javascript
function betterThanAverage(classPoints, yourPoints) {
let sum = 0;
for(let i = 0; i < classPoints.length; i++){
sum = sum + classPoints[i]
}
let avg = sum / classPoints.length;
return yourPoints > avg ? true : false;
}
```
* task 41
* How good are you really?
```javascript
function betterThanAverage(classPoints, yourPoints) {
  return classPoints.reduce((a, b) => a + b, 0)/ classPoints.length < yourPoints;
}
```
* task 42
* Divide and Conquer
```javascript
function divCon(x){
sumN = 0;
sumS = 0;
for (let i=0; i<x.length; i++){
if (typeof x[i] === 'number') sumN = sumN+x[i];
else sumS = sumS + +x[i];
} 
return sumN-sumS;
}
```
* task 43
* Calculate average
```javascript
function find_average(arr) {
return arr.reduce((sum, element) => sum + element, 0)/arr.length;
}
```
* task 44
* Calculate average
```javascript
function find_average(arr){
  let sum = 0;
  for (let i=0; i<arr.length; i++){
    sum = sum + arr[i];
  }
   return sum/arr.length;
}
```
* task 45
* Calculate average
```javascript
function find_average(array) {
 let sum = 0;
   for(let i = 0; i < array.length; i++){
   sum = sum + array[i];
  }
  let avg = sum / array.length;
  return avg;
}
```
* task 46
* Be Concise IV - Index of an element in an array
```javascript
let find = (a, e) => {
return a.indexOf(e) >= 0 ? a.indexOf(e) : "Not found";
}
```
* task 47
* A wolf in sheep's clothing
```javascript
function warnTheSheep(queue) {
if(queue[queue.length - 1] === "wolf")
return "Pls go away and stop eating my sheep";
for(let i = 0; i < queue.length - 1;i++){
if(queue[i] === "wolf")
return "Oi! Sheep number "+(queue.length - i - 1).toString()+"!"+" You are about to be eaten by a wolf!";
}
}
```
* task 48
* Training JS #4: Basic data types--Array
```javascript
function getLength(arr){
  return arr.length;
}
function getFirst(arr){
  //return the first element of arr
  return arr[0];
}
function getLast(arr){
  //return the last element of arr
  return arr[arr.length - 1];
}
function pushElement(arr){
  arr.push(1); 
  return arr;
}
function popElement(arr){
  arr.pop()
  return arr;
}
```
* task 49
* Powers of 2
```javascript
function powersOfTwo(n){
 let arr = [];
for(let i = 0; i <= n; i++){
 arr.push(Math.pow(2, i));
 }
return arr;
}
```
* task 50
* Array.diff
```javascript
function array_diff (a, b){
  return a.filter(aa => (!b.includes(aa)))
}
```
* task 51
* Array.diff
```javascript
function array_diff(a, b) {

    var arr = new Array();
    
    for(var i = 0;i<a.length;i++){
        if(b.indexOf(a[i])<0){
            arr.push(a[i]);
        }
    }
  
    return arr;
}
```
* task 52
* filterEvenLengthWords
```javascript
function filterEvenLengthWords(words) {
  return words.filter(s=>s.length%2===0)
}
```
* task 53
* filterEvenLengthWords
```javascript
const filterEvenLengthWords = words => words.filter(x => !(x.length % 2));
```
* task 54
* Find how many times
```javascript
function countWins(winnerList, country) {
  let wins = 0;
  for (let i = 0; i < winnerList.length; i++) {
    if (winnerList[i].country === country){
      wins += 1;
    }
  }
  return wins;
}
```
* task 55
* Find Duplicates
```javascript
function duplicates(a) {
  return a.filter((x, i) => a.indexOf(x) == i && a.indexOf(x) != a.lastIndexOf(x));
}
```
* task 56
* Find Duplicates
```javascript
function duplicates(arr) {
let a = arr.filter((el, i) => i === arr.indexOf(el) && i !== arr.lastIndexOf(el)); 
return a;
}
```
* task 57
* Train to remove duplicates from an array with filter()
```javascript
function unique(arr){
return arr.filter((x,y) => y === arr.index.Of(x));
}
```
* task 58 
* Train to remove duplicates from an array with filter()
```javascript
function unique(arr) {
  return arr.filter((x, i) => arr.indexOf(x) === i);
}
```
* task 59
* 
```javascript
function findOdd(arr) {
  return arr.find((item, index) => arr.filter(el => el == item).length % 2)
}
```
* task 60
* String Templates - Bug Fixing #5
```javascript
const buildString = (...v) => `I like ${v.join(', ')}!`
```
* task 61
* Unfinished Loop - Bug Fixing #1
```javascript
function createArray(number){
  var newArray = [];
  
  for(var counter = 1; counter <= number; counter++){
    newArray.push(counter);
  }
  
  return newArray;
}
```
* task 62
* Printing Array elements with Comma delimiters
```javascript
function printArray(array){
  return array.join();
}
```
* task 63
* Printing Array elements with Comma delimiters
```javascript
const printArray=array=>array.join();
```
* task 64
* Printing Array elements with Comma delimiters
```javascript
function printArray(array){
  return array.toString();
}
```
* task 65
* CSV representation of array
```javascript
function toCsvText(array) {
  let arr =[];
  for (i = 0; i < array.length; i++) {
    arr[i] = array[i].join(',');
  }
  return arr.join('\n');
}
```
* task 66
* Unfinished Loop - Bug Fixing #1
```javascript
function createArray(number){
  var newArray = [];
  
  for(var counter = 1; counter <= number; counter++){
    newArray.push(counter);
  }
  
  return newArray;
}
```
* task 67
* Generate range of integers
```javascript
function generateRange(min, max, step){
let arr = [];
for(let i = min; i <= max; i+= step){
arr.push(i);
}
return arr;
}
```
* task 68
* Classic Hello World
```javascript
// Print "Hello World!" to the screen
class Solution{
static main(arr){
console.log('Hello World!');
}
}
```
* task 69
* Count by X
```javascript
function countBy(x, n) {
  let z = [];
  for(let i = 1; i <=n; i++){
  z.push(x * i);
  }
  return z;
}
```
* task 70
* CSV representation of array
```javascript
function toCsvText(array) {
  array.forEach((item) => item.join(","));
  return array.join("\n");
}
```
* task 71
* CSV representation of array
```javascript
function toCsvText(array) {
  const newArr = [];
  for(let i = 0; i< array.length; i++){
    newArr.push(array[i].join(','))
  }
  return newArr.join('\n');
}
```
* task 72
* CSV representation of array
```javascript
function toCsvText(arr) {
   let res = '';
   for (let i = 0; i < arr.length; i++){
    if (i < arr.length -1) res = res + arr[i].join() + '\n';
     else res = res + arr[i].join() ;
    }
  return res;
} 
```
* task 73
* Formatting decimal places #0
```javascript
function twoDecimalPlaces(n) {
  return +n.toFixed(2);
}
```
* task 74
* Formatting decimal places #0
```javascript
function twoDecimalPlaces(n) {
 (n.toFixed(2));
return Math.round (n*100)/100 ;
}
```
* task 75
* Enumerable Magic #1 - True for All?
```javascript
function all( arr, fun ){
  return arr.every(fun)
}
```
* task 76
* Enumerable Magic #1 - True for All?
```javascript
function all( arr, fun ){
 for(i=0;i<arr.length;i++){
 if(fun(arr[i]) !== true){
 return false;
 }
 }
 return true;
};
```
* task 77
* The wheat/rice and chessboard problem
```javascript
function squaresNeeded(grains){ 
  let count = 0;
   let sum = 0;
   let x = 1; 
  while (sum < grains){ 
    sum += x; 
    count++ 
    x *= 2; 
  }  
 return count 
}
```
* task 78
* Beginner Series #3 Sum of Numbers
```javascript
function getSum(a, b){
    let sum = 0; 
   if (a < b)
 for (let i = a; i <= b; i++){
      sum += i  
  }  else for (let i = b; i <= a; i++){ 
    sum += i   
 } 
   return sum 
}
```
* task 79
* Beginner Series #3 Sum of Numbers
```javascript
function getSum(a, b){ 
 let max = Math.max (a, b); 
 let min = Math.min (a, b); 
 let sum = 0;  
 for (let i = min; i <= max; i++){  
  sum += i  
 } 
 return sum 
}
```
* task 80
* No zeros for heros
```javascript
function noBoringZeros(n) { 
 let str = n + '';  
 return +str.replace(/0+$/, '') }
```
* task 81
* What will be the odd one out?
```javascript
function oddOneOut(str) {
    var s = "", len = str.length;
    for (let i = 0; i < str.length; i++){
        let k = str.charAt(i);
        if (s.indexOf(k) === -1){
            s += k; 
        }else {
            s = s.replace(k,"");
        }
    }
    return s.split('');
}
```
* task 82
* Numbers to Objects
```javascript
function numObj(s){
let res = [];
for(let i = 0; i < s.length; i++){
let obj = {};
obj[s[i]] = String.fromCharCode(s[i]);
res.push(obj);
}
return res
}
```
* task 83
* Coding Meetup #5 - Higher-Order Functions Series - Prepare the count of languages
```javascript
function countLanguages(list) {
let answer = {};
for(let i = 0; i < list.length; i++){
if(answer[list[i].language]){
answer[list[i].language]++;
} else {
answer[list[i].language] = 1;
}
} 
return answer
}
```
* task 84
* Regexp Basics - is it a digit?
```javascript
String.prototype.digit = function() {
  let arr = this.match(/[0-9]/g);
  
  if (!arr) return false;
  else if (this.length === arr.length && arr.length === 1) return true;
  else return false;
};
```
* task 85
* Keep up the hoop
```javascript
function hoopCount(n) {
  return n >= 10 ?
    "Great, now move on to tricks" :
    "Keep at it until you get it";
}
```
* task 86
* Keep up the hoop
```javascript
function hoopCount (n) {
  if (n > 0 && n < 10) return "Keep at it until you get it";
  else return "Great, now move on to tricks";
}
```
* task 87
* Arithmetic progression
```javascript
const arithmeticSequenceElements = (a, r, n) => {
  let count = a
  let sequence = [a]
  for (let i = 1; i < n; i++) {
    count += r
    sequence.push(count)
  }
  return sequence.join(', ')
}
```
* task 88
* Split Strings
```javascript
const solution = str => `${str}_`.match(/../g)
```
* task 89
* Find the odd int
```javascript
function findOdd(array) {
  for (let i = 0; i < array.length; i++) {
    const element = array[i]
    let counter = 0

    for (let j = 0; j < array.length; j++) {
      if (element === array[j]) counter++
    }

    if (counter % 2 !== 0) return element
  }
}
```
* task 90
* Grasshopper - Array Mean
```javascript
let findAverage = function(nums){
  return nums.reduce((a, b) => a + b, 0) / nums.length;
}
```
* task 91
* Grasshopper - Array Mean
```javascript
const findAverage = nums => nums.reduce((a,el) => a + el) / nums.length;
```
* task 92
* Grasshopper - Array Mean
```javascript
let findAverage = function (nums){
let res=0;
for (let i=0; i<nums.length; i++){
  res+=nums[i];
}
res=res/nums.length;
return res;
}
```
* task 93
* Grasshopper - Array Mean
```javascript
function findAverage(nums) {
  return nums.reduce(function(a,b) {
    return a+b;
  }) / nums.length;
}
```
* task 94
* My head is at the wrong end!
```javascript
function fixTheMeerkat(arr) {
   let [a,b,c] = arr;
   return [c,b,a];
}
```
* task 95
* Beginner - Reduce but Grow
```javascript
const grow = x => {
  let res = 1;
  for (let i = 0; i < x.length; i++) {
    res *= x[i];
  }
  return res;
};
```
* task 96
* Beginner - Reduce but Grow
```javascript
function grow(x){
  return x.reduce((a, b)=> a * b,1);
}
```
* task 97
* Beginner - Reduce but Grow
```javascript
const grow = x => x.reduce((m,n)=>m*n, 1);
```
* task 98
* Array plus array
```javascript
function arrayPlusArray(arr1, arr2) {
  return arr1.concat(arr2).reduce((acc, cur) => acc + cur);
}
```
* task 99
* Array plus array
```javascript
function arrayPlusArray(arr1, arr2) {
  return arr1.reduce((sum, cur) => sum + cur) + arr2.reduce((sum, cur) => sum + cur);
}
```
* task 100
* Array plus array
```javascript
function arrayPlusArray(arr1, arr2) {
  let r = 0;
  for(let i=0; i<arr1.length;i++){
    r+=arr1[i] + arr2[i];
  }
  return r;
}
```
* task 101
* SpeedCode #2 - Array Madness
```javascript
function arrayMadness(a, b) {
  return a.reduce((prev, curr) => (prev + curr ** 2), 0) > b.reduce((prev, curr) => (prev + curr ** 3), 0);
}
```
* task 102
* SpeedCode #2 - Array Madness
```javascript
const arrayMadness=(a,b)=> a.reduce((acc,curr)=> acc + Math.pow(curr,2),0) >=b.reduce((acc,curr)=> acc + Math.pow(curr,3),0)
```
* task 103
* Enumerable Magic #25 - Take the First N Elements
```javascript
function take(arr, n) {
  return arr.slice(0, n);
}
```
* task 104
* Enumerable Magic #25 - Take the First N Elements
```javascript
const take = (a, n) => a.slice(0, n);
```
* task 105
* Enumerable Magic #25 - Take the First N Elements
```javascript
function take(arr, n) {
  return arr.splice(0,n);
}
```
* task 106
* Enumerable Magic #2 - True for Any?
```javascript
function any(arr, fun){
  return arr.some(fun)
}
```
* task 107
* Enumerable Magic #2 - True for Any?
```javascript
function any(arr, fun){
  for (var i=0; i<arr.length; ++i)
    if (fun(arr[i]))
      return true;
  return false;
}
```
* task 108
* Enumerable Magic #2 - True for Any?
```javascript
function any(arr, fun){
  return arr.some(function(element){
    return fun(element);
  });
}
```
* task 109
* Remove First and Last Character Part Two
```javascript
function array(strg){
    return strg.split(',').slice(1,-1).join(' ') || null
}
```
* task 110
* Remove First and Last Character Part Two
```javascript
function array(arr){
let a = arr.split(',');
if (a.length <=2) {return null;}
return a.slice(1,a.length-1).join(' ');
}
```
* task 111
* The Office I - Outed
```javascript
function outed(meet, boss){
let sum = meet[boss];
let a = 'Get Out Now!';
let b = 'Nice Work Champ!';
  for(let key in meet){
 sum += meet[key];
}
return (sum/Object.entries(meet).length <= 5) ? a : b
}
```
* task 112
* The Office I - Outed
```javascript
function outed(meet, boss){
  var sum = 0;
  var length = 0;
  for (var person in meet) {
    if (person === boss) {
      sum += meet[person];
    }
    sum += meet[person];
    length++;
  }
  var total = sum / length;
  if (total <= 5) {
    return 'Get Out Now!';
  } else {
    return 'Nice Work Champ!';
  }
}
```
* task 113
* Jenny's secret message
```javascript
function greet(name){  
  if(name === "Johnny")
    return "Hello, my love!";
  return "Hello, " + name + "!";
}
```
* task 114
* Jenny's secret message
```javascript
function greet(name){
  return name === "Johnny" ? "Hello, my love!" : `Hello, ${name}!`;
}
```
* task 115
* Template Strings
```javascript
let TempleStrings = function(obj, feature) {
  return `${obj} are ${feature}`;
}
```
* task 116
* Returning Strings
```javascript
function greet(name){
  return `Hello, ${name} how are you doing today?`;
}
```
* task 117
* Returning Strings
```javascript
function greet(name) {
  return "Hello, " + name + " how are you doing today?";
}
```
* task 118
* Grasshopper - Combine strings
```javascript
const combineNames = (a, b) => `${a} ${b}`;
```
* task 119
* Grasshopper - Combine strings
```javascript
let combineNames = function(first, last){
  return first + ' ' + last;  
};
```
* task 120
* Grasshopper - Debug sayHello
```javascript
function sayHello (name) {
  return 'Hello, ' +  name;
}
```
* task 121
* get character from ASCII Value
```javascript
getChar = c => String.fromCharCode(c);
```
* task 122
* 






