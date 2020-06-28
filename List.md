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

* Negative indexing means beginning from the end, `-1` refers to the last item, `-2` refers to 
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

# This will return the items from index 0 to index 4.

Output:

print(thislist[:4])
['apple', 'banana', 'cherry', 'orange']
```

* By leaving out the end value, the range will go on to the end of the list:

```python
* This example returns the items from "cherry" and to the end:

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

# This will return the items from index 2 to the end.

Output:

print(thislist[2:])
['cherry', 'orange', 'kiwi', 'melon', 'mango']
```

## 5. Range of Negative Indexes

* Specify negative indexes if you want to start the search from the end of the list:

```python
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

# Negative indexing means starting from the end of the list.

# This example returns the items from index -4 (included) to index -1 (excluded)

# Remember that the last item has the index -1,

Output:

print(thislist[-4:-1])
['orange', 'kiwi', 'melon']
```

## 6. Change Item Value

* To change the value of a specific item, refer to the index number:

```python
* Change the second item:

thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant"

Output:

print(thislist)
['apple', 'blackcurrant', 'cherry']
```

## 7. Loop Through a List

* You can loop through the list items by using a `for` loop:

```python
* Print all items in the list, one by one:

thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x)

Output:

apple
banana
cherry  
```

## 8. Check if Item Exists

* To determine if a specified item is present in a list use the in keyword:

```python
* Check if "apple" is present in the list:

thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")

Output:

Yes, 'apple' is in the fruits list  
```

## 9. List Length

* To determine how many items a list has, use the len() function:

```python
* Print the number of items in the list:

thislist = ["apple", "banana", "cherry"]

Output:

print(len(thislist))
3
```

## 10. Add Items

* To add an item to the end of the list, use the `append()` method:

```python
thislist = ["apple", "banana", "cherry"]

thislist.append("orange")

Output:

print(thislist)
['apple', 'banana', 'cherry', 'orange']
```

* To add an item at the specified index, use the `insert()` method:

```python
* Insert an item as the second position:

thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")

Output:

print(thislist)
['apple', 'orange', 'banana', 'cherry']
```

## 11. Remove Item

* There are several methods to remove items from a list:

```python
* The `remove()` method removes the specified item:

thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")

Output:

print(thislist)
['apple', 'cherry']
```

* The `pop()` method removes the specified index, (or the last item if index is not specified):

```python
thislist = ["apple", "banana", "cherry"]
thislist.pop(0)

Output:

print(thislist)
['banana', 'cherry']

or

thislist = ["apple", "banana", "cherry"]
thislist.pop()

Output:

print(thislist)
['apple', 'banana']
```

* The `del` keyword removes the specified index:

```python
thislist = ["apple", "banana", "cherry"]
del thislist[0]

Output:

print(thislist)
['banana', 'cherry']
```

* The del keyword can also delete the list completely:

```python
thislist = ["apple", "banana", "cherry"]
del thislist

Output:

print(thislist) 

Traceback (most recent call last):
  File "demo_list_del2.py", line 3, in <module>
    print(thislist) # this will cause an error because you have succsesfully deleted "thislist".
NameError: name 'thislist' is not defined
```

* The `clear()` method empties the list:


```python
thislist = ["apple", "banana", "cherry"]
thislist.clear()

Output:

print(thislist)
[]
```

## 12. Copy a List

* There are ways to make a copy, one way is to use the built-in List method `copy()`.

```python
* Make a copy of a list with the `copy()` method:

thislist = ["apple", "banana", "cherry"]
mylist = thislist.copy()

Output:

print(mylist)
['apple', 'banana', 'cherry']
```

* Another way to make a copy is to use the built-in method `list()`.

```python
* Make a copy of a list with the `list()` method:

thislist = ["apple", "banana", "cherry"]
mylist = list(thislist)

Output:

print(mylist)
['apple', 'banana', 'cherry']
```


## 13. Join Two Lists

* There are several ways to join, or concatenate, two or more lists in Python.

* One of the easiest ways are by using the `+` operator.


```python
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

list3 = list1 + list2

Output:

print(list3)
['a', 'b', 'c', 1, 2, 3]
```

> Please inbox **[me](https://www.facebook.com/shoriot)**, if you've any questions.