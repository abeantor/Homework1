# Python: Lists

## Overview

Python has four collection data types:

1. **List**: Ordered and mutable. Allows duplicate members.
2. **Tuple**: Ordered and immutable. Allows duplicate members.
3. **Set**: Unordered, unindexed, and mutable (you can add new items). Duplicate members are not allowed.
4. **Dictionary**: Unordered, indexed, and mutable. Duplicate keys are not allowed.

---

## Lists in Python

A **list** is an ordered collection of different data types. It is mutable, meaning you can modify its content. Lists can also be empty or contain items of varying data types.

---

## Creating a List

### Using `list()` Constructor
```python
empty_list = list()
print(empty_list)  # Output: []
print(len(empty_list))  # Output: 0
```

### Using Square Brackets `[]`
```python
empty_list = []
print(empty_list)  # Output: []
print(len(empty_list))  # Output: 0
```

### Lists with Initial Values
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print('Fruits:', fruits)  # Output: Fruits: ['banana', 'orange', 'mango', 'lemon']
print('Number of fruits:', len(fruits))  # Output: 4
```

---

## Accessing List Items

### Positive Indexing
Indexing starts at `0`.
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print(fruits[0])  # Output: banana
print(fruits[2])  # Output: mango
```

### Negative Indexing
Negative indices start at `-1` (last item).
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print(fruits[-1])  # Output: lemon
print(fruits[-3])  # Output: orange
```

---

## Unpacking List Items

You can unpack a list into variables:
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
first, second, third, *rest = fruits
print(first)  # Output: banana
print(rest)   # Output: ['lemon']
```

---

## Slicing Lists

### Positive Index Slicing
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print(fruits[1:3])  # Output: ['orange', 'mango']
print(fruits[:3])   # Output: ['banana', 'orange', 'mango']
print(fruits[::2])  # Output: ['banana', 'mango']
```

### Negative Index Slicing
```python
print(fruits[-3:-1])  # Output: ['orange', 'mango']
print(fruits[::-1])   # Output: ['lemon', 'mango', 'orange', 'banana']
```

---

## Modifying Lists

Lists are mutable, meaning you can change their content:
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
fruits[0] = 'avocado'
print(fruits)  # Output: ['avocado', 'orange', 'mango', 'lemon']
```

---

## Adding Items to a List

### Append Items
Adds an item to the end of the list.
```python
fruits.append('apple')
print(fruits)  # Output: ['banana', 'orange', 'mango', 'lemon', 'apple']
```

### Insert Items
Inserts an item at a specified position.
```python
fruits.insert(1, 'grape')
print(fruits)  # Output: ['banana', 'grape', 'orange', 'mango', 'lemon']
```

---

## Removing Items from a List

### Remove by Value
Removes the first occurrence of a value.
```python
fruits.remove('banana')
print(fruits)  # Output: ['orange', 'mango', 'lemon']
```

### Pop by Index
Removes and returns an item by its index (default is the last item).
```python
fruits.pop(2)
print(fruits)  # Output: ['orange', 'mango']
```

### Delete by Index
Deletes an item by its index.
```python
del fruits[1]
print(fruits)  # Output: ['orange', 'lemon']
```

### Clear All Items
Empties the list.
```python
fruits.clear()
print(fruits)  # Output: []
```

---

## List Operations

### Copying a List
```python
fruits_copy = fruits.copy()
print(fruits_copy)  # Output: ['banana', 'orange', 'mango', 'lemon']
```

### Joining Lists
```python
fruits = ['banana', 'orange']
vegetables = ['carrot', 'onion']
combined = fruits + vegetables
print(combined)  # Output: ['banana', 'orange', 'carrot', 'onion']
```

### Counting Items
```python
print(fruits.count('banana'))  # Output: 1
```

### Finding the Index of an Item
```python
print(fruits.index('orange'))  # Output: 1
```

### Reversing a List
```python
fruits.reverse()
print(fruits)  # Output: ['lemon', 'mango', 'orange', 'banana']
```

### Sorting a List
```python
fruits.sort()
print(fruits)  # Output: ['banana', 'lemon', 'mango', 'orange']
