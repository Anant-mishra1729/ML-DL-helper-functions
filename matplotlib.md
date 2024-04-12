## Show dataset preview
```python
def showData(X, y, n, ncols, figsize=(10, 4)):
    """
    Display a grid of images along with their labels.

    Parameters:
    X (list or array): List of image data.
    y (list or array): List of corresponding labels.
    n (int): Number of images to display.
    ncols (int): Number of columns in the grid.
    figsize (tuple, optional): Figure size. Default is (10, 4).
    """
    plt.figure(figsize=figsize)
    nrows = n // ncols + (n % ncols > 0)
    for i in range(n):
        ax = plt.subplot(nrows, ncols, i + 1)
        ax.imshow(X[i])
        ax.set_axis_off()
        ax.set_title(y[i])
```
![Screenshot_20240412_170433](https://github.com/Anant-mishra1729/ML-DL-useful-functions/assets/84588156/a51677d2-184a-49a8-b65c-2c9771b8134b)
