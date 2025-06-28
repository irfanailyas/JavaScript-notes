
1.EQUALITY CHECKING WITH EQUALITY == operator:-This does the type conversion and does the usual equality checking.
function check(val) {
if (val == 12) {
 return "equal";
}
return "not equal";
}
console.log(check(10));

2.EQUALITY CHECKING WITH STRICTLY EQUALITY OPERATOR === :- This does the equality checking too but doesnot do the type conversion i.e;
function check(val) {
if (val === 7) {
return "equal";
}
return "not equal";
}
console.log(check(10));
Here if we pass a number itself then it will be true and if we pass a string then it will be false.

3.CHECKING WITH INEQUALITY != OPERATOR:-
function check(val) {
if (val != 99) {
 return "yes";
}
return "no";
}
console.log(check(10));
Here we get "no".

4.CHECKING WITH STRICTLY INEQUALITY !== OPERATOR:-
function check(val) {
if (val !== 99) {
return "yes";
}
return "no";
}
console.log(check(10));
This is exact opposite of strictly inequality and likewise this too doesnot do the type conversion.

5.OPERATORS LIKE > >= < <=
6.LOGICAL OPERATORS :-
&& logical AND operator
|| logical OR operator

CONDITIONAL STATEMENTS:-
1.if statement
2.if-else statement
3.nested if statement
4.if-else if-else:- In this the logic or the statements should be ordered.
5.Chaining if-else if statements

EXAMPLE OF GOLF GAME SCORE:-
var names = ["Hole-in-one", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];
function golfScore(par,strokes) {
if (strokes == 1)
{
 return names[0];
}
else if(strokes <= par-2)
{
 return names[1];
}
else if(strokes == par-1)
{
 return names[2];
}
else if(strokes == par)
{
 return names[3];
}
else if(strokes == par+1)
{
 return names[4];
}
else if(strokes == par+2)
{
 return names[5];
}
else if(strokes == par+3)
{
 return names[6];
}
}
console.log(golfScore(5,4));

6.SWITCH CASE STATEMENTS:-
function cases(val) {
var answer = "";
switch(val) {
case 1:
 answer = "alpha":
 break;
case 2:
 answer = "beta";
 break;
default:
 answer = "stuff";
 break;
}
return answer;
}
console.log(cases(1));
Default is like the else statement in if-else statement.
















