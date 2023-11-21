```python
# Creating a List

# Empty list
empty_list = []

# List with elements
numbers = [1, 2, 3, 4, 5]

## Length of the list
length = len(numbers)  # Returns the number of elements in the list


# Accessing Elements
# First element (index 0)
first_element = numbers[0]  # 1

## Last element (negative indexing)
last_element = numbers[-1]  # 5

# Modifying a List
# Changing an element
numbers[0] = 10  # [10, 2, 3, 4, 5]

# Appending an element
numbers.append(6)  # [10, 2, 3, 4, 5, 6]

# Adding at a specific position
numbers.insert(1, 'a')  # [1, 'a', 2, 3, 4, 5, 7]

# Removing by value
numbers.remove('a')  # [1, 2, 3, 4, 5, 7]

# Removing by index and getting the value
popped_element = numbers.pop(1)  # 2, list is now [1, 3, 4, 5, 7]

# Sorting
# Sorting in place
numbers.sort()  # Sorts the list in ascending order

# Sorting without modifying
sorted_numbers = sorted(numbers)  # Returns a new sorted list

# Reversing in place
numbers.reverse()  # Reverses the elements of the list in place

# merge
list1 = [1, 2, 3]
list2 = [4, 5, 6]
merged_list = list1 + list2
# merged_list is [1, 2, 3, 4, 5, 6]

# Iterating over a list
for number in numbers:
    print(number)

# Advanced - List Comprehensions
# Creating a new list by applying an expression to each element
squared = [x**2 for x in numbers]
