FROM nikolaik/python-nodejs:python3.6-nodejs12-alpine 
COPY . /todo-app
WORKDIR /todo-app/
RUN pip3 install -r requirements.txt
WORKDIR /todo-app/todo/frontend
RUN npm run build
EXPOSE 8000
WORKDIR /todo-app/todo
CMD [ "python","manage.py","runserver","--insecure","0.0.0.0:8000" ]