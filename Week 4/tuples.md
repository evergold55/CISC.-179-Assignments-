## 1. Exercising tuples

**1a)** Take five inputs from a user and save them in a tuple called `my_tuple`

```
#my_tuple =(
    input("Enter value 1: "),
    input("Enter value 2: "),
    input("Enter value 3: "),
    input("Enter value 4: "),
    input("Enter value 5: ")
)

print(my_tuple)
```

**1b.** How do you assign a single element in a tuple?

```
# one_element_ tuple_ 1 = (10)
```

**1c.** `my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)` Count the repeated integers and print the result on the console.

```
# {1: 3, 2: 4, 3: 4, 4: 2, 5: 1}
```

**1d.** `my_tuple = my_tuple + my_tuple`

Proof that `my_tuple` in part c is different than the `my_tuple` in part d.

```
# my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)
print(id(my_tuple))



my_tuple= my_tuple + my_tuple
print(id(my_tuple))


```

**1e.** Explain why the following operations aren’t legal for the tuple. Answer without using the Python.

```
x = (1,2,3,4)
x.append(1)
x[1] = "hello"
del x[2]

"Tuples are immutable and cannot be modified."
```

## 2. Packing and unpacking tuples

Python permits tuples to appear on the left side of an assignment operator, in which case variables in the tuple receive the corresponding values from the tuple on the right side of the assignment operator. Here’s a simple example:

```
(one, two, three, four) =  (1, 2, 3, 4)
```

**2a.** What is the data type of each variable?
```x = (1, 2, 3, 4)
a, b, *c = x
a, b, c

print(type(x))
print(type(a))
print(type(b))
print(type(c))

<class 'tuple'>
<class 'int'>
<class 'int'>
<class 'list'>
```
**2b.** Python has an extended unpacking feature, allowing an element marked with * to absorb any number of elements not matching the other elements. For example,

```
x = (1, 2, 3, 4)
a, b, *c = x
a, b, c
```

```
(1, 2, [3, 4])
```

**2c.** What will be the result of `a, *b, c = x`?

```
(1,[2,3],4)
```

## 3. Memory management

```
my_x = [100,200,300,400]
my_y = (200,300,400,500)
```

Discuss how memory addresses are assigned to each index of the list and the tuple. Pay attention to new addresses & re-used addresses.

| Index |     my_x      |     my_x      |
| ----- | ----          | ----          |
| 0     | 4355733016    | 4355736216    |
| 1     | 4355736216    | 4332689648    |
| 2     | 4332689648    | 4332691792    |
| 3     | 4332691792    | 4334142352    |

## Challenges
