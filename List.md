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
# Print the second item of the list:

thislist = ["apple", "banana", "cherry"]

Output:

print(thislist[1])
banana
```

## 3. Negative Indexing

* Negative indexing means beginning from the end, `-1` refers to the last item, `-2` refers to 
the second last item etc.


```python
# Print the last item of the list:

thislist = ["apple", "banana", "cherry"]

Output:

print(thislist[-1])
cherry
```

## 4. Range of Indexes

* You can specify a range of indexes by specifying where to start and where to end the range.


```python
# Return the third, fourth, and fifth item:

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

# This will return the items from position 2 to 5.

# Remember that the first item is position 0,
# and note that the item in position 5 is NOT included

Output:

print(thislist[2:5])
['cherry', 'orange', 'kiwi']


Note: The search will start at index 2 (included) and end at index 5 (not included).
```

* By leaving out the start value, the range will start at the first item:

```python
# This example returns the items from the beginning to "orange":

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

# This will return the items from index 0 to index 4.

Output:

print(thislist[:4])
['apple', 'banana', 'cherry', 'orange']
```

* By leaving out the end value, the range will go on to the end of the list:

```python
# This example returns the items from "cherry" and to the end:

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

# This will return the items from index 2 to the end.

Output:

print(thislist[2:])
['cherry', 'orange', 'kiwi', 'melon', 'mango']
```

## 5. Range of Negative Indexes

* Specify negative indexes if you want to start the search from the end of the list:

```python
# This example returns the items from index -4 (included) to index -1 (excluded)

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

# Remember that the last item has the index -1,

Output:

print(thislist[-4:-1])
['orange', 'kiwi', 'melon']
```

## 6. Change Item Value

* To change the value of a specific item, refer to the index number:

```python
# Change the second item:

thislist = ["apple", "banana", "cherry"]

thislist[1] = "blackcurrant"

Output:

print(thislist)
['apple', 'blackcurrant', 'cherry']
```

## 7. Loop Through a List

* You can loop through the list items by using a `for` loop:

```python
# Print all items in the list, one by one:

thislist = ["apple", "banana", "cherry"]

for s in thislist:
  print(s)

Output:

apple
banana
cherry  
```

## 8. Check if Item Exists

* To determine if a specified item is present in a list use the `in` keyword:

```python
# Check if "apple" is present in the list:

thislist = ["apple", "banana", "cherry"]

if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")

Output:

Yes, 'apple' is in the fruits list  
```

## 9. List Length

* To determine how many items a list has, use the `len(` function:

```python
# Print the number of items in the list:

thislist = ["apple", "banana", "cherry"]

Output:

print(len(thislist))
3
```

## 10. Add Items

```python
1. append()
2. insert()
```

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
# Insert an item as the second position:

thislist = ["apple", "banana", "cherry"]

thislist.insert(1, "orange")

Output:

print(thislist)
['apple', 'orange', 'banana', 'cherry']
```

## 11. Remove Item

```python
1. remove()
2. pop()
3. del
4. clear()
```

* There are several methods to remove items from a list:

```python
# The `remove()` method removes the specified item:

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

* The `del` keyword can also delete the list completely:

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

```python
first_name = 'SD'
last_name = 'Shoriot'

full_name = first_name + " " + last_name
print(full_name)
SD Shoriot
```

* Another way to join two lists are by appending all the items from list2 into list1, 
one by one:

```python
* Append list2 into list1:


list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

for x in list2:
  list1.append(x)

Output:

print(list1)
['a', 'b', 'c', 1, 2, 3]
```

* Or you can use the `extend()` method, which purpose is to add elements from one list 
to another list:

```python
* Use the `extend()` method to add list2 at the end of list1:

list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

list1.extend(list2)

Output:

print(list1)
['a', 'b', 'c', 1, 2, 3]
```

## 14. The list() Constructor

* It is also possible to use the `list()` constructor to make a new list.

```python
* Using the list() constructor to make a List:

thislist = list(("apple", "banana", "cherry"))

Output:

print(thislist)
['apple', 'banana', 'cherry']
```


## 15. List Methods

* Python has a set of built-in methods that you can use on lists.

<pre>
<b>Method			Description</b>

1. append()		Adds an element at the end of the list
2. clear()		Removes all the elements from the list
3. copy()		Returns a copy of the list
4. count()		Returns the number of elements with the specified value
5. extend()		Add the elements of a list (or any iterable), to the end of the current list
6. index()		Returns the index of the first element with the specified value
7. insert()		Adds an element at the specified position
8. pop()		Removes the element at the specified position
9. remove()		Removes the item with the specified value
10. reverse()		Reverses the order of the list
11. sort()		Sorts the list
</pre>


> Please inbox **[me](https://www.facebook.com/shoriot)**, if you've any questions.