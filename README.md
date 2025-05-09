# Ex02 Django ORM Web Application
## Date: 23-04-25

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## ENTITY RELATIONSHIP DIAGRAM:

![er web](https://github.com/user-attachments/assets/242b6c77-5f6a-44f0-81b5-d2611b6dd41b)


## PROGRAM
```py
from django.contrib import admin

from django.contrib import admin
from .models import Employee,EmployeeAdmin

admin.site.register(Employee,EmployeeAdmin)


from django.db import models
from django.contrib import admin

class Employee(models.Model):
    eid = models.CharField(max_length=20, help_text="Employee ID")
    name = models.CharField(max_length=100)
    salary = models.IntegerField()
    age = models.IntegerField()
    email = models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display = ['eid', 'name', 'salary','age','email']
```


## OUTPUT
![alt text](<Screenshot 2025-04-23 202409.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
