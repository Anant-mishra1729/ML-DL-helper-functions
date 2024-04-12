## Show dataset preview
```python
def showData(X, y, n, ncols, figsize=(10, 4)):
    plt.figure(figsize=figsize)
    nrows = n // ncols + (n % ncols > 0)
    for i in range(n):
        ax = plt.subplot(nrows, ncols, i + 1)
        ax.imshow(X_train[i])
        ax.set_axis_off()
        ax.set_title(y_train[i])
```
![Screenshot_20240412_170433](https://github.com/Anant-mishra1729/ML-DL-useful-functions/assets/84588156/a51677d2-184a-49a8-b65c-2c9771b8134b)
