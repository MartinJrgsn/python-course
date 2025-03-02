[Home](/)

# Section 1

In this section we will learn the basics about using Anaconda Navigator and Jupyter Notebook. Once you have completed the instructions, or whenever you run into errors, you can find a notebook for this section [here](/Section%201/section-1.ipynb).

## Introduction to Anaconda Navigator

On the left-hand side of Anaconda Navigator you should see Home, Environments, Learning, Community, Documentation, Anaconda Blog, and some links to Anaconda's Social Media. Select Home, and ensure that your drop-down filters at the top of the Navigator says: "**All applications** on **base (root)**". Scroll down to where you can find Jupyter Notebook. If it is not already installed click **Install**, then click **Launch**. Anaconda Navigator can be used to install different applications that can be used for Python development. We can also install Python libraries from "Environments", but this will not be covered as of yet.

## Introduction to Jupyter Notebook

Jupyter Notebook is one of many ways you can write and run Python scripts in code cells in a notebook format. It also supports markdown in markdown cells. Jupyter Notebook has many use cases, ranging anywhere from learning and making notes to advanced topics such as data science.

After you click **Launch** a new tab will be opened in your default browser, and you will be met with Jupyter Notebook's User Interface (UI). From here you can navigate through your file system. You can create new directories (folders), files, or notebooks. You can also open files and notebooks. Notebooks are where you can write and run your code, in addition to taking notes (using markdown cells). This will be explained as we proceed.

### Create a Course Workspace

Let us get started by creating a directory (folder) that will be used to store our notebooks related to this course. This can be anywhere on your file system, but try to remember which directory you want to use for this course so that you can leave this course at any stage, and pick up at a later time. As I am writing and uploading this course to GitHub using Git, I have created a directory called Git. I have cloned my repository to my Git directory. This is the directory I will use to collect my different notebooks for this course.

If you have cloned this repository using Git, you may simply enter the cloned repository. I do not intend to cover Git during this course. Though it is, in my opinion, a necessary tool to learn if you want to write, version control, and share your code with others.

You can also download this course as a Zip-archive, extract the contents, and use my sources directly. However, you will often find that learning is more about doing something yourself, rather than blindly following instructions (E.g., running the code someone else has written as opposed to writing it yourself).

If you have not cloned this repository - navigate to, or create a directory for this course. You can do this by either right clicking inside Jupyter Notebook's UI, or clicking the **New** button at the top right in the UI. Then select **New Folder**. Select an appropriate name for this directory (i.e. "Git") and open the directory by left double-clicking on the directory. Inside your chosen directory, create a subdirectory that will be used exclusively for this project. Enter this subdirectory, and create your first notebook.

### Create a Notebook

You can create your first notebook similarily to how you created a new directory. Right click, and select **New Notebook**, or select the **New** button and select **Python 3 (ipykernel)**. If you are prompted to select a kernel, select the default option "Python 3 (ipykernel)", and click **Select**. You have now created your first notebook. We have not set a name for this Notebook, but assuming you have not created any other notebooks in your working directory the notebook will be named "*Untitled.ipynb*". We can change the name of the notebook by left clicking at the top of the UI where it says "Untitled". Rename the notebook to section-1.ipynb.

We now have a notebook called *section-1.ipynb* that is connected to the ipykernel which is what runs our code in the individual code cells.

#### Familiarize Yourself with the Notebook UI - *optional*

Starting with the most important options from the top:
- File:
    - New
        - Console
        Live ephemeral python environment
        - Notebook
        Python environment used to write, run, and document code
        - Terminal
        Integrated terminal in the Jupyter Notebook UI
        - Text file
        Simple .txt file
        - Markdown File
        Simple .md file
        - Python File
        Simple .py file (used for writing python scripts)
    - Save Notebook
    Saves the notebook you are currently in (I.e. section-1.ipynb)
    Windows & Linux shortcut CTRL+S, Mac OS shortcut CMD+S
    - Trust Notebook
    If you have downloaded a Notebook, it is not immediately trusted. Python scripts can cause harm to your system, because it runs with the same privileges as the user you have signed in with. This means that any files you can read, write, or execute, Python can perform the same actions. Always be careful when running unknown scripts, as it can lead to harm to your system.
    - Close and Shut Down Notebook
    When you are finished with your session, or a specific notebook, you can click this button to close it. This also frees up any memory that has been allocated to your session. Any variables that have been defined will have to be re-defined, because they have been de-allocated from memory.
    - Shut Down
    Shuts down the ipykernel, and ends the Jupyter Notebook session. You will no longer be able to access any notebooks from the UI, unless you re-launch Jupyter Notebook.
