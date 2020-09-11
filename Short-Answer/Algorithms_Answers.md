#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```python
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```


```
b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
```

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```

## Exercise II

initiate the function passing in the building n
set f = None

while f is None:
    get the midpoint of the building n

    if n[midpoint] breaks an egg:
        midpoint = midpoint / 2

    if n[midpoint] does not break an egg:
        for item in n[midpoint:]
            if egg breaks:
                f = n[item - 1]

if f is not None:
    return f


So there is a nested loop in this solution but using the midpoint I am able to cut the length of the building in half each iteration

If i am understanding this correctly it should run at O(log n) similair to a BST

