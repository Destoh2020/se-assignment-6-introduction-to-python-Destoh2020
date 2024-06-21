[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15310031&assignment_repo_type=AssignmentRepo)

# SE-Assignment-6

Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

Questions:

1. Python Basics:

   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
     Python is an interpreted, obejct-oriented, high-level programming langauge with dynamic semantics.

   Features that make more popular among developers include;
   i. Simple and readable syntax
   ii. Versatile and flexible.
   iii. Rich standard library.
   iv. Third party libraries and frameworks
   v. It is cross platform
   vi. It is interpreted and interactive
   vii. Community support.
   Python is used in;
   i. Web development - frameworks like django and flask are widely used for building web application APIs.
   ii. Data Analysis and Visualization - Libraries such as pandas, numpy and matplotlib make it the beat choice for data scientist and analysts.
   iii. Machine Learning and AI - Libraries like tensorflow, pytorch and scikit-learn are instrumental in developing machine learning models, neural networks amd deep learning algorithms.
   iv. Scientific computing - python is used in scientific computing for simulations, numerical analysis and complex mathematical problems.
   v. Education - its simplicity and readabiity make it the popular choice for teaching programming to begginers and in educational settings.
   vi. Game development - python along with framework leike Pygame can be used to develop 2D games and prototypes.

2. Installing Python:

   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
     To install python on windows
     i. Go to the official Python website and download the latest version of Python for Windows.
     ii. Choose either the Windows Installer (.exe file) or Windows x86-64 executable installer for 64-bit systems.
     iii. Once the download completes, double-click the downloaded installer (.exe file).
     iv. Check the box that says "Add Python x.x to PATH" during the installation process. This ensures Python is added to the system PATH, making it easier to run Python from the command line.
     v. Click "Install Now" and follow the prompts to complete the installation.
     To verify the installation
     i. Press Win + R, type cmd, and press Enter to open Command Prompt or open powershell terminal an run it as administrator.
     ii. Type python --version or python -V and press Enter.
     iii. You should see the installed Python version displayed (e.g., Python 3.12.1).
     To set up virtual enviroment
     i. Open Command Prompt if not already open.
     ii. Run the following command to install virtualenv using pip "pip install virtualenv"
     iii. Navigate to your project directory in Command Prompt
     iv. Run the following command to create a virtual environment named pythonvenv (you can replace pythonvenv with any name you prefer) "python -m pythonvenv venv"
     v. To activate the virtual environment, run "pythonvenv\Scripts\activate"
     vi. Your Command Prompt prompt will change to indicate the virtual environment is active, e.g., (pythonvenv) C:\path\to\your\project>.
     vii. While the virtual environment is active, you can install packages using pip as usual "pip install package_name" replace package_name with the name of the package you want to install (e.g pip install flask).

3. Python Syntax and Semantics:

   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
     {
     ```python
     #simple python program
     print("Hello, Python developers")
     ```
     }
     '#' symbol is used to show that the line is a comment and it is ignored during execution comments is used to describe the code for future reference or for others to understannd your code.
     The 'print' function in python is used to output to the console.
     it can accept one or more expressions enclosed in parentheses '()' sepearted by commas ','. The "" are used to signify that the text is a string.

4. Data Types and Variables:

   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
     The basic data types in python are;

   1. Integers ('int') - represent whole numbers
      ```python
      age = 30
      print(f"Age: {age} \n Type: {tpye(age)})
      ```
   2. Float ('float') - represent real numbers with decccimal points.
      ```python
      pi = 3.14159
      print(f"PI: {pi} \n Type: {tpye(pi)})
      ```
   3. string ('str') - represent sequence of characters enclosed within single or double quotes
      ```python
      name = "Desterian"
      print(f"Name: {name} \n Type: {tpye(name)})
      ```
   4. Boolean ('bool') - represent a boolean value which can be either 'True' or 'False'
      ```python
      is_loggedin = false
      print(f"isLoggediIn: {is_loggedin} \n Type: {tpye(isloggedin)})
      ```
   5. List - represent an ordered collection of items which can be of different data types enclosed in sqaure brackets '[]'. Separated by comas.
      ```python
      fruits = ['mangoes', 'oranges', 'pineapple']
      print(f"Fruits: {fruits} \n Type: {tpye(fruits)})
      ```
   6. Tuple - epresent an ordered collection of items which can be of different data types enclosed in parentheses '()' but they are immutable (can not be changed after creation.)
      ```python
      coordinates = (20, 45)
      print(f"Coordinate: {coordinates} \n Type: {tpye(coordinates)})
      ```
   7. Dictionary - represent a collection of key-value pairs.
      keys are unique and immutable, values can be of any data type. they are enclosed in in culr braces '{}' with key value pairs separated by colons ':'
      ```python
      person = {'name': 'Bob', 'age': 30, 'city': 'London'}
      print(f"Person: {person} \n Type: {type(person)}")
      ```

5. Control Structures:

   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
     Conditional statements are an essential part of programming in Python. They allow you to make decisions based on the values of variables or the result of comparisons.
     Example of if-else statement: Checking if someone is eligible to vote;

     ```python
      age = int(input("Enter your age: "))
      if age >= 18:
         print("You are eligible to vote.")
     else:
         print("You are not eligible to vote.")
     ```

     Example of a for loop: Printing from a list;

     ```python
     fruits = ["apple", "banana", "cherry"]
     for x in fruits:
      print(x)
     ```

