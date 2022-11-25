# profiles-rest-api

First we need to create a virtual environment. 
1. Clone an empty git repo
    git clone https://github.com/a-kumar5/profiles-rest-api.git 
2. New repo will be pulled to your local(In this case "profiles-rest-api" )
3. Create a virtual environment using 
    python -m venv ~/env
4. Once virtual environment is created, we need to activate the virtual environment.
    source ~/env/bin/activate
5. To deactivate the virtual environment.
    deactivate

Now we will install the required dependency for django(python virtual environment should be active).
1. Change to profiels-rest-api directory(cd profiles-rest-api)
2. Create a requirements.txt file and list out all the python packages required to install and save file.
    django==2.2
    djangorestframework=3.9.2
3. Install the packages listed in requirements.txt using pip.
    pip install -r requirements.txt 

Creating a django project.
1. Use command (django-admin.py startproject profiles_project .).
2. Above command will create a django project with name profiles_project. Profiles_project consists of init, settings, urls, wsgi python files. Also, the above command will create a manage.py file which is eventually used for different django functions including creating apps(apis inside project).
3. To create and api or apps. Use command python manage.py startapp profiles_api. This will create a new app with name profiles_api having it's own init, admin, apps, models, tests, views files by default.

Enabling the profiles_api(app) in profiles_project(project) in django.
1. Open the profiles_project that is the root project of our django project.
2. Inside the settings.py file under the installed apps include "rest_framework","profiles_api" as seen in commit.

Testing and commiting our changes
1. Using the django development web server, we can test and run the project.
2. First need to migrate the app. Using python manage.py migrate
3. Run the server using python manage.py runserver 