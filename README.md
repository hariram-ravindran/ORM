# Ex02 Django ORM Web Application
## Date: 27.10.2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

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
'''
admin.py

from django.contrib import admin
from .models import Customer,CustomerAdmin
admin.site.register(Customer,CustomerAdmin)

models.py

from django.db import models
from django.contrib import admin
class Customer(models.Model):
	cid=models.CharField(max_length=20,primary_key="cid")
	name=models.CharField(max_length=100)
	age=models.IntegerField()
	loan=models.IntegerField()
	years=models.IntegerField()
	email=models.EmailField()

class CustomerAdmin(admin.ModelAdmin):
	list_display=("cid","name","age","loan","years","email")
'''



## OUTPUT
![alt text](<Screenshot 2024-10-27 220920.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
