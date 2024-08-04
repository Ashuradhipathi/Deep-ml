*Write a Python function that computes the transpose of a given matrix.*

# Example 

```
        input: a = [[1,2,3],[4,5,6]]
        output: [[1,4],[2,5],[3,6]]
        reasoning: The transpose of a matrix is obtained by flipping rows and columns.
```

# Code

```python
def transpose_matrix(a: list[list[int|float]]) -> list[list[int|float]]:
    m:int = len(a)
    n:int = len(a[0])
    b = []
    for i in range(n):
      row = []
      for j in range(m):
        row.append(a[j][i])
      b.append(row)
        
    return b
```
![Transpose of a Matrix](https://github.com/Ashuradhipathi/Deep-ml/blob/main/media/Transpose%20of%20a%20Matrix.png)
