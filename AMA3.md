# AMA Notes

## 1. What are classes in CSS?
CSS classes allow reusable styling for multiple elements.

```html
<div class="box"></div>
```
```css
.box { padding: 10px; background: lightgray; }
```

## 2. What is a callback function in JS?
A callback is a function passed into another function to run later.

```javascript
setTimeout(() => console.log("Done"), 1000);
```

## 3. What is the difference between == and === in JS?
- `==` compares values with type conversion  
- `===` compares values without conversion

```javascript
"5" == 5   // true
"5" === 5  // false
```

## 4. What are loops in JS?
Loops repeat code until a condition is met.

```javascript
for (let i = 0; i < 3; i++) console.log(i);
```

## 5. What does git pull do?
Fetches updates from a remote branch and merges them into the current branch.

## 6. How does the z-index property work in CSS?
Defines which positioned element appears on top. Higher = above others.

## 7. What is the purpose of the JOIN clause in SQL?
JOIN connects rows from multiple tables based on matching columns.

```sql
SELECT * FROM users
JOIN orders ON users.id = orders.user_id;
```

## 8. What does the HTML <meta> tag do?
Provides metadata like charset and viewport settings.

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## 9. How do you create a dictionary in Python, and how do you access its values?
```python
person = {"name": "Jay", "age": 25}
person["name"]
```

## 10. What is the difference between synchronous and asynchronous JavaScript?
- Synchronous: runs line-by-line and blocks  
- Asynchronous: doesn't block (uses callbacks, promises, async/await)

## 11. What is the CSS box model?
Defines layout as:

content → padding → border → margin

## 12. What does the JavaScript map method do on arrays?
Creates a new array by transforming every element.

```javascript
[1,2,3].map(n => n * 2); // [2,4,6]
```
