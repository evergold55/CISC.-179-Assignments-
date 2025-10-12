# 1. While Loop
a.)
```python
n0= 112
while n0>0:
    n0= int(n0/2)
    print(n0)

"""Result:
56
28
14
7
3
1
0
"""
```
b.)
```python
n0= 112
while n0>0:
    n0= n0/2
    print(n0)
```

c.)
```python
while True:
    number1=int(input("What is your first number: "))
    number2=int(input("What is your second number: "))
    op=input("what arithmetic operation would you like to perform: ")
    if op=="+":
       print(number1+number2)
    elif op=="-":
        print(number1-number2)
    elif op=="*":
        print(number1*number2)
    elif op=="/":
        print(number1/number2)
    else:
        print("Invalid operation")
    print("would you like to continue? (y/n)")
    choice=input()
    if choice=="y":
        continue
    else:
        break
print("Have a good day.")
```
# 2. For Loops
```python
word=str(input("Enter a word: "))
print(f"Your text has:", {len(word)}, "letters")
counted = []

for ch in word:
    if ch not in counted:
        occurrences = word.count(ch)
        print(f"{ch} = {occurrences}")
        counted.append(ch)
```



