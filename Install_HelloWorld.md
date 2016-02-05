Installation 

JavaScript is plain text. You can use any text editor to read/write/edit plain text. Programmers' text editors will do syntax highlighting and checking. Some examples are: Sublime Text,  Notepad++, Atom, Brackets, Light Table, Vim. All text editors can be downloaded on any operating system (Windows, Mac, Unix/Linux) 
You need to enable JavaScript on your web browser where it is executed. Follow these steps to enable JavaScript on your web browser: http://www.enable-javascript.com/ 
 
Creating and Running Perl 
 
There are two options to run programs that you write: 

1. Browsers load HTML pages (option to load and execute JavaScript code vis <script> tag 
Create HTML page 
Put it to the same folder with .JS file 
In HTML have a <script tag that loads your code  
	<html> 
	<head> 
	<script src="myjsfile.js"></script> 
	</head> 
	<body> 
	</body> 
	</html> 

perl -v
Open this HTML file in Chrome (drag and drop, double click) 
2. Using sublime text via build systems features  
Built system is described on JSON file with .sublime-build extension. Create new one by going to Tools > Build System > New Build System and paste this code: 
{ "cmd": ["/usr/local/bin/node", "$file"], "selector": "source.js" } 
Save file as JavaScript.sublime-build inside User directory 
Create JavaScript file, code script and click Cmd + B (Mac) or F7 (Windows). Or go to Tools > Build 

// You can get started coding! 

The // is used to start comments in JavaScript programming. To write "Hello, World!", the progrom looks like this:

//JavaScript
<html><body><p>Header</p><script>altert('Hello, World!')</script><p>Footer</p></body></html> 
 
Sources

http://lifehacker.com/five-best-text-editors-1564907215 Accessed Feb.5, 2016

https://pawelgrzybek.com/javascript-console-in-sublime-text/ Accessed Feb.5, 2016

http://javascript.info/tutorial/hello-world Accessed Feb. 5, 2016
