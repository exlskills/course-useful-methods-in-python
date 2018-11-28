### Reversed & Sorted

Here I am going to introduce two new functions in python that are incredibly useful.  

#### Reversed

Reversed takes a list and puts it into the opposite order.  For example, if we have the string `Hello World, lets learn how to reverse a list` and we convert the string into a list that looks like:`['Hello', 'World,', 'lets', 'learn', 'how', 'to', 'reverse', 'a', 'list']`.

Now lets say that we want to reverse this list, below is the python code to reverse the list:

```python
#  Define our string
string = "Hello World, lets learn how to reverse a list"

# Split on spaces
string = string.split(' ')

# Reverse the string
reversed_string = list(reversed(string))

print(reversed_string)
```

This code prints out our list backwards: `['list', 'a', 'reverse', 'to', 'how', 'learn', 'lets', 'World,', 'Hello']`


The function **`reversed()`** also works on lists with numbers in it.


#### Sorted

We also have a function called sorted.  This seems very arbitrary for strings, but when working with numbers it can be incredibly useful.

```python
#Create the list
lst = [1,32,4,18,12,55,12,19]

#Sort the list
lst = list(sorted(lst))

# print out the sorted list
print(lst)
```
This gives us back the sorted list: `[1, 4, 12, 12, 18, 19, 32, 55]`
