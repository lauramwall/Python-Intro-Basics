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

Answer: 14 *(Using parentheses, the expression is evaluated as (2*5) first, then (10 // 3), then (16-3), and then (13+1))*


# Python Keywords
*(Cannot be used as variable names)*

| and | as | assert | break | class | continue |
| --- | --- | --- | --- | --- | --- |
| **def** | **del** | **elif** | **else** | **except** | **exec** |
| **finally** | **for** | **from** | **global** | **if** | **import** |
| **in** | **is** | **lambda** | **nonlocal** | **not** | **or** |
| **pass** | **raise** | **return** | **try** | **while** | **with** |
| **yield** | **True** | **False** | **None** |

# Vocabulary

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
