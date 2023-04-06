In this lesson, we will learn about while loops in Python, which are used to repeatedly execute a block of code as long as a given condition is True. We will cover the basic syntax and how to use while loops in various scenarios.

1) Basic syntax of a while loop:

```
while condition:
    # code to execute
```

2) Using a while loop to count down from a given number:

```
countdown = 10
while countdown > 0:
    print(countdown)
    countdown -= 1
```

3) Using a while loop to validate user input:

```
user_input = int(input("Enter a number between 1 and 10: "))
while user_input not in range(1, 11):
    user_input = int(input("Invalid input. Please enter a number between 1 and 10: "))
print("Valid input!")
```

4) Exercise: Write a program that generates the Fibonacci sequence up to a specified number using a while loop.
