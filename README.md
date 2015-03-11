# django-mongodb-demo
Django with MongoDB

**Prerequisite**

Following packages required to setup mongodb with django , so download these things and install it.

django-nonrel https://github.com/django-nonrel/django<br>
djangotoolbox https://github.com/django-nonrel/djangotoolbox<br>
pymongo https://pypi.python.org/pypi/pymongo/<br>

Now create django project using django-admin and edit database settings in your settgings py file ,

```
DATABASES = {
   'default' : {
      'ENGINE' : 'django_mongodb_engine',
      'NAME' : 'my_database'
   }
}
```

Now start mongodb engine using mongod.exe  by providing database path in the comand.

```
C:\Program Files\MongoDB 2.6 Standard\bin>mongod.exe --dbpath D:\<path-to-project>\db
```
**Do not close or interupt this commnad window.**

Now just create simple view and manupulate database database with django's ORM.


