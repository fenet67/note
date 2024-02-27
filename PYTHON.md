# PYTHON

# Python

Python is a high-level, interpreted programming language known for its simplicity and readability. It is widely used for various applications, including web development, data analysis, artificial intelligence, and automation.

### Variables and Data Types

In Python, variables are used to store data. They can hold different types of values, such as strings, numbers, lists, tuples, sets, and dictionaries.

- Strings: A sequence of characters, enclosed in single or double quotes. Example: `first_name = 'hanna'`
- Numbers: Integers (`int`) or floating-point numbers (`float`). Example: `age = 24`
- Lists: Ordered collections of items, enclosed in square brackets. Example: `student_list = ['hanna', 'beki', 'laura', 'tom']`
- Tuples: Immutable collections of items, enclosed in parentheses. Example: `names = ('hanna', 'tomi')`
- Sets: Unordered collections of unique items, enclosed in curly braces. Example: `stu_info = {'name': 'hanna', 'age': 55, 'sec': 'B', 'height': 1.3}`
- Dictionaries: Key-value pairs, enclosed in curly braces. Example: `stu_info = {'name': 'hanna', 'age': 55, 'sec': 'B', 'height': 1.3}`

### Control Flow Statements

Control flow statements allow you to control the execution of code based on certain conditions.

- `if` statement: Executes a block of code if a specified condition is true.
- `elif` statement: Allows for multiple conditions to be checked.
- `else` statement: Executes a block of code if none of the previous conditions are true.
- `for` loop: Iterates over a sequence of items a specified number of times.
- `range()` function: Generates a sequence of numbers within a specified range.

### Functions

Functions are blocks of reusable code that perform a specific task. They help in organizing code and making it more modular.

- `def` keyword: Defines a function.
- Function name: Descriptive name given to the function.
- Parameters: Inputs to the function.
- Code block: Contains the instructions to be executed when the function is called.
- `return` statement: Specifies the value to be returned from the function.

### Example:

```python
def greet():
    print('hello world')

def greet_with_name(name):
    print(f'hello: {name}')

greet()  # Output: hello world
greet_with_name('John')  # Output: hello: John

```

Python offers a wide range of libraries and frameworks that enhance its capabilities, making it a powerful and versatile language for various applications.

```python
first_name = 'hanna'
age = 24
print(type(first_name.count('e')))
#counts the number of occurrences of the character 'e' in the string **first_name.**
print(type(age))
# prints the type of the variable **age**. Since **age** is an integer, **type(age)** will be **int**.

student_list = ['hanna','beki','laura', 'tom']
student_list.append("hanna")#appends the string "hanna" to the end of the **student_list** list.
student_list.insert(3,"red")#inserts the string "red" at index 3 of the **student_list** list.
print(student_list)

#tuple  - does not update
names = ('hanna', 'tomi')

print(type(names))

#set  - no duplicated item it has to always be new   -how to know if it has duplicated value?
stu_info = {'name':'hanna',
            'age':55,
            'sec':'B',
            'height':1.3,
            'skill':['java','javascript','python']}

print(stu_info['height'])#prints the value associated with the key 'height' in the **stu_info** dictionary.
#controls the flow statement
for i in range(0,12):
   print(i)#starts a for loop that iterates over the range of numbers from 0 to 11 (inclusive).

for i in student_list:
    print(i)

for index, value in enumerate(student_list):
     print(value)

for value in (student_list):
    print(value)

#pass

adge = 45
if age > 18:
    print('adult')
elif(age < 18):
    print('under age')
else:
    print('error')

#function
def greet():
    print('hello world')

def greet_with_name(name):
    print(f'hello: {name}')

```

some key features of Python:

### **Interpreted Language:** Python is an interpreted language, which means that the code is executed line-by-line at runtime, without the need for a separate compilation step.

Example:

```python

1print("Hello, World!")

```

### **High-Level Language:** Python is a high-level language, which means that it abstracts away many of the low-level details of the computer, such as memory management.

Example:

```python

my_list = [1, 2, 3, 4, 5]
print(my_list[0])  # prints 1

```

### **Object-Oriented:** Python is an object-oriented language, which means that everything in Python is an object, including numbers, strings, and even functions.

