# Python Programming for Begginers Demo 0


```python
print("Hello world!")
```

    Hello world!


## Intro

- Everyone can learn programming, it's never been easier.
- This course is for those who want to use Python, practically starting day 1
- This course is for begginers to programming.
- Programming is creative
    - Problem solving
    - Many paths to the same place
- Automate boring, repetitive tasks
    - file naming
    - spread sheets
    - emails
    - online form
- Use a search engine, someone has probably had the same error
    - Stackoverflow
    - Github
    
## What is a program? 
    - Set(s) of instructions. Do this then do this. If this happens, then this. 
    - A program is made up of many algorithms
    - Software is often made up of many different programs
    - The lines between these can be blurry
    
## How does it work?
    - Computer code is an abstraction of the underlying hardware, a fixed set of logical operations on 32 or 64 bit values (think 0s and 1s) within the CPU. Computer code is converted to machine code, which the electronics can interface on. 
    - Data is stored in the CPU, Memory (RAM), Hardisk, Network... each one being slower than the next
    - Data is shuffled around from these locations, ultimately to the CPU to do some kind of processsing.. (add one, divide 2, goto this program, etc)

   
###  Example 1 - Driving to the mall from home
1. Get money & car keys
2. Leave house
3. Unlock the car
4. Open the car door
5. Get in the driver's side seat of the car
6. Put the keys in the ignition
7. Turn the ignition
8. Step your right foot on the brake
9. While foot is on brake, shift transmission
10. Accidentally reverse into the garage


### Example 2 - Looking for someone in a grocery store

- psudeocode

```java
while (parentNotFound) {
    foreach (aisle in aisles) {
        if (parentIsInAisle) {
            walkTowardsParent();
        }
    }
}
```

### Example 3

#### Example 3.1 (Standard Equations)

$$ g = \sum_{i=0}^{i=20}i*2$$


#### Example 3.2 (Java)

```java
int g = 0;
for (int i = 0; i <= 20; i++) {
    g += i * 2;
}
```

#### Example 3.3 (Python)
    
```python
g = 0;
for i in range(0, 21):
    g += 1 * 2

```

## Programming Languages

## Download Python 3.8

- Which version?
- Python 3.X is the newest version. 2.X is no longer supported.

### Windows

- Download it and install

http://python.org/
    
### MacOS

- Mac has python2 installed already

From your terminal...

```bash
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
$ brew install python3
```

### Ubuntu

```bash
$ sudo apt-get install python3
```

### Why Python?
- Easy to read
- "Batteries included"
- Dynamic typing
- The fastest growing programming language

## Running Python

- From your terminal (MacOS/Linux), or Command Prompt / Powershell (Windows)
- This opens up the interactive terminal which evaluates inputs

```bash
$ python
>>> 
``` 

Or run a python file

```bash
$ python file.py
```

### Programming environments
- IDLE (installed with Python)
- Text editors
- Professional Integrated Development Environments (IDES), can be helpful (code-completion, one-click run, warnings and errors)
   - PyCharm 
   - some obsure some important lessons about how code actually runs (terminals & environments)
   - compute & ram intensive
   
### Online Interactive Python

Try Python online without downloading

https://repl.it/

## Programming Basics

### Statements, Printing, Comments

- A statement is a line of code
- Code is executed line-by-line
- Printing will output to the screen / terminal
- Comments are ignored by the program


```python
print("I am a statement!")
print('I am also a statement!') # I am a line comment
print("Player number:", 1)

'''
I am a block comment 
'''
```

    I am a statement!
    I am also a statement!
    Player number: 1





    '\nI am a block comment \n'



### Math Expressions & Evaulation

- Like, math expressions.


```python
1 + 1
```




    2




```python
2 * 6
```




    12




```python
5 - 10
```




    -5




```python
(10 / 5) + (2.5 * 2) # PEMDAS
```




    7.0




```python
10 ** 2
```




    100



### Error Messages
- In certain conditions, your program can crash and will print an error message
    - Divide By Zero
    - Type Errors
    - Out of bounds
    - Out of memory
    - User defined
- Some error messages are helpful than others. It helps to use a search engine.


```python
8 / 0
```


    ---------------------------------------------------------------------------

    ZeroDivisionError                         Traceback (most recent call last)

    <ipython-input-9-340e47a3b5ce> in <module>
    ----> 1 8 / 0
    

    ZeroDivisionError: division by zero



