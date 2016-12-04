# lab-apps
In the future, I would like to create application that Predict stock market price especially NIKKEI 225.  
At the beginning, I have been implementing Sample Interface.  
Sample Interface has referenced [Django Girls Tutorial](https://www.gitbook.com/book/djangogirls/djangogirls-tutorial/details).  


## Cloud9 Setup
This project has been creating by [Cloud9](https://c9.io/).  

#### Python Setup
> ~/workspace $ **sudo mv /usr/bin/python /usr/bin/python2**  
> ~/workspace $ **sudo rm /usr/bin/python3**  
> ~/workspace $ **sudo ln -s /usr/bin/python3.5 /usr/bin/python3**  
> ~/workspace $ **sudo ln -s /usr/bin/python3 /usr/bin/python**  
  
#### Virtual Environment Setup  
> ~/workspace $ **cd ~**  
> ~ $ **python -m venv np-env**  
> ~ $ **cd workspace/**  
> ~/workspace $ **source ~/np-env/bin/activate**  
  
#### pip upgrade & Django install
> ~/workspace $ **pip install --upgrade pip**  
> ~/workspace $ **pip install --upgrade setuptools**  
> ~/workspace $ **pip install django dj-database-url gunicorn whitenoise**

#### Setup Postgres
> ~/workspace $ **sudo service postgresql start**
> ~/workspace $p **psql**  
> \# **CREATE USER <USER-NAME> WITH PASSWORD \'<PASSWORD>\' CREATEDB\;**  
> \# **CREATE DATABASE <DB-NAME> OWNER <USER-NAME>\;**  
> \# **\\q**  
> ~/workspace $ **pip install psycopg2**  
> ~/workspace $ **python manage.py migrate**  
> ~/workspace $ **python manage.py createsuperuser --username <USER-NAME2>**

## References
+ [Cloud9](https://c9.io/) - Cloud IDE
+ [Django Girls Tutorial](https://www.gitbook.com/book/djangogirls/djangogirls-tutorial/details) - Django Tutorial  
