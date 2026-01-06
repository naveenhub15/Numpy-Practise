# numpy exercises
```

#### 1. Import the numpy package under the name `np` (★☆☆)


```python
import numpy as np
```

#### 2. Print the numpy version and the configuration (★☆☆)


```python

```

#### 3. Create a null vector of size 10 (★☆☆)


```python
a=np.zeros(10)
a
```




    array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.])



#### 4. How to find the memory size of any array (★☆☆)


```python
np.size(a)
```




    10



#### 5. How to get the documentation of the numpy add function from the command line? (★☆☆)


```python
a=a+1
a
```




    array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.])



#### 6. Create a null vector of size 10 but the fifth value which is 1 (★☆☆)


```python
b=np.zeros(10)
b[5]=1
b
```




    array([0., 0., 0., 0., 0., 1., 0., 0., 0., 0.])



#### 7. Create a vector with values ranging from 10 to 49 (★☆☆)


```python
c=np.random.randint(10,49,15)
c
```




    array([39, 32, 41, 18, 15, 35, 20, 34, 31, 10, 27, 42, 27, 19, 25],
          dtype=int32)



#### 8. Reverse a vector (first element becomes last) (★☆☆)


```python
d=c[::-1]
d
```




    array([25, 19, 27, 42, 27, 10, 31, 34, 20, 35, 15, 18, 41, 32, 39],
          dtype=int32)



#### 9. Create a 3x3 matrix with values ranging from 0 to 8 (★☆☆)


```python
e=np.random.randint(0,8,size=(3,3))
e
```




    array([[5, 4, 7],
           [7, 5, 5],
           [0, 1, 4]], dtype=int32)



#### 10. Find indices of non-zero elements from [1,2,0,0,4,0] (★☆☆)


```python
f=[1,2,0,0,4,0]
indices=np.nonzero(f)[0]
indices
```




    array([0, 1, 4])



#### 11. Create a 3x3 identity matrix (★☆☆)


```python
g=np.eye(3,3)
g
```




    array([[1., 0., 0.],
           [0., 1., 0.],
           [0., 0., 1.]])



#### 12. Create a 3x3x3 array with random values (★☆☆)


```python
h=np.random.randint(10,99,size=(3,3,3))
h
```




    array([[[70, 73, 65],
            [73, 84, 70],
            [53, 35, 81]],
    
           [[76, 80, 36],
            [19, 80, 95],
            [24, 67, 39]],
    
           [[94, 11, 77],
            [91, 81, 12],
            [84, 47, 85]]], dtype=int32)



#### 13. Create a 10x10 array with random values and find the minimum and maximum values (★☆☆)


```python
i=np.random.randint(10,99,size=(10,10))
print(i)
print(i.min())
print(i.max())
```

    [[70 63 54 32 48 91 60 87 94 89]
     [80 14 33 10 58 62 46 42 66 43]
     [23 13 26 53 69 69 73 12 42 98]
     [93 28 52 39 96 76 54 96 89 71]
     [23 35 38 38 42 89 16 98 45 47]
     [50 38 85 25 46 47 66 88 94 46]
     [58 47 36 12 43 55 35 31 94 61]
     [85 37 34 20 14 46 28 93 89 35]
     [50 23 77 88 48 38 67 17 92 73]
     [87 40 35 56 73 74 23 58 89 15]]
    10
    98
    

#### 14. Create a random vector of size 30 and find the mean value (★☆☆)


```python
j=np.random.randint(1,50,30)
print(j)
j.mean()
```

    [10 41 17 23 20  6  8  9 22 37 13 29 26 33 22 39  8 12 30  5 34 15 34 31
     43 14 26 22  7 30]
    




    np.float64(22.2)



#### 15. Create a 2d array with 1 on the border and 0 inside (★☆☆)


```python
k=np.array([[1,1,1],
           [1,0,1],
           [1,1,1]])
k
```




    array([[1, 1, 1],
           [1, 0, 1],
           [1, 1, 1]])



```
