Matrix times Vector (easy)

*Write a Python function that takes the dot product of a matrix and a vector. return -1 if the matrix could not be dotted with the vector*

#
```

Example:
        input: a = [[1,2],[2,4]], b = [1,2]
        output:[5, 10] 
        reasoning: 1*1 + 2*2 = 5;
                   1*2+ 2*4 = 10
```

```python
def matrix_dot_vector(a:list[list[int|float]],b:list[int|float])-> list[int|float]:
  c:list[int|float] = []
  if(len(a)!=len(b)):
    return -1
  for row in a:
    val:int = 0
    for col_index in range(len(row)):
      val+=row[col_index]*b[col_index]
    c.append(val)
  return c
```



