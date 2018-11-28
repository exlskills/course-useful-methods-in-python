# Reading a file

When reading a file in python, you use a specific syntax.  The syntax is as follows:

Start the line `with open()` where the `with` is telling the compiler to use the open command.  After this, you need to provide the open with the argument of the file directory.

In the case of the google colab notebook, we are going to pass it a file that already exists and has the filepath: `'sample_data/california_housing_test.csv'`  

Now your line of code should look like: `with open('sample_data/california_housing_test.csv')`

We need to name the file that we are using and in general, I use the letter f, but this is arbitrary

`with open('sample_data/california_housing_test.csv') as f`

And finally, you need a colon.

```python
with open('sample_data/california_housing_test.csv') as f:
  ```
Now that we have the file as opened, f is an **iterable** and we can read each line in the file. Try printing out each line of the file using the code provided in the notebook.  (Shift + enter runs a code cell).

You may notice that the first line is the the headers and the following lines are data.  We may want to save the first line as a headers object.  To do this, we will iterate through the first line then stop, and save that line to a data object called headers.

You will see in **Section 1.1** the code in the cell below it does just that.


------




Now, we want to iterate through the remaining lines and add each one to a data matrix that we are creating.  To do this, we will use the same method as above to iterate (`for line in f`) and since we already read the first line, we no longer need to worry about that one.  As well, we will want to split each line at every comma & we learned about this in the intro to strings course.

You will see the additional code in **Section 1.2**


------



Data is now a large list of lists that we can use later on.  

Finally, there is a library called **Pandas** which we will use to make this into a nice table.  Pandas has a ton of uses, more than I can go into with this tutorial, so for now we will just use it and later on (in a another unit) I will explain it in more depth.

- When using files, it is common practice to always close the file, so you will see that I did this as well.

You will the see the final product in **Section 1.3**

You will notice that there are certain problems with our data, be we can manipulate it further later on.
