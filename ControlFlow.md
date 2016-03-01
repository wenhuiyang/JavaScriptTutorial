<h1>JavaScript Control Flow</h1>


<h2>One condition: if/else statement</h2>

In JavaScript, if/else statements can be use and else if as well as switch cases. 
<b>If</b> for a block of code to be executed when condition is true
<b>else</b> for a block of code to be executed when same condition is false
This is an example:

```JavaScript
If (guess = 12) {
output= “Good guess”;
} else {
	output= “Wrong guess”;
}
```

<b>else if</b> for a new condition to test if the first condition is false
This is an example:

```JavaScript
if (location <10) {
	loc = “Almost there”;
} else if (location<5) {
	loc= “Getting closer”;
} else {
	loc = “Yes, you’re here!”;
```

<h2>Multiple Conditions: If/else statements</h2>

JavaScript can have multiple conditions with switch statements 
<b>switch</b> for many alternative blocks of code to be executed.
Note: Must use break statements.
This is an example:

```JavaScript
switch (new Date(). getMonth( )) {
	case 0:
		month = “January”;
		break;
	case 1:
		month = “February”;
		break;
	case 2:
		month = “March”;
		break;
	case 3:
		month = “April”;
		break;
	case 4:
		month = “May”;
		break;
	case 5:
		month = “June”;
		break;
	case 6:
		month = “July”;
		break;
	case 7:
		month = “August”;
		break;
	case 8:
		month = “September”;
		break;
	case 9:
		month = “October”;
		break;
	case 10:
		month = “November”;
		break;
	case 11:
		month = “December”;
		break;
}
```

If/else statement with multiple conditions use and <b> &&</b> and or <b>||</b>
JavaScript has “short-circuit” logic:

```JavaScript
If (true == true || code.code) {
	//Passes, no errors because code isn’t defined
}
If (false && code.code){
	//Passes, no errors because code isn’t defined
}
```

<h2>Dangling else pitfall</h2>

The dangling else statement is not clear to which of the two if statements it belongs:
Note: Use Braces, problem solved. 

```JavaScript
If (answer = true) {
	If (guess = 4) {
		document.write("you guessed right!");
	} else {
		document.write("Guess again");
}
}
```
<h2>Loops</h2>

These can be used with all loops in JavaScript:
```JavaScript
break [<label>]  
	//Exit from a loop
continue [<label>]
	//Stop the current loop iteration, and immediately continue with the next one
```

Labels: an identifier followed by a colon. In front of a loop, the label allows you to break or continue that loop even from a loop nested inside of it. The name of the label becomes an argument of break or continue.
This is an example:

```JavaScript
function findoddnumber(list) {
	loop: {//label
		for (var i=0; i<list.length; i++) {
			var num = list[i];
			if (num%2) === 1) {
				console.log (‘Found:’ + num);
				break loop;
			}
		}
		console.log(“No odd number found.”);
		}
	console.log(“Complete search”);
}

```
<h2>Loop Statements: While </h2>
While loops execute statement as long as the condition holds. If it is always true, you have an infinite loop.
This is an example:
```JavaScript
While (x<10) {
	document.write(“Less than 10”)
}
```
<h2>Loop Statements: do-while </h2>
Do-while loops execute statements at least once and then as long as condition holds. 
This is an example: 
```JavaScript
var state;
do{
	state = prompt (“Enter your current state”);
} while (tries<10);

```

<h2>Loop Statements: for</h2>
For loops iterate for statement that holds true
This is an example:
```JavaScript
var arraylist = [ ‘a’, ‘b’, ‘c’];
for (var i=0; i<arraylist.length, i++){
	console.log(arraylist[i]);
}
```
<h2>Other Loop Statements: for-in, for each-in</h2>
Both of the loop statements are not recommend, do use with caution 
<b>For-in loop</b> iterates over all property keys of object including inherited ones. But rules apply:
-	Can use var to declare variables, but the scope of variables is always the complete surrounding function
-	Properties can be deleted during iteration
NOTE: Don’t use for-in for arrays, be careful with for-in for objects
<b>For each-in loops</b> exists only in Firefox. Do not recommend using. 

<h2>The with Statement </h2>
```JavaScript
var object = {student: ‘Victoria’};
with (object) {
	console.log (‘hello’ +first); //hello Victoria 
}
```
With statement is not recommended because there are three problems the with statement causes:
1.	<b>Performance suffers variable</b> lookup becomes slower
2.	<b>Code becomes less predictable</b> cannot determine what an identifier refers to by looking at its syntactic. 
3.	<b>Minifies can’t shorten variable names</b> inside the with statement, you can’t statically determine whether a name refers to a variable or a property. Because only variables can be renamed by minifies 

<h2>The debugger Statement</h2>
The syntax for the debugger statement:
```JavaScript
debugger;
```
only if debugger is action, this is the breakpoint. 


<h2>Sources</h2>

http://www.w3schools.com/js/js_switch.asp Accessed Feb 29, 2016

http://speakingjs.com/es5/ch13.html Accessed Feb 29, 2016

http://javascript.info/tutorial/setup-your-environment Accessed Feb 29, 2016

	









