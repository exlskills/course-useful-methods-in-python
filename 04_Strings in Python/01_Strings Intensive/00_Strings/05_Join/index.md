### Join

Finally, we are going to take a look at how we can take a list of strings and joining them together in a single string.  To start, here is the list that we will try to put back together with a space in between each word:

`['Hello','world,','lets','take','this','list','and','make','it','into','a','string']`

To join this, we will use the `.join()` method with a space.

```python
word_list = ['Hello','world,','lets','take','this',
              'list','and','make','it','into','a','string']

#Join with a space
string = ' '.join(word_list)

print(string)
```

This command goes through each word in the list and concatenates them together using a space.  This code section prints:

`"Hello world, lets take this list and make it into a string"`


As well, we could join the words using any character (or no characters).  For example, to join every word with a hyphen in between them the following code would be used:


```python
word_list = ['Hello','world,','lets','take','this',
              'list','and','make','it','into','a','string']
#Join with a hyphen
string = '-'.join(word_list)

print(string)
```

This gives us the string `"Hello-world,-lets-take-this-list-and-make-it-into-a-string"`

And finally to join with no character:

```python
word_list = ['Hello','world,','lets','take','this',
              'list','and','make','it','into','a','string']
#Join with no character
string = ''.join(word_list)

print(string)
```

Which gives us: `"Helloworld,letstakethislistandmakeitintoastring"`
