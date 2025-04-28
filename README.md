# Ex02 Django ORM Web Application
## Date: 08.03.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![WhatsApp Image 2025-04-28 at 19 18 23_6949148f](https://github.com/user-attachments/assets/c1400d99-1f39-46a2-b01f-9329fdec40c5)


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
from .models import Movies,MoviesAdmin
admin.site.register(Movies,MoviesAdmin)

models.py


from django.db import models
from django.contrib import admin
class Movies(models.Model):
    Movie_id=models.IntegerField(primary_key=True)
    Title=models.CharField(max_length=30)
    Rating=models.IntegerField()
    Language=models.CharField()
    Genre=models.CharField(max_length=20)
    noofseats=models.IntegerField()
    date=models.DateField()

class MoviesAdmin(admin.ModelAdmin):
    list_display=('Movie_id','Title','Rating','Language','Genre','noofseats','date')
```


## OUTPUT

![WhatsApp Image 2025-04-28 at 19 11 03_0c2cea59](https://github.com/user-attachments/assets/8c51d850-59fc-4076-8973-f81cdb6b47d2)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