Example:

```python
pythonEditDownloadCopy code
def greet(name):
    return f"Hello, {name}!"

my_function = greet
print(my_function("Alice"))  # prints "Hello, Alice!"

```

**Dynamic Typing:** Python is dynamically typed, which means that you don't need to declare the data type of a variable when you create it.

Example:

```python
my_variable = 10
print(type(my_variable))  # prints <class 'int'>

my_variable = "Hello, World!"
print(type(my_variable))  # prints <class 'str'>

```

**Standard Library:** Python has a large standard library, which includes modules for tasks such as file I/O, networking, and data processing.

Example:

```python

import os

print(os.listdir("."))  # prints a list of files and directories n the current directory

```

**Indentation:** Python uses indentation to define blocks of code, rather than curly braces.

Example:

```python

if True:
    print("This is true!")

for i in range(5):
    print(i)

```

**Comments:** Python uses the hash symbol (**`#`**) to start a comment.

Example:

```python

# This is a comment
print("This is not a comment")

```

**Variables:** In Python, variables are dynamically typed and can be assigned any value.

Example:

```python
my_variable = 10
my_variable = "Hello, World!"

```

**Keywords:** Python has a set of reserved words, known as keywords, that have special meanings and can't be used as variable names.

Example:

```python
    if True:
    print("This is an if statement")
 
    for i in range(5):
    print(i)

```

**Data Types:** Python has several built-in data types, including numbers, strings, lists, tuples, and dictionaries.

Example:

```python
my_number = 10
my_string = "Hello, World!"
my_list = [1, 2, 3, 4, 5]
my_tuple = (1, 2, 3, 4, 5)
my_dictionary = {"name": "Alice", "age": 30}

```

**Functions:** Functions are blocks of code that can be defined and called by name. They can take arguments and return values.

Example:

```python

def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))  # prints "Hello, Alice!"

```

**Control Flow:** Python has several control flow statements, including **`if`**, **`elif`**, **`else`**, **`for`**, and **`while`**.

Example:

```python
for i in range(5):
    if i % 2 == 0:
        print(f"{i} is even")
    else:
        print(f"{i} is odd")

```

**List Comprehensions:** List comprehensions are a concise way to create lists in Python.

Example:

```python
squares = [x**2 for x in range(10)]
print(squares)  # prints [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

```

**Modules and Packages:** Python has a module system that allows you to import and use code from other files.

Example:

```python
import math

print(math.sqrt(16))  # prints 4.0

```

**Exception Handling:** Python has a built-in exception handling system that allows you to catch and handle errors.

Example:

```python
try:
    print(10 / 0)
except ZeroDivisionError:
    print("You can't divide by zero!")

```

**Classes and Objects:** Python supports object-oriented programming with classes and objects.

Example:

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        return f"Hello, my name is {self.name} and I am {self.age} years old."

alice = Person("Alice", 30)
print(alice.greet())  # prints "Hello, my name is Alice and I am 30 years old."

```

**File I/O:** Python has built-in support for reading and writing files.

Example:

```python

with open("example.txt", "w") as file:
    file.write("Hello, World!")

with open("example.txt", "r") as file:
    print(file.read())  # prints "Hello, World!"

```

**Command-Line Arguments:** Python has a built-in module called **`argparse`** that allows you to easily handle command-line arguments.

Example:

```python

import argparse

parser = argparse.ArgumentParser(description="A simple example of using argparse")
parser.add_argument("--name", help="Your name")
parser.add_argument("--age", type=int, help="Your age")

args = parser.parse_args()

print(f"Hello, {args.name}! You are {args.age} years old.")

```

**Unit Testing:** Python has a built-in module called **`unittest`** that allows you to easily write and run unit tests for your code.

Example:

```python
import unittest

class TestStringMethods(unittest.TestCase):
    def test_upper(self):
        self.assertEqual('foo'.upper(), 'FOO')

    def test_isupper(self):
        self.assertTrue('FOO'.isupper())
        self.assertFalse('Foo'.isupper())

if __name__ == '__main__':
   unittest.main()

```

**Virtual Environments:** Python has a built-in module called **`venv`** that allows you to create isolated virtual environments for your projects.

Example:

```bash

