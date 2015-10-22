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


var alphaBet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
var lengthText = alphaBet.length;
console.log(lengthText)

//String Methods
//There are several string methods one can use you can find the list of methods online. 
var str = ["Hello", "World", "Eat", "Sleep", "Code", "Repeat"] ;
var pos = str.indexOf("Code"); //4
console.log(pos)

str = "Eat, Sleep, Code, Repeat";
var strRep = str.replace("Repeat","Again");
console.log(strRep)  //Eat, Sleep, Code, Again

var str = "Hello World!";       
var str2 = str.toUpperCase(); 
console.log(str2)  //Converts the string to Upper Case "HELLO WORLD!"

var str = "Hello World!";       
var str2 = str.toLowerCase(); 
console.log(str2)  //Converts the string to lower case "hello world!"


var str = "Programming Languages";
str.charAt(6);   //CharAt returns a character in that position "m"

var str = "Programming Languages";
str.charCodeAt(6);   //charCodeAt returns the unicode of the position //returns 109

var txt = "Programming Languages";       // String
txt.split(" "); //[ 'Programming', 'Languages' ]



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


####Local/Global Variables


```javascript

//This is a local variable

// cannot be used here
function mycarFunction() {
    var carName = "Tesla";
    // can only be used here
}


//This is a Global variable
var carName = " Tesla";

// can be used here
function mycarFunction() {
    // can be used here
}

```



####Commenting 
```javascript
/*
Everything that is beteen the symbols is commented.
*/

// This is also comment

``` 

####Operators

```javascript

//Arithmetic Opreators
 +    //addition
 *    //subtraction
 /    //division
 %    //modulus
 ++    //increment
 --   // deincrement
 
 //String Operators
 text1 = "Jonathan";
 text2 = "Moreno";
 text3 = text1 + " " + text2;
 console.log(text3); //Jonathan Moreno
 
 //Comparison and Logical Operators
 ==
 ===
 !=
 !==
 >
 <
 >=
 <=
 

```


####Data Types
```javascript

var length = 16;                               // Number
var lastName = "Moreno";                      // String
var cars = ["Eat", "Sleep", "Code"];           // Array
var x = {firstName:"Jonathan", lastName:"Moreno"};    // Object

```

####Objects
```javascript

//Object properties
var person = {
    firstName : "Jonathan",
    lastName  : "Moreno",
    ocupation : "programmer",
    eyeColor  : "brown"
};

person.firstName + " "+person.lastName + " is "+ "a " + person.ocupation + ".";
//Jonathan Moreno is a programmer.


```


####typeof Operator
```javascript

typeof "john" + " " +       //String
typeof 3.14 + " " +        //Number
typeof false + " " +       //Boolean
typeof [1,2,3,4] + " " +   //Object
typeof {name:'john', age:34}; //Object


```


####Functions
```javascript

function addFunction(num1, num2) {
    return num1 + num2;  // The function returns the sum of num1 and num2
}

addFunction(3 ,6)  //9


console.log("The sum of both numbers is" + " "+ addFunction(5,5));
//The sum of both numbers is 10



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
