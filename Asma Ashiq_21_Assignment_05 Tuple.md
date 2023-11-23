# Assignment 05: -

### 1. Create an empty tuple and print it.


```python
empty_tuple = ()
print(empty_tuple)

```

    ()
    




    tuple



 ### 2. Create a tuple of your favorite fruits and print it.


```python
favorite_fruits = ('apple', 'banana', 'grapes', 'mango')
print(favorite_fruits)
```

    ('apple', 'banana', 'grapes', 'mango')
    




    tuple



### 3.  Create a tuple that includes a mix of data types (integers, strings, floats).


```python
mixed_tuple = (46, "Asma", 5.2)
print(mixed_tuple)
```

    (46, 'Asma', 5.2)
    




    tuple



### 4. Access the first element of a tuple.


```python
tuple = (10, 20, 30, 40)
first_element = tuple[0]
print(first_element)

```

    (10, 20, 30, 40)
    


    10
    

### 5. Access the last element of a tuple.


```python
tuple = (10, 20, 30, 40)
last_element = tuple[-1]
print(last_element)
```



    40




### 6. Access the second and third elements of a tuple.


```python
tuple = (10, 20, 30, 40)
second_and_third_element = tuple[1:3]
print(second_and_third_element)
```

    (20, 30)
    

### 7. Slice a tuple to extract the first three elements.



```python
tuple = (10, 20, 30, 40)
first_three_elements = tuple[:3]
print(first_three_elements)

```

    (10, 20, 30)
    

### 8."Slice a tuple to extract the last three elements.


```python
tuple = (10, 20, 30, 40)
last_three_elements = tuple[-3:]
print(last_three_elements)

```

    (20, 30, 40)
    

### 9. Slice a tuple to get every second element.


```python
tuple = (10, 20, 30, 40)
every_second_element = tuple[1::2]
print(every_second_element)


```

    (20, 40)
    

### 10. Reverse a tuple using slicing.


```python
tuple = (10, 20, 30, 40)
reverse_tuple = tuple[::-1]
print(reverse_tuple)

```

    (40, 30, 20, 10)
    

### 11. "Create two tuples and concatenate them.


```python
a = "ASMA"
b = "ASHIQ"
concatenate = a + b
print(concatenate)
```

    ASMAASHIQ
    

### 12. Repeat a tuple multiple times using the repetition operator.


```python
tuple = "Asma" * 5
print(tuple)
```

    AsmaAsmaAsmaAsmaAsma
    

### 13. "Find the index of a specific element in a tuple using the index() method.


```python
tuple = (10, 20, 30, 40)
element_to_find = 40
index_of_element = tuple.index(element_to_find)
print(index_of_element)
```

    3
    

### 14. Count the number of occurrences of a specific element in a tuple using the count() method.
   


```python
tuple = (10, 20, 30, 40, 30, 50, 30)
element_to_count = 30
occurrences = tuple.count(element_to_count)
print(occurrences)
```

    3
    

### 15. "Sort a tuple of numbers in ascending order.



```python
my_tuple = (10, 20, 30, 40, 30, 50, 30)
sorted_tuple = tuple(sorted(my_tuple))
print(sorted_tuple)
```

    (10, 20, 30, 30, 30, 40, 50)
    

### 16.  Sort a tuple of strings in alphabetical order.
 

```python
my_tuple = ("apple", "pomegaranete", "bnana", "orange")
sorted_tuple = tuple(sorted(my_tuple))
print(sorted_tuple)
```

    ('apple', 'bnana', 'orange', 'pomegaranete')
    

### 17.  "Sort a tuple of tuples based on the second element of each inner tuple.
   

```python
my_tuple = ((1, 5), (3, 2), (2, 8), (4, 1))
sorted_tuple = tuple(sorted(my_tuple, key=lambda x: x[1]))
print(sorted_tuple)
```

    
    sorted_tuple ((4, 1), (3, 2), (1, 5), (2, 8))
    

### 18.  "Compare two tuples to see if they are equal in both value and identity."
   

```python
tuple1 = (1, 2, 3)
tuple2 = (1, 2, 3)
value_equal = tuple1 == tuple2
identity_equal = tuple1 is tuple2
print(value_equal)
print(identity_equal)

```

    Tuples are equal in terms of values = True
    Tuples are not identical in terms of identity = False
  

### 19.  "Create a shallow copy of a tuple and observe the effects of modifying one of the tuples."

    
```python
original_tuple = ([4, 5], 'x', 'y')
shallow_copy_tuple = tuple(original_tuple)
print(shallow_copy_tuple)
original_tuple[0].append(6)
print(original_tuple)
```
    
    original_tuple: ([4, 5], 'x', 'y')
    shalllow_copy_tuple: ([4, 5], 'x', 'y')
    After modifying original tuple
    original_tuple: ([4, 5, 6], 'x', 'y')
    shallow_copy_tuple: ([4, 5, 6], 'x', 'y')

### 20.    "Create a deep copy of a nested tuple and observe the effects of modifying one of the tuples."
   


```python
original_nested_tuple = ([1, 2], 'x', 'y')
deep_copy_nested_tuple = copy.deepcopy(original_nested_tuple)
print(deep_copy_nested_tuple)
original_nested_tuple[0].append(3)
print(original_nested_tuple)
```

    Original Nested Tuple: ([1, 2], 'a', 'b')
    Deep Copy Nested Tuple: ([1, 2], 'a', 'b')

    After modifying the original nested tuple:
    Original Nested Tuple: ([1, 2, 3], 'a', 'b')
    Deep Copy Nested Tuple: ([1, 2], 'a', 'b')

    

### 21.  "Pickle a tuple and save it to a file."


```python
import pickle
new_tuple = ([10] , 'ASMA')
with open('new_tuple.pkl', 'wb') as file:
pickle.dump(new_tuple, file)
print("Tuple pickled and saved to 'new_tuple.pkl'")
```

    Tuple pickled and saved to 'new_tuple.pkl'

    

### 22. "Unpickle a tuple from a file and display its content."


```python
import pickle
with open('new_tuple.pkl', 'rb') as file:
    loaded_tuple = pickle.load(file)
print("Tuple loaded from '_tuple.pkl':", loaded_tuple)

```

   Tuple loaded from '_tuple.pkl': ([10], 'ASMA')




