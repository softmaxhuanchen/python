```python
# Define a function
def greet():
    print("Hello, World!")

# Call the function
greet()

# Function with parameters
def greet(name):
    print(f"Hello, {name}!")

# Call the function with arguments
greet("Alice")

# Function that returns a value
def add(a, b):
    return a + b

# Call the function and use its return value
result = add(3, 4)  # 7

# Function with default parameter value
def greet(name="World"):
    print(f"Hello, {name}!")

# Call function without passing the optional argument
greet()  # "Hello, World!"
# Call function with argument
greet("Alice")  # "Hello, Alice!"

# Function with multiple parameters
def describe_pet(animal, name):
    print(f"I have a {animal} named {name}.")

# Call function with keyword arguments
describe_pet(name="Whiskers", animal="cat")

# Advanced

# Function to take arbitrary number of arguments
def add_all(*numbers):
    return sum(numbers)

# Call function with any number of arguments
result = add_all(1, 2, 3, 4)  # 10

# Function with arbitrary keyword arguments
def build_profile(**user_info):
    return user_info

# Call function with keyword arguments
profile = build_profile(name="Alice", age=25, city="New York")

# A simple lambda function
square = lambda x: x * x

# Use the lambda function
result = square(5)  # 25

# Function with annotations
def add(a: int, b: int) -> int:
    return a + b

# Annotations do not enforce type checks, they are informational
result = add(3, 4)  # 7

# Function with a docstring
def greet():
    """Display a simple greeting."""
    print("Hello!")

# Access docstring
print(greet.__doc__)
