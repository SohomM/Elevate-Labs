### TASK-1 CALCULATOR

The calculator program is designed as a simple command-line application that performs basic arithmetic operations such as addition, subtraction, multiplication, and division. Each operation is implemented as a separate function, which keeps the code modular and easy to understand. The main calculator function displays a menu where the user can choose the desired operation or exit the program. It uses a continuous loop so the calculator keeps running until the user decides to quit. For every valid choice, the program takes two numbers as input, performs the corresponding operation, and displays the result. Input validation is included to ensure that only numeric values are accepted, and special handling is provided to prevent errors such as division by zero. If the user enters an invalid choice or invalid numbers, the program shows an appropriate message and prompts again instead of crashing. Overall, the program demonstrates clean structure, error handling, and user interaction, making it a reliable and easy-to-use calculator application for the command line.

INTERVIEW QUESTIONS


1. Normalization is the process of organizing data in a database to minimize redundancy and improve data integrity by dividing tables into smaller, related tables and defining relationships between them.

2. A primary key uniquely identifies each record in a table and cannot have null values. A foreign key is a field in one table that refers to the primary key in another table, establishing a relationship between the two tables.

3. Constraints are rules applied to table columns to enforce data integrity. Examples include PRIMARY KEY, FOREIGN KEY, NOT NULL, UNIQUE, and CHECK.

4. A surrogate key is an artificially generated key (often an auto-incremented number) used to uniquely identify a record when a natural primary key is not available or practical.

5. Data redundancy can be avoided by normalizing the database, enforcing constraints, using proper keys, and designing relationships between tables effectively.

6. An ER (Entity-Relationship) diagram is a visual representation of entities, their attributes, and the relationships between them in a database.

7. The main types of relationships in DBMS are one-to-one, one-to-many, and many-to-many.

8. AUTO\_INCREMENT automatically generates a unique sequential number for a column, usually used for primary keys, ensuring that each new row has a distinct identifier.

9. The default storage engine in MySQL is InnoDB.

10. A composite key is a primary key made up of two or more columns that together uniquely identify a record in a table.

### TASK 2 - TO DO LIST


### 1. How do you open and write to a file in Python?
To open and write to a file in Python, use the `open()` function with write mode (`'w'`) or append mode (`'a'`). Example:
```python
with open('filename.txt', 'w') as file:
    file.write('Hello, world!')
```
This creates the file if it doesn't exist or overwrites it if it does.

***

### 2. What are common file modes?
- `'r'` : Read-only (file must exist)
- `'w'` : Write-only (creates or overwrites file)
- `'a'` : Append (creates file if not existing, writes at end)
- `'x'` : Create (fails if file exists)
- `'b'` : Binary mode (e.g. `'rb'`, `'wb'`)
- `'t'` : Text mode (default)
- Modes can be combined, e.g., `'r+'` (read and write).

***

### 3. What’s the use of .strip()?
`.strip()` removes any leading and trailing whitespace (spaces, tabs, newlines) from a string:
```python
line = "  hello \n"
print(line.strip())  # Output: "hello"
```
This is useful when processing text data from files.

***

### 4. How do lists work in Python?
Lists are mutable data structures that store ordered collections of items. Elements can be added, removed, or changed:
```python
tasks = ["task1", "task2"]
tasks.append("task3")
print(tasks)  # ['task1', 'task2', 'task3']
```
Lists support indexing, slicing, and iteration.

***

### 5. What is the difference between append() and insert()?
- `append(item)` adds an item to the end of the list.
- `insert(index, item)` inserts an item at a specific position.
```python
lst = [1, 2]
lst.append(3)      # [1, 2, 3]
lst.insert(1, 4)   # [1, 4, 2, 3]
```


***

### 6. How can you remove elements from a list?
Use different methods:
- `remove(value)` removes the first occurrence by value
- `pop(index)` removes and returns the element at the given index (default last)
- `del list[index]` deletes at a specific position
```python
lst = [1, 2, 3]
lst.remove(2)
x = lst.pop()
del lst[0]
```


***

### 7. What are context managers (with statement)?
A context manager (`with` statement) ensures resources like files are properly managed. Files are automatically closed after the block:
```python
with open('file.txt', 'w') as f:
    f.write('data')
# File is closed here
```
Helps prevent resource leaks and errors.

***

### 8. How do you loop through a file line by line?
Use a `for` loop directly on the file object:
```python
with open('myfile.txt', 'r') as file:
    for line in file:
        print(line.strip())
```
This reads one line at a time efficiently.

***

### 9. What is a data structure?
A data structure is a way of organizing and storing data so it can be accessed and modified efficiently. Examples include lists, dictionaries, sets, and tuples in Python.

***

### 10. What happens if the file doesn't exist?
- In `'r'` (read) mode: Raises a `FileNotFoundError`.
- In `'w'` or `'a'` mode: Creates a new empty file.

