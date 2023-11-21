## Basic Slicing
```python
# Creating a list for demonstration
my_list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Basic slicing syntax: list[start:stop:step]

# Getting a subset from index 2 to 5
subset = my_list[2:6]  # [2, 3, 4, 5]

# Slicing from the start to a specific index
first_part = my_list[:5]  # [0, 1, 2, 3, 4]

# Slicing from a specific index to the end
second_part = my_list[5:]  # [5, 6, 7, 8, 9]

# Slicing with negative indices

# Last three items
last_three = my_list[-3:]  # [7, 8, 9]

# Everything except the last two items
all_but_last_two = my_list[:-2]  # [0, 1, 2, 3, 4, 5, 6, 7]

# Slicing with a step

# Every second item
every_second = my_list[::2]  # [0, 2, 4, 6, 8]

# Every third item in reverse order
every_third_reverse = my_list[::-3]  # [9, 6, 3, 0]

# Slicing works similarly with strings

# String example
my_string = "Hello, World!"

# Slicing a substring
substring = my_string[7:12]  # "World"

# Reverse the string
reversed_string = my_string[::-1]  # "!dlroW ,olleH"

# Tuples and arrays can be sliced in the same way as lists

# Tuple example
my_tuple = (0, 1, 2, 3, 4, 5)

# Slicing a tuple
tuple_subset = my_tuple[2:5]  # (2, 3, 4)

# Slicing used in a loop
# This will start from the 9th element and go backwards to the very beginning of the list.

for number in numbers[9::-1]:
    print(number)
