# Python Programming Notes

## Introduction

* **What is Programming:** Just as we use languages like Hindi or English to communicate with each other, we use a programming language like Python to communicate with the computer. Programming is a way to instruct the computer to perform various tasks.
* **What is Python?** Python is a simple and easy-to-understand language which feels like reading simple English. This "Pseudo Code" nature of Python makes it easy to learn and understandable by beginners.
* **Features of Python:**
    * Easy to understand = Less development time.
    * Free and open source.
    * High-level language.
    * Portable (Works on Linux/Windows/Mac).
    * Fun to work with.
* **Installation:** Python can be easily installed from `python.org`.

---

## Chapter 1: Modules, Comments & Pip

* **First Program:** `print("Hello World")`. `print` is a function.
* **Modules:** A module is a file containing code written by somebody else (usually) which can be imported and used in our programs.
* **Pip:** Pip is the package manager for Python. You can use pip to install a module on your system (e.g., `pip install flask`).
* **Types of Modules:**
    1.  **Built-in modules:** Pre-installed in Python (e.g., `os`, `abc`).
    2.  **External modules:** Need to be installed using pip (e.g., `tensorflow`, `flask`).
* **REPL:** Using Python as a calculator by typing "python" on the terminal opens the REPL (Read Evaluate Print Loop).
* **Comments:** Used to write something the programmer does not want to execute (e.g., author name, date).
    * **Single line comments:** Written using `#`.
    * **Multi-line comments:** Written using `''' Comment '''`.

---

## Chapter 2: Variables and Datatypes

* **Variable:** A name given to a memory location in a program (container to store a value).
    * *Examples:* `a=30`, `b="Maya"`, `c=71.22`.
* **Rules for Variable Names:**
    * Can contain alphabets, digits, and underscores.
    * Can only start with an alphabet or underscore.
    * Cannot start with a digit.
    * No white space is allowed.
* **Data Types:** Python automatically identifies the type of data.
    1.  Integers (`int`).
    2.  Floating point numbers (`float`).
    3.  Strings (`str`).
    4.  Booleans (`bool`).
    5.  None.
* **Operators:**
    * **Arithmetic:** `+`, `-`, `*`, `/` etc.
    * **Assignment:** `=`, `+=`, `-=` etc.
    * **Comparison:** `==`, `>`, `>=`, `<`, `!=` etc.
    * **Logical:** `and`, `or`, `not`.
* **`type()` function:** Used to find the data type of a given variable.
* **Typecasting:** Converting one data type into another.
    * `str(31)` -> `"31"` (Integer to String).
    * `int("32")` -> `32` (String to Integer).
    * `float(32)` -> `32.0` (Integer to Float).
* **`input()` function:** Allows the user to take input from the keyboard.
    * **Important:** The output of `input()` is always a string.
    * Example: `a = input("Enter name")`. If user enters "Maya", `a` is "Maya".

---

## Chapter 3: Strings

* **Definition:** A sequence of characters enclosed in quotes (Single `'`, Double `"`, or Triple `'''`).
    * Examples: `a = 'Maya'`, `b = "Maya"`, `c = '''Maya'''`.
* **String Slicing:** A string can be sliced for getting a part of the string.
    * Consider string: `name = "Maya"` (Length = 4).
    * Indices: `M`=0, `a`=1, `y`=2, `a`=3.
    * Formula: `sl = name[ind_start : ind_end]`.
    * *Note:* First index is included, last index is *not* included.
    * Example: `sl[0:3]` returns `"May"` (characters from index 0 to 2).
    * **Negative Indices:** Indexing can happen from the end, where `-1` is the last character.
    * **Slicing with Skip Value:** `word[1:6:2]` returns characters from index 1 to 6 skipping every 2nd character.
* **String Functions:**
    * `len()`: Returns length of string. `len("Maya")` returns 4.
    * `endswith("aya")`: Returns True if string ends with "aya".
    * `count("a")`: Counts total number of occurrences of "a".
    * `capitalize()`: Capitalizes the first character of the string.
    * `find(word)`: Returns the index of the first occurrence of `word`.
    * `replace(old, new)`: Replaces `old` word with `new` word in the entire string.
