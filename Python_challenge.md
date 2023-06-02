


##  Write a Python function that takes a number as input and checks if it is prime. A prime number is a natural number greater than 1 that is divisible only by 1 and itself

```python
def is_prime(n):
    if n == 1:
        return False
    elif n == 2:
        return True
    else:
        for x in range(2,n):
            if n % x == 0:
                return False
        return True 
        
print(is_prime(9)) 
print(is_prime(11))



```

    False
    True

## Write a Python function that takes two lists as input and returns a new list containing the common elements between the two lists.

```python
def common_ele(list1, list2):
    new_list = []
    found_common = False  # Flag variable to track if any common elements are found
    
    for x in list1:
        if x in list2:
            new_list.append(x)
            found_common = True  # Set the flag to True if a common element is found
            
    if found_common:
        print("Common elements:", new_list)
    else:
        print("No common elements")

common_ele([1, 2, 3, 4], [5, 6, 7,8])
```

    No common elements

## Write a Python function that takes the following dictionary as input and returns a new dictionary where the keys and values are swapped. In other words, the function should create a new dictionary where the original values become the keys, and the original keys become the values.

original_dict = {“apple”: 1, “banana”: 2, “cherry”: 3}

```python
original_dict = {"apple": 1, "banana": 2, "cherry": 3}
def swapped_dictionary(original_dict):
        swapped_dictionary = {v:k for k,v in original_dict.items()}
        return swapped_dictionary
    
    
print(swapped_dictionary(original_dict))
    
        
```

    {1: 'apple', 2: 'banana', 3: 'cherry'}






