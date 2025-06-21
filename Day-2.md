
Variable names and function names in js are case sensitive.First letter should be capitalized.
Operation in variables:-
1.ADDITION, SUBTRACTION, MULTIPLICATION,DIVISION IS STRAIGHT FORWARD:-
var sum=10+10;
console.log(sum);
2.INCREMENTING(a++),DECREMENTING(a--).
3.DECIMAL NUMBER(FLOATING-POINT NUMBER) can be easily written by putting decimal points and operations like MULTIPLICATION,DIVISION,REMAINDER(%) can be done staright-forward.
4.Also operators like +=, -=, /= are there.
5.When js variables are declared they have an initial value of undefined.If you do any mathematical operation in it it will display NaN i.e, NOT A NUMBER.
STRING:-
String delcarations are done by using double quotes.There are escape characters which can be understood by the following example:-
var str="This is"my world"the worlds of"the people""
This will think that the second quote is the end of the string. That's when escape characters are used:-
var str="This is\"my world\"the worlds of\"the people""
This will print "This is"my world"the worlds of"the people""
\' single quote
\" double quote
\\ backslash
\n newline
\r carriage return
\t tab
\b backspace
\f formfeed
1.CONCATENATION OF STRING can be done by using + and += operators.
2.CONCATENATION with variable names :- 
  var name="hello"
  var str= + name + "my name"
  console.log(str);
3.LENGTH OF STRING can be found using .length
 var name="hello"
 len = name.length; 
 OUTPUT=5
4.BRACKETNOTATION :-(Similar to index of array,starts with 0)
 var name = "ADA";
 var letter = "";
 letter = name[0];
 console.log(letter);
OUTPUT=A
5.IMMUTABILITY:-Not cannot be changed at all ,we cannot change a single literal but can change the whole string and assign a new one.
6.To find the nth character we can use bracket notation or by specifying index.
7.To find the last character in a string :-
 var name = "hello";
 var last = name[name.length-1];

ARRAYS:-
It starts and ends with square brackets[]. It can include multiple dataypes.
var a1 = ["hello",12];
1.Accessing data from arrays can be done as:-
var a = a1[0];
2.To modify array data using index:-
var a = [1,2,3];
a[2]=4;
NESTED ARRAY:-One array inside another.
va ary=[[1,2,3],[4,5,6],[7,8,9],[[10,11,12],13,14]];
var data=ary[2][1];
console.log(data);
3.Manipulate or append an array to the end of array:- By using push() function.
var array = ["hello","heyy"];
var res = array.push(["you","are"]);
4.Remove  last element by using pop() function:-
var array = ["hello","heyy"];
var res = array.pop();
OUTPUT=Output of res will be heyy. The last element will be removed and remaining will be returned. Here heyy will be removed and only hello will be there in the array.
5.Manipulate array  by using shift() function:-
var array = ["hello","heyy"];
var res = array.shift();
OUTPUT=.Output of res will be hello. The first element from array will be removed and return the left ones . Here hello will be removed and heyy will be left in the array.
6.Manipulate with unshift() function:- Adds an element to the beginning of an array.
var array = ["hello","heyy"];
var res = array.unshift(["you"]);


FUNCTION:-Statements will be executed only when the function is called.
eg:-
function ourFunction() {
console.log("HEYYA, WORLD");
}
ourFunction(); //CALLING FUNCTION
1.Passing values to function with arguments:-
Parameters are variables that acts as placeholders for values to be input to afunction when it is called.
eg:-
function myFunction(a,b) {  
console.log(a-b);
}
myFunction(10,5);
 2.GLOBAL SCOPE AND FUNCTIONS:-
 Global scope for variables mean that they have scope or access anywhere within our javascript code. Variables defined outside the function has global scope. If in a function you declare a variable without var keyword such as name="hello"; then its scope becomes global throughout the code. But if you declare a variable within the function with a var keyword then its scope will be only within that function.
 3.LOCAL SCOPE AND FUNCTIONS:-
 The variables that are written within the function and within the function parameters, its scope will be local.
         It is possible to have local and global variables with same name, but the local variable gets more value than global one.i.e,
         var wear = "t-shirt";
         function lol() {
         var wear = "sweater";
         return wear;
         }
         console.log(lol());
OUTPUT= "sweater"         But if you call with console.log(wear); it will give "t-shirt".
4.RETURN VALUE FROM A FUNCTION WITH return KEYWORD.


STAND IN A LINE:-
Suppose we want to add an element to the end of an array and return the first element of an array.
JSON.stringify is a way of changing the array elements in the string format inorder to print out easily.
function addUp(arr,item) {
arr.push(item);
return arr.shift();
}
var array = [1,2,3,4,5];
console.log("BEFORE" + JSON.stringify(array));
console.log(addUp(array,6));
console.log("AFTER" + JSON.stringify(array));

if CONDITIONAL STATEMENT:-
function checkUp(a) {
if (a) {
return "YES";
}
return "NO";
}
var a = 13;