- Run
    - Run Selected Cell
    Allows you to execute the code in a code cell, or render the text in a markdown cell.
    - Run All Cells
    Runs every code and markdown cell in the entire notebook. If it fails at any step, it will not continue with the remaining cells.
- Kernel
    - Interrupt Kernel
    If your code seems to hang (E.g. gets stuck in an infinite loop), this can be used to force the execution of the code to stop.
    - Restart kernel and Clear Outputs of All Cells...
    Frees up memory by de-allocating variables. This means that any variables that have been previously defined in another code cell, will no longer be accessible.


#### Writing Code in a Notebook

In this section we will begin using the section-1.ipynb notebook to create markdown cells, and code cells where we will take notes, write and execute code.

##### Markdown Cells

The markdown cell allows for efficient note taking. In the Jupyter Notebook UI, select the first cell. There should be a drop down menu that says **Code**. Expand this drop down menu and select **Markdown**. You have now changed the cell from a code cell to a markdown cell. You can choose to copy the contents from the example below, or to write the contents in to your new markdown cell. You can render the markdown cell by either clicking the "Play button", selecting **Run** -> **Run Selected Cell**, or use the shortcut 'Shift+Enter'. The rendered result will show 

```markdown
# Markdown Cells

Markdown cells are useful for writing structured notes due to its simple, efficient and elegant formatting options. Some formats are illustrated below:

# H1 header
## H2 header
### H3 header
#### H4 header
##### H5 header
###### H6 header

## Math

Inline math: $ a \in A $

$$
x = \frac{-b + \sqrt{b^2 - 4ac}}{2a}
$$

## Lists

- Dotted lists
    - Nested dotted lists
 
1. Numbered lists
   1. Nested numbered lists

## Text formats

Plaintext

**bold**

*italic*

~strikethrough~
```

You can add python code snippets, (or other supported languages) to markdown cells using the following markdown syntax:


\`\`\`python
print(
    "This is an example of a code snippet in a markdown cell."
    "It has syntax highlighting in the form of colors."
)
\`\`\`

The markdown cell will have syntax highlighting, and will look similar to what you can see here:
```python
print(
    "This is an example of a code snippet in a markdown cell."
    "It has syntax highlighting in the form of colors."
)
```

Delete the markdown cell by selecting the cell you want to delete then click the Trash icon, or use the shortcut D, D (Press D consecutively two times). 

##### Code Cells

If you have deleted every cell in your notebook, you will only have one code cell in your notebook. If you want to keep your markdown cells, you can simply scroll to the bottom of your notebook, and select an empty cell. If there are no empty cells available, you can insert a new cell above or below the cell you have selected. If you want to insert a cell above, select a cell and press the A key once. If you want to insert a cell below, select a cell and press the B key once. There are also buttons that can be used for the same purpose.

Once you have created a new cell, you should ensure that the cell is of type "Code". This is done the same way you changed a cell type to "Markdown" in the [Markdown Cells](#markdown-cells) section above.

You can either copy the contents of the code snippet below, or manually write the block and inline comments to the code cell. Execute the code cell.

```python
"""
Code cells

This is a block comment.
The block comment starts and ends with three consecutive apostrophes.

Anything you write inside a block comment will not be executed by Python.
However, due to how Jupyter Notebook works, if you do not have any other code in a code cell, and run that cell, it will output the contents of the cell.
"""

