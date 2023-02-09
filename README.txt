Use Python 3.6.

Application
===========
Installation
------------
- install packets: pip install -r requirements.txt
- create "logs" directory near app.py file

Execution
---------
"python app.py" - the app will start on port 5000

Functionality
-------------
The app has two endpoints:
- http://localhost:5000/     - display a counter
- http://localhost:5000/logs - display the logs of "/" endpoint invocation

Third-party dependencies
------------------------
It is important that application depends on a Redis database. The Redis instance has to be available by redis:6379.



Automated tests
===============
Installation
------------
pip install -r test-requirements.txt

Execution
---------
pytest test_app.py --url http://localhost:5000
                         ^^^^^^^^^^^^^^^^^^^^^
                         URL to the app

