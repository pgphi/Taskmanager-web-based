***
Version 1.0
Author: Philipp Ganster
About this Project:With this web-based application users can create tasks, update and delete them.
The taskmanager shows when the task was created.
Link: https://mypersonaltaskmanager.herokuapp.com/
***


### Personal Workflow:

- Setup & Workflow
- Get a basic app runing
- Templates and static content 
- Setting up and using database (SQLite)
- Create a basic CRUD app
- Deploy to Heroku

#### Installing virtualenvironment for easier collaboration (packages not installed globally)
1) pip3 install virtualenv
3) virtualenv env
4) source env/bin/activate
5) (env) *now in virtualenvironment - install everything we need*

> Go to command palette using CTRL + Shift + P and select python: select interpreter and choose approprioate virtualenv

### For Deployment on Heroku Cloud:
1) >>> heroku login
2) install dependency --> >>> pip3 install gunicorn
3) freeze requirements --> >>> pip3 freeze > requirements.txt
4) initialize empty git repository --> >>> git init
4.2) add everything into this directory --> >>> git add .
4.3) commit everything to repository --> >>> git commit -m "Initialize App"
5) create heroku app --> >>>heroku create *appname*
6) see where app is being pushed --> >>> git remote -v
7) create Procfile to tell heroku what to do with all files --> >>> touch Procfile
7.1) add Procfile to repository --> >>> git add .
7.2) commit added file --> >>> git commit -m "Procfile Added"
7) push everything to heroku --> >>> git push heroku master

> >>> heroku info -s --> For further information i.e. web_url etc.
> >>> heroku logs --tail --app your_app_name --> for viewing errors


### In General in regard to Deployment:

####  If changes had to be made: 
1) *Make changes on application*
2) >>> git add .
3) >>> git commit -m "*description of changes*"
4) >>> git push heroku master
