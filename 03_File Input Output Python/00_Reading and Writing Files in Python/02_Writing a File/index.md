# Writing a file

Once again we are going to be using a google colab notebook to work on file IO (input, output).

To review what we covered in the last lecture:
1. We now know the syntax to open a file
2. Since files are iterables, we can go through files using a for loop
3. We can also read files line by line using the methon `.readline()`
4. We must close the file after we are done using it

### Onto writing files!

The link to the notebook that is going to be used for this lecture is [here](https://colab.research.google.com/drive/1XNbXwX8Waq-TWuUoW7MB7YI-Jbit2k3l)

Lets imagine that we have a matrix:
```python
matrix = [[1,2,3],
          [4,5,6],
          [7,8,9]]
```
 and we want to write it to a file called `'matrix.txt'`.

 We are going to need to open the file, save the data and then close the file.  Once we have done this, we can reopen the file and see the contents.


This is done in section 2.0 of the notebook.

Steps to writing a file:
1. Open the file for in **writing** mode
2. Write your data to the file
3. Close the file

----
### 2.1 Writing a new line
- It is also possible to write multiple lines and to do this, you want to use the character '\n'  

In section 2.1 of the notebook, you can see that I write a file with 2 lines.  

As well, I made the code to read and print each line of the file into a function!

-----
### 2.2 Using Pandas
Now we have been working with the built in functions in python, but as in the preivous lecture, we can use **Pandas** to make our life easier.  

We are going to follow these steps:
1. Make our matrix into a pandas data frame
2. Print out our data frame
3. Save our matrix to csv using Pandas