* **Escape Sequence Characters:** Sequence of characters after backslash `\`.
    * `\n` (newline), `\t` (tab), `\'` (single quote), `\\` (backslash).

---

## Chapter 4: Lists and Tuples

* **List:** Containers to store a set of values of any data type.
    * Example: `friends = ["Apple", "Akash", "Rohan", 7, False]`.
    * Indexing: `L1[0]`, `L1[1]` etc.
    * Slicing: `L1[0:2]`.
* **List Methods:**
    * `L1.sort()`: Updates list to sorted order.
    * `L1.reverse()`: Reverses the list.
    * `L1.append(8)`: Adds 8 to the end of the list.
    * `L1.insert(3,8)`: Adds 8 at index 3.
    * `L1.pop(2)`: Deletes element at index 2 and returns its value.
    * `L1.remove(21)`: Removes 21 from the list.
* **Tuples:** An immutable data type (cannot change).
    * `a = ()` (Empty tuple), `a = (1,)` (Tuple with one element needs a comma).
* **Tuple Methods:**
    * `count(1)`: Returns number of times 1 occurs.
    * `index(1)`: Returns index of first occurrence of 1.

---

## Chapter 5: Dictionary & Sets

* **Dictionary:** Collection of Key-Value pairs.
    * Syntax: `a = {"name": "Maya", "marks": "100", "list": [1,2,9]}`.
    * *Properties:* Unordered, Mutable, Indexed, Cannot contain duplicate keys.
