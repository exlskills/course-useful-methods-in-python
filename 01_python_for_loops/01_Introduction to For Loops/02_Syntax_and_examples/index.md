### Python For Loop Syntax
#### How to write a for loop

A couple of important reminders:
- Every **for loop** must start the same way (shown below)
- Everything inside the for loop must be indented


The basic formula for a **for loop** in python is below:


- **for** thing **in** iterable:

You replace the word thing with whatever you want to call each element in your iterable.  This is a variable that you come up with, so its name does not matter.  It is important though that you make sure you pass in the correct iterable and therefore the name for the iterable does matter.

For example if you had a list called `lst` that contained a couple of numbers, I would set up my for loop with the following:

-  **for** _number_ **in** _lst_:


### For Loop List Example
Below is an example of this in action, where we iterate through a list of numbers and print out each one:

```python
# Create the list
lst =  [1,2,3,4,5,6]

# Create the for loop
for number in lst:

  # Create print statement
  print(number)
```

### For Loop Set Example
Here is another example but instead of using a list, we are using a set

```python
# Create the set
st =  {1,2,3,4,5,6}

# Create the for loop
for number in st:

  # Create print statement
  print(number)
```

### For Loop Dictionary Items Example
Here is an example of iterating through all the items in a dictionary.  To iterate through just the keys, we would use `.keys()` and similarly, to iterate through all of the values we would use `.values()`

```python
# Create the dictionary
d =  {'a':1,'b':2,'c':3}

# Create the for loop
for item in d.items():

  # Create print statement
  print(item)
```

# For Loop with Letters in a String
Here we are going to go through all the letters in a string.  This is different than iterating though all the words in a string.  You should be able to test this out in the IDE.  The following example will be looping through words.

```python
# Create the dictionary
string = 'Hello World, How are you'

# Create the for loop
for character in string:

  # Create print statement
  print(character)
```

# For Loop with Words in a String
To iterate through a bunch of words, we need to split our string on each space.  The command to do this is `string.split(' ')` where we are using the space character to split.

```python
# Create the dictionary
string = 'Hello World, How are you'

print(string.split(' '))

# Create the for loop
for word in string.split(' '):

  # Create print statement
  print(word)
```
