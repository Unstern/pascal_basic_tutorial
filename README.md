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
Every pascal program generally has a heading statement, a declaration and an execution part strictly in that order.
Following format shows the basic syntax for a Pascal program −

program {name of the program};
uses {comma delimited names of libraries you use};
const {global constant declaration block};
var {global variable declaration block};

function {function declarations, if any};
{ local variables };

begin
 ...
end.

procedure { procedure declarations, if any};
{ local variables };
begin
 ...
end.

begin { main program block starts}
 ...
end. { the end of main program block }




Pascal Hello World Example
Following is a simple pascal code that would print the words "Hello, World!" −

program HelloWorld;
uses crt;

(* Here the main program block starts *)
begin
   writeln('Hello, World!');
   readkey;
end. 



This will produce following result on the terminal −

Hello, World!


Let us look various parts of the above program −

The first line of the program program HelloWorld; indicates the name of the program.

The second line of the program uses crt; is a preprocessor command, which tells the compiler to include the crt unit before going to actual compilation.

The next lines enclosed within begin and end statements are the main program block. Every block in Pascal is enclosed within a begin statement and an end statement. However, the end statement indicating the end of the main program is followed by a full stop (.) instead of semicolon (;).

The begin statement of the main program block is where the program execution begins.

The lines within (*...*) will be ignored by the compiler and it has been put to add a comment in the program.

The statement writeln('Hello, World!'); uses the writeln function available in Pascal which causes the message "Hello, World!" to be displayed on the screen.

The statement readkey; allows the display to pause until the user presses a key. It is part of the crt unit. A unit is like a library in Pascal.

The last statement end. ends your program.

Compile and Execute Pascal Program
Open a text editor and add the above-mentioned code.

Save the file as hello.pas

Open a command prompt and go to the directory, where you saved the file.

Type fpc hello.pas at command prompt and press enter to compile your code.

If there are no errors in your code, the command prompt will take you to the next line and would generate hello executable file and hello.o object file.

Now, type hello at command prompt to execute your program.

You will be able to see "Hello World" printed on the screen and program waits till you press any key.

$ fpc hello.pas
Free Pascal Compiler version 2.6.0 [2011/12/23] for x86_64
Copyright (c) 1993-2011 by Florian Klaempfl and others
Target OS: Linux for x86-64
Compiling hello.pas
Linking hello
8 lines compiled, 0.1 sec

$ ./hello
Hello, World!
Make sure that free pascal compiler fpc is in your path and that you are running it in the directory containing source file hello.pas
