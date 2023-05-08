# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from github.

### STEP 2:
Create a new app.

### STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Create django app and add student details.

## PROGRAM
## models.py 

from django.db import models
from django.contrib import admin


class Student(models.Model):
    referencenumber=models.CharField(primary_key=true,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')


## Admin.py
```
from django.contrib import admin
from myapp.models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin

## PROGRAM

Include your code here

## OUTPUT
![dj3](https://user-images.githubusercontent.com/120718823/236885066-c8460aa0-3b0e-4487-9e67-0e9f235b4d96.png)
![Screenshot (5)](https://user-images.githubusercontent.com/120718823/236885091-3f648a78-ce34-4790-8986-64649517606e.png)





## RESULT
Program excuted successfully
