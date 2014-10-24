Projectname
===========

This README documents whatever steps are necessary to get your application up and running.

## Install ##

**Create and activate your virtual environment**
    
    $ virtualenv [projectenv]
    $ cd [projectenv]
    $ source bin/activate

**Install Node**

    This process varies per platform.

**Install Less**

    $ npm install less

**Clone repository:**
    
    $ (projectenv) git clone [repository_location]/projectname.git

**Install dependencies:**

    $ (projectenv) cd [projectname]
    $ (projectenv) pip install -r requirements.txt

**Update base.py settings**

    Add "projectname" to the list of installed apps

    INSTALLED_APPS = ''

**Create local.py**
    
    $ (projectenv) cp projectname/settings/local_example.py projectname/settings/local.py

**Set environment variable for local settings into terminal:**

    $ (projectenv) export DJANGO_SETTINGS_MODULE=projectname.settings.local

**Update local.py settings**

    Follow the URL and generate a secret key for your project

    SECRET_KEY = ''

**Test your server:**
    
    $ (projectenv) python manage.py runserver 0.0.0.0:8000
    
    You should see the Django.. It worked! message when viewing http://localhost:8000


## Working ##

**Activate your virtualenv:**
    
    $ cd projectenv
    $ source bin/activate
    
**Run server:**
    
    $ cd projectname
    $ (projectenv) python manage.py runserver 0.0.0.0:8000
