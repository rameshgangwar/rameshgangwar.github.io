# Getting Help

* Suppose you have a function and you do not know what that function does. Then you can use help() to get the details of that function.

```python
help(abs)
```

* This description of function is called docstring. Built-in functions have docstrings. When you define a function for yourself, **do not** forget to include docstring in that functions. This helps other programs while reading your code. Use three double quotes to write docstings. Here is an example:

```python
def function_name():
    """
    Here you write about what a function does. This description is called docstring. This is what you get when you use help() to get the information about some function.
    docstrings always comes right after the header of the function.
    """
```

# Functions

## Default Arguements

Example of default argument in a function.
```python
def greet(who="Colin"):
    print("Hello,", who)
    
greet()
greet(who="Kaggle")
# (In this case, we don't need to specify the name of the argument, because it's unambiguous.)
greet("world")
```

## Functions Applied to functions

* High order function

```python
def mult_by_five(x):
    return 5 * x

def call(fn, arg):
    """Call fn on arg"""
    return fn(arg)

def squared_call(fn, arg):
    """Call fn on the result of calling fn on arg"""
    return fn(fn(arg))

print(
    call(mult_by_five, 1),
    squared_call(mult_by_five, 1), 
    sep='\n', # '\n' is the newline character - it starts a new line
)
```

## Booleans and Conditionals

## List and Tuples

* Lists are ordered and mutable.
* Objects contains methods and attributes.
* Difference between methods and functions.
* Tuples are immutable and unordered.
* Access 2D list item as follows:

```python
teams[-1][1]
```



