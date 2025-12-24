# AMA Notes

---

## 1. What is `urls.py`?

`urls.py` is the file responsible for **URL routing** in a Django project or app.
It maps URL patterns to view functions or class-based views. When a user requests a URL, Django checks `urls.py` to decide **which view should handle the request**.

Example:

```python
path("login/", views.login_view)
```

---

## 2. What is a template in Django?

A Django template is an **HTML file** that uses **Django Template Language (DTL)** to generate dynamic content.
Templates separate **presentation (UI)** from business logic and allow data to be rendered using variables, loops, and conditionals.

Example:

```html
<h1>Hello {{ user.username }}</h1>
```

---

## 3. What does the `settings.py` file do?

`settings.py` contains **all configuration settings** for a Django project.
It defines how the project behaves and connects its components.

It includes:

* Database configuration
* Installed apps
* Middleware
* Templates
* Static and media files
* Security settings

---

## 4. What will happen if we don't put the app in `INSTALLED_APPS`?

If an app is not added to `INSTALLED_APPS`:

* Django will **not recognize the app**
* Models will not be migrated
* Admin registrations will not work
* Signals and app configurations will be ignored

In short, the app will exist but **Django will not use it**.

---

## 5. What is a Django app?

A Django app is a **modular unit** that performs a specific function within a project, such as authentication, blog management, or user profiles.
A project can contain multiple apps, and apps can be reused across projects.

---

## 6. What does `makemigrations` do?

`makemigrations` creates **migration files** that track changes made to models.
These files describe how the database schema should change but **do not apply the changes** to the database.

It is usually followed by:

```bash
python manage.py migrate
```

---

## 7. Difference between `innerText` and `innerHTML`?

* `innerText` returns only the **visible text** inside an element.
* `innerHTML` returns **text plus HTML tags** inside the element.

Example:

```html
<p><b>Hello</b> World</p>
```

* `innerText` → `Hello World`
* `innerHTML` → `<b>Hello</b> World`

---

## 8. What is REST?

REST (Representational State Transfer) is an **architectural style** for designing web APIs.
It uses standard HTTP methods such as:

* GET – fetch data
* POST – create data
* PUT / PATCH – update data
* DELETE – remove data

REST APIs are **stateless**, scalable, and commonly use JSON for data exchange.

---

## 9. What is a client-server architecture?

Client-server architecture divides an application into two parts:

* **Client** – sends requests (browser, mobile app)
* **Server** – processes requests and returns responses

This separation improves scalability, security, and maintainability.

---

## 10. What is `manage.py` used for?

`manage.py` is a command-line utility used to **manage Django projects**.
It allows developers to:

* Run the development server
* Create apps
* Apply migrations
* Access the Django shell
* Create superusers

Example:

```bash
python manage.py runserver
```

---
