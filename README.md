# Ex02 Django ORM Web Application
## Date: 4/11/24

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![ORM(1)](https://github.com/user-attachments/assets/7303c463-2f53-4434-86e5-632330b17617)

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
from . models import Employee, EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin 
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```



## OUTPUT

![image](https://github.com/user-attachments/assets/e12f5704-3cb6-4cf6-937c-e3d63ef9d52c)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