python3 -m venv my_project_env
source my_project_env/bin/activate

```

# **Django**

Django is a high-level Python web framework that enables rapid development of secure and maintainable websites. Built by experienced developers, Django takes care of much of the hassle of web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source.

Django follows the "Don't Repeat Yourself" (DRY) principle, which means it promotes the reusability of components to minimize code repetition. This is achieved through a system of interchangeable, plug-and-play components that can be adapted to suit different projects.

It is designed to make the development process faster and easier by providing a set of tools and libraries that handle common web development tasks. Here's a step-by-step guide to creating a Django project with an example:

Step 1: Install Django

Before you can start using Django, you need to install it on your system. You can install Django using pip, which is a package manager for Python. Open your terminal or command prompt and type the following command:

```bash
pip install django

```

Step 2: Create a new Django project

Once Django is installed, you can create a new project using the following command:

```bash
django-admin startproject myproject

```

Replace "myproject" with the name of your project. This command will create a new directory with the same name as your project, which will contain several files and directories, including a [manage.py](http://manage.py/) file and a [settings.py](http://settings.py/) file.

Step 3: Create a new Django app

In Django, a project can consist of multiple apps. To create a new app, navigate to your project directory and type the following command:

```bash
python manage.py startapp myapp

```

Replace "myapp" with the name of your app. This command will create a new directory with the same name as your app, which will contain several files and directories, including a [views.py](http://views.py/) file and a [models.py](http://models.py/) file.

Step 4: Define your models

In Django, models are used to define the structure of your database. To define your models, open the [models.py](http://models.py/) file in your app directory and add the following code:

```python
from django.db import models

class MyModel(models.Model):
    name = models.CharField(max_length=100)
    age = models.IntegerField()
    email = models.EmailField()

```

This code defines a new model called "MyModel" with three fields: name, age, and email.

Step 5: Create your database

To create your database, open the [settings.py](http://settings.py/) file in your project directory and add the following code:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': 'mydatabase',
    }
}

```

This code defines a new SQLite3 database called "mydatabase".

Step 6: Create your migrations

To create your migrations, navigate to your app directory and type the following command:

```bash
python manage.py makemigrations

```

This command will create a new migration file in a migrations directory.

Step 7: Apply your migrations

To apply your migrations, type the following command:

```bash
python manage.py migrate

```

This command will create a new database with the structure defined by your models.

Step 8: Define your views

