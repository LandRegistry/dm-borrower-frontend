# dm-borrower-frontend

The Borrower Frontend provides a service for a Borrower to view and sign their
mortgage deeds online.

## Contents
- [Usage](#usage)
- [Install The Requirements](#install-the-requirements)
- [Run The App](#run-the-app)
- [Run The Unit Tests](#run-the-unit-tests)

## Usage
```
GET     /health                         -- renders standard Gov UK template
GET     /searchdeed                     -- borrower views deed landing page
POST    /searchdeed/search              -- POST search for deed (deed reference is in the request body)
```

## Install the requirements

Install the requirements
```
pip install -r requirements.txt
```

Optional: export variable for deed-api
```
> export DEED_API_BASE_HOST=http://localhost:8000
```

> default is localhost:9030


## Run the app
```
python run.py runserver -host 0.0.0.0
```
> optional ```--port 9000``` where 9000 is the number of a port you can supply to start the server on.


## Run the Unit Tests

Install the requirements
```
pip install -r requirements_test.txt
```

Run unit tests and provide coverage report

```
source test.sh
```
