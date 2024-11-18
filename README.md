 Ex02 Django ORM Web Application
## Date: 4/11/24

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2024-11-18 at 10 39 47_ff419d45](https://github.com/user-attachments/assets/3373b3a4-2f6b-4b2b-9e78-286785a47925)


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
~~~
models.py

from django.db import models
from django.contrib import admin
class Bank_loan (models.Model):
    customer_id=models.IntegerField(primary_key=True)
    customer_name=models.CharField(max_length=100)
    loan_amount=models.IntegerField()
    customer_age=models.IntegerField()
    email=models.EmailField()

class Bank_loanAdmin(admin.ModelAdmin):
    list_display=('customer_id','customer_name','loan_amount','customer_age','email')

~~~
    
admin.py

~~~
from django.contrib import admin
from .models import Bank_loan,Bank_loanAdmin
admin.site.register(Bank_loan,Bank_loanAdmin)
~~~

## OUTPUT

![Screenshot (7)](https://github.com/user-attachments/assets/bb35d9bf-cd6f-4a14-b560-4cb82eedfb91)
![Screenshot (6)](https://github.com/user-attachments/assets/9d5f7ba6-060a-49b1-8d6f-eaa907ac47fc)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
