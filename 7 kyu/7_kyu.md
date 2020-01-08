````javascript
#### Power of two.

function isPowerOfTwo(n){
let i = 1;
while ( n >1 ){
n = n/2;
}
return n===1;
}

### Filter the Number 

var FilterString = function(value) {
let b = '';
for(let i = 0; i < value.length; i ++){
if(isNaN(value[i]))
continue
b = b + value[i];
}
return +b;
}

#### Square Every Digit #####

function squareDigits(num){
  var num = num.toString();
  var res = ''
  for (var i = 0; i != num.length; i++){
    res += (Number(num[i]) * Number(num[i])).toString();
  }
  return Number(res);
}

#### You're a square! ####

var isSquare = function(n){
  return Number.isInteger(Math.sqrt(n));
}

### You're a square! ###

const isSquare = n => Math.sqrt(n) % 1 === 0

**********************************

### All Star Code Challenge #22 ###

function toTime(seconds) {
let hours = Math.floor(seconds / 3600);
let min = Math.floor((seconds - (hours*3600))/60 );
return `${hours} hour(s) and ${min} minute(s)`
}
