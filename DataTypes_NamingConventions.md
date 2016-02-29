JavaScript is dynamically weakly typed 

Six data types that are primitives: 
1.Boolean 
2.Null 
3. Undefined 
4. Number 
5. String 

Symbol (new in ECMAScript 6) 
6. and Object 
 
Examples: 

var length = 16;                               // Number 
var lastName = "Johnson";                      // String 
var cars = ["Saab", "Volvo", "BMW"];           // Array 
var x = {firstName:"John", lastName:"Doe"};    // Object 


Variables in JavaScript are like those in any other language; you use them to hold values that can be accessed in different places in the code. The identifiers are unique and consist of a combination of letter, digits, underscores and dollar signs. JavaScript does account for upper and lower case characters. MUST Begin with a character, dollar sign, or underscore: 
_variable 
_ _variable 
variable 
$variable 


A constructor function starting with new should always start with a capital letter  
  var example = new Application() 

Method/function should always start with a small letter  
  Function myFunction(){…} 

Variables with multiple words should always use an underscore between words 
  var coffee_shop =1; 

Element Classes and IDs. JavaScript can access elements by their ID attribute and class names. IDs and class names with multiple words should be separated by underscore (same a variables) 
  Ex.setAttribute("id", "distinct_id"); 

Private methods use leading underscore to separate them from public methods 
  "_getLast": function () {…} 
  Return this._getLast(); 



x = "5" + 6 
It will compile but x would be 56 because when numbers are in ""  it is the literal meaning  
Note: Always have spaces around operators and after commas 


1. Trusty/Falsy numbers:  The == / != operators will work as you might expect if the operands are of the same type (boolean), but if they are not, the == and != operators try to coerce the values 
JavaScript evaluates the values in the list below as false, and everything else as true: 
  false 
  null 
  empty string (“”) 
  0 
  NaN 
the strict === and !== operators are the best way to go 

2. () function : Can do many tasks but should be limited to: 
Allow script to run dynamically 
Parsing JSON (but JSON.parse() method works better) 
Try to stay away form eval()  

3. JavaScript uses variables of global proportions. This can cause complex sites with nasty bugs. Avoid using global variable because:  
  -Easy to have naming variable clashes  
  -Easy to overwrite wrong variables 
  -"Floaters" tend to hang around and do nothing, variables are not declared 
JavaScript doesn’t perform block scope, so variables you define can inadvertently become as error prone as global variables.  
 
 
JavaScript variables can be converted to a new variable and another data type: 
By the use of a JavaScript function 
Automatically by JavaScript itself 


Sources

http://www.w3schools.com/jsref/jsref_operators.asp Accessed Feb 11, 2016 

http://www.j-io.org/Javascript-Naming_Conventions Accessed Feb 11, 2016 

http://archive.oreilly.com/pub/a/javascript/excerpts/learning-javascript/javascript-datatypes-variables.html Accessed Feb 11, 2016 

http://www.w3schools.com/js/js_conventions.asp Accessed Feb 11, 2016 

http://rachelappel.com/common-javascript-mistakes-and-pitfalls-you-can-avoid/ Accessed Feb 11, 2016 

http://www.w3schools.com/js/js_datatypes.asp Accessed Feb 11, 2016 

http://www.w3schools.com/js/js_type_conversion.asp Accessed Feb 11, 2016 

