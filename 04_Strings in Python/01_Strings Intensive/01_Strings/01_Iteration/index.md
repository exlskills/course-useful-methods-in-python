### Iterating through a string

One of the most useful applications in python are for loops & iterables.  

An **Iterable** refers to a structure of data that the computer can go through one at a time.  In a list, each value can be iterated through, and the same holds true for a string.  Below is an example of iterating through the string `'Hello World'`

```python
# Initialize the string
String1 = 'Hello World'

#Create the for loop
for letter in String1:

  #Print the iterable (letter in this cases)
  print(letter)
```
This prints out the following:
```python
H
e
l
l
o

W
o
r
l
d
```

**Any time that you iterate through a string, you will be iterating through each one of the characters.**

This is very useful if you want to make a letter counter.  Lets say that you want to know the count of each letter in a sting.  To do this, you would use the following:


```python
String1 = 'Hello World' # Initialize the string

Letter_counter = {} # Initialize the dictionary to count the letters

# Iterate through all the letters
for letter in String1:

  # Conditional if we haven't seen the letter before
  if letter not in Letter_counter:
    Letter_counter[letter] = 1

  # Conditional if we have already seen the letter before
  else:
    Letter_counter[letter] += 1

print(Letter_counter)
```


This gives back the following dictionary:
```
{' ': 1, 'H': 1, 'W': 1, 'd': 1, 'e': 1, 'l': 3, 'o': 2, 'r': 1}
```
