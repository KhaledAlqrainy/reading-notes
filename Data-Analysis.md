# JupyterLab

>  is a next-generation web-based user interface for Project Jupyter, it enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner. 

* Documents and activities integrate with each other, enabling new workflows for interactive computing such as :

1- **Code Consoles** provide transient scratchpads for running code interactively, with full support for rich output. A code console can be linked to a notebook kernel as a computation log from the notebook, for example.

2- **Kernel-backed documents** enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.

3- **Notebook cell outputs** can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

4- Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. For example, it is easy to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.


# NumPy

> is a commonly used Python data analysis package, it  can speed up your workflow, and interface with other packages in the Python ecosystem.

### Lists Of Lists for CSV Data

* After we do the setup for cvs package, the data will read into list of lists, Each inner list is a row from the ssv file. As you may have noticed, each item in the entire list of lists is represented as a string, which will make it harder to do computations.

![Image](/lfl.PNG)


### Numpy 2-Dimensional Arrays

* we work with multidimensional arrays. We’ll dive into all of the possible types of multidimensional arrays later on, but for now, we’ll focus on 2-dimensional arrays. A 2-dimensional array is also known as a matrix, and is something you should be familiar with. In fact, it’s just a different way of thinking about a list of lists. A matrix has rows and columns.

### Creating A NumPy Array

* Once we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns

* One of the limitations of NumPy is that all the elements in an array have to be of the same type, so if we include the header row, all the elements in the array will be read in as strings.

### Indexing NumPy Arrays

* We can use array indexing to select individual elements, groups of elements, or entire rows and columns. 

### 1-Dimensional NumPy Arrays

*  A 1-dimensional array only needs a single index to retrieve an element. Each row and column in a 2-dimensional array is a 1-dimensional array. Just like a list of lists is analogous to a 2-dimensional array, a single list is analogous to a 1-dimensional array.

### NumPy Data Types

* **float** numeric floating point data.

* **int** integer data.

* **string**  character data.

* **object**  Python objects.

### Broadcasting

> NumPy performs broadcasting to try to match up elements. 

* The last dimension of each array is compared.
If the dimension lengths are equal, or one of the dimensions is of length 1, then we keep going.
If the dimension lengths aren’t equal, and none of the dimensions have length 1, then there’s an error.

* Continue checking dimensions until the shortest array is out of dimensions.

### Combining NumPy Arrays

* If we want to combine arrays horizontally, where the number of rows stay constant, but the columns are joined, then we can use the numpy.hstack function. The arrays we combine need to have the same number of rows for this to work.