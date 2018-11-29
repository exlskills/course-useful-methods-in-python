### Common Uses for Python Dictionaries

##### Review
They are Python’s built-in mapping type. They map keys, which can be any immutable type, to values, which can be any type (heterogeneous), just like the elements of a list or tuple. In other languages, they are called associative arrays since they associate a key with a value.

### Example Dictionary to Translate

As an example, lets create a dictionary to translate English words into Spanish.  Since we will be dealing with word, the keys will be strings in this case.

One way to create a dictionary is to start with the empty dictionary and add `key:value` pairs. As seen in the previous card, the empty dictionary is denoted {}.  Below, I will begin to create the dictionary that we can use for translation.

```python
# Initialize the dictionary
englist2spanish = {}

# Add the values for 1 & 2
englist2spanish["one"] = "uno"
englist2spanish["two"] = "dos"

#Print out the result
print(englist2spanish)

```


### Example Python Dictionary to look up specific Rainfall for a year


We could think of a situation where we want to look up the rainfall by a specific year.  In this case, a python dictionary would be a great resource as we can use the year for the key and the percentage of rainfall as the value.  Below is an example of this in action!

```python
# Create the dictionary
rain_percent = { 1980: '17%', 1981: '15%', 1982: '10%'}

# Print out the whole thing
print(rain_percent)

# Look up based on specific year
print(rain_percent[1980])

# Output:
# {1980: '17%', 1981: '15%', 1982: '10%'}
# 17%
````

In the next card we will look at some what python dictionaries **cannot achieve** but also we will look at some of the other powerful methods that can be sued with python dictionaries.
