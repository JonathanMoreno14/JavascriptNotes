# JavascriptNotes
This repository are notes that consist of basic Javascript features. These features include the usage of conditional statements, loops, arrays, functions with parameters ranging from arrays to objects. These notes are a reference for Javascript. Theres will be more items added.


##Basics

####Strings
```javascript
"This is a string "  //This is a string in Javascript

"It's okay";             // Single quote inside double quotes
//It's okay
"His name is 'John'";    // Single quotes inside double quotes
//His name is 'John'
'His name is "John"';    // Double quotes inside single quotes
//His name is "Johnny"


```

####Variables
These variables contain several implications that consist of a string, number, boolean expression, and array. 
```javascript
var thisVariable = 'Hello World';
var thisVariable = '14';
var thisVariable = true;
var thisVariable = [1, 14, 'Hello World', 'How are you doin?'] ;
``` 

####Assigned Variables with Arithmetic Operators
```javascript

// This are assigned variables 
var y = 5;
var x = 5;
console.log(x+y);  //10
console.log(x-y);  //0
console.log(x/y);  //1
console.log(x*y);  //25

var num1 = 5;
var num2 = 6;
var total = num1 + num2;  
console.log(total);  //11
var num1 = 5;
var num2 = 6;
var total = num1 * num2;
console.log(total);  //30

```


####Commenting 
```javascript
/*
Everything that is beteen the symbols is commented.
*/

// This is also comment

``` 



## This is a function with an array as the parameter
The function returns the sum of all the elements in an array. 

```javascript

  function loop(array){
  var count = 0;
   for(var i=0, n=array.length; i < n; i++) 
   { 
      count += array[i]; 
   }
   return count;
}


``` 

## This is a function with a person/object as it's parameters
The function returns the persons information. 

```javascript
function describePerson(person) {
      person = {};
      person.name = "Unknown";
      person.age = "Unknown";
      return person;
}

```


##This function has an array as it's parameters
This function loops through a given array 'nums' then searches each number and 'pushes' the odds and evens numbers into their respected arrays.

```javascript
var evens = [];
var odds = [];


var nums = [];
nums.sort();
function oddsAndEvens(nums){
for (var i = 0; i < nums.length; i++) {
  if (nums[i]%2){ 
            odds.push(nums[i]); 
        }
        else {
            evens.push(nums[i]); 
            
        }
}}

```

##This function has an object as it's user for the parameter
This function loops through the user object checking each value is truthly. If the value is falsy the object is removed. The function returns the truthly information about the user. 

```javascript
function truthyObjLoop(user){
    for(var key in user){
        if(user.hasOwnProperty(key) && !user[key]) 
        delete user[key];
    }
    return user;
}
```
