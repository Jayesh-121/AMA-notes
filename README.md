# AMA Notes

---

## **1. What Are Aliases?**

Aliases are temporary names given to tables or columns in SQL to make queries shorter, more readable, or easier to reference.

### **Column Alias Example**
```sql
SELECT first_name AS name
FROM employees;
```

### **Table Alias Example**
```sql
SELECT e.name, d.department_name
FROM employees AS e
JOIN departments AS d
ON e.dept_id = d.id;
```

Aliases **do not affect actual table or column names**.

---

## **2. What Is Multiple Inheritance?**

Multiple inheritance is when a class inherits from **more than one parent class**.

### **Example**
```python
class A:
    def method_a(self):
        return "A"

class B:
    def method_b(self):
        return "B"

class C(A, B):
    pass
```

Python resolves conflicts using **MRO (Method Resolution Order)**.

---

## **3. How to See All Databases Created in PostgreSQL?**

Run the following command inside the psql terminal:

```sql
\l
```

or

```sql
\list
```

---

## **4. Difference Between UNION and UNION ALL**

| Feature | UNION | UNION ALL |
|--------|-------|------------|
| Removes duplicates | ✔ Yes | ✖ No |
| Speed | Slower | Faster |
| Use case | When unique rows are needed | When duplicates are acceptable |

---

## **5. What is the Use of `self` Keyword?**

`self` refers to the **current instance** of a class.  
Allows access to instance attributes and methods.

### **Example**
```python
class Person:
    def __init__(self, name):
        self.name = name
```

---

## **6. What Is a Constructor in Python?**

A constructor (`__init__`) runs automatically when an object is created.

### **Example**
```python
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model
```

---

## **7. When and Why Do We Use Inheritance?**

### **When**
- When classes share common behavior  
- When extending or customizing functionality  

### **Why**
- Code reuse  
- Simpler class hierarchy  
- Supports polymorphism  

---

## **8. Is SQL Case Sensitive?**

### **SQL Keywords:** Not case sensitive  
`SELECT` = `select` = `SeLeCt`

### **Identifiers (tables/columns):**  
Case-sensitive **only** if created with quotes.

### **Data comparisons:**  
Case sensitivity depends on *collation*.

---

## **9. Print vs Return**

### **print()**
- Displays output to console  
- Used for debugging  

### **return**
- Sends a value back from a function  
- Ends function execution  

```python
def add(a, b):
    return a + b   # return gives result back
```

---

## **10. Difference Between Function and Method**

| Function | Method |
|----------|---------|
| Independent block of code | Defined inside a class |
| Called directly | Called on an object |
| No `self` | Has `self` parameter |

---

## **11. What Is `zip` in Python?**

`zip()` pairs items from multiple iterables element-wise.

### **Example**
```python
names = ["Jay", "Ana"]
scores = [95, 88]

print(list(zip(names, scores)))
```

Output:
```
[("Jay", 95), ("Ana", 88)]
```

---

## **12. What Is Abstraction?**

Abstraction means exposing **only essential features** while hiding internal implementation details.

### **Example**
```python
from abc import ABC, abstractmethod

class Payment(ABC):
    @abstractmethod
    def process(self):
        pass
```

Purpose:
- Reduce complexity  
- Enforce structure  
- Improve maintainability  

---
