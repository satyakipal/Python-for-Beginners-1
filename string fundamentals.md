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
str = "satyakipal"
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



* s[1:4] is 'ell' -- chars starting at index 1 and extending up to but not including index 4
* s[1:] is 'ello' -- omitting either index defaults to the start or end of the string
* s[:] is 'Hello' -- omitting both always gives us a copy of the whole thing (this is the pythonic way to copy a sequence like a string or list)
* s[1:100] is 'ello' -- an index that is too big is truncated down to the string length

The standard zero-based index numbers give easy access to chars near the start of the string. As an alternative, Python uses negative numbers to give easy access to the chars at the end of the string: s[-1] is the last char 'o', s[-2] is 'l' the next-to-last char, and so on. Negative index numbers count back from the end of the string:

* s[-1] is 'o' -- last char (1st from the end)
* s[-4] is 'e' -- 4th from the end
* s[:-3] is 'He' -- going up to but not including the last 3 chars.
* s[-3:] is 'llo' -- starting with the 3rd char from the end and extending to the end of the string.

It is a neat truism of slices that for any index n, s[:n] + s[n:] == s. This works even for n negative or out of bounds. Or put another way s[:n] and s[n:] always partition the string into two string parts, conserving all the characters. As we'll see in the list section later, slices work with lists too.

### How to print single quote or double quote on screen?
We can do that in the following two ways:

* First one is to use escape character to display the additional quote.
* The second way is by using mix quote, i.e., when we want to print single quote then using double quotes as delimiters and vice-versa.
Example-

print "Hi Mr Goose."
```python 
# use of escape sequence
print ("He said, \"Welcome to Goossy World\"" )   
 
print ("'Hey so happy to be here'")
 
# use of mix quotes
print ('Getting Goosy, "Loving it"')               
```
Output:
```python
>>>Hi Mr Goose.
He said, "Welcome to Goossy World"
Hey so happy to be here
Getting Goosy, "Loving it"
```




