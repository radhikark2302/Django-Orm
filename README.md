# Django ORM

## Overview
Django ORM (Object-Relational Mapper) allows developers to interact with databases using Python code instead of raw SQL. It provides an abstraction layer to simplify database queries, relationships, and migrations.
This repository is dedicated to writing Django ORM queries from **easy to hard**, helping developers understand and master Django's database operations.

## Features
- Simplified database interactions
- Built-in query optimization
- Support for multiple databases
- Migrations for schema changes
- Relationship management using ForeignKey, OneToOneField, and ManyToManyField

## Installation
Ensure you have Django installed:
```bash
pip install django
```

## Getting Started
1. Create a Django project:
   ```bash
   django-admin startproject myproject
   ```
2. Define models in `models.py`:
   ```python
   from django.db import models

   class Author(models.Model):
       name = models.CharField(max_length=100)
       age = models.IntegerField()
   ```
3. Run migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
4. Use the ORM in the Django shell:
   ```bash
   python manage.py shell
   ```
   ```python
   from myapp.models import Author
   author = Author.objects.create(name="John Doe", age=45)
   print(author.name)
   ```

## ORM Queries 
This repository will contain various Django ORM queries categorized by difficulty:
- **Basic Queries:** Creating, reading, updating, and deleting records
- **Intermediate Queries:** Filtering, ordering, and related field lookups
- **Advanced Queries:** Aggregations, annotations, subqueries, and complex joins

## Contributing
Feel free to open issues or submit pull requests to improve this repository.

## License
This project is licensed under the MIT License.



