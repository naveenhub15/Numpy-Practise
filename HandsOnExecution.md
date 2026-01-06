```python
line="*"
max_length=10
```


```python
print(line)
```

    *
    


```python
while len(line)<=max_length:
    print(line)
    line=line+"*"

```

    *
    **
    ***
    ****
    *****
    ******
    *******
    ********
    *********
    **********
    


```python
while len(line)>0:
    print(line)
    line=line[:-1]
```

    ***********
    **********
    *********
    ********
    *******
    ******
    *****
    ****
    ***
    **
    *
    


```python
line
```




    ''




```python
star="*"
space=" "
i=1
j=5
while i<5:
    while j>0:
        print(f"{j*space}{i*star}")
        i=i+1
        j=j-1
while j<5:
    while i>0:
        print(f"{j*space}{i*star}")
        i=i-1
        j=j+1
```

         *
        **
       ***
      ****
     *****
    ******
     *****
      ****
       ***
        **
         *
    


```python
x=0
y=5
star2="*"
gap=" "
while x<5:
    while y>0:
        print(f"{gap*y}{star2*x}*{star2*x}{gap*y}")
        x+=1
        y-=1
while y<5:
    while x>0:
        print(f"{gap*y}{star2*x}*{star2*x}{gap*y}")
        x-=1
        y+=1
```

         *     
        ***    
       *****   
      *******  
     ********* 
    ***********
     ********* 
      *******  
       *****   
        ***    
    


```python
person={
    "Name":"John Doe",
    "Sex":"Male",
    "Age":32,
    "Married":True}

for key in person:
    print("Key:", key, "," ,"Value:",person[key])
```

    Key: Name , Value: John Doe
    Key: Sex , Value: Male
    Key: Age , Value: 32
    Key: Married , Value: True
    


```python
for i in range(2,11,2):
    print(i)
```

    2
    4
    6
    8
    10
    


```python
person
```




    {'Name': 'John Doe', 'Sex': 'Male', 'Age': 32, 'Married': True}




```python
for s in person:
    print (s)
```

    Name
    Sex
    Age
    Married
    


```python
def filter(list):
    result=[]
    for number in list:
        if number%2==0:
            result.append(number)
    return result
```


```python
l1=list(range(1,11))
filter(l1)
```




    [2, 4, 6, 8, 10]




```python
filter([2,3,4,5,6])
print("a")
print(filter([2,3,4,5,6]))
```

    a
    [2, 4, 6]
    


```python
round(10.23847364732,10
    )
```




    10.2384736473




```python
import numpy as np
l1=list(range(1000000))
l2=list(range(1000000,2000000))
arr1=np.array(l1)
arr2=np.array(l2)

```


```python
%%time
s=0
for x,y in zip(l1,l2):
    s=s+(x*y)
print(s)
```

    833332333333500000
    CPU times: total: 484 ms
    Wall time: 491 ms
    


```python
%%time
arr3=arr1*arr2
int(arr3.sum())
```

    CPU times: total: 0 ns
    Wall time: 8.43 ms
    




    833332333333500000




```python
arr4=np.random.randint(10,100, size=(5,3))
arr5=arr4.copy()
```


```python
print(arr5)
```

    [[86 56 97]
     [51 81 12]
     [43 43 97]
     [95 28 41]
     [31 52 35]]
    


```python
arr6=np.array([[[40,61,92],
               [28,74,81]],
               [[86,88,16],
               [54,79,53]]])
```


```python
arr6
```




    array([[[40, 61, 92],
            [28, 74, 81]],
    
           [[86, 88, 16],
            [54, 79, 53]]])




```python
print(arr6.shape)
arr6.dtype
```

    (2, 2, 3)
    




    dtype('int64')




```python
arr6.sum(axis=1)
```




    array([[ 68, 135, 173],
           [140, 167,  69]])




```python
arr7=np.array([[40,61,92],
               [28,74,81],
               [86,88,16]])
```


```python
arr8=np.array([[1],
              [1],
              [1]])
arr7@arr8
```




    array([[193],
           [183],
           [190]])




```python
arr6
```




    array([[[40, 61, 92],
            [28, 74, 81]],
    
           [[86, 88, 16],
            [54, 79, 53]]])




```python
print(arr6[1,0,1:])
```

    [88 16]
    


```python

```
