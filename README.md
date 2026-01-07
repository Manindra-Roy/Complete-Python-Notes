# Python Programming Notes

## Introduction

* **[span_0](start_span)What is Programming:** Just as we use languages like Hindi or English to communicate with each other, we use a programming language like Python to communicate with the computer[span_0](end_span). [span_1](start_span)Programming is a way to instruct the computer to perform various tasks[span_1](end_span).
* **[span_2](start_span)What is Python?** Python is a simple and easy-to-understand language which feels like reading simple English[span_2](end_span). [span_3](start_span)This "Pseudo Code" nature of Python makes it easy to learn and understandable by beginners[span_3](end_span).
* **Features of Python:**
    * [span_4](start_span)Easy to understand = Less development time[span_4](end_span).
    * [span_5](start_span)Free and open source[span_5](end_span).
    * [span_6](start_span)High-level language[span_6](end_span).
    * [span_7](start_span)Portable (Works on Linux/Windows/Mac)[span_7](end_span).
    * [span_8](start_span)Fun to work with[span_8](end_span).
* **[span_9](start_span)Installation:** Python can be easily installed from `python.org`[span_9](end_span).

---

## Chapter 1: Modules, Comments & Pip

* **First Program:** `print("Hello World")`. [span_10](start_span)`print` is a function[span_10](end_span).
* **[span_11](start_span)Modules:** A module is a file containing code written by somebody else (usually) which can be imported and used in our programs[span_11](end_span).
* **Pip:** Pip is the package manager for Python. [span_12](start_span)You can use pip to install a module on your system (e.g., `pip install flask`)[span_12](end_span).
* **Types of Modules:**
    1.  **[span_13](start_span)Built-in modules:** Pre-installed in Python (e.g., `os`, `abc`)[span_13](end_span).
    2.  **[span_14](start_span)External modules:** Need to be installed using pip (e.g., `tensorflow`, `flask`)[span_14](end_span).
* **[span_15](start_span)REPL:** Using Python as a calculator by typing "python" on the terminal opens the REPL (Read Evaluate Print Loop)[span_15](end_span).
* **[span_16](start_span)Comments:** Used to write something the programmer does not want to execute (e.g., author name, date)[span_16](end_span).
    * **[span_17](start_span)Single line comments:** Written using `#`[span_17](end_span).
    * **[span_18](start_span)Multi-line comments:** Written using `''' Comment '''`[span_18](end_span).

---

## Chapter 2: Variables and Datatypes

* **[span_19](start_span)Variable:** A name given to a memory location in a program (container to store a value)[span_19](end_span).
    * *Examples:* `a=30`, `b="Maya"`, `c=71.22`.
* **Rules for Variable Names:**
    * [span_20](start_span)Can contain alphabets, digits, and underscores[span_20](end_span).
    * [span_21](start_span)Can only start with an alphabet or underscore[span_21](end_span).
    * [span_22](start_span)Cannot start with a digit[span_22](end_span).
    * [span_23](start_span)No white space is allowed[span_23](end_span).
* **[span_24](start_span)Data Types:** Python automatically identifies the type of data[span_24](end_span).
    1.  Integers (`int`).
    2.  Floating point numbers (`float`).
    3.  Strings (`str`).
    4.  Booleans (`bool`).
    5.  None.
* **Operators:**
    * **[span_25](start_span)Arithmetic:** `+`, `-`, `*`, `/` etc.[span_25](end_span).
    * **[span_26](start_span)Assignment:** `=`, `+=`, `-=` etc.[span_26](end_span).
    * **[span_27](start_span)Comparison:** `==`, `>`, `>=`, `<`, `!=` etc.[span_27](end_span).
    * **[span_28](start_span)Logical:** `and`, `or`, `not`[span_28](end_span).
