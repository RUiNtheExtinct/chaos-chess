[![Python 3.6](https://img.shields.io/badge/python-3.6-yellow.svg)](https://www.python.org/downloads/release/python-360/)
![Django 3.0](https://img.shields.io/badge/Django-3.0-green.svg)
[![license](https://img.shields.io/github/license/DAVFoundation/captain-n3m0.svg?style=flat-square)]()
# Chess-Gang

ASGI Django Server to play Chess in real-time using Django Channels and Redis.

Video Link : https://youtu.be/1vTLLf82KwE


## `master branch`
Master branch is for developement Django server to be run on local system (Windows). Follow these steps to use:  
1. Install all the dependencies by running `pipenv install` (install pipenv first)  
2. Ensure you have Redis running on `port #6379` for it to work correctly. This can be achieved using Docker (on Windows) by running the command `docker run -p 6379:6379 -d redis:5`  
3. Finally run server using `python manage.py runserver`  

## `prod branch`
Prod branch was made keeping in mind the end result of deployment on Heroku using the free-tier. You can view the version that I have deployed [here](https://chess-gang.herokuapp.com/). Follow these steps to deploy:  
1. Clone this branch and create a new application on Heroku  
2. Add the Heroku Redis addon to the application (free-tier available)  
3. Link the cloned repo to your application and deploy
