#Problem-Solving 

a.
```python
number_1= int(input("enter your 1st number:"))
number_2= int(input("enter your 2nd number:"))
number_3= int(input("enter your 3rd number:" ))

if number_1>number_2 and number_1>number_3:
    print("number 1 is the largest number")

if number_2>number_3 and number_2>number_1:
    print("number 2 is the largest number")
if number_3>number_1 and number_3>number_2:
    print("number 3 is the largest number")
```
b.
```python
#Approach 1
if int(input("Enter a number: "))%2==0:
    print("Even")
else:
    print("Odd")

#Since % only gives the remainder, if there is no remainder then the number is even
#Approach 2
if int(input("Enter a number: "))%2>0:
    print("odd")
else:
    print("even")

"""Similar to approach 1, if you use mudolo and there is a remainder then the number
odd because all remainders will be greater than 0
"""

#Approach 3
my_var = int(input("Enter a number: "))
if (my_var/2) == int(my_var/2):
    print("even")
else:
    print("odd")

"""if you divide the number entered by the user by 2 and the result is an integer, than the number is even but if the
resulting data type is not an integer because it has a decimal value than the number is odd"""
```
