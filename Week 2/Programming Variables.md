#Variable memory usage

```python
var1 = 10

#Memory address for var1=10
print(hex(id(var1)))

var1=100

#Memory address for var1=100
print(hex(id(var1)))
```
The Python interpreter assigned a new address to var1. There are two different addresses because the integers are different and therefore reside within different blocks of memory. The first memory location still exists because that object still exists in memory and can be reused if another variable gets assigned to it. 

```python
var2=100
print(hex(id(var2)))
```
The addresses for var1 and var2 are the same because they refer to the same object. 

#Memory Map

```python
str1='hello'
str2='world'

print(hex(id(str1[0]))), print(hex(id(str1[1]))), print(hex(id(str1[3]))), print(hex(id(str1[4])))



print(hex(id(str2[0]))), print(hex(id(str2[1]))), print(hex(id(str2[3]))), print(hex(id(str2[4])))
```

| Address in hexadecimal | Char |
| ---------------------- | ---- |
| #0x103f7a740           |  H   |
| #0x103f7a6b0           |  e   |
| #0x1023ae800           |  l   |
| #0x1023ae890           |  o   |
| #0x1023aea10           |  w   |
| #0x1034be920           |  r   |
| #0x1034be680           |  d   |


#Troubleshooting 
a. hello = "hello" 

valid

b. _var = 100 
valid

c. !var_1 = 200 
Cannot use ! as a character in the name of a variable

d. print = "print me" 
print is a reserved word and cannot be used as a variable name. 

e. False = 0
cannot use false as a variable name, because it is a keyword
