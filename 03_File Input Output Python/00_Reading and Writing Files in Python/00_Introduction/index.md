# File IO

File IO stands for **File Input Output**.  This implies reading and writing files.  This short course will cover how to read and write files using python, and we will be using **Google Colab Notebooks** to achieve this, and all of these lectures will be directly tied to a Notebook.  

Below are the instructions to getting started with **Google Colab Notebooks**

1. Follow [this link](https://colab.research.google.com/drive/1AFPMUJp3OTXKYnyaC-DI_WLhITmtWQMC) link to the notebook
2. Click **File** under the name of the document(_File IO Notebook.ipynb_)
3. Select option 9 -- _Save Copy in Drive_
4. Now you should have the notebook saved in your drive and we can begin with File IO

The syntax for opening a file in python is:
```python
file_object  = open(“filename”, “mode”)
```
where file_object is the variable to add the file object.

The modes are:

- ‘r’ – Read mode which is used when the file is only being read
- ‘w’ – Write mode which is used to edit and write new information to the file (any existing files with the same name will be erased when this mode is activated) 
- ‘a’ – Appending mode, which is used to add new data to the end of the file; that is new information is automatically amended to the end
- ‘r+’ – Special read and write mode, which is used to handle both actions when working with a file
