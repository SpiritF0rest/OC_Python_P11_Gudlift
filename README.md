# :shield: Gudlift-registration :shield:

This is a proof of concept (POC) project to show a light-weight version of our competition booking platform. The aim is the keep things as light as possible, and use feedback from the users to iterate.

***
## Table of Contents
1. [General Info](#general-info)
2. [Technologies](#technologies)
3. [Installation](#installation)
4. [Tests](#tests)

### :newspaper: General Info :newspaper:
***
This is an OpenClassrooms student Flask project. 
The objective is to correct the issues of the initial project and add tests to consolidate the application.

### :briefcase: Technologies :briefcase:
*** 
- [Flask](https://pypi.org/project/Flask/2.3.2/): Version ^2.3.2
- [Python](https://www.python.org/): Version ^3.10
- [Poetry](https://pypi.org/project/poetry/1.5.1/): Version 1.5.1
- [Pytest](https://pypi.org/project/pytest/): Version ^7.4.0
- [Flake8](https://pypi.org/project/flake8/): Version ^6.1.0
- [Coverage](https://pypi.org/project/coverage/): Version ^7.3.1

### :wrench: Installation :wrench:
***
In your directory for the project:

Clone repository from:
- [Gudlift](https://github.com/SpiritF0rest/OC_Python_P11_Gudlift)

#### :wrench: Virtual environment creation and use :wrench:

```
In terminal from cloned folder :
$ python3 -m venv env

To active the virtual environment:
$ source env/bin/activate

To install modules:
$ poetry install

To set Flask environmental variable:
$ export FLASK_APP=server.py

To run server:
$ python3 -m flask run

To deactive the virtual environment: 
$ deactivate
```

 Flask specification : check [here](https://flask.palletsprojects.com/en/1.1.x/quickstart/#a-minimal-application) for more details


#### :wrench: Notes :wrench:

The app is powered by [JSON files](https://www.tutorialspoint.com/json/json_quick_guide.htm). This is to get around having a DB until we actually need one. The main ones are:
     
* competitions.json - list of competitions
* clubs.json - list of clubs with relevant information. You can look here to see what email addresses the app will accept for login.

### :newspaper: Tests :newspaper:

```
To test:
$ pytest

To generate Flake 8 report:
$ flake8

To see coverage:
$ coverage run -m pytest
$ coverage report
$ coverage html
```

:snake: Enjoy :snake:
