### Lists

Now, we have been able to iterate through a string, but so far we have only had the ability to go through each letter.  Lets say for example that you are trying to iterate through each word in a string, rather than each letter.  Using python this is simple using the `string.split(' ')` method!

To begin, we can split a string apart based on any character we want.  This means we can split of spaces (`' '`) or commas (`','`) or any other character that we are using.

When you use the `.split()` method, it will return a list:

```Python
string = 'Hello World! We are learning about strings in Python'
string_list = string.split(' ')
```

This returns:
```python
['Hello','World!','We','are','learning','about','strings','in','Python']
```

Now we can iterate through each word in the list!  This means that we could count the number of words rather than letters in a document.


```python
string = 'Hello World! We are learning about strings in Python'

# Create a list of our words
string_list = string.split(' ')

# Initialize the dictionary to count the letters
word_counter = {}

# Iterate through all the letters
for word in string_list:

  # Conditional if we haven't seen the letter before
  if word not in word_counter:
    word_counter[word] = 1

  # Conditional if we have already seen the letter before
  else:
    word_counter[word] += 1

print(word_counter)
```

This prints out:
```python
{'Hello': 1, 'World!': 1, 'We': 1, 'are': 1, 'learning': 1, 'about': 1, 'strings': 1, 'in': 1, 'Python': 1}
```

And now you know how to build a word counter in python!
