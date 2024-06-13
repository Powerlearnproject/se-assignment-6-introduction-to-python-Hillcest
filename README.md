[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15269154&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
  
   - Python is a programming language mostly preferred by developers because of it's simplicity and the ability to be easily read and interpreted by the developers.
   - Python is effective in web based programming for example via frameworks like flask and Django. I personally use Python Flask for web development and I can comment that it is a good one as it is simple to write the backend that interacts well with the frontend.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   - To install Python, we head to https://www.python.org/downloads/ and install the preferred version.
   - We can verify if python is installed by typing in the command prompt python --version. If we see a python version number, then python is successfully installed in our machine.
  
   - To set up a virtual environment, we first ensure pip is installed in our machine by typing pip --version in our cmd.
   - We the install a virtual environment by typing pip install virtualenv in the cmd.
   - We then create a virtual environment by typing virtualenv "a preferred name"
   - Lastly we activate the virtualenv by typing "the virtual_env_name"/Scripts/activate
   - 

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   - print('Hello, World!')
   - Print() is a built in function in python that outputs the passed argument to the console. We enclose the argument in quotations either single or double to show the exact string to output.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   - String str e.g. "Hello World!"
   - Integers int for example 1,2,3,4
   - Float e.g. 3.14, 2.33
   - Boolean i.e. 'true' or 'false'
   - List e.g. ['apples', 'bananas', 'strawberry']
   - Dictionary e.g. {"name": 'Peter' , "age": '20'}

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
  
   - The use of conditional statements in python enables a certain block of code to be executed only when certain conditio(s) are met. This enables the code to do multiple operations based on different conditions as it will know what to do.
   - An example of if-else statement in python:
num1 = 34
if num1 < 0:
  print("this is a negative number")
else:
  print("This is a positive number")

A loop allows for the iteration in a list, dictionary or tuple and render the individual objects in them. This enables the reduction of repetition and it makes the code simple and easy to understand.

fruits = ["apple", "banana", "strawberry", "guava"]
for fruit in fruits:
  print(fruit)

  
example of a for loop

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
  
   - A function is a block of code that performs a specific task and returns an output that can be used somewhere else in the code.
   - An example:
  
     def add(x,y):
      sum = x + y
     return sum

     result = add(3,4)
     print(result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
  
   - List is an ordered collection of items whose items can be accessed by their index. They are created using square brackets i.e. numbers = [1,2,3,4,5]
   - Dictionaries are unordered collection of key-value pairs where values are accessed by their key.They are created using curly braces.

numbers = [1, 2, 3, 4, 5]

print("List of numbers:", numbers)
print("First number in the list:", numbers[0])
numbers.append(6)
print("List after adding an element:", numbers)
numbers.remove(3)
print("List after removing an element:", numbers)



person = {'name': 'Peter', 'age': 20, 'city': 'Nakuru'}
print("Dictionary:", person)
print("Name:", person['name'])
person['age'] = 26
print("Dictionary after updating age:", person)
person['country'] = 'USA'
print("Dictionary after adding a new key-value pair:", person)
del person['city']
print("Dictionary after deleting a key-value pair:", person)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   - Exception handling basically is the way we handle the errors that migh occur in our code. It is always necessary to handle them well to ensure continous use of the system without unexpected failures.
      An example of try except is:
     try:
       result = 10/0
     except Exception as e:
       print("A number cannot be divided by zero")

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   - A single file (or files) containing Python code that can be imported and used in other scripts.
   - To import a module, we use the format import "module_name"
     example:
     import math

     print("This is the square root of 5: " math.sqrt(20))

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
   
  Reading from a file:
  
Open the file in read mode, use read() or readlines() to read the content, and then close the file.

Writing to a file:
Open the file in write mode, use write() or writelines() to write content to the file, and then close the file.

try:
    with open('example.txt', 'r') as file:
        content = file.read()
        print("File content:")
        print(content)
except FileNotFoundError:
    print("The file does not exist.")

lines = ["Hello, World!", "This is a test.", "Writing to a file in Python."]
with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + '\n')
print("Content written to output.txt")

   

      References: https://youtu.be/kqtD5dpn9C8?si=6fKV8G4Ph4IuGB8x

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


