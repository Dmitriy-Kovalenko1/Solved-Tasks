````javascript

 #### Sleigh Authentication.

function Sleigh() {}

Sleigh.prototype.authenticate = function(name, password) {
  return name == "Santa Claus" && password == "Ho Ho Ho!";
}; 

#### Beginner Series #4 Cockroach.

function cockroachSpeed(s) {
  return Math.floor(s * 100000 / 60 / 60); 
}
#### Beginner Series #4 Cockroach other option. ###

function cockroachSpeed(s) {
  const secsInHour = 3600;  
  const centimetersInKilometers = 100000;
  
  return Math.floor((s*centimetersInKilometers)/secsInHour);



