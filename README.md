# Experiment With Django Channels

This is a real-time web app that shows what time it is on the server.
In addition every visitor of the page can choose the background color of the page for that visitor and other connected visitors.

## Quickstart

1. Install redis:
    
    On Mac OS X run:
    
        $ brew install redis
        
    Start redis server:
    
        $ brew services start redis
        
    Check if redis is reachable:
    
        $ redis-cli ping
        PONG

2. Create and activate a virtual environment:

        $ virtualenv venv
        $ . venv/bin/activate

3. Download and extract or clone this project.

4. Install pip requirements into the virtual environment:
        
        (venv)$ pip install -r requirements.txt

5. Run the local webserver:

        (venv)$ python manage.py runserver

6. In another Terminal tab, run the management command that will send time to channels:

        (venv)$ python manage.py provide_time

7. Open http://127.0.0.1:8000 in multiple web browsers and enjoy.
