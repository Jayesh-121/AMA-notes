# AMA Notes

---

## 1. Command to create a Django project?

To create a new Django project, use the following command:

```bash
django-admin startproject project_name
```

Example:

```bash
django-admin startproject mysite
```

This command creates the basic Django project structure with required configuration files.

---

## 2. What is `views.py` file?

`views.py` contains **view functions or class-based views** that handle incoming HTTP requests and return HTTP responses.
It acts as the **business logic layer** of a Django application.

---

## 3. What are `break`, `continue`, and `pass` in Python?

* **break** – immediately exits the loop
* **continue** – skips the current iteration and moves to the next one
* **pass** – does nothing; used as a placeholder where a statement is syntactically required

---

## 4. What is `on_delete=models.CASCADE`?

`on_delete=models.CASCADE` specifies that when a referenced object is deleted, **all related objects are also deleted automatically**.
It is commonly used with `ForeignKey` relationships.

---

## 5. What are static files in Django?

Static files are files used for the frontend that do not change dynamically.
They include:

* CSS files
* JavaScript files
* Images
* Fonts

Django provides a built-in static files framework to manage and serve these files efficiently.

---

## 6. What is the difference between `render()` and `redirect()`?

* `render()` combines a template with context data and returns an HTTP response displaying a page.
* `redirect()` sends an HTTP redirect response, navigating the user to a different URL.

---

## 7. What is `manage.py` used for?

`manage.py` is a command-line utility used to manage a Django project.
It allows developers to:

* Run the development server
* Create apps
* Apply migrations
* Open the Django shell
* Create superusers

---

## 8. What does `migrate` do?

`migrate` applies migration files to the database.
It updates the database schema to match the current state of Django models.

---

## 9. What is `transaction.atomic()`?

`transaction.atomic()` ensures that a block of database operations is executed as a **single transaction**.
If an error occurs, all changes are rolled back to maintain data integrity.

---

## 10. What is Django Admin?

Django Admin is an **auto-generated web interface** that allows developers to manage database records easily without writing custom UI code.

---

## 11. What is a model field?

A model field represents a **column in a database table**.
It defines the type of data stored, such as text, numbers, dates, or relationships.

Examples include `CharField`, `IntegerField`, `DateTimeField`, and `ForeignKey`.

---
