# AMA Notes

## 1. What are HTML attributes?
HTML attributes provide **additional information** about an HTML element.  
They appear inside the opening tag and follow the pattern: `name="value"`.

Example:
```html
<img src="image.jpg" alt="Profile picture">
```

## 2. What are functions in Python?
A function in Python is a reusable block of code designed to perform a specific task.

Example:
```python
def add(a, b):
    return a + b
```

## 3. What is the tag to include external CSS?
```html
<link rel="stylesheet" href="styles.css">
```

## 4. Explain Python list
A list in Python is an **ordered, mutable**, and **dynamic** collection.

Example:
```python
numbers = [1, 2, 3, "hello", True]
```

## 5. What is the difference between a shallow copy and a deep copy in Python?
- **Shallow copy:** Copies only the outer object; nested objects are referenced.
- **Deep copy:** Recursively copies all nested objects.

## 6. What is the purpose of a virtual environment in Python?
A virtual environment isolates a project’s dependencies from the system Python installation.

## 7. How can you view all Git remotes set for your local repository?
```bash
git remote -v
```

## 8. What is the difference between INNER JOIN and LEFT JOIN?
- **INNER JOIN:** Returns matching rows from both tables.
- **LEFT JOIN:** Returns all rows from the left table, with NULL for non-matching right rows.

## 9. How does the GROUP BY clause work in SQL?
`GROUP BY` groups rows with common values so aggregate functions apply per group.

## 10. In SQL, what happens if you perform a DELETE without a WHERE clause?
It deletes **all rows** in the table.

## 11. In Python, what’s the difference between using == and is?
- `==` → value equality  
- `is` → identity (same memory object)

## 12. What is git stash?
`git stash` temporarily saves (stashes) changes in your working directory without committing them, allowing you to switch branches or work elsewhere.
