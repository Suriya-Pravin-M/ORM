# Ex02 Django ORM Web Application
## Date: 21-03-2024
## Name: Suriya Pravin M
## Reg.no: 212223230223
## Dept: AI&DS

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-03-20 160647](https://github.com/Suriya-Pravin-M/ORM/assets/150010919/fbd20272-d95f-41c9-85db-e51dfc222005)


## DESIGN STEPS

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
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```

## OUTPUT

![Screenshot 2024-03-20 183801](https://github.com/Suriya-Pravin-M/ORM/assets/150010919/e3815b5d-9886-45d8-9e17-5dc7df75f710)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
