## Create a unit conversion program using functions


**1a.** The user selects kilometers per liter (kpl), and the response will be provided in miles per gallon (mpg). The units must be interchangeable, so the program will ask the user whether to convert from kpl to mpg or vice versa.

The program will prompt the user for input and deliver output with the appropriate units.

Additionally, the program will include input validation. For example, it will not accept letter inputs and will provide an error message to the user when invalid input is detected.

The function will also allow multiple arguments, enabling the user to convert multiple values at once.

Research and find out the conversion factor between the units.

```python
fuel_econ= input("Would you like to convert fuel econ to from mpg(miles per gallon) to kpl (kilometers per liter)? Or, \n"
                 "Would you like to convert fuel econ to from kpl (kilometers per liter) to mpg(miles per gallon)? (kpl/mpg): ")
if fuel_econ != "kpl" or "mpg":
    print("Improper entry; please enter kpl or mpg")
def kpl2mpg():
    fuel_econ_kpl = float(input("enter the fuel econ in kpl (kilometers per liter): "))
    kpl_to_mpg = fuel_econ_kpl * 2.352
    print("fuel econ in mpg: ", kpl_to_mpg )

def mpg2kpl():
    fuel_econ_mpg = float(input("enter the fuel econ in mpg: "))
    mpg_to_kpl = fuel_econ_mpg / 2.352
    print("fuel econ in kpl: ", mpg_to_kpl )

if fuel_econ == "kpl":
    print(mpg2kpl())
elif fuel_econ == "mpg":
    print(kpl2mpg())
```


**1b.** How would you write a function that could take any number of unnamed arguments and print their values out in reverse order?

```python
def list_reverser():
    user_list = input("Enter your list items separated by space: ").split()
    user_list.reverse()
    return user_list

print(list_reverser())
```

**1c.** What would be the result of changing a list or dictionary that was passed into a function as a parameter value? Which operations would be likely to create changes that would be visible outside the function? What steps might you take to minimize that risk?

  Would this be an acceptable answer:It would change that list/dictionary inside and outside the function because list and dictionaries are mutable data types. List operations that are used to mutate the list such as 'remove' or 'append' will be visible outside the function and dictionary operations such as 'pop' will be visible outside the function. Avoiding mutating parameters or using immutable data types is the best way to avoid making any accidental changes.
  ```python
fruits = ["apple", "banana", "blueberry"]
fruits_dict = {"apple":"red", "banana":"yellow", "blueberry":"blue"}

def fresh_fruits():
    print(fruits, fruits_dict)
    fruits.append("apple")
    fruits_dict["apple"] = "blue"
    print(fruits, fruits_dict)
"""result= ['apple', 'banana', 'blueberry'] {'apple': 'red', 'banana': 'yellow', 'blueberry': 'blue'}
['apple', 'banana', 'blueberry', 'apple'] {'apple': 'blue', 'banana': 'yellow', 'blueberry': 'blue'}"""
```




Explain the above statements with the help of code.

**1d.** Assuming that `x = 5`, what will be the value of `x` after `funct_1()` below executes? After `funct_2()` executes?

```python
x = 5
def funct_1():
  x=3

def funct_2():
  global x
  x=2
```
x will be = 5 after executing funct_1 because x=3 is a local variable and x=2 after funct_2 because x=2 gets declared globally.

## 2. Troubleshooting

Correct the following code. There might be more than one correct answers. Explain your reasoning.

```python
def my_func(a,b,**c):
  print(c)

my_func(1,2,3,4,5,6)

result

def my_func(a,b, **c):
  print(c)

my_func(1,2,c=3,d=4,e=5,f=6)
print()
```

Using the following code, x should print 100 but it prints 10, why?

```python
def my_func_global():
  x = 100

global x
x = 10
my_func_global()
print(x)
```

printing 'x' outputs 10 because it was declared as global.

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