In Django, views are used to handle HTTP requests and generate HTTP responses. To define your views, open the [views.py](http://views.py/) file in your app directory and add the following code:

```python
from django.http import HttpResponse

def my_view(request):
    return HttpResponse("Hello, world!")

```

This code defines a new view called "my\_view" that returns an HTTP response with the text "Hello, world!".

Step 9: Define your URLs

In Django, URLs are used to map HTTP requests to views. To define your URLs, open the [urls.py](http://urls.py/) file in your project directory and add the following code:

```python
from django.urls import path
from myapp.views import my_view

urlpatterns = [
    path('myview/', my_view),
]

```

This code defines a new URL pattern that maps HTTP requests to the "my\_view" view.

Step 10: Run your server

To run your server, type the following command:

```bash
python manage.py runserver

```

This command will start a new web server on your local machine. You can access your web application by navigating to [http://localhost:8000/myview/](http://localhost:8000/myview/) in your web browser.

In Django, a project typically consists of multiple apps.

1. **Django Project**:
    - A Django project is a collection of settings, configurations, and apps for a particular website or web application.
    - It serves as the overall container for your website.
    - The project folder typically contains settings.py (for project-wide settings), urls.py (for routing), and other configuration files.
    - You can create a Django project using the command **`django-admin startproject projectname`**.
2. **Django App**:
    - An app is a web application that does something – e.g., a blog, a database of public records, or a simple poll app.
    - Each Django app is intended to handle a specific functionality or set of related functionalities.
    - An app can be reused in other projects, which promotes modularity and reusability.
    - An app is a Python package that follows certain conventions, such as having a models.py file for database models, views.py for handling requests, and urls.py for URL routing within the app.
    - You can create a Django app using the command **`python manage.py startapp appname`**.
3. **Files and Directories**:
    - **settings.py**: Contains configuration settings for the Django project, including database configuration, static files configuration, middleware, installed apps, and more.
    - **urls.py**: Defines the URL patterns for the project. It maps URLs to views, directing the flow of incoming requests to appropriate functions.
    - **views.py**: Contains the view functions, which handle incoming requests and return appropriate HTTP responses. Views typically interact with models to fetch or manipulate data.
    - **models.py**: Defines the data models for the project. Django's ORM (Object-Relational Mapping) enables you to define these models using Python classes, which Django then translates into database tables.
    - **admin.py**: Allows you to register your models with the Django admin interface, enabling CRUD (Create, Read, Update, Delete) operations on your data through the admin interface.
    - **apps.py**: Configuration for the app itself. It includes metadata for the app, such as the app's name.
    - **migrations/**: Contains database migration files. Migrations are Django's way of propagating changes you make to your models (adding a field, deleting a model, etc.) into your database schema.
    - **templates/**: Directory for HTML templates used by the app's views to generate dynamic content.
    - **static/**: Directory for static files like CSS, JavaScript, images, etc., used by the app.
    - **tests.py**: Contains unit tests for the app.
    - **init.py**: An empty file that makes the directory a Python package.
    
    CRUD stands for Create, Read, Update, and Delete. These operations represent the four basic functions that are often performed on data in a database or application. Here's a brief explanation of each operation:
    
    1. **Create**: This operation involves adding new data to the database. For example, creating a new user account, adding a new blog post, or inserting a new product into an online store.
    2. **Read**: Reading refers to retrieving existing data from the database. This could involve fetching a list of all users, displaying the details of a specific blog post, or retrieving information about a particular product.
    3. **Update**: Updating involves modifying existing data in the database. For instance, updating a user's profile information, editing the content of a blog post, or changing the price of a product.
    4. **Delete**: This operation involves removing data from the database. For example, deleting a user account, removing a blog post, or discontinuing a product from the online store.
    
    Implementing CRUD operations in a Django project typically involves working with models, views, and templates:
    
    1. **Models**: Define the structure of your data using Django models. Each model class represents a database table, and each instance of the class represents a row in the table. You define fields on the model class to represent the attributes of your data.
    2. **Views**: Create view functions that handle HTTP requests and interact with the database to perform CRUD operations. These functions fetch data from the database, render templates with the retrieved data, process form submissions to create or update data, and delete data when required.
    3. **Templates**: Design HTML templates that display the data to users and provide forms for creating and updating data. Templates can include forms for user input, display data retrieved from the database, and provide links or buttons for users to perform CRUD operations.
    
    basic example of how to implement CRUD operations for a simple "todo" app in a Django project:
    
    1. **Define a Model**:
        
        ```python
        pythonCopy code
        # models.py
        from django.db import models
        
        class TodoItem(models.Model):
            title = models.CharField(max_length=100)
            completed = models.BooleanField(default=False)
        
        ```
        
    2. **Create Views**:
        
        ```python
        pythonCopy code
        # views.py
        from django.shortcuts import render, redirect
        from .models import TodoItem
        
        def todo_list(request):
            todos = TodoItem.objects.all()
            return render(request, 'todo/todo_list.html', {'todos': todos})
        
        def create_todo(request):
            if request.method == 'POST':
                title = request.POST['title']
                TodoItem.objects.create(title=title)
                return redirect('todo_list')
            return render(request, 'todo/create_todo.html')
        
        def delete_todo(request, todo_id):
            todo = TodoItem.objects.get(id=todo_id)
            todo.delete()
            return redirect('todo_list')
        
        ```
        
    3. **Create Templates**:
        - todo_list.html: Display a list of todo items.
        - create_todo.html: Form for creating a new todo item.
    4. **Define URLs**:
        
        ```python
        pythonCopy code
        # urls.py
        from django.urls import path
        from . import views
        
        urlpatterns = [
            path('', views.todo_list, name='todo_list'),
            path('create/', views.create_todo, name='create_todo'),
            path('delete/<int:todo_id>/', views.delete_todo, name='delete_todo'),
        ]
        
        ```