# This is an inline comment.
# The inline comment starts with the use of the pound sign: #
# It can be added next to code, and python will still run the code before the # sign
# You can have multiple lines with comments.
```

Since we have not written anything else in the code cell, except for the block and inline comments, we will get the following output after running the code cell:

```
[1]: '\nCode cells\n\nThis is a block comment.\nThe block comment starts and ends with three consecutive apostrophes.\n\nAnything you write inside a block comment will not be executed by Python.\nHowever, due to how Jupyter Notebook works, if you do not have any other code in a code cell, and run that cell, it will output the contents of the cell.\n'
```

You can delete the code cell if you wish, and continue to the [next section](#datatypes).

##### Datatypes

Starting with the basics of programming. In my point of view, programming is about achieving an expected result by carefully "moving data around". Data can be stored in variables. We will now create a variable containing an Integer. Integers are a subset of real numbers ($\R$) consisting of all negative natural numbers, all positive natural numbers, including 0, $\Z \subseteq \R$. Assuming you are using a 64-bit processor, the largest (unsigned) integer your processor can (efficiently) compute is $2^64-1 = 18446744073709551615$. Python can perform calculations using larger numbers at the cost of efficiency. This is out of scope, so let us reduce the complexity.

###### Integers

We can start of by creating a code cell. Insert the following code into your newly created code cell:

```python
my_integer = 10
```

What we have done is assigned the value $10$ to a variable called `my_integer`. Reading from the left to the right, "`my_integer` equals 10". You can also read this code as "set `my_integer` to 10", or "store the value 10 inside the variable `my_integer`. We can see the type of any variable using the `type` function.

Create a new code cell, insert the following, and run the code cell:

```python
type(my_integer)
```

The output will say `int`. `int` is short for integer, and when we get into type-hinting, we will use this amongst other types to indicate what the expected type for a function is. We will get back to type-hinting at a later stage. For now, create a new code cell and run the following:

```python
print(my_integer)
```

The print command allows us to print any values inside the parantheses to the standard output. In a notebook, the standard output can be seen just below the code cell. Due to how Jupyter Notebook works, we do not explictly have to use the `print` function to output something to the standard output. Insert the following in a new cell and run it.

```python
my_integer
```

As we can see, the output does indeed look similar to when we used the `print` function, but it is limited. For instance, if we want to look at the value multiple times, we do have to use the `print` function. We can see this in action by inserting and running the following code:

```python
my_integer
my_integer
```

Insert and run the following:

```python
print(my_integer)
print(my_integer)
```

Compare the output of the two most recent code cells, and notice that in the former code cell we only see the value `10` printed out once, and in the latter, twice.

We can expand on using the `my_integer` variable by performing some basic arithmetic operations.

**Addition**
We can add 10 and 5 together (`my_integer` + 5 = 10 + 5 = 15):

```python
print(my_integer + 5)
```

**Subtraction**
We can subtract 5 from 10 (`my_integer` - 5 = 10 - 5 = 5):

```python
print(my_integer - 5)
```

**Multiplication**
We can multiply `my_integer` with itself (`my_integer`\*`my_integer` = 10\*10 = 100):

```python
print(my_integer*my_integer)
```

**Division**
We can divide 1 by `my_integer` (1/`my_integer` = 1/10 = 0.1)

```python
print(1/my_integer)
```

We have now looked at some basic arithmetic operations using integers. Division naturally leads us into another datatype, `float`.

###### Floats

A float, a floating-point value, or a decimal, is any value that is represented by a integer with a decimal. We use a "full-stop" or a period as the decimal separator, not a comma.

We can define a new variable `my_float`, and assign the value from the division operation previously performed:

```python
my_float = 1/my_integer
```

We can see that the result of the division operation holds the same value as the variable definition we just performed:

```python
print(my_float)
```

We can find the type of the `my_float` variable like we did with the integer variable earlier:

```python
type(my_float)
```

The output states that the variable is indeed a float. We can also look at additional information about the type using the `print` function paired with the `type` function.

```python
print(type(my_float))
```

Instead of just stating `float` as the datatype, we now see a concept that will be covered later:
```
<class 'float'>
```

###### Strings

Continuing with different datatypes we can move onto strings. We can use string to output text. A typical first line of code for any programming language course, is to output the text "Hello World!" to standard output.

If we want to print the text "Hello World!" to standard output, we can do the following:

```python
print("Hello World!")
```

We can achieve the same result in many different ways. Below are four examples:

```python
hello = "Hello"
space = " "
world = "World"
exclamation_mark = "!"

print(hello + space + world + exclamation_mark)
print(hello, world + exclamation_mark)
print(f"{hello} {world}{exclamation_mark}")
```

```python
my_string = "Hello World!"
print(my_string)
```

The point about these different methods is to prove the point that there are many ways to achieve the same result, but some methods are easier to read than others. I will leave it up to you to decide which method is the easiest to understand. Complicated code increases the risk for making mistakes. The easier the code is to read, the easier it is to make changes to the code at a later stage.
