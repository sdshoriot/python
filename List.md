<h1><p align="center">List</p></h1>


* A list is a collection which is ordered and changeable. In Python lists are written 
with square brackets.

## 1. Create a List

```python
thislist = ["apple", "banana", "cherry"]

Output:

print(thislist)
['apple', 'banana', 'cherry']
```

## 2. Access Items

* You access the list items by referring to the index number:

```python
* Print the second item of the list:

thislist = ["apple", "banana", "cherry"]

Output:

print(thislist[1])
banana
```

## 3. Negative Indexing

* Negative indexing means beginning from the end, -1 refers to the last item, -2 refers to 
the second last item etc.


```python
* Print the last item of the list:

thislist = ["apple", "banana", "cherry"]

Output:

print(thislist[-1])
cherry
```

## 4. Range of Indexes

* You can specify a range of indexes by specifying where to start and where to end the range.

* When specifying a range, the return value will be a new list with the specified items.

```python
* Return the third, fourth, and fifth item:

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

# This will return the items from position 2 to 5.

# Remember that the first item is position 0,
# and note that the item in position 5 is NOT included

Output:

print(thislist[2:5])
['cherry', 'orange', 'kiwi']


Note: The search will start at index 2 (included) and end at index 5 (not included).

Remember that the first item has index 0.
```

* By leaving out the start value, the range will start at the first item:

```python
* This example returns the items from the beginning to "orange":

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

Output:

print(thislist[:4])
['apple', 'banana', 'cherry', 'orange']
```

> Please inbox **[me](https://www.facebook.com/shoriot)**, if you've any questions.