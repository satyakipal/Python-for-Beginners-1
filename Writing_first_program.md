### Python Promt
The `>>>` means that Python is ready and we can enter any command. The
workflow is really simple:

we enter a command --> press Enter--> Python displays the result. enter
another command -->press Enter-->Python displays another result and keep going.
### Knowing Your Friends
When you are visiting the IDE , you have no idea of how to do it. Probably you will start interacting python with a "Hello".Let's see what happens
if we just write something and press Enter.

```python
>>> Hello
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'Hello' is not defined
>>>
```
`error messages` are our friends.
This error message tells us what's wrong and where, and we'll learn what "name 'Hello' is not defined" meansin our upcomming articles.

That didn't worked. How about numbers?

```python
>>> 1234
1234
>>> -1234
-1234

```

Here we Go : ) .. Our first Python statement without an error.. 

### The Anchors

In any programming languages, a `comment` is a programmer-readable explanation or annotation in the source code(Lines we write in IDE ) of a  program.
They are added with the purpose of making the source code easier for humans to understand, and are generally ignored by compilers and interpreters.

##### How do we call this friend
They can be created by typing a
`#` and then some text after it, and they are useful when our code would be hard to understand without them.
```python
>>> 1234 # I am printing 1234
1234
>>> -1234 # I am printing -1234
-1234

```

### print()
One built-in function that we will use most often is ` print() `.
The print() function prints the specified message to the screen, or other standard output device.
The message can be a string, or any other object, the object will be converted into a string before written to the screen.

Let us study some examples to understand it better.
```python
>>> print("Python is Fun")
Python is Fun
>>> print(3+9)
12

```
## Our First Program:
Program to print `Hello World` to tthe Screen.

```python
>>> print("Hello World")
Hello World
```



Go to next Chapter- [Working with Inputs](https://github.com/satyakipal/Python-for-Beginners-1/blob/master/Working%20with%20Inputs.md)



