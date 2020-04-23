# Python Programming for Beginners Demo 0 - Python Basics


```python
print("Hello world!")
```

## Intro

- Everyone can learn programming, it's never been easier.
- This course is for those who want to use Python, practically starting day 1
- This course is for beginners to programming.
- Many great online courses out there, free & paid
    - [Coursera](https://www.coursera.org)
    - Udemy
    - [Pluralsight](https://pluralsight.com)
    - [Learning Python the hard way](https://github.com/ubarredo/LearnPythonTheHardWay)
- Programming is creative
    - Problem solving
    - Many paths to the same place
    - You don't need to be good at math
- Automate boring, repetitive tasks
    - Moving and renaming thousands of files and sorting them into folders
    - Filling out online forms—no typing required
    - Downloading files or copying text from a website whenever it updates
    - Having your computer text you custom notifications
    - Updating or formatting Excel spreadsheets
    - Checking your email and sending out prewritten responses
- Computers are a tool, we spend so much time clicking, and typing, when we could be solving actual problems instead.
- When unsure, use a search engine, someone has probably had the same error.
- Tons of documentation online

Other helpful resources:

- [Stackoverflow](https://stackoverflow.com)
- [Github](https://github.com)
- [Reddit](https://reddit.com/r/learnprogramming/)
    
## What is programming? 

- “Do this; then do that.”
- “If this condition is true, perform this action; otherwise, do that action.”
- “Do this action exactly 27 times.”
- “Keep doing that until this condition is true.”

    
## How does it work?
- Computer code is an abstraction of the underlying hardware, a fixed set of logical operations on 32 or 64 bit values (think 0s and 1s) within the CPU. Computer code is converted to machine code, which the electronics can interface on. 
- Data is stored in the CPU, Memory (RAM), Hardisk, Network... each one being slower than the next
- Data is shuffled around from these locations, ultimately to the CPU to do some kind of processsing.. (add one, divide 2, goto this program, etc)

### Example 1 - Looking for someone in a grocery store


------------------------

```java
while (parentNotFound) {
    foreach (aisle in aisles) {
        if (parentIsInAisle) {
            walkTowardsParent();
        }
    }
}
```

------------------------


## Programming Languages

## Download Python 3.8

- Which version?
- Python 3.X is the newest version. 2.X is no longer supported.

### Windows

- Download it and install

http://python.org/
    
### MacOS

- Mac has python2 installed already, but we are targeting **Python3**

From your terminal...

------------------------

```bash
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
$ brew install python3
```

------------------------

### Ubuntu

------------------------

```bash
$ sudo apt-get install python3
```

------------------------

### What is Python?

Python is a programming language (with syntax rules for writing what is considered valid Python code) and the Python interpreter software that reads source code (written in the Python language) and performs its instructions. You can download the Python interpreter for free at https://python.org/, and there are versions for Linux, macOS, and Windows.

The name Python comes from the surreal British comedy group Monty Python, not from the snake. Python programmers are affectionately called Pythonistas, and both Monty Python and serpentine references usually pepper Python tutorials and documentation.

I encourage you to type into the interactive shell, also called the REPL (Read-Evaluate-Print Loop), which lets you run (or execute) Python instructions one at a time and instantly shows you the results. 

Using the interactive shell is great for learning what basic Python instructions do, so give it a try as you follow along. You’ll remember the things you do much better than the things you only read.


### Getting started with IDLE
Open IDLE (should be installed with Python). An interactive shell will come up. Create a new file, and name it `test.py` You can use this python file to write python programs. Run it from the menu bar, or pressing `F5`

[IDLE Documentation](https://docs.python.org/3/library/idle.html)

- While the interactive shell is good for running Python instructions one at a time, to write entire Python programs, you’ll type the instructions into the file editor. The file editor is similar to text editors such as Notepad or TextMate, but it has some features specifically for entering source code.
- The interactive shell window will always be the one with the `>>>` prompt.
- The file editor window will not have the `>>>` prompt.

### Running Python on the Command Line (Optional)

- If you want to learn Python the hard way, using the command line is best way to learn.
- The command line/terminal/shell accepts text commands, and will output some result
- For Windows this is `Powershell.exe`, for MacOS, this is `Terminal.app`, for Linux, this is `/bin/bash`

Download a text editor, like [Atom](https://atom.io)


- From your terminal (MacOS/Linux), or Command Prompt / Powershell (Windows)
- This opens up the interactive terminal which evaluates inputs

------------------------
```bash
$ python
Python 3.7.7 (default, Mar 10 2020, 15:43:33)
[Clang 11.0.0 (clang-1100.0.33.17)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
``` 
------------------------

Or run a python file

------------------------

```bash
$ python file.py
```

------------------------

[More info](https://learnpythonthehardway.org/python3/ex0.html)
   
   
### Online Interactive Python

Try Python online without downloading

https://repl.it/

## Programming Basics

### Statements, Printing, Comments

- A statement is a line of code
- Code is executed line-by-line
- Printing will output to the screen / terminal
- Comments are ignored by the program

- Python ignores comments, and you can use them to write notes or remind yourself what the code is trying to do. Any text for the rest of the line following a hash mark (#) is part of a comment.
- Sometimes, programmers will put a # in front of a line of code to temporarily remove it while testing a program. This is called commenting out code, and it can be useful when you’re trying to figure out why a program isn’t working. You can remove the # later when you are ready to put the line back in.
- Python also ignores the blank line after the comment. You can add as many blank lines to your program as you want. This can make your code easier to read, like paragraphs in a book.


```python
print('I am a statement!') # I am a line comment
# print('I am also a statement!') 
print('Player number:', 1)

'''
I am a block comment 
'''
```

### Operators and expressions

In Python, 2 + 2 is called an expression, which is the most basic kind of programming instruction in the language. Expressions consist of **values** (such as 2) and **operators** (such as `+`), and they can always **evaluate** (that is, reduce) down to a single value. That means you can use expressions anywhere in Python code that you could also use a value.

------------------------

| Operator | Operation | Example | Evaluates to |
|----------|-----------|---------|--------------|
| **       | exponent  | 2 ** 3  | 8            |
|%         | Modulus/remainder   | 22 % 8|   6 | 
| // | Integer division/floored quotient | 22 // 8 | 2
| / |Division | 22 / 8 | 2.75 |
| *  |Multiplication | 3 * 5 | 15 |
| - | Subtraction | 5 - 2 | 3 | 
| + |  Addition | 2 + 2 | 4

------------------------


- The order of operations (also called precedence) of Python math operators is similar to that of mathematics.
- use parentheses to override the usual precedence if you need to.
- Whitespace in between the operators and values doesn’t matter for Python (except for the indentation at the beginning of the line), but a single space is convention


```python
1 + 1
```


```python
2 * 6
```


```python
5 - 10
```


```python
(5 - 1) * ((7 + 1) / (3 - 1)) # PEMDAS
```


```python
23 / 7
```


```python
23 // 7
```

### Modulus

- Another way to say it is, "X divided by Y with J remaining." For example, "100 divided by 16 with 4 remaining." The result of % is the J part, or the remaining part.


```python
23 % 7
```


```python
10 ** 2
```

### Error Messages
- Programs will crash if they contain code the computer can’t understand, which will cause Python to show an error message. An error message won’t break your computer, though, so don’t be afraid to make mistakes. A crash just means the program stopped running unexpectedly.

    - Divide By Zero
    - Type Errors
    - Out of bounds
    - Out of memory
    - User defined
- Some error messages are helpful than others. It helps to use a search engine.

- You can always test to see whether an instruction works by entering it into the interactive shell. Don’t worry about breaking the computer: the worst that could happen is that Python responds with an error message. Professional software developers get error messages while writing code all the time.


```python
8 / 0
```

## The Integer, Floating-Point, and String Data Types

Remember that expressions are just values combined with operators, and they always evaluate down to a single value. A data type is a category for values, and every value belongs to exactly one data type.

| Data type | Example |
|----------|----------|
| String  | "hello", 'hi', 'a', '64 cats' |
| Integer |  -2, -1, 0, 1, 2, 3, 4, 5 |
| Float   | -1.25, -1.0, -0.5, 0.0, 0.5, 1.0, 1.25 |



```python
# strings
print('hello world')
```

- strings can be surrounded by `'` or `"`
- `''` or `""` is considered an "empty string"
- forgetting to close a string leads to an error

## String Concatenation and Replication

The meaning of an operator may change based on the data types of the values next to it. 
For example, `+` is the addition operator when it operates on two integers or floating-point values. 
However, when `+` is used on two string values, it joins the strings as the string *concatenation* operator.


```python
'alice' + 'bob'
```

- The expression evaluates down to a single, new string value that combines the text of the two strings. However, if you try to use the + operator on a string and an integer value, Python will not know how to handle this, and it will display an error message.
- The error message can only concatenate str (not "int") to str means that Python thought you were trying to concatenate an integer to the string 'Alice'. Your code will have to explicitly convert the integer to a string because Python cannot do this automatically.


```python
# Mixing data types can crash your program or cause unexpected behavior
'alice' + 2
```

- The * operator multiplies two integer or floating-point values. But when the * operator is used on one string value and one integer value, it becomes the string replication operator.


```python
'Alice' * 5
```


```python
'Alice' * 5.0
```

## Storing Values in Variables

- A **variable** is like a box in the computer’s memory where you can store a single value. If you want to use the result of an evaluated expression later in your program, you can save it inside a variable.
- You’ll store values in variables with an **assignment statement**. An assignment statement consists of a variable name, an equal sign (called the **assignment operator**), and the value to be stored. If you enter the assignment statement spam = 42, then a variable named spam will have the integer value 42 stored in it.


```python
spam = 42
spam
```


```python
x = 0
y = 1
x + y
```

- A variable is initialized (or created) the first time a value is stored in it. After that, you can use it in expressions with other variables and values. When a variable is assigned a new value, the old value is forgotten, which is why printing `full_name` again printed `"Ghostface Killa"`. This is called overwriting the variable.


```python
first_name = "Biggie"
last_name = "Smalls"
full_name = first_name + " " + last_name # string concatenation
print(full_name)
```


```python
print(full_name)
```


```python
full_name = "Ghostface Killa"
print(full_name)
```

### Variable Names

- A good variable name describes the data it contains. Currently we've been using generic names for examples
- a descriptive name will help make your code more readable

Though you can name your variables almost anything, Python does have some naming restrictions. You can name a variable anything as long as it obeys the following three rules:

- It can be only one word with no spaces.
- It can use only letters, numbers, and the underscore (_) character.
- It can’t begin with a number.

------------------------

| Valid variable names | Invalid variable names |
|----------------------|------------------------|
| current_balance | current-balance (hyphens are not allowed) |
| currentBalance  | current balance (spaces are not allowed) |
| account4 |  4account (can’t begin with a number) |
| _42 |  42 (can’t begin with a number) |
| TOTAL_SUM | TOTAL_\\$UM (special characters like $ are not allowed)| 
| hello |  'hello' (special characters like ' are not allowed) |

------------------------


- Variable names are case-sensitive, so `first_name`, `First_name`, `first_nAme` are all different variables.

## Creating your first program

- Open up IDLE, and create a new python file, or use your favorite text editor.
- Type in the program below, and save the file, `demo0.py`.

------------------------

```python
# This program says hello and asks for my name.

print('Hello, world!')
print('What is your name?')    # ask for their name

my_name = input()
print('It is good to meet you, ' + my_name)

print('The length of your name is:')
print(len(my_name))

print('What is your age?')    # ask for their age
my_age = input()
print('You will be ' + str(int(my_age) + 1) + ' in a year.')
```

------------------------

- Run your program IDLE by pressing `F5`, or clicking "Run" from the menu.

### Optional example, running from command line
- If you are running from the command line, go the same folder as your python file, then run with the `python` command. You may need to run with `python3` if you have multiple versions installed on your machine

------------------------

```bash
# find where you saved your python file..such as your Desktop
$ cd ~/Desktop
$ python demo0.py
```
------------------------

## Dissecting Your Program

### The `print()` Function

- The `print()` function displays the string value inside its parentheses on the screen.


```python
print('Hello, world!')
```

- The line `print('Hello, world!')` means “Print out the text in the string 'Hello, world!'.” 
- When Python executes this line, you say that Python is **calling** the `print()` function and the string value is being passed to the function. A value that is **passed** to a function call is an **argument**. 
- Notice that the quotes are not printed to the screen. They just mark where the string begins and ends; they are not part of the string value.

### The `input()` Function
- The `input()` function waits for the user to type some text on the keyboard and press ENTER.
- This function call evaluates to a string equal to the user’s text, and the line of code assigns the myName variable to this string value.
- You can think of the input() function call as an expression that evaluates to whatever string the user typed in. - If the user entered `'Al'`, then the expression would evaluate to `my_name = 'Al'`.
- If you call `input()` and see an error message, like NameError: name 'Al' is not defined, the problem is that you’re running the code with Python 2 instead of Python 3.


```python
my_name = input()
print('It is good to meet you ' + my_name)
```

Remember that expressions can always evaluate to a single value. If `'Al'` is the value stored in `my_name`, then this expression evaluates to `'It is good to meet you, Al'`. This single string value is then passed to `print()`, which prints it on the screen.

### The `len()` Function
You can pass the len() function a string value (or a variable containing a string), and the function evaluates to the integer value of the number of characters in that string.


```python
len("hello")
```


```python
len("The quick brown fox jumped over the lazy dog")
```


```python
len('')
```


```python
len("")
```

- Just like those examples, `len(my_name)` evaluates to an integer. It is then passed to `print()` to be displayed on the screen. 
- The `print()` function allows you to pass it either integer values or string values, but notice the error that shows up when you type the following into the interactive shell:


```python
print('I am ' + 29 + ' years old.')
```

The print() function isn’t causing that error, but rather it’s the expression you tried to pass to print(). You get the same error message if you type the expression into the interactive shell on its own.


```python
'I am ' + 29 + ' years old.'
```

- Python gives an error because the `+` operator can only be used to add two integers together or concatenate two strings. 
- You can’t add an integer to a string, because this is ungrammatical in Python. 
- You can fix this by using a string version of the integer instead, as explained in the next section.

## The `str()`, `int()`, and `float()` Functions

- If you want to concatenate an integer such as `29` with a string to pass to `print()`, you’ll need to get the value `'29'`, which is the string form of `29`. The `str()` function can be passed an integer value and will evaluate to a string value version of the integer, as follows:


```python
str(29)
```


```python
print('I am ' + str(29) + ' years old.')
```

- Because `str(29)` evaluates to `'29'`, the expression `'I am ' + str(29) + ' years old.'` evaluates to `'I am ' + '29' + ' years old.'`, which in turn evaluates to `'I am 29 years old.'`. This is the value that is passed to the `print()` function.
- The `str()`, `int()`, and `float()` functions will evaluate to the string, integer, and floating-point forms of the value you pass, respectively. 
- Try converting some values in the interactive shell with these functions and watch what happens.


```python
str(0)
```


```python
str(-3.14)
```


```python
int('42')
```


```python
int('-99')
```


```python
int(1.25)
```


```python
float(3.14)
```


```python
float(10)
```

- The previous examples call the `str()`, `int()`, and `float()` functions and pass them values of the other data types to obtain a string, integer, or floating-point form of those values.
- The `str()` function is handy when you have an integer or float that you want to concatenate to a string. 
- The `int()` function is also helpful if you have a number as a string value that you want to use in some mathematics.
- For example, the `input()` function always returns a string, even if the user enters a number. Enter `spam = input()` into the interactive shell and enter 101 when it waits for your text.


```python
spam = input()
spam
```

The value stored inside spam isn’t the integer 101 but the string '101'. If you want to do math using the value in spam, use the int() function to get the integer form of spam and then store this as the new value in spam.


```python
spam = int(spam)
spam
```

Now you should be able to treat the spam variable as an integer instead of a string.


```python
spam
```

Note that if you pass a value to int() that it cannot evaluate as an integer, Python will display an error message.


```python
int('99.99')
```


```python
int('twelve')
```

The `int()` function is also useful if you need to round a floating-point number down.


```python
int(7.7)
```


```python
int(7.7) + 1
```

### TEXT AND NUMBER EQUIVALENCE

- Although the string value of a number is considered a completely different value from the integer or floating-point version, an integer can be equal to a floating point.

- We use `==` to denote **comparison**
- Comparisons always returns a type `boolean` which can be either `True` (1) or `False` (0)


```python
42 == '42'
```


```python
42 == 42.0
```




    True




```python
42.0 == 0042.000
```




    True



## Summary

You can compute expressions with a calculator or enter string concatenations with a word processor. You can even do string replication easily by copying and pasting text. But expressions, and their component values—operators, variables, and function calls—are the basic building blocks that make programs. Once you know how to handle these elements, you will be able to instruct Python to operate on large amounts of data for you.

It is good to remember the different types of operators (+, -, *, /, //, %, and ** for math operations, and + and * for string operations) and the three data types (integers, floating-point numbers, and strings) introduced in this chapter.

I introduced a few different functions as well. The print() and input() functions handle simple text output (to the screen) and input (from the keyboard). The len() function takes a string and evaluates to an int of the number of characters in the string. The str(), int(), and float() functions will evaluate to the string, integer, or floating-point number form of the value they are passed.

In the next chapter, you’ll learn how to tell Python to make intelligent decisions about what code to run, what code to skip, and what code to repeat based on the values it has. This is known as flow control, and it allows you to write programs that make intelligent decisions.

## Questions?

## Feedback?

## Practice Questions

1. Which of the following are operators, and which are values?

-------------------

```
*
'hello'
-88.8
-
/
+
5
```
-------------------------


2. Which of the following is a variable, and which is a string?
-------------------------

```
spam
'spam'
```
-------------------------

3. Name three data types.

4. What is an expression made up of? What do all expressions do?

5. This module introduced assignment statements, like `spam = 10`. What is the difference between an expression and a statement?

6. What does the variable `bacon` contain after the following code runs?

-------------------------
```
bacon = 20
bacon + 1
```
-------------------------

7. What should the following two expressions evaluate to?

-------------------------
```
'spam' + 'spamspam'
'spam' * 3
```
-------------------------

8. Why is `eggs` a valid variable name while `100` is invalid?

9. What three functions can be used to get the integer, floating-point number, or string version of a value?

10. Why does this expression cause an error? How can you fix it?

-------------------------

```
'I ate ' + 99 + ' burritos.'
```
-------------------------

Extra credit: Search online for the Python documentation for the len() function. It will be on a web page titled “Built-in Functions.” Skim the list of other functions Python has, look up what the round() function does, and experiment with it in the interactive shell.


## Credits

https://automatetheboringstuff.com/

