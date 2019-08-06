
# CatalogApp
This is a Catalog App with Google authentication runing on VM instance on Google Cloud Engine.

## Environment

python 2.7
Postgres

### Config O.S
    sudo apt update
    sudo apt git
    sudo apt install git
    sudo apt-get install nginx nginx-extras
    sudo adduser grader
    sudo usermod -aG sudo grader
    su - grader
    sudo ufw status
    sudo ufw allow 2200
    sudo ufw allow 80
    sudo ufw allow https
    sudo ufw deny 22
    sudo ufw logging on
    sudo ufw allow ntp
    sudo ufw status
    sudo apt install postgresql
    sudo mkdir /Project06
    sudo git clone https://github.com/diogo-as/Project06.git

### - Install python requirements

Type `$ pip install -r requirements.txt`

### - Google API

Type `$ export GOOGLE_CLIENT_ID = "your client ID"`
Type `$ export GOOGLE_CLIENT_SECRET = "your client SECRET"`

You can use as variables on views.py too.
### Populate DB
To populate database for example.

Type `$ python populate.py`

## Run CatalogApp

<<<<<<< HEAD
Type **`$ python views.py`** to run the Flask web server. In your browser visit **http://127.0.0.1:5000** to view the CatalogApp.  
You should be able to view all categories and itens.
=======
Type **`$ python views.py`** to run the Flask web server. In your browser visit **https://127.0.0.1:5000** to view the CatalogApp.  
You should be able to view all categories and itens. 
>>>>>>> b211009d2a0df040f2135d6de26ce097055ede31

To add, edit and delete categories and associated itens you need to login with Google authentication.

### API Json

Now type **https://127.0.0.1:5000/categories** on your browser to view all categories in json format.

Now type **https://127.0.0.1:5000/itens** on your browser to view all itens in json format.
