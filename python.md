# Python

## Contents:

- [Introduction](###-Introduction)
- [Online Playgrounds](###-Online-Playgrounds)
- [Important Links/Resources](###-Important-Links/Resources)
- [IDE/Editor](###-IDE/Editor)
- [Built-in Functions](###-Built-in-Functions)
- [Variables](###-Variables)
- [Data Types](###-Data-Types)
- [Operators](###-Operators)
- [Math Functions](###-Math-Functions)
- [Comments](###-Comments)
- [Escape Sequences](###-Escape-Sequences)
- [Formatted Strings](###-Formatted-Strings)
- [Strings](###-Strings)
- [List](<###-List-(similar-to-Array)>)
- [Dictionaries](<###-Dictionaries-(Same-as-Objects)>)
- [Tuple](<###-Tuple-(Immutable-List)>)
- [Sets](###-Sets)
- [Falsy Values](###-Falsy-Values)
- [Conditional Logic](###-Conditional-Logic)
- [Looping](###-Looping)
- [Important Keywords](###-Important-Keywords)
- [Important Functions](###-Important-Functions)
- [Functions](###-Functions)
- [Walrus Operator](<###-Walrus-Operator-(Python-3)>)
- [Scope](###-Scope)
- [Object Oriented Programming](###-Object-Oriented-Programming)
- [Lambda Expressions](###-Lambda-Expressions)
- [Comprehensions](###-Comprehensions)
- [Higher Order Functions](<###-Higher-Order-Functions-(HOF)>)
- [Decorators](###-Decorators)
- [Error Handling](###-Error-Handling)
- [Generators](###-Generators)
- [Modules/Packages](###-Modules/Packages)
- [Built-in Modules/Packages](###-Built-in-Modules/Packages)
- [pip](<###-pip-(Package-Installer-Python)>)
- [pdb](<###-pdb-(Python-Debugger)>)
- [File I/O](###-File-I/O)
- [Regular Expressions](###-Regular-Expressions)

### Introduction:

Python is mostly interpreted language.
We normally use cpython - Python Implementation in C Language. Python is just a documentation. There are various implementation of Python such as:

- Jython - Java Implementation
- IronPython

### Online Playgrounds:

- [https://replit.com/](https://replit.com/)
- [https://glot.io/](https://glot.io/)

### Important Links/Resources:

- [Python Installation](https://realpython.com/installing-python)
- [Built in Modules/Packages](https://docs.python.org/3/py-modindex.html)
- [External Modules/Packages](https://pypi.org/)
- [regex101](https://regex101.com/)
- [regexone](https://regexone.com/)

### IDE/Editor:

- VSCode
- Sublime Text 3
- Spyder
- PyCharm CE
- Jupyter

### Built-in Functions:

- print(<expression>) / print(<expression>, <end>)
- input(<help_text>)
- type(<variable/entity>)
- float(<expression>)
- bool(<expression>)
- int(<expression>)
- str(<expression>)
- bin(<expression>)
- min(<list>)
- max(<list>)
- not(<expression>)
- sum(<operands...>)
- <operand1> is <operand2>
- help(<entity>)
- \_\_doc\_\_

### Variables:

- Variables are written in snake_case in Python.

#### Definition:

<variable_name> = <value>

#### Access:

<variable_name>

### Data Types:

| Data Type              | Values     | Example          |
| ---------------------- | ---------- | ---------------- |
| int                    | -in-0-+in  | 1, 2, 3          |
| float                  | -in-0-+in  | 1.5, 2.75, 3.0   |
| bool                   | True/False | True, False      |
| str                    | -          | "", '', f'', r'' |
| set                    | -          | {1, 2, 3}        |
| list                   | -          | [1, 2, 3]        |
| tuple                  | -          | (1,2)            |
| dict                   | -          | {"a":1, "b":2}   |
| None                   | None       | -                |
| Class                  | -          | -                |
| Specialized Data Types | -          | -                |
| complex                | -          | -                |

### Operators:

#### Arithmetic Operators:

| Operator | Summary          |
| -------- | ---------------- |
| +        | addition         |
| -        | subtraction      |
| \*       | multiplication   |
| /        | division         |
| \*\*     | power of         |
| //       | integer division |
| %        | modulus          |

#### Logical Operators:

| Operator | Summary      |
| -------- | ------------ |
| and      | and          |
| or       | or           |
| not      | not          |
| > / >=   | ge / gte     |
| < / <=   | le / lte     |
| ==       | equality     |
| !=       | non-equality |

### Math Functions:

- round(<number>)
- abs(<number>)
- floor(<number>)
- ceil(<number>)

### Comments:

#### Single Line Comments:

```py
# this is a comment in python
```

#### Multi Line Comments:

```py
"""
this is a comment in python
"""
```

### Escape Sequences:

| Escape Sequence | Description   |
| --------------- | ------------- |
| \"              | Escape quotes |
| \'              | Escape quotes |
| \n              | new line      |
| \t              | tab           |

### Formatted Strings:

#### Python 3

```py
name="Sandip Bhambre"
f"This is a formatted string {name}"
```

#### Python 2

```py
name="Sandip Bhambre"
"This is a formatted string {}".format(name)
```

### Strings:

- Strings are immutable
- Strings start at index 0
- start-value | stop-value | step-value
  - start-value defaults to zero
  - stop-value defaults to string length
  - step-value defaults to 1

```py
name="Sandip Bhambre"
name(0:6) # Sandip
```

- To reverse a string we can simple use

```py
name="Sandip Bhambre"
name(::-1) # erbmahB pidnaS
```

#### String Actions:

```py
len(string)
string.upper()
string.lower()
string.capitalize()
string.find(substring)
string.replace(substring, replace_value)
```

### List (similar to Array):

- Lists are mutable
- start-value | stop-value | step-value
  - start-value defaults to zero
  - stop-value defaults to string length
  - step-value defaults to 1

```py
todo_list=[1 2, 3]
to_list(0) # 1

```

#### List Actions:

```py
[].insert(index, element)
[].append(element)
[].extend(list)
[].remove(element)
[].clear()
[].pop() / [].pop(index)
len(list)
range(start, stop, step)
[].copy()
[].count(element)
[].index(element)
[].reverse()
[].sort()
[][::-1]
element in list
```

#### List Unpacking

```py
my_list=[1, 2, 3, 4, 5]
x, y, z = my_list # x=1, y=2, z=3
x, y, z* = my_list # x=1, y=2, z=[3, 4, 5]
```

### Dictionaries (Same as Objects):

- Key-Value pair
- Key can be int, float, str, bool

```py
my_dict = {
  "a":1,
  "b":2,
  "c":3,
}
my_dict['a'] # 1
```

#### Dictionary Actions:

```py
{}.get(value, fallback)
{}.pop(key)
{}.popitem()
{}.copy()
{}.clear()
{}.items()
{}.values()
{}.keys()
key in dict
update(dict)
```

### Tuple (Immutable List):

```py
my_tuple(1, 2, 3)
```

#### Tuple Actions:

```py
().count(element)
().index(element)
len(tuple)
```

### Sets

- Unordered collection of unique values

```py
my_set={1, 2, 3, 4, 5}
```

#### Set Actions:

```py
{}.add(element)
set(list)
list(set)
element in set
len(set)
{}.copy()
{}.clear()
{}.discard(element)
{}.union(set) / set1 | set2
{}.intersection(set) | set1 & set2
{}.difference(set)
{}.difference_update(set)
{}.isdisjoint(set)
{}.issubset(set)
{}.issuperset(set)
```

### Falsy Values:

- False
- "" / ''
- 0
- None
- []
- {}
- ()
- set()
- range(0)

### Conditional Logic:

#### if / elif / else:

```py
if condition:
  code
elif condition:
  code
else:
  code
```

#### Ternary Operator (Python 2.4+):

```py
code if condition else code
```

### Looping:

#### for:

```py
for element in list/dictionary/set:
  code
# or
for key, value in dictionary.items():
  code
# or
for key, value in enumerate(list/range/string):
  code
```

#### while:

```py
while condition:
  code
# or
while condition:
  code
else:
  code
```

### Important Keywords:

- break
- continue
- pass
- return

### Important Functions:

- zip function merges multiple iterators and returns tuples
- reduce is part of Python standard library
- we need to import it from functools
- map(function, iterable)
- filter(function, iterable)
- reduce(function, iterable, default_accumulator_value)
- zip(iterables)

### Functions:

```py
def function_name(parameters):
  code

function_name(arguments)
```

- Functions usually have positional arguments where position of arguments is matters.
- Functions ocasionally can have keyword arguments in which arguments are written as

```py
function_name(parameter_name=argument_value)
```

- Functions also can have default parameters

```py
def function_name(parameter=default_value):
  code
```

- Function can support infinite number of arguments using \*args, \*\*kwargs

  - \*args returns tuple
  - \*\*kwargs returns dictionary

- Function parameters are prioritize as

  - parameters
  - \*args
  - default parameters
  - \*\*kwargs

- global keyword is used to access global variables inside functions
- nonlocal(Python3) can be used to access global variables inside functions

#### docstring (Document Functions):

```py
def function_name(parameter=default_value):
  '''
  information related to function
  '''
  code
```

### Walrus Operator (Python 3):

- Assigns value to a variable as part of larger expression.

### Scope:

- Python supports function scope
- Python scope is prioritize as
  - local
  - local parent
  - global
  - built in

### Object Oriented Programming:

#### Classes:

- self is current object pointer
- dir(object_name) returns methods and attributes of an object

```py
class ClassName():
  def __init__(self, parameters):
    self.parameter = parameter

  def method(self, parameters):
    code

object_name = ClassName(arguments)

object_name.attribute
object_name.method(arguments)
```

#### Class object attribute:

- can vbe defined outside of constructor
- same value for all objects

```py
class_obj_attr = value

ClassName.class_obj_attr
object_name.class_obj_attr
```

#### Class Methods and Static Methods:

- cls is class pointer which can be used to create objects

```py
@classmethod
def class_method_name(cls, parameters):
  code

ClassName.class_method_name(arguments)
object_name.class_method_name(arguments)

@staticmethod
def static_method_name(parameters):
  code

ClassName.static_method_name(arguments)
```

#### Access Modifies:

- Python doesn't have a concept of Access Modifiers
- As a python programmer, we agree on method or attribute name started with underscore(\_) are considered private

#### Inheritance:

```py
class ClassName():
  code

class ClassName2(ClassName):
  code
```

#### isinstance:

```py
isinstance(object_name, ClassName)
isinstance(ClassName1, ClassName2)
```

#### super:

```py
super().__init__(arguments)
```

#### Method Resolution Order (MRO):

- In case of inheritance, if the classes have same method names then which method gets executed is figure out by MRO
- ClassName.mro()

### Lambda Expressions:

- Are anonymous functions and created to be used only once

```py
lambda parameters: code
```

### Comprehensions:

- Comprehensions allows us to create list/dictionary/sets based on some conditions

```py
# List Comprehensions
list_name = [ output for item in iterable if condition ]
# Set Comprehensions
set_name = { output for item in iterable if condition }
# Dictionary Comprehensions
dictionary_name = { key:value for key, value in iterable if condition }
dictionary_name = { key:value for key, value in dictionary.items() if condition }
```

### Higher Order Functions (HOF):

- A function is a higher order function if
  - it returns a function
  - and/or accepts a function as a parameter

### Decorators:

- Decorators are used to supercharge functions
- They wrap another function to change or enhance it

```py
# definition
def decorator_function(input_function):
  def wrapper_function(parameters):
    input_function(arguments)
  return wrapper_function

# or

def decorator_function(input_function):
  def wrapper_function(*args, **kwargs):
    input_function(*args, **kwargs)
  return wrapper_function

# access
@decorator_function
def input_function(parameters):
  code

# or
decorator_function(input_function)
```

### Error Handling:

#### Common Exceptions:

- Exception
- IndexError
- KeyError
- TypeError
- UnicodeError
- SyntaxError
- NameError
- ValueError
- ZeroDivisionError
- FloatingPointError
- ImportError
- ModuleNotFoundError
- FileExistsError
- FileNotFoundError
- InterruptedError
- PermissionError
- EOFError
- RuntimeError
- TimeoutError

```py
try:
  code
except ExceptionName:
  # or
except ExceptionName as variable:
# or
except:
  code
else:
  code
finally:
  code
```

```py
raise Exception(message)
```

### Generators:

- Allows us to generate sequence of values over time
- yield keyword is used to pause execution
- next(gen_func) is used to resume execution

```py
def gen_func(parameters):
  code
```

### Modules/Packages:

- Modules are simple files which we can import to extend the functionality of a project
- Packages are directories
- Packages are used to group similar modules
- Every package must have an \_\_init\_\_.py file

```py
# Modules import
import module_name
import module_name as new_name
from module_name import function_name
from module_name import *
# Packages import
import packege_name.module_name
from packege_name import module_name
from packege_name.module_name import function_name
from packege_name.module_name import *
```

### Built-in Modules/Packages:

- email
- math
- os
- random
- sys
- collections
- datetime
- time
- array
- pdb
- pathlib
- re

### pip (Package Installer Python):

```py
pip3 -V
pip3 install package-name
pip3 install package-name==version-number
pip3 list
pip3 install –upgrade package-name
pip3 uninstall package-name
```

### pdb (Python Debugger):

```py
import pdb
pdb.set_trace()
```

### File I/O:

```py
file_obj = open(file_path)
file_obj.read()
file_obj.readline()
file_obj.readlines()
file_obj.seek(char-index)
file_obj.close()
with open(file_path) as file_obj:
<code-block>
open(file_path, mode)
# mode		r, r+, a
file_obj.write(text)
```

### Regular Expressions:

```py
re.search(pattern,string,flags)
regex_object = re.compile(pattern)
regex_object.find(string)
regex_object.findall(string)
regex_object.fullmatch(string)
regex_object.match(string, start, end)
r”string”		raw string
```

| Symbol | Meaning            |
| ------ | ------------------ |
| \s     | whitespace         |
| \S     | non whitespace     |
| \d     | digit              |
| \D     | non digit          |
| \w     | word character     |
| \W     | non word character |
