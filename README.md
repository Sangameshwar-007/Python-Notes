# Python-Notes


### Definition:
-A **tuple** is an **ordered, immutable** (cannot be changed after creation) collection of elements in Python.  
-It can store **heterogeneous**  data (i.e., different data types).                  
-A **tuple** allow the **duplicate values.**
-Slightly **faster** than **lists** for iteration.

**Example:**
```python
my_tuple= (10,20,50,"Hi",True)
print(my_tuple)
```
**Output:**

     (10, 20, 50, 'Hi', True)

**Accessing Elements:**
```python
my_tuple = (10, 20, 30, 40)

print(my_tuple[0])      # Output: 10
print(my_tuple[-1])     # Output: 40
print(my_tuple[1:3])    # Output: (20, 30)
```
## Tuple Methods:
**1.Concatenation:**
Tuples can be concatenated using the + operator. This operation combines two or more tuples to create a new tuple.

```python
my_tuple1 = (10,20,40)
my_tuple2 = (30,50,60)
my_tuple3 = my_tuple1 + my_tuple2    # Using Concatenation
print(my_tuple3)
```
**Output:**
```python
(10, 20, 40, 30, 50, 60)
```
**2.Repetition:**
creates a new tuple by repeating the original tuple's elements the specified number of times.

```python
my_tuple = 1,2,
new_tuple = my_tuple * 4
print(new_tuple)

```
**Output:**
```python
1, 2, 1, 2, 1, 2, 1, 2)
``` 

**3.Membership:**
 Checking if an item exists in the tuple.
 ```python
my_tuple = (11,21,20,32)
print(20 in my_tuple)      #Output: True
print(12 in my_tuple)      #Output: False
```
**4.Indexing:**
Accessing individual elements using their position (index).
```python
my_tuple = (1,2,3,4,5)
print(my_tuple[3])      #output: 4
print(my_tuple[-1])     #output:5  # reversed index
```

**5.Slicing:**
Getting a sub-tuple by specifying start, stop, and step.
```python
my_tuple = (10, 20, 30, 40, 50)
print(my_tuple[1:4]) 
print(my_tuple[::-1])    # reversed tuple
```
**Output:**
```python
(20, 30, 40)
(50, 40, 30, 20, 10)

```
**6.Length:**
Counting the number of elements in the tuple.
```python
tuple = ('hello world')
print(len(tuple))       #Output:11
```

**7.Iteration:**
Going through each element in the tuple one by one.

```python
tuple = ('apple', 'banana', 'cherry')
for fruit in tuple:
    print(fruit)

```
**Output:**
```python
apple
banana
cherry
```

**8.Max, Min, and Sum:**
Find the maximum, minimum, or sum of numeric tuple elements.
```python
nums = (4, 7, 1, 9)
print(max(nums))   
print(min(nums))  
print(sum(nums))   
```
**Output:**
```python
9
1
21
```
## Tupole Methods 
-They only **Two-built-in-function**

**1.Count() method:**
Counts how many times a specific element appears in the tuple.

```python
t1 = (1, 3, 2, 3)
print(t1.count(4))  #Output:2
```
**2.Index() method:**
Finds the first index of the specified element.
```python
t2 = (10, 20, 30,-30,40)
print(t2.index(-30))     #Output:3
```





 
 



    























 


