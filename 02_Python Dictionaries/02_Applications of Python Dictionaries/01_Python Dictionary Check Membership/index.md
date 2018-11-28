### How to Check Membership in Python

This card is going to be a little shorter, but the content is highly valuable.  

In many cases you may want to know if your python dictionary contains a certain element, and based on if it contains the element change your action.  

For example, assume I have a dictionary like the one in the last card:

- `fruits = {'banana':3,'apple':2, 'mango':1, 'kiwi':5}`

And you could imagine that I want to check to see if the fruit 'strawberry' is in the dictionary.  If it is, I want to assign it a add 2 to the current supply and if not, I want to initialize with a supply of 2.  

The first part of this is checking to see if the dictionary contains 'Strawberry'.  

We will do this using the following syntax:

- `'strawberry' in fruits`

This will return true or false, so we can create a conditional statement.  Below is the implementation of this in python.


```python
#Initialize the Dictionary
fruits = {'banana':3,'apple':2, 'mango':1, 'kiwi':5}

# Conditional statement
if 'stawberry' in fruits:
  fruits['strawberry'] += 2
else:
  fruits['strawberry'] = 2

# Add a print statement
print(fruit)

```
