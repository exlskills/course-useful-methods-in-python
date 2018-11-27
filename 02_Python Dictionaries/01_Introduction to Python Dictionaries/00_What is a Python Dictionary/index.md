### Python Dictionaries
#### What is a Python Dictionary?

A dictionary in python at the beginning seems like a weird concept. Even so, they are terribly useful and make a lot of sense after you have been using them for a while.  

If you have experience with JSON, you will immediately recognize the format of a dictionary.  But in case you haven't, **dictionaries are made of two elements: a key and a value**

#### Dictionaries, in Python, are also known as "mappings", because they "map" or "associate" key objects to value objects.


Below is an example of how you would define a dictionary:

- `d = {'key':'value'}`

A dictionary **key** must be either a string or an integer

A dictionary **value** can be a string, integer, float, list, set, tuple, or even another dictionary.  

Here are some built in operations for dictionaries.  The below examples assume a dictionary called `d`

- `len(d)`: returns the number of stored entries, i.e. the number of (key,value) pairs.
- `del d[key] `: deletes the key k together with his value
- `key  in d`: True, if a key k exists in the dictionary d
- `key not in d` True, if a key k doesn't exist in the dictionary d

In the following cars, we will look at some common uses, if it possible to sort, and how to update your python dictionary. 
