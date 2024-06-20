[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15303561&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

### Python Basics: ###
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is an interpreted, object-oriented, high-level programming language with dynamic semantics

Python features
   - Simple and readable syntax: Python's syntax is clear and easy to understand.
   - Interpreted: Python is an interpreted language, which means that you don't need to compile the code before running it, making the development process faster.
   - Versatility: It can be used for web development, data science, machine learning, automation, scripting, and more.
   - Extensive Libraries: It has a vast collection of pre-written code (libraries) for various tasks, saving development time for example django and flask
   - Cross-platform: Python code can run on multiple operating systems (Windows, macOS, Linux) without any modifications.
   Can be handled in a procedural, object-oriented, or functional way

Python Use Cases

- Web development: Using frameworks like Django and Flask.
- Data science and analytics: Utilizing libraries like Pandas, NumPy, and Matplotlib.
- Machine learning and AI: Implementing models with TensorFlow, Keras, and scikit-learn.
- Automation and scripting: Writing scripts to automate repetitive tasks.
- Scientific computing: Conducting research with SciPy and SymPy.
- Game Development: Python's PyGame library allows developers to create simple to complex games.



### Installing Python: ###
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

1. Step 1: Download Python
   - Go to the Python downloads page.https://www.python.org/downloads/
   - Click on the "Download Python" button.

2. Step 2: Run the Installer
   - Open the downloaded installer file.
   - Check the box that says "Add Python to PATH".
   - Click "Install Now".

3. Step 3: Verify Installation
   - Open Command Prompt.
   - Type [python --version] and press Enter. You should see the Python version that you installed.

4. Step 4:Setting up a virtual environment:
   - Create a new folder for your project. For example, if you want to create a project named "myproject", you can create a new folder named "myproject".
   - Navigate to your project directory.
   - Run the following command to create a virtual environment:
      - python -m venv myproject
   - Activate the virtual environment:
      - \env\Scripts\activate



### Python Syntax and Semantics: ###
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

A simple Python program that prints "Hello, World!" to the console:

```python
print("Hello, World!")
```
   - print(): Built-in function to display the output(contents in the parentheses) on the console.
   - "Hello, World!" is a string enclosed in double quotes or you can also use single quotes



### Data Types and Variables: ###
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   - Integers(int): which are are whole numbers
   - Float:this are floating numbers or numbers with decimal places
   - boolean (bool): This are value which display if something is true or False(logical values)
   - Strings(str):this are strings or values of text and are shown with double quotes
   - Tuples:this are ordered and immutable(cannot be changed) collections of items
   - dict(dictionaries):Unordered collections of key-value pairs.
   - set: Unordered collections of unique elements.
   - list: Ordered, mutable collections.


```python
# Integer
x = 10
print(W, type(W))

# Float
y = 4.234
print(y, type(y))

# String
name = "john thiongo"
print(name, type(name))

# Boolean
is_student = True
print(is_student, type(is_student))

# List
numbers = [1, 2, 3, 4, 5]
print(numbers, type(numbers))

# Tuple
coordinates = (20.0, 30.0)
print(coordinates, type(coordinates))

# Dictionary
person = {"name": "Thiongo", "age": 22}
print(person, type(person))

# Set
unique_numbers = {1, 2, 3, 3, 4}
print(unique_numbers, type(unique_numbers))

```



### Control Structures: ###
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

Control statements direct the flow of a Python program's execution. They introduce logic, decision-making, and looping. Key control statements in Python include if/else, for/while, break/continue, and pass.

conditional statements(if-else)

```python
age = 18

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")

```

in the above In if-else code, the code checks the value of the age variable. If the age is greater than or equal to 18, it prints "You are an adult." Otherwise, it will print "You are a minor.

Loops (for):

```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(f"I like {fruit}s.")
```

in this example the loop iterates over each item in the fruits list, and for each fruit, it prints a statement like "I like apples."



### Functions in Python: ###
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions in Python are reusable blocks of code that perform a specific task. They help in organizing code, promoting code reuse, and making it more readable and maintainable.

```python
def add(a, b):
    return a + b

# Calling the function
result = add(3, 5)
print(result)  # Output: 8
```

- def add(x, y):: Defines a function named add that takes two arguments, x and y.
- return x + y: Calculates the sum and returns the result.
- result = add(5, 3): Calls the add function with arguments 5 and 3, storing the returned value in the result.




### Lists and Dictionaries: ###
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

- Lists: Ordered, mutable collections of items. Can be accessed by index (starting from 0).
- Dictionaries: Unordered, mutable collections of key-value pairs. Accessed using keys.

```python
numbers = [1, 2, 3, 4]
print(numbers[1])  # Access second element (index 1)

# Modifying a list element
numbers[2] = 10

# Operations on lists
numbers.append(5)  # Adds element to the end of the list
numbers.remove(2)  # Remove the first sight of 2

people = {"name": "Thiongo", "age": 35}
print(people["name"])  # Access Index using key "name"

# Modifying a dictionary value
people["age"] = 40

# Operations on dictionaries
people["city"] = "New York"  # Add a new key-value pair
del people["age"]  # Remove the key-value pair with key "age"

```



### Exception Handling: ###
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

- When an error occurs or an exception python tries to normally stop the error and generate an error message
- using try, except, and finally blocks.

```python
try:
    # Code that might raise an exception
    result = 10 / 0  # Division by zero (exception)
except ZeroDivisionError:
    print("Division by zero is not allowed!")
finally:
    # Code that always executes, regardless of exceptions
    print("This code always executes.")

```

Explanation:
   - try block: Contains code that might raise an exception.
   - except block (which is optional): Handles specific exceptions (e.g., ZeroDivisionError here).
   - finally block (also optional): Code that always executes, even if no exception occurs or after an exception is handled.



### Modules and Packages: ###
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Modules are files containing Python code, while packages are directories containing multiple modules.

```python
import math

# Using a function from the math module
result = math.sqrt(16)
print(result)  # Output: 4.0
```



### File I/O: ###
   - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Python has several functions for creating,reading,updating, and deleting files

The The open() function takes two parameters; filename, and mode.

- "r" - Read - Default value. Opens a file for reading, error if the file does not exist
- "a" - Append - Opens a file for appending, creates the file if it does not exist
- "w" - Write - Opens a file for writing, creates the file if it does not exist
- "x" - Create - Creates the specified file, returns an error if the file exists

Reading from a file:

```python
# Reading from a file
with open("example.txt", "r") as file:
    content = file.read()
    print(content)

```

Writing to a file:

```python
# Writing to a file
lines = ["Hello, World!", "Python is great!"]
with open("output.txt", "w") as file:
    for line in lines:
        file.write(line + "\n")

```

### Sourses/references  ###

1. The official Python documentation (https://docs.python.org/)

2. https://www.datacamp.com/

3. https://www.w3schools.com/python/

4. https://www.tutorialspoint.com/python/index.html

5. https://stackoverflow.com





# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


