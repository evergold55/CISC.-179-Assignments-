# User input using input() function

## Objective

Understand how ```input()``` function is applied.

## Prerequisite

- Python literals
- Variables

## What do you need to complete this exercise?

- Please follow my video tutorial [installing Python and PyCharm CE on Windows](https://youtu.be/nFN0JW43GKY). Note: The version you see may differ slightly from what is shown in the video.
- Use the PyCharm IDE to write and compile your code. Submit your responses in a Markdown file on GitHub. Ensure that all code included in the Markdown file runs without errors. Refer to [Submitting Your Assignment Using GitHub](https://sdccd-edu.zoom.us/rec/share/F4rK6ZABMXlRn4aGlZ9P005e-iRKwq8rr9KuawDoJ77TdkybKU2tpf4l4QSe113g.ut4jpVaqaPY0oI7b?startTime=1725121532000) for detailed instructions.


### 1. User input
a. Write a program that prompts the user to enter the weight of a person in kilograms and outputs the equivalent weight in pounds. (Note that 1 kilogram = 2.2 pounds).
```python
kilograms = float(input("Enter the weight in kilograms: "))
pounds = kilograms * 2.2
print(f"The equivalent weight in pounds is: {pounds} lbs")
```

b. Interest on a credit card's unpaid balance is calculated using the average daily balance. Suppose that $netBalance$ is the balance shown in the bill, $payment$ is the payment made, $d1$ is the number of days in the billing cycle, and $d2$ is the number of days payment is made before biling cycle. Then, the average daily balance is: $$averageDailybalance = (netBalance \times d1 - payment \times d2)/d1$$. If the interest rate per month is, say, 0.0152, then the interest on the unpaid balance is: $interest = averageDailyBalance \times 0.0152$ Write a program that accepts as input $netBalance$, $payment$, $d1$, $d2$, and $interest rate per month$. The program outputs the interest.
```python
netBalance = float(input("Enter the net balance: "))
payment = float(input("Enter the payment made: "))
d1 = int(input("Enter the number of days in the billing cycle: "))
d2 = int(input("Enter the number of days payment is made before the billing cycle: "))
interestRatePerMonth = float(input("Enter the interest rate per month: "))
averageDailyBalance = (netBalance * d1 - payment * d2) / d1
interest = averageDailyBalance * interestRatePerMonth
print(f"The interest on the unpaid balance is: ${interest:.02f}")
```

c. Two cars A and B leave an intersection at the same time. Car A travels west at an average speed of x miles per hour and car B travels south at an average speed of y miles per hour. Write a program that prompts the user to enter the average speed of both the cars and the elapsed time (in hours and minutes) and outputs the (shortest) distance between the cars.

```python
import math

x = float(input("Speed of car A (west): "))
y = float(input("Speed of car B (south): "))

hrs = int(input("Hours: "))
mins = int(input("Minutes: "))

t = hrs + mins / 60

distA = x * t
distB = y * t

dist = math.sqrt(distA**2 + distB**2)

print("Distance between cars =", round(dist, 2), "miles")
```
### 2. Troubleshooting

Please troubleshoot the following issue without using Python, and explain your reasoning.

```python
a. hello = "hello"
hello is not a reserved keyword, so it can be used
b. _var = 100
Underscore is a valid character 
c. !var_1 = 200

d. print = "print me"
Print is a reserved word and cannot be used 
e. False = 0
False is a reserved word and cannot be used 
```

## Challenges

Please describe the challenges you faced during the exercise.

```python

# improper syntax usage

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

```

**End of exercise**



