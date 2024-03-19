# Ex02 Django ORM Web Application
## Date:

 07/11/2023

## AIM:
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![alt text](<Screenshot 2024-03-19 201818.png>)

## DESIGN STEPS:

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
admin.py
from django.contrib import admin
from .models import student,studentAdmin
admin.site.register(student,studentAdmin)

models.py
from django.db import models
from django.contrib import admin
class student (models.Model):
    name=models.CharField(max_length=20,help_text="student")
    rollno=models.IntegerField()
    refno=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class studentAdmin(admin.ModelAdmin):
    list_display=('name','rollno','refno','age','email')
```

## OUTPUT:

![alt text](<Screenshot 2024-03-19 200347.png>)

## RESULT:
The program  for creating student database using ORM is successful
