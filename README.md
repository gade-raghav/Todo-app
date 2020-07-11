# To-do

To-do is a simple django application which helps us to keep a track of everyday tasks.
This application has been written for learning purpose and is not very productive.

Backend  : written using python-django framework
Frontend : written using reactjs

## Requirements
* docker (not necessary)
* [python-3.6](https://www.python.org/downloads/release/python-3611/) 
* node-12.16.1>
Make sure you have the above requirements satisified.


# Usage
There are multiple ways to run this application.
First step is to clone the repository
```bash
git clone https://github.com/gadeRaghav/todo-app.git
```

##1. Run from ubuntu terminal as localhost


Switch to to-do directory and install the requirements from requirements.txt.(django, djangorestframework, django-cors-headers)
```bash
cd to-do/
pip3 install -r requirements.txt
```
To set-up frontend switch to to-do/frontend direcotry and run the following command.(It correctly bundles React in production mode and optimizes the build for the best performance.)
```bash
cd to-do/todo/frontend
npm run build
```
Finally switch to to-do/todo directory and run the server
```bash
cd to-do/todo
python3.6 manage.py runserver --insecure 0.0.0.0:8000
```
and access the app from [http://localhost:8000](http://localhost:8000) !!


Instead of going through the above steps, you can simply run the app in docker container
##2. Run using docker

Switch to to-do directory and run docker build
```bash
docker build --tag <tag-name> . 
```
Run docker image
```bash
docker run --publish 8000:8000 --name <container-name> --detach <tag-name>
```
and access the app from [http://localhost:8000](http://localhost:8000) !!



#Acknowledgement

Thanks to [nikolaik](https://hub.docker.com/u/nikolaik) for python-nodejs docker image.











