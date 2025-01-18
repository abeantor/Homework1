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
Using list() Constructor: The list() function creates an empty list or converts an iterable into a list.
```python
empty_list = list()
print(empty_list)  # Output: []
print(len(empty_list))  # Output: 0
```

### Using Square Brackets `[]`
Using Square Brackets ([]): Square brackets are a shorthand for creating lists.
```python
empty_list = []
print(empty_list)  # Output: []
print(len(empty_list))  # Output: 0
```

### Lists with Initial Values
Lists with Initial Values: Lists can be initialized with predefined elements.
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print('Fruits:', fruits)  # Output: Fruits: ['banana', 'orange', 'mango', 'lemon']
print('Number of fruits:', len(fruits))  # Output: 4
```

---

## Accessing List Items

### Positive Indexing
Positive Indexing: Access items using their position, starting at 0.
Indexing starts at `0`.
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print(fruits[0])  # Output: banana
print(fruits[2])  # Output: mango
```

### Negative Indexing
Negative Indexing: Access items from the end of the list, starting at -1.
Negative indices start at `-1` (last item).
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print(fruits[-1])  # Output: lemon
print(fruits[-3])  # Output: orange
```

---

## Unpacking List Items
Unpacking List Items: Assign individual items to variables in a list.
You can unpack a list into variables:
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
first, second, third, *rest = fruits
print(first)  # Output: banana
print(rest)   # Output: ['lemon']
```

---

## Slicing Lists
Positive Index Slicing: Extract a subset of the list using positive indices.
### Positive Index Slicing
```python
fruits = ['banana', 'orange', 'mango', 'lemon']
print(fruits[1:3])  # Output: ['orange', 'mango']
print(fruits[:3])   # Output: ['banana', 'orange', 'mango']
print(fruits[::2])  # Output: ['banana', 'mango']
```

### Negative Index Slicing
Negative Index Slicing: Extract a subset of the list using negative indices.
```python
print(fruits[-3:-1])  # Output: ['orange', 'mango']
print(fruits[::-1])   # Output: ['lemon', 'mango', 'orange', 'banana']
```

---

## Modifying Lists
Lists are mutable, so you can update their contents using index assignments.
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
Copying a List: Create a duplicate of a list using the copy() method.
```python
fruits_copy = fruits.copy()
print(fruits_copy)  # Output: ['banana', 'orange', 'mango', 'lemon']
```

### Joining Lists
Joining Lists: Combine two or more lists into one.
```python
fruits = ['banana', 'orange']
vegetables = ['carrot', 'onion']
combined = fruits + vegetables
print(combined)  # Output: ['banana', 'orange', 'carrot', 'onion']
```

### Counting Items
Counting Items: Count occurrences of a specific value in the list.
```python
print(fruits.count('banana'))  # Output: 1
```

### Finding the Index of an Item
Finding the Index of an Item: Get the index of the first occurrence of a value.
```python
print(fruits.index('orange'))  # Output: 1
```

### Reversing a List
Reversing a List: Reverse the order of the elements in the list.
```python
fruits.reverse()
print(fruits)  # Output: ['lemon', 'mango', 'orange', 'banana']
```

### Sorting a List
Sorting a List: Arrange the items in ascending or descending order.
```python
fruits.sort()
print(fruits)  # Output: ['banana', 'lemon', 'mango', 'orange']


# Python Exercises - Level 1

## 1. Declare an empty list

```python
empty_list = []
```

## 2. Declare a list with more than 5 items

```python
my_list = [1, 2, 3, 4, 5, 6, 7]
```

## 3. Find the length of your list

```python
list_length = len(my_list)
print(list_length)
```

## 4. Get the first item, the middle item and the last item of the list

```python
first_item = my_list[0]
middle_item = my_list[len(my_list) // 2]
last_item = my_list[-1]

print(first_item, middle_item, last_item)
```

## 5. Declare a list called `mixed_data_types`, put your(name, age, height, marital status, address)

```python
mixed_data_types = ["Abu", 25, 5.9, "Single", "Noakhali, Bangladesh"]
```

## 6. Declare a list variable named `it_companies` and assign initial values Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon.

```python
it_companies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"]
```

## 7. Print the list using print()

```python
print(it_companies)
```

## 8. Print the number of companies in the list

```python
print(len(it_companies))
```

## 9. Print the first, middle and last company

```python
first_company = it_companies[0]
middle_company = it_companies[len(it_companies) // 2]
last_company = it_companies[-1]

print(first_company, middle_company, last_company)
```

## 10. Print the list after modifying one of the companies

```python
it_companies[2] = "Microsoft Corporation"
print(it_companies)
```
