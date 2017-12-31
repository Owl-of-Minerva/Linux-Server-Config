Catalog App
=============
-------------
###  Login Info
* IP Address: 52.14.207.135
* Port Number: 2200
* User: grader


###  Software Installed 
* apache2
* git
* libapache2-mod-wsgi
* libapache2-mod-wsgi
* postgresql
* postgresql-contrib
* python-flask
* python-flask-sqlalchemy
* python-psycopg2
* python-oauth2client

### Configuration Change
#### Configure SSH for Nre User
* Create .ssh dir and add public key info to authorized_keys file
* Set ssh file permissions
* Change the port number from 22 to 2200, remove root login, forbid password login by modifying the /etc/ssh/sshd_config
* Use ufw to change the firewall rule to allow only port 2200, 80 and 123

#### PostgreSQL
* Create user catalog
* Disable remote login by modifying /etc/postgresql/9.3/main/pg_hba.conf