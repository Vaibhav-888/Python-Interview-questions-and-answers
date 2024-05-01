# Python-Interview-questions-and-answers

Q.1 What is the difference between the List and Tuple?
Answer: List: 1. Lists are mutable.                                                                                              Tuples: 1. Tuples are immutable.
              2. List is a container to contain different types of objects and is used to iterate objects.                               2. Tuple is also similar to list but contains immutable objects.
              3. Syntax of List: list = ['a', 'b', 'c', 1, 2, 3]                                                                         3. Syntax of Tuple: tuples = ('a', 'b', 'c', 1, 2 ,3)
              4. List iteration is slower.                                                                                               4. Tuple processing is faster than list.
              5. Lists consume more memory.                                                                                              5. Tuple consume less memory.
              6. Operations like insertion and deletion are better performed.                                                            6. Elements can be accessed better.

Q.2. What is Decorator? Explain with example.
Answer: A Decorator is just a function that takes another fuction as an argument, add some kind of functionality and then returns another function. 
All of this without altering the source code of the original function that you passed in.
```python
# Example:
def decorator_func(func):
        def wrapper_func():
                print("wrapper_func Worked")
                return wrapper_func

def show():
        print("Show Worked")
decorator_show = decorator_func(show)
decorator_show()

# Output: 
'''decorator_fun worked
wrapper_func Worked
Show Worked'''

# Alternative method to write:
@decorator_func
def display():
        print('display worked')
display()

# Output:
'''decorator_func worked
wrapper_func Worked
display worked'''
```
