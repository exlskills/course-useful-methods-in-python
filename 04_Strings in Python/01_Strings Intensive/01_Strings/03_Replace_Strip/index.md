### Replace and Strip

A very useful method is called `replace('char_to_replace','replacement')`.  We use this to get rid of punctuation or any characters that we do not want in our string.  For examples, consider the sentence with bad punctuation:

- `'Hello. World! Lets, get rid of some bad punctuation!'`

Here we want to get rid of the period after hello and the comma after lets.  To do this, we will use the `replace` method as is shown below.

```python
string = 'Hello. World! Lets, get rid of some bad punctuation!'

# Replace the comma
string_1 = string.replace(',','')

# Replace the period
string_2 = string_1.replace('.','')
print(string_2)
```
This gives back `Hello World! Lets get rid of some bad punctuation!`


 ----

Another useful method that we can use with strings is called `.strip()`. This will remove specific characters from **the end of a string** string that we do not want.  For example, if you are trying to count the occurrences of words in a string, you want to ignore all the periods and exclamation marks.  To do this we use the strip method:

```python
string = 'Hello World! Lets remove the exclamation mark!'

# Replace any exclamation mark or period at the end of the string
string_1 = string.strip('.!')  

print(string_1)
```
This gives back `Hello World! Lets remove the exclamation mark`.  You will notice that the string still has an exclamation mark after the _Hello World_ because the strip method only gets rid of characters at the end of a string.  


Both of these methods tend to be very useful for removing html tags from text
