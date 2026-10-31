Python arguments


```python
def greet(name):
    print("Hello", name)

```

1. Positional arguments
   The values are matched by their position:


```python
def add(a, b):
    print(a + b)

add(10, 20)

```

    30
    

2. Keyword arguments
   You can explicitly say which parameter gets which value:


```python
def student(name, age):
    print(name, age)

student(age=18, name="Ravi")

```

    Ravi 18
    

3. Default arguments
   A parameter can have a default value:


```python
def greet(name, message="Hello"):
    print(message, name)

greet("Ravi")

```

    Hello Ravi
    

4. *args
*args lets a function accept any number of positional arguments:



```python
def add(*numbers):
    print(numbers)

add(10, 20, 30, 40)

```

    (10, 20, 30, 40)
    

5. **kwargs
**kwargs lets a function accept any number of keyword arguments:


```python
def show(**info):
    print(info)

show(name="Ravi", age=18, city="Hyderabad")

```

    {'name': 'Ravi', 'age': 18, 'city': 'Hyderabad'}
    

Think: **kwargs = many named values packed into a dictionary.

Easy way to remember

def function(parameters):
             ↑
          placeholders

function(arguments)
          ↑
       actual values



```python
def introduce(name, age):   # name, age = parameters
    print(name, age)

introduce("Ravi", 18)       # "Ravi", 18 = arguments

```

    Ravi 18
    

Syntax Rule

4. Variable-Length Arguments — *args
Used when you don't know how many positional arguments will be provided.


```python
def add(*numbers):
    print(numbers)

add(10, 20, 30, 40)

```

    (10, 20, 30, 40)
    

5. Variable-Length Keyword Arguments — **kwargs
Used when you don't know how many keyword arguments will be provided.


```python
def details(**data):
    print(data)

details(name="Rahul", age=20, city="Hyderabad")

```

    {'name': 'Rahul', 'age': 20, 'city': 'Hyderabad'}
    

Quick Summary
Type	Example	Meaning
Positional	fun(10, 20)	Based on order
Keyword	fun(a=10, b=20)	Based on parameter name
Default	def fun(a=10)	Uses a default value
*args	fun(1, 2, 3)	Multiple positional arguments
**kwargs	fun(a=1, b=2)	Multiple keyword arguments
Easy way to remember:
*args → many values
**kwargs → many name=value pairs    


```python

```
