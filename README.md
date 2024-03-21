# Ex02 Django ORM Web Application
## DATE:13/03/2024
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![Screenshot 2024-03-21 083207](https://github.com/Balunithu/ORM/assets/161273477/55c78b24-596e-44e6-84db-406a4113918e)


## DESIGN STEPS:

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

models.py

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno")
      name=models.CharField(max_length=50)
      author=models.CharField(max_length=70)
      price=models.IntegerField()
      publisher=models.CharField(max_length=60)

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher")
```

## OUTPUT:

![Screenshot 2024-03-21 083656](https://github.com/Balunithu/ORM/assets/161273477/a3f318ec-b505-42c6-b63e-97f9dd9677ba)


## RESULT:
The program  for creating student database using ORM is successful
