# Nonogram Generator

Generate nonogram scenario randomly and Visualize with matplotlib

### Demo



### Prerequisites

`Jupyter notebook` `matplotlib` `numpy`


## Generator

```python 
def generator(size):
    board = np.random.randint(0, 2, size=(size, size))
    xl = get_line(board)
    board = board.T
    yl = get_line(board)
    board = board.T

    return xl, yl, board, size 
```

### Test

```python
xl, yl, board, size = generator(15)
render_board(yl, xl, board, size)
```


