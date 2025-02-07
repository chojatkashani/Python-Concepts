

# Reference Guide: Python


## Sections
- Built-in functions
- String methods
- List methods
- Additional syntax for working with strings and lists
- Regular expressions

---

## Built-in Functions
The following built-in functions are commonly used in Python.

### str()
Converts the input object to a string.
```python
str(10)  # Converts the integer 10 to the string "10"
```

### len()
Returns the number of elements in an object.
```python
print(len("security"))  # Returns and displays 8
```

---

## String Methods
The following methods can be applied to strings in Python.

### .upper()
Returns a copy of the string in all uppercase letters.
```python
print("Security".upper())  # Output: SECURITY
```

### .lower()
Returns a copy of the string in all lowercase letters.
```python
print("Security".lower())  # Output: security
```

### .index()
Finds the first occurrence of the input in a string and returns its location.
```python
print("Security".index("c"))  # Output: 2
```

---

## List Methods
The following methods can be applied to lists in Python.

### .insert()
Adds an element in a specific position inside the list.
```python
username_list = ["elarson", "fgarcia", "tshah"]
username_list.insert(2, "wjaffrey")
print(username_list)  # Output: ["elarson", "fgarcia", "wjaffrey", "tshah"]
```

### .remove()
Removes the first occurrence of a specific element inside a list.
```python
username_list = ["elarson", "bmoreno", "wjaffrey", "tshah"]
username_list.remove("elarson")
print(username_list)  # Output: ["bmoreno", "wjaffrey", "tshah"]
```

### .append()
Adds input to the end of a list.
```python
username_list.append("btang")
print(username_list)  # Output: ["bmoreno", "wjaffrey", "tshah", "btang"]
```

### .index()
Finds the first occurrence of an element in a list and returns its index.
```python
print(username_list.index("tshah"))  # Output: 2
```

---

## Additional Syntax for Working with Strings and Lists

### Concatenation (+)
Combines two strings or lists together.
```python
device_id = "IT" + "nwp12"
print(device_id)  # Output: ITnwp12
```

### Bracket Notation ([])
Uses indices to extract parts of a string or list.
```python
print("h32rb17"[0])  # Output: h
print("h32rb17"[0:3])  # Output: h32
```

---

## Regular Expressions
The following `re` module functions and regex symbols are useful for pattern searching in strings.

### re.findall()
Returns a list of matches to a regular expression.
```python
import re
print(re.findall("a53", "a53-32c .E"))  # Output: ["a53"]
```

### Common Regular Expression Symbols
#### \w (Alphanumeric Characters)
```python
print(re.findall("\w", "a53-32c .E"))  # Output: ["a", "5", "3", "3", "2", "c", "E"]
```

#### . (Matches Any Character)
```python
print(re.findall(".", "a53-32c .E"))  # Output: ["a", "5", "3", "-", "3", "2", "c", " ", ".", "E"]
```

#### \d (Matches Digits)
```python
print(re.findall("\d", "a53-32c .E"))  # Output: ["5", "3", "3", "2"]
```

#### \s (Matches Spaces)
```python
print(re.findall("\s", "a53-32c .E"))  # Output: [" "]
```

#### \. (Matches Period Character)
```python
print(re.findall("\.", "a53-32c .E"))  # Output: ["."]
```

#### + (One or More Occurrences)
```python
print(re.findall("\w+", "a53-32c .E"))  # Output: ["a53", "32c", "E"]
```

#### * (Zero or More Occurrences)
```python
print(re.findall("\w*", "a53-32c .E"))  # Output: ["a53", "", "32c", "", "", "E"]
```

#### { } (Exact Number of Occurrences)
```python
print(re.findall("\w{3}", "a53-32c .E"))  # Output: ["a53", "32c"]
```

---

End of Reference Guide
