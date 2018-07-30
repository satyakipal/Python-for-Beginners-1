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
a = 'Satyaki'
print a       # output is displayed
a[2] = 'E'
print a       # causes error

>>>Traceback (most recent call last):
   line 3, in 
    a[2] = 'E'
TypeError: 'str' object does not support item assignment

```
### Accessing characters in a string
We can access individual characters using indexing and a range of characters using slicing. Index starts from 0. 
Characters in a string can be accessed using the standard [ ] syntax
```python
s = 'hi'
print s[1]   
```
This will print "i"

Python allows negative indexing for its sequences.
The index of -1 refers to the last item, -2 to the second last item and so on.
We can access a range of items in a string by using the slicing operator (colon).
```python
str = 'satyakipal'
print('str = ', str)

#first character
print('str[0] = ', str[0])

#last character
print('str[-1] = ', str[-1])

#slicing 2nd to 5th character
print('str[1:5] = ', str[1:5])

#slicing 6th to 2nd last character
print('str[5:-2] = ', str[5:-2])
```
This will give the following output
```python
>>>str =  satyakipal
str[0] =  s
str[-1] =  l
str[1:5] =  atya
str[5:-2] =  kip
```

### String Sclicing
The "slice" syntax is a handy way to refer to sub-parts of sequences -- typically strings and lists. The slice s[start:end] is the elements beginning at start and extending up to` but not including end`. 

Suppose we have s = "Hello"



