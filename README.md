## About the App
This is a Restaurant Menu App with Django 
using Python.

## Foreign Keys in DB
author = models.ForeignKey(User, on_delete=models.CASCADE) 
(This is if user is deleted, let all his models be also deleted)

author = models.ForeignKey(User, on_delete=models.PROTECT) 
(In this case, you will not be able to delete the user and its models)

author = models.ForeignKey(User, on_delete=models.SET_NULL)
(If the user is deleted, let his models remain but, let his name be set to null)