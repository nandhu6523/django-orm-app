# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).


Include your ER diagram here

![ER](https://user-images.githubusercontent.com/123856724/233130720-8ce441ec-f844-43e9-832e-17ac27418d24.png)

## DESIGN STEPS

### STEP 1:
clone the repository from github.

### STEP 2:
create an admin interface for Django.

### STEP 3:
create an app and edit settings.py.

### STEP 4:
Makemigratons and migrate the changes.

## PROGRAM
'''
admin.py 

from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)

models.py

from django.db import models
from django.contrib import admin



class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
'''    

## OUTPUT

![orm out](https://user-images.githubusercontent.com/123856724/233130918-152c50eb-abb4-442c-9f82-746bd3cdda8c.png)

## RESULT
The program for creating an student database using ORM is executed successfully.
