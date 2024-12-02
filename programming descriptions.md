## Detailed explanation and examples of the requested programming concepts and how they work in Python.

---

### **1. `input()`**
- The `input()` function is used to get input from the user via the console.
- It always returns a string.

Example:
```python
name = input("Enter your name: ")  # Prompt the user and store input
print(f"Hello, {name}!")  # Print the input back with a greeting
```

---

### **2. Comments**
- Comments explain the purpose of the code.
- Use `#` for single-line comments and `"""` for multi-line comments.

Example:
```python
# This is a single-line comment

"""
This is a multi-line comment
Explaining the purpose of the program
"""

print("Comments are ignored by Python.")  # This prints text
```

---

### **3. `print()`**
- `print()` outputs text or data to the console.

#### Using `f-strings`:
```python
name = "Alice"
print(f"Hello, {name}!")  # Use an f-string to format output
```

#### Using `end=`:
```python
print("Hello", end=", ")  # Prevents a new line after the output
print("World!")  # Continues on the same line
```

#### Using `sep=`:
```python
print("apple", "banana", "cherry", sep=" | ")  # Custom separator
```

---

### **4. `int()`, `float()`, `str()`**
- `int()`: Converts data to an integer.
- `float()`: Converts data to a floating-point number.
- `str()`: Converts data to a string.

Example:
```python
age = int(input("Enter your age: "))  # Convert input to integer
height = float(input("Enter your height: "))  # Convert input to float
print("Your age is " + str(age))  # Convert age to string for concatenation
```

---

### **5. `.lower()`**
- Converts a string to lowercase.

Example:
```python
name = "Alice"
print(name.lower())  # Outputs "alice"
```

---

### **6. `abs()`**
- Returns the absolute value of a number.

Example:
```python
number = -5
print(abs(number))  # Outputs 5
```

---

### **7. Raising to a Power with `**`**
- Use `**` to raise a number to a power.

Example:
```python
print(2 ** 3)  # Outputs 8 (2 raised to the power of 3)
```

---

### **8. Division: `/`, `//`, and `%`**
- `/`: Regular division (float result).
- `//`: Floor division (integer result).
- `%`: Modulus (remainder).

Example:
```python
print(10 / 3)   # Outputs 3.3333333333333335
print(10 // 3)  # Outputs 3
print(10 % 3)   # Outputs 1
```

---

### **9. Printing Two Decimal Places (`:.2f`)**
- Format numbers to two decimal places.

Example:
```python
pi = 3.14159
print(f"{pi:.2f}")  # Outputs "3.14"
```

---

### **10. Indentation and Blocks**
- Python uses indentation to define code blocks (e.g., under `if`, `for`, `def`).

Example:
```python
if True:
    print("This is indented!")  # Indented block under the if statement
```

---

### **11. Sequencing**
- The order of statements matters in Python.

Example:
```python
print("Step 1")  # Executes first
print("Step 2")  # Executes second
```

---

### **12. Selection**
- Choose between different paths using `if`.

Example:
```python
x = 5
if x > 0:
    print("Positive")
else:
    print("Not positive")
```

---

### **13. `if` vs. `if/elif/else`**
- `if`: Multiple independent conditions.
- `if/elif/else`: Mutually exclusive conditions.

Example:
```python
x = 5

# Multiple independent if statements
if x > 0:
    print("Positive")
if x < 10:
    print("Less than 10")

# if/elif/else
if x > 10:
    print("Greater than 10")
elif x > 0:
    print("Positive but not greater than 10")
else:
    print("Non-positive")
```

---

### **14. Compound Conditional Statements**
- Combine conditions using `and`, `or`.

Example:
```python
x = 5
if x > 0 and x < 10:
    print("Positive and less than 10")
```

---

### **15. Using `.lower()` in Conditionals**
- Normalize strings for comparisons.

Example:
```python
answer = input("Yes or No? ").lower()
if answer == "yes":
    print("You said yes!")
```

---

### **16. Lists**
- Create, access, and modify lists.

Example:
```python
fruits = ["apple", "banana", "cherry"]  # Create a list
print(fruits[1])  # Access the second item
fruits.append("orange")  # Add an item
fruits.insert(1, "blueberry")  # Insert at index 1
fruits.remove("apple")  # Remove an item
fruits.sort()  # Sort the list
print(fruits)
```

---

### **17. Dictionaries**
- Store key-value pairs.

Example:
```python
person = {"name": "Alice", "age": 25}  # Create a dictionary
print(person["name"])  # Access a value
person["age"] = 26  # Modify a value
```

---

### **18. Loops**
- **Iterate over a range**:
  ```python
  for i in range(5):
      print(i)  # Outputs 0 to 4
  ```

- **Iterate over a string**:
  ```python
  for char in "hello":
      print(char)
  ```

- **Iterate over a list**:
  ```python
  fruits = ["apple", "banana", "cherry"]
  for fruit in fruits:
      print(fruit)
  ```

- **Iterate over a dictionary**:
  ```python
  person = {"name": "Alice", "age": 25}
  for key, value in person.items():
      print(key, value)
  ```

---

### **19. Functions**
- **Create**:
  ```python
  def greet(name):
      return f"Hello, {name}!"
  ```

- **Call**:
  ```python
  print(greet("Alice"))
  ```

---

### **20. Function Arguments**
- The value in `()` is assigned to the parameter.

Example:
```python
def greet(name):
    print(f"Hello, {name}!")  # `name` receives the argument passed during the call

greet("Alice")  # "Alice" is assigned to `name`
```

---

### **21. Using `return`**
- Return values from a function.

Example:
```python
def square(x):
    return x ** 2

result = square(4)
print(result)  # Outputs 16
```

---

### **22. Multiple Returns**
- Return multiple values.

Example:
```python
def get_stats(numbers):
    return max(numbers), min(numbers)

max_num, min_num = get_stats([1, 2, 3, 4, 5])
print(max_num, min_num)  # Outputs 5, 1
``` 
