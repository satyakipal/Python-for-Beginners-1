# In-built String Methods
Python has quite a few methods that string objects can call to perform frequency occurring task (related to string).
The important string methods will be discussed in this article.
## find()
The find() method returns the lowest index of the substring (if found). If not found, it returns -1.
### Syntax:
#### str.find(sub[, start[, end]] )
The find() method takes maximum of three parameters:
* sub - It's the substring to be searched in the str string.
* start and end (optional) - substring is searched within str[start:end]

```python
quote = 'Let it be, let it be, let it be'

result = quote.find('let it')
print("Substring 'let it':", result)

result = quote.find('small')
print("Substring 'small ':", result)

# How to use find()
if  (quote.find('be,') != -1):
  print("Contains substring 'be,'")
else:
  print("Doesn't contain substring")
 
quote = 'Do small things with great love'

# Substring is searched in 'hings with great love'
print(quote.find('small things', 10))

# Substring is searched in ' small things with great love' 
print(quote.find('small things', 2))

# Substring is searched in 'hings with great lov'
print(quote.find('o small ', 10, -1))

# Substring is searched in 'll things with'
print(quote.find('things ', 6, 20))
  ```
  ### Output
```python
>>>Substring 'let it': 11
Substring 'small ': -1
Contains substring 'be,'
-1
3
-1
9

```
[Try it online....](http://tpcg.io/0PFGSo)


## startswith()
The startswith() method returns True if a string starts with the specified prefix(string). If not, it returns False.
### Syntax:
#### str.startswith(prefix[, start[, end]])
The startswith() method takes maximum of three parameters:
* prefix - String or tuple of strings to be checked
* start (optional) - Beginning position where prefix is to be checked within the string.
* end (optional) - Ending position where prefix is to be checked within the string.

```python
text = "Python programming is easy."

# start parameter: 7
# 'programming is easy.' string is searched
result = text.startswith('programming is', 7)
print(result)

# start: 7, end: 18
# 'programming' string is searched
result = text.startswith('programming is', 7, 18)
print(result)

result = text.startswith('program', 7, 18)
print(result)
  ```
  ### Output
```python
>>>True
False
True

```
[Try it online....](http://tpcg.io/0PFGSo)
### endswith(“string”, beg, end) :-
The purpose of this function is to return true if the function ends with mentioned string(suffix) else return false.


## islower()
The islower() method returns True if all alphabets in a string are lowercase alphabets. If the string contains at least one uppercase alphabet, it returns False.
### Syntax:
#### string.islower()
The islower() method returns:
* True if all alphabets that exist in the string are lowercase alphabets.
* False if the string contains at least one uppercase alphabet.

```python
s = 'this is good'
print(s.islower())

s = 'th!s is a1so g00d'
print(s.islower())

s = 'this is Not good'
print(s.isupper())

  ```
  ### Output
```python
>>>True
True
False

```
[Try it online....](http://tpcg.io/0PFGSo)
### isupper(“string”) :-
This function returns true if all the letters in the string are upper cased, otherwise false.


## lower(),upper(),swapcase(),title() 
* lower() :- This function returns the new string with all the letters converted into its lower case.

* upper() :- This function returns the new string with all the letters converted into its upper case.
 
* swapcase() :- This function is used to swap the cases of string i.e upper case is converted to lower case and vice versa.

* title() :- This function converts the string to its title case i.e the first letter of every word of string is upper cased and else all are lower cased.



```python
str = "Man and WOmen ARE all EqUal"
 
# Coverting string into its lower case
str1 = str.lower();
print (" The lower case converted string is : " + str1)
 
# Coverting string into its upper case
str2 = str.upper();
print (" The upper case converted string is : " + str2)
 
# Coverting string into its swapped case
str3 = str.swapcase();
print (" The swap case converted string is : " + str3)
 
# Coverting string into its title case
str4 = str.title();
print (" The title case converted string is : " + str4)
  ```
  ### Output
```python
>>>TThe lower case converted string is : man and women are all equal
 The upper case converted string is : MAN AND WOMEN ARE ALL EQUAL
 The swap case converted string is : mAN AND woMEN are ALL eQuAL
 The title case converted string is : Man And Women Are All Equal

```
[Try it online....](http://tpcg.io/0PFGSo)





  
