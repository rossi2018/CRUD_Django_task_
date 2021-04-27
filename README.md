# CRUD_Django_task_
Task Title: CRUD Django task (adding more functionalities to the blog)

This is the web application for blog where you can register,login,reset the password and logout of the blog 

CRUD stands for Create, Retrieve, Update, Delete

**Installation**

The installation is very straightforward and make sure you are using at least python 3.8.5 and later.
Make sure *pip* setuptool is installed with python package.

Create virtual environment using using *pipenv*. To install  *pipenv*  use this command 

```
$pip install pipenv

```

After installing the *pipenv* create a directory   

```
$ mkdir django_crud
$ cd django_crud

```
Next, create python virtual environment using *pipenv* package for Django 
```
$ pipenv install django
```
When you create the python virtual environment by installing django. It must create two files which are *pipfile* and   *pipfile.lock* 



To Activate or get inside the pipenv  virtual environment in linux (Ubuntu 20.04).Use this command

```
$ pipenv shell
```

You’ll now notice that the name directory ( django_crude)  and a hash number is preceding our command prompt. This indicates we are now working within our virtual environment like this 

```
$(django101-z0e96VTa):
```

To know the version of django use in the virtual environment ,use this command 

```
$ (django101-z0e96VTa) :pip show django 
```

Deactivate virtual environment.
```
$(django101-z0e96VTa) : exit
```

To active the shell again type 

```
$ pipenv shell
```
To start a project inside python shell, type 

```
$(django101-z0e96VTa) : django-admin startproject <name of project> .

```
The dot(.) will place all the file inside the current directory and if you don't give it the dot it will make a subfolder which you may nor like 

After creating project the next thing to do is create an app using this command 

```
$ django-admin startapp <app name>
```

To  Launch the development server/project use this command:

```
$(django101-z0e96VTa) : python manage.py runserver
```

It will display :

***
*You have unapplied migrations; 
your project may not work properly until they are applied. 
Run 'python manage.py migrate' to apply them.*
***


**Migration** 

Migrations are Django's way of propagating changes you make to your models (adding a field, deleting a model, etc.) into your database schema. They're designed to be mostly automatic.
A migration is simply connecting to a database of some kind and in django case the database is sqlite and its trying to provision database so that we can set up user and permissions ,all sort of things.

When ever you see the display: *you have unapplied migration* simply  type this command to apply the migration 

```
$(django101-z0e96VTa) : python manage.py migrate
```


The migrate looks at the INSTALLED_APPS setting and creates any necessary database tables according to the database settings in your settings.py file and the database migrations.


**Running**

When all dependencies installed and configurations are set, run the application.

```
$(django101-z0e96VTa) :  python manage.py runserver
```

Access application by entering *http://127.0.0.1:8000/* or *http://localhost:8000/* url on browser.

Creating an admin user follow this [steps](https://docs.djangoproject.com/en/2.1/intro/tutorial02/#creating-an-admin-user). 

Access admin panel *http://127.0.0.1:8000/admin/* or *http://localhost:8000/admin/* url on browser.


**Testing**

*Note: Test cases are pending.*



**References**

* [Python](https://www.python.org)
* [django](https://www.djangoproject.com/)

