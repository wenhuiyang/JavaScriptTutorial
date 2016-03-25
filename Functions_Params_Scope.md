<h1>JavaScript</h1>

A <b>function</b> is a JavaScript procedure- a set of statements that performs a task or calculates a value. To use a function, you must define it somewhere in the scope from which you want to call it. 

<b>Function Declarations</b>
A function declaration consists of:
-	The name of the function
-	A list of arguments to the function, enclosed in parentheses and separated by commas
-	The JavaScript statements that define the function, enclosed in curly brackets { }.
An example of a function declaration:

```JavaScript
function squarearea (number) {
return number*number;
}
```

Non-primitive values such as an Object as a parameter are passed by reference; if the function changes the object’s properties, it changes the original value and are visible outside the function. This is an example:

```JavaScript
function myFunc (theObject) {
	theObject.class = “CS 330”
}
var myClass = {class: “CS 333”, section: 1, name: “Database Management Systems”};
var x, y;
x= myClass.class;  // x gets the value “CS 333”
myFunc (myClass);
y = myClass.class;  //y gets the value “CS 330” 
//The class property was changed by the function

```

<b>Function Expressions</b>
Function expressions can be anonymous, does not have to have a name. For example:
```JavaScript
var squarearea = function (number) {return number*number};
var x = squarearea (5) // x gets the value 25
```

Function expressions are useful when passing a function as an argument to another function. This is an example:

```JavaScript
function map (f, a) {
var result = [ ],  //Create a new Array
i;
for (i= 0; I != a. length; i++)
	result[i]= f(a[i]);
return result;
```

calling the function:

```JavaScript
	map(function(x) {return x* x* x}, [0,1,2,5,10]);
returns [0,1,8,125,1000]
```

A function is a “subprogram” that can be called by code external or internal to the function. In JavaScript, functions are first-class objects because they can have properties and methods just like any other object. But what is different is that functions can be called. Every function in JavaScript is a Function Ojbect. Function always returns a value whereas a procedure might not.
Functions must be in scope when they are called but the function declaration can appear below the call in the code.

JavaScript supports recursive functions, that call itself. 
This is an example:

```JavaScript
function factorial (num) 
{ 
//if number is 0, no
If (num <0) {
	Return -1;
}
//if the number is 0, its factorial is 1
else if (number== 0) {
	return 1;
}
//else, call recursively 
else {
	return (num * factorial (num-1));
}
}
var answer = factorial (10);
```

JavaScript functions can accept multiple parameters that are of different data types 
Parameter rules:
-	function definitions do not specify data types for parameters
-	functions do not perform type checking on the passed arguments
-	functions do not check the number of arguments received 
JavaScript is a dynamically typed language, it can be passed different data types 

JavaScript functions cannot return multiple values at the same time. It can return an array containing all values. 

If you declare a variable x in the main body and then declare a value of the same name inside a loop, this is a conflict because you are overriding the original variable. Cannot have two variables of the same name in the same scope.

If the other x is inside a function, it is possible and would not cause a conflict because it is in a different scope.

A variable declared outside a function becomes GLOBAL. A global variable has global scope: All scripts and functions on a web page can access it. This is an example:
```JavaScript
var name =”Bob”;
//any code here can use name
function myFunc () {
	//any code here can use name 
} 
```


Primitive parameters such as a number, are passed to function by value; it is passed to the function, the function changes the value of the parameter, this change is not changed globally
Non-primitive values such as an Object as a parameter are passed by reference; if the function changes the object’s properties, it changes the original value and are visible outside the function.


Take a look at how JavaScript passes its variables with this example:

``` JavaScript
var x = [“x”, “y”, “z”];
var y = [“a”, “b”, “c”];
x = y;
y [1] = “u”;
print x;  // x will print [“a”,”u”,”c”]
print y;  // y will print [“a”,”u”,”c”]
``


<h1>Sources</h1>


https://msdn.microsoft.com/en-us/library/wwbyhkx4(v=vs.94).aspx Accessed March 23, 2016 

http://www.w3schools.com/js/js_scope.asp Accessed March 23, 2016

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions Accessed March 23, 2016

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions Accessed March 23, 2016

http://www.w3schools.com/js/js_function_parameters.asp Accessed March 23, 2016

http://www.w3schools.com/js/js_function_parameters.asp Accessed March 23, 2016

