# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
```python

Include your code here

#IN Models.py:-

from django.db import models
from django.contrib import admin
```
## Create your models here.
class Student (models.Model): referencenumber=models.CharField(max_length=20,help_text="reference number") name=models.CharField(max_length=100) bloodgroup=models.CharField(max_length=100) age=models.IntegerField() email=models.EmailField()

class StudentAdmin(admin.ModelAdmin): list_display=('referencenumber','name','bloodgroup','age','email')

#IN Admin.py:-

from django.contrib import admin from.models import Student,StudentAdmin

## Register your models here.
admin.site.register(Student,StudentAdmin)

## OUTPUT
![image](https://github.com/aadhithya15/django-orm-app/assets/121165812/8da4cf6c-d67b-4a67-844b-21752611f1cb)

## RESULT
Thus a Django application to store and retrieve data from a database using Object Relational Mapping(ORM) is developed.