```python
1 == 1
```




    True




```python
1 == 0
```




    False




```python
"Joe" == "Joe"
```

## Variables

- Assign variables to values or expressions
- variable name must start with a character from a-z or A-Z (may not be a number, special character)
- do not use special keywords (True, False, with, type, print, List, Dict, import, is, not)


```python
x = 0
y = 1
x + y
```




    1




```python
first_name = "Biggie"
last_name = "Smalls"
full_name = first_name + " " + last_name # string concatenation
print(full_name)

full_name = "Ghostface Killa"
print(full_name)
```

    Biggie Smalls
    Ghostface Killa


## Basic Data Types

### String  `"string"`, `'string'`
- Integer  `1`, `2`, `3`
- Float    `5.4`,
- Boolean  `True`,`False`
- List     `[1,2,3,4]`, `["amy", "sarah", "lily"]`
- Dictionary `{apple: 1, pear: 2, lime: 7}`
- None


```python
# strings
print(type("hello world"))
address:str = "102 49th street"
print(type(address))

```

    <class 'str'>
    <class 'str'>
    <class 'int'>



```python
# integers
print(type(10))
```


```python
# Float
print(type(5.0))
print(5.0 + 4.5)
print(0.001 / 2)
print(1 + 1.0)
```

    <class 'float'>
    9.5
    0.0005
    2.0



```python
# booleans
isAsleep = True

if isAsleep:
    print("zzzz")
```

    zzzz



```python
# lists

emotions = ["fear", "happiness", "anger", "envy", "sadness"]

print(emotions[1]) # indexing 1-th element
print(len(emotions))
```

    happiness
    5



```python
# dictionary

values = {"penny": 0.01, "nickle": "0.05", "dime": "0.10", "quarter": 0.25, "dollar": "1.00"}
print(values)
print(values["dime"])
```

    {'penny': 0.01, 'nickle': '0.05', 'dime': '0.10', 'quarter': 0.25, 'dollar': '1.00'}
    0.10



```python
# Mixing data types can crash your program or cause unexpected behavior
1 + "2"
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-6-db092cb74d2d> in <module>
    ----> 1 1 + "2"
    

    TypeError: unsupported operand type(s) for +: 'int' and 'str'


### Type Casting
- Types can often be converted to other types in Python


```python
number = 1
print(number)
string = str(number) + " 2"
print(string)
```

    1
    1 2



```python
int("5") + 5
```




    10




```python
str(["list"])
```




    "['test']"



## Conditionals

- Running different blocks of code based on boolean values


```python
if (20 > 10):
    print("foo")
else:
    print("bar")
```

    foo



```python
if True:
    print("hello")
if not False:
    print("world")
```


```python
if True or False:
    print("foobar")
else:
    print("barfoo")
```

    foobar



```python
if 10 / 5 == 2:
    print("fizz")
```


```python
x = True
y = False
if not x:
    print(x)
elif y is False:
    print(y)
else:
    print("1")
```


```python
# This is the same as above
x = True
y = False
if !x:
    print(x)
elif y == False:
    print(y)
else:
    print("1")
```

## Functions

- functions take 0-n inputs and return an output
- If you don't return anything, Python will return `None`


```python
def add(a,b):
    return a + b

a = 5
b = 10
c = add(a,b)
print(c)
```

### Built in functions


```python
len("cowboy")
```




    6




```python
len(["1", "2", "3"])
```




    3




```python
type((1,2))
```




    tuple




```python
max(5,6)
```




    6




```python
abs(-10)
```




    10



## User input

- input()


```python
input_string = input("input the number of avocados you wish to buy")
cost_avocado = 2.49
input_number = int(input_string)

if input_number <= 0:
    print("Invalid number")
else:
    print("Please pay $", cost_avocado * input_number)
```

    input the number of avocados you wish to buy20
    Please pay $ 49.800000000000004


## Questions?

## Feedback

1. What was done well?
2. What could have been done better?
3. Would you attend another session? (Y/N)

Email me, or submit feedback at https://nlouie.com/courses

## Feedback

1. What was done well?
2. What could have been done better?
3. Would you attend another session? (Y/N)

Email me, or submit feedback at https://nlouie.com/courses

## Feedback

1. What was done well?
2. What could have been done better?
3. Would you attend another session? (Y/N)

Email me, or submit feedback at https://nlouie.com/courses
