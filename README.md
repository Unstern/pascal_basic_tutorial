# pascal_basic_tutorial

Pascal Program Structure
A Pascal program basically consists of the following parts −

Program name
Uses command
Type declarations
Constant declarations
Variables declarations
Functions declarations
Procedures declarations
Main program block
Statements and Expressions within each block
Comments
Every pascal program generally has a heading statement, a declaration and an execution part strictly in that order. Following format shows the basic syntax for a Pascal program −

program {name of the program}
uses {comma delimited names of libraries you use}
const {global constant declaration block}
var {global variable declaration block}

function {function declarations, if any}
{ local variables }
begin
...
end;

procedure { procedure declarations, if any}
{ local variables }
begin
...
end;

begin { main program block starts}
...
end. { the end of main program block }
Pascal Hello World Example
Following is a simple pascal code that would print the words "Hello, World!" −

 Live Demo
program HelloWorld;
uses crt;

(* Here the main program block starts *)
begin
   writeln('Hello, World!');
   readkey;
end. 
This will produce following result −

Hello, World!
