# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### Step 1:
Create a new django project and app

### Step 2:
Type code in views and urls.py

### Step 3:
create HTML files according to your places

### Step 4:
Give deatils about that places in html file

### Step 5:
Run the server
## PROGRAM
```python

from django.db import models
from django.contrib import admin

class GitDatabase(models.Model):
    username_primary_key = models.CharField(max_length=30, help_text="User name must be unique", primary_key=True,unique=True)
    password = models.CharField(max_length=30)
    firstname = models.CharField(max_length=20)
    lastname = models.CharField(max_length=20)
    profile_photo = models.ImageField()
    email = models.EmailField(max_length=50,unique=True)

class GitAdmin(admin.ModelAdmin):
    list_display = ('username_primary_key', 'password', 'firstname', 'lastname','profile_photo','email')

```
## OUTPUT
![output](/dataproject/django-data.png)

## RESULT
Thus a Django application is successfully developed to store and retrieve data from a database using Object Relational Mapping(ORM).
