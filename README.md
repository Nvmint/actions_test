# sec-employment-api
### Initial setup
#### Download required tools
​
To begin working on Secondary Employment, you'll require certain tools.
​
1. Download and install [Python (version)](https://www.python.org/downloads/).
2. Download and install a code editor (the recommended one is [Visual Studio Code](https://code.visualstudio.com/)).
3. You will require a 1Password account to access the environment files. [Create one](https://1password.com/ibm/) if you don't have already.
​
#### Python libraries you'll need
​
Using the next command to add all the python modules you'll need to work and run the project (recomended)
```bash
pip install -r requirements.txt
```

The modules that should be install are:
- Django
- django-cors-headers
- django-environ
- psycopg2
- pylint
- pylint-django
- coverage 

#### Set up the project with git

1. Make sure you have git or an equivalent software (i.e. GitHub Desktop) installed on your computer.
2. Login with your enterprise IBM GitHub account or [connect with an SSH key](https://docs.github.com/en/enterprise-server@3.2/authentication/connecting-to-github-with-ssh) (recommended).
3. Clone this repository (SSH): `git@github.ibm.com:Secondary-Employment/sec-employment-api.git`

#### Add the environment file

1. Request access to the project's 1Password vault:
​
In order to obtain the env file required for this project please request access to the 1password vault to any of the following contacts.
​
- @ahtziri.fernandez1
- @Bernardo Elizondo
​
2. Open the vault of the project and copy the contents from the `.env` file.


### Runnning the project

To run the project locally use next the command for windows:
```bash
py manage.py runserver
```
And for Mac OS:
```bash
python3 manage.py runserver
```
#### Running unit testing and coverage

Run to execute all the unit tests that are in the project and to recibe the report of the coverage
```bash
coverage run manage.py test ; coverage report   
```