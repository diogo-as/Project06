
# CatalogApp
This is a Catalog App with Google authentication runing on VM instance on Google Cloud Engine.
This app was developed for final project #06 of [Udacity](https://udacity.com "Udacity") FullStack nanodegree program.

## URL

   https://app.104.197.67.49.nip.io

## Environment

 - Python 2.7

 - Postgres

 - Nginx (config file of the app site config for reference:  nginx/default)
 
 - uWSGI (config file: [app.ini](https://github.com/diogo-as/Project06/blob/master/app.ini "app.ini"))
 
 -  Hosted at [Google Cloud Plataform](https://cloud.google.com "Google Cloud Plataform") (f1-micro (1 vCPUj, 0,6 GB RAM) )
  

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
	sudo cp /Project06/nginx/default /etc/nginx/sites-available

### - Install python requirements

Type `$ pip install -r requirements.txt`

### - Google API

Type `$ export GOOGLE_CLIENT_ID = "your client ID"`
Type `$ export GOOGLE_CLIENT_SECRET = "your client SECRET"`

You can use as variables on views.py too.

### Populate DB
To populate database for example.

Type `$ python populate.py`

## Access CatalogApp

In your browser visit **https://app.104.197.67.49.nip.io** to view the CatalogApp.  
You should be able to view all categories and itens.

To add, edit and delete categories and associated itens you need to login with Google authentication.

### API Json

Now type **https://app.104.197.67.49.nip.io/categories** on your browser to view all categories in json format.

Now type **https://app.104.197.67.49.nip.io/itens** on your browser to view all itens in json format.

## References
- [Udacity FullStack Nanodegree](https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd004 "Udacity FullStack Nanodegree")
- Google Login based on [Realpython.com](https://github.com/diogo-as/materials/tree/master/flask-google-login "Realpython.com")
- [Flask uswgi and nginx](https://www.digitalocean.com/community/tutorials/how-to-serve-flask-applications-with-uwsgi-and-nginx-on-ubuntu-16-04 "Flask uswgi and nginx")
- [UFW docs](https://help.ubuntu.com/community/UFW "UFW docs")
- [How to setup PostgresQL](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-16-04 "How to setup PostgresQL")
- [Virtual Environments](https://modwsgi.readthedocs.io/en/develop/user-guides/virtual-environments.html "Virtual Environments")
- [Flask uswgi and nginx](https://www.digitalocean.com/community/tutorials/how-to-serve-flask-applications-with-uwsgi-and-nginx-on-ubuntu-16-04 "Flask uswgi and nginx")
- Free HTTPs Cert from [Let´s Encrypt](https://letsencrypt.org/ "Let´s Encrypt")
- Free DNS name from [nip.io](https://nip.io/ "nip.io")


[1]: https://udacity.com "Udacity"
