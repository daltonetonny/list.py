# List-asignment-.py

# Step 1: Create an empty list
my_list = []

# Step 2: Append multiple elements in one go (better than multiple append calls)
my_list += [10, 20, 30, 40]

# Step 3: Insert 15 at index 1
my_list.insert(1, 15)

# Step 4: Extend the list with additional values
my_list.extend([50, 60, 70])

# Step 5: Remove the last element using slicing (faster than pop for large lists)
my_list = my_list[:-1]

# Step 6: Sort the list in ascending order
my_list.sort()

# Step 7: Find and print the index of the value 30 with error handling
try:
    index_30 = my_list.index(30)
    print(f"Index of 30: {index_30}")
except ValueError:
    print("30 not found in the list.")

# Print the final list in a readable format
print("Final Sorted List:", my_list)
