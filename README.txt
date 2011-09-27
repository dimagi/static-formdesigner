A totally static version of the compiled Dimagi GWT Form Designer.

This project serves the Form Designer locally, in case you don't 
have an out-of-the-box file serving solution on your development
machine.

This does NOT serve the latest version of Form Designer, only 
whatever is currently bundled with this code. For the latest
form designer, download the files on http://build.dimagi.com:250

Copy localsettings.py.example to localsettings.py and edit accordingly


After doing:
git submodule init
git submodule update
./manage.py syncdb
./manage.py runserver

you should be able to access Vellum (fdalpha) at
http://localhost:8000/static/fdalpha/index.html

and run all unit tests at
http://localhost:8000/static/fdalpha/test.html


Requires:

Django 1.3 or higher.
For older versions of Django, use django-staticfiles instead of the 
builtin contrib application.