* **[span_29](start_span)`type()` function:** Used to find the data type of a given variable[span_29](end_span).
* **[span_30](start_span)Typecasting:** Converting one data type into another[span_30](end_span).
    * `str(31)` $\rightarrow$ `"31"` (Integer to String).
    * `int("32")` $\rightarrow$ `32` (String to Integer).
    * `float(32)` $\rightarrow$ `32.0` (Integer to Float).
* **[span_31](start_span)`input()` function:** Allows the user to take input from the keyboard[span_31](end_span).
    * **[span_32](start_span)Important:** The output of `input()` is always a string[span_32](end_span).
    * Example: `a = input("Enter name")`. [span_33](start_span)If user enters "Maya", `a` is "Maya"[span_33](end_span).

---

## Chapter 3: Strings

* **[span_34](start_span)Definition:** A sequence of characters enclosed in quotes (Single `'`, Double `"`, or Triple `'''`)[span_34](end_span).
    * Examples: `a = 'Maya'`, `b = "Maya"`, `c = '''Maya'''`.
* **[span_35](start_span)String Slicing:** A string can be sliced for getting a part of the string[span_35](end_span).
    * Consider string: `name = "Maya"` (Length = 4).
    * Indices: `M`=0, `a`=1, `y`=2, `a`=3.
    * [span_36](start_span)Formula: `sl = name[ind_start : ind_end]`[span_36](end_span).
    * *[span_37](start_span)Note:* First index is included, last index is *not* included[span_37](end_span).
    * Example: `sl[0:3]` returns `"May"` (characters from index 0 to 2).
    * **[span_38](start_span)Negative Indices:** Indexing can happen from the end, where `-1` is the last character[span_38](end_span).
    * **[span_39](start_span)Slicing with Skip Value:** `word[1:6:2]` returns characters from index 1 to 6 skipping every 2nd character[span_39](end_span).
* **String Functions:**
    * `len()`: Returns length of string. [span_40](start_span)`len("Maya")` returns 4[span_40](end_span).
    * [span_41](start_span)`endswith("aya")`: Returns True if string ends with "aya"[span_41](end_span).
    * [span_42](start_span)`count("a")`: Counts total number of occurrences of "a"[span_42](end_span).
    * [span_43](start_span)`capitalize()`: Capitalizes the first character of the string[span_43](end_span).
    * [span_44](start_span)`find(word)`: Returns the index of the first occurrence of `word`[span_44](end_span).
    * [span_45](start_span)`replace(old, new)`: Replaces `old` word with `new` word in the entire string[span_45](end_span).
* **[span_46](start_span)Escape Sequence Characters:** Sequence of characters after backslash `\`[span_46](end_span).
    * [span_47](start_span)`\n` (newline), `\t` (tab), `\'` (single quote), `\\` (backslash)[span_47](end_span).

---

## Chapter 4: Lists and Tuples

* **[span_48](start_span)List:** Containers to store a set of values of any data type[span_48](end_span).
    * [span_49](start_span)Example: `friends = ["Apple", "Akash", "Rohan", 7, False]`[span_49](end_span).
    * [span_50](start_span)Indexing: `L1[0]`, `L1[1]` etc.[span_50](end_span).
    * [span_51](start_span)Slicing: `L1[0:2]`[span_51](end_span).
* **List Methods:**
    * [span_52](start_span)`L1.sort()`: Updates list to sorted order[span_52](end_span).
    * [span_53](start_span)`L1.reverse()`: Reverses the list[span_53](end_span).
    * [span_54](start_span)`L1.append(8)`: Adds 8 to the end of the list[span_54](end_span).
    * [span_55](start_span)`L1.insert(3,8)`: Adds 8 at index 3[span_55](end_span).
    * [span_56](start_span)`L1.pop(2)`: Deletes element at index 2 and returns its value[span_56](end_span).
    * [span_57](start_span)`L1.remove(21)`: Removes 21 from the list[span_57](end_span).
