## Variable Types
Variables are nothing but reserved memory locations to store values.
This means that when you create a variable you reserve some space in memory.
Based on the data type of a variable, the `interpreter` allocates memory and decides what can be stored in the reserved memory. 
Therefore, by assigning different data types to variables, you can store `integers`, `decimals` or `characters` in these variables.
#### Assigning Values to Variables
Python variables do not need explicit declaration to reserve memory space.
The declaration happens automatically when you assign a value to a variable. 
The equal sign `(=)` is used to assign values to variables.
The operand to the left of the = operator is the name of the variable and the operand to the right of the = operator is the value 
stored in the variable.

```python
counter = 100          # An integer assignment
miles   = 1000.0       # A floating point
name    = "John"       # A string

```
Here, 100, 1000.0 and "John" are the values assigned to counter, miles, and name variables, respectively.[Try it Online..](http://tpcg.io/WKTCEy
)
#### Multiple Assignment
Python allows you to assign a single value to several variables simultaneously. 

```python
a = b = c = 1
x , y , z = 10 , 20 , 30
```
First Line:  An integer object is created with the value 1, and all three variables are assigned to the same memory location.
Second Line: We have assigned multiple objects to multiple variables.[Try it Online..](http://tpcg.io/WKTCEy)
#### Standard Data Types
 Python has various standard data types that are used to define the operations possible on them and the storage method for each of them.

Python has five standard data types −

* Numbers
* [String]()
* [List]()
* [Tuple]()
* [Dictionary]()

#### Python Numbers
Number data types store numeric values. Number objects are created when you assign a value to them. For example −
```python
var1 = 1
var2 = 10
```
You can also delete the reference to a number object by using the `del` statement. 
```python
del var
del var_a, var_b
```
[Try it Online..](http://tpcg.io/WKTCEy)

Python supports four different numerical types −

* int (signed integers)
* long (long integers, they can also be represented in octal and hexadecimal)
* float (floating point real values)
*complex (complex numbers)

[Continue to Strings....]()
