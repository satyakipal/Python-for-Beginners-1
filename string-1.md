## Strings
A `character` is simply a symbol. For example, the English language has 26 characters.
A `string` is a sequence of characters.
Computers do not deal with characters, they deal with numbers (binary).
Even though you may see characters on your screen, internally it is stored and manipulated as a combination of 0's and 1's.
This conversion of character to a number is called encoding, and the reverse process is decoding. 
ASCII and Unicode are some of the popular encoding used.
In Python, string is a sequence of Unicode character.
Unicode was introduced to include every character in all languages and bring uniformity in encoding.
### How to create a string
Strings can be created by enclosing characters inside a single quote or double quotes.
Even triple quotes can be used in Python but generally used to represent multiline strings
```python
my_string = 'Hello'
print(my_string)

my_string = "Hello"
print(my_string)

my_string = '''Hello'''
print(my_string)

# triple quotes string can extend multiple lines
my_string = """Hello, welcome to
           the world of Python"""
print(my_string)
```
And the Output is:
```python
Hello
Hello
Hello
Hello, welcome to
           the world of Python

```
Python strings are "immutable" which means they cannot be changed after they are created.
We can simply reassign different strings to the same name.
```python
a = 'Geeks'
print a       # output is displayed
a[2] = 'E'
print a       # causes error

>>>Traceback (most recent call last):
   line 3, in 
    a[2] = 'E'
TypeError: 'str' object does not support item assignment

```
