# Python-Notes


### Tuple:
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
## Tupule Methods 
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

### List[]:
-A list in Python is an ordered, mutable (changeable) collection that can hold items of any data type.      
-numbers, strings, other lists, objects, etc.
- Ordered → Elements have a fixed position (index starting from 0).
- Mutable → You can add, remove, or change items after creation.

## Types of elements in a list
- Integers: [1, 2, 3]
- Strings: ["a", "b", "c"]
- Floats: [1.1, 2.2, 3.3]
- Booleans: [True, False]
- Mixed types: [1, "two", 3.0, False]
- Other lists (nested lists): [1, [2, 3], 4]


## Common list operations
**1.Indexing:**  Get a single item by its position.
```python
my_list = [10, 20, 30, 40]
print(my_list[0])  # Output: 10
print(my_list[-1]) # Output: 40 (last element)

```
**2.Slicing:**  Get a sublist by specifying start, stop, and step.
```python
print(my_list[1:3])   # [20, 30]
print(my_list[::2])   # [10, 30] (every second element)
```
**3.Concatenation:** Join two lists together.

```python
a = [1, 2]
b = [3, 4]
c = a + b
print(c)  # [1, 2, 3, 4]
```
**4.Repetition:** Repeat the list multiple times.
```python
d = [0, 1]
print(d * 3)  # [0, 1, 0, 1, 0, 1]
```
**5.Membership:** Check if an item is in the list.
```python
fruits = ["apple", "banana", "cherry"]
print("banana" in fruits)   # True
print("grape" not in fruits)  # True
```
**6.Length:**  Number of elements in the list.
print(len(fruits))  # 3

## Common list methods

| Method      | Description                                                        | Example                                    |
| ----------- | ------------------------------------------------------------------ | ------------------------------------------ |
| `append()`  | Adds a single item to the end of the list                          | `my_list.append(5)`                        |
| `extend()`  | Adds multiple items from another iterable (like a list) to the end | `my_list.extend([6, 7])`                   |
| `insert()`  | Inserts an item at a specified index                               | `my_list.insert(2, 'apple')`               |
| `remove()`  | Removes the **first** occurrence of a specified value              | `my_list.remove('apple')`                  |
| `pop()`     | Removes and returns the last item (or item at specified index)     | `item = my_list.pop()` or `my_list.pop(1)` |
| `clear()`   | Removes all items from the list, making it empty                   | `my_list.clear()`                          |
| `index()`   | Returns the index of the **first** occurrence of a value           | `i = my_list.index('apple')`               |
| `count()`   | Counts how many times a value appears in the list                  | `n = my_list.count('apple')`               |
| `sort()`    | Sorts the list in place (modifies the list itself)                 | `my_list.sort()`                           |
| `reverse()` | Reverses the order of elements in the list (in place)              | `my_list.reverse()`                        |
| `copy()`    | Returns a shallow copy of the list                                 | `new_list = my_list.copy()`                |


## List comprehension.
- A list comprehension is a concise way to create a new list by transforming, filtering, or generating elements from an existing iterable (like a list, range, etc.).


## Dictionary { }
-A **dictionary** is a built-in Python data structure that stores data in key-value pairs.            

-Keys must be unique and immutable (e.g., strings, numbers, tuples).          

**Common Methods of Dictionaries**

**1.dict.keys()**              
-Returns a view object containing all keys.
```python
person = {"name": "Alice", "age": 25, "city": "New York"}
print(person.keys())
```
**Output**
``` python 
dict_keys(['name', 'age', 'city'])
 ```

**2.dict.values()**          
-Returns a view object containing all values.
``` python 
print(person.values())
```
**Output**
```python
dict_values(['Alice', 25, 'New York'])
```
**3. dict.items()**               
-Returns a view object containing key-value pairs as tuples.
 ```python
print(person.items())
 ```
**Output**
```python 
dict_items([('name', 'Alice'), ('age', 25), ('city', 'New York')])
```
**4. dict.get(key, default)***              
-Returns the value for the specified key; returns default if the key is not found.
```python
print(person.get("age"))           # Existing key
print(person.get("country", "USA"))  # Missing key, use default
```
**Output:**
 ```python
25
USA
```
**5. dict.update(other_dict)**           
-Updates the dictionary with key-value pairs from another dictionary.
```python
person.update({"age": 26, "country": "USA"})
print(person)
```
**Output:**
```python
{'name': 'Alice', 'age': 26, 'city': 'New York', 'country': 'USA'}
```


**6. dict.pop(key, default)**                   
-Removes the item with the specified key and returns its value. If the key is missing, returns default.
```python
age = person.pop("age", 0)
print("Popped age:", age)
print(person)
```
**Output:**
```python
Popped age: 26
{'name': 'Alice', 'city': 'New York', 'country': 'USA'}
```
**7. dict.popitem()**
-Removes and returns the last inserted key-value pair as a tuple.
```python
last_item = person.popitem()
print("Last item:", last_item)
print(person)
```
**Output:**
```python
Last item: ('country', 'USA')
{'name': 'Alice', 'city': 'New York'}
```
**8. dict.clear()**               
-Removes all items from the dictionary.
```python
person.clear()
print(person)
```
**Output:**
```python
{}
```
**9. dict.copy()**               
-Returns a shallow copy of the dictionary.
```python
student = {"name": "John", "marks": 90}
student_copy = student.copy()
print(student_copy)
```
**Output:**
```python
{'name': 'John', 'marks': 90}
```
**10.dict.setdefault(key, default)**             
-Returns the value of the key. If key doesn’t exist, inserts it with the default value.
```python
student = {"name": "John"}
grade = student.setdefault("grade", "A")
print("Grade:", grade)
print(student)
```
**Output:**
```python
Grade: A
{'name': 'John', 'grade': 'A'}
```





















