### Python Dictionary with a For Loop

Using the dictionary structure with for loops is incredibly efficient in python.  In this card, I will show you some examples of ways to use dictionaries in for loops.

The first example I am going to cover is expanding a dictionary into a list of lists.  Lets imagine that you have a dictionary where the key is the product, and the value is the number of the product in stock.  Below is an example of how I want to change my data structure:

- **INPUT**

`fruits = {'banana':3,'apple':2, 'mango':1, 'kiwi':5}`

- **OUTPUT**
`fruits_list = [
    ['banana', 'banana', 'banana'],
    ['apple', 'apple'],
    ['mango'],
    ['kiwi', 'kiwi', 'kiwi', 'kiwi', 'kiwi']]`

To achieve this, we can start with writing out the steps to a solution.  

_We need to iterate all over fruits keys and build a list repeating the key `N=value` times._

I am going to do this using list comprehension.

- To iterate all over dict items you'll need `fruits.items()`
- To build a list repeating each key N times do: `[key]*N`
- As dict values indicate how many times to repeat, do: `[key]*value`


I can write this as a for loop and then convert it to list comprehension which I think is more intuitive.  Below is the code as a for loop:

```python  
# Initialize the dictionary
fruits = {'banana':3,'apple':2, 'mango':1, 'kiwi':5}

#Create blank list to append to
fruits_list = []

# Create the for loop
for fruit, quantity in fruits.items():

  # Append the list to the main list
  fruits_list.append([fruit]*quantity)


#Print out the final list
print(fruits_list)
```

Now we could do the same thing with a list comprehension. List comprehension is the act of putting a **for loop** into a list.  This may seem a little weird, but the makers of python realized that it was common enough to use a for loop to create a list that it was important to create a shortcut.  

List Comprehension is tough at first, because it feels unnatural, but the more you code in python, the more you will find the added benifits of using list comprehension.  **Just remember: Everything you do with list comprehension can be done with a for loop.  But the inverse is not true.**

### Syntax of List Comprehension

-`variable = [expression for item in list]`

You can also add a conditional statement into a list comprehension:

- ` variable = [ expression for item in list if conditional ]`

So how does this apply to the above problem?  Well, below I show how we can use this new format to assist us!

```python  
# Initialize the dictionary
fruits = {'banana':3,'apple':2, 'mango':1, 'kiwi':5}

#Create blank list to append to
fruits_list = [[fruit]*quantity for fruit, quantity in fruits.items()]

#print out the final list
print(fruits_list)
```

We will explore more list comprehension in the future, so for now just make sure you understand how we are using the `dictionary.items()` method
