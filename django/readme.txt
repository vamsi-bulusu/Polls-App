django-admin startproject mysite --->cmd for starting new project(mysite)
python manage.py startapp polls  --->cmd to create new app(polls)
*views can called by mapping app url to root project url*
python manage.py runserver       --->cmd to start wsgi server
<------------------------------------------------------------------------>
Database setup--->python manage.py migrate--->create tables
<------------------------------------------------------------------------>
Creating models--->Now we’ll define our models – essentially, our database layout, with additional metadata.
<------------------------------------------------------------------------>
Activating models--->That small bit of model code gives Django a lot of information. With it, Django is able to:

Create a database schema (CREATE TABLE statements) for this app.
Create a Python database-access API for accessing Question and Choice objects.

*include appconfig to our project settings
*save changes by running this cmd--->python manage.py makemigrations polls
<------------------------------------------------------------------------>
python manage.py sqlmigrate polls 0001--->cmd to view sql queries
python manage.py migrate-->save changes to the db
<------------------------------------------------------------------------>
Django-API
to open --->python manage.py shell(manage.py sets environ to current proj direct)
django api provides methods to work or operate on db such as save,delete,filter etc.
<------------------------------------------------------------------------>
Introducing django admin
creating an admin user ---> python manage.py createsuperuser
*add application to adminsite by registering-->admin.site.register(Question)