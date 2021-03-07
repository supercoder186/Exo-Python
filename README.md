# Exo-Python
The is a programming language designed to be simple and fast, written in python

<a name="Installation"></a>
## Installation
This project was built on Python 3

It does not have any dependencies. You can simply clone the repository

<a name="Usage"></a>
## Usage
### Running the Exo code

Exo.py is the program that will run the code. Run the command 
```shell
python exo path/to/file.exo
```


<a name="LanguageSpecification"></a>
## Language Specification

Note: Comments start with a #, similar to python. There are no multiline comments

<a name="types"></a>
### Data Types

There are four data types that the user can use: integer, float, string and function. In general, the following is true for operations:

- an Int and an Int will result in an Int
- a Float and a Float results in a Float
- a Float and an Int will result in a Float
- any number type and a String will result in a string

<a name="literals"></a>
### Literals

Literals are values like ```5, "hello", 6.6```. A number is considered a float if it has a decimal point; otherwise it is taken as an int. String literals are surrounded in quotation marks.

<a name="variables"></a>
### Variables

Variables are dynamically typed (data types can be changed). There is type inference, but you can explicitly state the type of the variable if you want the type to be explicit

```
var x = 5 + 3.0 # 5 + 3.0 = 8.0 so x is a float
string y = "Hello" + " World" # y is now a string
var y = "Hi" # y is now 'Hi'
int y = 1 # This will throw an error
var y = 1 # This will also throw an error
```

```
var x = 5
var x = 3
```

The syntax for initialization and assignment is identical.

```
var a = 6.0
var a = a + 1
```

<a name="if"></a>
### If Statements

If statements follow the following format:

```
if (condition){
  statements  #indents are optional
} elif (condition){
  statements
} else{
  statements
}
```

The elif clause is optional or can also be used as many times as necessary in a single if statement.

if statements can be nested. The else statement is also optional and can be ommited entirely:

```
if (condition){
  statements
} 
```

There is no boolean type in the language. Therefore the condition can also be an integer. If its value is 0, it will qualify as false, otherwise as true

```
x > 3
x + 1 < 40/x
5
```

<a name="while"></a>
### While Loops

A while loop can be represented like so:

```
while (condition){
   statements
}
```

While statements can also be nested inside one another and combined with If statements flexibly.

<a name="lists"></a>
### Lists

#### List usage

```
var x = [1, 2, 3]
var y = [4, 5, 6]
```

#### List Elements

List elements can be accessed through the square bracket notation:

```
var y = x[1] + 6  # x[1] gives the 2nd element of the list x
```

They can be assigned to just like variables, and there are no type checks on the element added to the array:

```
var x[10] = 345 + 3
```

<a name="print"></a>
### Print

The print statement prints whatever it is given to the screen.

```print("Hello World")```

It can be given variables, expressions, and array indices.

```
print(5 + (4.0 * 3))
print(x + y[1])
print("Hello" + " " + "World")
```

<a name="input"></a>
### Input

The input statement takes user input. There are 2 types: input, and input_int

```
var x = input() #This will be stored as a string value
var y = input_int() #This will be stored as an int value
```

It can only take String and Int inputs.

<a name="functions"></a>
### Functions

Functions are defined like so:

```
fun name(type arg1, type arg2){
  statements
  (return statement)
}
```

Arguments require types, but they are not type-checked

```
fun double(int a){
  int b = a * 2
  return b
}

fun triple(int a){
  return a * 3
}

fun concat_print(string a1, string a2){
  var a3 = a1 + " " + a2
  print(a3)
}
```
If there is no return statement, the function will return 0

This is the syntax to call a function:

```
var z = function(arg, arg2, ...)
```

The function call can be used just like a normal variable. For example:

```
var z = list1[add(x,y) - 2]
