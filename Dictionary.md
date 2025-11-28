
## 1. Creating and accessing dictionary

**1a)** Create dictionary of your choice of keys and values. Create dictionary size of 10 elements.

**1b.** Take inputs from a user and add them in a dictionary called `my_user_dict`

Here is the example of an user input:

SSN: 111-222-3333

Name: Steve Hawkins

The code continue to take user input and provide an option at the end of the user input; "Do you want to continue (Y/N)"

Identify how many keys you need to create a dictionary.

**Restrictions: Do not use functions and/or exceptions in this exercise**

```
my_dict= {
    "clouds": "white",
    "sky": "blue",
    "asphalt": "black",
    "apple": "red",
    "banana": "yellow",
    "grape": "purple",
    "grass": "green",
    "snow": "white",
    "lemon": "yellow",
    "coffee": "brown"
}

print(my_dict)

my_user_dict = {}

continue_input = "Y"

while continue_input == "Y":

    user_input = input("Enter key and value (format key: value): ")

    parts = user_input.split(":")

    key = parts[0].strip()
    value = parts[1].strip()

    my_user_dict[key] = value

    continue_input = input("Do you want to continue (Y/N)? ").upper()

print("Final dictionary:", my_user_dict)

```

**Converting tuples into a dictionary**

```
List of tuples where each tuple represents a key-value pair

a = [("a", 1), ("b", 2), ("c", 3)]

# Convert the list of tuples into a dictionary

res = dict(a)

print(res)
```

```
{'a': 1, 'b': 2, 'c': 3}
```

**1c.** Based on the given tuple, create a code which checks for valid key & value pairs, and check for key duplication.

The code should provide assistance to a user to correct the error. For key duplication, ask user to change the key

**Restrictions: Do not use functions and/or exceptions in this exercise**

```
[('Name', 'Sarah Connor'),
 ('Date of birth', '1 Jan 1980'),
 ('Address', '1000 Black Mountain Drive', 92126),
 ('Name', 'Jim Hawkins')]
```

**1d.** Convert the following list into a dictionary. Automate the process by using the loop.

**Restrictions: Do not use functions and/or exceptions in this exercise**

**1e.** Use the following text and count the number of words using dictionary. Remember The or the counts as 2.

**The tiger (Panthera tigris) is a large cat and a member of the genus Panthera native to Asia. It has a powerful, muscular body with a large head and paws, a long tail and orange fur with black, mostly vertical stripes. It is traditionally classified into nine recent subspecies, though some recognise only two subspecies, mainland Asian tigers and the island tigers of the Sunda Islands.**

## 2. Troubleshooting

```
d_orig = {123:"Coconut"}
d_copy = d_orig
print(d_orig)
print(d_copy)
```

```
{123: 'Coconut'}
{123: 'Coconut'}
```

**2a.** Change the content of `d_copy` and make sure the content does not affect the `d_orig` dictionary. Verify using the code.

```
# Write your code here
```

**2b.** If it changes the content of the original dictionary, then propose how can you solve this problem.

```
# Write your code here
```

**2c.** Write a code that generates the following error and explain why there is such an error.

```
TypeError: unhashable type: 'list'
```

```
# Write your code here
```

## Challenges

Please describe the challenges you faced during the exercise.

```python
# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

```

**End of exercise**
