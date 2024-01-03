GETTING-STARTED
======================================================
CREATE A VIRTUAL ENVIRONMENT:
======================================================
STEP1: CREATE A VIRTUAL ENVIRONMENT
py -m venv env
------------------------------------------------------
STEP2: IN TERMINAL(ADMIN)
Set-ExecutionPolicy unrestricted
------------------------------------------------------
STEP3: ACTIVATE VIRTUAL ENVIRONMENT
.\env\Scripts\activate.ps1
------------------------------------------------------
STEP4: INSTALL FLASK IN ENVIRONMENT
pip install flask
------------------------------------------------------
STEP5: PASTE MINIMAL FLASK APP (inside app.py file)
from flask import Flask
app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello, World!'
=========================================================================================================
===================================
TO CREATE A DATABASE FILE (todo.db)
===================================
On your terminal python:-
>>from app import app, db
>>app.app_context().push()
>>db.create_all()
>>exit()