# 1. Lists
a.)
```python
my_list = list(range(1,101))

print(type(my_list))

#method 1
my_list.append(103)
my_list.append(104)
print(my_list)

#method 2
my_list.remove(103)
print(my_list)

# method 3
my_list.insert(0,105)
print(my_list)

# method 4
my_list.clear()
print(my_list)
```
b.)
```python
"""You could use remove last 3 values, then use slicing assignment to insert
those values at the beginning of the list"""

list1=list(range(11))
print(list1)

del list1[8:11]
print(list1)

list1[0:0] =  [8,9,10]
print(list1)
```
c.) The objects in that range of indexes will be multiplied by 3

d.)
```python
my_list_ten=["sonic", "mario", "goku", "pacman", "sonic", "goku", "mario", "eminem", "skips", "rigby"]
print(type(my_list_ten))

my_list_ten_mem = [id(item) for item in my_list_ten]
print(my_list_ten_mem)

duplicates= list({(item) for item in my_list_ten if my_list_ten.count(item)>1})
print(duplicates)
duplicates= list({item for item in my_list_ten_mem if my_list_ten_mem.count(item)>1})
print(duplicates)
```

