```python
# Empty dictionary
empty_dict = {}

# Dictionary with key-value pairs
person = {"name": "Alice", "age": 25, "city": "New York"}

# Accessing value by key
name = person["name"]  # "Alice"

# Using get() to avoid KeyError
age = person.get("age")  # 25

# Adding a new key-value pair
person["email"] = "alice@example.com"

# Modifying an existing key
person["age"] = 26

# Removing a key-value pair
del person["city"]

# Removing a key-value pair with pop(), returns the value
email = person.pop("email")

# Check if a key exists in the dictionary
if "name" in person:
    print("Name is present")

# Iterating Over a Dictionary
# Iterating over keys
for key in person:
    print(key)

# Iterating over values
for value in person.values():
    print(value)

# Iterating over key-value pairs
for key, value in person.items():
    print(key, value)

# Number of key-value pairs in the dictionary
length = len(person)


# Creating a shallow copy of the dictionary
person_copy = person.copy()


# Nested dictionaries
nested_dict = {"person1": {"name": "Alice", "age": 25},
               "person2": {"name": "Bob", "age": 30}}

# Adanced

# Creating a dictionary from a comprehension
squares = {x: x*x for x in range(6)}

# Merging two dictionaries
other_details = {"occupation": "Engineer", "hobbies": ["Reading", "Cycling"]}
merged_dict = {**person, **other_details} #  unpacking two dict then merge
