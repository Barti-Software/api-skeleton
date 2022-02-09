## Setup
1. After cloning this repository, cd into it.
2. Set up virtual environment via ```python3 -m venv env``` 
3. Activate the virtual environment via ```source env/bin/activate```
4. If it's properly set up, ```which python``` should point to a python under api-skeleton/env.
5. Install dependencies via ```pip install -r requirements.txt```

## Starting local flask server
Under api-skeleton/src, run ```flask run --host=0.0.0.0 -p 8000```

By default, Flask runs with port 5000, but some MacOS services now listen on that port.

## Running unit tests
All the tests can be run via ```pytest``` under api-skeleton directory.

## Code Structure
This is meant to be barebones.

* src/app.py contains the code for setting up the flask app.
* src/endpoints.py contains all the code for enpoints.
* src/models.py contains all the database model definitions.
* src/extensions.py sets up the extensions (https://flask.palletsprojects.com/en/2.0.x/extensions/)