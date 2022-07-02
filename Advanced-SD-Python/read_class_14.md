# Read: Class 14

## Matplotlib

Matplotlib is a Python package for 2D-graphics, used for visualizing data.

**Note**: this package needs to be imported to be used of course.

### Creating a simple plot:

First import pyplot from matplotlib:
    
    import matplotlib.pyplot as plt

Then give the plot data, and use show() to render it:

    plt.plot([1, 2, 3, 4])
    plt.show()

![plot pic](https://matplotlib.org/2.0.2/mpl_examples/pyplots/pyplot_simple.png)

#### Some useful methods:

|**Method**|**Use**|
|----------|-------|
|plt.ylabel()|Allows naming the y axis|
|plt.xlabel()|Allows naming the x axis|
|plt.axis()|Allows specifying the min and max of each axis|
|plt.title()|Allows specifying a title for the plot|
|plt.grid()|Allows enabling and disabling the grid for the plot|
|plt.text()|Allows placing a text in a specific point|

**Note**: Line properties can be controlled by changing them with in the plt.plot().  

## Things I want to know more about

- Matplotlib.