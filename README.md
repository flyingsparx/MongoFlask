MongoFlask
=================

Companion code for this 
[blog post](http://www.willwebberley.net/#post/2013-02-21), though this walkthrough is more comprehensive.

Provides a simple example of using the Flask Python web framework using MongoDB.

1.
===

**This step covers**:
* Getting a working installation of [Python](http://www.python.org/)
* Installing [MongoDB](http://www.mongodb.org/)

Python and MongoDB can be downloaded from their respecitve websites, or installed through your OS distribution's package manager (if this is supported).

For example, in Arch Linux:
```
# pacman -S python2 python2-distribute
```
to install Python v2.* and some tools (including easy_install), and then:
```
# pacman -S mongodb 
```
to install MongoDB.


2.
===

Install Flask and MongoAlchemy (which is useful for handling the database). Use easy_install or pip, e.g.:
```
# easy_install flask
# easy_install Flask-MongoAlchemy
```

3.
===

Start the database server as a user. First make a directory to store the database and then run it:
```
$ mkdir data/db
$ mongodb --dbpath data/db
```


4.
=== 

Start your application. Either use the example in this repository, or create your own.
Once the development server is running your application, visit [localhost:5000](http://localhost:5000) to see it working.


FILE AND DIRECTORY INFO:
==========================

* *application.py*
    * Main application code
    * Handles routing for different URLs
    * Contains examples for:
        * Sessions (logging in and out)
        * Data storage (storing and accessing user data)
        * File uploads
        * Handling POST/GET requests differently
        * Routing error pages
    
* *templates/*
    * The HTML source files for the application
