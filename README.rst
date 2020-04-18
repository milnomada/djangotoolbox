## Djangotoolbox

 - Updated few items in [fields.py] to allow compatibility with Django >= 1.10
 - Django Subclassing was removed. See [here](https://docs.djangoproject.com/en/dev/internals/deprecation/)
 - Using native `import_module`
 

Moved from original [Djangotoolbox] project


Djangotoolbox provides a common API for running Django on
non-relational/NoSQL databases (currently via Django-nonrel_).


```
In ``djangotoolbox.db`` you can find base classes for writing
non-relational DB backends. Read
`Writing a non-relational Django backend`_
for more information.

In ``djangotoolbox.fields`` you can find several common field
types for non-relational DB backends (``ListField``, ``SetField``,
``DictField``, ``RawField``, ``BlobField``).

The ``djangotoolbox.admin`` module provides admin overrides for
making ``django.contrib.auth`` work correctly in the admin UI.
Simply add ``'djangotoolbox'`` to ``INSTALLED_APPS`` **after**
``django.contrib.admin``. This will disable features that
require JOINs. If you still need permission handling you should
use the `nonrel permission backend`_.
```


### Django-nonrel
http://django-nonrel.org/

Writing a non-relational Django backend:  
http://www.allbuttonspressed.com/blog/django/2010/04/Writing-a-non-relational-Django-backend  

Nonrel permission backend:  
https://github.com/django-nonrel/django-permission-backend-nonrel
