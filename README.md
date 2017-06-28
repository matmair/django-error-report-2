  ------------------
  django-error-report
  ------------------

View all Django Error detail in Django Admin.

Error-report save Django error traceback and details which would be the same beautiful exception page that Django displays when debugging is enabled and saves it to the database so you
can view it later.

It's simple alternative to django-sentry which is a paid option to see error detail.

You can create issues for feature you want in django-error-report in future.

Features
========

-   A simple user interface for browsing error records in the database.

Requirements
============
- Python 2.7
- Django > 1.6

Installation
============

1. To install, simply run:

    > pip install django-error-report

2.  Add `error_report` to your `INSTALLED_APPS` setting.
3.  Run `manage.py migrate` to create the database tables.

Configuration
=============

Required settings for Django-error-report should be added in settings.py file like this

    ERROR_DETAIL_SETTINGS = {
        "CONFIGURATION_OPTION": VALUE
    }
    
Available configuration options are below
- ERROR_DETAIL_ENABLE: Should Log error detail or not (True/False)
- ERROR_DETAIL_HEIGHT: Height of Iframe in admin (in pixels) 

