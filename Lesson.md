Lesson: Introduction to Functions in Python

In this lesson, we will learn the basics of using functions in Python to write cleaner, more organized, and reusable code. Functions are blocks of code that can be defined and called by name. They can accept inputs (called arguments) and return a value as output.

Why use functions?

Code reusability: Functions allow you to write code once and reuse it multiple times, reducing repetition and making your code easier to maintain.
Code organization: Functions help you break down your code into smaller, more manageable pieces, making it easier to understand and debug.
Easier collaboration: Functions make it easier for others to understand your code and work with it, as each function serves a specific purpose.
Defining a function

To define a function in Python, use the def keyword followed by the function name, a pair of parentheses, and a colon. The function body should be indented. Here's an example of a simple function that adds two numbers:

```
def add(a, b):
    result = a + b
    return result
```

Calling a function

To call a function, use the function name followed by a pair of parentheses with the arguments inside. Here's an example of how to call the add function we defined earlier:

```
sum = add(3, 4)
print(sum)  # Output: 7
```

Exercise: Refactoring code to use functions

In this exercise, we will refactor a simple program that calculates the area of a rectangle and a circle, to use functions instead of a single block of code.

Original code:

```
length = float(input("Enter the length of the rectangle: "))
width = float(input("Enter the width of the rectangle: "))
rectangle_area = length * width
print(f"The area of the rectangle is {rectangle_area}")

radius = float(input("Enter the radius of the circle: "))
circle_area = 3.14159 * (radius ** 2)
print(f"The area of the circle is {circle_area}")
```

Refactored code using functions:

```
def get_float_input(prompt):
    return float(input(prompt))

def calculate_rectangle_area(length, width):
    return length * width

def calculate_circle_area(radius):
    return 3.14159 * (radius ** 2)

def main():
    length = get_float_input("Enter the length of the rectangle: ")
    width = get_float_input("Enter the width of the rectangle: ")
    rectangle_area = calculate_rectangle_area(length, width)
    print(f"The area of the rectangle is {rectangle_area}")

    radius = get_float_input("Enter the radius of the circle: ")
    circle_area = calculate_circle_area(radius)
    print(f"The area of the circle is {circle_area}")

if __name__ == "__main__":
    main()
```


In the refactored code, we created functions for getting user input, calculating the area of a rectangle, and calculating the area of a circle. This makes the code more organized and easier to understand.

Practice

Now, try writing a program that converts temperatures between Celsius and Fahrenheit, using functions for input, calculation, and output. Remember to keep your functions small and focused on a specific task.

As you become more comfortable with functions, you will find that your code becomes more organized, easier to understand, and easier to maintain. Functions are an essential tool for any Python programmer, so practice using them often!
