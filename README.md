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
