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


  
