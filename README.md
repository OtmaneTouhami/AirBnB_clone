# HolbertonBnB: A Web Application Clone

HolbertonBnB is a comprehensive web application that emulates the functionality of AirBnB. This project encompasses a robust backend system, including a database for storage, an API for seamless communication, and a user-friendly front-end interface. Currently, the project focuses on developing the backend console, which serves as the foundation for the entire application.

## Overview

The primary objectives of this project are:

1. **Establish a Base Model**: Implement a parent class called `BaseModel` to handle the initialization, serialization, and deserialization of future instances.

2. **Implement Serialization/Deserialization Flow**: Create a simple workflow for serializing and deserializing instances, allowing for seamless conversion between instances, dictionaries, JSON strings, and file storage.

3. **Develop AirBnB Classes**: Build all the necessary classes required for the AirBnB application, such as `User`, `State`, `City`, and `Place`, inheriting from the `BaseModel` class.

4. **Create a Storage Engine**: Implement an abstracted storage engine for the project, utilizing file storage as the initial approach.

5. **Implement Unit Tests**: Develop comprehensive unit tests to validate the functionality of all classes and the storage engine, ensuring robustness and reliability.

## Command Interpreter

The first step in building this web application is to create a command interpreter to manage the AirBnB objects. This interpreter serves as the backbone for interacting with the application, enabling developers to perform various operations, such as:

- Creating new objects (e.g., a new `User` or a new `Place`)
- Retrieving objects from files, databases, or other storage mechanisms
- Performing operations on objects (counting, computing statistics, etc.)
- Updating attributes of existing objects
- Destroying objects

## Learning Objectives

Upon completion of this project, you will be able to:

- Understand how to create a Python package
- Develop a command interpreter in Python using the `cmd` module
- Grasp the concept of Unit testing and its implementation in large projects
- Serialize and deserialize classes
- Read and write JSON files
- Manage datetime objects
- Utilize UUIDs (Universally Unique Identifiers)
- Work with `*args` and `**kwargs` in Python
- Handle named arguments in functions

## How to start it, How to use it, with Examples.
**Execution**
Your shell should work like this in interactive mode:

```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
```
But also in non-interactive mode: (like the Shell project(simple shell) in C)

```
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
```

All tests should also pass in non-interactive mode:
```
$ echo "python3 -m unittest discover tests" | bash
```