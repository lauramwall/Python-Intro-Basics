# Introduction to Python - Basics

Examples are in no specific order. [Original open source book](http://interactivepython.org/runestone/static/thinkcspy/index.html).

# 1
"Hello, World!" Test:

Input | Output
------------ | -------------
``` print("Hello, World!") ``` | Hello, World!

# 2
Detecting value and data types of objects:

```
print(type("Hello, World!"))
print(type(17))
print(type(3.2))
print(type('This is a string.') )
print(type("And so is this.") )
print(type("""and this.""") )
print(type('''and even this...''') )
```

# 3
Double quoted strings can contain single quotes inside them:

```
print('''"Oh no", she exclaimed, "Ben's bike is broken!"''')
print('This is a string.')
print("""And so is this.""")
```

# 4
Triple quoted strings can even span multiple lines:


```
print("""This message will span
several lines
of the text.""")
```

# 5
The print function can print any number of values as long as you separate them by commas:


```
print(42, 17, 56, 34, 11, 4.35, 32)
print(3.4, "hello", 45)
```

# 6
Type conversion functions:

```
print(3.14, int(3.14))
print(3.9999, int(3.9999))       # This doesn't round to the closest int
print(3.0, int(3.0))
print(-3.999, int(-3.999))        # Note that the result is closer to zero

print("2345", int("2345"))        # Parse a string to produce an int
print(17, int(17))                # int even works on integers
print(int("23bottles"))
```

```
print(float("123.45"))
print(type(float("123.45")))
```

```
print(str(17))
print(str(123.45))
print(type(str(123.45)))
```

# 7
Assigning variables:

```
message = "What's up, Doc?"
n = 17
pi = 3.14159

print(message)
print(n)
print(pi)
```

# 8
Detecting values and data types of variables:

```
message = "What's up, Doc?"
n = 17
pi = 3.14159

print(type(message))
print(type(n))
print(type(pi))
```

# 9
```len``` is a built-in Python function that returns the number of characters in a string:

```
print(1 + 1)
print(len("hello"))
```

```
y = 3.14
x = len("hello")
print(x)
print(y)
```

# 10
Operators and operands *(The asterisk (\*) is the token for multiplication, and \*\* is the token for exponentiation)*:

```
print(2 + 3)
print(2 - 3)
print(2 * 3)
print(2 ** 3)
print(3 ** 2)
```

```
quotient = 7 // 3     # This is the integer division operator
print(quotient)
remainder = 7 % 3
print(remainder)
```

# 11
Converting minutes to hours:

```
minutes = 645
hours = minutes / 60
print(hours)
```

```
print(7 / 4)
print(7 // 4)
minutes = 645
hours = minutes // 60
print(hours)
```

# 12
User input:

```
n = input("Please enter your name: ")
print("Hello", n)
```

# 13
Program to convert seconds to hours and minutes:

```
str_seconds = input("Please enter the number of seconds you wish to convert")
total_secs = int(str_seconds)

hours = total_secs // 3600
secs_still_remaining = total_secs % 3600
minutes =  secs_still_remaining // 60
secs_finally_remaining = secs_still_remaining  % 60

print("Hrs=", hours, "mins=", minutes, "secs=", secs_finally_remaining)
```

# 14
Rules of precedence (Order of operations):

```
print(2 ** 3 ** 2)     # The right-most ** operator gets done first
print((2 ** 3) ** 2)   # Use parentheses to force the order you want
```

Check your understanding:

```
16 - 2 * 5 // 3 + 1
```

Answer: 14 *(Using parentheses, the expression is evaluated as (2\*5) first, then (10 // 3), then (16-3), and then (13+1))*

Check your understanding:

```
2 ** 2 ** 3 * 3
```

Answer: 768 *(Exponentiation has precedence over multiplication, but its precedence goes from right to left! So 2 ** 3 is 8, 2 ** 8 is 256 and 256 * 3 is 768)*

# 15
Reassignment of variables:

```
bruce = 5
print(bruce)
bruce = 7
print(bruce)
```

```
a = 5
b = a    # After executing this line, a and b are now equal
print(a, b)
a = 3    # After executing this line, a and b are no longer equal
print(a, b)
```

Check your understanding (Value of x and y):

```
x = 15
y = x
x = 22
```

Answer: x is 22 and y is 15

# 16
Updating and reassigning variables:

```
x = 6        # Initialize x
print(x)
x = x + 1    # Update x
print(x)
```

Note: Before you can update a variable, you have to initialize it, usually with a simple assignment. In the above example, x was initialized to 6.

Check your understanding (What is printed in the statement?):

```
x = 12
x = x - 3
x = x + 5
x = x + 1
print(x)
```

Answer: 15 *(Starting with 12, subtract 3, than add 5, and finally add 1)*

# 17
Problem solving program to detect time:

```
current_time_str = input("What is the current time (in hours 0-23)?")
wait_time_str = input("How many hours do you want to wait")

current_time_int = int(current_time_str)
wait_time_int = int(wait_time_str)

final_time_int = current_time_int + wait_time_int

final_answer = final_time_int % 24

print("The time after waiting is: ", final_answer)
```

# Python Keywords
*(Cannot be used as variable names)*

| and | as | assert | break | class | continue |
| --- | --- | --- | --- | --- | --- |
| **def** | **del** | **elif** | **else** | **except** | **exec** |
| **finally** | **for** | **from** | **global** | **if** | **import** |
| **in** | **is** | **lambda** | **nonlocal** | **not** | **or** |
| **pass** | **raise** | **return** | **try** | **while** | **with** |
| **yield** | **True** | **False** | **None** |

# Vocabulary (Part 1)

**activecode**<br />
    A unique interpreter environment that allows Python to be executed from within a web browser.<br /><br />
**algorithm**<br />
    A general step by step process for solving a problem.<br /><br />
**bug**<br />
    An error in a program.<br /><br />
**byte code**<br />
    An intermediate language between source code and object code. Many modern languages first compile source code into byte code and then interpret the byte code with a program called a virtual machine.<br /><br />
**codelens**<br />
    An interactive environment that allows the user to control the step by step execution of a Python program.<br /><br />
**comment**<br />
    Information in a program that is meant for other programmers (or anyone reading the source code) and has no effect on the execution of the program.<br /><br />
**compile**<br />
    To translate a program written in a high-level language into a low-level language all at once, in preparation for later execution.<br /><br />
**debugging**<br />
    The process of finding and removing any of the three kinds of programming errors.<br /><br />
**exception**<br />
    Another name for a runtime error.<br /><br />
**executable**<br />
    Another name for object code that is ready to be executed.<br /><br />
**formal language**<br />
    Any one of the languages that people have designed for specific purposes, such as representing mathematical ideas or computer programs; all programming languages are formal languages.<br /><br />
**high-level language**<br />
    A programming language like Python that is designed to be easy for humans to read and write.<br /><br />
**interpret**<br />
    To execute a program in a high-level language by translating it one line at a time.<br /><br />
**low-level language**<br />
    A programming language that is designed to be easy for a computer to execute; also called machine language or assembly language.<br /><br />
**natural language**<br />
    Any one of the languages that people speak that evolved naturally.<br /><br />
**object code**<br />
    The output of the compiler after it translates the program.<br /><br />
**parse**<br />
    To examine a program and analyze the syntactic structure.<br /><br />
**portability**<br />
    A property of a program that can run on more than one kind of computer.<br /><br />
**print function**<br />
    A function used in a program or script that causes the Python interpreter to display a value on its output device.<br /><br />
**problem solving**<br />
    The process of formulating a problem, finding a solution, and expressing the solution.<br /><br />
**program**<br />
    A sequence of instructions that specifies to a computer actions and computations to be performed.<br /><br />
**programming language**<br />
    A formal notation for representing solutions.<br /><br />
**Python shell**<br />
    An interactive user interface to the Python interpreter. The user of a Python shell types commands at the prompt (>>>), and presses the return key to send these commands immediately to the interpreter for processing.<br /><br />
**runtime error**<br />
    An error that does not occur until the program has started to execute but that prevents the program from continuing.<br /><br />
**semantic error**<br />
    An error in a program that makes it do something other than what the programmer intended.<br /><br />
**semantics**<br />
    The meaning of a program.<br /><br />
**shell mode**<br />
    A style of using Python where we type expressions at the command prompt, and the results are shown immediately. Contrast with source code, and see the entry under Python shell.<br /><br />
**source code**<br />
    A program, stored in a file, in a high-level language before being compiled or interpreted.<br /><br />
**syntax**<br />
    The structure of a program.<br /><br />
**syntax error**<br />
    An error in a program that makes it impossible to parse — and therefore impossible to interpret.<br /><br />
**token**<br />
    One of the basic elements of the syntactic structure of a program, analogous to a word in a natural language. <br /><br />
    
# Vocabulary (Part 2)

**assignment statement**<br />
    A statement that assigns a value to a name (variable). To the left of the assignment operator, ```=```, is a name. To the right of the assignment token is an expression which is evaluated by the Python interpreter and then assigned to the name. The difference between the left and right hand sides of the assignment statement is often confusing to new programmers.<br /><br />
**assignment token**<br />
    ```=``` is Python’s assignment token, which should not be confused with the mathematical comparison operator using the same symbol.<br /><br />
**class**<br />
    See **data type** below.<br /><br />
**comment**<br />
    Information in a program that is meant for other programmers (or anyone reading the source code) and has no effect on the execution of the program.<br /><br />
**data type**<br />
    A set of values. The type of a value determines how it can be used in expressions. So far, the types you have seen are integers (```int```), floating-point numbers (```float```), and strings (```str```).<br /><br />
**decrement**<br />
    Decrease by 1.<br /><br />
**evaluate**<br />
    To simplify an expression by performing the operations in order to yield a single value.<br /><br />
**expression**<br />
    A combination of operators and operands (variables and values) that represents a single result value. Expressions are evaluated to give that result.<br /><br />
**float**<br />
    A Python data type which stores floating-point numbers. Floating-point numbers are stored internally in two parts: a base and an exponent. When printed in the standard format, they look like decimal numbers. Beware of rounding errors when you use ```float```s, and remember that they are only approximate values.<br /><br />
**increment**<br />
    Both as a noun and as a verb, increment means to increase by 1.<br /><br />
**initialization** (of a variable)<br />
    To initialize a variable is to give it an initial value. Since in Python variables don’t exist until they are assigned values, they are initialized when they are created. In other programming languages this is not the case, and variables can be created without being initialized, in which case they have either default or garbage values.<br /><br />
**int**<br />
    A Python data type that holds positive and negative **whole** numbers.<br /><br />
**integer division**<br />
    An operation that divides one integer by another and yields an integer. Integer division yields only the whole number of times that the numerator is divisible by the denominator and discards any remainder.<br /><br />
**keyword**<br />
    A reserved word that is used by the compiler to parse program; you cannot use keywords like ```if```, ```def```, and ```while``` as variable names.<br /><br />
**modulus operator**<br />
    Also called remainder operator or integer remainder operator. Gives the remainder after performing integer division.<br /><br />
**object**<br />
    Also known as a data object (or data value). The fundamental things that programs are designed to manipulate (or that programmers ask to do things for them).<br /><br />
**operand**<br />
    One of the values on which an operator operates.<br /><br />
**operator**<br />
    A special symbol that represents a simple computation like addition, multiplication, or string concatenation.<br /><br />
**prompt string**<br />
    Used during interactive input to provide the user with hints as to what type of value to enter.<br /><br />
**reference diagram**<br />
    A picture showing a variable with an arrow pointing to the value (object) that the variable refers to. See also state snapshot.<br /><br />
**rules of precedence**<br />
    The set of rules governing the order in which expressions involving multiple operators and operands are evaluated.
**state snapshot**<br />
    A graphical representation of a set of variables and the values to which they refer, taken at a particular instant during the program’s execution.<br /><br />
**statement**<br />
    An instruction that the Python interpreter can execute. So far we have only seen the assignment statement, but we will soon meet the ```import``` statement and the ```for``` statement.<br /><br />
**str**<br />
    A Python data type that holds a string of characters.<br /><br />
**type conversion function**<br />
    A function that can convert a data value from one type to another.<br /><br />
**value**<br />
    A number or string (or other things to be named later) that can be stored in a variable or computed in an expression.<br /><br />
**variable**<br />
    A name that refers to a value.<br /><br />
**variable name**<br />
    A name given to a variable. Variable names in Python consist of a sequence of letters (a..z, A..Z, and \_) and digits (0..9) that begins with a letter. In best programming practice, variable names should be chosen so that they describe their use in the program, making the program self documenting.<br /><br />