6. Functions in Python:

   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

     - functions are blocks of code that perform a specific task when invoked.
       They are useful in;
       i. Modularity: Functions allow you to break down your program into smaller, manageable parts. Each function can focus on a specific task, enhancing code readability and maintainability.
       ii. Code Reusability: Once defined, functions can be called multiple times from different parts of the program without rewriting the same code, promoting efficient coding practices.
       iii. Abstraction: Functions hide the implementation details of their code block, allowing you to use them without needing to understand how they work internally. This simplifies the overall complexity of the program.
       iv. Parameter Passing: Functions can accept parameters (inputs) which enable them to work with different data each time they are called, making them versatile and adaptable.
       Function that takes two numbers and returns the sum:

     ```python
     def sum_two_numbers (num1, num2):
        return num1 + num2
     ```

   To call the function assign it to a variable lets call it result;

   result = sum_two_numbers(10,45)
   print(result)

7. Lists and Dictionaries:

   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   1. Lists in Python are ordered collections of items. They can contain elements of different data types, and elements are accessed by their position (index) in the list while Dictionaries in Python are unordered collections of key-value pairs. They associate each key with a value, allowing for efficient look-up of values based on keys.
   2. Lists are enclosed in square brackets [], and elements are separated by commas ',' while Dictionaries are enclosed in curly braces {}, and key-value pairs are separated by commas ,, with keys and values separated by colons :.
   3. Elements in a list are accessed using zero-based indexing (numbers[0] accesses the first element) while Elements in a dictionary are accessed using keys e.g (person['name'] accesses the value 'Alice'). if the name is 'Alice.
   4. Lists are mutable, meaning you can change, add, or remove elements after the list is created while Dictionaries are mutable, allowing for modification of values associated with existing keys and addition/removal of key-value pairs.

   ```python
      # Creating a list of numbers
      numbers = [1, 2, 3, 4, 5]

      # Creating a dictionary of person's information
      person = {'name': 'Alice', 'age': 30, 'city': 'New York'}

      # Printing the initial list and dictionary
      print("Initial List of Numbers:", numbers)
      print("Initial Dictionary of Person:", person)
      print()

      # Basic operations on list
      print("Basic Operations on List:")
      # Accessing elements
      print("First element of list:", numbers[0])
      # Appending an element
      numbers.append(6)
      print("List after appending 6:", numbers)
      # Removing an element
      numbers.remove(3)
      print("List after removing 3:", numbers)
      print()

      # Basic operations on dictionary
      print("Basic Operations on Dictionary:")
      # Accessing elements
      print("Name of the person:", person['name'])
      # Adding a new key-value pair
      person['gender'] = 'Female'
      print("Dictionary after adding gender:", person)
      # Updating an existing value
      person['age'] = 31
      print("Dictionary after updating age:", person)
      # Removing a key-value pair
      del person['city']
      print("Dictionary after removing city:", person)
      print()

      # Printing final list and dictionary
      print("Final List of Numbers:", numbers)
      print("Final Dictionary of Person:", person)
   ```

8. Exception Handling:

   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
     - Exception handling in is a way to manage errors that occur during program execution. Instead of terminating the program abruptly, exception handling allows the program to continue running or handle the error gracefully.

   ```python
   def divide_numbers(a, b):
      try:
         result = a / b
      except ZeroDivisionError:
         print("Error: Division by zero is not allowed.")
         result = None
      except TypeError:
         print("Error: Invalid input type. Please provide numbers.")
         result = None
      else:
         print(f"The result of dividing {a} by {b} is {result}.")
      finally:
         print("Execution of the divide_numbers function is complete.")
      return result

   # Test cases
   print(divide_numbers(10, 2))  # Output: The result of dividing 10 by 2 is 5.0.
   print(divide_numbers(5, 0))   # Output: Error: Division by zero is not allowed.
   print(divide_numbers(8, 'a')) # Output: Error: Invalid input type. Please provide numbers.
   ```

9. Modules and Packages:

   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
     - Modules in are files containing Python code that define functions, classes, and variables. They allow you to logically organize your Python code and reuse it across multiple scripts or projects.
     - Packages are directories that contain multiple Python module files along with an **init**.py file, which can be empty or contain initialization code for the package.
     - To import and use a module in your script, you can use the import statement. as shown in the example below;

```python
         # Importing the math module
         import math

         # Using math.sqrt() to calculate the square root of a number
         num = 25
         sqrt_num = math.sqrt(num)

         # Using math.pi to get the value of pi
         pi_value = math.pi

         # Using math.sin() to calculate the sine of an angle (in radians)
         angle_in_radians = math.radians(90)  # Convert 90 degrees to radians
         sin_value = math.sin(angle_in_radians)

         # Printing the results
         print(f"The square root of {num} is: {sqrt_num}")
         print(f"The value of pi is: {pi_value}")
         print(f"The sine of 90 degrees is: {sin_value}")
```

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
      - To read the contents of a file, you use the open() function with the mode 'r' (read mode). You can then use methods like read(), readline(), or readlines() to read the file's content.

```python
         # Script to read the content of a file and print it to the console

         # Open the file in read mode
         with open('example.txt', 'r') as file:
            # Read the entire content of the file
            content = file.read()

         # Print the content
         print(content)
```

      - To write to a file, you use the open() function with the mode 'w' (write mode) or 'a' (append mode). You can then use the write() method to write strings to the file.

```python
            # Script to write a list of strings to a file

            # List of strings to write to the file
            lines = [
               "Hello, world!",
               "Python is a great programming language.",
               "File handling is easy with Python."
            ]

            # Open the file in write mode
            with open('output.txt', 'w') as file:
               # Write each string to the file
               for line in lines:
                  file.write(line + '\n')  # Add a newline character after each string

            print("Content written to output.txt")
```

# Submission Guidelines:

- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