* **[span_58](start_span)Tuples:** An immutable data type (cannot change)[span_58](end_span).
    * [span_59](start_span)`a = ()` (Empty tuple), `a = (1,)` (Tuple with one element needs a comma)[span_59](end_span).
* **Tuple Methods:**
    * [span_60](start_span)`count(1)`: Returns number of times 1 occurs[span_60](end_span).
    * [span_61](start_span)`index(1)`: Returns index of first occurrence of 1[span_61](end_span).

---

## Chapter 5: Dictionary & Sets

* **[span_62](start_span)Dictionary:** Collection of Key-Value pairs[span_62](end_span).
    * [span_63](start_span)Syntax: `a = {"name": "Maya", "marks": "100", "list": [1,2,9]}`[span_63](end_span).
    * *[span_64](start_span)Properties:* Unordered, Mutable, Indexed, Cannot contain duplicate keys[span_64](end_span).
* **Dictionary Methods:**
    * [span_65](start_span)`items()`: Returns list of (key, value) tuples[span_65](end_span).
    * [span_66](start_span)`keys()`: Returns list containing dictionary's keys[span_66](end_span).
    * [span_67](start_span)`update({"friend": "Sam"})`: Updates the dictionary with supplied pairs[span_67](end_span).
    * [span_68](start_span)`get("name")`: Returns value of "name" (Returns `None` if key is missing, doesn't throw error)[span_68](end_span).
* **[span_69](start_span)Sets:** Collection of non-repetitive elements[span_69](end_span).
    * *[span_70](start_span)Properties:* Unordered, Unindexed, Immutable items (cannot change items inside, but can add/remove from set), No duplicate values[span_70](end_span).
    * [span_71](start_span)Example: `S = {1, 8, 2, 3}`[span_71](end_span).
* **Set Operations:**
    * [span_72](start_span)`len(s)`: Length of set[span_72](end_span).
    * [span_73](start_span)`remove(8)`: Removes 8 from set[span_73](end_span).
    * [span_74](start_span)`pop()`: Removes arbitrary element[span_74](end_span).
    * [span_75](start_span)`clear()`: Empties the set[span_75](end_span).
    * [span_76](start_span)`union({8, 11})`: Returns new set with all items from both sets[span_76](end_span).
    * [span_77](start_span)`intersection({8, 11})`: Returns set with only common items[span_77](end_span).

---

## Chapter 6: Conditional Expressions

* **[span_78](start_span)If-Elif-Else:** Used for decision making[span_78](end_span).
    * [span_79](start_span)Syntax: `if`, `elif` (else if), `else`[span_79](end_span).
    * [span_80](start_span)The ladder stops once a condition is met[span_80](end_span).
* **[span_81](start_span)Relational Operators:** `==`, `>=`, `<=`, etc.[span_81](end_span).
* **Logical Operators:**
    * [span_82](start_span)`and`: True if both true[span_82](end_span).
    * [span_83](start_span)`or`: True if at least one is true[span_83](end_span).
    * [span_84](start_span)`not`: Inverts True to False[span_84](end_span).

---

## Chapter 7: Loops

* **[span_85](start_span)While Loop:** Executes as long as the condition is true[span_85](end_span).
    * Example: `print("Maya")` 5 times using a loop.
* **[span_86](start_span)For Loop:** Used to iterate through a sequence (list, tuple, string)[span_86](end_span).
* **[span_87](start_span)Range Function:** `range(start, stop, step-size)` used to generate a sequence of numbers[span_87](end_span).
* **[span_88](start_span)For Loop with Else:** An optional `else` can be used; executed when the loop exhausts[span_88](end_span).
* **[span_89](start_span)Break Statement:** Exits the loop immediately[span_89](end_span).
* **[span_90](start_span)Continue Statement:** Skips the current iteration and moves to the next[span_90](end_span).
* **[span_91](start_span)Pass Statement:** A null statement that does nothing (instruction to "Do nothing")[span_91](end_span).

---

## Chapter 8: Functions & Recursions

* **[span_92](start_span)Function:** A group of statements performing a specific task[span_92](end_span). [span_93](start_span)Implements code reuse[span_93](end_span).
    * [span_94](start_span)Syntax: `def func1():`[span_94](end_span).
* **Types:**
    * **[span_95](start_span)Built-in:** `len()`, `print()`, `range()`[span_95](end_span).
    * **[span_96](start_span)User-defined:** Defined by the user[span_96](end_span).
* **[span_97](start_span)Arguments:** Values passed to the function[span_97](end_span).
    * [span_98](start_span)Example: `def greet(name): ... a = greet("Maya")`[span_98](end_span).
* **[span_99](start_span)Default Parameter Value:** Value used if no argument is passed (e.g., `def greet(name="Stranger"):`)[span_99](end_span).
* **[span_100](start_span)Recursion:** A function calling itself[span_100](end_span). [span_101](start_span)Used for direct mathematical formulas like factorial ($n! = n \times (n-1)!$)[span_101](end_span).

---

## Chapter 9: File I/O

* **[span_102](start_span)Files:** Used to persist data (store forever) because RAM is volatile[span_102](end_span).
* **Types:**
    1.  **[span_103](start_span)Text files:** `.txt`, `.c` etc.[span_103](end_span).
    2.  **[span_104](start_span)Binary files:** `.jpg`, `.dat` etc.[span_104](end_span).
* **[span_105](start_span)Opening a File:** `open("this.txt", "r")` takes filename and mode[span_105](end_span).
* **[span_106](start_span)Modes:** `r` (read), `w` (write), `a` (append), `+` (update), `rb` (read binary)[span_106](end_span).
* **Reading:**
    * [span_107](start_span)`f.read()`: Reads content[span_107](end_span).
    * [span_108](start_span)`f.readline()`: Reads one line at a time[span_108](end_span).
* **[span_109](start_span)Writing:** `f.write("text")`[span_109](end_span).
* **[span_110](start_span)With Statement:** Best way to open files; closes the file automatically (`with open(...) as f:`)[span_110](end_span).

---

## Chapter 10: Object Oriented Programming (OOP)

* **[span_111](start_span)Class:** A blueprint for creating objects[span_111](end_span). (Implements DRY - Don't Repeat Yourself principle).
* **[span_112](start_span)Object:** An instantiation of a class[span_112](end_span). [span_113](start_span)Memory is allocated only after object instantiation[span_113](end_span).
* **[span_114](start_span)Abstraction & Encapsulation:** Hiding implementation details[span_114](end_span).
* **Attributes:**
    * **[span_115](start_span)Class Attributes:** Belong to the class (e.g., `Company="Google"`)[span_115](end_span).
    * **[span_116](start_span)Instance Attributes:** Belong to the object (e.g., `maya.name`, `maya.salary`)[span_116](end_span). **[span_117](start_span)Note:** Instance attributes take preference over class attributes[span_117](end_span).
* **[span_118](start_span)`self` Parameter:** Refers to the instance of the class[span_118](end_span). Example: `maya.getSalary()` is equivalent to `Employee.getSalary(maya)`.
* **Static Method:** Defined using `@staticmethod`. [span_119](start_span)Used when a function doesn't need `self`[span_119](end_span).
* **[span_120](start_span)`__init__()` Constructor:** Special method run as soon as the object is created[span_120](end_span).
    * [span_121](start_span)Example: `maya = Employee("Maya")`[span_121](end_span).

---

## Chapter 11: Inheritance & More on OOP

* **[span_122](start_span)Inheritance:** Creating a new class from an existing class[span_122](end_span).
* **Types of Inheritance:**
    1.  **[span_123](start_span)Single:** One parent, one child[span_123](end_span).
    2.  **[span_124](start_span)Multiple:** Child inherits from more than one parent[span_124](end_span).
    3.  **[span_125](start_span)Multilevel:** Child becomes parent for another child[span_125](end_span).
* **[span_126](start_span)`super()` method:** Used to access methods of the superclass[span_126](end_span).
* **Class Methods:** Bound to the class, not the object. [span_127](start_span)Uses `@classmethod` decorator[span_127](end_span).
* **Property Decorators:**
    * [span_128](start_span)`@property` (Getter)[span_128](end_span).
    * [span_129](start_span)`@name.setter` (Setter)[span_129](end_span).
* **[span_130](start_span)[span_131](start_span)Operator Overloading:** Using Dunder methods to overload operators[span_130](end_span)[span_131](end_span).
    * [span_132](start_span)`p1 + p2` $\rightarrow$ `p1.__add__(p2)`[span_132](end_span).
    * [span_133](start_span)`p1 - p2` $\rightarrow$ `p1.__sub__(p2)`[span_133](end_span).
    * [span_134](start_span)`p1 * p2` $\rightarrow$ `p1.__mul__(p2)`[span_134](end_span).
    * [span_135](start_span)`p1 / p2` $\rightarrow$ `p1.__truediv__(p2)`[span_135](end_span).
    * [span_136](start_span)`p1 // p2` $\rightarrow$ `p1.__floordiv__(p2)`[span_136](end_span).
* **[span_137](start_span)Other Dunder Methods:** `__str__()`, `__len__()`[span_137](end_span).

---

## Chapter 12: Advanced Python 1

* **Exception Handling:**
    * [span_138](start_span)`try`: Code that might throw exception[span_138](end_span).
    * [span_139](start_span)`except`: Code that handles exception[span_139](end_span).
    * [span_140](start_span)`else`: Executed only if `try` was successful[span_140](end_span).
    * [span_141](start_span)`finally`: Executed regardless of error[span_141](end_span).
    * [span_142](start_span)`raise`: Used to raise custom exceptions[span_142](end_span).
* **`if __name__ == '__main__':`**: Evaluates to the name of the module. If run directly, it is set to `"__main__"`. [span_143](start_span)Used to check if module is run directly or imported[span_143](end_span).
* **[span_144](start_span)`global` keyword:** Used to modify a variable outside the current scope[span_144](end_span).
* **[span_145](start_span)`enumerate` function:** Adds counter to an iterable (`index`, `item`)[span_145](end_span).
* **[span_146](start_span)List Comprehensions:** Elegant way to create lists based on existing lists[span_146](end_span).
    * Example: `list2 = [i for item in list1 if item > 8]`.

---

## Chapter 13: Advanced Python 2

* **[span_147](start_span)Virtual Environment:** Isolated Python environment[span_147](end_span).
    * [span_148](start_span)Install: `pip install virtualenv`[span_148](end_span).
    * [span_149](start_span)Create: `virtualenv myprojectenv`[span_149](end_span).
    * [span_150](start_span)`pip freeze`: Returns all installed packages[span_150](end_span).
    * [span_151](start_span)`pip freeze > requirements.txt`: Creates requirements file[span_151](end_span).
* **[span_152](start_span)Lambda Functions:** Anonymous functions using `lambda` keyword[span_152](end_span).
    * [span_153](start_span)Syntax: `lambda arguments: expression`[span_153](end_span).
* **[span_154](start_span)`join` method:** Creates a string from iterable objects (e.g., `" and ".join(list)`)[span_154](end_span).
* **[span_155](start_span)`format` method:** Formats values inside string[span_155](end_span).
    * [span_156](start_span)Example: `"{} is a good {}".format("Maya", "boy")` (or "girl", depending on context)[span_156](end_span).
* **Map, Filter & Reduce:**
    * [span_157](start_span)`map(function, list)`: Applies function to all items[span_157](end_span).
    * [span_158](start_span)`filter(function, list)`: Creates list of items where function returns true[span_158](end_span).
    * [span_159](start_span)`reduce(function, list)`: Applies rolling computation (needs `functools`)[span_159](end_span).