* **Dictionary Methods:**
    * `items()`: Returns list of (key, value) tuples.
    * `keys()`: Returns list containing dictionary's keys.
    * `update({"friend": "Sam"})`: Updates the dictionary with supplied pairs.
    * `get("name")`: Returns value of "name" (Returns `None` if key is missing, doesn't throw error).
* **Sets:** Collection of non-repetitive elements.
    * *Properties:* Unordered, Unindexed, Immutable items (cannot change items inside, but can add/remove from set), No duplicate values.
    * Example: `S = {1, 8, 2, 3}`.
* **Set Operations:**
    * `len(s)`: Length of set.
    * `remove(8)`: Removes 8 from set.
    * `pop()`: Removes arbitrary element.
    * `clear()`: Empties the set.
    * `union({8, 11})`: Returns new set with all items from both sets.
    * `intersection({8, 11})`: Returns set with only common items.

---

## Chapter 6: Conditional Expressions

* **If-Elif-Else:** Used for decision making.
    * Syntax: `if`, `elif` (else if), `else`.
    * The ladder stops once a condition is met.
* **Relational Operators:** `==`, `>=`, `<=`, etc.
* **Logical Operators:**
    * `and`: True if both true.
    * `or`: True if at least one is true.
    * `not`: Inverts True to False.

---

## Chapter 7: Loops

* **While Loop:** Executes as long as the condition is true.
    * Example: `print("Maya")` 5 times using a loop.
* **For Loop:** Used to iterate through a sequence (list, tuple, string).
* **Range Function:** `range(start, stop, step-size)` used to generate a sequence of numbers.
* **For Loop with Else:** An optional `else` can be used; executed when the loop exhausts.
* **Break Statement:** Exits the loop immediately.
* **Continue Statement:** Skips the current iteration and moves to the next.
* **Pass Statement:** A null statement that does nothing (instruction to "Do nothing").

---

## Chapter 8: Functions & Recursions

* **Function:** A group of statements performing a specific task. Implements code reuse.
    * Syntax: `def func1():`.
* **Types:**
    * **Built-in:** `len()`, `print()`, `range()`.
    * **User-defined:** Defined by the user.
* **Arguments:** Values passed to the function.
    * Example: `def greet(name): ... a = greet("Maya")`.
* **Default Parameter Value:** Value used if no argument is passed (e.g., `def greet(name="Stranger"):`).
* **Recursion:** A function calling itself. Used for direct mathematical formulas like factorial.

---

## Chapter 9: File I/O

* **Files:** Used to persist data (store forever) because RAM is volatile.
* **Types:**
    1.  **Text files:** `.txt`, `.c` etc.
    2.  **Binary files:** `.jpg`, `.dat` etc.
* **Opening a File:** `open("this.txt", "r")` takes filename and mode.
* **Modes:** `r` (read), `w` (write), `a` (append), `+` (update), `rb` (read binary).
* **Reading:**
    * `f.read()`: Reads content.
    * `f.readline()`: Reads one line at a time.
* **Writing:** `f.write("text")`.
* **With Statement:** Best way to open files; closes the file automatically (`with open(...) as f:`).

---

## Chapter 10: Object Oriented Programming (OOP)

* **Class:** A blueprint for creating objects. (Implements DRY - Don't Repeat Yourself principle).
* **Object:** An instantiation of a class. Memory is allocated only after object instantiation.
* **Abstraction & Encapsulation:** Hiding implementation details.
* **Attributes:**
    * **Class Attributes:** Belong to the class (e.g., `Company="Google"`).
    * **Instance Attributes:** Belong to the object (e.g., `maya.name`, `maya.salary`). **Note:** Instance attributes take preference over class attributes.
* **`self` Parameter:** Refers to the instance of the class. Example: `maya.getSalary()` is equivalent to `Employee.getSalary(maya)`.
* **Static Method:** Defined using `@staticmethod`. Used when a function doesn't need `self`.
* **`__init__()` Constructor:** Special method run as soon as the object is created.
    * Example: `maya = Employee("Maya")`.

---

## Chapter 11: Inheritance & More on OOP

* **Inheritance:** Creating a new class from an existing class.
* **Types of Inheritance:**
    1.  **Single:** One parent, one child.
    2.  **Multiple:** Child inherits from more than one parent.
    3.  **Multilevel:** Child becomes parent for another child.
* **`super()` method:** Used to access methods of the superclass.
* **Class Methods:** Bound to the class, not the object. Uses `@classmethod` decorator.
* **Property Decorators:**
    * `@property` (Getter).
    * `@name.setter` (Setter).
* **Operator Overloading:** Using Dunder methods to overload operators.
    * `p1 + p2` -> `p1.__add__(p2)`.
    * `p1 - p2` -> `p1.__sub__(p2)`.
    * `p1 * p2` -> `p1.__mul__(p2)`.
    * `p1 / p2` -> `p1.__truediv__(p2)`.
    * `p1 // p2` -> `p1.__floordiv__(p2)`.
* **Other Dunder Methods:** `__str__()`, `__len__()`.

---

## Chapter 12: Advanced Python 1

* **Exception Handling:**
    * `try`: Code that might throw exception.
    * `except`: Code that handles exception.
    * `else`: Executed only if `try` was successful.
    * `finally`: Executed regardless of error.
    * `raise`: Used to raise custom exceptions.
* **`if __name__ == '__main__':`**: Evaluates to the name of the module. If run directly, it is set to `"__main__"`. Used to check if module is run directly or imported.
* **`global` keyword:** Used to modify a variable outside the current scope.
* **`enumerate` function:** Adds counter to an iterable (`index`, `item`).
* **List Comprehensions:** Elegant way to create lists based on existing lists.
    * Example: `list2 = [i for item in list1 if item > 8]`.

---

## Chapter 13: Advanced Python 2

* **Virtual Environment:** Isolated Python environment.
    * Install: `pip install virtualenv`.
    * Create: `virtualenv myprojectenv`.
    * `pip freeze`: Returns all installed packages.
    * `pip freeze > requirements.txt`: Creates requirements file.
* **Lambda Functions:** Anonymous functions using `lambda` keyword.
    * Syntax: `lambda arguments: expression`.
* **`join` method:** Creates a string from iterable objects (e.g., `" and ".join(list)`).
* **`format` method:** Formats values inside string.
    * Example: `"{} is a good {}".format("Maya", "boy")` (or "girl", depending on context).
* **Map, Filter & Reduce:**
    * `map(function, list)`: Applies function to all items.
    * `filter(function, list)`: Creates list of items where function returns true.
    * `reduce(function, list)`: Applies rolling computation (needs `functools`).
